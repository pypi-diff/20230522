# Comparing `tmp/JanusReader-0.6.0.tar.gz` & `tmp/JanusReader-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "JanusReader-0.6.0.tar", last modified: Mon May 22 13:31:29 2023, max compression
+gzip compressed data, was "JanusReader-0.6.1.tar", last modified: Mon May 22 13:35:56 2023, max compression
```

## Comparing `JanusReader-0.6.0.tar` & `JanusReader-0.6.1.tar`

### file list

```diff
@@ -1,18 +1,17 @@
-drwxr-xr-x   0 romolo.politi   (501) staff       (20)        0 2023-05-22 13:31:29.925830 JanusReader-0.6.0/
--rw-r--r--   0 romolo.politi   (501) staff       (20)      449 2023-05-22 13:31:29.925626 JanusReader-0.6.0/PKG-INFO
--rw-r--r--   0 romolo.politi   (501) staff       (20)      257 2023-05-10 08:09:29.000000 JanusReader-0.6.0/README.md
--rw-r--r--   0 romolo.politi   (501) staff       (20)      437 2023-05-22 12:55:55.000000 JanusReader-0.6.0/pyproject.toml
--rw-r--r--   0 romolo.politi   (501) staff       (20)       38 2023-05-22 13:31:29.925894 JanusReader-0.6.0/setup.cfg
-drwxr-xr-x   0 romolo.politi   (501) staff       (20)        0 2023-05-22 13:31:29.922310 JanusReader-0.6.0/src/
-drwxr-xr-x   0 romolo.politi   (501) staff       (20)        0 2023-05-22 13:31:29.924084 JanusReader-0.6.0/src/JanusReader/
--rw-r--r--   0 romolo.politi   (501) staff       (20)       88 2023-03-03 08:06:39.000000 JanusReader-0.6.0/src/JanusReader/__init__.py
--rw-r--r--   0 romolo.politi   (501) staff       (20)      103 2022-05-04 08:58:16.000000 JanusReader-0.6.0/src/JanusReader/exceptions.py
--rw-r--r--   0 romolo.politi   (501) staff       (20)    13722 2023-05-22 13:19:55.000000 JanusReader-0.6.0/src/JanusReader/janusReader.py
--rw-r--r--   0 romolo.politi   (501) staff       (20)     2302 2023-03-03 15:12:36.000000 JanusReader-0.6.0/src/JanusReader/vicar_head.py
-drwxr-xr-x   0 romolo.politi   (501) staff       (20)        0 2023-05-22 13:31:29.925333 JanusReader-0.6.0/src/JanusReader.egg-info/
--rw-r--r--   0 romolo.politi   (501) staff       (20)      449 2023-05-22 13:31:29.000000 JanusReader-0.6.0/src/JanusReader.egg-info/PKG-INFO
--rw-r--r--   0 romolo.politi   (501) staff       (20)      348 2023-05-22 13:31:29.000000 JanusReader-0.6.0/src/JanusReader.egg-info/SOURCES.txt
--rw-r--r--   0 romolo.politi   (501) staff       (20)        1 2023-05-22 13:31:29.000000 JanusReader-0.6.0/src/JanusReader.egg-info/dependency_links.txt
--rw-r--r--   0 romolo.politi   (501) staff       (20)       73 2023-05-22 13:31:29.000000 JanusReader-0.6.0/src/JanusReader.egg-info/requires.txt
--rw-r--r--   0 romolo.politi   (501) staff       (20)       16 2023-05-22 13:31:29.000000 JanusReader-0.6.0/src/JanusReader.egg-info/top_level.txt
--rwxr-xr-x   0 romolo.politi   (501) staff       (20)     1421 2023-05-22 11:20:37.000000 JanusReader-0.6.0/src/run.py
+drwxr-xr-x   0 romolo.politi   (501) staff       (20)        0 2023-05-22 13:35:56.470911 JanusReader-0.6.1/
+-rw-r--r--   0 romolo.politi   (501) staff       (20)      449 2023-05-22 13:35:56.470702 JanusReader-0.6.1/PKG-INFO
+-rw-r--r--   0 romolo.politi   (501) staff       (20)      257 2023-05-22 13:35:12.000000 JanusReader-0.6.1/README.md
+-rw-r--r--   0 romolo.politi   (501) staff       (20)      437 2023-05-22 13:35:42.000000 JanusReader-0.6.1/pyproject.toml
+-rw-r--r--   0 romolo.politi   (501) staff       (20)       38 2023-05-22 13:35:56.470976 JanusReader-0.6.1/setup.cfg
+drwxr-xr-x   0 romolo.politi   (501) staff       (20)        0 2023-05-22 13:35:56.467550 JanusReader-0.6.1/src/
+drwxr-xr-x   0 romolo.politi   (501) staff       (20)        0 2023-05-22 13:35:56.469112 JanusReader-0.6.1/src/JanusReader/
+-rw-r--r--   0 romolo.politi   (501) staff       (20)       88 2023-03-03 08:06:39.000000 JanusReader-0.6.1/src/JanusReader/__init__.py
+-rw-r--r--   0 romolo.politi   (501) staff       (20)      103 2022-05-04 08:58:16.000000 JanusReader-0.6.1/src/JanusReader/exceptions.py
+-rw-r--r--   0 romolo.politi   (501) staff       (20)    13490 2023-05-22 13:35:01.000000 JanusReader-0.6.1/src/JanusReader/janusReader.py
+-rw-r--r--   0 romolo.politi   (501) staff       (20)     2302 2023-03-03 15:12:36.000000 JanusReader-0.6.1/src/JanusReader/vicar_head.py
+drwxr-xr-x   0 romolo.politi   (501) staff       (20)        0 2023-05-22 13:35:56.470399 JanusReader-0.6.1/src/JanusReader.egg-info/
+-rw-r--r--   0 romolo.politi   (501) staff       (20)      449 2023-05-22 13:35:56.000000 JanusReader-0.6.1/src/JanusReader.egg-info/PKG-INFO
+-rw-r--r--   0 romolo.politi   (501) staff       (20)      337 2023-05-22 13:35:56.000000 JanusReader-0.6.1/src/JanusReader.egg-info/SOURCES.txt
+-rw-r--r--   0 romolo.politi   (501) staff       (20)        1 2023-05-22 13:35:56.000000 JanusReader-0.6.1/src/JanusReader.egg-info/dependency_links.txt
+-rw-r--r--   0 romolo.politi   (501) staff       (20)       73 2023-05-22 13:35:56.000000 JanusReader-0.6.1/src/JanusReader.egg-info/requires.txt
+-rw-r--r--   0 romolo.politi   (501) staff       (20)       12 2023-05-22 13:35:56.000000 JanusReader-0.6.1/src/JanusReader.egg-info/top_level.txt
```

### Comparing `JanusReader-0.6.0/src/JanusReader/janusReader.py` & `JanusReader-0.6.1/src/JanusReader/janusReader.py`

 * *Files 2% similar despite different names*

```diff
@@ -258,18 +258,14 @@
         self.Samples = int(getValue(elem[1], "pds:elements"))
         self.Lines = int(getValue(elem[0], "pds:elements"))
         # console.print(timeCoord)
 
             
         # if self.Format == "HALF":
         if self.level.lower()=='raw':
-            self.console.print(self.Offset)
-            self.console.print(self.Lines, self.Samples)
-            self.console.print(self.fileName.stat().st_size)
-            self.console.print(self.Lines*self.Samples*2+self.Offset)
             with open(self.fileName, 'rb') as f:
                 f.seek(self.Offset)
                 self.image = np.reshape(np.frombuffer(f.read(
                     self.Lines * self.Samples * 2), dtype=np.uint16), (self.Lines, self.Samples))
         else:
             with open(self.fileName, 'rb') as f:
                 self.image = np.reshape(np.frombuffer(
```

### Comparing `JanusReader-0.6.0/src/JanusReader/vicar_head.py` & `JanusReader-0.6.1/src/JanusReader/vicar_head.py`

 * *Files identical despite different names*

