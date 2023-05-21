# Comparing `tmp/jj_wingman-0.2.0.tar.gz` & `tmp/jj_wingman-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jj_wingman-0.2.0.tar", last modified: Sun May 21 21:46:22 2023, max compression
+gzip compressed data, was "jj_wingman-0.2.1.tar", last modified: Sun May 21 22:00:10 2023, max compression
```

## Comparing `jj_wingman-0.2.0.tar` & `jj_wingman-0.2.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-05-21 21:46:22.902831 jj_wingman-0.2.0/
--rw-rw-r--   0 jet       (1000) jet       (1000)     1074 2022-11-26 07:59:06.000000 jj_wingman-0.2.0/LICENSE.txt
--rw-rw-r--   0 jet       (1000) jet       (1000)    15185 2023-05-21 21:46:22.902831 jj_wingman-0.2.0/PKG-INFO
--rw-rw-r--   0 jet       (1000) jet       (1000)    13489 2023-03-07 18:53:37.000000 jj_wingman-0.2.0/README.md
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-05-21 21:46:22.902831 jj_wingman-0.2.0/jj_wingman.egg-info/
--rw-rw-r--   0 jet       (1000) jet       (1000)    15185 2023-05-21 21:46:22.000000 jj_wingman-0.2.0/jj_wingman.egg-info/PKG-INFO
--rw-rw-r--   0 jet       (1000) jet       (1000)      464 2023-05-21 21:46:22.000000 jj_wingman-0.2.0/jj_wingman.egg-info/SOURCES.txt
--rw-rw-r--   0 jet       (1000) jet       (1000)        1 2023-05-21 21:46:22.000000 jj_wingman-0.2.0/jj_wingman.egg-info/dependency_links.txt
--rw-rw-r--   0 jet       (1000) jet       (1000)      116 2023-05-21 21:46:22.000000 jj_wingman-0.2.0/jj_wingman.egg-info/entry_points.txt
--rw-rw-r--   0 jet       (1000) jet       (1000)       19 2023-05-21 21:46:22.000000 jj_wingman-0.2.0/jj_wingman.egg-info/requires.txt
--rw-rw-r--   0 jet       (1000) jet       (1000)        8 2023-05-21 21:46:22.000000 jj_wingman-0.2.0/jj_wingman.egg-info/top_level.txt
--rw-rw-r--   0 jet       (1000) jet       (1000)      927 2023-05-21 21:46:10.000000 jj_wingman-0.2.0/pyproject.toml
--rw-rw-r--   0 jet       (1000) jet       (1000)       38 2023-05-21 21:46:22.902831 jj_wingman-0.2.0/setup.cfg
--rw-rw-r--   0 jet       (1000) jet       (1000)       92 2023-03-07 18:49:10.000000 jj_wingman-0.2.0/setup.py
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-05-21 21:46:22.902831 jj_wingman-0.2.0/test/
--rw-rw-r--   0 jet       (1000) jet       (1000)     2737 2023-05-21 21:40:50.000000 jj_wingman-0.2.0/test/test_replay_buffer.py
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-05-21 21:46:22.902831 jj_wingman-0.2.0/wingman/
--rw-rw-r--   0 jet       (1000) jet       (1000)      218 2022-12-10 02:36:58.000000 jj_wingman-0.2.0/wingman/__init__.py
--rw-rw-r--   0 jet       (1000) jet       (1000)     4130 2023-03-07 18:48:06.000000 jj_wingman-0.2.0/wingman/cli_scripts.py
--rw-rw-r--   0 jet       (1000) jet       (1000)      288 2022-11-26 07:59:06.000000 jj_wingman-0.2.0/wingman/config.yaml
--rw-rw-r--   0 jet       (1000) jet       (1000)    10106 2023-03-07 18:50:52.000000 jj_wingman-0.2.0/wingman/neural_blocks.py
--rw-rw-r--   0 jet       (1000) jet       (1000)      777 2023-03-07 18:47:29.000000 jj_wingman-0.2.0/wingman/print_utils.py
--rw-rw-r--   0 jet       (1000) jet       (1000)     5675 2023-05-21 21:06:37.000000 jj_wingman-0.2.0/wingman/replay_buffer.py
--rw-rw-r--   0 jet       (1000) jet       (1000)     1033 2023-03-07 18:51:03.000000 jj_wingman-0.2.0/wingman/utils.py
--rw-rw-r--   0 jet       (1000) jet       (1000)    15009 2023-03-07 18:51:08.000000 jj_wingman-0.2.0/wingman/wingman.py
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-05-21 22:00:10.428175 jj_wingman-0.2.1/
+-rw-rw-r--   0 jet       (1000) jet       (1000)     1074 2022-11-26 07:59:06.000000 jj_wingman-0.2.1/LICENSE.txt
+-rw-rw-r--   0 jet       (1000) jet       (1000)    15185 2023-05-21 22:00:10.428175 jj_wingman-0.2.1/PKG-INFO
+-rw-rw-r--   0 jet       (1000) jet       (1000)    13489 2023-03-07 18:53:37.000000 jj_wingman-0.2.1/README.md
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-05-21 22:00:10.424175 jj_wingman-0.2.1/jj_wingman.egg-info/
+-rw-rw-r--   0 jet       (1000) jet       (1000)    15185 2023-05-21 22:00:10.000000 jj_wingman-0.2.1/jj_wingman.egg-info/PKG-INFO
+-rw-rw-r--   0 jet       (1000) jet       (1000)      464 2023-05-21 22:00:10.000000 jj_wingman-0.2.1/jj_wingman.egg-info/SOURCES.txt
+-rw-rw-r--   0 jet       (1000) jet       (1000)        1 2023-05-21 22:00:10.000000 jj_wingman-0.2.1/jj_wingman.egg-info/dependency_links.txt
+-rw-rw-r--   0 jet       (1000) jet       (1000)      116 2023-05-21 22:00:10.000000 jj_wingman-0.2.1/jj_wingman.egg-info/entry_points.txt
+-rw-rw-r--   0 jet       (1000) jet       (1000)       19 2023-05-21 22:00:10.000000 jj_wingman-0.2.1/jj_wingman.egg-info/requires.txt
+-rw-rw-r--   0 jet       (1000) jet       (1000)        8 2023-05-21 22:00:10.000000 jj_wingman-0.2.1/jj_wingman.egg-info/top_level.txt
+-rw-rw-r--   0 jet       (1000) jet       (1000)      927 2023-05-21 22:00:06.000000 jj_wingman-0.2.1/pyproject.toml
+-rw-rw-r--   0 jet       (1000) jet       (1000)       38 2023-05-21 22:00:10.428175 jj_wingman-0.2.1/setup.cfg
+-rw-rw-r--   0 jet       (1000) jet       (1000)       92 2023-03-07 18:49:10.000000 jj_wingman-0.2.1/setup.py
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-05-21 22:00:10.424175 jj_wingman-0.2.1/test/
+-rw-rw-r--   0 jet       (1000) jet       (1000)     2737 2023-05-21 21:40:50.000000 jj_wingman-0.2.1/test/test_replay_buffer.py
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-05-21 22:00:10.428175 jj_wingman-0.2.1/wingman/
+-rw-rw-r--   0 jet       (1000) jet       (1000)      218 2022-12-10 02:36:58.000000 jj_wingman-0.2.1/wingman/__init__.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)     4130 2023-03-07 18:48:06.000000 jj_wingman-0.2.1/wingman/cli_scripts.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)      288 2022-11-26 07:59:06.000000 jj_wingman-0.2.1/wingman/config.yaml
+-rw-rw-r--   0 jet       (1000) jet       (1000)    10106 2023-03-07 18:50:52.000000 jj_wingman-0.2.1/wingman/neural_blocks.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)      777 2023-03-07 18:47:29.000000 jj_wingman-0.2.1/wingman/print_utils.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)     5617 2023-05-21 21:59:51.000000 jj_wingman-0.2.1/wingman/replay_buffer.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)     1033 2023-03-07 18:51:03.000000 jj_wingman-0.2.1/wingman/utils.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)    15009 2023-03-07 18:51:08.000000 jj_wingman-0.2.1/wingman/wingman.py
```

### Comparing `jj_wingman-0.2.0/LICENSE.txt` & `jj_wingman-0.2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jj_wingman-0.2.0/PKG-INFO` & `jj_wingman-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jj_wingman
-Version: 0.2.0
+Version: 0.2.1
 Summary: Wingman library for AI projects.
 Author-email: Jet <taijunjet@hotmail.com>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `jj_wingman-0.2.0/README.md` & `jj_wingman-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `jj_wingman-0.2.0/jj_wingman.egg-info/PKG-INFO` & `jj_wingman-0.2.1/jj_wingman.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jj-wingman
-Version: 0.2.0
+Version: 0.2.1
 Summary: Wingman library for AI projects.
 Author-email: Jet <taijunjet@hotmail.com>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `jj_wingman-0.2.0/pyproject.toml` & `jj_wingman-0.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "jj_wingman"
-version = "0.2.0"
+version = "0.2.1"
 authors = [
   { name="Jet", email="taijunjet@hotmail.com" },
 ]
 description = "Wingman library for AI projects."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `jj_wingman-0.2.0/test/test_replay_buffer.py` & `jj_wingman-0.2.1/test/test_replay_buffer.py`

 * *Files identical despite different names*

### Comparing `jj_wingman-0.2.0/wingman/cli_scripts.py` & `jj_wingman-0.2.1/wingman/cli_scripts.py`

 * *Files identical despite different names*

### Comparing `jj_wingman-0.2.0/wingman/neural_blocks.py` & `jj_wingman-0.2.1/wingman/neural_blocks.py`

 * *Files identical despite different names*

### Comparing `jj_wingman-0.2.0/wingman/print_utils.py` & `jj_wingman-0.2.1/wingman/print_utils.py`

 * *Files identical despite different names*

### Comparing `jj_wingman-0.2.0/wingman/replay_buffer.py` & `jj_wingman-0.2.1/wingman/replay_buffer.py`

 * *Files 1% similar despite different names*

```diff
@@ -137,17 +137,14 @@
                     start, size=np.maximum(rollover, 0), replace=False
                 )
             else:
                 idx_start = np.random.choice(
                     self.mem_size, size=bulk_size, replace=False
                 )
                 idx_stop = []
-
-            print(idx_start)
-            print(idx_stop)
         else:
             idx_start = np.arange(start, stop)
             idx_stop = np.arange(0, rollover)
         indices = np.append(idx_start, idx_stop).astype(np.int64)
 
         # put things in memory
         for memory, thing in zip(self.memory, np_data):
```

### Comparing `jj_wingman-0.2.0/wingman/utils.py` & `jj_wingman-0.2.1/wingman/utils.py`

 * *Files identical despite different names*

### Comparing `jj_wingman-0.2.0/wingman/wingman.py` & `jj_wingman-0.2.1/wingman/wingman.py`

 * *Files identical despite different names*

