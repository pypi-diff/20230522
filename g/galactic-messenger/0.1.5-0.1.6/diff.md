# Comparing `tmp/galactic-messenger-0.1.5.tar.gz` & `tmp/galactic-messenger-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "galactic-messenger-0.1.5.tar", last modified: Mon May 22 03:46:27 2023, max compression
+gzip compressed data, was "galactic-messenger-0.1.6.tar", last modified: Mon May 22 03:49:03 2023, max compression
```

## Comparing `galactic-messenger-0.1.5.tar` & `galactic-messenger-0.1.6.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 akritworanithiphong   (501) staff       (20)        0 2023-05-22 03:46:27.379333 galactic-messenger-0.1.5/
--rw-r--r--   0 akritworanithiphong   (501) staff       (20)     1059 2023-05-19 03:05:50.000000 galactic-messenger-0.1.5/LICENSE
--rw-r--r--   0 akritworanithiphong   (501) staff       (20)      232 2023-05-19 04:30:41.000000 galactic-messenger-0.1.5/MANIFEST.in
--rw-r--r--   0 akritworanithiphong   (501) staff       (20)     5056 2023-05-22 03:46:27.379742 galactic-messenger-0.1.5/PKG-INFO
--rw-r--r--   0 akritworanithiphong   (501) staff       (20)     4322 2023-05-22 03:42:40.000000 galactic-messenger-0.1.5/README.md
-drwxr-xr-x   0 akritworanithiphong   (501) staff       (20)        0 2023-05-22 03:46:27.359256 galactic-messenger-0.1.5/galactic_messenger/
--rw-r--r--   0 akritworanithiphong   (501) staff       (20)      116 2023-05-19 04:47:42.000000 galactic-messenger-0.1.5/galactic_messenger/__init__.py
--rw-r--r--   0 akritworanithiphong   (501) staff       (20)      291 2023-05-19 02:56:12.000000 galactic-messenger-0.1.5/galactic_messenger/config.py
-drwxr-xr-x   0 akritworanithiphong   (501) staff       (20)        0 2023-05-22 03:46:27.372004 galactic-messenger-0.1.5/galactic_messenger/env/
--rw-r--r--   0 akritworanithiphong   (501) staff       (20)      564 2023-05-18 07:28:08.000000 galactic-messenger-0.1.5/galactic_messenger/env/env.py
-drwxr-xr-x   0 akritworanithiphong   (501) staff       (20)        0 2023-05-22 03:46:27.374374 galactic-messenger-0.1.5/galactic_messenger/src/
--rw-r--r--   0 akritworanithiphong   (501) staff       (20)     3312 2023-05-19 04:51:04.000000 galactic-messenger-0.1.5/galactic_messenger/src/mail.py
--rw-r--r--   0 akritworanithiphong   (501) staff       (20)     6307 2023-05-19 04:51:37.000000 galactic-messenger-0.1.5/galactic_messenger/src/telegram.py
--rw-r--r--   0 akritworanithiphong   (501) staff       (20)      476 2023-05-15 09:17:23.000000 galactic-messenger-0.1.5/galactic_messenger/src/utils.py
--rw-r--r--   0 akritworanithiphong   (501) staff       (20)     6278 2023-05-19 04:52:06.000000 galactic-messenger-0.1.5/galactic_messenger/src/whatsapp.py
-drwxr-xr-x   0 akritworanithiphong   (501) staff       (20)        0 2023-05-22 03:46:27.353228 galactic-messenger-0.1.5/galactic_messenger/tests/
-drwxr-xr-x   0 akritworanithiphong   (501) staff       (20)        0 2023-05-22 03:46:27.376414 galactic-messenger-0.1.5/galactic_messenger/tests/end_to_end/
--rw-r--r--   0 akritworanithiphong   (501) staff       (20)     4978 2023-05-19 04:52:42.000000 galactic-messenger-0.1.5/galactic_messenger/tests/end_to_end/test_mail.py
--rw-r--r--   0 akritworanithiphong   (501) staff       (20)     2144 2023-05-19 04:52:53.000000 galactic-messenger-0.1.5/galactic_messenger/tests/end_to_end/test_telegram.py
--rw-r--r--   0 akritworanithiphong   (501) staff       (20)     2141 2023-05-19 04:53:00.000000 galactic-messenger-0.1.5/galactic_messenger/tests/end_to_end/test_whatsapp.py
-drwxr-xr-x   0 akritworanithiphong   (501) staff       (20)        0 2023-05-22 03:46:27.378610 galactic-messenger-0.1.5/galactic_messenger/tests/unit/
--rw-r--r--   0 akritworanithiphong   (501) staff       (20)     3543 2023-05-19 04:53:09.000000 galactic-messenger-0.1.5/galactic_messenger/tests/unit/test_mail.py
--rw-r--r--   0 akritworanithiphong   (501) staff       (20)      496 2023-05-19 04:53:14.000000 galactic-messenger-0.1.5/galactic_messenger/tests/unit/test_utils.py
--rw-r--r--   0 akritworanithiphong   (501) staff       (20)     3030 2023-05-19 04:53:19.000000 galactic-messenger-0.1.5/galactic_messenger/tests/unit/test_whatsapp.py
-drwxr-xr-x   0 akritworanithiphong   (501) staff       (20)        0 2023-05-22 03:46:27.371436 galactic-messenger-0.1.5/galactic_messenger.egg-info/
--rw-r--r--   0 akritworanithiphong   (501) staff       (20)     5056 2023-05-22 03:46:27.000000 galactic-messenger-0.1.5/galactic_messenger.egg-info/PKG-INFO
--rw-r--r--   0 akritworanithiphong   (501) staff       (20)      801 2023-05-22 03:46:27.000000 galactic-messenger-0.1.5/galactic_messenger.egg-info/SOURCES.txt
--rw-r--r--   0 akritworanithiphong   (501) staff       (20)        1 2023-05-22 03:46:27.000000 galactic-messenger-0.1.5/galactic_messenger.egg-info/dependency_links.txt
--rw-r--r--   0 akritworanithiphong   (501) staff       (20)      391 2023-05-22 03:46:27.000000 galactic-messenger-0.1.5/galactic_messenger.egg-info/requires.txt
--rw-r--r--   0 akritworanithiphong   (501) staff       (20)       19 2023-05-22 03:46:27.000000 galactic-messenger-0.1.5/galactic_messenger.egg-info/top_level.txt
--rw-r--r--   0 akritworanithiphong   (501) staff       (20)      442 2023-05-12 09:46:57.000000 galactic-messenger-0.1.5/pyproject.toml
--rw-r--r--   0 akritworanithiphong   (501) staff       (20)      391 2023-05-19 03:07:47.000000 galactic-messenger-0.1.5/requirements.txt
--rw-r--r--   0 akritworanithiphong   (501) staff       (20)      495 2023-05-22 03:46:27.381737 galactic-messenger-0.1.5/setup.cfg
--rw-r--r--   0 akritworanithiphong   (501) staff       (20)      919 2023-05-22 03:46:23.000000 galactic-messenger-0.1.5/setup.py
+drwxr-xr-x   0 akritworanithiphong   (501) staff       (20)        0 2023-05-22 03:49:03.537693 galactic-messenger-0.1.6/
+-rw-r--r--   0 akritworanithiphong   (501) staff       (20)     1059 2023-05-19 03:05:50.000000 galactic-messenger-0.1.6/LICENSE
+-rw-r--r--   0 akritworanithiphong   (501) staff       (20)      232 2023-05-19 04:30:41.000000 galactic-messenger-0.1.6/MANIFEST.in
+-rw-r--r--   0 akritworanithiphong   (501) staff       (20)     5054 2023-05-22 03:49:03.538034 galactic-messenger-0.1.6/PKG-INFO
+-rw-r--r--   0 akritworanithiphong   (501) staff       (20)     4320 2023-05-22 03:48:36.000000 galactic-messenger-0.1.6/README.md
+drwxr-xr-x   0 akritworanithiphong   (501) staff       (20)        0 2023-05-22 03:49:03.519851 galactic-messenger-0.1.6/galactic_messenger/
+-rw-r--r--   0 akritworanithiphong   (501) staff       (20)      116 2023-05-19 04:47:42.000000 galactic-messenger-0.1.6/galactic_messenger/__init__.py
+-rw-r--r--   0 akritworanithiphong   (501) staff       (20)      291 2023-05-19 02:56:12.000000 galactic-messenger-0.1.6/galactic_messenger/config.py
+drwxr-xr-x   0 akritworanithiphong   (501) staff       (20)        0 2023-05-22 03:49:03.529967 galactic-messenger-0.1.6/galactic_messenger/env/
+-rw-r--r--   0 akritworanithiphong   (501) staff       (20)      564 2023-05-18 07:28:08.000000 galactic-messenger-0.1.6/galactic_messenger/env/env.py
+drwxr-xr-x   0 akritworanithiphong   (501) staff       (20)        0 2023-05-22 03:49:03.532739 galactic-messenger-0.1.6/galactic_messenger/src/
+-rw-r--r--   0 akritworanithiphong   (501) staff       (20)     3312 2023-05-19 04:51:04.000000 galactic-messenger-0.1.6/galactic_messenger/src/mail.py
+-rw-r--r--   0 akritworanithiphong   (501) staff       (20)     6307 2023-05-19 04:51:37.000000 galactic-messenger-0.1.6/galactic_messenger/src/telegram.py
+-rw-r--r--   0 akritworanithiphong   (501) staff       (20)      476 2023-05-15 09:17:23.000000 galactic-messenger-0.1.6/galactic_messenger/src/utils.py
+-rw-r--r--   0 akritworanithiphong   (501) staff       (20)     6278 2023-05-19 04:52:06.000000 galactic-messenger-0.1.6/galactic_messenger/src/whatsapp.py
+drwxr-xr-x   0 akritworanithiphong   (501) staff       (20)        0 2023-05-22 03:49:03.512932 galactic-messenger-0.1.6/galactic_messenger/tests/
+drwxr-xr-x   0 akritworanithiphong   (501) staff       (20)        0 2023-05-22 03:49:03.534964 galactic-messenger-0.1.6/galactic_messenger/tests/end_to_end/
+-rw-r--r--   0 akritworanithiphong   (501) staff       (20)     4978 2023-05-19 04:52:42.000000 galactic-messenger-0.1.6/galactic_messenger/tests/end_to_end/test_mail.py
+-rw-r--r--   0 akritworanithiphong   (501) staff       (20)     2144 2023-05-19 04:52:53.000000 galactic-messenger-0.1.6/galactic_messenger/tests/end_to_end/test_telegram.py
+-rw-r--r--   0 akritworanithiphong   (501) staff       (20)     2141 2023-05-19 04:53:00.000000 galactic-messenger-0.1.6/galactic_messenger/tests/end_to_end/test_whatsapp.py
+drwxr-xr-x   0 akritworanithiphong   (501) staff       (20)        0 2023-05-22 03:49:03.537107 galactic-messenger-0.1.6/galactic_messenger/tests/unit/
+-rw-r--r--   0 akritworanithiphong   (501) staff       (20)     3543 2023-05-19 04:53:09.000000 galactic-messenger-0.1.6/galactic_messenger/tests/unit/test_mail.py
+-rw-r--r--   0 akritworanithiphong   (501) staff       (20)      496 2023-05-19 04:53:14.000000 galactic-messenger-0.1.6/galactic_messenger/tests/unit/test_utils.py
+-rw-r--r--   0 akritworanithiphong   (501) staff       (20)     3030 2023-05-19 04:53:19.000000 galactic-messenger-0.1.6/galactic_messenger/tests/unit/test_whatsapp.py
+drwxr-xr-x   0 akritworanithiphong   (501) staff       (20)        0 2023-05-22 03:49:03.529235 galactic-messenger-0.1.6/galactic_messenger.egg-info/
+-rw-r--r--   0 akritworanithiphong   (501) staff       (20)     5054 2023-05-22 03:49:03.000000 galactic-messenger-0.1.6/galactic_messenger.egg-info/PKG-INFO
+-rw-r--r--   0 akritworanithiphong   (501) staff       (20)      801 2023-05-22 03:49:03.000000 galactic-messenger-0.1.6/galactic_messenger.egg-info/SOURCES.txt
+-rw-r--r--   0 akritworanithiphong   (501) staff       (20)        1 2023-05-22 03:49:03.000000 galactic-messenger-0.1.6/galactic_messenger.egg-info/dependency_links.txt
+-rw-r--r--   0 akritworanithiphong   (501) staff       (20)      391 2023-05-22 03:49:03.000000 galactic-messenger-0.1.6/galactic_messenger.egg-info/requires.txt
+-rw-r--r--   0 akritworanithiphong   (501) staff       (20)       19 2023-05-22 03:49:03.000000 galactic-messenger-0.1.6/galactic_messenger.egg-info/top_level.txt
+-rw-r--r--   0 akritworanithiphong   (501) staff       (20)      442 2023-05-12 09:46:57.000000 galactic-messenger-0.1.6/pyproject.toml
+-rw-r--r--   0 akritworanithiphong   (501) staff       (20)      391 2023-05-19 03:07:47.000000 galactic-messenger-0.1.6/requirements.txt
+-rw-r--r--   0 akritworanithiphong   (501) staff       (20)      495 2023-05-22 03:49:03.540048 galactic-messenger-0.1.6/setup.cfg
+-rw-r--r--   0 akritworanithiphong   (501) staff       (20)      919 2023-05-22 03:48:00.000000 galactic-messenger-0.1.6/setup.py
```

### Comparing `galactic-messenger-0.1.5/LICENSE` & `galactic-messenger-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `galactic-messenger-0.1.5/PKG-INFO` & `galactic-messenger-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: galactic-messenger
-Version: 0.1.5
+Version: 0.1.6
 Summary: Galactic Messenger is a versatile and efficient Python package designed for sending messages across multiple platforms.
 Home-page: https://github.com/Invigilo-AI/Galactic-Messenger
 Author: InvigiloAI
 Author-email: contact@invigilo.ai
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -88,15 +88,14 @@
 
 Galactic Messenger seamlessly handles batch requests, allowing you to send multiple messages simultaneously. You can provide an array of messages to the sender functions for efficient batch processing.
 
 ```python
 async def main():
     # Sending multiple Telegram messages in a batch
     telegram_sender = setup_telegram("your_telegram_token")
-
     await telegram_sender(
         [
             {
                 "chatId": "chat_id_1",
                 "text": "Message 1",
             },
             {
@@ -110,15 +109,14 @@
                 "videoBytes": open("./video.png", "rb").read(),
             },
         ]
     )
 
     # Sending multiple WhatsApp messages in a batch
     whatsapp_sender = setup_whatsapp("http://your-whatsapp-api-endpoint")
-
     await whatsapp_sender(
         [
             {
                 "chatId": "chat_id_1",
                 "text": "Message 1",
             },
             {
```

### Comparing `galactic-messenger-0.1.5/README.md` & `galactic-messenger-0.1.6/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -70,15 +70,14 @@
 
 Galactic Messenger seamlessly handles batch requests, allowing you to send multiple messages simultaneously. You can provide an array of messages to the sender functions for efficient batch processing.
 
 ```python
 async def main():
     # Sending multiple Telegram messages in a batch
     telegram_sender = setup_telegram("your_telegram_token")
-
     await telegram_sender(
         [
             {
                 "chatId": "chat_id_1",
                 "text": "Message 1",
             },
             {
@@ -92,15 +91,14 @@
                 "videoBytes": open("./video.png", "rb").read(),
             },
         ]
     )
 
     # Sending multiple WhatsApp messages in a batch
     whatsapp_sender = setup_whatsapp("http://your-whatsapp-api-endpoint")
-
     await whatsapp_sender(
         [
             {
                 "chatId": "chat_id_1",
                 "text": "Message 1",
             },
             {
```

### Comparing `galactic-messenger-0.1.5/galactic_messenger/env/env.py` & `galactic-messenger-0.1.6/galactic_messenger/env/env.py`

 * *Files identical despite different names*

### Comparing `galactic-messenger-0.1.5/galactic_messenger/src/mail.py` & `galactic-messenger-0.1.6/galactic_messenger/src/mail.py`

 * *Files identical despite different names*

### Comparing `galactic-messenger-0.1.5/galactic_messenger/src/telegram.py` & `galactic-messenger-0.1.6/galactic_messenger/src/telegram.py`

 * *Files identical despite different names*

### Comparing `galactic-messenger-0.1.5/galactic_messenger/src/whatsapp.py` & `galactic-messenger-0.1.6/galactic_messenger/src/whatsapp.py`

 * *Files identical despite different names*

### Comparing `galactic-messenger-0.1.5/galactic_messenger/tests/end_to_end/test_mail.py` & `galactic-messenger-0.1.6/galactic_messenger/tests/end_to_end/test_mail.py`

 * *Files identical despite different names*

### Comparing `galactic-messenger-0.1.5/galactic_messenger/tests/end_to_end/test_telegram.py` & `galactic-messenger-0.1.6/galactic_messenger/tests/end_to_end/test_telegram.py`

 * *Files identical despite different names*

### Comparing `galactic-messenger-0.1.5/galactic_messenger/tests/end_to_end/test_whatsapp.py` & `galactic-messenger-0.1.6/galactic_messenger/tests/end_to_end/test_whatsapp.py`

 * *Files identical despite different names*

### Comparing `galactic-messenger-0.1.5/galactic_messenger/tests/unit/test_mail.py` & `galactic-messenger-0.1.6/galactic_messenger/tests/unit/test_mail.py`

 * *Files identical despite different names*

### Comparing `galactic-messenger-0.1.5/galactic_messenger/tests/unit/test_whatsapp.py` & `galactic-messenger-0.1.6/galactic_messenger/tests/unit/test_whatsapp.py`

 * *Files identical despite different names*

### Comparing `galactic-messenger-0.1.5/galactic_messenger.egg-info/PKG-INFO` & `galactic-messenger-0.1.6/galactic_messenger.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: galactic-messenger
-Version: 0.1.5
+Version: 0.1.6
 Summary: Galactic Messenger is a versatile and efficient Python package designed for sending messages across multiple platforms.
 Home-page: https://github.com/Invigilo-AI/Galactic-Messenger
 Author: InvigiloAI
 Author-email: contact@invigilo.ai
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -88,15 +88,14 @@
 
 Galactic Messenger seamlessly handles batch requests, allowing you to send multiple messages simultaneously. You can provide an array of messages to the sender functions for efficient batch processing.
 
 ```python
 async def main():
     # Sending multiple Telegram messages in a batch
     telegram_sender = setup_telegram("your_telegram_token")
-
     await telegram_sender(
         [
             {
                 "chatId": "chat_id_1",
                 "text": "Message 1",
             },
             {
@@ -110,15 +109,14 @@
                 "videoBytes": open("./video.png", "rb").read(),
             },
         ]
     )
 
     # Sending multiple WhatsApp messages in a batch
     whatsapp_sender = setup_whatsapp("http://your-whatsapp-api-endpoint")
-
     await whatsapp_sender(
         [
             {
                 "chatId": "chat_id_1",
                 "text": "Message 1",
             },
             {
```

### Comparing `galactic-messenger-0.1.5/galactic_messenger.egg-info/SOURCES.txt` & `galactic-messenger-0.1.6/galactic_messenger.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `galactic-messenger-0.1.5/setup.py` & `galactic-messenger-0.1.6/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name="galactic-messenger",
-    version="0.1.5",
+    version="0.1.6",
     author="InvigiloAI",
     author_email="contact@invigilo.ai",
     description="Galactic Messenger is a versatile and efficient Python package designed for sending messages across multiple platforms.",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/Invigilo-AI/Galactic-Messenger",
     packages=find_packages(),
```

