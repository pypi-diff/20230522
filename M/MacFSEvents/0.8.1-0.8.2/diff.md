# Comparing `tmp/MacFSEvents-0.8.1.tar.gz` & `tmp/MacFSEvents-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/MacFSEvents-0.8.1.tar", last modified: Wed Feb 21 11:40:44 2018, max compression
+gzip compressed data, was "MacFSEvents-0.8.2.tar", last modified: Mon May 22 20:16:14 2023, max compression
```

## Comparing `MacFSEvents-0.8.1.tar` & `MacFSEvents-0.8.2.tar`

### file list

```diff
@@ -1,20 +1,15 @@
-drwxr-xr-x   0 mborch     (501) staff       (20)        0 2018-02-21 11:40:44.000000 MacFSEvents-0.8.1/
--rw-r--r--   0 mborch     (501) staff       (20)       35 2017-10-23 06:47:33.000000 MacFSEvents-0.8.1/.gitignore
--rw-r--r--   0 mborch     (501) staff       (20)      270 2017-10-23 06:47:33.000000 MacFSEvents-0.8.1/.travis.yml
--rw-r--r--   0 mborch     (501) staff       (20)     2219 2018-02-21 11:40:23.000000 MacFSEvents-0.8.1/CHANGES.rst
--rw-r--r--   0 mborch     (501) staff       (20)     1287 2017-10-23 08:23:59.000000 MacFSEvents-0.8.1/LICENSE.txt
-drwxr-xr-x   0 mborch     (501) staff       (20)        0 2018-02-21 11:40:44.000000 MacFSEvents-0.8.1/MacFSEvents.egg-info/
--rw-r--r--   0 mborch     (501) staff       (20)    10071 2018-02-21 11:40:43.000000 MacFSEvents-0.8.1/MacFSEvents.egg-info/PKG-INFO
--rw-r--r--   0 mborch     (501) staff       (20)      291 2018-02-21 11:40:43.000000 MacFSEvents-0.8.1/MacFSEvents.egg-info/SOURCES.txt
--rw-r--r--   0 mborch     (501) staff       (20)        1 2018-02-21 11:40:43.000000 MacFSEvents-0.8.1/MacFSEvents.egg-info/dependency_links.txt
--rw-r--r--   0 mborch     (501) staff       (20)        1 2017-10-23 06:47:39.000000 MacFSEvents-0.8.1/MacFSEvents.egg-info/not-zip-safe
--rw-r--r--   0 mborch     (501) staff       (20)       19 2018-02-21 11:40:43.000000 MacFSEvents-0.8.1/MacFSEvents.egg-info/top_level.txt
--rw-r--r--   0 mborch     (501) staff       (20)    10071 2018-02-21 11:40:44.000000 MacFSEvents-0.8.1/PKG-INFO
--rw-r--r--   0 mborch     (501) staff       (20)     4718 2017-10-23 06:47:33.000000 MacFSEvents-0.8.1/README.rst
--rw-r--r--   0 mborch     (501) staff       (20)    10752 2018-02-21 07:44:12.000000 MacFSEvents-0.8.1/_fsevents.c
--rw-r--r--   0 mborch     (501) staff       (20)     1182 2017-10-23 06:47:33.000000 MacFSEvents-0.8.1/compat.c
--rw-r--r--   0 mborch     (501) staff       (20)     1662 2017-10-23 06:47:33.000000 MacFSEvents-0.8.1/compat.h
--rw-r--r--   0 mborch     (501) staff       (20)     9606 2018-02-21 07:44:04.000000 MacFSEvents-0.8.1/fsevents.py
--rw-r--r--   0 mborch     (501) staff       (20)       38 2018-02-21 11:40:44.000000 MacFSEvents-0.8.1/setup.cfg
--rw-r--r--   0 mborch     (501) staff       (20)     1761 2018-02-21 11:40:25.000000 MacFSEvents-0.8.1/setup.py
--rw-r--r--   0 mborch     (501) staff       (20)    20100 2018-02-21 07:44:04.000000 MacFSEvents-0.8.1/tests.py
+drwxr-xr-x   0 mborch     (503) staff       (20)        0 2023-05-22 20:16:14.787247 MacFSEvents-0.8.2/
+-rw-r--r--   0 mborch     (503) staff       (20)     1287 2023-05-22 20:13:46.000000 MacFSEvents-0.8.2/LICENSE.txt
+drwxr-xr-x   0 mborch     (503) staff       (20)        0 2023-05-22 20:16:14.786979 MacFSEvents-0.8.2/MacFSEvents.egg-info/
+-rw-r--r--   0 mborch     (503) staff       (20)     7964 2023-05-22 20:16:14.000000 MacFSEvents-0.8.2/MacFSEvents.egg-info/PKG-INFO
+-rw-r--r--   0 mborch     (503) staff       (20)      238 2023-05-22 20:16:14.000000 MacFSEvents-0.8.2/MacFSEvents.egg-info/SOURCES.txt
+-rw-r--r--   0 mborch     (503) staff       (20)        1 2023-05-22 20:16:14.000000 MacFSEvents-0.8.2/MacFSEvents.egg-info/dependency_links.txt
+-rw-r--r--   0 mborch     (503) staff       (20)        1 2023-05-22 20:16:14.000000 MacFSEvents-0.8.2/MacFSEvents.egg-info/not-zip-safe
+-rw-r--r--   0 mborch     (503) staff       (20)       19 2023-05-22 20:16:14.000000 MacFSEvents-0.8.2/MacFSEvents.egg-info/top_level.txt
+-rw-r--r--   0 mborch     (503) staff       (20)     7964 2023-05-22 20:16:14.787132 MacFSEvents-0.8.2/PKG-INFO
+-rw-r--r--   0 mborch     (503) staff       (20)     4718 2023-05-22 20:13:46.000000 MacFSEvents-0.8.2/README.rst
+-rw-r--r--   0 mborch     (503) staff       (20)    10752 2023-05-22 20:13:46.000000 MacFSEvents-0.8.2/_fsevents.c
+-rw-r--r--   0 mborch     (503) staff       (20)     1182 2023-05-22 20:13:46.000000 MacFSEvents-0.8.2/compat.c
+-rw-r--r--   0 mborch     (503) staff       (20)     9607 2023-05-22 20:13:46.000000 MacFSEvents-0.8.2/fsevents.py
+-rw-r--r--   0 mborch     (503) staff       (20)       38 2023-05-22 20:16:14.787294 MacFSEvents-0.8.2/setup.cfg
+-rw-r--r--   0 mborch     (503) staff       (20)     1761 2023-05-22 20:15:53.000000 MacFSEvents-0.8.2/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `MacFSEvents-0.8.1/LICENSE.txt` & `MacFSEvents-0.8.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `MacFSEvents-0.8.1/README.rst` & `MacFSEvents-0.8.2/README.rst`

 * *Files identical despite different names*

### Comparing `MacFSEvents-0.8.1/_fsevents.c` & `MacFSEvents-0.8.2/_fsevents.c`

 * *Files identical despite different names*

### Comparing `MacFSEvents-0.8.1/compat.c` & `MacFSEvents-0.8.2/compat.c`

 * *Files identical despite different names*

### Comparing `MacFSEvents-0.8.1/fsevents.py` & `MacFSEvents-0.8.2/fsevents.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,15 +73,15 @@
 
     def __str__(self):
         vals = []
         for k, s in self._svals:
             if self & k:
                 vals.append(s)
 
-        res = "[" + "|".join(vals) + "]"
+        return "[" + "|".join(vals) + "]"
 
 
 # inotify event flags
 IN_MODIFY = 0x00000002
 IN_ATTRIB = 0x00000004
 IN_CREATE = 0x00000100
 IN_DELETE = 0x00000200
```

### Comparing `MacFSEvents-0.8.1/setup.py` & `MacFSEvents-0.8.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
               sources = ['_fsevents.c', 'compat.c'],
               extra_link_args = ["-framework","CoreFoundation",
                                "-framework","CoreServices"],
              ),
     ]
 
 setup(name = "MacFSEvents",
-      version = "0.8.1",
+      version = "0.8.2",
       description = "Thread-based interface to file system observation primitives.",
       long_description = "\n\n".join((read('README.rst'), read('CHANGES.rst'))),
       license = "BSD",
       data_files = [("", ["LICENSE.txt"])],
       author = "Malthe Borch",
       author_email = "mborch@gmail.com",
       url = 'https://github.com/malthe/macfsevents',
```

