# Comparing `tmp/shellcrafter-1.0.4.tar.gz` & `tmp/shellcrafter-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shellcrafter-1.0.4.tar", last modified: Sun May 14 00:02:10 2023, max compression
+gzip compressed data, was "shellcrafter-1.0.5.tar", last modified: Mon May 22 15:35:13 2023, max compression
```

## Comparing `shellcrafter-1.0.4.tar` & `shellcrafter-1.0.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 00:02:10.443976 shellcrafter-1.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-05-14 00:02:10.443976 shellcrafter-1.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-05-14 00:01:48.000000 shellcrafter-1.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-05-14 00:01:48.000000 shellcrafter-1.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-14 00:02:10.443976 shellcrafter-1.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-05-14 00:01:48.000000 shellcrafter-1.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 00:02:10.443976 shellcrafter-1.0.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 00:02:10.443976 shellcrafter-1.0.4/src/shellcrafter/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 00:01:48.000000 shellcrafter-1.0.4/src/shellcrafter/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1121 2023-05-14 00:01:48.000000 shellcrafter-1.0.4/src/shellcrafter/ascii_hex_stack_push_converter.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    11958 2023-05-14 00:01:48.000000 shellcrafter-1.0.4/src/shellcrafter/find_gadgets.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7011 2023-05-14 00:01:48.000000 shellcrafter-1.0.4/src/shellcrafter/keyst_api.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1082 2023-05-14 00:01:48.000000 shellcrafter-1.0.4/src/shellcrafter/ror_hash.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 00:02:10.443976 shellcrafter-1.0.4/src/shellcrafter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-05-14 00:02:10.000000 shellcrafter-1.0.4/src/shellcrafter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-05-14 00:02:10.000000 shellcrafter-1.0.4/src/shellcrafter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 00:02:10.000000 shellcrafter-1.0.4/src/shellcrafter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-05-14 00:02:10.000000 shellcrafter-1.0.4/src/shellcrafter.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-14 00:02:10.000000 shellcrafter-1.0.4/src/shellcrafter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-14 00:02:10.000000 shellcrafter-1.0.4/src/shellcrafter.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:35:13.531230 shellcrafter-1.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-05-22 15:35:13.531230 shellcrafter-1.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-05-22 15:34:48.000000 shellcrafter-1.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-05-22 15:34:48.000000 shellcrafter-1.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 15:35:13.531230 shellcrafter-1.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-05-22 15:34:48.000000 shellcrafter-1.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:35:13.527230 shellcrafter-1.0.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:35:13.531230 shellcrafter-1.0.5/src/shellcrafter/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 15:34:48.000000 shellcrafter-1.0.5/src/shellcrafter/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1100 2023-05-22 15:34:48.000000 shellcrafter-1.0.5/src/shellcrafter/ascii_hex_stack_push_converter.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11958 2023-05-22 15:34:48.000000 shellcrafter-1.0.5/src/shellcrafter/find_gadgets.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7011 2023-05-22 15:34:48.000000 shellcrafter-1.0.5/src/shellcrafter/keyst_api.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1082 2023-05-22 15:34:48.000000 shellcrafter-1.0.5/src/shellcrafter/ror_hash.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:35:13.531230 shellcrafter-1.0.5/src/shellcrafter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-05-22 15:35:13.000000 shellcrafter-1.0.5/src/shellcrafter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-05-22 15:35:13.000000 shellcrafter-1.0.5/src/shellcrafter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 15:35:13.000000 shellcrafter-1.0.5/src/shellcrafter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-05-22 15:35:13.000000 shellcrafter-1.0.5/src/shellcrafter.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-22 15:35:13.000000 shellcrafter-1.0.5/src/shellcrafter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-22 15:35:13.000000 shellcrafter-1.0.5/src/shellcrafter.egg-info/top_level.txt
```

### Comparing `shellcrafter-1.0.4/PKG-INFO` & `shellcrafter-1.0.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shellcrafter
-Version: 1.0.4
+Version: 1.0.5
 Summary: A package containing scripts for developing and generating shellcode
 Home-page: https://github.com/totekuh/shellcrafter
 Author: totekuh
 Author-email: totekuh@protonmail.com
 Project-URL: Bug Reports, https://github.com/totekuh/shellcrafter/issues
 Project-URL: Source, https://github.com/totekuh/shellcrafter
```

### Comparing `shellcrafter-1.0.4/README.md` & `shellcrafter-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `shellcrafter-1.0.4/setup.py` & `shellcrafter-1.0.5/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python3
 
-version = "1.0.4"
+version = "1.0.5"
 
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
```

### Comparing `shellcrafter-1.0.4/src/shellcrafter/ascii_hex_stack_push_converter.py` & `shellcrafter-1.0.5/src/shellcrafter/ascii_hex_stack_push_converter.py`

 * *Files 12% similar despite different names*

```diff
@@ -19,15 +19,14 @@
 def str_to_hex_little_endian_push(s):
     hex_str = binascii.hexlify(s.encode('utf-8')).decode('utf-8')
     hex_str = ''.join(reversed([hex_str[i:i+2] for i in range(0, len(hex_str), 2)]))
     if len(hex_str) % 8 != 0:
         hex_str = '0' * (8 - len(hex_str) % 8) + hex_str
     result = os.linesep.join([hex_str[i:i + 8] for i in range(0, len(hex_str), 8)])
     result = [f"push 0x{h}" for h in result.split(os.linesep)]
-    result.reverse()
     for h in result:
         print(h)
 
 def main():
     options = get_arguments()
     string = options.input
     str_to_hex_little_endian_push(s=string)
```

### Comparing `shellcrafter-1.0.4/src/shellcrafter/find_gadgets.py` & `shellcrafter-1.0.5/src/shellcrafter/find_gadgets.py`

 * *Files identical despite different names*

### Comparing `shellcrafter-1.0.4/src/shellcrafter/keyst_api.py` & `shellcrafter-1.0.5/src/shellcrafter/keyst_api.py`

 * *Files identical despite different names*

### Comparing `shellcrafter-1.0.4/src/shellcrafter/ror_hash.py` & `shellcrafter-1.0.5/src/shellcrafter/ror_hash.py`

 * *Files identical despite different names*

### Comparing `shellcrafter-1.0.4/src/shellcrafter.egg-info/PKG-INFO` & `shellcrafter-1.0.5/src/shellcrafter.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shellcrafter
-Version: 1.0.4
+Version: 1.0.5
 Summary: A package containing scripts for developing and generating shellcode
 Home-page: https://github.com/totekuh/shellcrafter
 Author: totekuh
 Author-email: totekuh@protonmail.com
 Project-URL: Bug Reports, https://github.com/totekuh/shellcrafter/issues
 Project-URL: Source, https://github.com/totekuh/shellcrafter
```

