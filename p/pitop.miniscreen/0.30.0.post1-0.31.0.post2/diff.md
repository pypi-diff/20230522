# Comparing `tmp/pitop.miniscreen-0.30.0.post1.tar.gz` & `tmp/pitop.miniscreen-0.31.0.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pitop.miniscreen-0.30.0.post1.tar", last modified: Fri Dec 16 14:08:29 2022, max compression
+gzip compressed data, was "dist/pitop.miniscreen-0.31.0.post2.tar", last modified: Mon May 22 19:13:12 2023, max compression
```

## Comparing `pitop.miniscreen-0.30.0.post1.tar` & `pitop.miniscreen-0.31.0.post2.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-16 14:08:29.000000 pitop.miniscreen-0.30.0.post1/
--rw-r--r--   0 runner    (1001) docker     (122)       38 2022-12-16 14:07:48.000000 pitop.miniscreen-0.30.0.post1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)      966 2022-12-16 14:08:29.000000 pitop.miniscreen-0.30.0.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      128 2022-12-16 14:07:48.000000 pitop.miniscreen-0.30.0.post1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-16 14:08:29.000000 pitop.miniscreen-0.30.0.post1/pitop/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-16 14:08:29.000000 pitop.miniscreen-0.30.0.post1/pitop/miniscreen/
--rw-r--r--   0 runner    (1001) docker     (122)       35 2022-12-16 14:07:48.000000 pitop.miniscreen-0.30.0.post1/pitop/miniscreen/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-16 14:08:29.000000 pitop.miniscreen-0.30.0.post1/pitop/miniscreen/buttons/
--rw-r--r--   0 runner    (1001) docker     (122)       92 2022-12-16 14:07:48.000000 pitop.miniscreen-0.30.0.post1/pitop/miniscreen/buttons/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4448 2022-12-16 14:07:48.000000 pitop.miniscreen-0.30.0.post1/pitop/miniscreen/buttons/buttons.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-16 14:08:29.000000 pitop.miniscreen-0.30.0.post1/pitop/miniscreen/images/
--rw-r--r--   0 runner    (1001) docker     (122)    80224 2022-12-16 14:07:48.000000 pitop.miniscreen-0.30.0.post1/pitop/miniscreen/images/rocket.gif
--rw-r--r--   0 runner    (1001) docker     (122)     5895 2022-12-16 14:07:48.000000 pitop.miniscreen-0.30.0.post1/pitop/miniscreen/miniscreen.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-16 14:08:29.000000 pitop.miniscreen-0.30.0.post1/pitop/miniscreen/oled/
--rw-r--r--   0 runner    (1001) docker     (122)       23 2022-12-16 14:07:48.000000 pitop.miniscreen-0.30.0.post1/pitop/miniscreen/oled/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7871 2022-12-16 14:07:48.000000 pitop.miniscreen-0.30.0.post1/pitop/miniscreen/oled/assistant.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-16 14:08:29.000000 pitop.miniscreen-0.30.0.post1/pitop/miniscreen/oled/core/
--rw-r--r--   0 runner    (1001) docker     (122)      137 2022-12-16 14:07:48.000000 pitop.miniscreen-0.30.0.post1/pitop/miniscreen/oled/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    15619 2022-12-16 14:07:48.000000 pitop.miniscreen-0.30.0.post1/pitop/miniscreen/oled/core/canvas.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-16 14:08:29.000000 pitop.miniscreen-0.30.0.post1/pitop/miniscreen/oled/core/contrib/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-16 14:07:48.000000 pitop.miniscreen-0.30.0.post1/pitop/miniscreen/oled/core/contrib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-16 14:08:29.000000 pitop.miniscreen-0.30.0.post1/pitop/miniscreen/oled/core/contrib/luma/
--rw-r--r--   0 runner    (1001) docker     (122)     1123 2022-12-16 14:07:48.000000 pitop.miniscreen-0.30.0.post1/pitop/miniscreen/oled/core/contrib/luma/LICENSE.rst
--rw-r--r--   0 runner    (1001) docker     (122)      165 2022-12-16 14:07:48.000000 pitop.miniscreen-0.30.0.post1/pitop/miniscreen/oled/core/contrib/luma/README.md
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-16 14:07:48.000000 pitop.miniscreen-0.30.0.post1/pitop/miniscreen/oled/core/contrib/luma/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-16 14:08:29.000000 pitop.miniscreen-0.30.0.post1/pitop/miniscreen/oled/core/contrib/luma/core/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-16 14:07:48.000000 pitop.miniscreen-0.30.0.post1/pitop/miniscreen/oled/core/contrib/luma/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      237 2022-12-16 14:07:48.000000 pitop.miniscreen-0.30.0.post1/pitop/miniscreen/oled/core/contrib/luma/core/const.py
--rw-r--r--   0 runner    (1001) docker     (122)     2641 2022-12-16 14:07:48.000000 pitop.miniscreen-0.30.0.post1/pitop/miniscreen/oled/core/contrib/luma/core/device.py
--rw-r--r--   0 runner    (1001) docker     (122)      640 2022-12-16 14:07:48.000000 pitop.miniscreen-0.30.0.post1/pitop/miniscreen/oled/core/contrib/luma/core/error.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-16 14:08:29.000000 pitop.miniscreen-0.30.0.post1/pitop/miniscreen/oled/core/contrib/luma/core/interface/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-16 14:07:48.000000 pitop.miniscreen-0.30.0.post1/pitop/miniscreen/oled/core/contrib/luma/core/interface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7434 2022-12-16 14:07:48.000000 pitop.miniscreen-0.30.0.post1/pitop/miniscreen/oled/core/contrib/luma/core/interface/serial.py
--rw-r--r--   0 runner    (1001) docker     (122)     2407 2022-12-16 14:07:48.000000 pitop.miniscreen-0.30.0.post1/pitop/miniscreen/oled/core/contrib/luma/core/mixin.py
--rw-r--r--   0 runner    (1001) docker     (122)     1258 2022-12-16 14:07:48.000000 pitop.miniscreen-0.30.0.post1/pitop/miniscreen/oled/core/contrib/luma/core/threadpool.py
--rw-r--r--   0 runner    (1001) docker     (122)     7044 2022-12-16 14:07:48.000000 pitop.miniscreen-0.30.0.post1/pitop/miniscreen/oled/core/contrib/luma/core/virtual.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-16 14:08:29.000000 pitop.miniscreen-0.30.0.post1/pitop/miniscreen/oled/core/contrib/luma/oled/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-16 14:07:48.000000 pitop.miniscreen-0.30.0.post1/pitop/miniscreen/oled/core/contrib/luma/oled/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      498 2022-12-16 14:07:48.000000 pitop.miniscreen-0.30.0.post1/pitop/miniscreen/oled/core/contrib/luma/oled/const.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-16 14:08:29.000000 pitop.miniscreen-0.30.0.post1/pitop/miniscreen/oled/core/contrib/luma/oled/device/
--rw-r--r--   0 runner    (1001) docker     (122)     3432 2022-12-16 14:07:48.000000 pitop.miniscreen-0.30.0.post1/pitop/miniscreen/oled/core/contrib/luma/oled/device/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3980 2022-12-16 14:07:48.000000 pitop.miniscreen-0.30.0.post1/pitop/miniscreen/oled/core/device_controller.py
--rw-r--r--   0 runner    (1001) docker     (122)     3387 2022-12-16 14:07:48.000000 pitop.miniscreen-0.30.0.post1/pitop/miniscreen/oled/core/fps_regulator.py
--rw-r--r--   0 runner    (1001) docker     (122)     1508 2022-12-16 14:07:48.000000 pitop.miniscreen-0.30.0.post1/pitop/miniscreen/oled/core/lock.py
--rw-r--r--   0 runner    (1001) docker     (122)    22476 2022-12-16 14:07:48.000000 pitop.miniscreen-0.30.0.post1/pitop/miniscreen/oled/oled.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-16 14:08:29.000000 pitop.miniscreen-0.30.0.post1/pitop.miniscreen.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      966 2022-12-16 14:08:29.000000 pitop.miniscreen-0.30.0.post1/pitop.miniscreen.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1597 2022-12-16 14:08:29.000000 pitop.miniscreen-0.30.0.post1/pitop.miniscreen.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-12-16 14:08:29.000000 pitop.miniscreen-0.30.0.post1/pitop.miniscreen.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      145 2022-12-16 14:08:29.000000 pitop.miniscreen-0.30.0.post1/pitop.miniscreen.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        6 2022-12-16 14:08:29.000000 pitop.miniscreen-0.30.0.post1/pitop.miniscreen.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2022-12-16 14:08:29.000000 pitop.miniscreen-0.30.0.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     2111 2022-12-16 14:07:48.000000 pitop.miniscreen-0.30.0.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 19:13:12.000000 pitop.miniscreen-0.31.0.post2/
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-22 19:12:55.000000 pitop.miniscreen-0.31.0.post2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)      966 2023-05-22 19:13:12.000000 pitop.miniscreen-0.31.0.post2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      128 2023-05-22 19:12:55.000000 pitop.miniscreen-0.31.0.post2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 19:13:12.000000 pitop.miniscreen-0.31.0.post2/pitop/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 19:13:12.000000 pitop.miniscreen-0.31.0.post2/pitop/miniscreen/
+-rw-r--r--   0 runner    (1001) docker     (122)       35 2023-05-22 19:12:55.000000 pitop.miniscreen-0.31.0.post2/pitop/miniscreen/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 19:13:12.000000 pitop.miniscreen-0.31.0.post2/pitop/miniscreen/buttons/
+-rw-r--r--   0 runner    (1001) docker     (122)       92 2023-05-22 19:12:55.000000 pitop.miniscreen-0.31.0.post2/pitop/miniscreen/buttons/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4448 2023-05-22 19:12:55.000000 pitop.miniscreen-0.31.0.post2/pitop/miniscreen/buttons/buttons.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 19:13:12.000000 pitop.miniscreen-0.31.0.post2/pitop/miniscreen/images/
+-rw-r--r--   0 runner    (1001) docker     (122)    80224 2023-05-22 19:12:55.000000 pitop.miniscreen-0.31.0.post2/pitop/miniscreen/images/rocket.gif
+-rw-r--r--   0 runner    (1001) docker     (122)     5895 2023-05-22 19:12:55.000000 pitop.miniscreen-0.31.0.post2/pitop/miniscreen/miniscreen.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 19:13:12.000000 pitop.miniscreen-0.31.0.post2/pitop/miniscreen/oled/
+-rw-r--r--   0 runner    (1001) docker     (122)       23 2023-05-22 19:12:55.000000 pitop.miniscreen-0.31.0.post2/pitop/miniscreen/oled/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7871 2023-05-22 19:12:55.000000 pitop.miniscreen-0.31.0.post2/pitop/miniscreen/oled/assistant.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 19:13:12.000000 pitop.miniscreen-0.31.0.post2/pitop/miniscreen/oled/core/
+-rw-r--r--   0 runner    (1001) docker     (122)      137 2023-05-22 19:12:55.000000 pitop.miniscreen-0.31.0.post2/pitop/miniscreen/oled/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15619 2023-05-22 19:12:55.000000 pitop.miniscreen-0.31.0.post2/pitop/miniscreen/oled/core/canvas.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 19:13:12.000000 pitop.miniscreen-0.31.0.post2/pitop/miniscreen/oled/core/contrib/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-22 19:12:55.000000 pitop.miniscreen-0.31.0.post2/pitop/miniscreen/oled/core/contrib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 19:13:12.000000 pitop.miniscreen-0.31.0.post2/pitop/miniscreen/oled/core/contrib/luma/
+-rw-r--r--   0 runner    (1001) docker     (122)     1123 2023-05-22 19:12:55.000000 pitop.miniscreen-0.31.0.post2/pitop/miniscreen/oled/core/contrib/luma/LICENSE.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      165 2023-05-22 19:12:55.000000 pitop.miniscreen-0.31.0.post2/pitop/miniscreen/oled/core/contrib/luma/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-22 19:12:55.000000 pitop.miniscreen-0.31.0.post2/pitop/miniscreen/oled/core/contrib/luma/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 19:13:12.000000 pitop.miniscreen-0.31.0.post2/pitop/miniscreen/oled/core/contrib/luma/core/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-22 19:12:55.000000 pitop.miniscreen-0.31.0.post2/pitop/miniscreen/oled/core/contrib/luma/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      237 2023-05-22 19:12:55.000000 pitop.miniscreen-0.31.0.post2/pitop/miniscreen/oled/core/contrib/luma/core/const.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2641 2023-05-22 19:12:55.000000 pitop.miniscreen-0.31.0.post2/pitop/miniscreen/oled/core/contrib/luma/core/device.py
+-rw-r--r--   0 runner    (1001) docker     (122)      640 2023-05-22 19:12:55.000000 pitop.miniscreen-0.31.0.post2/pitop/miniscreen/oled/core/contrib/luma/core/error.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 19:13:12.000000 pitop.miniscreen-0.31.0.post2/pitop/miniscreen/oled/core/contrib/luma/core/interface/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-22 19:12:55.000000 pitop.miniscreen-0.31.0.post2/pitop/miniscreen/oled/core/contrib/luma/core/interface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7433 2023-05-22 19:12:55.000000 pitop.miniscreen-0.31.0.post2/pitop/miniscreen/oled/core/contrib/luma/core/interface/serial.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2407 2023-05-22 19:12:55.000000 pitop.miniscreen-0.31.0.post2/pitop/miniscreen/oled/core/contrib/luma/core/mixin.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1258 2023-05-22 19:12:55.000000 pitop.miniscreen-0.31.0.post2/pitop/miniscreen/oled/core/contrib/luma/core/threadpool.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7044 2023-05-22 19:12:55.000000 pitop.miniscreen-0.31.0.post2/pitop/miniscreen/oled/core/contrib/luma/core/virtual.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 19:13:12.000000 pitop.miniscreen-0.31.0.post2/pitop/miniscreen/oled/core/contrib/luma/oled/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-22 19:12:55.000000 pitop.miniscreen-0.31.0.post2/pitop/miniscreen/oled/core/contrib/luma/oled/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      498 2023-05-22 19:12:55.000000 pitop.miniscreen-0.31.0.post2/pitop/miniscreen/oled/core/contrib/luma/oled/const.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 19:13:12.000000 pitop.miniscreen-0.31.0.post2/pitop/miniscreen/oled/core/contrib/luma/oled/device/
+-rw-r--r--   0 runner    (1001) docker     (122)     3432 2023-05-22 19:12:55.000000 pitop.miniscreen-0.31.0.post2/pitop/miniscreen/oled/core/contrib/luma/oled/device/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3980 2023-05-22 19:12:55.000000 pitop.miniscreen-0.31.0.post2/pitop/miniscreen/oled/core/device_controller.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3387 2023-05-22 19:12:55.000000 pitop.miniscreen-0.31.0.post2/pitop/miniscreen/oled/core/fps_regulator.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1508 2023-05-22 19:12:55.000000 pitop.miniscreen-0.31.0.post2/pitop/miniscreen/oled/core/lock.py
+-rw-r--r--   0 runner    (1001) docker     (122)    22475 2023-05-22 19:12:55.000000 pitop.miniscreen-0.31.0.post2/pitop/miniscreen/oled/oled.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 19:13:12.000000 pitop.miniscreen-0.31.0.post2/pitop.miniscreen.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      966 2023-05-22 19:13:12.000000 pitop.miniscreen-0.31.0.post2/pitop.miniscreen.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1597 2023-05-22 19:13:12.000000 pitop.miniscreen-0.31.0.post2/pitop.miniscreen.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-22 19:13:12.000000 pitop.miniscreen-0.31.0.post2/pitop.miniscreen.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      145 2023-05-22 19:13:12.000000 pitop.miniscreen-0.31.0.post2/pitop.miniscreen.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        6 2023-05-22 19:13:12.000000 pitop.miniscreen-0.31.0.post2/pitop.miniscreen.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-22 19:13:12.000000 pitop.miniscreen-0.31.0.post2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     2111 2023-05-22 19:12:55.000000 pitop.miniscreen-0.31.0.post2/setup.py
```

### Comparing `pitop.miniscreen-0.30.0.post1/PKG-INFO` & `pitop.miniscreen-0.31.0.post2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: pitop.miniscreen
-Version: 0.30.0.post1
+Version: 0.31.0.post2
 Summary: pi-top Python SDK.
 Home-page: https://github.com/pi-top/pi-top-Python-SDK
 Author: pi-top
 Author-email: deb-maintainers@pi-top.com
 License: Apache Software License
 Description: ===========================
         pi-top Python Miniscreen
```

### Comparing `pitop.miniscreen-0.30.0.post1/pitop/miniscreen/buttons/buttons.py` & `pitop.miniscreen-0.31.0.post2/pitop/miniscreen/buttons/buttons.py`

 * *Files identical despite different names*

### Comparing `pitop.miniscreen-0.30.0.post1/pitop/miniscreen/images/rocket.gif` & `pitop.miniscreen-0.31.0.post2/pitop/miniscreen/images/rocket.gif`

 * *Files identical despite different names*

### Comparing `pitop.miniscreen-0.30.0.post1/pitop/miniscreen/miniscreen.py` & `pitop.miniscreen-0.31.0.post2/pitop/miniscreen/miniscreen.py`

 * *Files identical despite different names*

### Comparing `pitop.miniscreen-0.30.0.post1/pitop/miniscreen/oled/assistant.py` & `pitop.miniscreen-0.31.0.post2/pitop/miniscreen/oled/assistant.py`

 * *Files identical despite different names*

### Comparing `pitop.miniscreen-0.30.0.post1/pitop/miniscreen/oled/core/canvas.py` & `pitop.miniscreen-0.31.0.post2/pitop/miniscreen/oled/core/canvas.py`

 * *Files identical despite different names*

### Comparing `pitop.miniscreen-0.30.0.post1/pitop/miniscreen/oled/core/contrib/luma/LICENSE.rst` & `pitop.miniscreen-0.31.0.post2/pitop/miniscreen/oled/core/contrib/luma/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `pitop.miniscreen-0.30.0.post1/pitop/miniscreen/oled/core/contrib/luma/core/device.py` & `pitop.miniscreen-0.31.0.post2/pitop/miniscreen/oled/core/contrib/luma/core/device.py`

 * *Files identical despite different names*

### Comparing `pitop.miniscreen-0.30.0.post1/pitop/miniscreen/oled/core/contrib/luma/core/error.py` & `pitop.miniscreen-0.31.0.post2/pitop/miniscreen/oled/core/contrib/luma/core/error.py`

 * *Files identical despite different names*

### Comparing `pitop.miniscreen-0.30.0.post1/pitop/miniscreen/oled/core/contrib/luma/core/interface/serial.py` & `pitop.miniscreen-0.31.0.post2/pitop/miniscreen/oled/core/contrib/luma/core/interface/serial.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,15 +44,14 @@
     :param RST: The GPIO pin to connect reset (RES / RST) to.
     :type RST: int
     """
 
     def __init__(
         self, transfer_size=4096, reset_hold_time=0, reset_release_time=0, **kwargs
     ):
-
         self._transfer_size = transfer_size
 
         self._SCLK = self._configure(kwargs.get("SCLK"))
         self._SDA = self._configure(kwargs.get("SDA"))
         self._CE = self._configure(kwargs.get("CE"))
         self._DC = self._configure(kwargs.get("DC"))
         self._RST = self._configure(kwargs.get("RST"))
```

### Comparing `pitop.miniscreen-0.30.0.post1/pitop/miniscreen/oled/core/contrib/luma/core/mixin.py` & `pitop.miniscreen-0.31.0.post2/pitop/miniscreen/oled/core/contrib/luma/core/mixin.py`

 * *Files identical despite different names*

### Comparing `pitop.miniscreen-0.30.0.post1/pitop/miniscreen/oled/core/contrib/luma/core/threadpool.py` & `pitop.miniscreen-0.31.0.post2/pitop/miniscreen/oled/core/contrib/luma/core/threadpool.py`

 * *Files identical despite different names*

### Comparing `pitop.miniscreen-0.30.0.post1/pitop/miniscreen/oled/core/contrib/luma/core/virtual.py` & `pitop.miniscreen-0.31.0.post2/pitop/miniscreen/oled/core/contrib/luma/core/virtual.py`

 * *Files identical despite different names*

### Comparing `pitop.miniscreen-0.30.0.post1/pitop/miniscreen/oled/core/contrib/luma/oled/device/__init__.py` & `pitop.miniscreen-0.31.0.post2/pitop/miniscreen/oled/core/contrib/luma/oled/device/__init__.py`

 * *Files identical despite different names*

### Comparing `pitop.miniscreen-0.30.0.post1/pitop/miniscreen/oled/core/device_controller.py` & `pitop.miniscreen-0.31.0.post2/pitop/miniscreen/oled/core/device_controller.py`

 * *Files identical despite different names*

### Comparing `pitop.miniscreen-0.30.0.post1/pitop/miniscreen/oled/core/fps_regulator.py` & `pitop.miniscreen-0.31.0.post2/pitop/miniscreen/oled/core/fps_regulator.py`

 * *Files identical despite different names*

### Comparing `pitop.miniscreen-0.30.0.post1/pitop/miniscreen/oled/core/lock.py` & `pitop.miniscreen-0.31.0.post2/pitop/miniscreen/oled/core/lock.py`

 * *Files identical despite different names*

### Comparing `pitop.miniscreen-0.30.0.post1/pitop/miniscreen/oled/oled.py` & `pitop.miniscreen-0.31.0.post2/pitop/miniscreen/oled/oled.py`

 * *Files 0% similar despite different names*

```diff
@@ -542,15 +542,14 @@
 
     ####################
     # Internal support #
     ####################
     def __auto_play(self, image, loop=False):
         while True:
             for frame in self.assistant.get_frame_iterator(image):
-
                 if self.__kill_thread:
                     break
 
                 self.display_image(frame)
                 # Wait for animated image's frame length
                 sleep(float(frame.info["duration"] / 1000))  # ms to s
```

### Comparing `pitop.miniscreen-0.30.0.post1/pitop.miniscreen.egg-info/PKG-INFO` & `pitop.miniscreen-0.31.0.post2/pitop.miniscreen.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: pitop.miniscreen
-Version: 0.30.0.post1
+Version: 0.31.0.post2
 Summary: pi-top Python SDK.
 Home-page: https://github.com/pi-top/pi-top-Python-SDK
 Author: pi-top
 Author-email: deb-maintainers@pi-top.com
 License: Apache Software License
 Description: ===========================
         pi-top Python Miniscreen
```

### Comparing `pitop.miniscreen-0.30.0.post1/pitop.miniscreen.egg-info/SOURCES.txt` & `pitop.miniscreen-0.31.0.post2/pitop.miniscreen.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pitop.miniscreen-0.30.0.post1/setup.py` & `pitop.miniscreen-0.31.0.post2/setup.py`

 * *Files identical despite different names*

