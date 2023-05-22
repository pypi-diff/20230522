# Comparing `tmp/piwaterflow-0.5.3.tar.gz` & `tmp/piwaterflow-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "piwaterflow-0.5.3.tar", last modified: Tue May  9 06:53:27 2023, max compression
+gzip compressed data, was "piwaterflow-0.5.4.tar", last modified: Mon May 22 06:18:58 2023, max compression
```

## Comparing `piwaterflow-0.5.3.tar` & `piwaterflow-0.5.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 06:53:27.301129 piwaterflow-0.5.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-05-09 06:53:27.301129 piwaterflow-0.5.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-05-09 06:53:13.000000 piwaterflow-0.5.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 06:53:27.297129 piwaterflow-0.5.3/piwaterflow/
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-09 06:53:13.000000 piwaterflow-0.5.3/piwaterflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-05-09 06:53:13.000000 piwaterflow-0.5.3/piwaterflow/config-template.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-05-09 06:53:13.000000 piwaterflow-0.5.3/piwaterflow/config_waterflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 06:53:27.301129 piwaterflow-0.5.3/piwaterflow/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 06:53:13.000000 piwaterflow-0.5.3/piwaterflow/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-05-09 06:53:13.000000 piwaterflow-0.5.3/piwaterflow/tests/test_000.py
--rw-r--r--   0 runner    (1001) docker     (123)    21459 2023-05-09 06:53:13.000000 piwaterflow-0.5.3/piwaterflow/waterflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 06:53:27.301129 piwaterflow-0.5.3/piwaterflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-05-09 06:53:27.000000 piwaterflow-0.5.3/piwaterflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-05-09 06:53:27.000000 piwaterflow-0.5.3/piwaterflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 06:53:27.000000 piwaterflow-0.5.3/piwaterflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-09 06:53:27.000000 piwaterflow-0.5.3/piwaterflow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-09 06:53:27.000000 piwaterflow-0.5.3/piwaterflow.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 06:53:27.301129 piwaterflow-0.5.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-05-09 06:53:13.000000 piwaterflow-0.5.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 06:53:27.301129 piwaterflow-0.5.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 06:53:13.000000 piwaterflow-0.5.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-05-09 06:53:13.000000 piwaterflow-0.5.3/tests/test_000_loop.py
--rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-05-09 06:53:13.000000 piwaterflow-0.5.3/tests/test_001_forward.py
--rw-r--r--   0 runner    (1001) docker     (123)     2463 2023-05-09 06:53:13.000000 piwaterflow-0.5.3/tests/test_002_reverse.py
--rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-05-09 06:53:13.000000 piwaterflow-0.5.3/tests/test_003_lock.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:18:58.631210 piwaterflow-0.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-05-22 06:18:58.631210 piwaterflow-0.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-05-22 06:18:43.000000 piwaterflow-0.5.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:18:58.627210 piwaterflow-0.5.4/piwaterflow/
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-22 06:18:43.000000 piwaterflow-0.5.4/piwaterflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-05-22 06:18:43.000000 piwaterflow-0.5.4/piwaterflow/config-template.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-05-22 06:18:43.000000 piwaterflow-0.5.4/piwaterflow/config_waterflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:18:58.631210 piwaterflow-0.5.4/piwaterflow/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 06:18:43.000000 piwaterflow-0.5.4/piwaterflow/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-05-22 06:18:43.000000 piwaterflow-0.5.4/piwaterflow/tests/test_000.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21323 2023-05-22 06:18:43.000000 piwaterflow-0.5.4/piwaterflow/waterflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:18:58.631210 piwaterflow-0.5.4/piwaterflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-05-22 06:18:58.000000 piwaterflow-0.5.4/piwaterflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-05-22 06:18:58.000000 piwaterflow-0.5.4/piwaterflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 06:18:58.000000 piwaterflow-0.5.4/piwaterflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-22 06:18:58.000000 piwaterflow-0.5.4/piwaterflow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-22 06:18:58.000000 piwaterflow-0.5.4/piwaterflow.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 06:18:58.631210 piwaterflow-0.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-05-22 06:18:43.000000 piwaterflow-0.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:18:58.631210 piwaterflow-0.5.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 06:18:43.000000 piwaterflow-0.5.4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-05-22 06:18:43.000000 piwaterflow-0.5.4/tests/test_000_loop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-05-22 06:18:43.000000 piwaterflow-0.5.4/tests/test_001_forward.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2463 2023-05-22 06:18:43.000000 piwaterflow-0.5.4/tests/test_002_reverse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-05-22 06:18:43.000000 piwaterflow-0.5.4/tests/test_003_lock.py
```

### Comparing `piwaterflow-0.5.3/PKG-INFO` & `piwaterflow-0.5.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: piwaterflow
-Version: 0.5.3
+Version: 0.5.4
 Summary: Raspberry Pi Waterflow resilient system
 Home-page: https://github.com/Phornee/piwaterflow
 Author: Ismael Raya
 Author-email: phornee@gmail.com
 License: UNKNOWN
 Description: # PiWaterflow
         This is a resilient watering system, executed in a Raspberry Pi to control irrigation valves using relays.
```

### Comparing `piwaterflow-0.5.3/README.md` & `piwaterflow-0.5.4/README.md`

 * *Files identical despite different names*

### Comparing `piwaterflow-0.5.3/piwaterflow/config-template.yml` & `piwaterflow-0.5.4/piwaterflow/config-template.yml`

 * *Files identical despite different names*

### Comparing `piwaterflow-0.5.3/piwaterflow/config_waterflow.py` & `piwaterflow-0.5.4/piwaterflow/config_waterflow.py`

 * *Files identical despite different names*

### Comparing `piwaterflow-0.5.3/piwaterflow/tests/test_000.py` & `piwaterflow-0.5.4/piwaterflow/tests/test_000.py`

 * *Files identical despite different names*

### Comparing `piwaterflow-0.5.3/piwaterflow/waterflow.py` & `piwaterflow-0.5.4/piwaterflow/waterflow.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,37 +31,34 @@
     def __init__(self, template_config_path: str = None, dry_run: bool = False):
         """__init__ of the function
         Args:
             template_config_path (str, optional): Template config to use. Defaults to None.
             dry_run (bool, optional): If true, it will just simulate, and wont make any change. Defaults to False.
         """
         self.homevar = os.path.join(str(Path.home()), 'var', self.class_name())
+        
+        self.dry_run = dry_run
 
         if dry_run:
-            self.dry_run = True
             self.homevar = os.path.join(self.homevar, 'dryrun')
             if os.path.exists(self.homevar): # Only one instance of waterflow can run at a time, so this is safe
                 shutil.rmtree(self.homevar)
             if not os.path.exists(self.homevar):
                 os.makedirs(self.homevar)
-            dry_run_abs_path = ""
-        else:
-            self.dry_run = False
-            dry_run_abs_path = None
 
         self.debuglogger = Logger(self.class_name(), 'waterflow', dry_run=dry_run)
         self.userlogger = Logger(self.class_name(), 'loop', dry_run=dry_run)
 
         if not template_config_path:
             template_config_path = os.path.join(Path(__file__).parent.resolve(), './config-template.yml')
 
         self.config = WaterflowConfig(package_name=self.class_name(),
-                                        template_path=template_config_path,
-                                        config_file_name="config.yml",
-                                        dry_run_abs_path=dry_run_abs_path)
+                                      template_path=template_config_path,
+                                      config_file_name="config.yml",
+                                      dry_run=dry_run)
 
         influx_conn_type = self.config['influxdbconn'].get('type', 'influx')
         self.conn = influxdb_factory(influx_conn_type)
         self.conn.openConn(self.config['influxdbconn'])
 
     def __del__(self):
         if self.dry_run:
```

### Comparing `piwaterflow-0.5.3/piwaterflow.egg-info/PKG-INFO` & `piwaterflow-0.5.4/piwaterflow.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: piwaterflow
-Version: 0.5.3
+Version: 0.5.4
 Summary: Raspberry Pi Waterflow resilient system
 Home-page: https://github.com/Phornee/piwaterflow
 Author: Ismael Raya
 Author-email: phornee@gmail.com
 License: UNKNOWN
 Description: # PiWaterflow
         This is a resilient watering system, executed in a Raspberry Pi to control irrigation valves using relays.
```

### Comparing `piwaterflow-0.5.3/setup.py` & `piwaterflow-0.5.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="piwaterflow",
-    version="0.5.3",
+    version="0.5.4",
     author="Ismael Raya",
     author_email="phornee@gmail.com",
     description="Raspberry Pi Waterflow resilient system",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Phornee/piwaterflow",
     packages=setuptools.find_packages(),
@@ -21,14 +21,14 @@
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
         "Topic :: Home Automation",
     ],
     install_requires=[
         'log_mgr>=0.0.2',
-        'config_yml>=0.2.3',
+        'config_yml>=0.3.0',
         'RPi.GPIO>=0.7.0',
         'fake-rpigpio>=0.1.1',
         'influxdb_wrapper>=0.0.3'
     ],
     python_requires='>=3.6',
 )
```

### Comparing `piwaterflow-0.5.3/tests/test_000_loop.py` & `piwaterflow-0.5.4/tests/test_000_loop.py`

 * *Files identical despite different names*

### Comparing `piwaterflow-0.5.3/tests/test_001_forward.py` & `piwaterflow-0.5.4/tests/test_001_forward.py`

 * *Files identical despite different names*

### Comparing `piwaterflow-0.5.3/tests/test_002_reverse.py` & `piwaterflow-0.5.4/tests/test_002_reverse.py`

 * *Files identical despite different names*

### Comparing `piwaterflow-0.5.3/tests/test_003_lock.py` & `piwaterflow-0.5.4/tests/test_003_lock.py`

 * *Files identical despite different names*

