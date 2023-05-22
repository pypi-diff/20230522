# Comparing `tmp/joeflow-1.2.2.tar.gz` & `tmp/joeflow-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "joeflow-1.2.2.tar", last modified: Fri Jan  6 11:11:35 2023, max compression
+gzip compressed data, was "joeflow-1.2.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `joeflow-1.2.2.tar` & `joeflow-1.2.3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0     1522 2023-01-06 11:11:15.432740 joeflow-1.2.2/LICENSE
--rw-r--r--   0        0        0     3128 2023-01-06 11:11:15.432740 joeflow-1.2.2/README.rst
--rw-r--r--   0        0        0      158 2023-01-06 11:11:15.432740 joeflow-1.2.2/joeflow/__init__.py
--rw-r--r--   0        0        0      160 2023-01-06 11:11:35.176799 joeflow-1.2.2/joeflow/_version.py
--rw-r--r--   0        0        0     4220 2023-01-06 11:11:15.432740 joeflow-1.2.2/joeflow/admin.py
--rw-r--r--   0        0        0      286 2023-01-06 11:11:15.432740 joeflow-1.2.2/joeflow/apps.py
--rw-r--r--   0        0        0      824 2023-01-06 11:11:15.432740 joeflow-1.2.2/joeflow/conf.py
--rw-r--r--   0        0        0        0 2023-01-06 11:11:15.432740 joeflow-1.2.2/joeflow/contrib/__init__.py
--rw-r--r--   0        0        0     1234 2023-01-06 11:11:15.432740 joeflow-1.2.2/joeflow/contrib/reversion.py
--rw-r--r--   0        0        0     1387 2023-01-06 11:11:15.432740 joeflow-1.2.2/joeflow/forms.py
--rw-r--r--   0        0        0        0 2023-01-06 11:11:15.432740 joeflow-1.2.2/joeflow/management/__init__.py
--rw-r--r--   0        0        0        0 2023-01-06 11:11:15.432740 joeflow-1.2.2/joeflow/management/commands/__init__.py
--rw-r--r--   0        0        0     2304 2023-01-06 11:11:15.432740 joeflow-1.2.2/joeflow/management/commands/render_workflow_graph.py
--rw-r--r--   0        0        0     4956 2023-01-06 11:11:15.432740 joeflow-1.2.2/joeflow/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2023-01-06 11:11:15.432740 joeflow-1.2.2/joeflow/migrations/__init__.py
--rw-r--r--   0        0        0    18595 2023-01-06 11:11:15.432740 joeflow-1.2.2/joeflow/models.py
--rw-r--r--   0        0        0        0 2023-01-06 11:11:15.432740 joeflow-1.2.2/joeflow/runner/__init__.py
--rw-r--r--   0        0        0     1995 2023-01-06 11:11:15.432740 joeflow-1.2.2/joeflow/runner/celery.py
--rw-r--r--   0        0        0     2029 2023-01-06 11:11:15.432740 joeflow-1.2.2/joeflow/runner/dramatiq.py
--rw-r--r--   0        0        0      288 2023-01-06 11:11:15.432740 joeflow-1.2.2/joeflow/tasks/__init__.py
--rw-r--r--   0        0        0      807 2023-01-06 11:11:15.432740 joeflow-1.2.2/joeflow/tasks/human.py
--rw-r--r--   0        0        0     3763 2023-01-06 11:11:15.432740 joeflow-1.2.2/joeflow/tasks/machine.py
--rw-r--r--   0        0        0       36 2023-01-06 11:11:15.432740 joeflow-1.2.2/joeflow/typing.py
--rw-r--r--   0        0        0     2745 2023-01-06 11:11:15.432740 joeflow-1.2.2/joeflow/utils.py
--rw-r--r--   0        0        0     3399 2023-01-06 11:11:15.432740 joeflow-1.2.2/joeflow/views.py
--rw-r--r--   0        0        0     2622 2023-01-06 11:11:15.432740 joeflow-1.2.2/pyproject.toml
--rw-r--r--   0        0        0     5557 1970-01-01 00:00:00.000000 joeflow-1.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1522 2023-05-22 11:15:09.599767 joeflow-1.2.3/LICENSE
+-rw-r--r--   0        0        0     3128 2023-05-22 11:15:09.599767 joeflow-1.2.3/README.rst
+-rw-r--r--   0        0        0      158 2023-05-22 11:15:09.599767 joeflow-1.2.3/joeflow/__init__.py
+-rw-r--r--   0        0        0      160 2023-05-22 11:15:25.075769 joeflow-1.2.3/joeflow/_version.py
+-rw-r--r--   0        0        0     4220 2023-05-22 11:15:09.599767 joeflow-1.2.3/joeflow/admin.py
+-rw-r--r--   0        0        0      286 2023-05-22 11:15:09.599767 joeflow-1.2.3/joeflow/apps.py
+-rw-r--r--   0        0        0      824 2023-05-22 11:15:09.599767 joeflow-1.2.3/joeflow/conf.py
+-rw-r--r--   0        0        0        0 2023-05-22 11:15:09.599767 joeflow-1.2.3/joeflow/contrib/__init__.py
+-rw-r--r--   0        0        0     1234 2023-05-22 11:15:09.599767 joeflow-1.2.3/joeflow/contrib/reversion.py
+-rw-r--r--   0        0        0     1387 2023-05-22 11:15:09.599767 joeflow-1.2.3/joeflow/forms.py
+-rw-r--r--   0        0        0        0 2023-05-22 11:15:09.599767 joeflow-1.2.3/joeflow/management/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-22 11:15:09.599767 joeflow-1.2.3/joeflow/management/commands/__init__.py
+-rw-r--r--   0        0        0     2304 2023-05-22 11:15:09.599767 joeflow-1.2.3/joeflow/management/commands/render_workflow_graph.py
+-rw-r--r--   0        0        0     4955 2023-05-22 11:15:09.599767 joeflow-1.2.3/joeflow/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2023-05-22 11:15:09.599767 joeflow-1.2.3/joeflow/migrations/__init__.py
+-rw-r--r--   0        0        0    18595 2023-05-22 11:15:09.599767 joeflow-1.2.3/joeflow/models.py
+-rw-r--r--   0        0        0        0 2023-05-22 11:15:09.599767 joeflow-1.2.3/joeflow/runner/__init__.py
+-rw-r--r--   0        0        0     1995 2023-05-22 11:15:09.599767 joeflow-1.2.3/joeflow/runner/celery.py
+-rw-r--r--   0        0        0     2158 2023-05-22 11:15:09.599767 joeflow-1.2.3/joeflow/runner/dramatiq.py
+-rw-r--r--   0        0        0      288 2023-05-22 11:15:09.599767 joeflow-1.2.3/joeflow/tasks/__init__.py
+-rw-r--r--   0        0        0      807 2023-05-22 11:15:09.599767 joeflow-1.2.3/joeflow/tasks/human.py
+-rw-r--r--   0        0        0     3763 2023-05-22 11:15:09.599767 joeflow-1.2.3/joeflow/tasks/machine.py
+-rw-r--r--   0        0        0       36 2023-05-22 11:15:09.599767 joeflow-1.2.3/joeflow/typing.py
+-rw-r--r--   0        0        0     2745 2023-05-22 11:15:09.599767 joeflow-1.2.3/joeflow/utils.py
+-rw-r--r--   0        0        0     3399 2023-05-22 11:15:09.599767 joeflow-1.2.3/joeflow/views.py
+-rw-r--r--   0        0        0     2622 2023-05-22 11:15:09.599767 joeflow-1.2.3/pyproject.toml
+-rw-r--r--   0        0        0     5557 1970-01-01 00:00:00.000000 joeflow-1.2.3/PKG-INFO
```

### Comparing `joeflow-1.2.2/LICENSE` & `joeflow-1.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `joeflow-1.2.2/README.rst` & `joeflow-1.2.3/README.rst`

 * *Files identical despite different names*

### Comparing `joeflow-1.2.2/joeflow/admin.py` & `joeflow-1.2.3/joeflow/admin.py`

 * *Files identical despite different names*

### Comparing `joeflow-1.2.2/joeflow/conf.py` & `joeflow-1.2.3/joeflow/conf.py`

 * *Files identical despite different names*

### Comparing `joeflow-1.2.2/joeflow/contrib/reversion.py` & `joeflow-1.2.3/joeflow/contrib/reversion.py`

 * *Files identical despite different names*

### Comparing `joeflow-1.2.2/joeflow/forms.py` & `joeflow-1.2.3/joeflow/forms.py`

 * *Files identical despite different names*

### Comparing `joeflow-1.2.2/joeflow/management/commands/render_workflow_graph.py` & `joeflow-1.2.3/joeflow/management/commands/render_workflow_graph.py`

 * *Files identical despite different names*

### Comparing `joeflow-1.2.2/joeflow/migrations/0001_initial.py` & `joeflow-1.2.3/joeflow/migrations/0001_initial.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 from django.conf import settings
 from django.db import migrations, models
 
 import joeflow.models
 
 
 class Migration(migrations.Migration):
-
     initial = True
 
     dependencies = [
         ("contenttypes", "0002_remove_content_type_name"),
         migrations.swappable_dependency(settings.AUTH_USER_MODEL),
     ]
```

### Comparing `joeflow-1.2.2/joeflow/models.py` & `joeflow-1.2.3/joeflow/models.py`

 * *Files identical despite different names*

### Comparing `joeflow-1.2.2/joeflow/runner/celery.py` & `joeflow-1.2.3/joeflow/runner/celery.py`

 * *Files identical despite different names*

### Comparing `joeflow-1.2.2/joeflow/runner/dramatiq.py` & `joeflow-1.2.3/joeflow/runner/dramatiq.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     _dramatiq_task_runner.send_with_options(
         args=(task_pk, workflow_pk),
         delay=countdown,
         retries=retries,
     )
 
 
-class RetryError(Exception):
+class RetryError(dramatiq.errors.Retry):
     """Raised to retry a task if the task result is ``False``."""
 
     pass
 
 
 @dramatiq.actor(
     queue_name=settings.JOEFLOW_CELERY_QUEUE_NAME,
@@ -52,14 +52,18 @@
         except OperationalError:
             raise
         except:  # NoQA
             task.fail()
             logger.exception("Execution of %r failed", task)
         else:
             if result is False:
-                logger.info("Task returned False, retrying …")
+                _dramatiq_task_runner.logger.info("%r returned False, retrying …", task)
                 raise RetryError("Task returned False, retrying …")
             elif result is True:
                 result = None
-            logger.info("Task completed successful, starting next tasks: %s", result)
+            _dramatiq_task_runner.logger.info(
+                "%r completed successfully, starting next tasks: %s",
+                task,
+                result,
+            )
             task.start_next_tasks(next_nodes=result)
             task.finish()
```

### Comparing `joeflow-1.2.2/joeflow/tasks/human.py` & `joeflow-1.2.3/joeflow/tasks/human.py`

 * *Files identical despite different names*

### Comparing `joeflow-1.2.2/joeflow/tasks/machine.py` & `joeflow-1.2.3/joeflow/tasks/machine.py`

 * *Files identical despite different names*

### Comparing `joeflow-1.2.2/joeflow/utils.py` & `joeflow-1.2.3/joeflow/utils.py`

 * *Files identical despite different names*

### Comparing `joeflow-1.2.2/joeflow/views.py` & `joeflow-1.2.3/joeflow/views.py`

 * *Files identical despite different names*

### Comparing `joeflow-1.2.2/pyproject.toml` & `joeflow-1.2.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `joeflow-1.2.2/PKG-INFO` & `joeflow-1.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: joeflow
-Version: 1.2.2
+Version: 1.2.3
 Summary: The lean workflow automation framework for machines with heart.
 Keywords: django,process,automation,workflow,framework,task
 Author-email: Johannes Maron <johannes@maron.family>
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
```

