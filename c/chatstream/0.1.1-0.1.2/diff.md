# Comparing `tmp/ChatStream-0.1.1.tar.gz` & `tmp/chatstream-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ChatStream-0.1.1.tar", last modified: Mon May 22 02:20:13 2023, max compression
+gzip compressed data, was "chatstream-0.1.2.tar", last modified: Mon May 22 02:39:00 2023, max compression
```

## Comparing `ChatStream-0.1.1.tar` & `chatstream-0.1.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-05-22 02:20:13.000892 ChatStream-0.1.1/
-drwxrwxrwx   0        0        0        0 2023-05-22 02:20:12.986374 ChatStream-0.1.1/ChatStream.egg-info/
--rw-rw-rw-   0        0        0     6926 2023-05-22 02:20:12.000000 ChatStream-0.1.1/ChatStream.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      599 2023-05-22 02:20:12.000000 ChatStream-0.1.1/ChatStream.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-22 02:20:12.000000 ChatStream-0.1.1/ChatStream.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2023-05-22 02:20:12.000000 ChatStream-0.1.1/ChatStream.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-05-22 02:20:12.000000 ChatStream-0.1.1/ChatStream.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    11356 2023-05-21 23:57:09.000000 ChatStream-0.1.1/LICENSE
--rw-rw-rw-   0        0        0     6926 2023-05-22 02:20:12.999892 ChatStream-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     6103 2023-05-22 01:43:46.000000 ChatStream-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-22 02:20:12.998891 ChatStream-0.1.1/chatstream/
--rw-rw-rw-   0        0        0      168 2023-05-21 23:57:09.000000 ChatStream-0.1.1/chatstream/__init__.py
--rw-rw-rw-   0        0        0     8430 2023-05-21 23:57:09.000000 ChatStream-0.1.1/chatstream/chat_core.py
--rw-rw-rw-   0        0        0     8648 2023-05-21 23:57:09.000000 ChatStream-0.1.1/chatstream/chat_process.py
--rw-rw-rw-   0        0        0     2644 2023-05-21 23:57:09.000000 ChatStream-0.1.1/chatstream/chat_process_mock.py
--rw-rw-rw-   0        0        0     6416 2023-05-22 01:34:57.000000 ChatStream-0.1.1/chatstream/chat_prompt.py
--rw-rw-rw-   0        0        0    20904 2023-05-22 00:16:49.000000 ChatStream-0.1.1/chatstream/chat_stream.py
--rw-rw-rw-   0        0        0     3146 2023-05-21 23:57:09.000000 ChatStream-0.1.1/chatstream/mock_response_example_text.py
-drwxrwxrwx   0        0        0        0 2023-05-22 02:20:12.999892 ChatStream-0.1.1/chatstream/request_handler/
--rw-rw-rw-   0        0        0        0 2023-05-21 23:57:09.000000 ChatStream-0.1.1/chatstream/request_handler/__init__.py
--rw-rw-rw-   0        0        0     4071 2023-05-21 23:57:09.000000 ChatStream-0.1.1/chatstream/request_handler/request_handler.py
--rw-rw-rw-   0        0        0     4916 2023-05-21 23:57:09.000000 ChatStream-0.1.1/chatstream/request_handler/simple_session_request_handler.py
--rw-rw-rw-   0        0        0     3356 2023-05-21 23:57:09.000000 ChatStream-0.1.1/chatstream/sampling_utils.py
--rw-rw-rw-   0        0        0      803 2023-05-21 23:57:09.000000 ChatStream-0.1.1/chatstream/util_request_id.py
--rw-rw-rw-   0        0        0       42 2023-05-22 02:20:13.000892 ChatStream-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1000 2023-05-22 02:03:34.000000 ChatStream-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-22 02:39:00.391983 chatstream-0.1.2/
+drwxrwxrwx   0        0        0        0 2023-05-22 02:39:00.376145 chatstream-0.1.2/ChatStream.egg-info/
+-rw-rw-rw-   0        0        0     6926 2023-05-22 02:39:00.000000 chatstream-0.1.2/ChatStream.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      768 2023-05-22 02:39:00.000000 chatstream-0.1.2/ChatStream.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-22 02:39:00.000000 chatstream-0.1.2/ChatStream.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2023-05-22 02:39:00.000000 chatstream-0.1.2/ChatStream.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-05-22 02:39:00.000000 chatstream-0.1.2/ChatStream.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    11356 2023-05-21 23:57:09.000000 chatstream-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0     6926 2023-05-22 02:39:00.391983 chatstream-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     6103 2023-05-22 01:43:46.000000 chatstream-0.1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-22 02:39:00.389978 chatstream-0.1.2/chatstream/
+-rw-rw-rw-   0        0        0      168 2023-05-21 23:57:09.000000 chatstream-0.1.2/chatstream/__init__.py
+-rw-rw-rw-   0        0        0     8430 2023-05-21 23:57:09.000000 chatstream-0.1.2/chatstream/chat_core.py
+-rw-rw-rw-   0        0        0     8648 2023-05-21 23:57:09.000000 chatstream-0.1.2/chatstream/chat_process.py
+-rw-rw-rw-   0        0        0     2644 2023-05-21 23:57:09.000000 chatstream-0.1.2/chatstream/chat_process_mock.py
+-rw-rw-rw-   0        0        0     6416 2023-05-22 01:34:57.000000 chatstream-0.1.2/chatstream/chat_prompt.py
+-rw-rw-rw-   0        0        0    20904 2023-05-22 00:16:49.000000 chatstream-0.1.2/chatstream/chat_stream.py
+-rw-rw-rw-   0        0        0     3146 2023-05-21 23:57:09.000000 chatstream-0.1.2/chatstream/mock_response_example_text.py
+drwxrwxrwx   0        0        0        0 2023-05-22 02:39:00.390982 chatstream-0.1.2/chatstream/request_handler/
+-rw-rw-rw-   0        0        0        0 2023-05-21 23:57:09.000000 chatstream-0.1.2/chatstream/request_handler/__init__.py
+-rw-rw-rw-   0        0        0     4071 2023-05-21 23:57:09.000000 chatstream-0.1.2/chatstream/request_handler/request_handler.py
+-rw-rw-rw-   0        0        0     4916 2023-05-21 23:57:09.000000 chatstream-0.1.2/chatstream/request_handler/simple_session_request_handler.py
+-rw-rw-rw-   0        0        0     3356 2023-05-21 23:57:09.000000 chatstream-0.1.2/chatstream/sampling_utils.py
+-rw-rw-rw-   0        0        0      803 2023-05-21 23:57:09.000000 chatstream-0.1.2/chatstream/util_request_id.py
+-rw-rw-rw-   0        0        0       42 2023-05-22 02:39:00.391983 chatstream-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1001 2023-05-22 02:38:03.000000 chatstream-0.1.2/setup.py
```

### Comparing `ChatStream-0.1.1/ChatStream.egg-info/PKG-INFO` & `chatstream-0.1.2/ChatStream.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: ChatStream
-Version: 0.1.1
+Name: chatstream
+Version: 0.1.2
 Summary: Streaming chat server building blocks for FastAPI/Starlette
 Home-page: https://github.com/riversun/ChatStream
 Author: Tom Misawa
 Author-email: riversun.org@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `ChatStream-0.1.1/ChatStream.egg-info/SOURCES.txt` & `chatstream-0.1.2/ChatStream.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -11,10 +11,15 @@
 chatstream/chat_process.py
 chatstream/chat_process_mock.py
 chatstream/chat_prompt.py
 chatstream/chat_stream.py
 chatstream/mock_response_example_text.py
 chatstream/sampling_utils.py
 chatstream/util_request_id.py
+chatstream.egg-info/PKG-INFO
+chatstream.egg-info/SOURCES.txt
+chatstream.egg-info/dependency_links.txt
+chatstream.egg-info/requires.txt
+chatstream.egg-info/top_level.txt
 chatstream/request_handler/__init__.py
 chatstream/request_handler/request_handler.py
 chatstream/request_handler/simple_session_request_handler.py
```

### Comparing `ChatStream-0.1.1/LICENSE` & `chatstream-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ChatStream-0.1.1/PKG-INFO` & `chatstream-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: ChatStream
-Version: 0.1.1
+Name: chatstream
+Version: 0.1.2
 Summary: Streaming chat server building blocks for FastAPI/Starlette
 Home-page: https://github.com/riversun/ChatStream
 Author: Tom Misawa
 Author-email: riversun.org@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `ChatStream-0.1.1/README.md` & `chatstream-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `ChatStream-0.1.1/chatstream/chat_core.py` & `chatstream-0.1.2/chatstream/chat_core.py`

 * *Files identical despite different names*

### Comparing `ChatStream-0.1.1/chatstream/chat_process.py` & `chatstream-0.1.2/chatstream/chat_process.py`

 * *Files identical despite different names*

### Comparing `ChatStream-0.1.1/chatstream/chat_process_mock.py` & `chatstream-0.1.2/chatstream/chat_process_mock.py`

 * *Files identical despite different names*

### Comparing `ChatStream-0.1.1/chatstream/chat_prompt.py` & `chatstream-0.1.2/chatstream/chat_prompt.py`

 * *Files identical despite different names*

### Comparing `ChatStream-0.1.1/chatstream/chat_stream.py` & `chatstream-0.1.2/chatstream/chat_stream.py`

 * *Files identical despite different names*

### Comparing `ChatStream-0.1.1/chatstream/mock_response_example_text.py` & `chatstream-0.1.2/chatstream/mock_response_example_text.py`

 * *Files identical despite different names*

### Comparing `ChatStream-0.1.1/chatstream/request_handler/request_handler.py` & `chatstream-0.1.2/chatstream/request_handler/request_handler.py`

 * *Files identical despite different names*

### Comparing `ChatStream-0.1.1/chatstream/request_handler/simple_session_request_handler.py` & `chatstream-0.1.2/chatstream/request_handler/simple_session_request_handler.py`

 * *Files identical despite different names*

### Comparing `ChatStream-0.1.1/chatstream/sampling_utils.py` & `chatstream-0.1.2/chatstream/sampling_utils.py`

 * *Files identical despite different names*

### Comparing `ChatStream-0.1.1/chatstream/util_request_id.py` & `chatstream-0.1.2/chatstream/util_request_id.py`

 * *Files identical despite different names*

### Comparing `ChatStream-0.1.1/setup.py` & `chatstream-0.1.2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
-    name="ChatStream",
-    version="0.1.1",
+    name="chatstream",
+    version="0.1.2",
     author="Tom Misawa",
     author_email="riversun.org@gmail.com",
     description="Streaming chat server building blocks for FastAPI/Starlette",
     long_description=open("README.md", "r").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/riversun/ChatStream",
     packages=find_packages(exclude=["tests.*", "tests", "examples.*", "examples"]),
@@ -18,13 +18,13 @@
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
     ],
     python_requires=">=3.8",
     install_requires=[
         "torch",
-        "transformers"
+        "transformers",
         "fastapi",
         "fastsession",
         "tokflow"
     ]
 )
```

