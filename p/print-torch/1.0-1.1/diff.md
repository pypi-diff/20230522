# Comparing `tmp/print_torch-1.0.tar.gz` & `tmp/print_torch-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "print_torch-1.0.tar", last modified: Tue Feb 21 10:37:24 2023, max compression
+gzip compressed data, was "print_torch-1.1.tar", last modified: Mon May 22 18:19:42 2023, max compression
```

## Comparing `print_torch-1.0.tar` & `print_torch-1.1.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-02-21 10:37:24.076408 print_torch-1.0/
--rw-rw-rw-   0        0        0     1087 2023-02-21 10:28:32.000000 print_torch-1.0/LICENSE
--rw-rw-rw-   0        0        0      591 2023-02-21 10:37:24.076408 print_torch-1.0/PKG-INFO
--rw-rw-rw-   0        0        0      117 2023-02-21 10:33:10.000000 print_torch-1.0/README.md
--rw-rw-rw-   0        0        0      680 2023-02-21 10:34:24.000000 print_torch-1.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-02-21 10:37:24.076408 print_torch-1.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-02-21 10:37:24.060782 print_torch-1.0/src/
-drwxrwxrwx   0        0        0        0 2023-02-21 10:37:24.060782 print_torch-1.0/src/print_torch/
--rw-rw-rw-   0        0        0     4716 2023-02-21 10:37:09.000000 print_torch-1.0/src/print_torch/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-21 10:37:24.076408 print_torch-1.0/src/print_torch.egg-info/
--rw-rw-rw-   0        0        0      591 2023-02-21 10:37:24.000000 print_torch-1.0/src/print_torch.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      216 2023-02-21 10:37:24.000000 print_torch-1.0/src/print_torch.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-21 10:37:24.000000 print_torch-1.0/src/print_torch.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-02-21 10:37:24.000000 print_torch-1.0/src/print_torch.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 18:19:40.000000 print_torch-1.1/
+-rw-r--r--   0 root         (0) root         (0)     1067 2023-05-22 18:15:47.000000 print_torch-1.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1516 2023-05-22 18:19:42.000000 print_torch-1.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      985 2023-05-22 18:17:49.000000 print_torch-1.1/README.md
+-rw-r--r--   0 root         (0) root         (0)       84 2023-05-22 18:15:47.000000 print_torch-1.1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)      700 2023-05-22 18:19:42.000000 print_torch-1.1/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 18:19:40.000000 print_torch-1.1/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 18:19:40.000000 print_torch-1.1/src/print_torch/
+-rw-r--r--   0 root         (0) root         (0)     5442 2023-05-22 18:15:47.000000 print_torch-1.1/src/print_torch/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 18:19:40.000000 print_torch-1.1/src/print_torch.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1516 2023-05-22 18:19:40.000000 print_torch-1.1/src/print_torch.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      264 2023-05-22 18:19:40.000000 print_torch-1.1/src/print_torch.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-22 18:19:40.000000 print_torch-1.1/src/print_torch.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2023-05-22 18:19:40.000000 print_torch-1.1/src/print_torch.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-05-22 18:19:40.000000 print_torch-1.1/src/print_torch.egg-info/top_level.txt
```

### Comparing `print_torch-1.0/LICENSE` & `print_torch-1.1/LICENSE`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2023 Yuyao Huang
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+MIT License
+
+Copyright (c) 2023 Yuyao Huang
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
```

