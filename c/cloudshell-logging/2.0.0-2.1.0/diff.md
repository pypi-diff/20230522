# Comparing `tmp/cloudshell-logging-2.0.0.zip` & `tmp/cloudshell-logging-2.1.0.zip`

## zipinfo {}

```diff
@@ -1,57 +1,57 @@
-Zip file size: 48822 bytes, number of entries: 55
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-04 15:50 cloudshell-logging-2.0.0/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-04 15:50 cloudshell-logging-2.0.0/cloudshell/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-04 15:50 cloudshell-logging-2.0.0/tests/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-04 15:50 cloudshell-logging-2.0.0/cloudshell_logging.egg-info/
--rw-r--r--  2.0 unx    97622 b- defN 23-May-04 15:50 cloudshell-logging-2.0.0/LICENSE.htm
--rw-r--r--  2.0 unx       18 b- defN 23-May-04 15:50 cloudshell-logging-2.0.0/test_requirements.txt
--rw-r--r--  2.0 unx        5 b- defN 23-May-04 15:50 cloudshell-logging-2.0.0/version.txt
--rw-r--r--  2.0 unx       38 b- defN 23-May-04 15:50 cloudshell-logging-2.0.0/setup.cfg
--rw-r--r--  2.0 unx        0 b- defN 23-May-04 15:50 cloudshell-logging-2.0.0/requirements.txt
--rw-r--r--  2.0 unx      776 b- defN 23-May-04 15:50 cloudshell-logging-2.0.0/setup.py
--rw-r--r--  2.0 unx       71 b- defN 23-May-04 15:50 cloudshell-logging-2.0.0/dev_requirements.txt
--rw-r--r--  2.0 unx     4723 b- defN 23-May-04 15:50 cloudshell-logging-2.0.0/README.md
--rw-r--r--  2.0 unx     1016 b- defN 23-May-04 15:50 cloudshell-logging-2.0.0/tox.ini
--rw-r--r--  2.0 unx       34 b- defN 23-May-04 15:50 cloudshell-logging-2.0.0/MANIFEST.in
--rw-r--r--  2.0 unx      254 b- defN 23-May-04 15:50 cloudshell-logging-2.0.0/PKG-INFO
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-04 15:50 cloudshell-logging-2.0.0/cloudshell/logging/
--rw-r--r--  2.0 unx       76 b- defN 23-May-04 15:50 cloudshell-logging-2.0.0/cloudshell/__init__.py
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-04 15:50 cloudshell-logging-2.0.0/cloudshell/logging/utils/
--rw-r--r--  2.0 unx    13248 b- defN 23-May-04 15:50 cloudshell-logging-2.0.0/cloudshell/logging/qs_logger.py
--rw-r--r--  2.0 unx      970 b- defN 23-May-04 15:50 cloudshell-logging-2.0.0/cloudshell/logging/qs_config_parser.py
--rw-r--r--  2.0 unx     1537 b- defN 23-May-04 15:50 cloudshell-logging-2.0.0/cloudshell/logging/context_filters.py
--rw-r--r--  2.0 unx        0 b- defN 23-May-04 15:50 cloudshell-logging-2.0.0/cloudshell/logging/__init__.py
--rw-r--r--  2.0 unx     1648 b- defN 23-May-04 15:50 cloudshell-logging-2.0.0/cloudshell/logging/memory_handler.py
--rw-r--r--  2.0 unx      712 b- defN 23-May-04 15:50 cloudshell-logging-2.0.0/cloudshell/logging/qs_config.ini
--rw-r--r--  2.0 unx      198 b- defN 23-May-04 15:50 cloudshell-logging-2.0.0/cloudshell/logging/utils/venv.py
--rw-r--r--  2.0 unx      927 b- defN 23-May-04 15:50 cloudshell-logging-2.0.0/cloudshell/logging/utils/patch_logging_shutdown.py
--rw-r--r--  2.0 unx     1088 b- defN 23-May-04 15:50 cloudshell-logging-2.0.0/cloudshell/logging/utils/error_handling_context_manager.py
--rw-r--r--  2.0 unx        0 b- defN 23-May-04 15:50 cloudshell-logging-2.0.0/cloudshell/logging/utils/__init__.py
--rw-r--r--  2.0 unx      681 b- defN 23-May-04 15:50 cloudshell-logging-2.0.0/cloudshell/logging/utils/decorators.py
--rw-r--r--  2.0 unx     1020 b- defN 23-May-04 15:50 cloudshell-logging-2.0.0/cloudshell/logging/utils/log_exec_info.py
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-04 15:50 cloudshell-logging-2.0.0/tests/logging/
--rw-r--r--  2.0 unx        0 b- defN 23-May-04 15:50 cloudshell-logging-2.0.0/tests/__init__.py
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-04 15:50 cloudshell-logging-2.0.0/tests/logging/test_logger_in_threads/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-04 15:50 cloudshell-logging-2.0.0/tests/logging/utils/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-04 15:50 cloudshell-logging-2.0.0/tests/logging/test_debug_logs/
--rw-r--r--  2.0 unx      287 b- defN 23-May-04 15:50 cloudshell-logging-2.0.0/tests/logging/conftest.py
--rw-r--r--  2.0 unx     2505 b- defN 23-May-04 15:50 cloudshell-logging-2.0.0/tests/logging/test_memory_handler.py
--rw-r--r--  2.0 unx     2290 b- defN 23-May-04 15:50 cloudshell-logging-2.0.0/tests/logging/test_qs_config_parser.py
--rw-r--r--  2.0 unx    12256 b- defN 23-May-04 15:50 cloudshell-logging-2.0.0/tests/logging/test_qs_logger.py
--rw-r--r--  2.0 unx        0 b- defN 23-May-04 15:50 cloudshell-logging-2.0.0/tests/logging/__init__.py
--rw-r--r--  2.0 unx      297 b- defN 23-May-04 15:50 cloudshell-logging-2.0.0/tests/logging/test_qs_config.ini
--rw-r--r--  2.0 unx     1815 b- defN 23-May-04 15:50 cloudshell-logging-2.0.0/tests/logging/test_log_exec_info.py
--rw-r--r--  2.0 unx     5264 b- defN 23-May-04 15:50 cloudshell-logging-2.0.0/tests/logging/test_logger_in_threads/test_getting_logger.py
--rw-r--r--  2.0 unx      163 b- defN 23-May-04 15:50 cloudshell-logging-2.0.0/tests/logging/test_logger_in_threads/package_file.py
--rw-r--r--  2.0 unx        0 b- defN 23-May-04 15:50 cloudshell-logging-2.0.0/tests/logging/test_logger_in_threads/__init__.py
--rw-r--r--  2.0 unx     1750 b- defN 23-May-04 15:50 cloudshell-logging-2.0.0/tests/logging/utils/test_command_logging.py
--rw-r--r--  2.0 unx      923 b- defN 23-May-04 15:50 cloudshell-logging-2.0.0/tests/logging/utils/test_error_handling_context_manager.py
--rw-r--r--  2.0 unx        0 b- defN 23-May-04 15:50 cloudshell-logging-2.0.0/tests/logging/utils/__init__.py
--rw-r--r--  2.0 unx      388 b- defN 23-May-04 15:50 cloudshell-logging-2.0.0/tests/logging/test_debug_logs/package_file.py
--rw-r--r--  2.0 unx        0 b- defN 23-May-04 15:50 cloudshell-logging-2.0.0/tests/logging/test_debug_logs/__init__.py
--rw-r--r--  2.0 unx     1945 b- defN 23-May-04 15:50 cloudshell-logging-2.0.0/tests/logging/test_debug_logs/test_debug_logs_on_error.py
--rw-r--r--  2.0 unx       17 b- defN 23-May-04 15:50 cloudshell-logging-2.0.0/cloudshell_logging.egg-info/top_level.txt
--rw-r--r--  2.0 unx     1474 b- defN 23-May-04 15:50 cloudshell-logging-2.0.0/cloudshell_logging.egg-info/SOURCES.txt
--rw-r--r--  2.0 unx      254 b- defN 23-May-04 15:50 cloudshell-logging-2.0.0/cloudshell_logging.egg-info/PKG-INFO
--rw-r--r--  2.0 unx        1 b- defN 23-May-04 15:50 cloudshell-logging-2.0.0/cloudshell_logging.egg-info/dependency_links.txt
-55 files, 158291 bytes uncompressed, 38592 bytes compressed:  75.6%
+Zip file size: 48940 bytes, number of entries: 55
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-22 15:00 cloudshell-logging-2.1.0/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-22 15:00 cloudshell-logging-2.1.0/tests/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-22 15:00 cloudshell-logging-2.1.0/cloudshell/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-22 15:00 cloudshell-logging-2.1.0/cloudshell_logging.egg-info/
+-rw-r--r--  2.0 unx     4723 b- defN 23-May-22 15:00 cloudshell-logging-2.1.0/README.md
+-rw-r--r--  2.0 unx       18 b- defN 23-May-22 15:00 cloudshell-logging-2.1.0/test_requirements.txt
+-rw-r--r--  2.0 unx        6 b- defN 23-May-22 15:00 cloudshell-logging-2.1.0/version.txt
+-rw-r--r--  2.0 unx    97622 b- defN 23-May-22 15:00 cloudshell-logging-2.1.0/LICENSE.htm
+-rw-r--r--  2.0 unx       34 b- defN 23-May-22 15:00 cloudshell-logging-2.1.0/MANIFEST.in
+-rw-r--r--  2.0 unx        0 b- defN 23-May-22 15:00 cloudshell-logging-2.1.0/requirements.txt
+-rw-r--r--  2.0 unx      254 b- defN 23-May-22 15:00 cloudshell-logging-2.1.0/PKG-INFO
+-rw-r--r--  2.0 unx      776 b- defN 23-May-22 15:00 cloudshell-logging-2.1.0/setup.py
+-rw-r--r--  2.0 unx       71 b- defN 23-May-22 15:00 cloudshell-logging-2.1.0/dev_requirements.txt
+-rw-r--r--  2.0 unx     1016 b- defN 23-May-22 15:00 cloudshell-logging-2.1.0/tox.ini
+-rw-r--r--  2.0 unx       38 b- defN 23-May-22 15:00 cloudshell-logging-2.1.0/setup.cfg
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-22 15:00 cloudshell-logging-2.1.0/tests/logging/
+-rw-r--r--  2.0 unx        0 b- defN 23-May-22 15:00 cloudshell-logging-2.1.0/tests/__init__.py
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-22 15:00 cloudshell-logging-2.1.0/tests/logging/utils/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-22 15:00 cloudshell-logging-2.1.0/tests/logging/test_debug_logs/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-22 15:00 cloudshell-logging-2.1.0/tests/logging/test_logger_in_threads/
+-rw-r--r--  2.0 unx     2505 b- defN 23-May-22 15:00 cloudshell-logging-2.1.0/tests/logging/test_memory_handler.py
+-rw-r--r--  2.0 unx     2290 b- defN 23-May-22 15:00 cloudshell-logging-2.1.0/tests/logging/test_qs_config_parser.py
+-rw-r--r--  2.0 unx    12256 b- defN 23-May-22 15:00 cloudshell-logging-2.1.0/tests/logging/test_qs_logger.py
+-rw-r--r--  2.0 unx     1815 b- defN 23-May-22 15:00 cloudshell-logging-2.1.0/tests/logging/test_log_exec_info.py
+-rw-r--r--  2.0 unx      287 b- defN 23-May-22 15:00 cloudshell-logging-2.1.0/tests/logging/conftest.py
+-rw-r--r--  2.0 unx        0 b- defN 23-May-22 15:00 cloudshell-logging-2.1.0/tests/logging/__init__.py
+-rw-r--r--  2.0 unx      297 b- defN 23-May-22 15:00 cloudshell-logging-2.1.0/tests/logging/test_qs_config.ini
+-rw-r--r--  2.0 unx      923 b- defN 23-May-22 15:00 cloudshell-logging-2.1.0/tests/logging/utils/test_error_handling_context_manager.py
+-rw-r--r--  2.0 unx        0 b- defN 23-May-22 15:00 cloudshell-logging-2.1.0/tests/logging/utils/__init__.py
+-rw-r--r--  2.0 unx     1750 b- defN 23-May-22 15:00 cloudshell-logging-2.1.0/tests/logging/utils/test_command_logging.py
+-rw-r--r--  2.0 unx     1945 b- defN 23-May-22 15:00 cloudshell-logging-2.1.0/tests/logging/test_debug_logs/test_debug_logs_on_error.py
+-rw-r--r--  2.0 unx        0 b- defN 23-May-22 15:00 cloudshell-logging-2.1.0/tests/logging/test_debug_logs/__init__.py
+-rw-r--r--  2.0 unx      388 b- defN 23-May-22 15:00 cloudshell-logging-2.1.0/tests/logging/test_debug_logs/package_file.py
+-rw-r--r--  2.0 unx     5264 b- defN 23-May-22 15:00 cloudshell-logging-2.1.0/tests/logging/test_logger_in_threads/test_getting_logger.py
+-rw-r--r--  2.0 unx        0 b- defN 23-May-22 15:00 cloudshell-logging-2.1.0/tests/logging/test_logger_in_threads/__init__.py
+-rw-r--r--  2.0 unx      163 b- defN 23-May-22 15:00 cloudshell-logging-2.1.0/tests/logging/test_logger_in_threads/package_file.py
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-22 15:00 cloudshell-logging-2.1.0/cloudshell/logging/
+-rw-r--r--  2.0 unx       76 b- defN 23-May-22 15:00 cloudshell-logging-2.1.0/cloudshell/__init__.py
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-22 15:00 cloudshell-logging-2.1.0/cloudshell/logging/utils/
+-rw-r--r--  2.0 unx     1537 b- defN 23-May-22 15:00 cloudshell-logging-2.1.0/cloudshell/logging/context_filters.py
+-rw-r--r--  2.0 unx        0 b- defN 23-May-22 15:00 cloudshell-logging-2.1.0/cloudshell/logging/__init__.py
+-rw-r--r--  2.0 unx    13794 b- defN 23-May-22 15:00 cloudshell-logging-2.1.0/cloudshell/logging/qs_logger.py
+-rw-r--r--  2.0 unx      712 b- defN 23-May-22 15:00 cloudshell-logging-2.1.0/cloudshell/logging/qs_config.ini
+-rw-r--r--  2.0 unx     1648 b- defN 23-May-22 15:00 cloudshell-logging-2.1.0/cloudshell/logging/memory_handler.py
+-rw-r--r--  2.0 unx      970 b- defN 23-May-22 15:00 cloudshell-logging-2.1.0/cloudshell/logging/qs_config_parser.py
+-rw-r--r--  2.0 unx     1088 b- defN 23-May-22 15:00 cloudshell-logging-2.1.0/cloudshell/logging/utils/error_handling_context_manager.py
+-rw-r--r--  2.0 unx      681 b- defN 23-May-22 15:00 cloudshell-logging-2.1.0/cloudshell/logging/utils/decorators.py
+-rw-r--r--  2.0 unx      198 b- defN 23-May-22 15:00 cloudshell-logging-2.1.0/cloudshell/logging/utils/venv.py
+-rw-r--r--  2.0 unx        0 b- defN 23-May-22 15:00 cloudshell-logging-2.1.0/cloudshell/logging/utils/__init__.py
+-rw-r--r--  2.0 unx     1020 b- defN 23-May-22 15:00 cloudshell-logging-2.1.0/cloudshell/logging/utils/log_exec_info.py
+-rw-r--r--  2.0 unx      927 b- defN 23-May-22 15:00 cloudshell-logging-2.1.0/cloudshell/logging/utils/patch_logging_shutdown.py
+-rw-r--r--  2.0 unx        1 b- defN 23-May-22 15:00 cloudshell-logging-2.1.0/cloudshell_logging.egg-info/dependency_links.txt
+-rw-r--r--  2.0 unx       17 b- defN 23-May-22 15:00 cloudshell-logging-2.1.0/cloudshell_logging.egg-info/top_level.txt
+-rw-r--r--  2.0 unx      254 b- defN 23-May-22 15:00 cloudshell-logging-2.1.0/cloudshell_logging.egg-info/PKG-INFO
+-rw-r--r--  2.0 unx     1474 b- defN 23-May-22 15:00 cloudshell-logging-2.1.0/cloudshell_logging.egg-info/SOURCES.txt
+55 files, 158838 bytes uncompressed, 38710 bytes compressed:  75.6%
```

## zipnote {}

```diff
@@ -1,166 +1,166 @@
-Filename: cloudshell-logging-2.0.0/
+Filename: cloudshell-logging-2.1.0/
 Comment: 
 
-Filename: cloudshell-logging-2.0.0/cloudshell/
+Filename: cloudshell-logging-2.1.0/tests/
 Comment: 
 
-Filename: cloudshell-logging-2.0.0/tests/
+Filename: cloudshell-logging-2.1.0/cloudshell/
 Comment: 
 
-Filename: cloudshell-logging-2.0.0/cloudshell_logging.egg-info/
+Filename: cloudshell-logging-2.1.0/cloudshell_logging.egg-info/
 Comment: 
 
-Filename: cloudshell-logging-2.0.0/LICENSE.htm
+Filename: cloudshell-logging-2.1.0/README.md
 Comment: 
 
-Filename: cloudshell-logging-2.0.0/test_requirements.txt
+Filename: cloudshell-logging-2.1.0/test_requirements.txt
 Comment: 
 
-Filename: cloudshell-logging-2.0.0/version.txt
+Filename: cloudshell-logging-2.1.0/version.txt
 Comment: 
 
-Filename: cloudshell-logging-2.0.0/setup.cfg
+Filename: cloudshell-logging-2.1.0/LICENSE.htm
 Comment: 
 
-Filename: cloudshell-logging-2.0.0/requirements.txt
+Filename: cloudshell-logging-2.1.0/MANIFEST.in
 Comment: 
 
-Filename: cloudshell-logging-2.0.0/setup.py
+Filename: cloudshell-logging-2.1.0/requirements.txt
 Comment: 
 
-Filename: cloudshell-logging-2.0.0/dev_requirements.txt
+Filename: cloudshell-logging-2.1.0/PKG-INFO
 Comment: 
 
-Filename: cloudshell-logging-2.0.0/README.md
+Filename: cloudshell-logging-2.1.0/setup.py
 Comment: 
 
-Filename: cloudshell-logging-2.0.0/tox.ini
+Filename: cloudshell-logging-2.1.0/dev_requirements.txt
 Comment: 
 
-Filename: cloudshell-logging-2.0.0/MANIFEST.in
+Filename: cloudshell-logging-2.1.0/tox.ini
 Comment: 
 
-Filename: cloudshell-logging-2.0.0/PKG-INFO
+Filename: cloudshell-logging-2.1.0/setup.cfg
 Comment: 
 
-Filename: cloudshell-logging-2.0.0/cloudshell/logging/
+Filename: cloudshell-logging-2.1.0/tests/logging/
 Comment: 
 
-Filename: cloudshell-logging-2.0.0/cloudshell/__init__.py
+Filename: cloudshell-logging-2.1.0/tests/__init__.py
 Comment: 
 
-Filename: cloudshell-logging-2.0.0/cloudshell/logging/utils/
+Filename: cloudshell-logging-2.1.0/tests/logging/utils/
 Comment: 
 
-Filename: cloudshell-logging-2.0.0/cloudshell/logging/qs_logger.py
+Filename: cloudshell-logging-2.1.0/tests/logging/test_debug_logs/
 Comment: 
 
-Filename: cloudshell-logging-2.0.0/cloudshell/logging/qs_config_parser.py
+Filename: cloudshell-logging-2.1.0/tests/logging/test_logger_in_threads/
 Comment: 
 
-Filename: cloudshell-logging-2.0.0/cloudshell/logging/context_filters.py
+Filename: cloudshell-logging-2.1.0/tests/logging/test_memory_handler.py
 Comment: 
 
-Filename: cloudshell-logging-2.0.0/cloudshell/logging/__init__.py
+Filename: cloudshell-logging-2.1.0/tests/logging/test_qs_config_parser.py
 Comment: 
 
-Filename: cloudshell-logging-2.0.0/cloudshell/logging/memory_handler.py
+Filename: cloudshell-logging-2.1.0/tests/logging/test_qs_logger.py
 Comment: 
 
-Filename: cloudshell-logging-2.0.0/cloudshell/logging/qs_config.ini
+Filename: cloudshell-logging-2.1.0/tests/logging/test_log_exec_info.py
 Comment: 
 
-Filename: cloudshell-logging-2.0.0/cloudshell/logging/utils/venv.py
+Filename: cloudshell-logging-2.1.0/tests/logging/conftest.py
 Comment: 
 
-Filename: cloudshell-logging-2.0.0/cloudshell/logging/utils/patch_logging_shutdown.py
+Filename: cloudshell-logging-2.1.0/tests/logging/__init__.py
 Comment: 
 
-Filename: cloudshell-logging-2.0.0/cloudshell/logging/utils/error_handling_context_manager.py
+Filename: cloudshell-logging-2.1.0/tests/logging/test_qs_config.ini
 Comment: 
 
-Filename: cloudshell-logging-2.0.0/cloudshell/logging/utils/__init__.py
+Filename: cloudshell-logging-2.1.0/tests/logging/utils/test_error_handling_context_manager.py
 Comment: 
 
-Filename: cloudshell-logging-2.0.0/cloudshell/logging/utils/decorators.py
+Filename: cloudshell-logging-2.1.0/tests/logging/utils/__init__.py
 Comment: 
 
-Filename: cloudshell-logging-2.0.0/cloudshell/logging/utils/log_exec_info.py
+Filename: cloudshell-logging-2.1.0/tests/logging/utils/test_command_logging.py
 Comment: 
 
-Filename: cloudshell-logging-2.0.0/tests/logging/
+Filename: cloudshell-logging-2.1.0/tests/logging/test_debug_logs/test_debug_logs_on_error.py
 Comment: 
 
-Filename: cloudshell-logging-2.0.0/tests/__init__.py
+Filename: cloudshell-logging-2.1.0/tests/logging/test_debug_logs/__init__.py
 Comment: 
 
-Filename: cloudshell-logging-2.0.0/tests/logging/test_logger_in_threads/
+Filename: cloudshell-logging-2.1.0/tests/logging/test_debug_logs/package_file.py
 Comment: 
 
-Filename: cloudshell-logging-2.0.0/tests/logging/utils/
+Filename: cloudshell-logging-2.1.0/tests/logging/test_logger_in_threads/test_getting_logger.py
 Comment: 
 
-Filename: cloudshell-logging-2.0.0/tests/logging/test_debug_logs/
+Filename: cloudshell-logging-2.1.0/tests/logging/test_logger_in_threads/__init__.py
 Comment: 
 
-Filename: cloudshell-logging-2.0.0/tests/logging/conftest.py
+Filename: cloudshell-logging-2.1.0/tests/logging/test_logger_in_threads/package_file.py
 Comment: 
 
-Filename: cloudshell-logging-2.0.0/tests/logging/test_memory_handler.py
+Filename: cloudshell-logging-2.1.0/cloudshell/logging/
 Comment: 
 
-Filename: cloudshell-logging-2.0.0/tests/logging/test_qs_config_parser.py
+Filename: cloudshell-logging-2.1.0/cloudshell/__init__.py
 Comment: 
 
-Filename: cloudshell-logging-2.0.0/tests/logging/test_qs_logger.py
+Filename: cloudshell-logging-2.1.0/cloudshell/logging/utils/
 Comment: 
 
-Filename: cloudshell-logging-2.0.0/tests/logging/__init__.py
+Filename: cloudshell-logging-2.1.0/cloudshell/logging/context_filters.py
 Comment: 
 
-Filename: cloudshell-logging-2.0.0/tests/logging/test_qs_config.ini
+Filename: cloudshell-logging-2.1.0/cloudshell/logging/__init__.py
 Comment: 
 
-Filename: cloudshell-logging-2.0.0/tests/logging/test_log_exec_info.py
+Filename: cloudshell-logging-2.1.0/cloudshell/logging/qs_logger.py
 Comment: 
 
-Filename: cloudshell-logging-2.0.0/tests/logging/test_logger_in_threads/test_getting_logger.py
+Filename: cloudshell-logging-2.1.0/cloudshell/logging/qs_config.ini
 Comment: 
 
-Filename: cloudshell-logging-2.0.0/tests/logging/test_logger_in_threads/package_file.py
+Filename: cloudshell-logging-2.1.0/cloudshell/logging/memory_handler.py
 Comment: 
 
-Filename: cloudshell-logging-2.0.0/tests/logging/test_logger_in_threads/__init__.py
+Filename: cloudshell-logging-2.1.0/cloudshell/logging/qs_config_parser.py
 Comment: 
 
-Filename: cloudshell-logging-2.0.0/tests/logging/utils/test_command_logging.py
+Filename: cloudshell-logging-2.1.0/cloudshell/logging/utils/error_handling_context_manager.py
 Comment: 
 
-Filename: cloudshell-logging-2.0.0/tests/logging/utils/test_error_handling_context_manager.py
+Filename: cloudshell-logging-2.1.0/cloudshell/logging/utils/decorators.py
 Comment: 
 
-Filename: cloudshell-logging-2.0.0/tests/logging/utils/__init__.py
+Filename: cloudshell-logging-2.1.0/cloudshell/logging/utils/venv.py
 Comment: 
 
-Filename: cloudshell-logging-2.0.0/tests/logging/test_debug_logs/package_file.py
+Filename: cloudshell-logging-2.1.0/cloudshell/logging/utils/__init__.py
 Comment: 
 
-Filename: cloudshell-logging-2.0.0/tests/logging/test_debug_logs/__init__.py
+Filename: cloudshell-logging-2.1.0/cloudshell/logging/utils/log_exec_info.py
 Comment: 
 
-Filename: cloudshell-logging-2.0.0/tests/logging/test_debug_logs/test_debug_logs_on_error.py
+Filename: cloudshell-logging-2.1.0/cloudshell/logging/utils/patch_logging_shutdown.py
 Comment: 
 
-Filename: cloudshell-logging-2.0.0/cloudshell_logging.egg-info/top_level.txt
+Filename: cloudshell-logging-2.1.0/cloudshell_logging.egg-info/dependency_links.txt
 Comment: 
 
-Filename: cloudshell-logging-2.0.0/cloudshell_logging.egg-info/SOURCES.txt
+Filename: cloudshell-logging-2.1.0/cloudshell_logging.egg-info/top_level.txt
 Comment: 
 
-Filename: cloudshell-logging-2.0.0/cloudshell_logging.egg-info/PKG-INFO
+Filename: cloudshell-logging-2.1.0/cloudshell_logging.egg-info/PKG-INFO
 Comment: 
 
-Filename: cloudshell-logging-2.0.0/cloudshell_logging.egg-info/dependency_links.txt
+Filename: cloudshell-logging-2.1.0/cloudshell_logging.egg-info/SOURCES.txt
 Comment: 
 
 Zip file comment:
```

## Comparing `cloudshell-logging-2.0.0/LICENSE.htm` & `cloudshell-logging-2.1.0/LICENSE.htm`

 * *Files identical despite different names*

## Comparing `cloudshell-logging-2.0.0/setup.py` & `cloudshell-logging-2.1.0/setup.py`

 * *Files identical despite different names*

## Comparing `cloudshell-logging-2.0.0/README.md` & `cloudshell-logging-2.1.0/README.md`

 * *Files identical despite different names*

## Comparing `cloudshell-logging-2.0.0/tox.ini` & `cloudshell-logging-2.1.0/tox.ini`

 * *Files identical despite different names*

## Comparing `cloudshell-logging-2.0.0/cloudshell/logging/qs_logger.py` & `cloudshell-logging-2.1.0/cloudshell/logging/qs_logger.py`

 * *Files 5% similar despite different names*

```diff
@@ -71,25 +71,28 @@
     config["MEMORY_LOG_SIZE"] = int(
         os.getenv("QS_MEMORY_LOG_SIZE", config.get("MEMORY_LOG_SIZE", 500))
     )
 
     return config
 
 
-def _set_log_level(logger, config):
-    log_level = config.get("LOG_LEVEL", DEFAULT_LEVEL)
-
+def set_log_level(logger: logging.Logger, level: int):
     for handler in logger.handlers:
         if not isinstance(handler, LimitedMemoryHandler):
             try:
-                handler.setLevel(log_level)
+                handler.setLevel(level)
             except ValueError:
                 handler.setLevel(DEFAULT_LEVEL)
 
 
+def set_log_level_from_config(logger, config):
+    log_level = config.get("LOG_LEVEL", DEFAULT_LEVEL)
+    set_log_level(logger, log_level)
+
+
 def _get_log_path_config(config):
     """Get log path based on the environment variable or Windows/Unix config setting.
 
     :param dict[str] config:
     :rtype: str
     """
     if "LOG_PATH" in os.environ:
@@ -162,14 +165,15 @@
 
 
 def get_qs_logger(
     log_group: str = "Ungrouped",
     log_category: str = "cloudshell",
     log_file_prefix: str = "QS",
     exec_info: dict | None = None,
+    use_context: bool = True,
 ) -> logging.Logger:
     """Create cloudshell specific singleton logger.
 
     :param log_group: This folder will be grouped under this name.
     The default implementation of the group is a folder under the logs directory.
     According to the CloudShell logging standard pass the reservation id as this value
     when applicable, otherwise use the operation name (e.g 'Autoload').
@@ -181,71 +185,89 @@
     specified prefix. According to the logging standard the prefix should be the
     name of the resource the command is executing on. For environment commands
     use the command name.
 
     :param exec_info: dict with execution info {LOG_LEVEL: {KEY: VALUE}}
         VALUE can be a string or list of strings
 
+    :param use_context: if True, use context to filter logs for different files
+
     :return: the logger object
     """
-    set_logger_context(folder_name=log_group, file_prefix=log_file_prefix)
+    if use_context:
+        set_logger_context(folder_name=log_group, file_prefix=log_file_prefix)
     config = get_settings()
     _LOGGER_LOCK.acquire()
     try:
         if log_group in _LOGGER_CONTAINER:
             logger = _LOGGER_CONTAINER[log_group]
             # log level may change between executions
-            _set_log_level(logger, config)
+            set_log_level_from_config(logger, config)
         else:
             logger = _create_logger(
-                log_group, log_category, log_file_prefix, config=config
+                log_group,
+                log_category,
+                log_file_prefix,
+                config=config,
+                use_context=use_context,
             )
             _LOGGER_CONTAINER[log_group] = logger
             # we have to set log level before logging exec info
-            _set_log_level(logger, config)
+            set_log_level_from_config(logger, config)
             if exec_info:
                 log_execution_info(logger, exec_info)
     finally:
         _LOGGER_LOCK.release()
 
     return logger
 
 
-def _create_logger(log_group, log_category, log_file_prefix, config=None):
+def _create_logger(
+    log_group: str,
+    log_category: str,
+    log_file_prefix: str,
+    config=None,
+    use_context: bool = True,
+) -> logging.Logger:
     """Create logging handler.
 
     :param log_group: This folder will be grouped under this name.
     The default implementation of the group is a folder under the logs directory.
     According to the CloudShell logging standard pass the reservation id as this value
     when applicable, otherwise use the operation name (e.g 'Autoload').
-    :type log_group: str
 
     :param log_category: All messages to this logger will be prefixed by the
     category name. The category name should be the name of the shell/driver
-    :type log_category: str
 
     :param log_file_prefix: The log file generated by this logger will have this
     specified prefix. According to the logging standard the prefix should be the name
     of the resource the command is executing on. For environment commands
     use the command name.
-    :type log_file_prefix: str
 
-    :return: the logger object
-    :rtype: logging.Logger
+    :param config: config dict
+
+    :param use_context: if True, use context to filter logs for different files
     """
     config = config or get_settings()
     logger = logging.getLogger(log_category)
     logger.setLevel(logging.DEBUG)
-    _add_handler_with_context(logger, config, log_file_prefix, log_group)
-    _add_handler_without_context(logger, config)
+    _add_main_handlers(logger, config, log_file_prefix, log_group, use_context)
+    if use_context:
+        _add_missing_context_handler(logger, config)
 
     return logger
 
 
-def _add_handler_with_context(logger, config, file_prefix, folder_name) -> None:
+def _add_main_handlers(
+    logger: logging.Logger,
+    config: dict,
+    file_prefix: str,
+    folder_name: str,
+    use_context: bool,
+) -> None:
     filter_by_context = FilterByContext(
         logger.name,
         folder_name=folder_name,
         file_prefix=file_prefix,  # use original file prefix
     )
     log_file_prefix = re.sub(" ", "_", file_prefix)
 
@@ -254,15 +276,16 @@
         hdlr1 = logging.FileHandler(log_path, mode="a")
         hdlr2 = _add_memory_handler(log_path, config)
         hdlrs = (hdlr1, hdlr2)
     else:
         hdlrs = (logging.StreamHandler(sys.stdout),)
 
     for hdlr in hdlrs:
-        hdlr.addFilter(filter_by_context)
+        if use_context:
+            hdlr.addFilter(filter_by_context)
 
         formatter = MultiLineFormatter(config["LOG_FORMAT"])
         hdlr.setFormatter(formatter)
 
         logger.addHandler(hdlr)
 
 
@@ -278,15 +301,15 @@
 
     formatter = MultiLineFormatter(config["LOG_FORMAT"])
     target_hdlr.setFormatter(formatter)
 
     return memory_hdlr
 
 
-def _add_handler_without_context(logger, config) -> None:
+def _add_missing_context_handler(logger: logging.Logger, config: dict) -> None:
     log_path = _get_log_path_config(config)
     if not log_path:
         return  # we save missed logs only for file handlers
 
     missing_logs_name = "missed_logs.log"
     missing_logs_path = os.path.join(log_path, missing_logs_name)
```

## Comparing `cloudshell-logging-2.0.0/cloudshell/logging/qs_config_parser.py` & `cloudshell-logging-2.1.0/cloudshell/logging/qs_config_parser.py`

 * *Files identical despite different names*

## Comparing `cloudshell-logging-2.0.0/cloudshell/logging/context_filters.py` & `cloudshell-logging-2.1.0/cloudshell/logging/context_filters.py`

 * *Files identical despite different names*

## Comparing `cloudshell-logging-2.0.0/cloudshell/logging/memory_handler.py` & `cloudshell-logging-2.1.0/cloudshell/logging/memory_handler.py`

 * *Files identical despite different names*

## Comparing `cloudshell-logging-2.0.0/cloudshell/logging/qs_config.ini` & `cloudshell-logging-2.1.0/cloudshell/logging/qs_config.ini`

 * *Files identical despite different names*

## Comparing `cloudshell-logging-2.0.0/cloudshell/logging/utils/patch_logging_shutdown.py` & `cloudshell-logging-2.1.0/cloudshell/logging/utils/patch_logging_shutdown.py`

 * *Files identical despite different names*

## Comparing `cloudshell-logging-2.0.0/cloudshell/logging/utils/error_handling_context_manager.py` & `cloudshell-logging-2.1.0/cloudshell/logging/utils/error_handling_context_manager.py`

 * *Files identical despite different names*

## Comparing `cloudshell-logging-2.0.0/cloudshell/logging/utils/decorators.py` & `cloudshell-logging-2.1.0/cloudshell/logging/utils/decorators.py`

 * *Files identical despite different names*

## Comparing `cloudshell-logging-2.0.0/cloudshell/logging/utils/log_exec_info.py` & `cloudshell-logging-2.1.0/cloudshell/logging/utils/log_exec_info.py`

 * *Files identical despite different names*

## Comparing `cloudshell-logging-2.0.0/tests/logging/test_memory_handler.py` & `cloudshell-logging-2.1.0/tests/logging/test_memory_handler.py`

 * *Files identical despite different names*

## Comparing `cloudshell-logging-2.0.0/tests/logging/test_qs_config_parser.py` & `cloudshell-logging-2.1.0/tests/logging/test_qs_config_parser.py`

 * *Files identical despite different names*

## Comparing `cloudshell-logging-2.0.0/tests/logging/test_qs_logger.py` & `cloudshell-logging-2.1.0/tests/logging/test_qs_logger.py`

 * *Files identical despite different names*

## Comparing `cloudshell-logging-2.0.0/tests/logging/test_log_exec_info.py` & `cloudshell-logging-2.1.0/tests/logging/test_log_exec_info.py`

 * *Files identical despite different names*

## Comparing `cloudshell-logging-2.0.0/tests/logging/test_logger_in_threads/test_getting_logger.py` & `cloudshell-logging-2.1.0/tests/logging/test_logger_in_threads/test_getting_logger.py`

 * *Files identical despite different names*

## Comparing `cloudshell-logging-2.0.0/tests/logging/utils/test_command_logging.py` & `cloudshell-logging-2.1.0/tests/logging/utils/test_command_logging.py`

 * *Files identical despite different names*

## Comparing `cloudshell-logging-2.0.0/tests/logging/utils/test_error_handling_context_manager.py` & `cloudshell-logging-2.1.0/tests/logging/utils/test_error_handling_context_manager.py`

 * *Files identical despite different names*

## Comparing `cloudshell-logging-2.0.0/tests/logging/test_debug_logs/test_debug_logs_on_error.py` & `cloudshell-logging-2.1.0/tests/logging/test_debug_logs/test_debug_logs_on_error.py`

 * *Files identical despite different names*

## Comparing `cloudshell-logging-2.0.0/cloudshell_logging.egg-info/SOURCES.txt` & `cloudshell-logging-2.1.0/cloudshell_logging.egg-info/SOURCES.txt`

 * *Files identical despite different names*

