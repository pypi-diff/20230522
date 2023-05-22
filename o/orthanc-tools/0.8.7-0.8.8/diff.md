# Comparing `tmp/orthanc_tools-0.8.7.tar.gz` & `tmp/orthanc_tools-0.8.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "orthanc_tools-0.8.7.tar", last modified: Thu Apr 27 17:23:35 2023, max compression
+gzip compressed data, was "orthanc_tools-0.8.8.tar", last modified: Mon May 22 08:38:07 2023, max compression
```

## Comparing `orthanc_tools-0.8.7.tar` & `orthanc_tools-0.8.8.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:23:35.943842 orthanc_tools-0.8.7/
--rw-r--r--   0 runner    (1001) docker     (123)     7651 2023-04-27 17:21:05.000000 orthanc_tools-0.8.7/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-04-27 17:21:05.000000 orthanc_tools-0.8.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6286 2023-04-27 17:23:35.943842 orthanc_tools-0.8.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5278 2023-04-27 17:21:05.000000 orthanc_tools-0.8.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:23:35.935842 orthanc_tools-0.8.7/orthanc_tools/
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-04-27 17:21:05.000000 orthanc_tools-0.8.7/orthanc_tools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:23:35.935842 orthanc_tools-0.8.7/orthanc_tools/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-04-27 17:21:05.000000 orthanc_tools-0.8.7/orthanc_tools/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-04-27 17:21:05.000000 orthanc_tools-0.8.7/orthanc_tools/helpers/old_files_deleter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-04-27 17:21:05.000000 orthanc_tools-0.8.7/orthanc_tools/helpers/scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-04-27 17:21:05.000000 orthanc_tools-0.8.7/orthanc_tools/helpers/time_out.py
--rw-r--r--   0 runner    (1001) docker     (123)      763 2023-04-27 17:21:05.000000 orthanc_tools-0.8.7/orthanc_tools/helpers/timer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:23:35.943842 orthanc_tools-0.8.7/orthanc_tools/hl7Lib/
--rw-r--r--   0 runner    (1001) docker     (123)      654 2023-04-27 17:21:05.000000 orthanc_tools-0.8.7/orthanc_tools/hl7Lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-27 17:21:05.000000 orthanc_tools-0.8.7/orthanc_tools/hl7Lib/hl7.py
--rw-r--r--   0 runner    (1001) docker     (123)     3098 2023-04-27 17:21:05.000000 orthanc_tools-0.8.7/orthanc_tools/hl7Lib/hl7_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     8957 2023-04-27 17:21:05.000000 orthanc_tools-0.8.7/orthanc_tools/hl7Lib/hl7_dicom_worklist_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-04-27 17:21:05.000000 orthanc_tools-0.8.7/orthanc_tools/hl7Lib/hl7_error.py
--rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-04-27 17:21:05.000000 orthanc_tools-0.8.7/orthanc_tools/hl7Lib/hl7_message_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2123 2023-04-27 17:21:05.000000 orthanc_tools-0.8.7/orthanc_tools/hl7Lib/hl7_message_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2343 2023-04-27 17:21:05.000000 orthanc_tools-0.8.7/orthanc_tools/hl7Lib/hl7_orm_worklist_msg_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2422 2023-04-27 17:21:05.000000 orthanc_tools-0.8.7/orthanc_tools/hl7Lib/hl7_oru_report_msg_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-04-27 17:21:05.000000 orthanc_tools-0.8.7/orthanc_tools/hl7Lib/hl7_report_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1604 2023-04-27 17:21:05.000000 orthanc_tools-0.8.7/orthanc_tools/hl7Lib/hl7_report_series_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     9002 2023-04-27 17:21:05.000000 orthanc_tools-0.8.7/orthanc_tools/hl7Lib/hl7_server.py
--rw-r--r--   0 runner    (1001) docker     (123)     5736 2023-04-27 17:21:05.000000 orthanc_tools-0.8.7/orthanc_tools/hl7Lib/hl7_worklist_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     8355 2023-04-27 17:21:05.000000 orthanc_tools-0.8.7/orthanc_tools/orthanc_cloner.py
--rw-r--r--   0 runner    (1001) docker     (123)    17563 2023-04-27 17:21:05.000000 orthanc_tools-0.8.7/orthanc_tools/orthanc_comparator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-04-27 17:21:05.000000 orthanc_tools-0.8.7/orthanc_tools/orthanc_folder_importer.py
--rw-r--r--   0 runner    (1001) docker     (123)    17448 2023-04-27 17:21:05.000000 orthanc_tools-0.8.7/orthanc_tools/orthanc_forwarder.py
--rw-r--r--   0 runner    (1001) docker     (123)    10904 2023-04-27 17:21:05.000000 orthanc_tools-0.8.7/orthanc_tools/orthanc_monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)    10017 2023-04-27 17:21:05.000000 orthanc_tools-0.8.7/orthanc_tools/orthanc_test_db_populator.py
--rw-r--r--   0 runner    (1001) docker     (123)    15347 2023-04-27 17:21:05.000000 orthanc_tools-0.8.7/orthanc_tools/pacs_migrator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:23:35.935842 orthanc_tools-0.8.7/orthanc_tools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6286 2023-04-27 17:23:35.000000 orthanc_tools-0.8.7/orthanc_tools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-04-27 17:23:35.000000 orthanc_tools-0.8.7/orthanc_tools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 17:23:35.000000 orthanc_tools-0.8.7/orthanc_tools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-04-27 17:23:35.000000 orthanc_tools-0.8.7/orthanc_tools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-27 17:23:35.000000 orthanc_tools-0.8.7/orthanc_tools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-04-27 17:21:05.000000 orthanc_tools-0.8.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2612 2023-04-27 17:21:05.000000 orthanc_tools-0.8.7/release-notes.md
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-27 17:23:35.943842 orthanc_tools-0.8.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     6609 2023-04-27 17:21:05.000000 orthanc_tools-0.8.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:23:35.943842 orthanc_tools-0.8.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    18962 2023-04-27 17:21:05.000000 orthanc_tools-0.8.7/tests/test_3_orthancs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4275 2023-04-27 17:21:05.000000 orthanc_tools-0.8.7/tests/test_old_files_deleter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:38:07.549486 orthanc_tools-0.8.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     7651 2023-05-22 08:35:16.000000 orthanc_tools-0.8.8/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-05-22 08:35:16.000000 orthanc_tools-0.8.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6286 2023-05-22 08:38:07.549486 orthanc_tools-0.8.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5278 2023-05-22 08:35:16.000000 orthanc_tools-0.8.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:38:07.545486 orthanc_tools-0.8.8/orthanc_tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-05-22 08:35:16.000000 orthanc_tools-0.8.8/orthanc_tools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:38:07.549486 orthanc_tools-0.8.8/orthanc_tools/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-22 08:35:16.000000 orthanc_tools-0.8.8/orthanc_tools/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-05-22 08:35:16.000000 orthanc_tools-0.8.8/orthanc_tools/helpers/old_files_deleter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-05-22 08:35:16.000000 orthanc_tools-0.8.8/orthanc_tools/helpers/scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-05-22 08:35:16.000000 orthanc_tools-0.8.8/orthanc_tools/helpers/time_out.py
+-rw-r--r--   0 runner    (1001) docker     (123)      763 2023-05-22 08:35:16.000000 orthanc_tools-0.8.8/orthanc_tools/helpers/timer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:38:07.549486 orthanc_tools-0.8.8/orthanc_tools/hl7Lib/
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-05-22 08:35:16.000000 orthanc_tools-0.8.8/orthanc_tools/hl7Lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-22 08:35:16.000000 orthanc_tools-0.8.8/orthanc_tools/hl7Lib/hl7.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3098 2023-05-22 08:35:16.000000 orthanc_tools-0.8.8/orthanc_tools/hl7Lib/hl7_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8957 2023-05-22 08:35:16.000000 orthanc_tools-0.8.8/orthanc_tools/hl7Lib/hl7_dicom_worklist_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-05-22 08:35:16.000000 orthanc_tools-0.8.8/orthanc_tools/hl7Lib/hl7_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-05-22 08:35:16.000000 orthanc_tools-0.8.8/orthanc_tools/hl7Lib/hl7_message_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2123 2023-05-22 08:35:16.000000 orthanc_tools-0.8.8/orthanc_tools/hl7Lib/hl7_message_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2343 2023-05-22 08:35:16.000000 orthanc_tools-0.8.8/orthanc_tools/hl7Lib/hl7_orm_worklist_msg_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2422 2023-05-22 08:35:16.000000 orthanc_tools-0.8.8/orthanc_tools/hl7Lib/hl7_oru_report_msg_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-05-22 08:35:16.000000 orthanc_tools-0.8.8/orthanc_tools/hl7Lib/hl7_report_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1604 2023-05-22 08:35:16.000000 orthanc_tools-0.8.8/orthanc_tools/hl7Lib/hl7_report_series_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9002 2023-05-22 08:35:16.000000 orthanc_tools-0.8.8/orthanc_tools/hl7Lib/hl7_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5736 2023-05-22 08:35:16.000000 orthanc_tools-0.8.8/orthanc_tools/hl7Lib/hl7_worklist_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8355 2023-05-22 08:35:16.000000 orthanc_tools-0.8.8/orthanc_tools/orthanc_cloner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17563 2023-05-22 08:35:16.000000 orthanc_tools-0.8.8/orthanc_tools/orthanc_comparator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-05-22 08:35:16.000000 orthanc_tools-0.8.8/orthanc_tools/orthanc_folder_importer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17448 2023-05-22 08:35:16.000000 orthanc_tools-0.8.8/orthanc_tools/orthanc_forwarder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10891 2023-05-22 08:35:16.000000 orthanc_tools-0.8.8/orthanc_tools/orthanc_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10017 2023-05-22 08:35:16.000000 orthanc_tools-0.8.8/orthanc_tools/orthanc_test_db_populator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15347 2023-05-22 08:35:16.000000 orthanc_tools-0.8.8/orthanc_tools/pacs_migrator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:38:07.545486 orthanc_tools-0.8.8/orthanc_tools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6286 2023-05-22 08:38:07.000000 orthanc_tools-0.8.8/orthanc_tools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-05-22 08:38:07.000000 orthanc_tools-0.8.8/orthanc_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 08:38:07.000000 orthanc_tools-0.8.8/orthanc_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-22 08:38:07.000000 orthanc_tools-0.8.8/orthanc_tools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-22 08:38:07.000000 orthanc_tools-0.8.8/orthanc_tools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-05-22 08:35:16.000000 orthanc_tools-0.8.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2704 2023-05-22 08:35:16.000000 orthanc_tools-0.8.8/release-notes.md
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-22 08:38:07.549486 orthanc_tools-0.8.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     6609 2023-05-22 08:35:16.000000 orthanc_tools-0.8.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:38:07.549486 orthanc_tools-0.8.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    18962 2023-05-22 08:35:16.000000 orthanc_tools-0.8.8/tests/test_3_orthancs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4275 2023-05-22 08:35:16.000000 orthanc_tools-0.8.8/tests/test_old_files_deleter.py
```

### Comparing `orthanc_tools-0.8.7/LICENSE.txt` & `orthanc_tools-0.8.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `orthanc_tools-0.8.7/PKG-INFO` & `orthanc_tools-0.8.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: orthanc_tools
-Version: 0.8.7
+Version: 0.8.8
 Summary: Python Orthanc Tools
 Home-page: https://github.com/orthanc-team/python-orthanc-tools
 Author: Orthanc Team
 Author-email: info@orthanc.team
 Project-URL: Bug Reports, https://github.com/orthanc-team/python-orthanc-tools/issues
 Project-URL: Funding, https://orthanc.team
 Project-URL: Source, https://github.com/orthanc-team/python-orthanc-tools/
```

### Comparing `orthanc_tools-0.8.7/README.md` & `orthanc_tools-0.8.8/README.md`

 * *Files identical despite different names*

### Comparing `orthanc_tools-0.8.7/orthanc_tools/__init__.py` & `orthanc_tools-0.8.8/orthanc_tools/__init__.py`

 * *Files identical despite different names*

### Comparing `orthanc_tools-0.8.7/orthanc_tools/helpers/old_files_deleter.py` & `orthanc_tools-0.8.8/orthanc_tools/helpers/old_files_deleter.py`

 * *Files identical despite different names*

### Comparing `orthanc_tools-0.8.7/orthanc_tools/helpers/scheduler.py` & `orthanc_tools-0.8.8/orthanc_tools/helpers/scheduler.py`

 * *Files identical despite different names*

### Comparing `orthanc_tools-0.8.7/orthanc_tools/helpers/time_out.py` & `orthanc_tools-0.8.8/orthanc_tools/helpers/time_out.py`

 * *Files identical despite different names*

### Comparing `orthanc_tools-0.8.7/orthanc_tools/helpers/timer.py` & `orthanc_tools-0.8.8/orthanc_tools/helpers/timer.py`

 * *Files identical despite different names*

### Comparing `orthanc_tools-0.8.7/orthanc_tools/hl7Lib/__init__.py` & `orthanc_tools-0.8.8/orthanc_tools/hl7Lib/__init__.py`

 * *Files identical despite different names*

### Comparing `orthanc_tools-0.8.7/orthanc_tools/hl7Lib/hl7_client.py` & `orthanc_tools-0.8.8/orthanc_tools/hl7Lib/hl7_client.py`

 * *Files identical despite different names*

### Comparing `orthanc_tools-0.8.7/orthanc_tools/hl7Lib/hl7_dicom_worklist_builder.py` & `orthanc_tools-0.8.8/orthanc_tools/hl7Lib/hl7_dicom_worklist_builder.py`

 * *Files identical despite different names*

### Comparing `orthanc_tools-0.8.7/orthanc_tools/hl7Lib/hl7_error.py` & `orthanc_tools-0.8.8/orthanc_tools/hl7Lib/hl7_error.py`

 * *Files identical despite different names*

### Comparing `orthanc_tools-0.8.7/orthanc_tools/hl7Lib/hl7_message_parser.py` & `orthanc_tools-0.8.8/orthanc_tools/hl7Lib/hl7_message_parser.py`

 * *Files identical despite different names*

### Comparing `orthanc_tools-0.8.7/orthanc_tools/hl7Lib/hl7_message_validator.py` & `orthanc_tools-0.8.8/orthanc_tools/hl7Lib/hl7_message_validator.py`

 * *Files identical despite different names*

### Comparing `orthanc_tools-0.8.7/orthanc_tools/hl7Lib/hl7_orm_worklist_msg_handler.py` & `orthanc_tools-0.8.8/orthanc_tools/hl7Lib/hl7_orm_worklist_msg_handler.py`

 * *Files identical despite different names*

### Comparing `orthanc_tools-0.8.7/orthanc_tools/hl7Lib/hl7_oru_report_msg_handler.py` & `orthanc_tools-0.8.8/orthanc_tools/hl7Lib/hl7_oru_report_msg_handler.py`

 * *Files identical despite different names*

### Comparing `orthanc_tools-0.8.7/orthanc_tools/hl7Lib/hl7_report_parser.py` & `orthanc_tools-0.8.8/orthanc_tools/hl7Lib/hl7_report_parser.py`

 * *Files identical despite different names*

### Comparing `orthanc_tools-0.8.7/orthanc_tools/hl7Lib/hl7_report_series_builder.py` & `orthanc_tools-0.8.8/orthanc_tools/hl7Lib/hl7_report_series_builder.py`

 * *Files identical despite different names*

### Comparing `orthanc_tools-0.8.7/orthanc_tools/hl7Lib/hl7_server.py` & `orthanc_tools-0.8.8/orthanc_tools/hl7Lib/hl7_server.py`

 * *Files identical despite different names*

### Comparing `orthanc_tools-0.8.7/orthanc_tools/hl7Lib/hl7_worklist_parser.py` & `orthanc_tools-0.8.8/orthanc_tools/hl7Lib/hl7_worklist_parser.py`

 * *Files identical despite different names*

### Comparing `orthanc_tools-0.8.7/orthanc_tools/orthanc_cloner.py` & `orthanc_tools-0.8.8/orthanc_tools/orthanc_cloner.py`

 * *Files identical despite different names*

### Comparing `orthanc_tools-0.8.7/orthanc_tools/orthanc_comparator.py` & `orthanc_tools-0.8.8/orthanc_tools/orthanc_comparator.py`

 * *Files identical despite different names*

### Comparing `orthanc_tools-0.8.7/orthanc_tools/orthanc_folder_importer.py` & `orthanc_tools-0.8.8/orthanc_tools/orthanc_folder_importer.py`

 * *Files identical despite different names*

### Comparing `orthanc_tools-0.8.7/orthanc_tools/orthanc_forwarder.py` & `orthanc_tools-0.8.8/orthanc_tools/orthanc_forwarder.py`

 * *Files identical despite different names*

### Comparing `orthanc_tools-0.8.7/orthanc_tools/orthanc_monitor.py` & `orthanc_tools-0.8.8/orthanc_tools/orthanc_monitor.py`

 * *Files 0% similar despite different names*

```diff
@@ -162,15 +162,15 @@
                 return
 
             done = False
 
             while not done and self._is_running:  # read as fast as you can while there are still events
 
                 if self._scheduler:
-                    self._scheduler.wait_right_time_to_run(logger=logger)
+                    self._scheduler.wait_right_time_to_run()
 
                 # get the list of changes from orthanc
                 try:
                     changes, last_sequence_id, done = self._api_client.get_changes(
                         since=last_sequence_id,
                         limit=100
                     )
```

### Comparing `orthanc_tools-0.8.7/orthanc_tools/orthanc_test_db_populator.py` & `orthanc_tools-0.8.8/orthanc_tools/orthanc_test_db_populator.py`

 * *Files identical despite different names*

### Comparing `orthanc_tools-0.8.7/orthanc_tools/pacs_migrator.py` & `orthanc_tools-0.8.8/orthanc_tools/pacs_migrator.py`

 * *Files identical despite different names*

### Comparing `orthanc_tools-0.8.7/orthanc_tools.egg-info/PKG-INFO` & `orthanc_tools-0.8.8/orthanc_tools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: orthanc-tools
-Version: 0.8.7
+Version: 0.8.8
 Summary: Python Orthanc Tools
 Home-page: https://github.com/orthanc-team/python-orthanc-tools
 Author: Orthanc Team
 Author-email: info@orthanc.team
 Project-URL: Bug Reports, https://github.com/orthanc-team/python-orthanc-tools/issues
 Project-URL: Funding, https://orthanc.team
 Project-URL: Source, https://github.com/orthanc-team/python-orthanc-tools/
```

### Comparing `orthanc_tools-0.8.7/orthanc_tools.egg-info/SOURCES.txt` & `orthanc_tools-0.8.8/orthanc_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `orthanc_tools-0.8.7/release-notes.md` & `orthanc_tools-0.8.8/release-notes.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,17 @@
+v 0.8.8
+=======
+
+- `OrthancMonitor`: fixed monitor
+
+v 0.8.7
+=======
+
+- Forget it
+
 v 0.8.6
 =======
 
 - `OrthancTestDbPopulator`: new feature: number of series/instances
 
 v 0.8.5
 =======
```

### Comparing `orthanc_tools-0.8.7/setup.py` & `orthanc_tools-0.8.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
     # Versions should comply with PEP 440:
     # https://www.python.org/dev/peps/pep-0440/
     #
     # For a discussion on single-sourcing the version across setup.py and the
     # project code, see
     # https://packaging.python.org/guides/single-sourcing-package-version/
-    version='0.8.7',  # Required
+    version='0.8.8',  # Required
 
     # This is a one-line description or tagline of what your project does. This
     # corresponds to the "Summary" metadata field:
     # https://packaging.python.org/specifications/core-metadata/#summary
     description='Python Orthanc Tools',  # Optional
 
     # This is an optional longer description of your project that represents
```

### Comparing `orthanc_tools-0.8.7/tests/test_3_orthancs.py` & `orthanc_tools-0.8.8/tests/test_3_orthancs.py`

 * *Files identical despite different names*

### Comparing `orthanc_tools-0.8.7/tests/test_old_files_deleter.py` & `orthanc_tools-0.8.8/tests/test_old_files_deleter.py`

 * *Files identical despite different names*

