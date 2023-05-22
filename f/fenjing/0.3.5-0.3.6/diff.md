# Comparing `tmp/fenjing-0.3.5.tar.gz` & `tmp/fenjing-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fenjing-0.3.5.tar", last modified: Sat May 20 12:11:01 2023, max compression
+gzip compressed data, was "fenjing-0.3.6.tar", last modified: Mon May 22 14:28:14 2023, max compression
```

## Comparing `fenjing-0.3.5.tar` & `fenjing-0.3.6.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 12:11:01.751224 fenjing-0.3.5/
--rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-05-20 12:10:42.000000 fenjing-0.3.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-20 12:10:42.000000 fenjing-0.3.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6505 2023-05-20 12:11:01.751224 fenjing-0.3.5/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)     6068 2023-05-20 12:10:42.000000 fenjing-0.3.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-20 12:10:42.000000 fenjing-0.3.5/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 12:11:01.751224 fenjing-0.3.5/fenjing/
--rwxr-xr-x   0 runner    (1001) docker     (123)      202 2023-05-20 12:10:42.000000 fenjing-0.3.5/fenjing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-20 12:10:42.000000 fenjing-0.3.5/fenjing/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6635 2023-05-20 12:10:42.000000 fenjing-0.3.5/fenjing/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-05-20 12:10:42.000000 fenjing-0.3.5/fenjing/colorize.py
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-05-20 12:10:42.000000 fenjing-0.3.5/fenjing/config_payload.py
--rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-05-20 12:10:42.000000 fenjing-0.3.5/fenjing/const.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       37 2023-05-20 12:10:42.000000 fenjing-0.3.5/fenjing/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-05-20 12:10:42.000000 fenjing-0.3.5/fenjing/form.py
--rw-r--r--   0 runner    (1001) docker     (123)     5614 2023-05-20 12:10:42.000000 fenjing-0.3.5/fenjing/form_cracker.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4234 2023-05-20 12:10:42.000000 fenjing-0.3.5/fenjing/full_payload_gen.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2846 2023-05-20 12:10:42.000000 fenjing-0.3.5/fenjing/int_vars.py
--rw-r--r--   0 runner    (1001) docker     (123)    28571 2023-05-20 12:10:42.000000 fenjing-0.3.5/fenjing/payload_gen.py
--rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-05-20 12:10:42.000000 fenjing-0.3.5/fenjing/requester.py
--rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-05-20 12:10:42.000000 fenjing-0.3.5/fenjing/scan_url.py
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-05-20 12:10:42.000000 fenjing-0.3.5/fenjing/shell_payload.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 12:11:01.751224 fenjing-0.3.5/fenjing/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     9139 2023-05-20 12:10:42.000000 fenjing-0.3.5/fenjing/templates/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-05-20 12:10:42.000000 fenjing-0.3.5/fenjing/waf_func_gen.py
--rw-r--r--   0 runner    (1001) docker     (123)     9104 2023-05-20 12:10:42.000000 fenjing-0.3.5/fenjing/webui.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 12:11:01.751224 fenjing-0.3.5/fenjing.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6505 2023-05-20 12:11:01.000000 fenjing-0.3.5/fenjing.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-05-20 12:11:01.000000 fenjing-0.3.5/fenjing.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 12:11:01.000000 fenjing-0.3.5/fenjing.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-20 12:11:01.000000 fenjing-0.3.5/fenjing.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-20 12:11:01.000000 fenjing-0.3.5/fenjing.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-20 12:10:42.000000 fenjing-0.3.5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-20 12:11:01.751224 fenjing-0.3.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      944 2023-05-20 12:10:42.000000 fenjing-0.3.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 14:28:14.067323 fenjing-0.3.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-05-22 14:28:00.000000 fenjing-0.3.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-22 14:28:00.000000 fenjing-0.3.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6552 2023-05-22 14:28:14.067323 fenjing-0.3.6/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6115 2023-05-22 14:28:00.000000 fenjing-0.3.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-22 14:28:00.000000 fenjing-0.3.6/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 14:28:14.063323 fenjing-0.3.6/fenjing/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      202 2023-05-22 14:28:00.000000 fenjing-0.3.6/fenjing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-22 14:28:00.000000 fenjing-0.3.6/fenjing/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8080 2023-05-22 14:28:00.000000 fenjing-0.3.6/fenjing/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-05-22 14:28:00.000000 fenjing-0.3.6/fenjing/colorize.py
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-05-22 14:28:00.000000 fenjing-0.3.6/fenjing/config_payload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-05-22 14:28:00.000000 fenjing-0.3.6/fenjing/const.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       37 2023-05-22 14:28:00.000000 fenjing-0.3.6/fenjing/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-05-22 14:28:00.000000 fenjing-0.3.6/fenjing/form.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5614 2023-05-22 14:28:00.000000 fenjing-0.3.6/fenjing/form_cracker.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4234 2023-05-22 14:28:00.000000 fenjing-0.3.6/fenjing/full_payload_gen.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2846 2023-05-22 14:28:00.000000 fenjing-0.3.6/fenjing/int_vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28571 2023-05-22 14:28:00.000000 fenjing-0.3.6/fenjing/payload_gen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-05-22 14:28:00.000000 fenjing-0.3.6/fenjing/requester.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-05-22 14:28:00.000000 fenjing-0.3.6/fenjing/scan_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-05-22 14:28:00.000000 fenjing-0.3.6/fenjing/shell_payload.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 14:28:14.067323 fenjing-0.3.6/fenjing/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     9139 2023-05-22 14:28:00.000000 fenjing-0.3.6/fenjing/templates/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-05-22 14:28:00.000000 fenjing-0.3.6/fenjing/waf_func_gen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9104 2023-05-22 14:28:00.000000 fenjing-0.3.6/fenjing/webui.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 14:28:14.063323 fenjing-0.3.6/fenjing.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6552 2023-05-22 14:28:14.000000 fenjing-0.3.6/fenjing.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-05-22 14:28:14.000000 fenjing-0.3.6/fenjing.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 14:28:14.000000 fenjing-0.3.6/fenjing.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-22 14:28:14.000000 fenjing-0.3.6/fenjing.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-22 14:28:14.000000 fenjing-0.3.6/fenjing.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-22 14:28:00.000000 fenjing-0.3.6/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 14:28:14.067323 fenjing-0.3.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-05-22 14:28:00.000000 fenjing-0.3.6/setup.py
```

### Comparing `fenjing-0.3.5/LICENSE` & `fenjing-0.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `fenjing-0.3.5/PKG-INFO` & `fenjing-0.3.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fenjing
-Version: 0.3.5
+Version: 0.3.6
 Summary: A Jinja SSTI cracker for CTF competitions
 Home-page: https://github.com/Marven11/Fenjing
 Author: Marven11
 Author-email: marven11@example.com
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Operating System :: OS Independent
@@ -200,12 +200,14 @@
     config_payload = config_payload(waf)
 
     print(f"{shell_payload=}")
     print(f"{config_payload=}")
 
 ```
 
+其他使用例可以看[这里](examples.md)
+
 ## 项目结构
 
 [![](https://mermaid.ink/img/pako:eNp1U01TwyAQ_SsMM-2p-QM5eHA86kU9aTqZLVkaRgKRD2vt9L8LwZQkrRwYeLzdfbyFE2W6QVpSLvWBtWAceb2vFAnD-t3eQN8S74S0JIFxMC21ET-YEYOfHq1DkyGuTTcNUdblbVqhapaVLJpCqJCIA8NpSSneOdiSQxEOO6FARmybGQfc-cjZRQ4XBrn-TuB2loYUxV3CLyLIQkWUbnPQakWakI85oRV5fpyUBF5zr1i9RzW_eM0MsI-pHZaBqr2Rt3lJ1FW6waCFuB6OUkMz0ZfFjZ2LI7hYf4GZ8GyLUtZ_8bPWcLG_xrnP7PkNb4LzNGQ9LzdccJlxAKf79UL15YGMfbv2djyZ-5vmocv_xC3cvyUvWk83tAvvDUQTvsgphlbUtdhhRcuwVOidAVnRSp0DFbzTL0fFaOmMxw31fQMOHwSE1nU0PExpA9qDetM677ERTpun9A2H33j-BR2iIbY?type=png)](https://mermaid.live/edit#pako:eNp1U01TwyAQ_SsMM-2p-QM5eHA86kU9aTqZLVkaRgKRD2vt9L8LwZQkrRwYeLzdfbyFE2W6QVpSLvWBtWAceb2vFAnD-t3eQN8S74S0JIFxMC21ET-YEYOfHq1DkyGuTTcNUdblbVqhapaVLJpCqJCIA8NpSSneOdiSQxEOO6FARmybGQfc-cjZRQ4XBrn-TuB2loYUxV3CLyLIQkWUbnPQakWakI85oRV5fpyUBF5zr1i9RzW_eM0MsI-pHZaBqr2Rt3lJ1FW6waCFuB6OUkMz0ZfFjZ2LI7hYf4GZ8GyLUtZ_8bPWcLG_xrnP7PkNb4LzNGQ9LzdccJlxAKf79UL15YGMfbv2djyZ-5vmocv_xC3cvyUvWk83tAvvDUQTvsgphlbUtdhhRcuwVOidAVnRSp0DFbzTL0fFaOmMxw31fQMOHwSE1nU0PExpA9qDetM677ERTpun9A2H33j-BR2iIbY)
```

### Comparing `fenjing-0.3.5/README.md` & `fenjing-0.3.6/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -187,12 +187,14 @@
     config_payload = config_payload(waf)
 
     print(f"{shell_payload=}")
     print(f"{config_payload=}")
 
 ```
 
+其他使用例可以看[这里](examples.md)
+
 ## 项目结构
 
 [![](https://mermaid.ink/img/pako:eNp1U01TwyAQ_SsMM-2p-QM5eHA86kU9aTqZLVkaRgKRD2vt9L8LwZQkrRwYeLzdfbyFE2W6QVpSLvWBtWAceb2vFAnD-t3eQN8S74S0JIFxMC21ET-YEYOfHq1DkyGuTTcNUdblbVqhapaVLJpCqJCIA8NpSSneOdiSQxEOO6FARmybGQfc-cjZRQ4XBrn-TuB2loYUxV3CLyLIQkWUbnPQakWakI85oRV5fpyUBF5zr1i9RzW_eM0MsI-pHZaBqr2Rt3lJ1FW6waCFuB6OUkMz0ZfFjZ2LI7hYf4GZ8GyLUtZ_8bPWcLG_xrnP7PkNb4LzNGQ9LzdccJlxAKf79UL15YGMfbv2djyZ-5vmocv_xC3cvyUvWk83tAvvDUQTvsgphlbUtdhhRcuwVOidAVnRSp0DFbzTL0fFaOmMxw31fQMOHwSE1nU0PExpA9qDetM677ERTpun9A2H33j-BR2iIbY?type=png)](https://mermaid.live/edit#pako:eNp1U01TwyAQ_SsMM-2p-QM5eHA86kU9aTqZLVkaRgKRD2vt9L8LwZQkrRwYeLzdfbyFE2W6QVpSLvWBtWAceb2vFAnD-t3eQN8S74S0JIFxMC21ET-YEYOfHq1DkyGuTTcNUdblbVqhapaVLJpCqJCIA8NpSSneOdiSQxEOO6FARmybGQfc-cjZRQ4XBrn-TuB2loYUxV3CLyLIQkWUbnPQakWakI85oRV5fpyUBF5zr1i9RzW_eM0MsI-pHZaBqr2Rt3lJ1FW6waCFuB6OUkMz0ZfFjZ2LI7hYf4GZ8GyLUtZ_8bPWcLG_xrnP7PkNb4LzNGQ9LzdccJlxAKf79UL15YGMfbv2djyZ-5vmocv_xC3cvyUvWk83tAvvDUQTvsgphlbUtdhhRcuwVOidAVnRSp0DFbzTL0fFaOmMxw31fQMOHwSE1nU0PExpA9qDetM677ERTpun9A2H33j-BR2iIbY)
```

### Comparing `fenjing-0.3.5/fenjing/cli.py` & `fenjing-0.3.6/fenjing/cli.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import logging
 from urllib.parse import urlparse
 from traceback import print_exc
-from typing import Callable, List
+from typing import Callable, List, Dict
 from functools import partial
 
 from .form import Form
 from .form_cracker import FormCracker
 from .full_payload_gen import FullPayloadGen
 from .scan_url import yield_form
 from .requester import Requester
@@ -61,47 +61,69 @@
         try:
             result = cmd_exec(cmd)
             print(result)
         except Exception:
             print_exc()
 
 
+def parse_headers_cookies(headers_list: List[str], cookies: str) -> Dict[str, str]:
+    headers = {}
+    if headers_list:
+        for header in headers_list:
+            k, _, v = header.partition(": ")
+            if not k or not v:
+                logger.warning(f"Failed parsing {repr(header)}, ignored.")
+                continue
+            if k.capitalize() != k:
+                logger.warning(f"Header {k} is not capitalized, fixed.")
+                k = k.capitalize()
+            headers[k] = v
+    if cookies:
+        headers["Cookie"] = cookies
+    return headers
+    
+
 @click.group()
 def main():
     pass
 
 
 @main.command()
 @click.option("--url", "-u", help="form所在的URL")
 @click.option("--action", "-a", default=None, help="form的action，默认为当前路径")
 @click.option("--method", "-m", default="POST", help="form的提交方式，默认为POST")
 @click.option("--inputs", "-i", help="form的参数，以逗号分隔")
 @click.option("--interval", default=0.0, help="每次请求的间隔")
 @click.option("--user-agent", default=DEFAULT_USER_AGENT, help="请求时使用的User Agent")
+@click.option("--header", default=[], multiple=True, help="请求时使用的Headers")
+@click.option("--cookies", default="", help="请求时使用的Cookie")
 def get_config(
         url: str,
         action: str,
         method: str,
         inputs: str,
         interval: float,
-        user_agent: str):
+        user_agent: str,
+        header: tuple,
+        cookies: str):
     """
     攻击指定的表单，并获得目标服务器的flask config
     """
     print(TITLE)
     assert all(param is not None for param in [
                url, inputs]), "Please check your param"
     form = Form(
         action=action or urlparse(url).path,
         method=method,
         inputs=inputs.split(",")
     )
     requester = Requester(
         interval=interval,
-        user_agent=user_agent
+        user_agent=user_agent,
+        headers=parse_headers_cookies(headers_list=list(header), cookies=cookies)
     )
     cracker = FormCracker(
         url=url,
         form=form,
         requester=requester
     )
     result = cracker.crack()
@@ -120,36 +142,41 @@
 @click.option("--url", "-u", help="form所在的URL")
 @click.option("--action", "-a", default=None, help="form的action，默认为当前路径")
 @click.option("--method", "-m", default="POST", help="form的提交方式，默认为POST")
 @click.option("--inputs", "-i", help="form的参数，以逗号分隔")
 @click.option("--exec-cmd", "-e", default="", help="成功后执行的shell指令，不填则成功后进入交互模式")
 @click.option("--interval", default=0.0, help="每次请求的间隔")
 @click.option("--user-agent", default=DEFAULT_USER_AGENT, help="请求时使用的User Agent")
+@click.option("--header", default=[], multiple=True, help="请求时使用的Headers")
+@click.option("--cookies", default="", help="请求时使用的Cookie")
 def crack(
         url: str,
         action: str,
         method: str,
         inputs: str,
         exec_cmd: str,
         interval: float,
-        user_agent: str):
+        user_agent: str,
+        header: tuple,
+        cookies: str):
     """
     攻击指定的表单
     """
     print(TITLE)
     assert all(param is not None for param in [
                url, inputs]), "Please check your param"
     form = Form(
         action=action or urlparse(url).path,
         method=method,
         inputs=inputs.split(",")
     )
     requester = Requester(
         interval=interval,
-        user_agent=user_agent
+        user_agent=user_agent,
+        headers=parse_headers_cookies(headers_list=list(header), cookies=cookies)
     )
     cracker = FormCracker(
         url=url,
         form=form,
         requester=requester
     )
     result = cracker.crack()
@@ -167,20 +194,26 @@
 
 
 @main.command()
 @click.option("--url", "-u", help="需要扫描的URL")
 @click.option("--exec-cmd", "-e", default="", help="成功后执行的shell指令，不填则进入交互模式")
 @click.option("--interval", default=0.0, help="每次请求的间隔")
 @click.option("--user-agent", default=DEFAULT_USER_AGENT, help="请求时使用的User Agent")
-def scan(url, exec_cmd, interval, user_agent):
+@click.option("--header", default=[], multiple=True, help="请求时使用的Headers")
+@click.option("--cookies", default="", help="请求时使用的Cookie")
+def scan(url, exec_cmd, interval, user_agent, header, cookies):
     """
     扫描指定的网站
     """
     print(TITLE)
-    requester = Requester(interval=interval, user_agent=user_agent)
+    requester = Requester(
+        interval=interval, 
+        user_agent=user_agent, 
+        headers=parse_headers_cookies(headers_list=list(header), cookies=cookies)
+    )
     for page_url, forms in yield_form(requester, url):
         for form in forms:
             cracker = FormCracker(url=page_url, form=form, requester=requester)
             result = cracker.crack()
             if result is None:
                 continue
             full_payload_gen, field = result
```

### Comparing `fenjing-0.3.5/fenjing/colorize.py` & `fenjing-0.3.6/fenjing/colorize.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.3.5/fenjing/config_payload.py` & `fenjing-0.3.6/fenjing/config_payload.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.3.5/fenjing/const.py` & `fenjing-0.3.6/fenjing/const.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.3.5/fenjing/form.py` & `fenjing-0.3.6/fenjing/form.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.3.5/fenjing/form_cracker.py` & `fenjing-0.3.6/fenjing/form_cracker.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.3.5/fenjing/full_payload_gen.py` & `fenjing-0.3.6/fenjing/full_payload_gen.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.3.5/fenjing/int_vars.py` & `fenjing-0.3.6/fenjing/int_vars.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.3.5/fenjing/payload_gen.py` & `fenjing-0.3.6/fenjing/payload_gen.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.3.5/fenjing/requester.py` & `fenjing-0.3.6/fenjing/requester.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,25 +11,29 @@
     def __init__(
         self,
         interval=0.0,
         timeout=10,
         retry_times=5,
         retry_interval=1,
         retry_status=(429, ),
-        user_agent=DEFAULT_USER_AGENT
+        user_agent=DEFAULT_USER_AGENT,
+        headers={},
     ):
         self.interval = interval
         self.timeout = timeout
         self.retry_times = retry_times
         self.retry_interval = retry_interval
         self.retry_status = retry_status
         self.session = requests.Session()
         self.session.headers.update({"User-Agent": user_agent})
         self.last_request_time = 0
 
+        if headers:
+            self.session.headers.update(headers)
+
     def request_once(self, **kwargs):
         duration = time.perf_counter() - self.last_request_time
         if duration < self.interval:
             time.sleep(self.interval - duration)
 
         if "timeout" not in kwargs:
             kwargs["timeout"] = self.timeout
```

### Comparing `fenjing-0.3.5/fenjing/scan_url.py` & `fenjing-0.3.6/fenjing/scan_url.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.3.5/fenjing/shell_payload.py` & `fenjing-0.3.6/fenjing/shell_payload.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.3.5/fenjing/templates/index.html` & `fenjing-0.3.6/fenjing/templates/index.html`

 * *Files identical despite different names*

### Comparing `fenjing-0.3.5/fenjing/waf_func_gen.py` & `fenjing-0.3.6/fenjing/waf_func_gen.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.3.5/fenjing/webui.py` & `fenjing-0.3.6/fenjing/webui.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.3.5/fenjing.egg-info/PKG-INFO` & `fenjing-0.3.6/fenjing.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fenjing
-Version: 0.3.5
+Version: 0.3.6
 Summary: A Jinja SSTI cracker for CTF competitions
 Home-page: https://github.com/Marven11/Fenjing
 Author: Marven11
 Author-email: marven11@example.com
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Operating System :: OS Independent
@@ -200,12 +200,14 @@
     config_payload = config_payload(waf)
 
     print(f"{shell_payload=}")
     print(f"{config_payload=}")
 
 ```
 
+其他使用例可以看[这里](examples.md)
+
 ## 项目结构
 
 [![](https://mermaid.ink/img/pako:eNp1U01TwyAQ_SsMM-2p-QM5eHA86kU9aTqZLVkaRgKRD2vt9L8LwZQkrRwYeLzdfbyFE2W6QVpSLvWBtWAceb2vFAnD-t3eQN8S74S0JIFxMC21ET-YEYOfHq1DkyGuTTcNUdblbVqhapaVLJpCqJCIA8NpSSneOdiSQxEOO6FARmybGQfc-cjZRQ4XBrn-TuB2loYUxV3CLyLIQkWUbnPQakWakI85oRV5fpyUBF5zr1i9RzW_eM0MsI-pHZaBqr2Rt3lJ1FW6waCFuB6OUkMz0ZfFjZ2LI7hYf4GZ8GyLUtZ_8bPWcLG_xrnP7PkNb4LzNGQ9LzdccJlxAKf79UL15YGMfbv2djyZ-5vmocv_xC3cvyUvWk83tAvvDUQTvsgphlbUtdhhRcuwVOidAVnRSp0DFbzTL0fFaOmMxw31fQMOHwSE1nU0PExpA9qDetM677ERTpun9A2H33j-BR2iIbY?type=png)](https://mermaid.live/edit#pako:eNp1U01TwyAQ_SsMM-2p-QM5eHA86kU9aTqZLVkaRgKRD2vt9L8LwZQkrRwYeLzdfbyFE2W6QVpSLvWBtWAceb2vFAnD-t3eQN8S74S0JIFxMC21ET-YEYOfHq1DkyGuTTcNUdblbVqhapaVLJpCqJCIA8NpSSneOdiSQxEOO6FARmybGQfc-cjZRQ4XBrn-TuB2loYUxV3CLyLIQkWUbnPQakWakI85oRV5fpyUBF5zr1i9RzW_eM0MsI-pHZaBqr2Rt3lJ1FW6waCFuB6OUkMz0ZfFjZ2LI7hYf4GZ8GyLUtZ_8bPWcLG_xrnP7PkNb4LzNGQ9LzdccJlxAKf79UL15YGMfbv2djyZ-5vmocv_xC3cvyUvWk83tAvvDUQTvsgphlbUtdhhRcuwVOidAVnRSp0DFbzTL0fFaOmMxw31fQMOHwSE1nU0PExpA9qDetM677ERTpun9A2H33j-BR2iIbY)
```

### Comparing `fenjing-0.3.5/fenjing.egg-info/SOURCES.txt` & `fenjing-0.3.6/fenjing.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fenjing-0.3.5/setup.py` & `fenjing-0.3.6/setup.py`

 * *Files identical despite different names*

