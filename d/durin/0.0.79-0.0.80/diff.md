# Comparing `tmp/durin-0.0.79.tar.gz` & `tmp/durin-0.0.80.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "durin-0.0.79.tar", last modified: Wed May 10 12:23:18 2023, max compression
+gzip compressed data, was "durin-0.0.80.tar", last modified: Mon May 22 11:52:44 2023, max compression
```

## Comparing `durin-0.0.79.tar` & `durin-0.0.80.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:23:18.946756 durin-0.0.79/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-10 12:23:08.000000 durin-0.0.79/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2929 2023-05-10 12:23:18.946756 durin-0.0.79/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)     2683 2023-05-10 12:23:08.000000 durin-0.0.79/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:23:18.942756 durin-0.0.79/bin/
--rwxr-xr-x   0 runner    (1001) docker     (123)       34 2023-05-10 12:23:08.000000 durin-0.0.79/bin/durin
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:23:18.942756 durin-0.0.79/durin/
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-05-10 12:23:08.000000 durin-0.0.79/durin/Profiler.py
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-05-10 12:23:08.000000 durin-0.0.79/durin/Read_profilers.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       80 2023-05-10 12:23:08.000000 durin-0.0.79/durin/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      475 2023-05-10 12:23:08.000000 durin-0.0.79/durin/__main__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      766 2023-05-10 12:23:08.000000 durin-0.0.79/durin/actuator.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4148 2023-05-10 12:23:08.000000 durin-0.0.79/durin/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:23:18.942756 durin-0.0.79/durin/controller/
--rwxr-xr-x   0 runner    (1001) docker     (123)       40 2023-05-10 12:23:08.000000 durin-0.0.79/durin/controller/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      344 2023-05-10 12:23:08.000000 durin-0.0.79/durin/controller/dvs.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4307 2023-05-10 12:23:08.000000 durin-0.0.79/durin/controller/server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:23:18.942756 durin-0.0.79/durin/controller/test/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:23:08.000000 durin-0.0.79/durin/controller/test/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      947 2023-05-10 12:23:08.000000 durin-0.0.79/durin/controller/test/test_stream.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4694 2023-05-10 12:23:08.000000 durin-0.0.79/durin/durin.py
--rwxr-xr-x   0 runner    (1001) docker     (123)   181742 2023-05-10 12:23:08.000000 durin-0.0.79/durin/durin_birdseye.jpg
--rwxr-xr-x   0 runner    (1001) docker     (123)      504 2023-05-10 12:23:08.000000 durin-0.0.79/durin/dvs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:23:18.946756 durin-0.0.79/durin/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-05-10 12:23:08.000000 durin-0.0.79/durin/examples/CPU_test.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 12:23:08.000000 durin-0.0.79/durin/examples/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2281 2023-05-10 12:23:08.000000 durin-0.0.79/durin/examples/braitenberg.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2631 2023-05-10 12:23:08.000000 durin-0.0.79/durin/examples/commands.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1632 2023-05-10 12:23:08.000000 durin-0.0.79/durin/examples/dashboard.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      923 2023-05-10 12:23:08.000000 durin-0.0.79/durin/examples/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-05-10 12:23:08.000000 durin-0.0.79/durin/examples/plot.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      589 2023-05-10 12:23:08.000000 durin-0.0.79/durin/examples/record.py
--rw-r--r--   0 runner    (1001) docker     (123)     2865 2023-05-10 12:23:08.000000 durin-0.0.79/durin/examples/stats.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:23:18.946756 durin-0.0.79/durin/io/
--rwxr-xr-x   0 runner    (1001) docker     (123)      673 2023-05-10 12:23:08.000000 durin-0.0.79/durin/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5073 2023-05-10 12:23:08.000000 durin-0.0.79/durin/io/command.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1442 2023-05-10 12:23:08.000000 durin-0.0.79/durin/io/gamepad.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6181 2023-05-10 12:23:08.000000 durin-0.0.79/durin/io/network.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      525 2023-05-10 12:23:08.000000 durin-0.0.79/durin/io/ringbuffer.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1824 2023-05-10 12:23:08.000000 durin-0.0.79/durin/io/runnable.py
--rw-r--r--   0 runner    (1001) docker     (123)     9042 2023-05-10 12:23:08.000000 durin-0.0.79/durin/io/schema.capnp
--rwxr-xr-x   0 runner    (1001) docker     (123)     7102 2023-05-10 12:23:08.000000 durin-0.0.79/durin/sensor.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    14672 2023-05-10 12:23:08.000000 durin-0.0.79/durin/ui.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:23:18.942756 durin-0.0.79/durin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2929 2023-05-10 12:23:18.000000 durin-0.0.79/durin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      906 2023-05-10 12:23:18.000000 durin-0.0.79/durin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 12:23:18.000000 durin-0.0.79/durin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-10 12:23:18.000000 durin-0.0.79/durin.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-10 12:23:18.000000 durin-0.0.79/durin.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 12:23:18.946756 durin-0.0.79/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)      663 2023-05-10 12:23:08.000000 durin-0.0.79/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 11:52:44.428178 durin-0.0.80/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-22 11:52:35.000000 durin-0.0.80/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2929 2023-05-22 11:52:44.428178 durin-0.0.80/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2683 2023-05-22 11:52:35.000000 durin-0.0.80/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 11:52:44.424178 durin-0.0.80/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       34 2023-05-22 11:52:35.000000 durin-0.0.80/bin/durin
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 11:52:44.424178 durin-0.0.80/durin/
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-05-22 11:52:35.000000 durin-0.0.80/durin/Profiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-05-22 11:52:35.000000 durin-0.0.80/durin/Read_profilers.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       80 2023-05-22 11:52:35.000000 durin-0.0.80/durin/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      475 2023-05-22 11:52:35.000000 durin-0.0.80/durin/__main__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      766 2023-05-22 11:52:35.000000 durin-0.0.80/durin/actuator.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4148 2023-05-22 11:52:35.000000 durin-0.0.80/durin/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 11:52:44.424178 durin-0.0.80/durin/controller/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       40 2023-05-22 11:52:35.000000 durin-0.0.80/durin/controller/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      344 2023-05-22 11:52:35.000000 durin-0.0.80/durin/controller/dvs.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4307 2023-05-22 11:52:35.000000 durin-0.0.80/durin/controller/server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 11:52:44.424178 durin-0.0.80/durin/controller/test/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 11:52:35.000000 durin-0.0.80/durin/controller/test/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      947 2023-05-22 11:52:35.000000 durin-0.0.80/durin/controller/test/test_stream.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4694 2023-05-22 11:52:35.000000 durin-0.0.80/durin/durin.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)   181742 2023-05-22 11:52:35.000000 durin-0.0.80/durin/durin_birdseye.jpg
+-rwxr-xr-x   0 runner    (1001) docker     (123)      504 2023-05-22 11:52:35.000000 durin-0.0.80/durin/dvs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 11:52:44.428178 durin-0.0.80/durin/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-05-22 11:52:35.000000 durin-0.0.80/durin/examples/CPU_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 11:52:35.000000 durin-0.0.80/durin/examples/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2281 2023-05-22 11:52:35.000000 durin-0.0.80/durin/examples/braitenberg.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2631 2023-05-22 11:52:35.000000 durin-0.0.80/durin/examples/commands.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1448 2023-05-22 11:52:35.000000 durin-0.0.80/durin/examples/dashboard.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      923 2023-05-22 11:52:35.000000 durin-0.0.80/durin/examples/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-05-22 11:52:35.000000 durin-0.0.80/durin/examples/plot.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      589 2023-05-22 11:52:35.000000 durin-0.0.80/durin/examples/record.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2865 2023-05-22 11:52:35.000000 durin-0.0.80/durin/examples/stats.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 11:52:44.428178 durin-0.0.80/durin/io/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      673 2023-05-22 11:52:35.000000 durin-0.0.80/durin/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5073 2023-05-22 11:52:35.000000 durin-0.0.80/durin/io/command.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1442 2023-05-22 11:52:35.000000 durin-0.0.80/durin/io/gamepad.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6181 2023-05-22 11:52:35.000000 durin-0.0.80/durin/io/network.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      525 2023-05-22 11:52:35.000000 durin-0.0.80/durin/io/ringbuffer.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1824 2023-05-22 11:52:35.000000 durin-0.0.80/durin/io/runnable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9042 2023-05-22 11:52:35.000000 durin-0.0.80/durin/io/schema.capnp
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7102 2023-05-22 11:52:35.000000 durin-0.0.80/durin/sensor.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14773 2023-05-22 11:52:35.000000 durin-0.0.80/durin/ui.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 11:52:44.424178 durin-0.0.80/durin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2929 2023-05-22 11:52:44.000000 durin-0.0.80/durin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-05-22 11:52:44.000000 durin-0.0.80/durin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 11:52:44.000000 durin-0.0.80/durin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-22 11:52:44.000000 durin-0.0.80/durin.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-22 11:52:44.000000 durin-0.0.80/durin.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 11:52:44.428178 durin-0.0.80/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)      663 2023-05-22 11:52:35.000000 durin-0.0.80/setup.py
```

### Comparing `durin-0.0.79/PKG-INFO` & `durin-0.0.80/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: durin
-Version: 0.0.79
+Version: 0.0.80
 Summary: Python control interface for the Durin robot
 Maintainer: Jens E. Pedersen
 Maintainer-email: jeped@kth.se
 License: LGPLv3
 Description-Content-Type: text/markdown
 Provides-Extra: aestream
```

### Comparing `durin-0.0.79/README.md` & `durin-0.0.80/README.md`

 * *Files identical despite different names*

### Comparing `durin-0.0.79/durin/actuator.py` & `durin-0.0.80/durin/actuator.py`

 * *Files identical despite different names*

### Comparing `durin-0.0.79/durin/cli.py` & `durin-0.0.80/durin/cli.py`

 * *Files identical despite different names*

### Comparing `durin-0.0.79/durin/controller/server.py` & `durin-0.0.80/durin/controller/server.py`

 * *Files identical despite different names*

### Comparing `durin-0.0.79/durin/controller/test/test_stream.py` & `durin-0.0.80/durin/controller/test/test_stream.py`

 * *Files identical despite different names*

### Comparing `durin-0.0.79/durin/durin.py` & `durin-0.0.80/durin/durin.py`

 * *Files identical despite different names*

### Comparing `durin-0.0.79/durin/durin_birdseye.jpg` & `durin-0.0.80/durin/durin_birdseye.jpg`

 * *Files identical despite different names*

### Comparing `durin-0.0.79/durin/examples/braitenberg.py` & `durin-0.0.80/durin/examples/braitenberg.py`

 * *Files identical despite different names*

### Comparing `durin-0.0.79/durin/examples/commands.py` & `durin-0.0.80/durin/examples/commands.py`

 * *Files identical despite different names*

### Comparing `durin-0.0.79/durin/examples/dashboard.py` & `durin-0.0.80/durin/examples/dashboard.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,21 +4,15 @@
 
 
 if __name__ == "__main__":
 
     # We start a connectioen to the robot
     # and can now read from and write to the robot via the variable "durin"
     # Notice the UI class, which differs from the (more efficient) standalone Durin interface
-    # the debug flag enables/disables some ugly data on the dashboard
-    if len(sys.argv) == 2:
-        debug = (sys.argv[1] == "debug")
-    else:
-        debug = False
-
-    with DurinUI("durin1.local", debug=debug) as durin:
+    with DurinUI("durin1.local") as durin:
         # Loop until the user quits
         is_running = True
         durin(GetSystemInfo())  # Ask to get IP address, MAC address and Durin ID
         gotSystemInfo = False
 
         while not gotSystemInfo:
             """ Wait until IP address, MAC address, and Durin ID are read"""
```

### Comparing `durin-0.0.79/durin/examples/main.py` & `durin-0.0.80/durin/examples/main.py`

 * *Files identical despite different names*

### Comparing `durin-0.0.79/durin/examples/plot.py` & `durin-0.0.80/durin/examples/plot.py`

 * *Files identical despite different names*

### Comparing `durin-0.0.79/durin/examples/record.py` & `durin-0.0.80/durin/examples/record.py`

 * *Files identical despite different names*

### Comparing `durin-0.0.79/durin/examples/stats.py` & `durin-0.0.80/durin/examples/stats.py`

 * *Files identical despite different names*

### Comparing `durin-0.0.79/durin/io/__init__.py` & `durin-0.0.80/durin/io/__init__.py`

 * *Files identical despite different names*

### Comparing `durin-0.0.79/durin/io/command.py` & `durin-0.0.80/durin/io/command.py`

 * *Files identical despite different names*

### Comparing `durin-0.0.79/durin/io/gamepad.py` & `durin-0.0.80/durin/io/gamepad.py`

 * *Files identical despite different names*

### Comparing `durin-0.0.79/durin/io/network.py` & `durin-0.0.80/durin/io/network.py`

 * *Files identical despite different names*

### Comparing `durin-0.0.79/durin/io/ringbuffer.py` & `durin-0.0.80/durin/io/ringbuffer.py`

 * *Files identical despite different names*

### Comparing `durin-0.0.79/durin/io/runnable.py` & `durin-0.0.80/durin/io/runnable.py`

 * *Files identical despite different names*

### Comparing `durin-0.0.79/durin/io/schema.capnp` & `durin-0.0.80/durin/io/schema.capnp`

 * *Files identical despite different names*

### Comparing `durin-0.0.79/durin/sensor.py` & `durin-0.0.80/durin/sensor.py`

 * *Files identical despite different names*

### Comparing `durin-0.0.79/durin/ui.py` & `durin-0.0.80/durin/ui.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,21 +56,21 @@
 UWB_PLACEMENT = (x, 0.1+29*d)              # Upper left corner
 
 TOF_STATUS_PLACEMENT = (x, 0.1+25*d)
 
 
 class DurinUI(Durin):
     def __init__(self, *args, **kwargs):
-        self.debug = kwargs.pop("debug", False)
         super().__init__(*args, **kwargs)
         self.gamepad = Gamepad()
 
         self.ip = None
         self.mac = None
         self.id = None
+        self.debug = False
 
         self.vertical = 0
         self.horizontal = 0
         self.tau = 0.9999
         self.rot = 0
 
     def __enter__(self):
@@ -153,14 +153,16 @@
                     self.horizontal = -500
                 elif event.key == pygame.K_RIGHT or event.key == pygame.K_d:
                     self.horizontal = 500
                 elif event.key == pygame.K_q:
                     self.rot = 500
                 elif event.key == pygame.K_e:
                     self.rot = -500
+                elif event.key == pygame.K_g:
+                    self.debug = not self.debug
 
             elif event.type == pygame.KEYUP:
                 # Key released
                 if event.key == pygame.K_UP or event.key == pygame.K_w or event.key == pygame.K_DOWN or event.key == pygame.K_s:
                     self.vertical = 0
                 if event.key == pygame.K_LEFT or event.key == pygame.K_d or event.key == pygame.K_RIGHT or event.key == pygame.K_a:
                     self.horizontal = 0
@@ -185,14 +187,15 @@
         tofs = (np.tanh((obs.tof / 1000)) * 255).astype(np.int32)
 
         # Rotated surfaces
         rotated_surfaces = []
 
         for o in range(len(self.surfaces)):
             surface = self.surfaces[o]
+            surface.fill((0, 0, 0, 0))
             square_size = math.ceil(min(surface_width, surface_height) / 8)
             for i in range(8):
                 for j in range(8):
                     left = i * square_size
                     top = j * square_size
                     square_rect = pygame.Rect(left, top, square_size, square_size)
                     color_value = tofs[o][i][j]
@@ -245,15 +248,15 @@
                 self.render_text(str(imu[type][xyz]), (IMU_PLACEMENT[0]+(xyz+1)*3*d, IMU_PLACEMENT[1]+(type+1)*d))
 
         # Update ToF status ###################
         summed_status = [0] * 8
         for i in range(8):
             tot = 0
             for v in obs.tof_status[i].flat:
-                if v != 0 and v != 3:
+                if v != 0:
                     tot += 1
             summed_status[i] = tot
 
         self.render_text(f"ToF: reported faulty pixels", (TOF_STATUS_PLACEMENT[0], TOF_STATUS_PLACEMENT[1]), "o")
         self.render_text(f"0: {summed_status[0]}", (TOF_STATUS_PLACEMENT[0] + 0 * d * 2, TOF_STATUS_PLACEMENT[1] + d))
         self.render_text(f"1: {summed_status[1]}", (TOF_STATUS_PLACEMENT[0] + 1 * d * 2, TOF_STATUS_PLACEMENT[1] + d))
         self.render_text(f"2: {summed_status[2]}", (TOF_STATUS_PLACEMENT[0] + 2 * d * 2, TOF_STATUS_PLACEMENT[1] + d))
```

### Comparing `durin-0.0.79/durin.egg-info/PKG-INFO` & `durin-0.0.80/durin.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: durin
-Version: 0.0.79
+Version: 0.0.80
 Summary: Python control interface for the Durin robot
 Maintainer: Jens E. Pedersen
 Maintainer-email: jeped@kth.se
 License: LGPLv3
 Description-Content-Type: text/markdown
 Provides-Extra: aestream
```

### Comparing `durin-0.0.79/durin.egg-info/SOURCES.txt` & `durin-0.0.80/durin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `durin-0.0.79/setup.py` & `durin-0.0.80/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     requirements = fp.read().split("\n")
 
 with open("README.md", "r") as fp:
     long_description = fp.read()
 
 setup(
     name="durin",
-    version="0.0.79",
+    version="0.0.80",
     install_requires=requirements,
     packages=find_packages(),
     license="LGPLv3",
     maintainer="Jens E. Pedersen",
     maintainer_email="jeped@kth.se",
     extras_require={"aestream": ["aestream"]},
     scripts=["bin/durin"],
```

