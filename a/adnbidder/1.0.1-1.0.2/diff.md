# Comparing `tmp/adnbidder-1.0.1.tar.gz` & `tmp/adnbidder-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adnbidder-1.0.1.tar", last modified: Fri May 19 01:34:20 2023, max compression
+gzip compressed data, was "adnbidder-1.0.2.tar", last modified: Mon May 22 03:05:13 2023, max compression
```

## Comparing `adnbidder-1.0.1.tar` & `adnbidder-1.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 01:34:20.150368 adnbidder-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-19 01:34:09.000000 adnbidder-1.0.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-05-19 01:34:20.150368 adnbidder-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      996 2023-05-19 01:34:09.000000 adnbidder-1.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 01:34:20.150368 adnbidder-1.0.1/adnbidder/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-19 01:34:09.000000 adnbidder-1.0.1/adnbidder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13223 2023-05-19 01:34:09.000000 adnbidder-1.0.1/adnbidder/bidder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 01:34:20.150368 adnbidder-1.0.1/adnbidder.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-05-19 01:34:20.000000 adnbidder-1.0.1/adnbidder.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-05-19 01:34:20.000000 adnbidder-1.0.1/adnbidder.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 01:34:20.000000 adnbidder-1.0.1/adnbidder.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-19 01:34:20.000000 adnbidder-1.0.1/adnbidder.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-19 01:34:20.000000 adnbidder-1.0.1/adnbidder.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 01:34:20.150368 adnbidder-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-05-19 01:34:09.000000 adnbidder-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 03:05:13.364913 adnbidder-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-22 03:04:59.000000 adnbidder-1.0.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-05-22 03:05:13.364913 adnbidder-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-05-22 03:04:59.000000 adnbidder-1.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 03:05:13.364913 adnbidder-1.0.2/adnbidder/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-22 03:04:59.000000 adnbidder-1.0.2/adnbidder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13292 2023-05-22 03:04:59.000000 adnbidder-1.0.2/adnbidder/bidder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 03:05:13.364913 adnbidder-1.0.2/adnbidder.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-05-22 03:05:13.000000 adnbidder-1.0.2/adnbidder.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-05-22 03:05:13.000000 adnbidder-1.0.2/adnbidder.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 03:05:13.000000 adnbidder-1.0.2/adnbidder.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-22 03:05:13.000000 adnbidder-1.0.2/adnbidder.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-22 03:05:13.000000 adnbidder-1.0.2/adnbidder.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 03:05:13.364913 adnbidder-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-05-22 03:04:59.000000 adnbidder-1.0.2/setup.py
```

### Comparing `adnbidder-1.0.1/LICENSE.txt` & `adnbidder-1.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `adnbidder-1.0.1/README.md` & `adnbidder-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `adnbidder-1.0.1/adnbidder/bidder.py` & `adnbidder-1.0.2/adnbidder/bidder.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,25 +66,28 @@
         :param api_scheme: https or http
         :param api_host: Hostname for Adnuntius API server
         """
         api_location = api_scheme + '://' + api_host + '/api'
         self.api_client = Api(None, None, api_location, api_key=api_key)
         self.api_client.defaultArgs['context'] = network_id
         self.loop_period = timedelta(minutes=5)
-        self.exit = Event()
-        for sig in ('TERM', 'HUP', 'INT'):
-            signal.signal(getattr(signal, 'SIG' + sig), self.shutdown)
+        self.exit = None
 
     def start(self):
         """
         Starts the bidding service.
         This runs the main service loop, which periodically fetches the current bidding data for
         each active line-item and makes adjustments to the bid prices as required.
         """
         print('Bidder started!')
+        self.exit = Event()
+
+        for sig in ('TERM', 'HUP', 'INT'):
+            signal.signal(getattr(signal, 'SIG' + sig), self.shutdown)
+
         while not self.exit.is_set():
             self.update_all_bids()
             self.call_back()
             self.exit.wait(self.loop_period.total_seconds())
         sys.exit(0)
 
     def update_all_bids(self):
@@ -174,16 +177,17 @@
     def shutdown(self, sig=None, frame=None):
         """
         Shuts down the bidder immediately
         :param sig:
         :param frame:
         :return:
         """
-        print('Shutting down bidder...')
-        self.exit.set()
+        if self.exit is not None:
+            print('Shutting down bidder...')
+            self.exit.set()
 
     def call_back(self):
         """
         A method stub that can be overridden by child classes.
         This method will be called once per cycle in the main service loop.
         :return:
         """
```

### Comparing `adnbidder-1.0.1/setup.py` & `adnbidder-1.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import pathlib
 from setuptools import setup
 
 HERE = pathlib.Path(__file__).parent
 README = (HERE / "README.md").read_text()
 setup(
     name="adnbidder",
-    version="1.0.1",
+    version="1.0.2",
     description="A simple client for controlling bidding in the Adnuntius platform",
     long_description="A simple client for controlling bidding in the Adnuntius platform",
     url="https://github.com/Adnuntius/adnuntius-bidder",
     author="Adnuntius",
     author_email="tech@adnuntius.com",
     license="MIT",
     classifiers=[
```

