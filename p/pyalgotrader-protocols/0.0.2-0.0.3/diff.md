# Comparing `tmp/pyalgotrader-protocols-0.0.2.tar.gz` & `tmp/pyalgotrader-protocols-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyalgotrader-protocols-0.0.2.tar", last modified: Wed May 17 01:41:42 2023, max compression
+gzip compressed data, was "pyalgotrader-protocols-0.0.3.tar", last modified: Mon May 22 02:31:32 2023, max compression
```

## Comparing `pyalgotrader-protocols-0.0.2.tar` & `pyalgotrader-protocols-0.0.3.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxrwxr-x   0 krunaldodiya  (1000) krunaldodiya  (1000)        0 2023-05-17 01:41:41.995088 pyalgotrader-protocols-0.0.2/
--rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)        0 2023-03-22 08:25:41.000000 pyalgotrader-protocols-0.0.2/LICENSE
--rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)      405 2023-05-17 01:41:41.995088 pyalgotrader-protocols-0.0.2/PKG-INFO
--rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)       23 2023-03-22 08:25:41.000000 pyalgotrader-protocols-0.0.2/README.md
-drwxrwxr-x   0 krunaldodiya  (1000) krunaldodiya  (1000)        0 2023-05-17 01:41:41.995088 pyalgotrader-protocols-0.0.2/pyalgotrader_protocols/
--rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)      190 2023-03-22 08:25:41.000000 pyalgotrader-protocols-0.0.2/pyalgotrader_protocols/__init__.py
--rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)      573 2023-03-22 08:25:41.000000 pyalgotrader-protocols-0.0.2/pyalgotrader_protocols/algorithm.py
--rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)      434 2023-03-22 08:25:41.000000 pyalgotrader-protocols-0.0.2/pyalgotrader_protocols/broker.py
--rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)      622 2023-03-22 08:25:41.000000 pyalgotrader-protocols-0.0.2/pyalgotrader_protocols/broker_manager.py
--rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)      498 2023-05-15 02:37:46.000000 pyalgotrader-protocols-0.0.2/pyalgotrader_protocols/chart.py
--rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)       37 2023-05-17 01:39:43.000000 pyalgotrader-protocols-0.0.2/pyalgotrader_protocols/data_manager.py
--rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)      490 2023-03-22 08:25:41.000000 pyalgotrader-protocols-0.0.2/pyalgotrader_protocols/feed.py
--rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)      191 2023-05-15 02:37:46.000000 pyalgotrader-protocols-0.0.2/pyalgotrader_protocols/indicator.py
--rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)      491 2023-03-22 08:25:41.000000 pyalgotrader-protocols-0.0.2/pyalgotrader_protocols/store.py
--rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)      210 2023-03-22 08:25:41.000000 pyalgotrader-protocols-0.0.2/pyalgotrader_protocols/strategy.py
--rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)      131 2023-03-22 08:25:41.000000 pyalgotrader-protocols-0.0.2/pyalgotrader_protocols/symbol.py
-drwxrwxr-x   0 krunaldodiya  (1000) krunaldodiya  (1000)        0 2023-05-17 01:41:41.995088 pyalgotrader-protocols-0.0.2/pyalgotrader_protocols.egg-info/
--rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)      405 2023-05-17 01:41:41.000000 pyalgotrader-protocols-0.0.2/pyalgotrader_protocols.egg-info/PKG-INFO
--rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)      638 2023-05-17 01:41:41.000000 pyalgotrader-protocols-0.0.2/pyalgotrader_protocols.egg-info/SOURCES.txt
--rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)        1 2023-05-17 01:41:41.000000 pyalgotrader-protocols-0.0.2/pyalgotrader_protocols.egg-info/dependency_links.txt
--rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)        9 2023-05-17 01:41:41.000000 pyalgotrader-protocols-0.0.2/pyalgotrader_protocols.egg-info/requires.txt
--rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)       23 2023-05-17 01:41:41.000000 pyalgotrader-protocols-0.0.2/pyalgotrader_protocols.egg-info/top_level.txt
--rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)       38 2023-05-17 01:41:41.995088 pyalgotrader-protocols-0.0.2/setup.cfg
--rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)      878 2023-05-17 01:40:10.000000 pyalgotrader-protocols-0.0.2/setup.py
+drwxrwxr-x   0 krunaldodiya  (1000) krunaldodiya  (1000)        0 2023-05-22 02:31:32.222827 pyalgotrader-protocols-0.0.3/
+-rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)        0 2023-03-22 08:25:41.000000 pyalgotrader-protocols-0.0.3/LICENSE
+-rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)      405 2023-05-22 02:31:32.222827 pyalgotrader-protocols-0.0.3/PKG-INFO
+-rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)       23 2023-03-22 08:25:41.000000 pyalgotrader-protocols-0.0.3/README.md
+drwxrwxr-x   0 krunaldodiya  (1000) krunaldodiya  (1000)        0 2023-05-22 02:31:32.222827 pyalgotrader-protocols-0.0.3/pyalgotrader_protocols/
+-rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)      190 2023-03-22 08:25:41.000000 pyalgotrader-protocols-0.0.3/pyalgotrader_protocols/__init__.py
+-rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)      573 2023-03-22 08:25:41.000000 pyalgotrader-protocols-0.0.3/pyalgotrader_protocols/algorithm.py
+-rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)      434 2023-03-22 08:25:41.000000 pyalgotrader-protocols-0.0.3/pyalgotrader_protocols/broker.py
+-rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)      622 2023-03-22 08:25:41.000000 pyalgotrader-protocols-0.0.3/pyalgotrader_protocols/broker_manager.py
+-rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)      498 2023-05-15 02:37:46.000000 pyalgotrader-protocols-0.0.3/pyalgotrader_protocols/chart.py
+-rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)       21 2023-05-22 02:29:28.000000 pyalgotrader-protocols-0.0.3/pyalgotrader_protocols/data.py
+-rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)       37 2023-05-17 01:49:18.000000 pyalgotrader-protocols-0.0.3/pyalgotrader_protocols/data_manager.py
+-rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)      493 2023-05-22 02:29:11.000000 pyalgotrader-protocols-0.0.3/pyalgotrader_protocols/feed.py
+-rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)      191 2023-05-15 02:37:46.000000 pyalgotrader-protocols-0.0.3/pyalgotrader_protocols/indicator.py
+-rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)      491 2023-03-22 08:25:41.000000 pyalgotrader-protocols-0.0.3/pyalgotrader_protocols/store.py
+-rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)      210 2023-03-22 08:25:41.000000 pyalgotrader-protocols-0.0.3/pyalgotrader_protocols/strategy.py
+-rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)      131 2023-03-22 08:25:41.000000 pyalgotrader-protocols-0.0.3/pyalgotrader_protocols/symbol.py
+drwxrwxr-x   0 krunaldodiya  (1000) krunaldodiya  (1000)        0 2023-05-22 02:31:32.222827 pyalgotrader-protocols-0.0.3/pyalgotrader_protocols.egg-info/
+-rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)      405 2023-05-22 02:31:32.000000 pyalgotrader-protocols-0.0.3/pyalgotrader_protocols.egg-info/PKG-INFO
+-rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)      669 2023-05-22 02:31:32.000000 pyalgotrader-protocols-0.0.3/pyalgotrader_protocols.egg-info/SOURCES.txt
+-rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)        1 2023-05-22 02:31:32.000000 pyalgotrader-protocols-0.0.3/pyalgotrader_protocols.egg-info/dependency_links.txt
+-rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)        9 2023-05-22 02:31:32.000000 pyalgotrader-protocols-0.0.3/pyalgotrader_protocols.egg-info/requires.txt
+-rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)       23 2023-05-22 02:31:32.000000 pyalgotrader-protocols-0.0.3/pyalgotrader_protocols.egg-info/top_level.txt
+-rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)       38 2023-05-22 02:31:32.222827 pyalgotrader-protocols-0.0.3/setup.cfg
+-rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)      878 2023-05-22 02:29:54.000000 pyalgotrader-protocols-0.0.3/setup.py
```

### Comparing `pyalgotrader-protocols-0.0.2/pyalgotrader_protocols/algorithm.py` & `pyalgotrader-protocols-0.0.3/pyalgotrader_protocols/algorithm.py`

 * *Files identical despite different names*

### Comparing `pyalgotrader-protocols-0.0.2/pyalgotrader_protocols/broker_manager.py` & `pyalgotrader-protocols-0.0.3/pyalgotrader_protocols/broker_manager.py`

 * *Files identical despite different names*

### Comparing `pyalgotrader-protocols-0.0.2/pyalgotrader_protocols.egg-info/SOURCES.txt` & `pyalgotrader-protocols-0.0.3/pyalgotrader_protocols.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 README.md
 setup.py
 pyalgotrader_protocols/__init__.py
 pyalgotrader_protocols/algorithm.py
 pyalgotrader_protocols/broker.py
 pyalgotrader_protocols/broker_manager.py
 pyalgotrader_protocols/chart.py
+pyalgotrader_protocols/data.py
 pyalgotrader_protocols/data_manager.py
 pyalgotrader_protocols/feed.py
 pyalgotrader_protocols/indicator.py
 pyalgotrader_protocols/store.py
 pyalgotrader_protocols/strategy.py
 pyalgotrader_protocols/symbol.py
 pyalgotrader_protocols.egg-info/PKG-INFO
```

### Comparing `pyalgotrader-protocols-0.0.2/setup.py` & `pyalgotrader-protocols-0.0.3/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 with readme.open("r") as f:
     long_description = f.read()
 
 setuptools.setup(
     include_package_data=True,
     data_files=[(current_directory, ["README.md", "LICENSE"])],
     name="pyalgotrader-protocols",
-    version="0.0.2",
+    version="0.0.3",
     description="PyAlgoTrader Protocols",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/krunaldodiya/pyalgotrader-protocols",
     author="Krunal Dodiya",
     author_email="kunal.dodiya1@gmail.com",
     packages=setuptools.find_packages(),
```

