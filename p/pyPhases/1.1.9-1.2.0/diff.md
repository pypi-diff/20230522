# Comparing `tmp/pyPhases-1.1.9.tar.gz` & `tmp/pyPhases-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyPhases-1.1.9.tar", last modified: Tue Feb 21 07:20:39 2023, max compression
+gzip compressed data, was "pyPhases-1.2.0.tar", last modified: Mon May 22 06:34:00 2023, max compression
```

## Comparing `pyPhases-1.1.9.tar` & `pyPhases-1.2.0.tar`

### file list

```diff
@@ -1,71 +1,73 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-21 07:20:39.377918 pyPhases-1.1.9/
--rw-rw-rw-   0 root         (0) root         (0)     1053 2023-02-21 07:20:22.000000 pyPhases-1.1.9/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       59 2023-02-21 07:20:22.000000 pyPhases-1.1.9/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     4666 2023-02-21 07:20:39.377918 pyPhases-1.1.9/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     4180 2023-02-21 07:20:22.000000 pyPhases-1.1.9/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-21 07:20:39.360916 pyPhases-1.1.9/pyPhases/
--rw-rw-rw-   0 root         (0) root         (0)     3045 2023-02-21 07:20:22.000000 pyPhases-1.1.9/pyPhases/Data.py
--rw-rw-rw-   0 root         (0) root         (0)     3189 2023-02-21 07:20:22.000000 pyPhases-1.1.9/pyPhases/Phase.py
--rw-rw-rw-   0 root         (0) root         (0)      434 2023-02-21 07:20:22.000000 pyPhases-1.1.9/pyPhases/PluginAdapter.py
--rw-rw-rw-   0 root         (0) root         (0)    15517 2023-02-21 07:20:22.000000 pyPhases-1.1.9/pyPhases/Project.py
--rw-rw-rw-   0 root         (0) root         (0)      396 2023-02-21 07:20:23.000000 pyPhases-1.1.9/pyPhases/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-21 07:20:39.362916 pyPhases-1.1.9/pyPhases/decorator/
--rw-rw-rw-   0 root         (0) root         (0)     1156 2023-02-21 07:20:22.000000 pyPhases-1.1.9/pyPhases/decorator/Decorator.py
--rw-rw-rw-   0 root         (0) root         (0)       33 2023-02-21 07:20:22.000000 pyPhases-1.1.9/pyPhases/decorator/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-21 07:20:39.363916 pyPhases-1.1.9/pyPhases/exporter/
--rw-rw-rw-   0 root         (0) root         (0)     2691 2023-02-21 07:20:22.000000 pyPhases-1.1.9/pyPhases/exporter/DataExporter.py
--rw-rw-rw-   0 root         (0) root         (0)     1006 2023-02-21 07:20:22.000000 pyPhases-1.1.9/pyPhases/exporter/PickleExporter.py
--rw-rw-rw-   0 root         (0) root         (0)       39 2023-02-21 07:20:22.000000 pyPhases-1.1.9/pyPhases/exporter/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-21 07:20:39.365917 pyPhases-1.1.9/pyPhases/test/
--rw-rw-rw-   0 root         (0) root         (0)     2276 2023-02-21 07:20:22.000000 pyPhases-1.1.9/pyPhases/test/MockLogger.py
--rw-rw-rw-   0 root         (0) root         (0)      352 2023-02-21 07:20:22.000000 pyPhases-1.1.9/pyPhases/test/Mocks.py
--rw-rw-rw-   0 root         (0) root         (0)     1983 2023-02-21 07:20:22.000000 pyPhases-1.1.9/pyPhases/test/TestCase.py
--rw-rw-rw-   0 root         (0) root         (0)      375 2023-02-21 07:20:22.000000 pyPhases-1.1.9/pyPhases/test/TestCaseIntegration.py
--rw-rw-rw-   0 root         (0) root         (0)      704 2023-02-21 07:20:22.000000 pyPhases-1.1.9/pyPhases/test/TestRun.py
--rw-rw-rw-   0 root         (0) root         (0)      148 2023-02-21 07:20:22.000000 pyPhases-1.1.9/pyPhases/test/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-21 07:20:39.367917 pyPhases-1.1.9/pyPhases/util/
--rw-rw-rw-   0 root         (0) root         (0)     2691 2023-02-21 07:20:22.000000 pyPhases-1.1.9/pyPhases/util/BatchProgress.py
--rw-rw-rw-   0 root         (0) root         (0)     1505 2023-02-21 07:20:22.000000 pyPhases-1.1.9/pyPhases/util/CSVLogger.py
--rw-rw-rw-   0 root         (0) root         (0)      777 2023-02-21 07:20:22.000000 pyPhases-1.1.9/pyPhases/util/EventBus.py
--rw-rw-rw-   0 root         (0) root         (0)     1514 2023-02-21 07:20:22.000000 pyPhases-1.1.9/pyPhases/util/Logger.py
--rw-rw-rw-   0 root         (0) root         (0)      573 2023-02-21 07:20:22.000000 pyPhases-1.1.9/pyPhases/util/Optionizable.py
--rw-rw-rw-   0 root         (0) root         (0)       80 2023-02-21 07:20:22.000000 pyPhases-1.1.9/pyPhases/util/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1775 2023-02-21 07:20:22.000000 pyPhases-1.1.9/pyPhases/util/pdict.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-21 07:20:39.361916 pyPhases-1.1.9/pyPhases.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4666 2023-02-21 07:20:39.000000 pyPhases-1.1.9/pyPhases.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1536 2023-02-21 07:20:39.000000 pyPhases-1.1.9/pyPhases.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-02-21 07:20:39.000000 pyPhases-1.1.9/pyPhases.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-02-21 07:20:39.000000 pyPhases-1.1.9/pyPhases.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-02-21 07:20:39.000000 pyPhases-1.1.9/pyPhases.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)       12 2023-02-21 07:20:22.000000 pyPhases-1.1.9/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-02-21 07:20:39.377918 pyPhases-1.1.9/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      763 2023-02-21 07:20:23.000000 pyPhases-1.1.9/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-21 07:20:39.368917 pyPhases-1.1.9/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-02-21 07:20:22.000000 pyPhases-1.1.9/tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-21 07:20:39.370917 pyPhases-1.1.9/tests/test/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-02-21 07:20:22.000000 pyPhases-1.1.9/tests/test/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1752 2023-02-21 07:20:22.000000 pyPhases-1.1.9/tests/test/test_BaseTest.py
--rw-rw-rw-   0 root         (0) root         (0)      873 2023-02-21 07:20:22.000000 pyPhases-1.1.9/tests/test/test_IntegrationTest.py
--rw-rw-rw-   0 root         (0) root         (0)      910 2023-02-21 07:20:22.000000 pyPhases-1.1.9/tests/test/test_Mocks.py
--rw-rw-rw-   0 root         (0) root         (0)      825 2023-02-21 07:20:22.000000 pyPhases-1.1.9/tests/test/test_TestRun.py
--rw-rw-rw-   0 root         (0) root         (0)      372 2023-02-21 07:20:22.000000 pyPhases-1.1.9/tests/test_acceptance.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-21 07:20:39.375917 pyPhases-1.1.9/tests/unit/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-02-21 07:20:22.000000 pyPhases-1.1.9/tests/unit/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5184 2023-02-21 07:20:22.000000 pyPhases-1.1.9/tests/unit/test_BatchProgress.py
--rw-rw-rw-   0 root         (0) root         (0)     6054 2023-02-21 07:20:22.000000 pyPhases-1.1.9/tests/unit/test_Data.py
--rw-rw-rw-   0 root         (0) root         (0)     1519 2023-02-21 07:20:22.000000 pyPhases-1.1.9/tests/unit/test_DataExporter.py
--rw-rw-rw-   0 root         (0) root         (0)      350 2023-02-21 07:20:22.000000 pyPhases-1.1.9/tests/unit/test_Decorator.py
--rw-rw-rw-   0 root         (0) root         (0)      964 2023-02-21 07:20:22.000000 pyPhases-1.1.9/tests/unit/test_EventBus.py
--rw-rw-rw-   0 root         (0) root         (0)     3016 2023-02-21 07:20:22.000000 pyPhases-1.1.9/tests/unit/test_Logger.py
--rw-rw-rw-   0 root         (0) root         (0)     3076 2023-02-21 07:20:22.000000 pyPhases-1.1.9/tests/unit/test_Loggermock.py
--rw-rw-rw-   0 root         (0) root         (0)      638 2023-02-21 07:20:22.000000 pyPhases-1.1.9/tests/unit/test_Optionizable.py
--rw-rw-rw-   0 root         (0) root         (0)     4985 2023-02-21 07:20:22.000000 pyPhases-1.1.9/tests/unit/test_Phase.py
--rw-rw-rw-   0 root         (0) root         (0)      795 2023-02-21 07:20:22.000000 pyPhases-1.1.9/tests/unit/test_PluginAdapter.py
--rw-rw-rw-   0 root         (0) root         (0)    16555 2023-02-21 07:20:22.000000 pyPhases-1.1.9/tests/unit/test_Project.py
--rw-rw-rw-   0 root         (0) root         (0)     3838 2023-02-21 07:20:22.000000 pyPhases-1.1.9/tests/unit/test_csvlogger.py
--rw-rw-rw-   0 root         (0) root         (0)     1184 2023-02-21 07:20:22.000000 pyPhases-1.1.9/tests/unit/test_exporter_pickleexporter.py
--rw-rw-rw-   0 root         (0) root         (0)     3186 2023-02-21 07:20:22.000000 pyPhases-1.1.9/tests/unit/test_pdict.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-21 07:20:39.376917 pyPhases-1.1.9/tests/util/
--rw-rw-rw-   0 root         (0) root         (0)      874 2023-02-21 07:20:22.000000 pyPhases-1.1.9/tests/util/ExporterTestHelper.py
--rw-rw-rw-   0 root         (0) root         (0)     1856 2023-02-21 07:20:22.000000 pyPhases-1.1.9/tests/util/PhaseGenerator.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-02-21 07:20:22.000000 pyPhases-1.1.9/tests/util/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 06:34:00.597839 pyPhases-1.2.0/
+-rw-rw-rw-   0 root         (0) root         (0)     1053 2023-05-22 06:33:46.000000 pyPhases-1.2.0/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       59 2023-05-22 06:33:46.000000 pyPhases-1.2.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     4666 2023-05-22 06:34:00.597839 pyPhases-1.2.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     4180 2023-05-22 06:33:46.000000 pyPhases-1.2.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 06:34:00.589840 pyPhases-1.2.0/pyPhases/
+-rw-rw-rw-   0 root         (0) root         (0)     3043 2023-05-22 06:33:46.000000 pyPhases-1.2.0/pyPhases/Data.py
+-rw-rw-rw-   0 root         (0) root         (0)     3319 2023-05-22 06:33:46.000000 pyPhases-1.2.0/pyPhases/Phase.py
+-rw-rw-rw-   0 root         (0) root         (0)      466 2023-05-22 06:33:46.000000 pyPhases-1.2.0/pyPhases/PluginAdapter.py
+-rw-rw-rw-   0 root         (0) root         (0)    15638 2023-05-22 06:33:46.000000 pyPhases-1.2.0/pyPhases/Project.py
+-rw-rw-rw-   0 root         (0) root         (0)      396 2023-05-22 06:33:48.000000 pyPhases-1.2.0/pyPhases/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 06:34:00.590839 pyPhases-1.2.0/pyPhases/decorator/
+-rw-rw-rw-   0 root         (0) root         (0)     1156 2023-05-22 06:33:46.000000 pyPhases-1.2.0/pyPhases/decorator/Decorator.py
+-rw-rw-rw-   0 root         (0) root         (0)       33 2023-05-22 06:33:46.000000 pyPhases-1.2.0/pyPhases/decorator/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 06:34:00.590839 pyPhases-1.2.0/pyPhases/exporter/
+-rw-rw-rw-   0 root         (0) root         (0)     2660 2023-05-22 06:33:46.000000 pyPhases-1.2.0/pyPhases/exporter/DataExporter.py
+-rw-rw-rw-   0 root         (0) root         (0)     1025 2023-05-22 06:33:46.000000 pyPhases-1.2.0/pyPhases/exporter/PickleExporter.py
+-rw-rw-rw-   0 root         (0) root         (0)       39 2023-05-22 06:33:46.000000 pyPhases-1.2.0/pyPhases/exporter/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 06:34:00.591839 pyPhases-1.2.0/pyPhases/test/
+-rw-rw-rw-   0 root         (0) root         (0)     2278 2023-05-22 06:33:46.000000 pyPhases-1.2.0/pyPhases/test/MockLogger.py
+-rw-rw-rw-   0 root         (0) root         (0)      354 2023-05-22 06:33:46.000000 pyPhases-1.2.0/pyPhases/test/Mocks.py
+-rw-rw-rw-   0 root         (0) root         (0)     2098 2023-05-22 06:33:46.000000 pyPhases-1.2.0/pyPhases/test/TestCase.py
+-rw-rw-rw-   0 root         (0) root         (0)      375 2023-05-22 06:33:46.000000 pyPhases-1.2.0/pyPhases/test/TestCaseIntegration.py
+-rw-rw-rw-   0 root         (0) root         (0)      704 2023-05-22 06:33:46.000000 pyPhases-1.2.0/pyPhases/test/TestRun.py
+-rw-rw-rw-   0 root         (0) root         (0)      148 2023-05-22 06:33:46.000000 pyPhases-1.2.0/pyPhases/test/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 06:34:00.593840 pyPhases-1.2.0/pyPhases/util/
+-rw-rw-rw-   0 root         (0) root         (0)     2692 2023-05-22 06:33:46.000000 pyPhases-1.2.0/pyPhases/util/BatchProgress.py
+-rw-rw-rw-   0 root         (0) root         (0)     1495 2023-05-22 06:33:46.000000 pyPhases-1.2.0/pyPhases/util/CSVLogger.py
+-rw-rw-rw-   0 root         (0) root         (0)      775 2023-05-22 06:33:46.000000 pyPhases-1.2.0/pyPhases/util/EventBus.py
+-rw-rw-rw-   0 root         (0) root         (0)      768 2023-05-22 06:33:46.000000 pyPhases-1.2.0/pyPhases/util/EventBusStatic.py
+-rw-rw-rw-   0 root         (0) root         (0)     1526 2023-05-22 06:33:46.000000 pyPhases-1.2.0/pyPhases/util/Logger.py
+-rw-rw-rw-   0 root         (0) root         (0)      573 2023-05-22 06:33:46.000000 pyPhases-1.2.0/pyPhases/util/Optionizable.py
+-rw-rw-rw-   0 root         (0) root         (0)       80 2023-05-22 06:33:46.000000 pyPhases-1.2.0/pyPhases/util/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1755 2023-05-22 06:33:46.000000 pyPhases-1.2.0/pyPhases/util/pdict.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 06:34:00.590839 pyPhases-1.2.0/pyPhases.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4666 2023-05-22 06:34:00.000000 pyPhases-1.2.0/pyPhases.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1583 2023-05-22 06:34:00.000000 pyPhases-1.2.0/pyPhases.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-22 06:34:00.000000 pyPhases-1.2.0/pyPhases.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-05-22 06:34:00.000000 pyPhases-1.2.0/pyPhases.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-05-22 06:34:00.000000 pyPhases-1.2.0/pyPhases.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      370 2023-05-22 06:33:46.000000 pyPhases-1.2.0/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)       12 2023-05-22 06:33:46.000000 pyPhases-1.2.0/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-22 06:34:00.597839 pyPhases-1.2.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      763 2023-05-22 06:33:48.000000 pyPhases-1.2.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 06:34:00.593840 pyPhases-1.2.0/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-22 06:33:46.000000 pyPhases-1.2.0/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 06:34:00.594839 pyPhases-1.2.0/tests/test/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-22 06:33:46.000000 pyPhases-1.2.0/tests/test/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1752 2023-05-22 06:33:46.000000 pyPhases-1.2.0/tests/test/test_BaseTest.py
+-rw-rw-rw-   0 root         (0) root         (0)      873 2023-05-22 06:33:46.000000 pyPhases-1.2.0/tests/test/test_IntegrationTest.py
+-rw-rw-rw-   0 root         (0) root         (0)      910 2023-05-22 06:33:46.000000 pyPhases-1.2.0/tests/test/test_Mocks.py
+-rw-rw-rw-   0 root         (0) root         (0)      825 2023-05-22 06:33:46.000000 pyPhases-1.2.0/tests/test/test_TestRun.py
+-rw-rw-rw-   0 root         (0) root         (0)      367 2023-05-22 06:33:46.000000 pyPhases-1.2.0/tests/test_acceptance.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 06:34:00.596840 pyPhases-1.2.0/tests/unit/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-22 06:33:46.000000 pyPhases-1.2.0/tests/unit/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5149 2023-05-22 06:33:46.000000 pyPhases-1.2.0/tests/unit/test_BatchProgress.py
+-rw-rw-rw-   0 root         (0) root         (0)     6047 2023-05-22 06:33:46.000000 pyPhases-1.2.0/tests/unit/test_Data.py
+-rw-rw-rw-   0 root         (0) root         (0)     1518 2023-05-22 06:33:46.000000 pyPhases-1.2.0/tests/unit/test_DataExporter.py
+-rw-rw-rw-   0 root         (0) root         (0)      349 2023-05-22 06:33:46.000000 pyPhases-1.2.0/tests/unit/test_Decorator.py
+-rw-rw-rw-   0 root         (0) root         (0)      963 2023-05-22 06:33:46.000000 pyPhases-1.2.0/tests/unit/test_EventBus.py
+-rw-rw-rw-   0 root         (0) root         (0)     3074 2023-05-22 06:33:46.000000 pyPhases-1.2.0/tests/unit/test_Logger.py
+-rw-rw-rw-   0 root         (0) root         (0)     3146 2023-05-22 06:33:46.000000 pyPhases-1.2.0/tests/unit/test_Loggermock.py
+-rw-rw-rw-   0 root         (0) root         (0)      638 2023-05-22 06:33:46.000000 pyPhases-1.2.0/tests/unit/test_Optionizable.py
+-rw-rw-rw-   0 root         (0) root         (0)     5056 2023-05-22 06:33:46.000000 pyPhases-1.2.0/tests/unit/test_Phase.py
+-rw-rw-rw-   0 root         (0) root         (0)      795 2023-05-22 06:33:46.000000 pyPhases-1.2.0/tests/unit/test_PluginAdapter.py
+-rw-rw-rw-   0 root         (0) root         (0)    17896 2023-05-22 06:33:46.000000 pyPhases-1.2.0/tests/unit/test_Project.py
+-rw-rw-rw-   0 root         (0) root         (0)     3838 2023-05-22 06:33:46.000000 pyPhases-1.2.0/tests/unit/test_csvlogger.py
+-rw-rw-rw-   0 root         (0) root         (0)     1073 2023-05-22 06:33:46.000000 pyPhases-1.2.0/tests/unit/test_exporter_pickleexporter.py
+-rw-rw-rw-   0 root         (0) root         (0)     3509 2023-05-22 06:33:46.000000 pyPhases-1.2.0/tests/unit/test_pdict.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 06:34:00.596840 pyPhases-1.2.0/tests/util/
+-rw-rw-rw-   0 root         (0) root         (0)      866 2023-05-22 06:33:46.000000 pyPhases-1.2.0/tests/util/ExporterTestHelper.py
+-rw-rw-rw-   0 root         (0) root         (0)     2044 2023-05-22 06:33:46.000000 pyPhases-1.2.0/tests/util/PhaseGenerator.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-22 06:33:46.000000 pyPhases-1.2.0/tests/util/__init__.py
```

### Comparing `pyPhases-1.1.9/LICENSE` & `pyPhases-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyPhases-1.1.9/PKG-INFO` & `pyPhases-1.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyPhases
-Version: 1.1.9
+Version: 1.2.0
 Summary: A Framework for creating a boilerplate template for ai projects that are ready for MLOps
 Home-page: https://gitlab.com/tud.ibmt/pyPhases
 Author: Franz Ehrlich
 Author-email: fehrlichd@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pyPhases-1.1.9/README.md` & `pyPhases-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `pyPhases-1.1.9/pyPhases/Data.py` & `pyPhases-1.2.0/pyPhases/Data.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 
         value = self.project.getConfig(tagname)
         flat = Data.flatten(value)
         if self.hasTobeHashed(value):
             self.logDebug("config value %s has to be hashed: %s" % (tagname, flat))
         return flat
 
-    def getDependencyDict(self, tagNames = None):
+    def getDependencyDict(self, tagNames=None):
         dep = {}
         tagNames = tagNames if tagNames is not None else self.dataTags
         for tagname in tagNames:
             if tagname in self.project.dataNames:
                 tags = self.project.dataNames[tagname].dataTags
                 self.logDebug("Data %s depends on different dataset %s: %s" % (self.name, tagname, tags))
                 dep.update(self.getDependencyDict(self.project.dataNames[tagname].dataTags))
```

### Comparing `pyPhases-1.1.9/pyPhases/Phase.py` & `pyPhases-1.2.0/pyPhases/Phase.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,34 +11,36 @@
     summary = {}
     inputs = []
     model = None
     runMethod = "main"
     project: Project = None
     decorators = None
 
-    def __init__(self, exportData=None, options={}) -> None:
+    def __init__(self, exportData=None, options=None) -> None:
+        if options is None:
+            options = {}
         super().__init__(options)
         self.exportData = exportData or []
         self.exportDataStrings = None
         self._prepared = False
 
     def prepare(self):
         if self._prepared:
             return
-        self.logDebug("Prepare phase: " + self.name)
+        self.logDebug(f"Prepare phase: {self.name}")
         self.exportData = list(map(lambda s: Data.create(s, self.project), self.exportData))
         self.exportDataStrings = list(map(lambda data: data.name, self.exportData))
         self.prepareConfig()
         self._prepared = True
 
         phaseName = self.getId()
         if phaseName in self.project.config:
             for index in self.project.config[phaseName]:
                 value = self.project.config[phaseName][index]
-                self.logDebug("Overwrite Config %s for phase %s with %s" % (index, phaseName, value))
+                self.logDebug(f"Overwrite Config {index} for phase {phaseName} with {value}")
                 setattr(self, index, value)
 
         def configChanged(changed):
             if changed is None:
                 self.prepareConfig()
                 self.project.addConfig(self.config)
 
@@ -60,34 +62,40 @@
 
     def getConfig(self, configName, defaultValue=None):
         return self.project.getConfig(configName, defaultValue)
 
     def setConfig(self, configName, value):
         return self.project.setConfig(configName, value)
 
-    def getData(self, dataName: str, expectedReturnType=None, version: str = "current", options={}, generate=True):
+    def getData(self, dataName: str, expectedReturnType=None, version: str = "current", options=None, generate=True):
+        if options is None:
+            options = {}
         return self.project.getData(
-            dataName=dataName, expectedReturnType=expectedReturnType, version=version, options=options, generate=generate
+            dataName=dataName,
+            expectedReturnType=expectedReturnType,
+            version=version,
+            options=options,
+            generate=generate,
         )
 
     def registerData(self, dataName: str, data, version: str = "current", save: bool = True):
         return self.project.registerData(dataName=dataName, data=data, version=version, save=save)
 
     def generateData(self, name):
         self.run()
 
     def getId(self):
-        return self.name if self.name else type(self).__name__
+        return self.name or type(self).__name__
 
     def run(self):
         phaseName = self.getId()
-        self.log("RUN phase %s: %s" % (phaseName, self.name))
+        self.log(f"RUN phase {phaseName}: {self.name}")
 
         def methodNotFound():
-            self.logError("The current phase needs the following method defined: " + self.runMethod)
+            self.logError(f"The current phase needs the following method defined: {self.runMethod}")
 
         method = getattr(self, self.runMethod, methodNotFound)
         decorators = self.getDecorators()
 
         for decorator in decorators:
             decorator.before(self)
```

### Comparing `pyPhases-1.1.9/pyPhases/Project.py` & `pyPhases-1.2.0/pyPhases/Project.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import contextlib
 import importlib
 import json
 from copy import deepcopy
 from pathlib import Path
 from typing import Iterator
 
 import yaml
@@ -47,38 +48,38 @@
         self.namespace = namespace
         self.dataNames = {}
         self.classes = []
         self.exporters = []
         self.classesMap = {}
         self.registeredData = {}
         self.config = pdict()
-        self.configBackup = None
+        self.configBackups = []
         self.phaseIndex = 0
         self.decorators = []
         self.debug = False
         self.testRun = False
         self.phaseMap = {}
         self.logLevel = None
         self.gridOutput = None
         self.plugins = []
         self.systemExporter = {"PickleExporter": "pyPhases"}
 
     def registerDecorator(self, decorator: Decorator):
         """registers a decorator to the project that is run before and after each phase"""
-        self.logDebug("Register Decorator: " + type(decorator).__name__)
+        self.logDebug(f"Register Decorator: {type(decorator).__name__}")
         self.decorators.append(decorator)
 
     def registerExporter(self, exporter):
         """registers an exporter to the project that can handle data types and transform oder save objects"""
-        self.logDebug("Register Exporter: " + type(exporter).__name__)
+        self.logDebug(f"Register Exporter: {type(exporter).__name__}")
         self.exporters.append(exporter)
 
     def getExporterForIntsance(self, instance) -> DataExporter:
         """return a exporter that can handle the given instance, if such a exporter exists else None"""
-        self.logDebug("Get Exporter For: " + type(instance).__name__)
+        self.logDebug(f"Get Exporter For: {type(instance).__name__}")
         return self.getExporterForType(type(instance))
 
     def getExporterForType(self, theType, reinit=True) -> DataExporter:
         """return a exporter that can handle the given type, if such a exporter exists else None
 
         Args:
             theType (_type_): the type that should be exported
@@ -89,149 +90,167 @@
         """
         exporters = self.exporters
 
         if theType is None:
             return None
 
         for exporter in exporters:
-            self.logDebug("Check: " + type(exporter).__name__)
+            self.logDebug(f"Check: {type(exporter).__name__}")
             if exporter.checkType(theType):
                 self.logDebug("Found exporter")
-                if reinit:
-                    return exporter.reinit()
-                else:
-                    return exporter
+                return exporter.reinit() if reinit else exporter
         return None
 
     def getDataFromName(self, dataName: str, version: str = "current") -> Data:
         """returns a data object for the given data name
 
         Args:
             dataName (str): the name of the data
             version (str, optional): version string
 
         Returns:
             Data: the data object
         """
 
         if dataName not in self.dataNames:
-            raise Exception("The DataWrapper with name %s was not defined and does not exist in any phase" % (dataName))
+            raise Exception(f"The DataWrapper with name {dataName} was not defined and does not exist in any phase")
 
         dataObj = self.dataNames[dataName]
         dataObj.version = version
 
         return dataObj
 
     def registerStream(self, dataName, expectedReturnType, options, version: str = "current"):
         """registers a stream for the given data name, a stream can be a reference to a file for example"""
         dataObj = self.getDataFromName(dataName, version=version)
         dataId = dataObj.getDataId()
 
         exporter = self.getExporterForType(expectedReturnType)
         if exporter is None:
-            raise Exception("No stream exporter found for type %s" % (expectedReturnType))
+            raise Exception(f"No stream exporter found for type {expectedReturnType}")
         return exporter.stream(dataId, options)
 
-    def getExporterAndId(self, dataName, expectedReturnType, options={}, version: str = "current"):
+    def getExporterAndId(self, dataName, expectedReturnType, options=None, version: str = "current"):
         """returns a exporter and the data id as a string for the given data name
 
         Args:
             dataName (str): the identifiation name of the data
             expectedReturnType (type): the expedted type of the data (is required to select the right exporter)
 
         Returns:
             (Exporter, str): a tuple of the exporter and the data id
         """
+        options = options or {}
 
         dataObj = self.getDataFromName(dataName, version=version)
         dataId = dataObj.getDataId()
 
         try:
             exporter = self.getExporterForType(expectedReturnType, reinit=False)
             return exporter, dataId
-        except Exception:
-            raise Exception("No stream exporter found for this")
+        except Exception as e:
+            raise Exception("No stream exporter found for this") from e
 
     def dataExists(self, data: Data):
         """returns true if the given data object is registered in the project"""
         return data.getDataId() in self.registeredData
 
-    def dataExistIn(self, dataName: str, expectedReturnType=None, version: str = "current", options=None):
+    def dataExistIn(
+        self,
+        dataName: str,
+        expectedReturnType=None,
+        version: str = "current",
+    ):
         """returns true if the exporter can read the data"""
 
         dataObj = self.getDataFromName(dataName, version=version)
         dataId = dataObj.getDataId()
 
         if dataId in self.registeredData:
             return True
 
         # check if the can be loaded by the exporter
         exporter = self.getExporterForType(expectedReturnType)
-        if exporter is None:
-            return False
+        return False if exporter is None else exporter.exists(dataId)
 
-        return exporter.exists(dataId, options)
-
-    def unregister(self, dataName: str, expectedReturnType=None, version: str = "current", options=None):
+    def unregister(
+        self,
+        dataName: str,
+        expectedReturnType=None,
+        version: str = "current",
+        options=None,
+    ):
         """unregisters a data from the project memory, it will not delete the data itself"""
         dataObj = self.getDataFromName(dataName, version=version)
         dataId = dataObj.getDataId()
         del self.registeredData[dataId]
 
-    def getData(self, dataName: str, expectedReturnType=None, version: str = "current", options=None, generate=True):
+    def getData(
+        self,
+        dataName: str,
+        expectedReturnType=None,
+        version: str = "current",
+        options=None,
+        generate=True,
+    ):
         """
         returns either a registerd data in the project memory,
         loads the data from a exporter or generates the data from a phase
         """
 
         options = options or {}
 
         dataObj = self.getDataFromName(dataName, version=version)
         dataId = dataObj.getDataId()
 
-        self.logDebug("Try to get Data: " + dataId)
+        self.logDebug(f"Try to get Data: {dataId}")
 
         # just generated Data
         if dataId in self.registeredData:
-            self.logDebug("Data in memory: " + dataId)
+            self.logDebug(f"Data in memory: {dataId}")
             return self.registeredData[dataId]
 
         # load from exporter layer
         exporter = self.getExporterForType(expectedReturnType)
         if exporter is not None:
-            try:
+            with contextlib.suppress(DataNotFound):
                 exporter.currentDataObj = dataObj
                 return exporter.read(dataId, options)
-            except DataNotFound:
-                pass
-
         # data not found, generate from phase
         if generate and version == "current":
-            self.logWarning("Data " + dataId + " was not found, try to find phase to generate it")
+            self.logWarning(f"Data {dataId} was not found, try to find phase to generate it")
             return self.generateData(dataName, expectedReturnType, version, options)
 
-        raise DataNotFound("Data " + dataName + " was not found: %s" % dataId)
+        raise DataNotFound(f"Data {dataName}" + f" was not found: {dataId}")
 
-    def generateData(self, dataName: str, expectedReturnType=None, version: str = "current", options={}):
+    def generateData(self, dataName: str, expectedReturnType=None, version: str = "current", options=None):
         """forces the data generation for a specific dataName"""
+        options = options or {}
         for phase in self.getPhases():
             if dataName in phase.exportDataStrings:
                 returnedData = phase.generateData(dataName)
                 if returnedData is not None:
                     return returnedData
                 try:
                     return self.getData(dataName, expectedReturnType, version, options, generate=False)
-                except DataNotFound:
+                except DataNotFound as e:
                     raise DataNotFound(
-                        "try to generate data %s with phase %s but it was not registerd" % (dataName, phase.getId())
-                    )
+                        f"try to generate data {dataName} with phase {phase.getId()} but it was not registerd"
+                    ) from e
 
-        raise DataNotFound("Data " + dataName + " was not found")
+        raise DataNotFound(f"Data {dataName} was not found")
 
-    def registerData(self, dataName: str, data, version: str = "current", save: bool = True, options=None):
+    def registerData(
+        self,
+        dataName: str,
+        data,
+        version: str = "current",
+        save: bool = True,
+        options=None,
+    ):
         """registers a data object in the project memory and saves it through the exporter
 
         Args:
             dataName (str): the identifiation name of the data
             data: the data object
             save (bool): if set to false the project will not try to save the data
 
@@ -241,22 +260,22 @@
         options = options or {}
         dataObj = self.getDataFromName(dataName, version=version)
         dataId = dataObj.getDataId()
 
         # save to runtime project
         self.registeredData[dataId] = data
 
-        if save is False:
+        if not save:
             return
 
         # save through exporter
         exporter = self.getExporterForIntsance(data)
         if exporter is None:
             self.logWarning(
-                "No exporter for datatype (" + type(data).__name__ + ") the data " + dataName + " will not be automaticly save"
+                f"No exporter for datatype ({type(data).__name__}) the data {dataName} will not be automaticly save"
             )
             return
         exporter.currentDataObj = dataObj
         exporter.write(dataId, data, options)
 
     def setConfig(self, name: str, value):
         """
@@ -274,21 +293,21 @@
         (f.e. project.getConfig('foo.bar.value1')
         """
         if name not in self.config:
             if "." in name:
                 name = name.split(".")
             try:
                 return self.config[name]
-            except KeyError:
-                self.config[name] = defaultValue
+            except KeyError as e:
                 if defaultValue is None and raiseException:
                     raise ConfigNotFoundException(
-                        "The Config entry '%s' was not found, if you rely on a earlier config entry in a previous phase make sure you put the config entry in the __init__ section of the phase"
-                        % (name)
-                    )
+                        f"The Config entry '{name}' was not found, if you rely on a earlier config entry in a previous phase"
+                        + "make sure you put the config entry in the __init__ section of the phase"
+                    ) from e
+                return defaultValue
         return self.config[name]
 
     def saveConfig(
         self,
         path: str,
         dataName=None,
         version: str = "current",
@@ -301,15 +320,15 @@
         """
         if dataName is not None:
             config = self.getDataFromName(dataName, version=version).getDependencyDict()
         else:
             config = self.config
 
         with open(path, "w+") as f:
-            self.log("save config from file %s" % path)
+            self.log(f"save config from file {path}")
             json.dump(config, f)
 
     def importConfigsByImportValue(self, key, baseConfig, filePath):
         importedConfigs = []
         if key in baseConfig:
             for relPath in baseConfig[key]:
                 path = Path(Path(filePath).parent, relPath)
@@ -327,23 +346,23 @@
         loadedConfig = pdict()
 
         with open(filePath, "r") as configFile:
             yamlContent = configFile.read()
             fileConfig = yaml.load(yamlContent, Loader=SafeLoader)
 
         if fileConfig is None:
-            return {}
+            return loadedConfig
 
         importedConfigsBefore = self.importConfigsByImportValue("importBefore", fileConfig, filePath)
         importedConfigsAfter = self.importConfigsByImportValue("importAfter", fileConfig, filePath)
 
         for subConfig in importedConfigsBefore:
             loadedConfig.update(subConfig)
 
-        self.logDebug("parse user config: %s" % filePath)
+        self.logDebug(f"parse user config: {filePath}")
         loadedConfig.update(fileConfig)
 
         for subConfig in importedConfigsAfter:
             loadedConfig.update(subConfig)
         return loadedConfig
 
     def loadAndApplyConfig(self, filePath):
@@ -410,25 +429,24 @@
         phase.run()
         self.trigger("afterRun")
 
     def getPhase(self, name: str) -> Phase:
         """get a specific phase by name"""
 
         if name not in self.phaseMap:
-            raise PhaseNotFoundException("Phase %s not found" % name)
+            raise PhaseNotFoundException(f"Phase {name} not found")
 
         return self.phaseMap[name]
 
     def getPhases(self) -> Iterator[Phase]:
         """get a generator for all phases"""
-        for phase in self.phases:
-            yield phase
+        yield from self.phases
 
     def __enter__(self):
         """enter a config scope and backup the old config"""
-        self.configBackup = deepcopy(self.config)
+        self.configBackups.append(deepcopy(self.config))
         return self
 
     def __exit__(self, exception_type, exception_value, traceback):
         """exit the config scope and restore the old config"""
-        self.config = self.configBackup
+        self.config = self.configBackups.pop()
         self.trigger("configChanged", None)
```

### Comparing `pyPhases-1.1.9/pyPhases/decorator/Decorator.py` & `pyPhases-1.2.0/pyPhases/decorator/Decorator.py`

 * *Files identical despite different names*

### Comparing `pyPhases-1.1.9/pyPhases/exporter/DataExporter.py` & `pyPhases-1.2.0/pyPhases/exporter/DataExporter.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,22 +10,20 @@
     """
     Data exporter is an abstract class that should be used to define new data exporters.
     A data exporter can handle data from a specific type and read or write it to self definded
     storage.
 
     The data exporter should handle all ingoing and outgoing data for the project.
     """
+
     recreate: bool = True
     currentDataObj: Data = None
 
-
     def initialOptions(self, defaultOptions=None):
-        return {
-            "basePath": "./data"
-        }
+        return {"basePath": "./data"}
 
     @abstractmethod
     def checkType(self, type) -> bool:
         """this method needs to be overwritten and checks if the exporter is compatible to a given type
 
         Returns:
             bool: returns True if the exporter can handle the given type.
@@ -45,16 +43,15 @@
         """this method can be called if the streaming process finished (for example the writing process)
 
         dataId ([type]): the full data id (with all config values) is passed to the stream
         """
         pass
 
     def reinit(self):
-        """recreate the current datatype if the exporter needs to be recreated with every exported/imported type.
-        """
+        """recreate the current datatype if the exporter needs to be recreated with every exported/imported type."""
         if not self.recreate:
             return self
         return type(self)(self.options)
 
     def exists(self, path):
         """checks if there is data to a given path
```

### Comparing `pyPhases-1.1.9/pyPhases/exporter/PickleExporter.py` & `pyPhases-1.2.0/pyPhases/exporter/PickleExporter.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,24 +1,29 @@
 import pickle
 
 from pyPhases.exporter.DataExporter import DataExporter
 from pyPhases.Data import DataNotFound
 
+
 class PickleExporter(DataExporter):
     supportedTypes = []
 
     try:
         import pandas
+
         supportedTypes.append(pandas.DataFrame)
-    except ImportError: pass
+    except ImportError:
+        pass
 
     try:
         import numpy
+
         supportedTypes.append(numpy.ndarray)
-    except ImportError: pass
+    except ImportError:
+        pass
 
     """ An Exporter that supports a lot of default formats using pickle"""
 
     def checkType(self, type):
         return type in self.supportedTypes or issubclass(type, (str, int, bool, float, list, dict, tuple))
 
     def read(self, dataId, options={}):
```

### Comparing `pyPhases-1.1.9/pyPhases/test/MockLogger.py` & `pyPhases-1.2.0/pyPhases/test/MockLogger.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 from pyPhases import LogLevel
 from unittest.mock import patch
 
-class LoggerMock():
 
+class LoggerMock:
     def __init__(self, mock) -> None:
         self.mock = mock
 
     def expectLogMessage(self, msg, system=None, level=LogLevel.INFO):
         self.assertLogMessageLike(msg, system, level, exact=True)
 
-
     def assertLogMessageLike(self, contains, expectedSystem=None, expectedLevel=None, exact=False):
         """Assert that a log message contains the given message."""
         self.mock.assert_called()
         args = list(self.mock.call_args[0]) + list(self.mock.call_args[1].values())
         if len(args) == 1:
             message = args
             system = None
@@ -21,39 +20,36 @@
         elif len(args) == 2:
             message, system = args
             level = LogLevel.INFO
         else:
             message, system, level = args
 
         if expectedLevel is not None:
-            assert level == expectedLevel, "The Log message is of a diffrent type: %s"%level
+            assert level == expectedLevel, "The Log message is of a diffrent type: %s" % level
         if expectedSystem is not None:
-            assert system == expectedSystem, "The Log message if from a diffrent system: %s"%system
+            assert system == expectedSystem, "The Log message if from a diffrent system: %s" % system
 
         if exact:
-            assert message == contains, "The last log message does not match '%s': %s"%(contains, message)
+            assert message == contains, "The last log message does not match '%s': %s" % (contains, message)
         else:
-            assert contains in message, "The last log message does not contain '%s': %s"%(contains, message)
+            assert contains in message, "The last log message does not contain '%s': %s" % (contains, message)
 
     def assertWarningLike(self, contains, expectedSystem=None):
         self.assertLogMessageLike(contains, expectedSystem=expectedSystem, expectedLevel=LogLevel.WARNING)
 
     def assertErrorLike(self, contains, expectedSystem=None):
         self.assertLogMessageLike(contains, expectedSystem=expectedSystem, expectedLevel=LogLevel.ERROR)
 
     def assertSuccessLike(self, contains, expectedSystem=None):
         self.assertLogMessageLike(contains, expectedSystem=expectedSystem, expectedLevel=LogLevel.SUCCESS)
 
 
-
 def mockLogger(func):
-
     def inner1(*args, **kwargs):
-
-        patcher = patch('pyPhases.Logger.log')
+        patcher = patch("pyPhases.Logger.log")
         mock_read = patcher.start()
 
         args = list(args)
         selfArg = args.pop(0)
 
         # args = [selfArg] + [LoggerMock(mock_read)] + args
         args = [selfArg] + [LoggerMock(mock_read)] + args
```

### Comparing `pyPhases-1.1.9/pyPhases/test/TestCase.py` & `pyPhases-1.2.0/pyPhases/test/TestCase.py`

 * *Files 7% similar despite different names*

```diff
@@ -21,14 +21,15 @@
             self.logError(
                 "There is no Project set in static attribute TestCase.project, please use `phases test ...` to run your tests"
             )
         else:
             self.phase.project = TestCase.project
         super().__init__(methodName)
         self.restoreConfig = None
+        self.cleanData = True
 
     def config(self):
         return None
 
     def data(self):
         return {}
 
@@ -45,21 +46,23 @@
 
     def assertDataEqual(self, dataname, value):
         data = self.getData(dataname)
         self.assertEqual(data, value)
 
     def prepare(self) -> None:
         self.beforePrepare()
+        if self.cleanData:
+            TestCase.project.registeredData = {}
         config = self.config()
         config = pdict() if config is None else config
         registerData = self.data()
         self.phaseConfig = config
 
-        for field in config:
-            TestCase.project.setConfig(field, config[field])
+        TestCase.project.addConfig(config)
+        TestCase.project.trigger("configChanged", None)
 
         for field, data in registerData.items():
             TestCase.project.registerData(field, data)
 
         if self.phase is not None:
             self.phase.prepare()
```

### Comparing `pyPhases-1.1.9/pyPhases/test/TestRun.py` & `pyPhases-1.2.0/pyPhases/test/TestRun.py`

 * *Files identical despite different names*

### Comparing `pyPhases-1.1.9/pyPhases/util/BatchProgress.py` & `pyPhases-1.2.0/pyPhases/util/BatchProgress.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
         self.initBatchList(batchList)
         self.asynchronous = False
 
     def initBatchList(self, batchList):
         if batchList is not None:
             self.batchList = batchList if batchList is not None else self.batchList
             if self.startAt > 0:
-                self.batchList = self.batchList[self.startAt:]
+                self.batchList = self.batchList[self.startAt :]
             length = len(batchList)
             self.threads = min(self.threadCount, length, 40)
         return self.batchList
 
     def start(self, batchFunc, batchList=None, afterBatch=None):
         pool = None
         data = None
```

### Comparing `pyPhases-1.1.9/pyPhases/util/CSVLogger.py` & `pyPhases-1.2.0/pyPhases/util/CSVLogger.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import csv
 from pathlib import Path
 
 
 class CSVLogger:
-
     def __init__(self, csvLogFilePath: str):
         self.csvLogFilePath = csvLogFilePath
 
     def cleanCsv(self):
         if Path(self.csvLogFilePath).exists():
             Path(self.csvLogFilePath).unlink()
 
@@ -28,15 +27,15 @@
         csvFileHanlder.close()
 
     def getRowsReader(self, reader, removeHeader=True):
         try:
             with open(self.csvLogFilePath, "r", newline="") as csv_file:
                 rows = list(reader(csv_file))
                 # remove header
-                if removeHeader and len(rows) > 0:
+                if removeHeader and rows:
                     rows.pop(0)
         except FileNotFoundError:
             rows = []
         return rows
 
     def getRowsAsDict(self):
         return self.getRowsReader(csv.DictReader, removeHeader=False)
```

### Comparing `pyPhases-1.1.9/pyPhases/util/EventBus.py` & `pyPhases-1.2.0/pyPhases/util/EventBus.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 class EventBus:
     eventMap = {}
 
     def __init__(self):
         self.eventMap = {}
 
     def on(self, eventName, function):
-
         if eventName not in self.eventMap:
             self.eventMap[eventName] = []
         self.eventMap[eventName].append(function)
 
     def once(self, eventName, function):
-
         if eventName not in self.eventMap:
             self.eventMap[eventName] = []
 
         add = True
         for cb in self.eventMap[eventName]:
             if cb.__qualname__ == function.__qualname__:
                 add = False
```

### Comparing `pyPhases-1.1.9/pyPhases/util/Logger.py` & `pyPhases-1.2.0/pyPhases/util/Logger.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,15 +22,15 @@
             msg = "\033[33;1;4m%s\033[0m" % (msg)
         if level == LogLevel.ERROR:
             msg = "\033[31;1;4m%s\033[0m" % (msg)
         if level == LogLevel.SUCCESS:
             msg = "\033[32;1;4m%s\033[0m" % (msg)
 
         if Logger.verboseLevel.value <= level.value:
-            print(msg, end=end)
+            print(msg, end=end, flush=True)
 
 
 def classLogger(class_):
     def log(self, msg, level=LogLevel.INFO):
         system = type(self).__name__
         Logger.log(msg, system, level)
```

### Comparing `pyPhases-1.1.9/pyPhases/util/Optionizable.py` & `pyPhases-1.2.0/pyPhases/util/Optionizable.py`

 * *Files identical despite different names*

### Comparing `pyPhases-1.1.9/pyPhases/util/pdict.py` & `pyPhases-1.2.0/pyPhases/util/pdict.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,53 +3,51 @@
         k = args[0] if len(args) == 1 else args
         if not isinstance(k, list) and not isinstance(k, tuple):
             return super().__getitem__(k)
 
         value = self
         for field in k:
             try:
+                if isinstance(value, list):
+                    field = int(field)
                 value = value.__getitem__(field)
             except KeyError as e:
-                if create:
-                    v = pdict({})
-                    value.__setitem__(field, v)
-                    value = value.__getitem__(field)
-                else:
+                if not create:
                     raise e
 
+                v = pdict({})
+                value.__setitem__(field, v)
+                value = value.__getitem__(field)
         return value
 
     def __setitem__(self, orgPath, v):
         if not isinstance(orgPath, list) and not isinstance(orgPath, tuple):
             return super().__setitem__(orgPath, v)
+
         orgPath = list(orgPath)
-        value = self
-        k = orgPath.copy()
-        overwriteField = k.pop()
-        for field in k:
-            try:
-                value = value.__getitem__(field)
-            except KeyError:
-                value.__setitem__(field, pdict())
-                value = value.__getitem__(field)
-        value[overwriteField] = v
+        parentPath = orgPath[:-1]
+        overwriteField = orgPath[-1]
+        parent = self[parentPath]
+
+        if isinstance(parent, list):
+            overwriteField = int(overwriteField)
+        parent[overwriteField] = v
 
     def setdefaults(self, defaultDict):
         for key, value in pdict(defaultDict).items():
             if key in self:
-                if isinstance(self[key], dict):
+                if isinstance(self[key], dict) and bool(value):
+                    self[key] = pdict(self[key])
                     self[key].setdefaults(value)
             else:
                 self[key] = value
-        return self
 
     def update(self, values, path=None):
         path = path or []
         for field in values:
             value = values[field]
 
             if isinstance(value, dict) and field in self:
                 self[field] = pdict(self[field])
                 self[field].update(value)
             else:
                 self[field] = value
-        pass
```

### Comparing `pyPhases-1.1.9/pyPhases.egg-info/PKG-INFO` & `pyPhases-1.2.0/pyPhases.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyPhases
-Version: 1.1.9
+Version: 1.2.0
 Summary: A Framework for creating a boilerplate template for ai projects that are ready for MLOps
 Home-page: https://gitlab.com/tud.ibmt/pyPhases
 Author: Franz Ehrlich
 Author-email: fehrlichd@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pyPhases-1.1.9/pyPhases.egg-info/SOURCES.txt` & `pyPhases-1.2.0/pyPhases.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 LICENSE
 MANIFEST.in
 README.md
+pyproject.toml
 requirements.txt
 setup.py
 pyPhases/Data.py
 pyPhases/Phase.py
 pyPhases/PluginAdapter.py
 pyPhases/Project.py
 pyPhases/__init__.py
@@ -23,14 +24,15 @@
 pyPhases/test/TestCase.py
 pyPhases/test/TestCaseIntegration.py
 pyPhases/test/TestRun.py
 pyPhases/test/__init__.py
 pyPhases/util/BatchProgress.py
 pyPhases/util/CSVLogger.py
 pyPhases/util/EventBus.py
+pyPhases/util/EventBusStatic.py
 pyPhases/util/Logger.py
 pyPhases/util/Optionizable.py
 pyPhases/util/__init__.py
 pyPhases/util/pdict.py
 tests/__init__.py
 tests/test_acceptance.py
 tests/test/__init__.py
```

### Comparing `pyPhases-1.1.9/setup.py` & `pyPhases-1.2.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pyPhases",
-    version="v1.1.9"[1:],
+    version="v1.2.0"[1:],
     author="Franz Ehrlich",
     author_email="fehrlichd@gmail.com",
     description="A Framework for creating a boilerplate template for ai projects that are ready for MLOps",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://gitlab.com/tud.ibmt/pyPhases",
     packages=setuptools.find_packages(exclude="tests"),
```

### Comparing `pyPhases-1.1.9/tests/test/test_BaseTest.py` & `pyPhases-1.2.0/tests/test/test_BaseTest.py`

 * *Files identical despite different names*

### Comparing `pyPhases-1.1.9/tests/test/test_IntegrationTest.py` & `pyPhases-1.2.0/tests/test/test_IntegrationTest.py`

 * *Files identical despite different names*

### Comparing `pyPhases-1.1.9/tests/test/test_Mocks.py` & `pyPhases-1.2.0/tests/test/test_Mocks.py`

 * *Files identical despite different names*

### Comparing `pyPhases-1.1.9/tests/test/test_TestRun.py` & `pyPhases-1.2.0/tests/test/test_TestRun.py`

 * *Files identical despite different names*

### Comparing `pyPhases-1.1.9/tests/unit/test_BatchProgress.py` & `pyPhases-1.2.0/tests/unit/test_BatchProgress.py`

 * *Files 4% similar despite different names*

```diff
@@ -87,32 +87,26 @@
         function = MagicMock()
         bp = BatchProgress([1, 2, 3])
         bp.useMultiThreading = True
         bp.threads = 1
 
         with patch("multiprocessing.pool.Pool.map") as mock_map:
             bp.start(function)
-            mock_map.assert_has_calls([
-                call(function, [1]),
-                call(function, [2]),
-                call(function, [3])
-            ])
+            mock_map.assert_has_calls([call(function, [1]), call(function, [2]), call(function, [3])])
 
     def test_start_multithreading_asynchron(self):
         function = MagicMock()
         bp = BatchProgress([1, 2, 3])
         bp.useMultiThreading = True
         bp.threads = 2
 
         with patch("multiprocessing.pool.Pool.imap_unordered") as mock_map:
             bp.asynchronous = True
             bp.start(function)
-            mock_map.assert_has_calls([
-                call(function, [1, 2, 3])
-            ])
+            mock_map.assert_has_calls([call(function, [1, 2, 3])])
 
     def test_start_multithreading_asynchron_afterbatch(self):
         function = MagicMock()
         mock_afterBatch = MagicMock()
 
         bp = BatchProgress([1, 2, 3])
         bp.useMultiThreading = True
@@ -120,37 +114,38 @@
 
         with patch("multiprocessing.pool.Pool.imap_unordered") as mock_map:
             mock_map.return_value = ["r0", "r1", "r2"]
 
             bp.asynchronous = True
             bp.start(function, afterBatch=mock_afterBatch)
 
-            mock_map.assert_has_calls([
-                call(function, [1, 2, 3])
-            ])
-
-            mock_afterBatch.assert_has_calls([
-                call("r0"),
-                call("r1"),
-                call("r2"),
-            ])
+            mock_map.assert_has_calls([call(function, [1, 2, 3])])
 
-    def test_async_queue(self):
+            mock_afterBatch.assert_has_calls(
+                [
+                    call("r0"),
+                    call("r1"),
+                    call("r2"),
+                ]
+            )
 
+    def test_async_queue(self):
         def function(seconds):
             print("SLEEP FOR %s" % seconds)
             sleep(seconds)
             print("SLEEP FOR %s finished" % seconds)
             return seconds
 
         mock_afterBatch = MagicMock()
 
         bp = BatchProgress()
         bp.threads = 3
         bp.asyncQueue(function, [0.1, 0.2, 0.3, 0.05], update=mock_afterBatch)
 
-        mock_afterBatch.assert_has_calls([
-            call(0.1, 0.1),
-            call(0.2, 0.2),
-            call(0.3, 0.3),
-            call(0.05, 0.05),
-        ])
+        mock_afterBatch.assert_has_calls(
+            [
+                call(0.1, 0.1),
+                call(0.2, 0.2),
+                call(0.3, 0.3),
+                call(0.05, 0.05),
+            ]
+        )
```

### Comparing `pyPhases-1.1.9/tests/unit/test_Data.py` & `pyPhases-1.2.0/tests/unit/test_Data.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,83 +1,80 @@
 from unittest import TestCase
 from pyPhases.Data import Data
 from pyPhases.Project import Project
 from pyPhases.util.pdict import pdict
 
 
 class TestData(TestCase):
-
     def defaultTestData(self):
         testProject = Project("myProject")
         testProject.config = {"a": "foo", "b": "bar", "c": "c"}
 
         Data("myData", testProject, ["a"])
-        Data("myData2",testProject, ["a", "b"])
+        Data("myData2", testProject, ["a", "b"])
 
         return Data.create("testData", testProject, ["c", "myData"])
 
-
     def test_toString(self):
         testData = Data("myData", Project())
         self.assertEqual(str(testData), "myData")
 
     def test_Init(self):
-        testData = Data("test", Project(),  ["a", "b"])
+        testData = Data("test", Project(), ["a", "b"])
         self.assertEqual(testData.name, "test")
         self.assertEqual(testData.dataTags, ["a", "b"])
         self.assertEqual(testData.project.dataNames["test"], testData)
 
     def test_create(self):
         testProject = Project("myProject")
         testData = Data.create("test", testProject, ["a", "b"])
         self.assertEqual(testData.name, "test")
         self.assertEqual(testData.dataTags, ["a", "b"])
         self.assertEqual(testData.project.dataNames["test"], testData)
 
     def test_hasTobeHashed(self):
-        testData = Data("test", Project(),  ["a", "b"])
+        testData = Data("test", Project(), ["a", "b"])
         self.assertEqual(testData.hasTobeHashed(["a"]), True)
         self.assertEqual(testData.hasTobeHashed({"foo": "bar"}), True)
         self.assertEqual(testData.hasTobeHashed(pdict()), True)
         self.assertEqual(testData.hasTobeHashed(pdict({"foo": "bar"})), True)
 
         self.assertEqual(testData.hasTobeHashed("foo"), False)
         self.assertEqual(testData.hasTobeHashed(5), False)
         self.assertEqual(testData.hasTobeHashed(None), False)
 
     def test_flattenLongString(self):
-        testData = Data("test", Project(),  ["a", "b"])
+        testData = Data("test", Project(), ["a", "b"])
         self.assertEqual(testData.flattenLongString("foo"), "0beec7b5")
         self.assertEqual(testData.flattenLongString("foo bar"), "3773dea6")
         self.assertEqual(testData.flattenLongString("foo bar baz"), "c7567e8b")
         self.assertEqual(testData.flattenLongString("foo bar baz "), "f72f7597")
 
         self.assertEqual(testData.flattenLongString(str(["foo"])), "68681ff7")
         self.assertEqual(testData.flattenLongString(str({"foo": "bar"})), "8f3536a8")
 
     def test_flatten(self):
-        testData = Data("test", Project(),  ["a", "b"])
+        testData = Data("test", Project(), ["a", "b"])
         self.assertEqual(testData.flatten("foo"), "foo")
         self.assertEqual(testData.flatten(5), "5")
         self.assertEqual(testData.flatten(None), None)
         self.assertEqual(testData.flatten(["foo"]), "68681ff7")
         self.assertEqual(testData.flatten({"foo": "bar"}), "8f3536a8")
 
-
         self.assertEqual(testData.flatten("foo-bar"), "foo-bar")
         # remove spaces and brackets
         self.assertEqual(testData.flatten("foo (-)  bar"), "foo-bar")
 
         # replace special chars
         self.assertEqual(testData.flatten("€"), "-")
         self.assertEqual(testData.flatten("\\"), "-")
         self.assertEqual(testData.flatten("ß"), "-")
         self.assertEqual(testData.flatten("$"), "-")
         self.assertEqual(testData.flatten("&"), "-")
-        self.assertEqual(testData.flatten("\""), "-")
+        self.assertEqual(testData.flatten('"'), "-")
 
     def test_flattenConfigValues(self):
         self.assertEqual(Data.flattenConfigValues("foo bar"), "foobar")
 
     def test_getTagValueFromConfig(self):
         testProject = Project("myProject")
         testProject.config = {"a": "foo", "b": "bar", "c": "c"}
@@ -96,42 +93,42 @@
         self.assertEqual(testData._getTagValue("myData2"), "foo-bar")
 
     def test_getDependencyDictOnConfig(self):
         testProject = Project("myProject")
         testProject.config = {"a": "foo", "b": "bar", "c": "c"}
 
         testData = Data.create("testData", testProject, ["a", "b"])
-        self.assertEqual(testData.getDependencyDict(["a"]), {'a': 'foo'})
-        self.assertEqual(testData.getDependencyDict(["b"]), {'b': 'bar'})
-        self.assertEqual(testData.getDependencyDict(["a", "b"]), {'a': 'foo', 'b': 'bar'})
-        self.assertEqual(testData.getDependencyDict(), {'a': 'foo', 'b': 'bar'})
+        self.assertEqual(testData.getDependencyDict(["a"]), {"a": "foo"})
+        self.assertEqual(testData.getDependencyDict(["b"]), {"b": "bar"})
+        self.assertEqual(testData.getDependencyDict(["a", "b"]), {"a": "foo", "b": "bar"})
+        self.assertEqual(testData.getDependencyDict(), {"a": "foo", "b": "bar"})
 
     def test_getDependencyDictOnData(self):
         testProject = Project("myProject")
         Data("myData", testProject, ["a"])
         Data("myData2", testProject, ["a", "b"])
         testProject.config = {"a": "foo", "b": "bar", "c": "c"}
 
         testData = Data.create("testData", testProject, ["c", "myData"])
-        self.assertEqual(testData.getDependencyDict(["a"]), {'a': 'foo'})
-        self.assertEqual(testData.getDependencyDict(["b"]), {'b': 'bar'})
-        self.assertEqual(testData.getDependencyDict(["a", "b"]), {'a': 'foo', 'b': 'bar'})
-        self.assertEqual(testData.getDependencyDict(["myData"]), {'a': 'foo'})
-        self.assertEqual(testData.getDependencyDict(["myData2"]), {'a': 'foo', 'b': 'bar'})
+        self.assertEqual(testData.getDependencyDict(["a"]), {"a": "foo"})
+        self.assertEqual(testData.getDependencyDict(["b"]), {"b": "bar"})
+        self.assertEqual(testData.getDependencyDict(["a", "b"]), {"a": "foo", "b": "bar"})
+        self.assertEqual(testData.getDependencyDict(["myData"]), {"a": "foo"})
+        self.assertEqual(testData.getDependencyDict(["myData2"]), {"a": "foo", "b": "bar"})
 
-        self.assertEqual(testData.getDependencyDict(), {'c': 'c', 'a': 'foo'})
+        self.assertEqual(testData.getDependencyDict(), {"c": "c", "a": "foo"})
 
     def test_parseDatanames(self):
         testData = self.defaultTestData()
-        self.assertEqual(testData.parseDatanames(["c", "myData"]), 'c-foo')
+        self.assertEqual(testData.parseDatanames(["c", "myData"]), "c-foo")
 
     def test_getTagString(self):
         testData = self.defaultTestData()
-        self.assertEqual(testData.getTagString(), 'c-foo')
+        self.assertEqual(testData.getTagString(), "c-foo")
 
     def test_str(self):
         testData = self.defaultTestData()
-        self.assertEqual(str(testData), 'testDatac-foo')
+        self.assertEqual(str(testData), "testDatac-foo")
 
     def test_getDataId(self):
         testData = self.defaultTestData()
-        self.assertEqual(testData.getDataId(), 'testDatac-foo--current')
+        self.assertEqual(testData.getDataId(), "testDatac-foo--current")
```

### Comparing `pyPhases-1.1.9/tests/unit/test_DataExporter.py` & `pyPhases-1.2.0/tests/unit/test_DataExporter.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from unittest import TestCase
 from unittest.mock import patch
 
 from pyPhases.exporter.DataExporter import DataExporter
 
 
 class TestpyDataExporter(TestCase):
-
     def test_initialOption(self):
         exporter = DataExporter()
         self.assertEqual(exporter.getOption("basePath"), "./data")
 
     def test_notimplemented(self):
         exporter = DataExporter()
         self.assertRaises(Exception, exporter.stream, None)
```

### Comparing `pyPhases-1.1.9/tests/unit/test_EventBus.py` & `pyPhases-1.2.0/tests/unit/test_EventBus.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 from unittest import TestCase
 from pyPhases.util.EventBus import EventBus
 from unittest.mock import MagicMock
 
 
 class TestpyEventBus(TestCase):
-
     def test_on(self):
         eventBus = EventBus()
         callback = lambda: 5
-        eventBus.on('event1', callback)
-        self.assertIn('event1', eventBus.eventMap)
-        self.assertIn(callback, eventBus.eventMap['event1'])
+        eventBus.on("event1", callback)
+        self.assertIn("event1", eventBus.eventMap)
+        self.assertIn(callback, eventBus.eventMap["event1"])
 
     def test_once(self):
         eventBus = EventBus()
         callback = lambda: 5
-        eventBus.once('event1', callback)
-        eventBus.once('event1', callback)
-        self.assertIn('event1', eventBus.eventMap)
-        self.assertEqual(len(eventBus.eventMap['event1']), 1)
-        self.assertIn(callback, eventBus.eventMap['event1'])
+        eventBus.once("event1", callback)
+        eventBus.once("event1", callback)
+        self.assertIn("event1", eventBus.eventMap)
+        self.assertEqual(len(eventBus.eventMap["event1"]), 1)
+        self.assertIn(callback, eventBus.eventMap["event1"])
 
     def test_trigger(self):
         eventBus = EventBus()
         callback = MagicMock()
 
-        eventBus.on('event1', callback)
-        eventBus.trigger('event1', 'value1', 'value2')
-        callback.assert_called_with('value1', 'value2')
+        eventBus.on("event1", callback)
+        eventBus.trigger("event1", "value1", "value2")
+        callback.assert_called_with("value1", "value2")
```

### Comparing `pyPhases-1.1.9/tests/unit/test_Logger.py` & `pyPhases-1.2.0/tests/unit/test_Logger.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,87 +1,91 @@
 from unittest import TestCase
 from pyPhases.util.EventBus import EventBus
 from unittest.mock import MagicMock, patch
 from pyPhases.util.Logger import classLogger, Logger, LogLevel
 
 
 class TestLogger(TestCase):
-
-    @patch('builtins.print')
+    @patch("builtins.print")
     def test_Logger(self, mockPrint):
         Logger.verboseLevel = LogLevel.DEBUG
         Logger.log("test message", "test")
-        mockPrint.assert_called_with("[test] test message", end="\n")
+        mockPrint.assert_called_with("[test] test message", end="\n", flush=True)
 
-    @patch('builtins.print')
+    @patch("builtins.print")
     def test_LoggerToHigh(self, mockPrint):
         Logger.verboseLevel = LogLevel.ERROR
         Logger.log("test message", "test")
         mockPrint.assert_not_called()
 
-    @patch('builtins.print')
+    @patch("builtins.print")
     def test_LoggerWarning(self, mockPrint):
         Logger.verboseLevel = LogLevel.DEBUG
         Logger.log("test message", "test", LogLevel.WARNING)
-        mockPrint.assert_called_with("\033[33;1;4m%s\033[0m"%"[test] test message", end="\n")
+        mockPrint.assert_called_with("\033[33;1;4m%s\033[0m" % "[test] test message", end="\n", flush=True)
 
-    @patch('builtins.print')
+    @patch("builtins.print")
     def test_LoggerError(self, mockPrint):
         Logger.verboseLevel = LogLevel.DEBUG
         Logger.log("test message", "test", LogLevel.ERROR)
-        mockPrint.assert_called_with("\033[31;1;4m%s\033[0m"%"[test] test message", end="\n")
+        mockPrint.assert_called_with("\033[31;1;4m%s\033[0m" % "[test] test message", end="\n", flush=True)
 
-    @patch('builtins.print')
+    @patch("builtins.print")
     def test_LoggerSuccess(self, mockPrint):
         Logger.verboseLevel = LogLevel.DEBUG
         Logger.log("test message", "test", LogLevel.SUCCESS)
-        mockPrint.assert_called_with("\033[32;1;4m%s\033[0m"%"[test] test message", end="\n")
+        mockPrint.assert_called_with("\033[32;1;4m%s\033[0m" % "[test] test message", end="\n", flush=True)
 
-    @patch('pyPhases.util.Logger.Logger.log')
+    @patch("pyPhases.util.Logger.Logger.log")
     def test_classLoggerLog(self, logMock):
         @classLogger
         class MyClass:
             pass
+
         myClass = MyClass()
 
         myClass.log("test message", LogLevel.SUCCESS)
         logMock.assert_called_with("test message", "MyClass", LogLevel.SUCCESS)
 
-    @patch('pyPhases.util.Logger.Logger.log')
+    @patch("pyPhases.util.Logger.Logger.log")
     def test_classLoggerDebug(self, logMock):
         @classLogger
         class MyClass:
             pass
+
         myClass = MyClass()
 
         myClass.logDebug("test message")
         logMock.assert_called_with("test message", "MyClass", level=LogLevel.DEBUG)
 
-    @patch('pyPhases.util.Logger.Logger.log')
+    @patch("pyPhases.util.Logger.Logger.log")
     def test_classLoggerSuccess(self, logMock):
         @classLogger
         class MyClass:
             pass
+
         myClass = MyClass()
 
         myClass.logSuccess("test message")
         logMock.assert_called_with("test message", "MyClass", level=LogLevel.SUCCESS)
 
-    @patch('pyPhases.util.Logger.Logger.log')
+    @patch("pyPhases.util.Logger.Logger.log")
     def test_classLoggerWarning(self, logMock):
         @classLogger
         class MyClass:
             pass
+
         myClass = MyClass()
 
         myClass.logWarning("test message")
         logMock.assert_called_with("test message", "MyClass", level=LogLevel.WARNING)
 
-    @patch('pyPhases.util.Logger.Logger.log')
+    @patch("pyPhases.util.Logger.Logger.log")
     def test_classLoggerError(self, logMock):
         @classLogger
         class MyClass:
             pass
+
         myClass = MyClass()
 
         myClass.logError("test message")
         logMock.assert_called_with("test message", "MyClass", level=LogLevel.ERROR)
```

### Comparing `pyPhases-1.1.9/tests/unit/test_Loggermock.py` & `pyPhases-1.2.0/tests/unit/test_Loggermock.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,20 +4,25 @@
 from pyPhases import LogLevel
 from pyPhases.test.MockLogger import LoggerMock, mockLogger
 from pyPhases.util.Logger import classLogger
 
 
 @classLogger
 class TestLoggerMock(unittest.TestCase):
-
     @mockLogger
     def test_log_info(self, mock):
         self.log("test message")
         mock.expectLogMessage("test message", "TestLoggerMock", LogLevel.INFO)
-        self.assertRaises(AssertionError, mock.expectLogMessage, "message", "TestLoggerMock", LogLevel.INFO)
+        self.assertRaises(
+            AssertionError,
+            mock.expectLogMessage,
+            "message",
+            "TestLoggerMock",
+            LogLevel.INFO,
+        )
 
     @mockLogger
     def test_log_warning(self, mock):
         self.logWarning("test message")
         mock.expectLogMessage("test message", "TestLoggerMock", LogLevel.WARNING)
 
     @mockLogger
```

### Comparing `pyPhases-1.1.9/tests/unit/test_Optionizable.py` & `pyPhases-1.2.0/tests/unit/test_Optionizable.py`

 * *Files identical despite different names*

### Comparing `pyPhases-1.1.9/tests/unit/test_Phase.py` & `pyPhases-1.2.0/tests/unit/test_Phase.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from unittest import TestCase
 from pyPhases.Phase import Phase
 from pyPhases.Project import Project
 from unittest.mock import MagicMock
 from pyPhases.Data import Data
 
-class TestPhase(TestCase):
 
+class TestPhase(TestCase):
     def getDefaultPhase(self):
         return self.getDefaultPhaseAndProject()[0]
 
     def getDefaultPhaseAndProject(self):
         testProject = Project()
         testProject.config = {"a": "foo", "b": "bar", "Phase": {"phaseConfig": "value"}}
         testPhase = Phase(["a", "b"], {"foo": "bar"})
@@ -26,16 +26,18 @@
         self.assertEqual(testPhase.exportData, ["a", "b"])
         self.assertEqual(testPhase.options, {"foo": "bar"})
         self.assertEqual(testPhase.exportDataStrings, None)
         self.assertEqual(testPhase._prepared, False)
 
     def test_getId(self):
         testPhase = self.getDefaultPhase()
+
         class MyPhase(Phase):
             pass
+
         self.assertEqual(testPhase.getId(), "Phase")
         self.assertEqual(MyPhase().getId(), "MyPhase")
 
     def test_getId_name(self):
         testPhase = Phase()
         testPhase.name = "CustomName"
         self.assertEqual(testPhase.getId(), "CustomName")
@@ -68,34 +70,39 @@
         decorator.filter.assert_called_once_with(testPhase)
 
         decorator.filter.reset_mock()
         testPhase.decorators = projectDecorators
         self.assertEqual(testPhase.getDecorators(), projectDecorators)
         decorator.filter.assert_not_called()
 
-
     def test_getConfig(self):
         testPhase = self.getDefaultPhase()
         testPhase.project = MagicMock()
         testPhase.getConfig("test")
-        testPhase.project.getConfig.assert_called_with("test",None)
+        testPhase.project.getConfig.assert_called_with("test", None)
         testPhase.getConfig("test", 5)
-        testPhase.project.getConfig.assert_called_with("test",5)
+        testPhase.project.getConfig.assert_called_with("test", 5)
 
     def test_setConfig(self):
         testPhase = self.getDefaultPhase()
         testPhase.project = MagicMock()
         testPhase.setConfig("test", "value")
-        testPhase.project.setConfig.assert_called_with("test","value")
+        testPhase.project.setConfig.assert_called_with("test", "value")
 
     def test_getData(self):
         testPhase = self.getDefaultPhase()
         testPhase.project = MagicMock()
         testPhase.getData("test", None, "current", {}, True)
-        testPhase.project.getData.assert_called_with(dataName="test", expectedReturnType=None, version="current", options={}, generate=True)
+        testPhase.project.getData.assert_called_with(
+            dataName="test",
+            expectedReturnType=None,
+            version="current",
+            options={},
+            generate=True,
+        )
 
     def test_registerData(self):
         testPhase = self.getDefaultPhase()
         testPhase.project = MagicMock()
         testPhase.registerData("test", {}, "current", True)
         testPhase.project.registerData.assert_called_with(dataName="test", data={}, version="current", save=True)
 
@@ -127,11 +134,7 @@
         testPhase.decorators = [decoratorMock]
 
         testPhase.run()
 
         testPhase.main2.assert_called_once()
         decoratorMock.before.assert_called_once_with(testPhase)
         decoratorMock.after.assert_called_once_with(testPhase)
-
-
-
-
```

### Comparing `pyPhases-1.1.9/tests/unit/test_PluginAdapter.py` & `pyPhases-1.2.0/tests/unit/test_PluginAdapter.py`

 * *Files identical despite different names*

### Comparing `pyPhases-1.1.9/tests/unit/test_Project.py` & `pyPhases-1.2.0/tests/unit/test_Project.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 from pyPhases.exporter.PickleExporter import PickleExporter
 from unittest.mock import MagicMock, call, patch, mock_open
 from pyPhases.Phase import Phase
 from pyPhases.util.pdict import pdict
 
 
 class TestProject(TestCase):
-
     def test_registerDecorator(self):
         decorator = Decorator()
         project = Project()
         project.registerDecorator(decorator)
         self.assertIn(decorator, project.decorators)
 
     def test_registerExporter(self):
@@ -120,33 +119,33 @@
         project.registerExporter(exporter)
         Data("test", project)
 
         exporterObject = MagicMock()
         exporter.stream = exporterObject
         exporter.reinit = MagicMock(return_value=exporterObject)
 
-        project.dataExistIn("test", str, "testversion", options={"foo": "bar"})
+        project.dataExistIn("test", str, "testversion")
 
         exporter.reinit.assert_called_once()
-        exporterObject.exists.assert_called_with("test--testversion", {"foo": "bar"})
+        exporterObject.exists.assert_called_with("test--testversion")
 
     def test_dataExistInIsRegistered(self):
         project = Project()
         Data("test", project)
 
         project.registerData("test", "test")
 
         exist = project.dataExistIn("test", str)
         self.assertTrue(exist)
 
     def test_dataExistInNoExporter(self):
         project = Project()
         Data("test", project)
 
-        r = project.dataExistIn("test", str, "testversion", options={"foo": "bar"})
+        r = project.dataExistIn("test", str, "testversion")
 
         self.assertEqual(r, False)
 
     def test_unregister(self):
         project = Project()
         exporter = PickleExporter()
         project.registerExporter(exporter)
@@ -168,15 +167,22 @@
         project.registerExporter(exporter)
         Data("test", project)
 
         exporterObject = MagicMock()
         exporter.stream = exporterObject
         exporter.reinit = MagicMock(return_value=exporterObject)
 
-        self.assertRaises(KeyError, project.unregister, "test", str, "testversion", options={"foo": "bar"})
+        self.assertRaises(
+            KeyError,
+            project.unregister,
+            "test",
+            str,
+            "testversion",
+            options={"foo": "bar"},
+        )
 
     def test_getDataRegistered(self):
         project = Project()
         exporter = PickleExporter()
         project.registerExporter(exporter)
         Data("test", project)
 
@@ -215,39 +221,48 @@
     def test_generateData(self):
         project = Project()
         phase = Phase([Data("dataname", project)])
         project.addPhaseAndPrepare(phase)
 
         def generateData(id):
             phase.registerData("dataname", "test")
+
         phase.generateData = generateData
 
         teststr = project.generateData("dataname", str, "current")
         self.assertEqual(teststr, "test")
         self.assertEqual(project.registeredData["dataname--current"], "test")
 
     def test_generateDataWithoutRegister(self):
         project = Project()
         phase = Phase([Data("test", project)])
         project.addPhaseAndPrepare(phase)
 
         def generateData(id):
             return "test"
+
         phase.generateData = generateData
 
         teststr = project.generateData("test", str, "current")
         self.assertEqual(teststr, "test")
         self.assertNotIn("dataname--current", project.registeredData)
 
     def test_getDataGenerateNoGeneration(self):
         project = Project()
         phase = Phase([Data("test", project)])
         project.addPhaseAndPrepare(phase)
 
-        self.assertRaises(DataNotFound, project.generateData, "test", str, "current", options={"foo": "bar"})
+        self.assertRaises(
+            DataNotFound,
+            project.generateData,
+            "test",
+            str,
+            "current",
+            options={"foo": "bar"},
+        )
 
     def test_registerData(self):
         project = Project()
         exporter = PickleExporter()
         project.registerExporter(exporter)
         Data("test", project)
 
@@ -277,46 +292,58 @@
         self.assertEqual(project.registeredData["test--testversion"], "teststr")
 
     def test_setConfig(self):
         project = Project()
         project.setConfig("test", "test")
         self.assertEqual(project.config["test"], "test")
 
-    def test_setConfigDotNotation(self):
-        project = Project()
-        project.setConfig("test.blub", "test")
-        self.assertEqual(project.config["test"]["blub"], "test")
-
     def test_getConfig(self):
         project = Project()
         project.config["test"] = "test"
         self.assertEqual(project.getConfig("test"), "test")
 
     def test_getConfigDotNotation(self):
         project = Project()
         project.config["test"] = {"blub": "test"}
         self.assertEqual(project.getConfig("test.blub"), "test")
 
     def test_getConfigKeyError(self):
         project = Project()
         self.assertRaises(ConfigNotFoundException, project.getConfig, "test")
 
-    @patch('builtins.open', new_callable=mock_open, read_data='data')
+    def test_setConfigKeyError(self):
+        project = Project()
+        self.assertRaises(KeyError, project.setConfig, "test.blub", 5)
+
+    def get_getConfigDefault(self):
+        project = Project()
+        self.assertEqual(project.getConfig("nonExisting", "def"), "def")
+
+    def get_getConfigDefaultDot(self):
+        project = Project()
+        self.assertEqual(project.getConfig("nonExisting.test", "def"), "def")
+
+    def get_getConfigNotOverwrite(self):
+        project = Project()
+        self.assertEqual(project.getConfig("nonExisting.test", "def"), "def")
+        self.assertRaises(ConfigNotFoundException, project.getConfig, "nonExisting.test")
+
+    @patch("builtins.open", new_callable=mock_open, read_data="data")
     def test_saveConfig(self, m):
         json.dump = MagicMock()
         project = Project()
         project.setConfig("foo", "bar")
 
         m.return_value.__enter__.return_value = "data"
         project.saveConfig("myConfig.json")
 
         m.assert_called_with("myConfig.json", "w+")
         json.dump.assert_called_with({"foo": "bar"}, "data")
 
-    @patch('builtins.open', new_callable=mock_open, read_data='')
+    @patch("builtins.open", new_callable=mock_open, read_data="")
     def test_saveConfig_tailor(self, m):
         json.dump = MagicMock()
         project = Project()
         Data("test", project, ["subconfig"])
         project.config = {"subconfig": {"foo": "bar"}, "othervalue": "test"}
         m.return_value.__enter__.return_value = "data"
 
@@ -324,45 +351,47 @@
 
         m.assert_called_with("myConfig.json", "w+")
         json.dump.assert_called_with({"subconfig": {"foo": "bar"}}, "data")
 
     def test_importConfigsByImportValue(self):
         project = Project()
         project.loadConfig = MagicMock(return_value="a")
-        filePath = '/test1/test2/test3/test.yaml'
+        filePath = "/test1/test2/test3/test.yaml"
         baseConfig = {
             "foo": "bar",
             "test": [
                 "../test.yml",
                 "b.yml",
-            ]
+            ],
         }
         r = project.importConfigsByImportValue("test", baseConfig, filePath)
 
-        project.loadConfig.assert_has_calls([
-            call(Path('/test1/test2/test3/../test.yml')),
-            call(Path('/test1/test2/test3/b.yml')),
-        ])
+        project.loadConfig.assert_has_calls(
+            [
+                call(Path("/test1/test2/test3/../test.yml")),
+                call(Path("/test1/test2/test3/b.yml")),
+            ]
+        )
 
         self.assertEqual(r, ["a", "a"])
         self.assertEqual(baseConfig, {"foo": "bar"})
 
-    @patch('builtins.open', new_callable=mock_open, read_data='{"foo": "bar"}')
+    @patch("builtins.open", new_callable=mock_open, read_data='{"foo": "bar"}')
     def test_loadConfig(self, m):
         project = Project()
         project.config = pdict()
 
         config = project.loadConfig("myConfig.json")
 
         m.assert_called_with("myConfig.json", "r")
         self.assertIn("foo", config)
         self.assertEqual(config["foo"], "bar")
         self.assertEqual(project.config, {})
 
-    @patch('builtins.open', new_callable=mock_open, read_data='{"foo": "bar"}')
+    @patch("builtins.open", new_callable=mock_open, read_data='{"foo": "bar"}')
     def test_loadAndApplyConfig(self, m):
         project = Project()
         project.config = {"a": "b"}
 
         config = project.loadAndApplyConfig("myConfig.json")
 
         m.assert_called_with("myConfig.json", "r")
@@ -371,23 +400,22 @@
 
     def test_addConfig(self):
         project = Project()
         project.config = pdict({"foo": "keep", "foofoo": {"bar": "overwrite", "foo2": "keep"}})
         updateConfig = pdict({"foo2": "add", "foofoo": {"bar": "foo", "bar2": "add"}})
         project.addConfig(updateConfig)
 
-        self.assertEqual(project.config, {
-            "foo": "keep",
-            "foo2": "add",
-            "foofoo": {
-                "bar": "foo",
-                "foo2": "keep",
-                "bar2": "add"
-            }
-        })
+        self.assertEqual(
+            project.config,
+            {
+                "foo": "keep",
+                "foo2": "add",
+                "foofoo": {"bar": "foo", "foo2": "keep", "bar2": "add"},
+            },
+        )
 
     def test_addPhaseAndPrepare(self):
         project = Project()
         phase = Phase()
         project.addPhaseAndPrepare(phase)
         self.assertEqual(project.phases[0], phase)
         self.assertEqual(project.phases[0].name, "Phase")
@@ -397,29 +425,28 @@
         project = Project()
         phase = Phase()
         project.addPhaseAndPrepare(phase, "test")
         self.assertEqual(project.phases[0], phase)
         self.assertEqual(project.phases[0].name, "test")
         self.assertEqual(project.phaseMap["test"], phase)
 
-    @patch('pathlib.Path.exists', return_value=True)
+    @patch("pathlib.Path.exists", return_value=True)
     def test_addPlugin(self, m):
         project = Project()
 
         project.loadConfig = MagicMock(return_value={"foo2": "bar2"})
         pluginModule = MagicMock()
         importlib.import_module = MagicMock(return_value=pluginModule)
 
         pluginModule.__file__ = "pluginPath"
         project.addPlugin("myPlugin", {"foo": "bar"})
 
         plugin = importlib.import_module.return_value.Plugin
         pluginObj = importlib.import_module.return_value.Plugin.return_value
 
-
         importlib.import_module.assert_called_once_with(".Plugin", package="myPlugin")
         plugin.assert_called_once_with(project, {"foo": "bar"})
         self.assertEqual(project.plugins[0], pluginObj)
         pluginObj.initPlugin.assert_not_called()
         project.trigger("configChanged", None)
         pluginObj.initPlugin.assert_called_once()
 
@@ -466,21 +493,39 @@
 
         self.assertEqual(project.getPhase("Phase"), phase)
 
     def test_getPhaseNotExist(self):
         project = Project()
         self.assertRaises(PhaseNotFoundException, project.getPhase, "Phase")
 
-
     def test_enterContext(self):
         project = Project()
         project.config = pdict({"foo": "bar"})
         project.trigger = MagicMock()
 
         with project as p:
             p.setConfig("foo", "bar2")
             self.assertEqual(project.config["foo"], "bar2")
             project.trigger.assert_called_once_with("configChanged", "foo")
 
         self.assertEqual(project.config["foo"], "bar")
         project.trigger.assert_called_with("configChanged", None)
 
+    def test_nestedContexts(self):
+        project = Project()
+        project.config = pdict({"foo": "bar"})
+        project.trigger = MagicMock()
+
+        with project as p:
+            p.setConfig("foo", "bar2")
+            self.assertEqual(project.config["foo"], "bar2")
+            project.trigger.assert_called_once_with("configChanged", "foo")
+
+            with p:
+                p.setConfig("foo", "bar3")
+                self.assertEqual(project.config["foo"], "bar3")
+                project.trigger.assert_called_with("configChanged", "foo")
+
+            self.assertEqual(project.config["foo"], "bar2")
+
+        self.assertEqual(project.config["foo"], "bar")
+        project.trigger.assert_called_with("configChanged", None)
```

### Comparing `pyPhases-1.1.9/tests/unit/test_csvlogger.py` & `pyPhases-1.2.0/tests/unit/test_csvlogger.py`

 * *Files identical despite different names*

### Comparing `pyPhases-1.1.9/tests/unit/test_pdict.py` & `pyPhases-1.2.0/tests/unit/test_pdict.py`

 * *Files 9% similar despite different names*

```diff
@@ -101,7 +101,21 @@
 
         self.assertIn("config", a)
         self.assertIn("loader", a["config"])
         self.assertIn("a", a["config"]["loader"])
         self.assertIn("b", a["config"]["loader"])
         self.assertEqual(a["config"]["loader"]["a"], 5)
         self.assertEqual(a["config"]["loader"]["b"], 5)
+
+    def test_listStringIndex1(self):
+        a = pdict({"config": [0, 1]})
+
+        a["config", "0"] = 5
+
+        self.assertEqual(a["config", "0"], 5)
+
+    def test_listStringIndex2(self):
+        a = pdict({"config": {"a": [0, 1]}})
+
+        a["config", "a", "0"] = 5
+
+        self.assertEqual(a["config", "a", "0"], 5)
```

### Comparing `pyPhases-1.1.9/tests/util/ExporterTestHelper.py` & `pyPhases-1.2.0/tests/util/ExporterTestHelper.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,37 +1,31 @@
 from abc import abstractmethod
 
-class ExporterTestHelper():
 
+class ExporterTestHelper:
     @abstractmethod
     def getExporter(self):
         pass
 
     @abstractmethod
     def getSupportedObjects(self):
         pass
 
     def testCheckSupportedTypes(self):
         exporter = self.getExporter()
 
         for obj in self.getSupportedObjects():
             self.assertEqual(exporter.checkType(type(obj)), True)
 
-
     def testExportImport(self):
-
         exporter = self.getExporter()
 
         for index, obj in enumerate(self.getSupportedObjects()):
             dataId = "test" + str(index)
             self.assertFalse(exporter.exists(dataId))
             exporter.write(dataId, obj)
             self.assertTrue(exporter.exists(dataId))
 
             importedModel = exporter.read(dataId)
 
             self.assertIsInstance(importedModel, type(obj))
             self.assertEqual(importedModel, obj)
-
-
-
-
```

