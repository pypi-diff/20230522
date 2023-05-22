# Comparing `tmp/x_decorator-1.0.0.tar.gz` & `tmp/x_decorator-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "x_decorator-1.0.0.tar", last modified: Tue May  9 14:43:52 2023, max compression
+gzip compressed data, was "x_decorator-1.0.1.tar", last modified: Mon May 22 09:28:29 2023, max compression
```

## Comparing `x_decorator-1.0.0.tar` & `x_decorator-1.0.1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 14:43:52.131518 x_decorator-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 14:43:42.000000 x_decorator-1.0.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-05-09 14:43:42.000000 x_decorator-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-09 14:43:42.000000 x_decorator-1.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-05-09 14:43:52.131518 x_decorator-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-05-09 14:43:42.000000 x_decorator-1.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-05-09 14:43:42.000000 x_decorator-1.0.0/long_description.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-05-09 14:43:52.131518 x_decorator-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-05-09 14:43:42.000000 x_decorator-1.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 14:43:52.127518 x_decorator-1.0.0/x_decorator/
--rw-r--r--   0 runner    (1001) docker     (123)      992 2023-05-09 14:43:42.000000 x_decorator-1.0.0/x_decorator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-05-09 14:43:42.000000 x_decorator-1.0.0/x_decorator/circuit_breaker_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-05-09 14:43:42.000000 x_decorator-1.0.0/x_decorator/concurrent_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-05-09 14:43:42.000000 x_decorator-1.0.0/x_decorator/count_calls_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)      473 2023-05-09 14:43:42.000000 x_decorator-1.0.0/x_decorator/debug_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-05-09 14:43:42.000000 x_decorator-1.0.0/x_decorator/email_on_failure_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-05-09 14:43:42.000000 x_decorator-1.0.0/x_decorator/log_execution_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-05-09 14:43:42.000000 x_decorator-1.0.0/x_decorator/memoize_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-05-09 14:43:42.000000 x_decorator-1.0.0/x_decorator/queue_processor_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)      898 2023-05-09 14:43:42.000000 x_decorator-1.0.0/x_decorator/rate_limit_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-05-09 14:43:42.000000 x_decorator-1.0.0/x_decorator/retry_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-05-09 14:43:42.000000 x_decorator-1.0.0/x_decorator/run_at_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-05-09 14:43:42.000000 x_decorator-1.0.0/x_decorator/scheduler_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-05-09 14:43:42.000000 x_decorator-1.0.0/x_decorator/singleton_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3553 2023-05-09 14:43:42.000000 x_decorator-1.0.0/x_decorator/state_machine_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-05-09 14:43:42.000000 x_decorator-1.0.0/x_decorator/timing_decorator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 14:43:52.131518 x_decorator-1.0.0/x_decorator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-05-09 14:43:52.000000 x_decorator-1.0.0/x_decorator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      857 2023-05-09 14:43:52.000000 x_decorator-1.0.0/x_decorator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 14:43:52.000000 x_decorator-1.0.0/x_decorator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 14:43:52.000000 x_decorator-1.0.0/x_decorator.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-09 14:43:52.000000 x_decorator-1.0.0/x_decorator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-09 14:43:52.000000 x_decorator-1.0.0/x_decorator.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 09:28:29.480227 x_decorator-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 09:28:15.000000 x_decorator-1.0.1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-05-22 09:28:15.000000 x_decorator-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-22 09:28:15.000000 x_decorator-1.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-05-22 09:28:29.484227 x_decorator-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-05-22 09:28:15.000000 x_decorator-1.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-05-22 09:28:15.000000 x_decorator-1.0.1/long_description.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-05-22 09:28:29.484227 x_decorator-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-05-22 09:28:15.000000 x_decorator-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 09:28:29.480227 x_decorator-1.0.1/x_decorator/
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-05-22 09:28:15.000000 x_decorator-1.0.1/x_decorator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-05-22 09:28:15.000000 x_decorator-1.0.1/x_decorator/circuit_breaker_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-05-22 09:28:15.000000 x_decorator-1.0.1/x_decorator/concurrent_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-05-22 09:28:15.000000 x_decorator-1.0.1/x_decorator/count_calls_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-05-22 09:28:15.000000 x_decorator-1.0.1/x_decorator/debug_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-05-22 09:28:15.000000 x_decorator-1.0.1/x_decorator/email_on_failure_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-05-22 09:28:15.000000 x_decorator-1.0.1/x_decorator/log_execution_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-05-22 09:28:15.000000 x_decorator-1.0.1/x_decorator/memoize_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-05-22 09:28:15.000000 x_decorator-1.0.1/x_decorator/queue_processor_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2023-05-22 09:28:15.000000 x_decorator-1.0.1/x_decorator/rate_limit_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-05-22 09:28:15.000000 x_decorator-1.0.1/x_decorator/retry_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-05-22 09:28:15.000000 x_decorator-1.0.1/x_decorator/run_at_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-05-22 09:28:15.000000 x_decorator-1.0.1/x_decorator/scheduler_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-05-22 09:28:15.000000 x_decorator-1.0.1/x_decorator/singleton_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3553 2023-05-22 09:28:15.000000 x_decorator-1.0.1/x_decorator/state_machine_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-05-22 09:28:15.000000 x_decorator-1.0.1/x_decorator/timing_decorator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 09:28:29.480227 x_decorator-1.0.1/x_decorator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-05-22 09:28:29.000000 x_decorator-1.0.1/x_decorator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      857 2023-05-22 09:28:29.000000 x_decorator-1.0.1/x_decorator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 09:28:29.000000 x_decorator-1.0.1/x_decorator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 09:28:29.000000 x_decorator-1.0.1/x_decorator.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-22 09:28:29.000000 x_decorator-1.0.1/x_decorator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-22 09:28:29.000000 x_decorator-1.0.1/x_decorator.egg-info/top_level.txt
```

### Comparing `x_decorator-1.0.0/LICENSE` & `x_decorator-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `x_decorator-1.0.0/PKG-INFO` & `x_decorator-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: x_decorator
-Version: 1.0.0
+Version: 1.0.1
 Summary: X Decorator [X Decorator is a python package for decorators that used for a variety of purposes, such as logging, memoization, and more.]
 Home-page: https://github.com/shokr/x_decorator
 Author: Muhammed Shokr
 Author-email: mohammedshokr2014@gmail.com
 Maintainer: Muhammed Shokr
 Maintainer-email: mohammedshokr2014@gmail.com
 License: BSD-3-Clause
```

### Comparing `x_decorator-1.0.0/README.md` & `x_decorator-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `x_decorator-1.0.0/setup.cfg` & `x_decorator-1.0.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `x_decorator-1.0.0/setup.py` & `x_decorator-1.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `x_decorator-1.0.0/x_decorator/__init__.py` & `x_decorator-1.0.1/x_decorator/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-__version__ = "1.0.0"
+__version__ = "1.0.1"
 
 from .circuit_breaker_decorator import CircuitBreaker as X_CircuitBreaker
 from .concurrent_decorator import x_concurrent as x_concurrent
 from .count_calls_decorator import count_calls as x_count_calls
 from .debug_decorator import debug as x_debug
-from .email_on_failure_decorator import email_on_failure as x_email_on_failure
+# from .email_on_failure_decorator import email_on_failure as x_email_on_failure
 from .log_execution_decorator import log_execution as x_log_execution
 from .memoize_decorator import memoize as x_memoize
 from .queue_processor_decorator import queue_processor as x_queue_processor
 from .rate_limit_decorator import rate_limit as x_rate_limit
 from .retry_decorator import retry as x_retry
 from .run_at_decorator import run_at as x_run_at
 # from .scheduler_decorator import scheduler as x_scheduler
```

### Comparing `x_decorator-1.0.0/x_decorator/circuit_breaker_decorator.py` & `x_decorator-1.0.1/x_decorator/circuit_breaker_decorator.py`

 * *Files identical despite different names*

### Comparing `x_decorator-1.0.0/x_decorator/email_on_failure_decorator.py` & `x_decorator-1.0.1/x_decorator/email_on_failure_decorator.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,44 +1,45 @@
-import smtplib
+# import smtplib
+# import traceback
 
-from email.mime.text import MIMEText
+# from email.mime.text import MIMEText
 
 
-def email_on_failure(sender_email, password, recipient_email):
-    """
-        a very useful decorator in production systems is the notification decorator.
-        Once again, even with several retries,
-        even a well-tested codebase fails. And when that happens,
-         we need to inform someone about it to take quick action.
-
-
-         EX:
-         @email_on_failure(sender_email='your_email@gmail.com', password='your_password',
-                  recipient_email='recipient_email@gmail.com')
-        def my_function():
-            # code that might fail
-            pass
-    """
-
-    def decorator(func):
-        def wrapper(*args, **kwargs):
-            try:
-                return func(*args, **kwargs)
-            except Exception as e:
-                # format the error message and traceback
-                err_msg = f"Error: {str(e)}\n\nTraceback:\n{traceback.format_exc()}"
-
-                # create the email message
-                message = MIMEText(err_msg)
-                message['Subject'] = f"{func.__name__} failed"
-                message['From'] = sender_email
-                message['To'] = recipient_email
-
-                # send the email
-                with smtplib.SMTP_SSL('smtp.gmail.com', 465) as smtp:
-                    smtp.login(sender_email, password)
-                    smtp.sendmail(sender_email, recipient_email, message.as_string())
+# def email_on_failure(sender_email, password, recipient_email):
+#     """
+#         a very useful decorator in production systems is the notification decorator.
+#         Once again, even with several retries,
+#         even a well-tested codebase fails. And when that happens,
+#          we need to inform someone about it to take quick action.
+
+
+#          EX:
+#          @email_on_failure(sender_email='your_email@gmail.com', password='your_password',
+#                   recipient_email='recipient_email@gmail.com')
+#         def my_function():
+#             # code that might fail
+#             pass
+#     """
+
+#     def decorator(func):
+#         def wrapper(*args, **kwargs):
+#             try:
+#                 return func(*args, **kwargs)
+#             except Exception as e:
+#                 # format the error message and traceback
+#                 err_msg = f"Error: {str(e)}\n\nTraceback:\n{traceback.format_exc()}"
+
+#                 # create the email message
+#                 message = MIMEText(err_msg)
+#                 message['Subject'] = f"{func.__name__} failed"
+#                 message['From'] = sender_email
+#                 message['To'] = recipient_email
+
+#                 # send the email
+#                 with smtplib.SMTP_SSL('smtp.gmail.com', 465) as smtp:
+#                     smtp.login(sender_email, password)
+#                     smtp.sendmail(sender_email, recipient_email, message.as_string())
 
-                # re-raise the exception
-                raise
+#                 # re-raise the exception
+#                 raise
 
-        return wrapper
+#         return wrapper
```

### Comparing `x_decorator-1.0.0/x_decorator/log_execution_decorator.py` & `x_decorator-1.0.1/x_decorator/log_execution_decorator.py`

 * *Files identical despite different names*

### Comparing `x_decorator-1.0.0/x_decorator/memoize_decorator.py` & `x_decorator-1.0.1/x_decorator/memoize_decorator.py`

 * *Files identical despite different names*

### Comparing `x_decorator-1.0.0/x_decorator/queue_processor_decorator.py` & `x_decorator-1.0.1/x_decorator/queue_processor_decorator.py`

 * *Files identical despite different names*

### Comparing `x_decorator-1.0.0/x_decorator/rate_limit_decorator.py` & `x_decorator-1.0.1/x_decorator/rate_limit_decorator.py`

 * *Files identical despite different names*

### Comparing `x_decorator-1.0.0/x_decorator/retry_decorator.py` & `x_decorator-1.0.1/x_decorator/retry_decorator.py`

 * *Files identical despite different names*

### Comparing `x_decorator-1.0.0/x_decorator/run_at_decorator.py` & `x_decorator-1.0.1/x_decorator/run_at_decorator.py`

 * *Files identical despite different names*

### Comparing `x_decorator-1.0.0/x_decorator/scheduler_decorator.py` & `x_decorator-1.0.1/x_decorator/scheduler_decorator.py`

 * *Files identical despite different names*

### Comparing `x_decorator-1.0.0/x_decorator/state_machine_decorator.py` & `x_decorator-1.0.1/x_decorator/state_machine_decorator.py`

 * *Files identical despite different names*

### Comparing `x_decorator-1.0.0/x_decorator/timing_decorator.py` & `x_decorator-1.0.1/x_decorator/timing_decorator.py`

 * *Files identical despite different names*

### Comparing `x_decorator-1.0.0/x_decorator.egg-info/PKG-INFO` & `x_decorator-1.0.1/x_decorator.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: x-decorator
-Version: 1.0.0
+Version: 1.0.1
 Summary: X Decorator [X Decorator is a python package for decorators that used for a variety of purposes, such as logging, memoization, and more.]
 Home-page: https://github.com/shokr/x_decorator
 Author: Muhammed Shokr
 Author-email: mohammedshokr2014@gmail.com
 Maintainer: Muhammed Shokr
 Maintainer-email: mohammedshokr2014@gmail.com
 License: BSD-3-Clause
```

### Comparing `x_decorator-1.0.0/x_decorator.egg-info/SOURCES.txt` & `x_decorator-1.0.1/x_decorator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

