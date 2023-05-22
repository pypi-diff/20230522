# Comparing `tmp/app_transport_framework_library-0.1.2.tar.gz` & `tmp/app_transport_framework_library-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "app_transport_framework_library-0.1.2.tar", max compression
+gzip compressed data, was "app_transport_framework_library-0.1.3.tar", max compression
```

## Comparing `app_transport_framework_library-0.1.2.tar` & `app_transport_framework_library-0.1.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     3846 2023-05-16 22:12:18.801764 app_transport_framework_library-0.1.2/README.md
--rw-r--r--   0        0        0        0 2023-05-16 20:50:56.861597 app_transport_framework_library-0.1.2/app_transport_framework_library/__init__.py
--rw-r--r--   0        0        0     6555 2023-05-16 21:05:07.926034 app_transport_framework_library-0.1.2/app_transport_framework_library/atf_bundle_processor.py
--rw-r--r--   0        0        0      824 2023-05-16 21:36:51.746182 app_transport_framework_library-0.1.2/app_transport_framework_library/base_use_case_handler.py
--rw-r--r--   0        0        0      279 2023-05-16 21:02:55.215837 app_transport_framework_library-0.1.2/app_transport_framework_library/models/bundle_focus_content.py
--rw-r--r--   0        0        0      393 2023-05-16 20:49:20.422907 app_transport_framework_library-0.1.2/app_transport_framework_library/models/empfangsbestaetigung.py
--rw-r--r--   0        0        0      350 2023-05-16 20:49:20.422907 app_transport_framework_library-0.1.2/app_transport_framework_library/models/event.py
--rw-r--r--   0        0        0      295 2023-05-16 20:49:20.422907 app_transport_framework_library-0.1.2/app_transport_framework_library/models/message_to_send.py
--rw-r--r--   0        0        0     1138 2023-05-16 21:02:46.011962 app_transport_framework_library-0.1.2/app_transport_framework_library/ressource_creators/message_bundle_creator.py
--rw-r--r--   0        0        0     1197 2023-05-16 20:49:20.422907 app_transport_framework_library-0.1.2/app_transport_framework_library/ressource_creators/message_header_creator.py
--rw-r--r--   0        0        0     1780 2023-05-16 21:03:31.391345 app_transport_framework_library-0.1.2/app_transport_framework_library/ressource_creators/operation_outcome_bundle_creator.py
--rw-r--r--   0        0        0      838 2023-05-16 20:49:20.422907 app_transport_framework_library-0.1.2/app_transport_framework_library/ressource_creators/operation_outcome_creator.py
--rw-r--r--   0        0        0     3905 2023-05-16 21:06:16.989096 app_transport_framework_library-0.1.2/app_transport_framework_library/ressource_creators/test_message_creator.py
--rw-r--r--   0        0        0     1613 2023-05-16 21:38:28.224802 app_transport_framework_library-0.1.2/app_transport_framework_library/use_cases/empfangsbestaetigung_handler.py
--rw-r--r--   0        0        0     1931 2023-05-16 21:39:27.990263 app_transport_framework_library-0.1.2/app_transport_framework_library/use_cases/selbsttest_lieferung_handler.py
--rw-r--r--   0        0        0      377 2023-05-16 22:12:45.733987 app_transport_framework_library-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     4355 1970-01-01 00:00:00.000000 app_transport_framework_library-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     3846 2023-05-16 22:12:18.801764 app_transport_framework_library-0.1.3/README.md
+-rw-r--r--   0        0        0        0 2023-05-16 20:50:56.861597 app_transport_framework_library-0.1.3/app_transport_framework_library/__init__.py
+-rw-r--r--   0        0        0     6555 2023-05-16 21:05:07.926034 app_transport_framework_library-0.1.3/app_transport_framework_library/atf_bundle_processor.py
+-rw-r--r--   0        0        0      824 2023-05-16 21:36:51.746182 app_transport_framework_library-0.1.3/app_transport_framework_library/base_use_case_handler.py
+-rw-r--r--   0        0        0      279 2023-05-16 21:02:55.215837 app_transport_framework_library-0.1.3/app_transport_framework_library/models/bundle_focus_content.py
+-rw-r--r--   0        0        0      393 2023-05-16 20:49:20.422907 app_transport_framework_library-0.1.3/app_transport_framework_library/models/empfangsbestaetigung.py
+-rw-r--r--   0        0        0      350 2023-05-16 20:49:20.422907 app_transport_framework_library-0.1.3/app_transport_framework_library/models/event.py
+-rw-r--r--   0        0        0      295 2023-05-16 20:49:20.422907 app_transport_framework_library-0.1.3/app_transport_framework_library/models/message_to_send.py
+-rw-r--r--   0        0        0     1138 2023-05-16 21:02:46.011962 app_transport_framework_library-0.1.3/app_transport_framework_library/ressource_creators/message_bundle_creator.py
+-rw-r--r--   0        0        0     1197 2023-05-16 20:49:20.422907 app_transport_framework_library-0.1.3/app_transport_framework_library/ressource_creators/message_header_creator.py
+-rw-r--r--   0        0        0     1780 2023-05-16 21:03:31.391345 app_transport_framework_library-0.1.3/app_transport_framework_library/ressource_creators/operation_outcome_bundle_creator.py
+-rw-r--r--   0        0        0      838 2023-05-16 20:49:20.422907 app_transport_framework_library-0.1.3/app_transport_framework_library/ressource_creators/operation_outcome_creator.py
+-rw-r--r--   0        0        0     3905 2023-05-16 21:06:16.989096 app_transport_framework_library-0.1.3/app_transport_framework_library/ressource_creators/test_message_creator.py
+-rw-r--r--   0        0        0     1613 2023-05-16 21:38:28.224802 app_transport_framework_library-0.1.3/app_transport_framework_library/use_cases/empfangsbestaetigung_handler.py
+-rw-r--r--   0        0        0     1931 2023-05-16 21:39:27.990263 app_transport_framework_library-0.1.3/app_transport_framework_library/use_cases/selbsttest_lieferung_handler.py
+-rw-r--r--   0        0        0      375 2023-05-22 21:26:06.304416 app_transport_framework_library-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     4348 1970-01-01 00:00:00.000000 app_transport_framework_library-0.1.3/PKG-INFO
```

### Comparing `app_transport_framework_library-0.1.2/README.md` & `app_transport_framework_library-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `app_transport_framework_library-0.1.2/app_transport_framework_library/atf_bundle_processor.py` & `app_transport_framework_library-0.1.3/app_transport_framework_library/atf_bundle_processor.py`

 * *Files identical despite different names*

### Comparing `app_transport_framework_library-0.1.2/app_transport_framework_library/base_use_case_handler.py` & `app_transport_framework_library-0.1.3/app_transport_framework_library/base_use_case_handler.py`

 * *Files identical despite different names*

### Comparing `app_transport_framework_library-0.1.2/app_transport_framework_library/ressource_creators/message_bundle_creator.py` & `app_transport_framework_library-0.1.3/app_transport_framework_library/ressource_creators/message_bundle_creator.py`

 * *Files identical despite different names*

### Comparing `app_transport_framework_library-0.1.2/app_transport_framework_library/ressource_creators/message_header_creator.py` & `app_transport_framework_library-0.1.3/app_transport_framework_library/ressource_creators/message_header_creator.py`

 * *Files identical despite different names*

### Comparing `app_transport_framework_library-0.1.2/app_transport_framework_library/ressource_creators/operation_outcome_bundle_creator.py` & `app_transport_framework_library-0.1.3/app_transport_framework_library/ressource_creators/operation_outcome_bundle_creator.py`

 * *Files identical despite different names*

### Comparing `app_transport_framework_library-0.1.2/app_transport_framework_library/ressource_creators/operation_outcome_creator.py` & `app_transport_framework_library-0.1.3/app_transport_framework_library/ressource_creators/operation_outcome_creator.py`

 * *Files identical despite different names*

### Comparing `app_transport_framework_library-0.1.2/app_transport_framework_library/ressource_creators/test_message_creator.py` & `app_transport_framework_library-0.1.3/app_transport_framework_library/ressource_creators/test_message_creator.py`

 * *Files identical despite different names*

### Comparing `app_transport_framework_library-0.1.2/app_transport_framework_library/use_cases/empfangsbestaetigung_handler.py` & `app_transport_framework_library-0.1.3/app_transport_framework_library/use_cases/empfangsbestaetigung_handler.py`

 * *Files identical despite different names*

### Comparing `app_transport_framework_library-0.1.2/app_transport_framework_library/use_cases/selbsttest_lieferung_handler.py` & `app_transport_framework_library-0.1.3/app_transport_framework_library/use_cases/selbsttest_lieferung_handler.py`

 * *Files identical despite different names*

### Comparing `app_transport_framework_library-0.1.2/PKG-INFO` & `app_transport_framework_library-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: app-transport-framework-library
-Version: 0.1.2
+Version: 0.1.3
 Summary: 
 Author: Sven Sommer
 Author-email: rob.hoffmann@posteo.de
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: fhir-resources (>=7.0.0,<8.0.0)
+Requires-Dist: fhir-resources (==6.1.0)
 Description-Content-Type: text/markdown
 
 # ATF Library
 
 Die App-Transport-Framework (ATF) Library ist eine Python-Bibliothek zur Verarbeitung und Handhabung von ATF-Nachrichten (<https://simplifier.net/app-transport-framework>) im FHIR-Format. Die Bibliothek bietet eine einfache Möglichkeit, verschiedene Anwendungsfälle und ihre zugehörigen Handler zu registrieren und zu verwalten.
 
 ## Installation
```

