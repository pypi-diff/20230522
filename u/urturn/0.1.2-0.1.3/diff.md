# Comparing `tmp/urturn-0.1.2.tar.gz` & `tmp/urturn-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "urturn-0.1.2.tar", last modified: Thu May 18 12:10:41 2023, max compression
+gzip compressed data, was "urturn-0.1.3.tar", last modified: Mon May 22 20:07:09 2023, max compression
```

## Comparing `urturn-0.1.2.tar` & `urturn-0.1.3.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 12:10:41.965477 urturn-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-18 12:10:26.000000 urturn-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-05-18 12:10:41.965477 urturn-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-18 12:10:26.000000 urturn-0.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 12:10:41.965477 urturn-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-05-18 12:10:26.000000 urturn-0.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 12:10:41.965477 urturn-0.1.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4639 2023-05-18 12:10:26.000000 urturn-0.1.2/tests/test_job.py
--rw-r--r--   0 runner    (1001) docker     (123)     7430 2023-05-18 12:10:26.000000 urturn-0.1.2/tests/test_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-05-18 12:10:26.000000 urturn-0.1.2/tests/test_trigger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-05-18 12:10:26.000000 urturn-0.1.2/tests/test_webapp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 12:10:41.965477 urturn-0.1.2/urturn/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-18 12:10:41.000000 urturn-0.1.2/urturn/REQUIREMENTS
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-18 12:10:41.000000 urturn-0.1.2/urturn/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 12:10:26.000000 urturn-0.1.2/urturn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7169 2023-05-18 12:10:26.000000 urturn-0.1.2/urturn/job.py
--rw-r--r--   0 runner    (1001) docker     (123)     4037 2023-05-18 12:10:26.000000 urturn-0.1.2/urturn/scheduler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 12:10:41.965477 urturn-0.1.2/urturn/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     6119 2023-05-18 12:10:26.000000 urturn-0.1.2/urturn/templates/adapted.min.css
--rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-05-18 12:10:26.000000 urturn-0.1.2/urturn/templates/details.css
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-05-18 12:10:26.000000 urturn-0.1.2/urturn/templates/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     2770 2023-05-18 12:10:26.000000 urturn-0.1.2/urturn/templates/job_config.html
--rw-r--r--   0 runner    (1001) docker     (123)     2885 2023-05-18 12:10:26.000000 urturn-0.1.2/urturn/trigger.py
--rw-r--r--   0 runner    (1001) docker     (123)     3301 2023-05-18 12:10:26.000000 urturn-0.1.2/urturn/webapp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 12:10:41.965477 urturn-0.1.2/urturn.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-05-18 12:10:41.000000 urturn-0.1.2/urturn.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-05-18 12:10:41.000000 urturn-0.1.2/urturn.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 12:10:41.000000 urturn-0.1.2/urturn.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-18 12:10:41.000000 urturn-0.1.2/urturn.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-18 12:10:41.000000 urturn-0.1.2/urturn.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:07:09.224119 urturn-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-22 20:06:57.000000 urturn-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-05-22 20:07:09.224119 urturn-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-22 20:06:57.000000 urturn-0.1.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 20:07:09.224119 urturn-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-05-22 20:06:57.000000 urturn-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:07:09.220119 urturn-0.1.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4639 2023-05-22 20:06:57.000000 urturn-0.1.3/tests/test_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7430 2023-05-22 20:06:57.000000 urturn-0.1.3/tests/test_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-05-22 20:06:57.000000 urturn-0.1.3/tests/test_trigger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-05-22 20:06:57.000000 urturn-0.1.3/tests/test_webapp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:07:09.220119 urturn-0.1.3/urturn/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-22 20:07:09.000000 urturn-0.1.3/urturn/REQUIREMENTS
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-22 20:07:09.000000 urturn-0.1.3/urturn/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 20:06:57.000000 urturn-0.1.3/urturn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7169 2023-05-22 20:06:57.000000 urturn-0.1.3/urturn/job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3850 2023-05-22 20:06:57.000000 urturn-0.1.3/urturn/scheduler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:07:09.224119 urturn-0.1.3/urturn/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     6119 2023-05-22 20:06:57.000000 urturn-0.1.3/urturn/templates/adapted.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-05-22 20:06:57.000000 urturn-0.1.3/urturn/templates/details.css
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-05-22 20:06:57.000000 urturn-0.1.3/urturn/templates/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2770 2023-05-22 20:06:57.000000 urturn-0.1.3/urturn/templates/job_config.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2885 2023-05-22 20:06:57.000000 urturn-0.1.3/urturn/trigger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3323 2023-05-22 20:06:57.000000 urturn-0.1.3/urturn/webapp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:07:09.220119 urturn-0.1.3/urturn.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-05-22 20:07:09.000000 urturn-0.1.3/urturn.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-05-22 20:07:09.000000 urturn-0.1.3/urturn.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 20:07:09.000000 urturn-0.1.3/urturn.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-22 20:07:09.000000 urturn-0.1.3/urturn.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-22 20:07:09.000000 urturn-0.1.3/urturn.egg-info/top_level.txt
```

### Comparing `urturn-0.1.2/LICENSE` & `urturn-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `urturn-0.1.2/setup.py` & `urturn-0.1.3/setup.py`

 * *Files identical despite different names*

### Comparing `urturn-0.1.2/tests/test_job.py` & `urturn-0.1.3/tests/test_job.py`

 * *Files identical despite different names*

### Comparing `urturn-0.1.2/tests/test_scheduler.py` & `urturn-0.1.3/tests/test_scheduler.py`

 * *Files identical despite different names*

### Comparing `urturn-0.1.2/tests/test_trigger.py` & `urturn-0.1.3/tests/test_trigger.py`

 * *Files identical despite different names*

### Comparing `urturn-0.1.2/tests/test_webapp.py` & `urturn-0.1.3/tests/test_webapp.py`

 * *Files identical despite different names*

### Comparing `urturn-0.1.2/urturn/job.py` & `urturn-0.1.3/urturn/job.py`

 * *Files identical despite different names*

### Comparing `urturn-0.1.2/urturn/scheduler.py` & `urturn-0.1.3/urturn/scheduler.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,12 @@
 """Scheduler for execution jobs concurrently"""
 
 from typing import List, Optional, Dict
 import time
 from datetime import datetime
-import os
-
-import signal
 
 from .trigger import Trigger
 from .job import JobConfig, JobEvent
 
 
 class Scheduler:
     """Scheduler class that runs jobs according to their configurations and triggers.
@@ -95,19 +92,15 @@
             time.sleep(1)
 
     def _kill_all_running_jobs(self):
         for job_conf in self.job_configs:
             if not job_conf.current_execution:
                 continue
 
-            if os.name == 'posix':
-                job_conf.current_execution.process.send_signal(
-                    signal.SIGTERM)
-            else:
-                job_conf.current_execution.process.terminate()
+            job_conf.current_execution.process.kill()
 
     def stop(self):
         """Stop the scheduler's loop.
 
         Sets the running attribute to False, causing the scheduler's loop to terminate.
         """
         self._kill_all_running_jobs()
```

### Comparing `urturn-0.1.2/urturn/templates/adapted.min.css` & `urturn-0.1.3/urturn/templates/adapted.min.css`

 * *Files identical despite different names*

### Comparing `urturn-0.1.2/urturn/templates/details.css` & `urturn-0.1.3/urturn/templates/details.css`

 * *Files identical despite different names*

### Comparing `urturn-0.1.2/urturn/templates/index.html` & `urturn-0.1.3/urturn/templates/index.html`

 * *Files identical despite different names*

### Comparing `urturn-0.1.2/urturn/templates/job_config.html` & `urturn-0.1.3/urturn/templates/job_config.html`

 * *Files identical despite different names*

### Comparing `urturn-0.1.2/urturn/trigger.py` & `urturn-0.1.3/urturn/trigger.py`

 * *Files identical despite different names*

### Comparing `urturn-0.1.2/urturn/webapp.py` & `urturn-0.1.3/urturn/webapp.py`

 * *Files 4% similar despite different names*

```diff
@@ -76,20 +76,20 @@
             (job_conf for job_conf in self.scheduler.job_configs if job_conf.name == job_name),
             None)
         if job is None:
             return "Job not found", 404
 
         return render_template("job_config.html", job=job)
 
-    def run(self, port=8000, debug=False):
+    def run(self, host=None, port=8000, debug=False):
         """Start the web application with the specified debug mode.
 
         Args:
             debug (bool, optional): Run the web application in debug mode. Defaults to False.
         """
 
         # Start the scheduler in a separate thread
         scheduler_thread = Thread(target=self.scheduler.start)
         scheduler_thread.daemon = True
         scheduler_thread.start()
 
-        self.app.run(port=port, debug=debug, use_reloader=False)
+        self.app.run(host=host, port=port, debug=debug, use_reloader=False)
```

