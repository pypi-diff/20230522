# Comparing `tmp/rick-mailer-1.0.0.tar.gz` & `tmp/rick-mailer-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rick-mailer-1.0.0.tar", last modified: Fri Nov 25 18:23:31 2022, max compression
+gzip compressed data, was "rick-mailer-1.0.1.tar", last modified: Mon May 22 07:45:12 2023, max compression
```

## Comparing `rick-mailer-1.0.0.tar` & `rick-mailer-1.0.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxr-x   0 jpinheiro  (1000) jpinheiro  (1000)        0 2022-11-25 18:23:31.476595 rick-mailer-1.0.0/
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     1552 2022-11-24 13:47:35.000000 rick-mailer-1.0.0/LICENSE
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     2297 2022-11-25 18:23:31.476595 rick-mailer-1.0.0/PKG-INFO
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     1247 2022-11-25 18:21:42.000000 rick-mailer-1.0.0/README.md
-drwxrwxr-x   0 jpinheiro  (1000) jpinheiro  (1000)        0 2022-11-25 18:23:31.472595 rick-mailer-1.0.0/rick_mailer/
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     2106 2022-11-25 17:46:52.000000 rick-mailer-1.0.0/rick_mailer/__init__.py
-drwxrwxr-x   0 jpinheiro  (1000) jpinheiro  (1000)        0 2022-11-25 18:23:31.472595 rick-mailer-1.0.0/rick_mailer/backends/
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)      833 2022-11-25 18:06:25.000000 rick-mailer-1.0.0/rick_mailer/backends/__init__.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     1764 2022-11-25 16:14:41.000000 rick-mailer-1.0.0/rick_mailer/backends/base.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     1448 2022-11-25 16:14:41.000000 rick-mailer-1.0.0/rick_mailer/backends/console.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)      909 2022-11-25 16:14:41.000000 rick-mailer-1.0.0/rick_mailer/backends/locmem.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     5077 2022-11-25 16:14:41.000000 rick-mailer-1.0.0/rick_mailer/backends/smtp.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)    17667 2022-11-25 16:14:41.000000 rick-mailer-1.0.0/rick_mailer/message.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     1669 2022-11-25 16:14:41.000000 rick-mailer-1.0.0/rick_mailer/utils.py
-drwxrwxr-x   0 jpinheiro  (1000) jpinheiro  (1000)        0 2022-11-25 18:23:31.472595 rick-mailer-1.0.0/rick_mailer.egg-info/
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     2297 2022-11-25 18:23:31.000000 rick-mailer-1.0.0/rick_mailer.egg-info/PKG-INFO
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)      567 2022-11-25 18:23:31.000000 rick-mailer-1.0.0/rick_mailer.egg-info/SOURCES.txt
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)        1 2022-11-25 18:23:31.000000 rick-mailer-1.0.0/rick_mailer.egg-info/dependency_links.txt
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)        1 2022-11-25 16:33:18.000000 rick-mailer-1.0.0/rick_mailer.egg-info/not-zip-safe
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)       12 2022-11-25 18:23:31.000000 rick-mailer-1.0.0/rick_mailer.egg-info/requires.txt
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)       18 2022-11-25 18:23:31.000000 rick-mailer-1.0.0/rick_mailer.egg-info/top_level.txt
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     1209 2022-11-25 18:23:31.476595 rick-mailer-1.0.0/setup.cfg
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)       38 2022-11-25 16:07:53.000000 rick-mailer-1.0.0/setup.py
-drwxrwxr-x   0 jpinheiro  (1000) jpinheiro  (1000)        0 2022-11-25 18:23:31.472595 rick-mailer-1.0.0/tests/
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)       39 2022-11-25 12:52:37.000000 rick-mailer-1.0.0/tests/__init__.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)      591 2022-11-25 13:24:15.000000 rick-mailer-1.0.0/tests/common.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)      476 2022-11-25 13:03:04.000000 rick-mailer-1.0.0/tests/custombackend.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)    19977 2022-11-25 18:07:29.000000 rick-mailer-1.0.0/tests/test_backends.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)    38354 2022-11-25 13:26:35.000000 rick-mailer-1.0.0/tests/test_mailer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 07:45:12.008975 rick-mailer-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-05-22 07:44:52.000000 rick-mailer-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-05-22 07:45:12.008975 rick-mailer-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-05-22 07:44:52.000000 rick-mailer-1.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 07:45:12.004975 rick-mailer-1.0.1/rick_mailer/
+-rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-05-22 07:44:52.000000 rick-mailer-1.0.1/rick_mailer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 07:45:12.004975 rick-mailer-1.0.1/rick_mailer/backends/
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-05-22 07:44:52.000000 rick-mailer-1.0.1/rick_mailer/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-05-22 07:44:52.000000 rick-mailer-1.0.1/rick_mailer/backends/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-05-22 07:44:52.000000 rick-mailer-1.0.1/rick_mailer/backends/console.py
+-rw-r--r--   0 runner    (1001) docker     (123)      909 2023-05-22 07:44:52.000000 rick-mailer-1.0.1/rick_mailer/backends/locmem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5077 2023-05-22 07:44:52.000000 rick-mailer-1.0.1/rick_mailer/backends/smtp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17667 2023-05-22 07:44:52.000000 rick-mailer-1.0.1/rick_mailer/message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-05-22 07:44:52.000000 rick-mailer-1.0.1/rick_mailer/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 07:45:12.004975 rick-mailer-1.0.1/rick_mailer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-05-22 07:45:11.000000 rick-mailer-1.0.1/rick_mailer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-05-22 07:45:11.000000 rick-mailer-1.0.1/rick_mailer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 07:45:11.000000 rick-mailer-1.0.1/rick_mailer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 07:45:11.000000 rick-mailer-1.0.1/rick_mailer.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-22 07:45:11.000000 rick-mailer-1.0.1/rick_mailer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-22 07:45:11.000000 rick-mailer-1.0.1/rick_mailer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-05-22 07:45:12.008975 rick-mailer-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 07:44:52.000000 rick-mailer-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 07:45:12.008975 rick-mailer-1.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-22 07:44:52.000000 rick-mailer-1.0.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-05-22 07:44:52.000000 rick-mailer-1.0.1/tests/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-05-22 07:44:52.000000 rick-mailer-1.0.1/tests/custombackend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20071 2023-05-22 07:44:52.000000 rick-mailer-1.0.1/tests/test_backends.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38249 2023-05-22 07:44:52.000000 rick-mailer-1.0.1/tests/test_mailer.py
```

### Comparing `rick-mailer-1.0.0/LICENSE` & `rick-mailer-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `rick-mailer-1.0.0/PKG-INFO` & `rick-mailer-1.0.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: rick-mailer
-Version: 1.0.0
+Version: 1.0.1
 Summary: Simple library to send emails
-Home-page: https://github.com/oddbit-project/rick-mailer
+Home-page: https://git.oddbit.org/OddBit/rick-mailer
 Author: João Pinheiro
 License: BSD-3-Clause
-Project-URL: Documentation, https://oddbit-project.github.io/rick-mailer/
-Project-URL: Source, https://github.com/oddbit-project/rick-mailer
-Platform: UNKNOWN
+Project-URL: Documentation, https://docs.oddbit.org/rick-mailer/
+Project-URL: Source, https://git.oddbit.org/OddBit/rick-mailer
 Classifier: Environment :: Web Environment
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
@@ -20,23 +19,22 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# Rick-mailer - SMTP Client
-
+# Rick-mailer - Library to send emails 
 
 [![Tests](https://github.com/oddbit-project/rick-mailer/workflows/Tests/badge.svg?branch=master)](https://github.com/oddbit-project/rick-mailer/actions)
 [![pypi](https://img.shields.io/pypi/v/rick-mailer.svg)](https://pypi.org/project/rick-mailer/)
 [![license](https://img.shields.io/pypi/l/rick-mailer.svg)](https://github.com/oddbit-project/rick-mailer/blob/master/LICENSE)
 
 
-rick_mailer is a standalone version of Django's email client implementation, with minor changes. 
+rick_mailer is a standalone version of Django's email library implementation, with minor changes.
 
 ## Installation
 
 ```shell
 $ pip3 install rick-mailer
 ```
 
@@ -61,9 +59,7 @@
 
 ## Related tools
 
 Check out [MailHog](https://github.com/mailhog/MailHog), a mail testing tool for developers.
 
 ## License
 As rick_mailer is mostly Django code, it is licensed under Django license and copyright - see the included [License file](LICENSE).
-
-
```

### Comparing `rick-mailer-1.0.0/README.md` & `rick-mailer-1.0.1/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,15 @@
-# Rick-mailer - SMTP Client
-
+# Rick-mailer - Library to send emails 
 
 [![Tests](https://github.com/oddbit-project/rick-mailer/workflows/Tests/badge.svg?branch=master)](https://github.com/oddbit-project/rick-mailer/actions)
 [![pypi](https://img.shields.io/pypi/v/rick-mailer.svg)](https://pypi.org/project/rick-mailer/)
 [![license](https://img.shields.io/pypi/l/rick-mailer.svg)](https://github.com/oddbit-project/rick-mailer/blob/master/LICENSE)
 
 
-rick_mailer is a standalone version of Django's email client implementation, with minor changes. 
+rick_mailer is a standalone version of Django's email library implementation, with minor changes.
 
 ## Installation
 
 ```shell
 $ pip3 install rick-mailer
 ```
```

### Comparing `rick-mailer-1.0.0/rick_mailer/__init__.py` & `rick-mailer-1.0.1/rick_mailer/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,24 +24,24 @@
     "SafeMIMEMultipart",
     "DEFAULT_ATTACHMENT_MIME_TYPE",
     "make_msgid",
     "BadHeaderError",
     "forbid_multi_line_headers",
     "Mailer",
     "SMTPFactory",
-    "Mailer"
+    "Mailer",
 ]
 
 
 class Mailer:
     def __init__(self, backend: BaseEmailBackend):
         self.backend = backend
 
     def send_mail(
-            self, subject, message, from_email, recipient_list, html_message=None
+        self, subject, message, from_email, recipient_list, html_message=None
     ):
         """
         Easy wrapper for sending a single message to a recipient list. All members
         of the recipient list will see the other recipients in the 'To' field.
 
         If from_email is None, use the DEFAULT_FROM_EMAIL setting.
         If auth_user is None, use the EMAIL_HOST_USER setting.
```

### Comparing `rick-mailer-1.0.0/rick_mailer/backends/__init__.py` & `rick-mailer-1.0.1/rick_mailer/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `rick-mailer-1.0.0/rick_mailer/backends/base.py` & `rick-mailer-1.0.1/rick_mailer/backends/base.py`

 * *Files identical despite different names*

### Comparing `rick-mailer-1.0.0/rick_mailer/backends/console.py` & `rick-mailer-1.0.1/rick_mailer/backends/console.py`

 * *Files identical despite different names*

### Comparing `rick-mailer-1.0.0/rick_mailer/backends/locmem.py` & `rick-mailer-1.0.1/rick_mailer/backends/locmem.py`

 * *Files identical despite different names*

### Comparing `rick-mailer-1.0.0/rick_mailer/backends/smtp.py` & `rick-mailer-1.0.1/rick_mailer/backends/smtp.py`

 * *Files identical despite different names*

### Comparing `rick-mailer-1.0.0/rick_mailer/message.py` & `rick-mailer-1.0.1/rick_mailer/message.py`

 * *Files identical despite different names*

### Comparing `rick-mailer-1.0.0/rick_mailer/utils.py` & `rick-mailer-1.0.1/rick_mailer/utils.py`

 * *Files identical despite different names*

### Comparing `rick-mailer-1.0.0/rick_mailer.egg-info/PKG-INFO` & `rick-mailer-1.0.1/rick_mailer.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: rick-mailer
-Version: 1.0.0
+Version: 1.0.1
 Summary: Simple library to send emails
-Home-page: https://github.com/oddbit-project/rick-mailer
+Home-page: https://git.oddbit.org/OddBit/rick-mailer
 Author: João Pinheiro
 License: BSD-3-Clause
-Project-URL: Documentation, https://oddbit-project.github.io/rick-mailer/
-Project-URL: Source, https://github.com/oddbit-project/rick-mailer
-Platform: UNKNOWN
+Project-URL: Documentation, https://docs.oddbit.org/rick-mailer/
+Project-URL: Source, https://git.oddbit.org/OddBit/rick-mailer
 Classifier: Environment :: Web Environment
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
@@ -20,23 +19,22 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# Rick-mailer - SMTP Client
-
+# Rick-mailer - Library to send emails 
 
 [![Tests](https://github.com/oddbit-project/rick-mailer/workflows/Tests/badge.svg?branch=master)](https://github.com/oddbit-project/rick-mailer/actions)
 [![pypi](https://img.shields.io/pypi/v/rick-mailer.svg)](https://pypi.org/project/rick-mailer/)
 [![license](https://img.shields.io/pypi/l/rick-mailer.svg)](https://github.com/oddbit-project/rick-mailer/blob/master/LICENSE)
 
 
-rick_mailer is a standalone version of Django's email client implementation, with minor changes. 
+rick_mailer is a standalone version of Django's email library implementation, with minor changes.
 
 ## Installation
 
 ```shell
 $ pip3 install rick-mailer
 ```
 
@@ -61,9 +59,7 @@
 
 ## Related tools
 
 Check out [MailHog](https://github.com/mailhog/MailHog), a mail testing tool for developers.
 
 ## License
 As rick_mailer is mostly Django code, it is licensed under Django license and copyright - see the included [License file](LICENSE).
-
-
```

### Comparing `rick-mailer-1.0.0/rick_mailer.egg-info/SOURCES.txt` & `rick-mailer-1.0.1/rick_mailer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rick-mailer-1.0.0/setup.cfg` & `rick-mailer-1.0.1/setup.cfg`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [metadata]
 name = rick-mailer
-version = 1.0.0
-url = https://github.com/oddbit-project/rick-mailer
+version = 1.0.1
+url = https://git.oddbit.org/OddBit/rick-mailer
 author = João Pinheiro
 description = Simple library to send emails
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = BSD-3-Clause
 classifiers = 
 	Environment :: Web Environment
@@ -17,24 +17,24 @@
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
 	Topic :: Internet :: WWW/HTTP :: Dynamic Content
 	Topic :: Software Development :: Libraries :: Python Modules
 project_urls = 
-	Documentation = https://oddbit-project.github.io/rick-mailer/
-	Source = https://github.com/oddbit-project/rick-mailer
+	Documentation = https://docs.oddbit.org/rick-mailer/
+	Source = https://git.oddbit.org/OddBit/rick-mailer
 
 [options]
 python_requires = >=3.8
 packages = find:
 include_package_data = true
 zip_safe = false
 install_requires = 
-	rick~=0.4.6
+	rick>=0.4.6
 
 [bdist_rpm]
 doc_files = docs README.md
 
 [flake8]
 exclude = dist,build,.git,.tox,./tests/
 extend-ignore = E501, W504 ,F401
```

### Comparing `rick-mailer-1.0.0/tests/common.py` & `rick-mailer-1.0.1/tests/common.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from email import message_from_bytes
 
 
 class HeadersCheckMixin:
-
     def assertMessageHasHeaders(self, message, headers):
         """
         Asserts that the `message` has all `headers`.
 
         message: can be an instance of an email.Message subclass or a string
                  with the contents of an email message.
         headers: should be a set of (header-name, header-value) tuples.
```

### Comparing `rick-mailer-1.0.0/tests/test_backends.py` & `rick-mailer-1.0.1/tests/test_backends.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 from rick_mailer.backends import SMTPEmailBackend
 from rick_mailer.backends import registry, SMTPFactory
 from rick_mailer import EmailMessage, Mailer, BadHeaderError
 from tests.common import HeadersCheckMixin
 
 
 class BaseBackendTest(HeadersCheckMixin):
-
     def setup_method(self, test_method):
         self.email_backend = None
 
     def teardown_method(self, test_method):
         pass
 
     def assertStartsWith(self, first, second):
@@ -96,42 +95,47 @@
         )
         email2 = EmailMessage(
             "Subject", "Content2", "from@example.com", ["to@example.com"]
         )
         # send_messages() may take a list or an iterator.
         emails_lists = ([email1, email2], iter((email1, email2)))
         for emails_list in emails_lists:
+            self.flush_mailbox()
             num_sent = self.email_backend.send_messages(emails_list)
             assert num_sent == 2
-            messages = self.get_mailbox_content()
-            assert len(messages) == 2
-            assert messages[0].get_payload() == "Content1"
-            assert messages[1].get_payload() == "Content2"
+            msgs = self.get_mailbox_content()
+            assert len(msgs) == 2
+            assert msgs[0].get_payload() == "Content1"
+            assert msgs[1].get_payload() == "Content2"
             self.flush_mailbox()
 
     def test_send_verbose_name(self):
         email = EmailMessage(
             "Subject",
             "Content",
             '"Firstname Sürname" <from@example.com>',
             ["to@example.com"],
         )
         email.send(self.email_backend)
         message = self.get_the_message()
         assert message["subject"] == "Subject"
         assert message.get_payload() == "Content"
-        assert message["from"] == "=?utf-8?q?Firstname_S=C3=BCrname?= <from@example.com>"
+        assert (
+            message["from"] == "=?utf-8?q?Firstname_S=C3=BCrname?= <from@example.com>"
+        )
 
     def test_plaintext_send_mail(self):
         """
         Test send_mail without the html_message
         regression test for adding html_message parameter to send_mail()
         """
         mailer = Mailer(self.email_backend)
-        mailer.send_mail("Subject", "Content", "sender@example.com", ["nobody@example.com"])
+        mailer.send_mail(
+            "Subject", "Content", "sender@example.com", ["nobody@example.com"]
+        )
         message = self.get_the_message()
 
         assert message.get("subject") == "Subject"
         assert message.get_all("to") == ["nobody@example.com"]
         assert message.is_multipart() is False
         assert message.get_payload() == "Content"
         assert message.get_content_type() == "text/plain"
@@ -185,15 +189,17 @@
         assert message.as_string().find("\nDate: ") != -1
 
     def test_idn_send(self):
         """
         Regression test for #14301
         """
         mailer = Mailer(self.email_backend)
-        assert mailer.send_mail("Subject", "Content", "from@öäü.com", ["to@öäü.com"]) == 1
+        assert (
+            mailer.send_mail("Subject", "Content", "from@öäü.com", ["to@öäü.com"]) == 1
+        )
         message = self.get_the_message()
         assert message.get("subject") == "Subject"
         assert message.get("from") == "from@xn--4ca9at.com"
         assert message.get("to") == "to@xn--4ca9at.com"
 
         self.flush_mailbox()
         m = EmailMessage(
@@ -249,31 +255,31 @@
         assert closed[0] is True
 
 
 class TestMemBackend(BaseBackendTest):
     email_backend = None
 
     def setup_method(self, test_method):
-        self.email_backend = registry.get('mem')()
+        self.email_backend = registry.get("mem")()
 
     def teardown_method(self, test_method):
         self.flush_mailbox()
 
     def get_mailbox_content(self):
         return [m.message() for m in rick_mailer.outbox]
 
     def flush_mailbox(self):
         rick_mailer.outbox = []
 
     def test_locmem_shared_messages(self):
         """
         Make sure that the locmen backend populates the outbox.
         """
-        connection = registry.get('mem')()
-        connection2 = registry.get('mem')()
+        connection = registry.get("mem")()
+        connection2 = registry.get("mem")()
         email = EmailMessage(
             "Subject",
             "Content",
             "bounce@example.com",
             ["to@example.com"],
             headers={"From": "from@example.com"},
         )
@@ -287,44 +293,43 @@
         with pytest.raises(BadHeaderError):
             mailer.send_mail(
                 "Subject\nMultiline", "Content", "from@example.com", ["to@example.com"]
             )
 
 
 class TestConsoleBackend(BaseBackendTest):
-
     def setup_method(self, test_method):
         self.__stdout = sys.stdout
         self.stream = sys.stdout = StringIO()
-        self.email_backend = registry.get('console')()
+        self.email_backend = registry.get("console")()
 
     def teardown_method(self, test_method):
         sys.stdout = self.__stdout
         del self.__stdout
         self.flush_mailbox()
 
     def flush_mailbox(self):
+        self.stream.truncate(0)
         self.stream.seek(0)
 
     def get_mailbox_content(self):
         messages = self.stream.getvalue().split("\n" + ("-" * 79) + "\n")
-        return [message_from_bytes(m.encode()) for m in messages if m]
+        result = []
+        for m in messages:
+            if len(m) > 0:
+                result.append(message_from_bytes(m.encode()))
+        return result
 
     def test_console_stream_kwarg(self):
         """
         The console backend can be pointed at an arbitrary stream.
         """
         s = StringIO()
-        mailer = Mailer(registry.get('console')(stream=s))
-        mailer.send_mail(
-            "Subject",
-            "Content",
-            "from@example.com",
-            ["to@example.com"]
-        )
+        mailer = Mailer(registry.get("console")(stream=s))
+        mailer.send_mail("Subject", "Content", "from@example.com", ["to@example.com"])
         message = s.getvalue().split("\n" + ("-" * 79) + "\n")[0].encode()
         self.assertMessageHasHeaders(
             message,
             {
                 ("MIME-Version", "1.0"),
                 ("Content-Type", 'text/plain; charset="utf-8"'),
                 ("Content-Transfer-Encoding", "7bit"),
@@ -360,37 +365,32 @@
         return "250 OK"
 
     def flush_mailbox(self):
         self.mailbox[:] = []
 
 
 class BaseSMTPBackendTest(BaseBackendTest):
-
     def setup_method(self, test_method):
         with socket.socket() as s:
             s.bind(("127.0.0.1", 0))
             port = s.getsockname()[1]
         self.smtp_handler = SMTPHandler()
         self.smtp_controller = Controller(
             self.smtp_handler,
             hostname="127.0.0.1",
             port=port,
         )
-        self.config = {
-                'smtp_host': '127.0.0.1',
-                'smtp_port': port
-            }
+        self.config = {"smtp_host": "127.0.0.1", "smtp_port": port}
         self.smtp_controller.start()
 
     def teardown_method(self, test_method):
         self.smtp_controller.stop()
 
 
 class TestSMTPBackend(BaseSMTPBackendTest):
-
     def setup_method(self, test_method):
         super().setup_method(test_method)
         self.smtp_handler.flush_mailbox()
         self.email_backend = SMTPFactory(self.config)
 
     def teardown_method(self, test_method):
         self.smtp_handler.flush_mailbox()
@@ -400,16 +400,16 @@
         self.smtp_handler.flush_mailbox()
 
     def get_mailbox_content(self):
         return self.smtp_handler.mailbox
 
     def test_email_authentication_use_settings(self):
         cfg = self.config
-        cfg['smtp_username'] = "not empty username"
-        cfg['smtp_password'] = "not empty password"
+        cfg["smtp_username"] = "not empty username"
+        cfg["smtp_password"] = "not empty password"
 
         backend = SMTPFactory(cfg)
         assert backend.username == "not empty username"
         assert backend.password == "not empty password"
 
     def test_email_disabled_authentication(self):
         backend = SMTPFactory(self.config)
@@ -418,16 +418,16 @@
 
     def test_auth_attempted(self):
         """
         Opening the backend with non empty username/password tries
         to authenticate against the SMTP server.
         """
         cfg = self.config
-        cfg['smtp_username'] = "not empty username"
-        cfg['smtp_password'] = "not empty password"
+        cfg["smtp_username"] = "not empty username"
+        cfg["smtp_password"] = "not empty password"
         backend = SMTPFactory(cfg)
         with pytest.raises(SMTPException):
             with backend:
                 pass
 
     def test_server_open(self):
         """
@@ -442,101 +442,100 @@
         backend = SMTPFactory(self.config)
         # Simulate an already open connection.
         backend.connection = True
         assert backend.open() is False
 
     def test_email_tls_use_settings(self):
         cfg = self.config
-        cfg['smtp_use_tls'] = True
+        cfg["smtp_use_tls"] = True
         backend = SMTPFactory(cfg)
         assert backend.use_tls is True
 
     def test_email_tls_override_settings(self):
         cfg = self.config
-        cfg['smtp_use_tls'] = False
+        cfg["smtp_use_tls"] = False
         backend = SMTPFactory(cfg)
         assert backend.use_tls is False
 
     def test_email_tls_default_disabled(self):
         backend = SMTPFactory(self.config)
         assert backend.use_tls is False
 
     def test_ssl_tls_mutually_exclusive(self):
         with pytest.raises(ValueError):
             cfg = self.config
-            cfg['smtp_use_ssl'] = True
-            cfg['smtp_use_tls'] = True
+            cfg["smtp_use_ssl"] = True
+            cfg["smtp_use_tls"] = True
             backend = SMTPFactory(cfg)
 
     def test_email_ssl_use_settings(self):
         cfg = self.config
-        cfg['smtp_use_ssl'] = True
+        cfg["smtp_use_ssl"] = True
         backend = SMTPFactory(cfg)
         assert backend.use_ssl is True
 
     def test_email_ssl_override_settings(self):
         cfg = self.config
-        cfg['smtp_use_ssl'] = False
+        cfg["smtp_use_ssl"] = False
         backend = SMTPFactory(cfg)
         assert backend.use_ssl is False
 
     def test_email_ssl_default_disabled(self):
         backend = SMTPFactory(self.config)
         assert backend.use_ssl is False
 
     def test_email_ssl_certfile_use_settings(self):
         cfg = self.config
-        cfg['smtp_ssl_certfile'] = 'foo'
+        cfg["smtp_ssl_certfile"] = "foo"
         backend = SMTPFactory(cfg)
-        assert backend.ssl_certfile == 'foo'
+        assert backend.ssl_certfile == "foo"
 
     def test_email_ssl_certfile_default_disabled(self):
         backend = SMTPFactory(self.config)
         assert backend.ssl_certfile is None
 
     def test_email_ssl_keyfile_use_settings(self):
         cfg = self.config
-        cfg['smtp_ssl_keyfile'] = 'foo'
+        cfg["smtp_ssl_keyfile"] = "foo"
         backend = SMTPFactory(cfg)
-        assert backend.ssl_keyfile == 'foo'
+        assert backend.ssl_keyfile == "foo"
 
     def test_email_ssl_keyfile_default_disabled(self):
         backend = SMTPFactory(self.config)
         assert backend.ssl_keyfile is None
 
     def test_email_tls_attempts_starttls(self):
         cfg = self.config
-        cfg['smtp_use_tls'] = True
+        cfg["smtp_use_tls"] = True
         backend = SMTPFactory(cfg)
         assert backend.use_tls is True
         with pytest.raises(SMTPException):
             with backend:
                 pass
 
     def test_email_ssl_attempts_ssl_connection(self):
         cfg = self.config
-        cfg['smtp_use_ssl'] = True
+        cfg["smtp_use_ssl"] = True
         backend = SMTPFactory(cfg)
         assert backend.use_ssl is True
         with pytest.raises(SSLError):
             with backend:
                 pass
 
     def test_connection_timeout_default(self):
         backend = SMTPFactory(self.config)
         assert backend.timeout is None
 
     def test_connection_timeout_custom(self):
         """The timeout parameter can be customized."""
         cfg = self.config
-        cfg['smtp_timeout'] = 42
+        cfg["smtp_timeout"] = 42
         backend = SMTPFactory(cfg)
         assert backend.timeout == 42
 
-
     def test_email_msg_uses_crlf(self):
         """#23063 -- RFC-compliant messages are sent over SMTP."""
         send = SMTP.send
         try:
             smtp_messages = []
 
             def mock_send(self, s):
@@ -564,15 +563,14 @@
             msg = msg.replace("\r\n", "")
             assert msg.find("\r") == -1
             assert msg.find("\n") == -1
 
         finally:
             SMTP.send = send
 
-
     def test_send_messages_after_open_failed(self):
         """
         send_messages() shouldn't try to send messages if open() raises an
         exception after initializing the connection.
         """
         backend = SMTPEmailBackend()
 
@@ -581,21 +579,19 @@
         backend.connection = object()
         backend.open = lambda: None
         email = EmailMessage(
             "Subject", "Content", "from@example.com", ["to@example.com"]
         )
         assert backend.send_messages([email]) == 0
 
-
     def test_send_messages_empty_list(self):
         backend = SMTPEmailBackend()
         backend.connection = object()
         assert backend.send_messages([]) == 0
 
-
     def test_send_messages_zero_sent(self):
         """A message isn't sent if it doesn't have any recipients."""
         backend = SMTPEmailBackend()
         backend.connection = object
         email = EmailMessage("Subject", "Content", "from@example.com", to=[])
         sent = backend.send_messages([email])
         assert sent == 0
```

### Comparing `rick-mailer-1.0.0/tests/test_mailer.py` & `rick-mailer-1.0.1/tests/test_mailer.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,16 @@
 import rick_mailer as mail
 from rick_mailer.backends import SMTPEmailBackend, ConsoleEmailBackend, MemEmailBackend
 from rick_mailer.message import sanitize_address
 from rick_mailer.backends import registry
 from rick_mailer import (
     DNS_NAME,
     EmailMessage,
-    EmailMultiAlternatives, BadHeaderError,
+    EmailMultiAlternatives,
+    BadHeaderError,
 )
 from .custombackend import EmailBackend
 from .common import HeadersCheckMixin
 
 
 class TestMail(HeadersCheckMixin):
     """
@@ -75,15 +76,15 @@
         assert message["From"] == "from@example.com"
         assert message["To"] == "to@example.com, other@example.com"
 
     def test_header_omitted_for_no_to_recipients(self):
         message = EmailMessage(
             "Subject", "Content", "from@example.com", cc=["cc@example.com"]
         ).message()
-        assert str(message).find('To') == -1
+        assert str(message).find("To") == -1
 
     def test_recipients_with_empty_strings(self):
         """
         Empty strings in various recipient arguments are always stripped
         off the final recipient list.
         """
         email = EmailMessage(
@@ -91,15 +92,19 @@
             "Content",
             "from@example.com",
             ["to@example.com", ""],
             cc=["cc@example.com", ""],
             bcc=["", "bcc@example.com"],
             reply_to=["", None],
         )
-        assert email.recipients() == ["to@example.com", "cc@example.com", "bcc@example.com"]
+        assert email.recipients() == [
+            "to@example.com",
+            "cc@example.com",
+            "bcc@example.com",
+        ]
 
     def test_cc(self):
         """Regression test for #7722"""
         email = EmailMessage(
             "Subject",
             "Content",
             "from@example.com",
@@ -131,15 +136,14 @@
         email = EmailMessage(
             "Subject",
             "Content",
             "from@example.com",
             ["to@example.com", "other@example.com"],
             cc=["cc@example.com", "cc.other@example.com"],
             bcc=["bcc@example.com"],
-
         )
         message = email.message()
         assert message["Cc"] == "cc@example.com, cc.other@example.com"
         assert email.recipients() == [
             "to@example.com",
             "other@example.com",
             "cc@example.com",
@@ -250,16 +254,18 @@
             "Long subject lines that get wrapped should contain a space continuation "
             "character to get expected behavior in Outlook and Thunderbird",
             "Content",
             "from@example.com",
             ["to@example.com"],
         )
         message = email.message()
-        assert message[
-                   "Subject"].encode() == b"Long subject lines that get wrapped should contain a space continuation\n character to get expected behavior in Outlook and Thunderbird"
+        assert (
+            message["Subject"].encode()
+            == b"Long subject lines that get wrapped should contain a space continuation\n character to get expected behavior in Outlook and Thunderbird"
+        )
 
     def test_message_header_overrides(self):
         """
         Specifying dates or message-ids in the extra headers overrides the
         default values (#9233)
         """
         headers = {"date": "Fri, 09 Nov 2001 01:08:47 -0000", "Message-ID": "foo"}
@@ -308,28 +314,36 @@
             "Content",
             "bounce@example.com",
             ["list-subscriber@example.com", "list-subscriber2@example.com"],
             headers={"To": "mailing-list@example.com"},
         )
         message = email.message()
         assert message["To"] == "mailing-list@example.com"
-        assert email.to == ["list-subscriber@example.com", "list-subscriber2@example.com"]
+        assert email.to == [
+            "list-subscriber@example.com",
+            "list-subscriber2@example.com",
+        ]
 
         # If we don't set the To header manually, it should default to the `to`
         # argument to the constructor.
         email = EmailMessage(
             "Subject",
             "Content",
             "bounce@example.com",
             ["list-subscriber@example.com", "list-subscriber2@example.com"],
         )
         message = email.message()
 
-        assert message["To"] == "list-subscriber@example.com, list-subscriber2@example.com"
-        assert email.to == ["list-subscriber@example.com", "list-subscriber2@example.com"]
+        assert (
+            message["To"] == "list-subscriber@example.com, list-subscriber2@example.com"
+        )
+        assert email.to == [
+            "list-subscriber@example.com",
+            "list-subscriber2@example.com",
+        ]
 
     def test_to_in_headers_only(self):
         message = EmailMessage(
             "Subject",
             "Content",
             "bounce@example.com",
             headers={"To": "to@example.com"},
@@ -386,38 +400,47 @@
         """
         email = EmailMessage(
             "Subject",
             "Content",
             "from@example.com",
             ['"Firstname Sürname" <to@example.com>', "other@example.com"],
         )
-        assert email.message()["To"] == "=?utf-8?q?Firstname_S=C3=BCrname?= <to@example.com>, other@example.com"
+        assert (
+            email.message()["To"]
+            == "=?utf-8?q?Firstname_S=C3=BCrname?= <to@example.com>, other@example.com"
+        )
 
         email = EmailMessage(
             "Subject",
             "Content",
             "from@example.com",
             ['"Sürname, Firstname" <to@example.com>', "other@example.com"],
         )
-        assert email.message()["To"] == "=?utf-8?q?S=C3=BCrname=2C_Firstname?= <to@example.com>, other@example.com"
+        assert (
+            email.message()["To"]
+            == "=?utf-8?q?S=C3=BCrname=2C_Firstname?= <to@example.com>, other@example.com"
+        )
 
     def test_unicode_headers(self):
         email = EmailMessage(
             "Gżegżółka",
             "Content",
             "from@example.com",
             ["to@example.com"],
             headers={
                 "Sender": '"Firstname Sürname" <sender@example.com>',
                 "Comments": "My Sürname is non-ASCII",
             },
         )
         message = email.message()
         assert message["Subject"] == "=?utf-8?b?R8W8ZWfFvMOzxYJrYQ==?="
-        assert message["Sender"] == "=?utf-8?q?Firstname_S=C3=BCrname?= <sender@example.com>"
+        assert (
+            message["Sender"]
+            == "=?utf-8?q?Firstname_S=C3=BCrname?= <sender@example.com>"
+        )
         assert message["Comments"] == "=?utf-8?q?My_S=C3=BCrname_is_non-ASCII?="
 
     def test_safe_mime_multipart(self):
         """
         Make sure headers can be set with a different encoding than utf-8 in
         SafeMIMEMultipart as well
         """
@@ -430,16 +453,22 @@
             text_content,
             from_email,
             [to],
             headers=headers,
         )
         msg.attach_alternative(html_content, "text/html")
         msg.encoding = "iso-8859-1"
-        assert msg.message()["To"] == "=?iso-8859-1?q?S=FCrname=2C_Firstname?= <to@example.com>"
-        assert msg.message()["Subject"] == "=?iso-8859-1?q?Message_from_Firstname_S=FCrname?="
+        assert (
+            msg.message()["To"]
+            == "=?iso-8859-1?q?S=FCrname=2C_Firstname?= <to@example.com>"
+        )
+        assert (
+            msg.message()["Subject"]
+            == "=?iso-8859-1?q?Message_from_Firstname_S=FCrname?="
+        )
 
     def test_safe_mime_multipart_with_attachments(self):
         """
         EmailMultiAlternatives includes alternatives if the body is empty and
         it has attachments.
         """
         msg = EmailMultiAlternatives(body="")
@@ -501,26 +530,34 @@
             payload0,
             {
                 ("MIME-Version", "1.0"),
                 ("Content-Type", 'text/plain; charset="iso-8859-1"'),
                 ("Content-Transfer-Encoding", "quoted-printable"),
             },
         )
-        assert payload0.as_bytes().endswith(b"\n\nFirstname S=FCrname is a great guy.") is True
+        assert (
+            payload0.as_bytes().endswith(b"\n\nFirstname S=FCrname is a great guy.")
+            is True
+        )
 
         payload1 = msg.message().get_payload(1)
         self.assertMessageHasHeaders(
             payload1,
             {
                 ("MIME-Version", "1.0"),
                 ("Content-Type", 'text/html; charset="iso-8859-1"'),
                 ("Content-Transfer-Encoding", "quoted-printable"),
             },
         )
-        assert payload1.as_bytes().endswith(b"\n\n<p>Firstname S=FCrname is a <strong>great</strong> guy.</p>") is True
+        assert (
+            payload1.as_bytes().endswith(
+                b"\n\n<p>Firstname S=FCrname is a <strong>great</strong> guy.</p>"
+            )
+            is True
+        )
 
     def test_attachments(self):
         """Regression test for #9367"""
         headers = {"Date": "Fri, 09 Nov 2001 01:08:47 -0000", "Message-ID": "foo"}
         subject, from_email, to = "hello", "from@example.com", "to@example.com"
         text_content = "This is an important message."
         html_content = "<p>This is an <strong>important</strong> message.</p>"
@@ -578,15 +615,15 @@
             ("file_png", None),
             ("file_txt.png", "image/png"),
             ("file_png.txt", "text/plain"),
             ("file.eml", "message/rfc822"),
         )
         test_mimetypes = ["text/plain", "image/png", None]
 
-        connection = registry.get('testing')()
+        connection = registry.get("testing")()
         for basename, real_mimetype in files:
             for mimetype in test_mimetypes:
                 email = EmailMessage(
                     "subject", "body", "from@example.com", ["to@example.com"]
                 )
                 assert mimetypes.guess_type(basename)[0] == real_mimetype
                 assert email.attachments == []
@@ -596,15 +633,15 @@
                 email.attach_file(file_path, mimetype=mimetype)
                 assert len(email.attachments) == 1
                 assert email.attachments[0][0].find(basename) > -1
                 msgs_sent_num = email.send(connection)
                 assert msgs_sent_num == 1
 
     def test_attach_text_as_bytes(self):
-        connection = registry.get('testing')()
+        connection = registry.get("testing")()
         msg = EmailMessage("subject", "body", "from@example.com", ["to@example.com"])
         msg.attach("file.txt", b"file content")
         sent_num = msg.send(connection)
         assert sent_num == 1
         filename, content, mimetype = self.get_decoded_attachments(msg)[0]
         assert filename == "file.txt"
         assert content == b"file content"
@@ -654,48 +691,43 @@
             email_msg.attach("file.txt", mimetype="application/pdf")
 
     def test_arbitrary_keyword(self):
         """
         Make sure that get_connection() accepts arbitrary keyword that might be
         used with custom backends.
         """
-        c = registry.get('testing')(fail_silently=True, foo="bar")
+        c = registry.get("testing")(fail_silently=True, foo="bar")
         assert c.fail_silently is True
 
     def test_custom_backend(self):
         """Test custom backend defined in this suite."""
-        conn = registry.get('testing')()
+        conn = registry.get("testing")()
         assert hasattr(conn, "test_outbox") is True
         email = EmailMessage(
             "Subject",
             "Content",
             "bounce@example.com",
             ["to@example.com"],
             headers={"From": "from@example.com"},
         )
         conn.send_messages([email])
         assert len(conn.test_outbox) == 1
 
     def test_backend_arg(self):
         """Test backend argument of mail.get_connection()"""
-        assert isinstance(registry.get('smtp')(), SMTPEmailBackend) is True
-        assert isinstance(registry.get('mem')(), MemEmailBackend) is True
-        assert isinstance(registry.get('console')(), ConsoleEmailBackend) is True
+        assert isinstance(registry.get("smtp")(), SMTPEmailBackend) is True
+        assert isinstance(registry.get("mem")(), MemEmailBackend) is True
+        assert isinstance(registry.get("console")(), ConsoleEmailBackend) is True
 
     def test_connection_arg(self):
         """Test connection argument to send_mail(), et. al."""
         # Send using non-default connection
-        connection = registry.get('testing')()
+        connection = registry.get("testing")()
         mailer = mail.Mailer(connection)
-        mailer.send_mail(
-            "Subject",
-            "Content",
-            "from@example.com",
-            ["to@example.com"]
-        )
+        mailer.send_mail("Subject", "Content", "from@example.com", ["to@example.com"])
         assert len(connection.test_outbox) == 1
         assert connection.test_outbox[0].subject == "Subject"
 
         connection.test_outbox = []
         mailer.send_mass_mail(
             [
                 ("Subject1", "Content1", "from1@example.com", ["to1@example.com"]),
@@ -843,103 +875,103 @@
             },
         )
         assert message.get_payload() == encoding.body_encode(body)
 
     def test_sanitize_address(self):
         """Email addresses are properly sanitized."""
         for email_address, encoding, expected_result in (
-                # ASCII addresses.
-                ("to@example.com", "ascii", "to@example.com"),
-                ("to@example.com", "utf-8", "to@example.com"),
-                (("A name", "to@example.com"), "ascii", "A name <to@example.com>"),
-                (
-                        ("A name", "to@example.com"),
-                        "utf-8",
-                        "A name <to@example.com>",
-                ),
-                ("localpartonly", "ascii", "localpartonly"),
-                # ASCII addresses with display names.
-                ("A name <to@example.com>", "ascii", "A name <to@example.com>"),
-                ("A name <to@example.com>", "utf-8", "A name <to@example.com>"),
-                ('"A name" <to@example.com>', "ascii", "A name <to@example.com>"),
-                ('"A name" <to@example.com>', "utf-8", "A name <to@example.com>"),
-                # Unicode addresses (supported per RFC-6532).
-                ("tó@example.com", "utf-8", "=?utf-8?b?dMOz?=@example.com"),
-                ("to@éxample.com", "utf-8", "to@xn--xample-9ua.com"),
-                (
-                        ("Tó Example", "tó@example.com"),
-                        "utf-8",
-                        "=?utf-8?q?T=C3=B3_Example?= <=?utf-8?b?dMOz?=@example.com>",
-                ),
-                # Unicode addresses with display names.
-                (
-                        "Tó Example <tó@example.com>",
-                        "utf-8",
-                        "=?utf-8?q?T=C3=B3_Example?= <=?utf-8?b?dMOz?=@example.com>",
-                ),
-                (
-                        "To Example <to@éxample.com>",
-                        "ascii",
-                        "To Example <to@xn--xample-9ua.com>",
-                ),
-                (
-                        "To Example <to@éxample.com>",
-                        "utf-8",
-                        "To Example <to@xn--xample-9ua.com>",
-                ),
-                # Addresses with two @ signs.
-                ('"to@other.com"@example.com', "utf-8", r'"to@other.com"@example.com'),
-                (
-                        '"to@other.com" <to@example.com>',
-                        "utf-8",
-                        '"to@other.com" <to@example.com>',
-                ),
-                (
-                        ("To Example", "to@other.com@example.com"),
-                        "utf-8",
-                        'To Example <"to@other.com"@example.com>',
-                ),
-                # Addresses with long unicode display names.
-                (
-                        "Tó Example very long" * 4 + " <to@example.com>",
-                        "utf-8",
-                        "=?utf-8?q?T=C3=B3_Example_very_longT=C3=B3_Example_very_longT"
-                        "=C3=B3_Example_?=\n"
-                        " =?utf-8?q?very_longT=C3=B3_Example_very_long?= "
-                        "<to@example.com>",
-                ),
-                (
-                        ("Tó Example very long" * 4, "to@example.com"),
-                        "utf-8",
-                        "=?utf-8?q?T=C3=B3_Example_very_longT=C3=B3_Example_very_longT"
-                        "=C3=B3_Example_?=\n"
-                        " =?utf-8?q?very_longT=C3=B3_Example_very_long?= "
-                        "<to@example.com>",
-                ),
-                # Address with long display name and unicode domain.
-                (
-                        ("To Example very long" * 4, "to@exampl€.com"),
-                        "utf-8",
-                        "To Example very longTo Example very longTo Example very longT"
-                        "o Example very\n"
-                        " long <to@xn--exampl-nc1c.com>",
-                ),
+            # ASCII addresses.
+            ("to@example.com", "ascii", "to@example.com"),
+            ("to@example.com", "utf-8", "to@example.com"),
+            (("A name", "to@example.com"), "ascii", "A name <to@example.com>"),
+            (
+                ("A name", "to@example.com"),
+                "utf-8",
+                "A name <to@example.com>",
+            ),
+            ("localpartonly", "ascii", "localpartonly"),
+            # ASCII addresses with display names.
+            ("A name <to@example.com>", "ascii", "A name <to@example.com>"),
+            ("A name <to@example.com>", "utf-8", "A name <to@example.com>"),
+            ('"A name" <to@example.com>', "ascii", "A name <to@example.com>"),
+            ('"A name" <to@example.com>', "utf-8", "A name <to@example.com>"),
+            # Unicode addresses (supported per RFC-6532).
+            ("tó@example.com", "utf-8", "=?utf-8?b?dMOz?=@example.com"),
+            ("to@éxample.com", "utf-8", "to@xn--xample-9ua.com"),
+            (
+                ("Tó Example", "tó@example.com"),
+                "utf-8",
+                "=?utf-8?q?T=C3=B3_Example?= <=?utf-8?b?dMOz?=@example.com>",
+            ),
+            # Unicode addresses with display names.
+            (
+                "Tó Example <tó@example.com>",
+                "utf-8",
+                "=?utf-8?q?T=C3=B3_Example?= <=?utf-8?b?dMOz?=@example.com>",
+            ),
+            (
+                "To Example <to@éxample.com>",
+                "ascii",
+                "To Example <to@xn--xample-9ua.com>",
+            ),
+            (
+                "To Example <to@éxample.com>",
+                "utf-8",
+                "To Example <to@xn--xample-9ua.com>",
+            ),
+            # Addresses with two @ signs.
+            ('"to@other.com"@example.com', "utf-8", r'"to@other.com"@example.com'),
+            (
+                '"to@other.com" <to@example.com>',
+                "utf-8",
+                '"to@other.com" <to@example.com>',
+            ),
+            (
+                ("To Example", "to@other.com@example.com"),
+                "utf-8",
+                'To Example <"to@other.com"@example.com>',
+            ),
+            # Addresses with long unicode display names.
+            (
+                "Tó Example very long" * 4 + " <to@example.com>",
+                "utf-8",
+                "=?utf-8?q?T=C3=B3_Example_very_longT=C3=B3_Example_very_longT"
+                "=C3=B3_Example_?=\n"
+                " =?utf-8?q?very_longT=C3=B3_Example_very_long?= "
+                "<to@example.com>",
+            ),
+            (
+                ("Tó Example very long" * 4, "to@example.com"),
+                "utf-8",
+                "=?utf-8?q?T=C3=B3_Example_very_longT=C3=B3_Example_very_longT"
+                "=C3=B3_Example_?=\n"
+                " =?utf-8?q?very_longT=C3=B3_Example_very_long?= "
+                "<to@example.com>",
+            ),
+            # Address with long display name and unicode domain.
+            (
+                ("To Example very long" * 4, "to@exampl€.com"),
+                "utf-8",
+                "To Example very longTo Example very longTo Example very longT"
+                "o Example very\n"
+                " long <to@xn--exampl-nc1c.com>",
+            ),
         ):
             assert sanitize_address(email_address, encoding) == expected_result
 
     def test_sanitize_address_invalid(self):
         for email_address in (
-                # Invalid address with two @ signs.
-                "to@other.com@example.com",
-                # Invalid address without the quotes.
-                "to@other.com <to@example.com>",
-                # Other invalid addresses.
-                "@",
-                "to@",
-                "@example.com",
+            # Invalid address with two @ signs.
+            "to@other.com@example.com",
+            # Invalid address without the quotes.
+            "to@other.com <to@example.com>",
+            # Other invalid addresses.
+            "@",
+            "to@",
+            "@example.com",
         ):
             with pytest.raises(ValueError):
                 sanitize_address(email_address, encoding="utf-8")
 
     def test_sanitize_address_header_injection(self):
         msg = "Invalid address; address parts cannot contain newlines."
         tests = [
@@ -958,15 +990,14 @@
         with pytest.raises(ValueError):
             email_msg.attach_alternative(None, "text/html")
         with pytest.raises(ValueError):
             email_msg.attach_alternative("<p>content</p>", None)
 
 
 class TestMailTimeZone:
-
     def test_date_header_utc(self):
         """
         Datetime should be in UTC.
         """
         email = EmailMessage(
             "Subject", "Body", "bounce@example.com", ["to@example.com"]
         )
```

