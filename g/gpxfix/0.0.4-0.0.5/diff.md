# Comparing `tmp/gpxfix-0.0.4.tar.gz` & `tmp/gpxfix-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpxfix-0.0.4.tar", last modified: Sun Oct 30 11:25:20 2022, max compression
+gzip compressed data, was "gpxfix-0.0.5.tar", last modified: Mon May 22 06:22:57 2023, max compression
```

## Comparing `gpxfix-0.0.4.tar` & `gpxfix-0.0.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 11:25:20.223742 gpxfix-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (121)     1050 2022-10-30 11:25:11.000000 gpxfix-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     4664 2022-10-30 11:25:20.223742 gpxfix-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4056 2022-10-30 11:25:11.000000 gpxfix-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 11:25:20.223742 gpxfix-0.0.4/bin/
--rw-r--r--   0 runner    (1001) docker     (121)       48 2022-10-30 11:25:11.000000 gpxfix-0.0.4/bin/gpxfix
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 11:25:20.223742 gpxfix-0.0.4/gpxfix/
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-10-30 11:25:11.000000 gpxfix-0.0.4/gpxfix/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    26025 2022-10-30 11:25:11.000000 gpxfix-0.0.4/gpxfix/main.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 11:25:20.223742 gpxfix-0.0.4/gpxfix.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4664 2022-10-30 11:25:20.000000 gpxfix-0.0.4/gpxfix.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      220 2022-10-30 11:25:20.000000 gpxfix-0.0.4/gpxfix.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-30 11:25:20.000000 gpxfix-0.0.4/gpxfix.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       30 2022-10-30 11:25:20.000000 gpxfix-0.0.4/gpxfix.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        7 2022-10-30 11:25:20.000000 gpxfix-0.0.4/gpxfix.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-10-30 11:25:20.223742 gpxfix-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1517 2022-10-30 11:25:11.000000 gpxfix-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 06:22:57.809618 gpxfix-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (122)     1050 2023-05-22 06:22:38.000000 gpxfix-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)     4664 2023-05-22 06:22:57.809618 gpxfix-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     4056 2023-05-22 06:22:38.000000 gpxfix-0.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 06:22:57.805618 gpxfix-0.0.5/bin/
+-rw-r--r--   0 runner    (1001) docker     (122)       48 2023-05-22 06:22:38.000000 gpxfix-0.0.5/bin/gpxfix
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 06:22:57.805618 gpxfix-0.0.5/gpxfix/
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-22 06:22:38.000000 gpxfix-0.0.5/gpxfix/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    26021 2023-05-22 06:22:38.000000 gpxfix-0.0.5/gpxfix/main.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 06:22:57.805618 gpxfix-0.0.5/gpxfix.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     4664 2023-05-22 06:22:57.000000 gpxfix-0.0.5/gpxfix.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      220 2023-05-22 06:22:57.000000 gpxfix-0.0.5/gpxfix.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-22 06:22:57.000000 gpxfix-0.0.5/gpxfix.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       30 2023-05-22 06:22:57.000000 gpxfix-0.0.5/gpxfix.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        7 2023-05-22 06:22:57.000000 gpxfix-0.0.5/gpxfix.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-22 06:22:57.809618 gpxfix-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1517 2023-05-22 06:22:38.000000 gpxfix-0.0.5/setup.py
```

### Comparing `gpxfix-0.0.4/LICENSE` & `gpxfix-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `gpxfix-0.0.4/PKG-INFO` & `gpxfix-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpxfix
-Version: 0.0.4
+Version: 0.0.5
 Summary: gpxfix: GUI to fix .gpx tracks with missing sections
 Home-page: https://github.com/jannisborn/gpxfix
 Author: Jannis Born
 Author-email: jannis.born@gmx.de
 License: MIT
 Keywords: GPX,Tracking,Sports,Running,Cycling,Strava
 Classifier: Intended Audience :: Developers
```

### Comparing `gpxfix-0.0.4/README.md` & `gpxfix-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `gpxfix-0.0.4/gpxfix/main.py` & `gpxfix-0.0.5/gpxfix/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -496,15 +496,15 @@
             gpx_extension = ElementTree.fromstring(extension_string)
             trackpoint.extensions.append(gpx_extension)
             gpx_segment.points.append(trackpoint)
 
         # Compute cumulative time needed for the snippet (in seconds)
         if thresh != len(dataOld) and thresh != 0:  # Regular case
             cum_Time = (
-                self.gpx["main"]["parsed"].tracks[0].segments[0].points[thresh + 1].time
+                self.gpx["main"]["parsed"].tracks[0].segments[0].points[thresh].time
                 - gpx_segment.points[-1].time
             ).total_seconds()
 
             # Compute cumulative (pointwise) distance of GPX track and compare to GoogleMaps
             dataNew.append(
                 gpx_segment.points[-1]
             )  # To be able to compute distance for first point
```

### Comparing `gpxfix-0.0.4/gpxfix.egg-info/PKG-INFO` & `gpxfix-0.0.5/gpxfix.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpxfix
-Version: 0.0.4
+Version: 0.0.5
 Summary: gpxfix: GUI to fix .gpx tracks with missing sections
 Home-page: https://github.com/jannisborn/gpxfix
 Author: Jannis Born
 Author-email: jannis.born@gmx.de
 License: MIT
 Keywords: GPX,Tracking,Sports,Running,Cycling,Strava
 Classifier: Intended Audience :: Developers
```

### Comparing `gpxfix-0.0.4/setup.py` & `gpxfix-0.0.5/setup.py`

 * *Files identical despite different names*

