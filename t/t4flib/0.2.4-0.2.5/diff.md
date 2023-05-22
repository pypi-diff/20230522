# Comparing `tmp/t4flib-0.2.4-py2.py3-none-any.whl.zip` & `tmp/t4flib-0.2.5-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 10810 bytes, number of entries: 12
+Zip file size: 11061 bytes, number of entries: 12
 -rw-rw-r--  2.0 unx        0 b- defN 23-May-11 18:20 t4flib/__init__.py
 -rw-rw-r--  2.0 unx      892 b- defN 23-May-17 17:25 t4flib/config.py
 -rw-rw-r--  2.0 unx      971 b- defN 23-May-17 15:49 t4flib/data_helper.py
 -rw-rw-r--  2.0 unx     6145 b- defN 23-May-17 15:49 t4flib/file_helper.py
--rw-rw-r--  2.0 unx     4758 b- defN 23-May-17 18:39 t4flib/filetransfer_helper.py
+-rw-rw-r--  2.0 unx     5700 b- defN 23-May-22 13:49 t4flib/filetransfer_helper.py
 -rw-rw-r--  2.0 unx     7420 b- defN 23-May-17 15:49 t4flib/functional_helper.py
 -rw-rw-r--  2.0 unx     3235 b- defN 23-May-17 15:49 t4flib/gcloud_helper.py
 -rw-rw-r--  2.0 unx      876 b- defN 23-May-17 15:14 t4flib/log_helper.py
--rw-rw-r--  2.0 unx     1747 b- defN 23-May-17 18:51 t4flib-0.2.4.dist-info/METADATA
--rw-rw-r--  2.0 unx      110 b- defN 23-May-17 18:51 t4flib-0.2.4.dist-info/WHEEL
--rw-rw-r--  2.0 unx        7 b- defN 23-May-17 18:51 t4flib-0.2.4.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      919 b- defN 23-May-17 18:51 t4flib-0.2.4.dist-info/RECORD
-12 files, 27080 bytes uncompressed, 9278 bytes compressed:  65.7%
+-rw-rw-r--  2.0 unx     1747 b- defN 23-May-22 14:02 t4flib-0.2.5.dist-info/METADATA
+-rw-rw-r--  2.0 unx      110 b- defN 23-May-22 14:02 t4flib-0.2.5.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        7 b- defN 23-May-22 14:02 t4flib-0.2.5.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      919 b- defN 23-May-22 14:02 t4flib-0.2.5.dist-info/RECORD
+12 files, 28022 bytes uncompressed, 9529 bytes compressed:  66.0%
```

## zipnote {}

```diff
@@ -18,20 +18,20 @@
 
 Filename: t4flib/gcloud_helper.py
 Comment: 
 
 Filename: t4flib/log_helper.py
 Comment: 
 
-Filename: t4flib-0.2.4.dist-info/METADATA
+Filename: t4flib-0.2.5.dist-info/METADATA
 Comment: 
 
-Filename: t4flib-0.2.4.dist-info/WHEEL
+Filename: t4flib-0.2.5.dist-info/WHEEL
 Comment: 
 
-Filename: t4flib-0.2.4.dist-info/top_level.txt
+Filename: t4flib-0.2.5.dist-info/top_level.txt
 Comment: 
 
-Filename: t4flib-0.2.4.dist-info/RECORD
+Filename: t4flib-0.2.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## t4flib/filetransfer_helper.py

```diff
@@ -1,19 +1,21 @@
+from .config import FT_PARAM_FILEPATH, FT_GRAVITEE_KEY, FT_GRAVITEE_URL
+from .log_helper import logger
+from .file_helper import get_all_file_by_filemask
+
 import requests
 from requests.adapters import HTTPAdapter
 from urllib3.util.retry import Retry
 import json
 import csv
 import os
-from .config import FT_PARAM_FILEPATH, FT_GRAVITEE_KEY, FT_GRAVITEE_URL
-from .log_helper import logger
-from .file_helper import get_all_file_by_filemask
 import shutil
-import time
 import urllib3
+import logging
+import datetime
 
 
 class ft_flow:
     flow_name = ''
     server = ''
     ft_key = ''
     filemask = ''
@@ -80,33 +82,46 @@
         return flows
 
     except Exception as e:
         logger('ERROR', f'{str(e)}')
 
 
 def send_file_by_filetransfer(flow_name):
-    logger('INFO', f'Envoi dans filetransfer du flux {flow_name}')
+    logger('INFO', f'Envoi dans filetransfer du flux {flow_name} dans le fichier {FT_PARAM_FILEPATH}')
     urllib3.disable_warnings(urllib3.exceptions.InsecureRequestWarning)
     ft_flows_to_send = get_flow_attributes_in_file(flow_name)
+    execution_timestamp=datetime.datetime.now().strftime('%Y-%m-%d')
 
     if len(ft_flows_to_send) > 0:
+
         session = requests.Session()
         retry = Retry(total=5, backoff_factor=0.1, status_forcelist=[401, 403, 404, 429, 500, 502, 503, 504])
         adapter = HTTPAdapter(max_retries=retry)
         session.mount('http://', adapter)
         session.mount('https://', adapter)
 
         headers = {
             "Content-type": "application/json",
             "X-Gravitee-api-Key": FT_GRAVITEE_KEY
         }
 
         for ft_flow_to_send in ft_flows_to_send:
 
+            logging.basicConfig(filename=os.path.join(ft_flow_to_send.path_to_log, f'{flow_name}_{execution_timestamp}.log'), format='%(name)s - %(asctime)s - %(levelname)s - %(message)s', force=True)
+            log_f=logging.getLogger() 
+            log_f.setLevel(logging.DEBUG) 
+
             logger('DEBUG', f'{ft_flow_to_send.path_to_get_file}/{ft_flow_to_send.filemask}')
+            log_f.debug(f'{ft_flow_to_send.path_to_get_file}/{ft_flow_to_send.filemask}')
+
+            files = get_all_file_by_filemask(ft_flow_to_send.path_to_get_file, ft_flow_to_send.filemask)
+            if len(files) == 0:
+                log_f.warning('Pas de fichier trouvé')
+                continue
+
             for file in get_all_file_by_filemask(ft_flow_to_send.path_to_get_file, ft_flow_to_send.filemask):
 
                 shutil.copy(str(file.absolute()), ft_flow_to_send.path_out)
 
                 body_request = json.dumps({
                     "flow": ft_flow_to_send.flow_name,
                     "userId": ft_flow_to_send.server,
@@ -115,16 +130,19 @@
                 })
 
                 try:
                     response = requests.post(FT_GRAVITEE_URL, headers=headers, data=body_request, verify=False)
                     ret = response.status_code
                 except requests.exceptions.RequestException as e:
                     logger("Error", f"{e}")
+                    log_f.error(str(e))
                     ret = None
 
                 if ret in [202, 200]:
 
                     logger("INFO", f"Le flux {flow_name} contenant le fichier {str(file)} est parti")
+                    log_f.info(f"Le flux {flow_name} contenant le fichier {str(file)} est parti")
                 else:
 
                     logger('ERROR', f"Un code erreur API : {ret} a eu lieu")
                     logger('ERROR', f"Erreur lors de l'appel à l'API statut => {ret}")
+                    log_f.error(f"Erreur lors de l'appel à l'API statut => {ret}")
```

## Comparing `t4flib-0.2.4.dist-info/METADATA` & `t4flib-0.2.5.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: t4flib
-Version: 0.2.4
+Version: 0.2.5
 Summary: Librairie de fonction utiles pour T4F
 Home-page: http://gitlab.dev.fr.auchan.com/tech4finance/t4flib.git
 Author: Corentin DEVROUETE
 Author-email: cdevrouete@advanced-schema.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

## Comparing `t4flib-0.2.4.dist-info/RECORD` & `t4flib-0.2.5.dist-info/RECORD`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 t4flib/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 t4flib/config.py,sha256=fHt2THXtajPzzV_gnHPZNVmez09ODLfIFrt4cTXgZsE,892
 t4flib/data_helper.py,sha256=SdKdv2U1EXtHJcfEff_I8zIlMWv56-xLZqczAw4kOUU,971
 t4flib/file_helper.py,sha256=NYIgOrA1iJBUcodtaRlDIsIHoivonLme4PmFZB1nQLw,6145
-t4flib/filetransfer_helper.py,sha256=WSZtS7WyMnDAxB_LEI7_nJDjfSaOd9RjYnAiC4c5-rA,4758
+t4flib/filetransfer_helper.py,sha256=8dL9dqJ_Kgory2nQ2Hoexv2Xw1IqBFFneEr-I7tS714,5700
 t4flib/functional_helper.py,sha256=CfbwrMufVRwCQNg9us9tujS3oeCmxql18vmo7B5lUAI,7420
 t4flib/gcloud_helper.py,sha256=sy5EpA2iVlcNlveP77N3iUCERNZXabSVOOcz8rifO6I,3235
 t4flib/log_helper.py,sha256=pu_y3m7iHWpkgYnxLYAlQjWjqknMGDcCDjHV6w4YYDc,876
-t4flib-0.2.4.dist-info/METADATA,sha256=v7Anc7QLrGH5s1gT8Nf8LjKXy4FU8txWdVO1RX0CdgU,1747
-t4flib-0.2.4.dist-info/WHEEL,sha256=a-zpFRIJzOq5QfuhBzbhiA1eHTzNCJn8OdRvhdNX0Rk,110
-t4flib-0.2.4.dist-info/top_level.txt,sha256=-05r3tdNDBMHneiATbWVqDQI7djLF9N83J6mAMcxbp8,7
-t4flib-0.2.4.dist-info/RECORD,,
+t4flib-0.2.5.dist-info/METADATA,sha256=pPB8jH81zrCNkX0-KH_B0pgQttcePVNTY4YWp517uH8,1747
+t4flib-0.2.5.dist-info/WHEEL,sha256=a-zpFRIJzOq5QfuhBzbhiA1eHTzNCJn8OdRvhdNX0Rk,110
+t4flib-0.2.5.dist-info/top_level.txt,sha256=-05r3tdNDBMHneiATbWVqDQI7djLF9N83J6mAMcxbp8,7
+t4flib-0.2.5.dist-info/RECORD,,
```

