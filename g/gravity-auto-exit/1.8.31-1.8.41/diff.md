# Comparing `tmp/gravity_auto_exit-1.8.31-py3-none-any.whl.zip` & `tmp/gravity_auto_exit-1.8.41-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 5904 bytes, number of entries: 11
+Zip file size: 6179 bytes, number of entries: 11
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Feb-03 11:23 gravity_auto_exit/__init__.py
 -rw-rw-rw-  2.0 fat      978 b- defN 22-Nov-06 04:54 gravity_auto_exit/logger.py
--rw-rw-rw-  2.0 fat     7553 b- defN 23-May-18 05:51 gravity_auto_exit/main.py
--rw-rw-rw-  2.0 fat      172 b- defN 23-Apr-27 06:33 gravity_auto_exit/mixins.py
+-rw-rw-rw-  2.0 fat     7786 b- defN 23-May-22 10:47 gravity_auto_exit/main.py
+-rw-rw-rw-  2.0 fat      654 b- defN 23-May-18 11:53 gravity_auto_exit/mixins.py
 -rw-rw-rw-  2.0 fat      327 b- defN 22-Nov-06 04:14 gravity_auto_exit/settings.py
 -rw-rw-rw-  2.0 fat        0 b- defN 22-Nov-06 04:12 gravity_auto_exit/logs/__init__.py
--rw-rw-rw-  2.0 fat     1091 b- defN 23-May-18 06:06 gravity_auto_exit-1.8.31.dist-info/LICENSE
--rw-rw-rw-  2.0 fat      409 b- defN 23-May-18 06:06 gravity_auto_exit-1.8.31.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-May-18 06:06 gravity_auto_exit-1.8.31.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       18 b- defN 23-May-18 06:06 gravity_auto_exit-1.8.31.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      944 b- defN 23-May-18 06:06 gravity_auto_exit-1.8.31.dist-info/RECORD
-11 files, 11584 bytes uncompressed, 4276 bytes compressed:  63.1%
+-rw-rw-rw-  2.0 fat     1091 b- defN 23-May-22 10:48 gravity_auto_exit-1.8.41.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat      409 b- defN 23-May-22 10:48 gravity_auto_exit-1.8.41.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-May-22 10:48 gravity_auto_exit-1.8.41.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       18 b- defN 23-May-22 10:48 gravity_auto_exit-1.8.41.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      944 b- defN 23-May-22 10:48 gravity_auto_exit-1.8.41.dist-info/RECORD
+11 files, 12299 bytes uncompressed, 4551 bytes compressed:  63.0%
```

## zipnote {}

```diff
@@ -12,23 +12,23 @@
 
 Filename: gravity_auto_exit/settings.py
 Comment: 
 
 Filename: gravity_auto_exit/logs/__init__.py
 Comment: 
 
-Filename: gravity_auto_exit-1.8.31.dist-info/LICENSE
+Filename: gravity_auto_exit-1.8.41.dist-info/LICENSE
 Comment: 
 
-Filename: gravity_auto_exit-1.8.31.dist-info/METADATA
+Filename: gravity_auto_exit-1.8.41.dist-info/METADATA
 Comment: 
 
-Filename: gravity_auto_exit-1.8.31.dist-info/WHEEL
+Filename: gravity_auto_exit-1.8.41.dist-info/WHEEL
 Comment: 
 
-Filename: gravity_auto_exit-1.8.31.dist-info/top_level.txt
+Filename: gravity_auto_exit-1.8.41.dist-info/top_level.txt
 Comment: 
 
-Filename: gravity_auto_exit-1.8.31.dist-info/RECORD
+Filename: gravity_auto_exit-1.8.41.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## gravity_auto_exit/main.py

```diff
@@ -2,20 +2,21 @@
 import os
 import threading
 import time
 import uuid
 from cad.main import CAD
 from whikoperator.main import Wpicoperator
 import requests
+from gravity_auto_exit import mixins
 from gravity_auto_exit.logger import logger
 from neurocore_worker.main import NeuroCoreWorker
 from qodex_recognition.main import MailNumberRecognitionRus
 
 
-class AutoExit:
+class AutoExit(mixins.ImgCutter):
     def __init__(self, cam_host, cam_login, cam_password,
                  neurocore_login, neurocore_password,
                  auth_method='Digest', engine_callback=None,
                  debug=False, failed_callback=None,
                  resize_photo: tuple = False, cam_port=80,
                  catch_event='Line Crossing',
                  simple_callback_func=None,
@@ -36,29 +37,31 @@
         cam_ip = cam_host.replace('http://', '')
         cam_ip = f"{cam_ip}:{cam_port}"
         if not logger:
             logger.getLogger(type(self).__name__)
         else:
             logger.name = type(self).__name__
         self.active = True
-        self.resize_photo = resize_photo
+        if resize_photo:
+            self.size = resize_photo
         self.cam = Wpicoperator(
             cam_ip=cam_ip,
             cam_login=cam_login,
             cam_pass=cam_password,
             auth_method=auth_method)
         self.callback_request_url = None
         self.debug = debug
         self.last_take = datetime.datetime.now()
         self.failed_callback = failed_callback
         self.engine_callback = engine_callback
         self.wait_started = False
         self.cycle_started = False
         logger.debug('AUTO_EXIT has started successfully')
 
+
     def set_active(self, activity_bool: bool):
         self.active = activity_bool
 
     def set_can_wait_others(self, boolean: bool):
         self.can_wait_others = boolean
 
     def start(self):
@@ -79,15 +82,15 @@
             return
         if self.engine and not self.engine.status_ready:
             logger.debug("Engine is not ready!")
             return
         logger.debug(f'Sleeping before: {self.sleep_before}')
         time.sleep(self.sleep_before)
         logger.debug("Recognise cycle has been started")
-        for i in range(3):
+        for i in range(5):
             if self.engine and not self.engine.status_ready:
                 logger.info("Cancel cycle for engine is not ready")
                 return
             logger.debug(f"Recognise cycle {i} of 5")
             time.sleep(i + 0.2)
             if not self.active:
                 self.active = True
@@ -133,14 +136,17 @@
                       params={'number': number})
 
     def try_recognise_plate(self):
         logger.debug(f'Taking photo...')
         photo = self.cam.take_shot()
         if not photo:
             return photo
+        if self.size:
+            photo = self.cut_photo(photo)
+        return
         result = self.get_car_number(photo)
         result = self._recognise(photo)
         return result
 
     def _recognise(self, photo):
         return self.neurocore_worker.get_car_number(photo)
 
@@ -193,18 +199,20 @@
     inst = CADRecogniseMail(  #
         #'http://192.168.60.107',
          #'http://172.16.6.176',
         "http://127.0.0.1",
         'admin',
         'Assa+123',
         debug=True,
-        #        cam_port=80,
+        # left, upper, right, lower
+        resize_photo=(100, 100, 1200, 1080),
+    #cam_port=80,
         # 1920*1080
-        cam_port=83,
+        cam_port=82,
         neurocore_login='admin',
         neurocore_password='admin',
         engine_callback=engine_callback
     )
     inst.set_token(os.environ.get("mail_token"))
-    inst.start()
-    #res = inst.try_recognise_plate()
+    #inst.start()
+    res = inst.try_recognise_plate()
     #print(res['number'])
```

## gravity_auto_exit/mixins.py

```diff
@@ -1,8 +1,28 @@
+import io
+from PIL import Image
+
 class NumberRecognitionService:
     get_number_link = None
 
     def get_number(self, photo):
         pass
 
 class MailRecService(NumberRecognitionService):
     pass
+
+
+class ImgCutter:
+    size = None
+
+    def cut_photo(self, photo):
+        if not self.size:
+            return photo
+        img = Image.open(io.BytesIO(photo))
+        # left, upper, right, lower
+        # 2592*1944
+        im_r = img.crop(self.size)
+        im_r.show()
+        img_byte_arr = io.BytesIO()
+        im_r.save(img_byte_arr, format='PNG')
+        img_byte_arr = img_byte_arr.getvalue()
+        return img_byte_arr
```

## Comparing `gravity_auto_exit-1.8.31.dist-info/LICENSE` & `gravity_auto_exit-1.8.41.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `gravity_auto_exit-1.8.31.dist-info/RECORD` & `gravity_auto_exit-1.8.41.dist-info/RECORD`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 gravity_auto_exit/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 gravity_auto_exit/logger.py,sha256=fqAx0eDI7R3dEGnnkoIqaTbg2qrcVuRUGAeDFnMQktA,978
-gravity_auto_exit/main.py,sha256=SOcqQ8QSkDMIxZRNAq4D9CrXqWhfmHQnfRlCm_LULCU,7553
-gravity_auto_exit/mixins.py,sha256=zzTClSits8whf-zHfeQwZANFAAymMSsL3oK539L_yz0,172
+gravity_auto_exit/main.py,sha256=NS7vbHK5-G4N-j1oGx7vdu60L6AwJWXtDZ_HJUngEI0,7786
+gravity_auto_exit/mixins.py,sha256=o3GoP9Itk2-tlxkfcUHtme7s1DoY_tdB99S9TdIomRs,654
 gravity_auto_exit/settings.py,sha256=W4ZrNBbyEsoDMvEAvRK5AH6Q2DLrK2tCzVX3i069rpE,327
 gravity_auto_exit/logs/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-gravity_auto_exit-1.8.31.dist-info/LICENSE,sha256=6kbiFSfobTZ7beWiKnHpN902HgBx-Jzgcme0SvKqhKY,1091
-gravity_auto_exit-1.8.31.dist-info/METADATA,sha256=2r-Mq29ZjgYncEaHjziWjnODAv5HSzl2Bt6q14L6-2U,409
-gravity_auto_exit-1.8.31.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-gravity_auto_exit-1.8.31.dist-info/top_level.txt,sha256=O896kTA32MK0-JQ_QK-QUsag8oA7wVEeEJGjgZiBpt4,18
-gravity_auto_exit-1.8.31.dist-info/RECORD,,
+gravity_auto_exit-1.8.41.dist-info/LICENSE,sha256=6kbiFSfobTZ7beWiKnHpN902HgBx-Jzgcme0SvKqhKY,1091
+gravity_auto_exit-1.8.41.dist-info/METADATA,sha256=0XTy5DrLjIfbW2OSfKmj6lR1q2G5qzD562Ts256perI,409
+gravity_auto_exit-1.8.41.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+gravity_auto_exit-1.8.41.dist-info/top_level.txt,sha256=O896kTA32MK0-JQ_QK-QUsag8oA7wVEeEJGjgZiBpt4,18
+gravity_auto_exit-1.8.41.dist-info/RECORD,,
```

