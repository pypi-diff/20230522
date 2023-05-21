# Comparing `tmp/microdot-1.3.0.tar.gz` & `tmp/microdot-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "microdot-1.3.0.tar", last modified: Sat Apr  8 16:21:30 2023, max compression
+gzip compressed data, was "microdot-1.3.1.tar", last modified: Sun May 21 22:37:39 2023, max compression
```

## Comparing `microdot-1.3.0.tar` & `microdot-1.3.1.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 mgrinberg   (502) staff       (20)        0 2023-04-08 16:21:30.021456 microdot-1.3.0/
--rw-r--r--   0 mgrinberg   (502) staff       (20)     1072 2020-02-18 23:41:59.000000 microdot-1.3.0/LICENSE
--rw-r--r--   0 mgrinberg   (502) staff       (20)     1525 2023-04-08 16:21:30.021861 microdot-1.3.0/PKG-INFO
--rw-r--r--   0 mgrinberg   (502) staff       (20)      847 2022-08-07 14:45:44.000000 microdot-1.3.0/README.md
--rw-r--r--   0 mgrinberg   (502) staff       (20)      104 2021-06-05 23:20:28.000000 microdot-1.3.0/pyproject.toml
--rw-r--r--   0 mgrinberg   (502) staff       (20)     1035 2023-04-08 16:21:30.023421 microdot-1.3.0/setup.cfg
--rwxr-xr-x   0 mgrinberg   (502) staff       (20)       38 2021-06-05 23:12:41.000000 microdot-1.3.0/setup.py
-drwxr-xr-x   0 mgrinberg   (502) staff       (20)        0 2023-04-08 16:21:30.000315 microdot-1.3.0/src/
-drwxr-xr-x   0 mgrinberg   (502) staff       (20)        0 2023-04-08 16:21:30.004421 microdot-1.3.0/src/microdot.egg-info/
--rw-r--r--   0 mgrinberg   (502) staff       (20)     1525 2023-04-08 16:21:29.000000 microdot-1.3.0/src/microdot.egg-info/PKG-INFO
--rw-r--r--   0 mgrinberg   (502) staff       (20)     1018 2023-04-08 16:21:29.000000 microdot-1.3.0/src/microdot.egg-info/SOURCES.txt
--rw-r--r--   0 mgrinberg   (502) staff       (20)        1 2023-04-08 16:21:29.000000 microdot-1.3.0/src/microdot.egg-info/dependency_links.txt
--rw-r--r--   0 mgrinberg   (502) staff       (20)        1 2021-06-06 10:08:26.000000 microdot-1.3.0/src/microdot.egg-info/not-zip-safe
--rw-r--r--   0 mgrinberg   (502) staff       (20)      248 2023-04-08 16:21:29.000000 microdot-1.3.0/src/microdot.egg-info/top_level.txt
--rw-r--r--   0 mgrinberg   (502) staff       (20)    46220 2023-04-08 16:20:20.000000 microdot-1.3.0/src/microdot.py
--rw-r--r--   0 mgrinberg   (502) staff       (20)     4912 2023-04-08 16:20:20.000000 microdot-1.3.0/src/microdot_asgi.py
--rw-r--r--   0 mgrinberg   (502) staff       (20)     2855 2023-04-08 16:20:20.000000 microdot-1.3.0/src/microdot_asgi_websocket.py
--rw-r--r--   0 mgrinberg   (502) staff       (20)    17370 2023-04-08 16:20:20.000000 microdot-1.3.0/src/microdot_asyncio.py
--rw-r--r--   0 mgrinberg   (502) staff       (20)     7828 2023-04-08 16:20:20.000000 microdot-1.3.0/src/microdot_asyncio_test_client.py
--rw-r--r--   0 mgrinberg   (502) staff       (20)     3780 2023-04-08 16:20:20.000000 microdot-1.3.0/src/microdot_asyncio_websocket.py
--rw-r--r--   0 mgrinberg   (502) staff       (20)     1128 2023-04-08 16:20:20.000000 microdot-1.3.0/src/microdot_jinja.py
--rw-r--r--   0 mgrinberg   (502) staff       (20)     2966 2023-04-08 16:20:20.000000 microdot-1.3.0/src/microdot_session.py
--rw-r--r--   0 mgrinberg   (502) staff       (20)    10818 2023-04-08 16:20:20.000000 microdot-1.3.0/src/microdot_test_client.py
--rw-r--r--   0 mgrinberg   (502) staff       (20)     1331 2023-04-08 16:20:20.000000 microdot-1.3.0/src/microdot_utemplate.py
--rw-r--r--   0 mgrinberg   (502) staff       (20)     5935 2023-04-08 16:20:20.000000 microdot-1.3.0/src/microdot_websocket.py
--rw-r--r--   0 mgrinberg   (502) staff       (20)     3486 2023-04-08 16:20:20.000000 microdot-1.3.0/src/microdot_websocket_alt.py
--rw-r--r--   0 mgrinberg   (502) staff       (20)     2364 2023-04-08 16:20:20.000000 microdot-1.3.0/src/microdot_wsgi.py
-drwxr-xr-x   0 mgrinberg   (502) staff       (20)        0 2023-04-08 16:21:30.020610 microdot-1.3.0/tests/
--rw-r--r--   0 mgrinberg   (502) staff       (20)     6572 2023-04-08 16:20:20.000000 microdot-1.3.0/tests/test_cors.py
--rw-r--r--   0 mgrinberg   (502) staff       (20)     1818 2023-04-08 16:20:20.000000 microdot-1.3.0/tests/test_jinja.py
--rw-r--r--   0 mgrinberg   (502) staff       (20)    24051 2023-04-08 16:20:20.000000 microdot-1.3.0/tests/test_microdot.py
--rw-r--r--   0 mgrinberg   (502) staff       (20)     5072 2023-04-08 16:20:20.000000 microdot-1.3.0/tests/test_microdot_asgi.py
--rw-r--r--   0 mgrinberg   (502) staff       (20)    24173 2023-04-08 16:20:20.000000 microdot-1.3.0/tests/test_microdot_asyncio.py
--rw-r--r--   0 mgrinberg   (502) staff       (20)     2087 2023-04-08 16:20:20.000000 microdot-1.3.0/tests/test_microdot_asyncio_websocket.py
--rw-r--r--   0 mgrinberg   (502) staff       (20)     2670 2023-04-08 16:20:20.000000 microdot-1.3.0/tests/test_microdot_websocket.py
--rw-r--r--   0 mgrinberg   (502) staff       (20)     3449 2023-04-08 16:20:20.000000 microdot-1.3.0/tests/test_microdot_wsgi.py
--rw-r--r--   0 mgrinberg   (502) staff       (20)     2367 2023-03-23 00:04:52.000000 microdot-1.3.0/tests/test_multidict.py
--rw-r--r--   0 mgrinberg   (502) staff       (20)     5785 2023-04-08 16:16:17.000000 microdot-1.3.0/tests/test_request.py
--rw-r--r--   0 mgrinberg   (502) staff       (20)     5272 2023-04-08 16:20:20.000000 microdot-1.3.0/tests/test_request_asyncio.py
--rw-r--r--   0 mgrinberg   (502) staff       (20)    12042 2023-03-21 00:28:33.000000 microdot-1.3.0/tests/test_response.py
--rw-r--r--   0 mgrinberg   (502) staff       (20)     5784 2023-04-08 16:20:20.000000 microdot-1.3.0/tests/test_response_asyncio.py
--rw-r--r--   0 mgrinberg   (502) staff       (20)     3855 2023-04-08 16:20:20.000000 microdot-1.3.0/tests/test_session.py
--rw-r--r--   0 mgrinberg   (502) staff       (20)     4050 2020-02-18 23:41:59.000000 microdot-1.3.0/tests/test_url_pattern.py
--rw-r--r--   0 mgrinberg   (502) staff       (20)      403 2022-09-24 18:55:50.000000 microdot-1.3.0/tests/test_urlencode.py
--rw-r--r--   0 mgrinberg   (502) staff       (20)     1752 2023-04-08 16:20:20.000000 microdot-1.3.0/tests/test_utemplate.py
+drwxr-xr-x   0 mgrinberg   (502) staff       (20)        0 2023-05-21 22:37:39.925662 microdot-1.3.1/
+-rw-r--r--   0 mgrinberg   (502) staff       (20)     1072 2020-02-18 23:41:59.000000 microdot-1.3.1/LICENSE
+-rw-r--r--   0 mgrinberg   (502) staff       (20)     1525 2023-05-21 22:37:39.925885 microdot-1.3.1/PKG-INFO
+-rw-r--r--   0 mgrinberg   (502) staff       (20)      847 2022-08-07 14:45:44.000000 microdot-1.3.1/README.md
+-rw-r--r--   0 mgrinberg   (502) staff       (20)      104 2021-06-05 23:20:28.000000 microdot-1.3.1/pyproject.toml
+-rw-r--r--   0 mgrinberg   (502) staff       (20)     1035 2023-05-21 22:37:39.926865 microdot-1.3.1/setup.cfg
+-rwxr-xr-x   0 mgrinberg   (502) staff       (20)       38 2021-06-05 23:12:41.000000 microdot-1.3.1/setup.py
+drwxr-xr-x   0 mgrinberg   (502) staff       (20)        0 2023-05-21 22:37:39.906470 microdot-1.3.1/src/
+drwxr-xr-x   0 mgrinberg   (502) staff       (20)        0 2023-05-21 22:37:39.909988 microdot-1.3.1/src/microdot.egg-info/
+-rw-r--r--   0 mgrinberg   (502) staff       (20)     1525 2023-05-21 22:37:39.000000 microdot-1.3.1/src/microdot.egg-info/PKG-INFO
+-rw-r--r--   0 mgrinberg   (502) staff       (20)     1018 2023-05-21 22:37:39.000000 microdot-1.3.1/src/microdot.egg-info/SOURCES.txt
+-rw-r--r--   0 mgrinberg   (502) staff       (20)        1 2023-05-21 22:37:39.000000 microdot-1.3.1/src/microdot.egg-info/dependency_links.txt
+-rw-r--r--   0 mgrinberg   (502) staff       (20)        1 2021-06-06 10:08:26.000000 microdot-1.3.1/src/microdot.egg-info/not-zip-safe
+-rw-r--r--   0 mgrinberg   (502) staff       (20)      248 2023-05-21 22:37:39.000000 microdot-1.3.1/src/microdot.egg-info/top_level.txt
+-rw-r--r--   0 mgrinberg   (502) staff       (20)    46254 2023-05-21 22:22:24.000000 microdot-1.3.1/src/microdot.py
+-rw-r--r--   0 mgrinberg   (502) staff       (20)     4912 2023-05-21 22:22:24.000000 microdot-1.3.1/src/microdot_asgi.py
+-rw-r--r--   0 mgrinberg   (502) staff       (20)     2855 2023-05-21 22:22:24.000000 microdot-1.3.1/src/microdot_asgi_websocket.py
+-rw-r--r--   0 mgrinberg   (502) staff       (20)    17370 2023-05-21 22:22:24.000000 microdot-1.3.1/src/microdot_asyncio.py
+-rw-r--r--   0 mgrinberg   (502) staff       (20)     7828 2023-05-21 22:22:24.000000 microdot-1.3.1/src/microdot_asyncio_test_client.py
+-rw-r--r--   0 mgrinberg   (502) staff       (20)     3780 2023-05-21 22:22:24.000000 microdot-1.3.1/src/microdot_asyncio_websocket.py
+-rw-r--r--   0 mgrinberg   (502) staff       (20)     1128 2023-05-21 22:22:24.000000 microdot-1.3.1/src/microdot_jinja.py
+-rw-r--r--   0 mgrinberg   (502) staff       (20)     2966 2023-05-21 22:22:24.000000 microdot-1.3.1/src/microdot_session.py
+-rw-r--r--   0 mgrinberg   (502) staff       (20)    10818 2023-05-21 22:22:24.000000 microdot-1.3.1/src/microdot_test_client.py
+-rw-r--r--   0 mgrinberg   (502) staff       (20)     1331 2023-05-21 22:22:24.000000 microdot-1.3.1/src/microdot_utemplate.py
+-rw-r--r--   0 mgrinberg   (502) staff       (20)     5935 2023-05-21 22:22:24.000000 microdot-1.3.1/src/microdot_websocket.py
+-rw-r--r--   0 mgrinberg   (502) staff       (20)     3486 2023-05-21 22:22:24.000000 microdot-1.3.1/src/microdot_websocket_alt.py
+-rw-r--r--   0 mgrinberg   (502) staff       (20)     2364 2023-05-21 22:22:24.000000 microdot-1.3.1/src/microdot_wsgi.py
+drwxr-xr-x   0 mgrinberg   (502) staff       (20)        0 2023-05-21 22:37:39.925071 microdot-1.3.1/tests/
+-rw-r--r--   0 mgrinberg   (502) staff       (20)     6572 2023-05-21 22:22:24.000000 microdot-1.3.1/tests/test_cors.py
+-rw-r--r--   0 mgrinberg   (502) staff       (20)     1818 2023-05-21 22:22:24.000000 microdot-1.3.1/tests/test_jinja.py
+-rw-r--r--   0 mgrinberg   (502) staff       (20)    24051 2023-05-21 22:22:24.000000 microdot-1.3.1/tests/test_microdot.py
+-rw-r--r--   0 mgrinberg   (502) staff       (20)     5072 2023-05-21 22:22:24.000000 microdot-1.3.1/tests/test_microdot_asgi.py
+-rw-r--r--   0 mgrinberg   (502) staff       (20)    24173 2023-05-21 22:22:24.000000 microdot-1.3.1/tests/test_microdot_asyncio.py
+-rw-r--r--   0 mgrinberg   (502) staff       (20)     2087 2023-05-21 22:22:24.000000 microdot-1.3.1/tests/test_microdot_asyncio_websocket.py
+-rw-r--r--   0 mgrinberg   (502) staff       (20)     2670 2023-05-21 22:22:24.000000 microdot-1.3.1/tests/test_microdot_websocket.py
+-rw-r--r--   0 mgrinberg   (502) staff       (20)     3449 2023-05-21 22:22:24.000000 microdot-1.3.1/tests/test_microdot_wsgi.py
+-rw-r--r--   0 mgrinberg   (502) staff       (20)     2367 2023-03-23 00:04:52.000000 microdot-1.3.1/tests/test_multidict.py
+-rw-r--r--   0 mgrinberg   (502) staff       (20)     5785 2023-04-08 16:16:17.000000 microdot-1.3.1/tests/test_request.py
+-rw-r--r--   0 mgrinberg   (502) staff       (20)     5272 2023-05-21 22:22:24.000000 microdot-1.3.1/tests/test_request_asyncio.py
+-rw-r--r--   0 mgrinberg   (502) staff       (20)    12042 2023-03-21 00:28:33.000000 microdot-1.3.1/tests/test_response.py
+-rw-r--r--   0 mgrinberg   (502) staff       (20)     5784 2023-05-21 22:22:24.000000 microdot-1.3.1/tests/test_response_asyncio.py
+-rw-r--r--   0 mgrinberg   (502) staff       (20)     3855 2023-05-21 22:22:24.000000 microdot-1.3.1/tests/test_session.py
+-rw-r--r--   0 mgrinberg   (502) staff       (20)     4188 2023-05-21 22:22:15.000000 microdot-1.3.1/tests/test_url_pattern.py
+-rw-r--r--   0 mgrinberg   (502) staff       (20)      403 2022-09-24 18:55:50.000000 microdot-1.3.1/tests/test_urlencode.py
+-rw-r--r--   0 mgrinberg   (502) staff       (20)     1752 2023-05-21 22:22:24.000000 microdot-1.3.1/tests/test_utemplate.py
```

### Comparing `microdot-1.3.0/LICENSE` & `microdot-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `microdot-1.3.0/PKG-INFO` & `microdot-1.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: microdot
-Version: 1.3.0
+Version: 1.3.1
 Summary: The impossibly small web framework for MicroPython
 Home-page: https://github.com/miguelgrinberg/microdot
 Author: Miguel Grinberg
 Author-email: miguel.grinberg@gmail.com
 Project-URL: Bug Tracker, https://github.com/miguelgrinberg/microdot/issues
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
```

### Comparing `microdot-1.3.0/README.md` & `microdot-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `microdot-1.3.0/setup.cfg` & `microdot-1.3.1/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = microdot
-version = 1.3.0
+version = 1.3.1
 author = Miguel Grinberg
 author_email = miguel.grinberg@gmail.com
 description = The impossibly small web framework for MicroPython
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/miguelgrinberg/microdot
 project_urls =
```

### Comparing `microdot-1.3.0/src/microdot.egg-info/PKG-INFO` & `microdot-1.3.1/src/microdot.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: microdot
-Version: 1.3.0
+Version: 1.3.1
 Summary: The impossibly small web framework for MicroPython
 Home-page: https://github.com/miguelgrinberg/microdot
 Author: Miguel Grinberg
 Author-email: miguel.grinberg@gmail.com
 Project-URL: Bug Tracker, https://github.com/miguelgrinberg/microdot/issues
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
```

### Comparing `microdot-1.3.0/src/microdot.egg-info/SOURCES.txt` & `microdot-1.3.1/src/microdot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `microdot-1.3.0/src/microdot.py` & `microdot-1.3.1/src/microdot.py`

 * *Files 1% similar despite different names*

```diff
@@ -304,16 +304,17 @@
     #: Example::
     #:
     #:    Request.max_readline = 16 * 1024  # 16KB lines allowed
     max_readline = 2 * 1024
 
     #: Specify a suggested read timeout to use when reading the request. Set to
     #: 0 to disable the use of a timeout. This timeout should be considered a
-    #: suggestion only, as some platforms may not support it.
-    socket_read_timeout = 0.1
+    #: suggestion only, as some platforms may not support it. The default is
+    #: 1 second.
+    socket_read_timeout = 1
 
     class G:
         pass
 
     def __init__(self, app, client_addr, method, url, http_version, headers,
                  body=None, stream=None, sock=None):
         #: The application instance to which this request belongs.
@@ -731,15 +732,15 @@
                     type_, name = segment.rsplit(':', 1)
                 else:
                     type_ = 'string'
                     name = segment
                 if type_ == 'string':
                     pattern = '[^/]+'
                 elif type_ == 'int':
-                    pattern = '\\d+'
+                    pattern = '-?\\d+'
                 elif type_ == 'path':
                     pattern = '.+'
                 elif type_.startswith('re:'):
                     pattern = type_[3:]
                 else:
                     raise ValueError('invalid URL segment type')
                 use_regex = True
@@ -1159,15 +1160,15 @@
 
         req = None
         res = None
         try:
             req = Request.create(self, stream, addr, sock)
             res = self.dispatch_request(req)
         except socket_timeout_error as exc:  # pragma: no cover
-            if exc.errno and exc.errno not in [60, 110]:
+            if exc.errno and exc.errno != errno.ETIMEDOUT:
                 print_exception(exc)  # not a timeout
         except Exception as exc:  # pragma: no cover
             print_exception(exc)
         try:
             if res and res != Response.already_handled:  # pragma: no branch
                 res.write(stream)
             stream.close()
```

### Comparing `microdot-1.3.0/src/microdot_asgi.py` & `microdot-1.3.1/src/microdot_asgi.py`

 * *Files identical despite different names*

### Comparing `microdot-1.3.0/src/microdot_asgi_websocket.py` & `microdot-1.3.1/src/microdot_asgi_websocket.py`

 * *Files identical despite different names*

### Comparing `microdot-1.3.0/src/microdot_asyncio.py` & `microdot-1.3.1/src/microdot_asyncio.py`

 * *Files identical despite different names*

### Comparing `microdot-1.3.0/src/microdot_asyncio_test_client.py` & `microdot-1.3.1/src/microdot_asyncio_test_client.py`

 * *Files identical despite different names*

### Comparing `microdot-1.3.0/src/microdot_asyncio_websocket.py` & `microdot-1.3.1/src/microdot_asyncio_websocket.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
             b'Sec-WebSocket-Accept: ' + response + b'\r\n\r\n')
 
     async def receive(self):
         while True:
             opcode, payload = await self._read_frame()
             send_opcode, data = self._process_websocket_frame(opcode, payload)
             if send_opcode:  # pragma: no cover
-                await self.send(send_opcode, data)
+                await self.send(data, send_opcode)
             elif data:  # pragma: no branch
                 return data
 
     async def send(self, data, opcode=None):
         frame = self._encode_websocket_frame(
             opcode or (self.TEXT if isinstance(data, str) else self.BINARY),
             data)
```

### Comparing `microdot-1.3.0/src/microdot_jinja.py` & `microdot-1.3.1/src/microdot_jinja.py`

 * *Files identical despite different names*

### Comparing `microdot-1.3.0/src/microdot_session.py` & `microdot-1.3.1/src/microdot_session.py`

 * *Files identical despite different names*

### Comparing `microdot-1.3.0/src/microdot_test_client.py` & `microdot-1.3.1/src/microdot_test_client.py`

 * *Files identical despite different names*

### Comparing `microdot-1.3.0/src/microdot_utemplate.py` & `microdot-1.3.1/src/microdot_utemplate.py`

 * *Files identical despite different names*

### Comparing `microdot-1.3.0/src/microdot_websocket.py` & `microdot-1.3.1/src/microdot_websocket.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
             b'Sec-WebSocket-Accept: ' + response + b'\r\n\r\n')
 
     def receive(self):
         while True:
             opcode, payload = self._read_frame()
             send_opcode, data = self._process_websocket_frame(opcode, payload)
             if send_opcode:  # pragma: no cover
-                self.send(send_opcode, data)
+                self.send(data, send_opcode)
             elif data:  # pragma: no branch
                 return data
 
     def send(self, data, opcode=None):
         frame = self._encode_websocket_frame(
             opcode or (self.TEXT if isinstance(data, str) else self.BINARY),
             data)
```

### Comparing `microdot-1.3.0/src/microdot_websocket_alt.py` & `microdot-1.3.1/src/microdot_websocket_alt.py`

 * *Files identical despite different names*

### Comparing `microdot-1.3.0/src/microdot_wsgi.py` & `microdot-1.3.1/src/microdot_wsgi.py`

 * *Files identical despite different names*

### Comparing `microdot-1.3.0/tests/test_cors.py` & `microdot-1.3.1/tests/test_cors.py`

 * *Files identical despite different names*

### Comparing `microdot-1.3.0/tests/test_jinja.py` & `microdot-1.3.1/tests/test_jinja.py`

 * *Files identical despite different names*

### Comparing `microdot-1.3.0/tests/test_microdot.py` & `microdot-1.3.1/tests/test_microdot.py`

 * *Files identical despite different names*

### Comparing `microdot-1.3.0/tests/test_microdot_asgi.py` & `microdot-1.3.1/tests/test_microdot_asgi.py`

 * *Files identical despite different names*

### Comparing `microdot-1.3.0/tests/test_microdot_asyncio.py` & `microdot-1.3.1/tests/test_microdot_asyncio.py`

 * *Files identical despite different names*

### Comparing `microdot-1.3.0/tests/test_microdot_asyncio_websocket.py` & `microdot-1.3.1/tests/test_microdot_asyncio_websocket.py`

 * *Files identical despite different names*

### Comparing `microdot-1.3.0/tests/test_microdot_websocket.py` & `microdot-1.3.1/tests/test_microdot_websocket.py`

 * *Files identical despite different names*

### Comparing `microdot-1.3.0/tests/test_microdot_wsgi.py` & `microdot-1.3.1/tests/test_microdot_wsgi.py`

 * *Files identical despite different names*

### Comparing `microdot-1.3.0/tests/test_multidict.py` & `microdot-1.3.1/tests/test_multidict.py`

 * *Files identical despite different names*

### Comparing `microdot-1.3.0/tests/test_request.py` & `microdot-1.3.1/tests/test_request.py`

 * *Files identical despite different names*

### Comparing `microdot-1.3.0/tests/test_request_asyncio.py` & `microdot-1.3.1/tests/test_request_asyncio.py`

 * *Files identical despite different names*

### Comparing `microdot-1.3.0/tests/test_response.py` & `microdot-1.3.1/tests/test_response.py`

 * *Files identical despite different names*

### Comparing `microdot-1.3.0/tests/test_response_asyncio.py` & `microdot-1.3.1/tests/test_response_asyncio.py`

 * *Files identical despite different names*

### Comparing `microdot-1.3.0/tests/test_session.py` & `microdot-1.3.1/tests/test_session.py`

 * *Files identical despite different names*

### Comparing `microdot-1.3.0/tests/test_url_pattern.py` & `microdot-1.3.1/tests/test_url_pattern.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,18 +52,20 @@
         self.assertIsNone(p.match('/users/'))
         self.assertIsNone(p.match('/users/abc'))
         self.assertIsNone(p.match('/users/123abc'))
         self.assertIsNone(p.match('/users/123/abc'))
 
         p = URLPattern('/users/<int:id>/<int:id2>/')
         self.assertEqual(p.match('/users/123/456/'), {'id': 123, 'id2': 456})
+        self.assertEqual(p.match('/users/123/-456/'), {'id': 123, 'id2': -456})
         self.assertIsNone(p.match('/users/'))
-        self.assertIsNone(p.match('/users/123/456'))
+        self.assertIsNone(p.match('/users/123/-456'))
         self.assertIsNone(p.match('/users/123/abc/'))
-        self.assertIsNone(p.match('/users/123/456/abc'))
+        self.assertIsNone(p.match('/users/123/-456/abc'))
+        self.assertIsNone(p.match('/users/--123/456/'))
 
     def test_path_argument(self):
         p = URLPattern('/users/<path:path>')
         self.assertEqual(p.match('/users/123'), {'path': '123'})
         self.assertEqual(p.match('/users/123/'), {'path': '123/'})
         self.assertEqual(p.match('/users/abc/def'), {'path': 'abc/def'})
         self.assertIsNone(p.match('/users/'))
```

### Comparing `microdot-1.3.0/tests/test_utemplate.py` & `microdot-1.3.1/tests/test_utemplate.py`

 * *Files identical despite different names*

