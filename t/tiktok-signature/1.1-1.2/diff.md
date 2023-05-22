# Comparing `tmp/tiktok_signature-1.1.tar.gz` & `tmp/tiktok_signature-1.2.tar.gz`

## Comparing `tiktok_signature-1.1.tar` & `tiktok_signature-1.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 tiktok_signature-1.1/tiktok_signature/__init__.py
--rw-r--r--   0        0        0   381016 2020-02-02 00:00:00.000000 tiktok_signature-1.1/tiktok_signature/scripts.py
--rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 tiktok_signature-1.1/tiktok_signature/server.py
--rw-r--r--   0        0        0     5304 2020-02-02 00:00:00.000000 tiktok_signature-1.1/tiktok_signature/signature.py
--rw-r--r--   0        0        0     3237 2020-02-02 00:00:00.000000 tiktok_signature-1.1/.gitignore
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 tiktok_signature-1.1/LICENSE
--rw-r--r--   0        0        0     1181 2020-02-02 00:00:00.000000 tiktok_signature-1.1/README.md
--rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 tiktok_signature-1.1/pyproject.toml
--rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 tiktok_signature-1.1/PKG-INFO
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 tiktok_signature-1.2/tiktok_signature/__init__.py
+-rw-r--r--   0        0        0   381016 2020-02-02 00:00:00.000000 tiktok_signature-1.2/tiktok_signature/scripts.py
+-rw-r--r--   0        0        0     1440 2020-02-02 00:00:00.000000 tiktok_signature-1.2/tiktok_signature/server.py
+-rw-r--r--   0        0        0     5293 2020-02-02 00:00:00.000000 tiktok_signature-1.2/tiktok_signature/signature.py
+-rw-r--r--   0        0        0     3237 2020-02-02 00:00:00.000000 tiktok_signature-1.2/.gitignore
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 tiktok_signature-1.2/LICENSE
+-rw-r--r--   0        0        0     1271 2020-02-02 00:00:00.000000 tiktok_signature-1.2/README.md
+-rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 tiktok_signature-1.2/pyproject.toml
+-rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 tiktok_signature-1.2/PKG-INFO
```

### Comparing `tiktok_signature-1.1/tiktok_signature/scripts.py` & `tiktok_signature-1.2/tiktok_signature/scripts.py`

 * *Files identical despite different names*

### Comparing `tiktok_signature-1.1/tiktok_signature/signature.py` & `tiktok_signature-1.2/tiktok_signature/signature.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import base64
 import random
 from urllib.parse import urlparse
 
 from Crypto.Cipher import AES
 from Crypto.Util.Padding import pad
-from playwright.async_api._generated import Page, Playwright, Request, Route
+from playwright.async_api import Page, Playwright, Request, Route
 from .scripts import signer, bogus, webmssdk
 
 
 class Signer:
     def __init__(
         self,
         playwright: Playwright,
```

### Comparing `tiktok_signature-1.1/.gitignore` & `tiktok_signature-1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `tiktok_signature-1.1/LICENSE` & `tiktok_signature-1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tiktok_signature-1.1/README.md` & `tiktok_signature-1.2/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -18,44 +18,45 @@
 
     class Config:
         env_file = ".env"
         env_file_encoding = "utf-8"
 
 
 async def main():
-    playwright = await async_playwright().start()
     settings = Settings()
-    try:
+    async with async_playwright() as playwright:
         server = await make_server(playwright=playwright, host=settings.host, port=settings.port)
         await server.start()
         await asyncio.Event().wait()
-    finally:
-        await playwright.stop()
 
 asyncio.run(main())
 
 ```
 
 **As package**
 
 ```python
 import asyncio
 
 from tiktok_signature import Signer
 from playwright.async_api import async_playwright
 
 async def main():
-    playwright = await async_playwright().start()
-    try:
+    async with async_playwright() as playwright:
         signer = Signer(playwright=playwright)
         await signer.init()
         await signer.sign("url")
-    finally:
-        await playwright.stop()
         
 asyncio.run(main())
 
 ```
 
 **Docker**
 
-Soon...
+You can build image yourself
+```
+docker build . -t tiktok-signature
+```
+or use already ready
+```
+docker run --name=tiktok-signature --restart=always -p 8002:8002 -e port=8002 sheldygg/tiktok-signature
+```
```

### Comparing `tiktok_signature-1.1/pyproject.toml` & `tiktok_signature-1.2/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -15,14 +15,15 @@
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
 ]
 dependencies = [
     "playwright",
     "pycryptodome"
 ]
+[project.optional-dependencies]
 server = [
     "aiohttp"
 ]
 
 [project.urls]
 Homepage = "https://github.com/sheldygg/tiktok-signature"
```

### Comparing `tiktok_signature-1.1/PKG-INFO` & `tiktok_signature-1.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 Metadata-Version: 2.1
 Name: tiktok-signature
-Version: 1.1
+Version: 1.2
 Summary: Some tool
 Project-URL: Homepage, https://github.com/sheldygg/tiktok-signature
 Author: sheldy
 License-Expression: MIT
 License-File: LICENSE
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: playwright
 Requires-Dist: pycryptodome
+Provides-Extra: server
+Requires-Dist: aiohttp; extra == 'server'
 Description-Content-Type: text/markdown
 
 # Tiktok Signature
 
 ```pip install tiktok-signature```
 
 **Server**
@@ -32,44 +34,45 @@
 
     class Config:
         env_file = ".env"
         env_file_encoding = "utf-8"
 
 
 async def main():
-    playwright = await async_playwright().start()
     settings = Settings()
-    try:
+    async with async_playwright() as playwright:
         server = await make_server(playwright=playwright, host=settings.host, port=settings.port)
         await server.start()
         await asyncio.Event().wait()
-    finally:
-        await playwright.stop()
 
 asyncio.run(main())
 
 ```
 
 **As package**
 
 ```python
 import asyncio
 
 from tiktok_signature import Signer
 from playwright.async_api import async_playwright
 
 async def main():
-    playwright = await async_playwright().start()
-    try:
+    async with async_playwright() as playwright:
         signer = Signer(playwright=playwright)
         await signer.init()
         await signer.sign("url")
-    finally:
-        await playwright.stop()
         
 asyncio.run(main())
 
 ```
 
 **Docker**
 
-Soon...
+You can build image yourself
+```
+docker build . -t tiktok-signature
+```
+or use already ready
+```
+docker run --name=tiktok-signature --restart=always -p 8002:8002 -e port=8002 sheldygg/tiktok-signature
+```
```

