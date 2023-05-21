# Comparing `tmp/loquax-0.1.3.tar.gz` & `tmp/loquax-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "loquax-0.1.3.tar", last modified: Sun May 21 22:26:18 2023, max compression
+gzip compressed data, was "loquax-0.1.4.tar", last modified: Sun May 21 23:37:02 2023, max compression
```

## Comparing `loquax-0.1.3.tar` & `loquax-0.1.4.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 matthieucourt   (501) staff       (20)        0 2023-05-21 22:26:18.694016 loquax-0.1.3/
--rw-r--r--   0 matthieucourt   (501) staff       (20)    35149 2023-02-10 04:45:57.000000 loquax-0.1.3/LICENSE
--rw-r--r--   0 matthieucourt   (501) staff       (20)     2180 2023-05-21 22:26:18.693764 loquax-0.1.3/PKG-INFO
--rw-r--r--   0 matthieucourt   (501) staff       (20)     1628 2023-05-21 22:22:52.000000 loquax-0.1.3/README.md
-drwxr-xr-x   0 matthieucourt   (501) staff       (20)        0 2023-05-21 22:26:18.685374 loquax-0.1.3/loquax/
--rw-r--r--   0 matthieucourt   (501) staff       (20)       44 2023-05-19 13:53:25.000000 loquax-0.1.3/loquax/__init__.py
-drwxr-xr-x   0 matthieucourt   (501) staff       (20)        0 2023-05-21 22:26:18.689257 loquax-0.1.3/loquax/abstractions/
--rw-r--r--   0 matthieucourt   (501) staff       (20)      191 2023-05-19 13:53:25.000000 loquax-0.1.3/loquax/abstractions/__init__.py
--rw-r--r--   0 matthieucourt   (501) staff       (20)     1637 2023-05-19 13:53:25.000000 loquax-0.1.3/loquax/abstractions/constants.py
--rw-r--r--   0 matthieucourt   (501) staff       (20)     9318 2023-05-21 22:15:45.000000 loquax-0.1.3/loquax/abstractions/linguistic_entities.py
--rw-r--r--   0 matthieucourt   (501) staff       (20)     1092 2023-05-21 06:24:06.000000 loquax-0.1.3/loquax/abstractions/phonology.py
--rw-r--r--   0 matthieucourt   (501) staff       (20)     2526 2023-05-19 13:53:25.000000 loquax-0.1.3/loquax/abstractions/syllabification.py
-drwxr-xr-x   0 matthieucourt   (501) staff       (20)        0 2023-05-21 22:26:18.690273 loquax-0.1.3/loquax/languages/
--rw-r--r--   0 matthieucourt   (501) staff       (20)       25 2023-05-19 13:53:25.000000 loquax-0.1.3/loquax/languages/__init__.py
--rw-r--r--   0 matthieucourt   (501) staff       (20)      925 2023-05-19 13:53:25.000000 loquax-0.1.3/loquax/languages/latin.py
-drwxr-xr-x   0 matthieucourt   (501) staff       (20)        0 2023-05-21 22:26:18.691562 loquax-0.1.3/loquax/languages/latin_conf/
--rw-r--r--   0 matthieucourt   (501) staff       (20)        0 2023-05-19 19:53:03.000000 loquax-0.1.3/loquax/languages/latin_conf/__init__.py
--rw-r--r--   0 matthieucourt   (501) staff       (20)     1058 2023-05-19 13:53:25.000000 loquax-0.1.3/loquax/languages/latin_conf/constants.py
--rw-r--r--   0 matthieucourt   (501) staff       (20)     3361 2023-05-19 13:53:25.000000 loquax-0.1.3/loquax/languages/latin_conf/rules.py
--rw-r--r--   0 matthieucourt   (501) staff       (20)      574 2023-05-19 13:53:25.000000 loquax-0.1.3/loquax/languages/latin_conf/tokenizer.py
-drwxr-xr-x   0 matthieucourt   (501) staff       (20)        0 2023-05-21 22:26:18.693114 loquax-0.1.3/loquax/text_processing/
--rw-r--r--   0 matthieucourt   (501) staff       (20)      107 2023-05-19 13:53:25.000000 loquax-0.1.3/loquax/text_processing/__init__.py
--rw-r--r--   0 matthieucourt   (501) staff       (20)     1105 2023-05-19 13:53:25.000000 loquax-0.1.3/loquax/text_processing/commons.py
--rw-r--r--   0 matthieucourt   (501) staff       (20)     3458 2023-05-21 22:13:30.000000 loquax-0.1.3/loquax/text_processing/processing.py
-drwxr-xr-x   0 matthieucourt   (501) staff       (20)        0 2023-05-21 22:26:18.686970 loquax-0.1.3/loquax.egg-info/
--rw-r--r--   0 matthieucourt   (501) staff       (20)     2180 2023-05-21 22:26:18.000000 loquax-0.1.3/loquax.egg-info/PKG-INFO
--rw-r--r--   0 matthieucourt   (501) staff       (20)      680 2023-05-21 22:26:18.000000 loquax-0.1.3/loquax.egg-info/SOURCES.txt
--rw-r--r--   0 matthieucourt   (501) staff       (20)        1 2023-05-21 22:26:18.000000 loquax-0.1.3/loquax.egg-info/dependency_links.txt
--rw-r--r--   0 matthieucourt   (501) staff       (20)        7 2023-05-21 22:26:18.000000 loquax-0.1.3/loquax.egg-info/top_level.txt
--rw-r--r--   0 matthieucourt   (501) staff       (20)      183 2023-05-19 13:53:25.000000 loquax-0.1.3/pyproject.toml
--rw-r--r--   0 matthieucourt   (501) staff       (20)       38 2023-05-21 22:26:18.694103 loquax-0.1.3/setup.cfg
--rw-r--r--   0 matthieucourt   (501) staff       (20)      779 2023-05-21 22:26:08.000000 loquax-0.1.3/setup.py
+drwxr-xr-x   0 matthieucourt   (501) staff       (20)        0 2023-05-21 23:37:02.857317 loquax-0.1.4/
+-rw-r--r--   0 matthieucourt   (501) staff       (20)    35149 2023-02-10 04:45:57.000000 loquax-0.1.4/LICENSE
+-rw-r--r--   0 matthieucourt   (501) staff       (20)     2180 2023-05-21 23:37:02.857033 loquax-0.1.4/PKG-INFO
+-rw-r--r--   0 matthieucourt   (501) staff       (20)     1628 2023-05-21 22:22:52.000000 loquax-0.1.4/README.md
+drwxr-xr-x   0 matthieucourt   (501) staff       (20)        0 2023-05-21 23:37:02.846290 loquax-0.1.4/loquax/
+-rw-r--r--   0 matthieucourt   (501) staff       (20)       44 2023-05-19 13:53:25.000000 loquax-0.1.4/loquax/__init__.py
+drwxr-xr-x   0 matthieucourt   (501) staff       (20)        0 2023-05-21 23:37:02.850868 loquax-0.1.4/loquax/abstractions/
+-rw-r--r--   0 matthieucourt   (501) staff       (20)      191 2023-05-19 13:53:25.000000 loquax-0.1.4/loquax/abstractions/__init__.py
+-rw-r--r--   0 matthieucourt   (501) staff       (20)     1637 2023-05-19 13:53:25.000000 loquax-0.1.4/loquax/abstractions/constants.py
+-rw-r--r--   0 matthieucourt   (501) staff       (20)     9318 2023-05-21 22:15:45.000000 loquax-0.1.4/loquax/abstractions/linguistic_entities.py
+-rw-r--r--   0 matthieucourt   (501) staff       (20)     1092 2023-05-21 06:24:06.000000 loquax-0.1.4/loquax/abstractions/phonology.py
+-rw-r--r--   0 matthieucourt   (501) staff       (20)     2526 2023-05-19 13:53:25.000000 loquax-0.1.4/loquax/abstractions/syllabification.py
+drwxr-xr-x   0 matthieucourt   (501) staff       (20)        0 2023-05-21 23:37:02.852212 loquax-0.1.4/loquax/languages/
+-rw-r--r--   0 matthieucourt   (501) staff       (20)       25 2023-05-19 13:53:25.000000 loquax-0.1.4/loquax/languages/__init__.py
+-rw-r--r--   0 matthieucourt   (501) staff       (20)      925 2023-05-19 13:53:25.000000 loquax-0.1.4/loquax/languages/latin.py
+drwxr-xr-x   0 matthieucourt   (501) staff       (20)        0 2023-05-21 23:37:02.854102 loquax-0.1.4/loquax/languages/latin_conf/
+-rw-r--r--   0 matthieucourt   (501) staff       (20)        0 2023-05-19 19:53:03.000000 loquax-0.1.4/loquax/languages/latin_conf/__init__.py
+-rw-r--r--   0 matthieucourt   (501) staff       (20)     1058 2023-05-19 13:53:25.000000 loquax-0.1.4/loquax/languages/latin_conf/constants.py
+-rw-r--r--   0 matthieucourt   (501) staff       (20)     3361 2023-05-19 13:53:25.000000 loquax-0.1.4/loquax/languages/latin_conf/rules.py
+-rw-r--r--   0 matthieucourt   (501) staff       (20)      574 2023-05-19 13:53:25.000000 loquax-0.1.4/loquax/languages/latin_conf/tokenizer.py
+drwxr-xr-x   0 matthieucourt   (501) staff       (20)        0 2023-05-21 23:37:02.856278 loquax-0.1.4/loquax/text_processing/
+-rw-r--r--   0 matthieucourt   (501) staff       (20)      107 2023-05-19 13:53:25.000000 loquax-0.1.4/loquax/text_processing/__init__.py
+-rw-r--r--   0 matthieucourt   (501) staff       (20)     1105 2023-05-19 13:53:25.000000 loquax-0.1.4/loquax/text_processing/commons.py
+-rw-r--r--   0 matthieucourt   (501) staff       (20)     3463 2023-05-21 23:09:01.000000 loquax-0.1.4/loquax/text_processing/processing.py
+drwxr-xr-x   0 matthieucourt   (501) staff       (20)        0 2023-05-21 23:37:02.847979 loquax-0.1.4/loquax.egg-info/
+-rw-r--r--   0 matthieucourt   (501) staff       (20)     2180 2023-05-21 23:37:02.000000 loquax-0.1.4/loquax.egg-info/PKG-INFO
+-rw-r--r--   0 matthieucourt   (501) staff       (20)      680 2023-05-21 23:37:02.000000 loquax-0.1.4/loquax.egg-info/SOURCES.txt
+-rw-r--r--   0 matthieucourt   (501) staff       (20)        1 2023-05-21 23:37:02.000000 loquax-0.1.4/loquax.egg-info/dependency_links.txt
+-rw-r--r--   0 matthieucourt   (501) staff       (20)        7 2023-05-21 23:37:02.000000 loquax-0.1.4/loquax.egg-info/top_level.txt
+-rw-r--r--   0 matthieucourt   (501) staff       (20)      183 2023-05-19 13:53:25.000000 loquax-0.1.4/pyproject.toml
+-rw-r--r--   0 matthieucourt   (501) staff       (20)       38 2023-05-21 23:37:02.857407 loquax-0.1.4/setup.cfg
+-rw-r--r--   0 matthieucourt   (501) staff       (20)      779 2023-05-21 23:36:43.000000 loquax-0.1.4/setup.py
```

### Comparing `loquax-0.1.3/LICENSE` & `loquax-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `loquax-0.1.3/PKG-INFO` & `loquax-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: loquax
-Version: 0.1.3
+Version: 0.1.4
 Summary: A Classical Phonology framework
 Home-page: https://github.com/mattlianje/loquax
 Author: Matthieu Court
 Author-email: matthieu.court@protonmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: loquax Version: 0.1.3 Summary: A Classical
+Metadata-Version: 2.1 Name: loquax Version: 0.1.4 Summary: A Classical
 Phonology framework Home-page: https://github.com/mattlianje/loquax Author:
 Matthieu Court Author-email: matthieu.court@protonmail.com License: UNKNOWN
 Platform: UNKNOWN Classifier: Development Status :: 3 - Alpha Classifier:
 Intended Audience :: Science/Research Classifier: License :: OSI Approved ::
 GNU General Public License v3 (GPLv3) Classifier: Programming Language ::
 Python :: 3.10 Requires-Python: >=3.10 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `loquax-0.1.3/README.md` & `loquax-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `loquax-0.1.3/loquax/abstractions/constants.py` & `loquax-0.1.4/loquax/abstractions/constants.py`

 * *Files identical despite different names*

### Comparing `loquax-0.1.3/loquax/abstractions/linguistic_entities.py` & `loquax-0.1.4/loquax/abstractions/linguistic_entities.py`

 * *Files identical despite different names*

### Comparing `loquax-0.1.3/loquax/abstractions/phonology.py` & `loquax-0.1.4/loquax/abstractions/phonology.py`

 * *Files identical despite different names*

### Comparing `loquax-0.1.3/loquax/abstractions/syllabification.py` & `loquax-0.1.4/loquax/abstractions/syllabification.py`

 * *Files identical despite different names*

### Comparing `loquax-0.1.3/loquax/languages/latin.py` & `loquax-0.1.4/loquax/languages/latin.py`

 * *Files identical despite different names*

### Comparing `loquax-0.1.3/loquax/languages/latin_conf/constants.py` & `loquax-0.1.4/loquax/languages/latin_conf/constants.py`

 * *Files identical despite different names*

### Comparing `loquax-0.1.3/loquax/languages/latin_conf/rules.py` & `loquax-0.1.4/loquax/languages/latin_conf/rules.py`

 * *Files identical despite different names*

### Comparing `loquax-0.1.3/loquax/languages/latin_conf/tokenizer.py` & `loquax-0.1.4/loquax/languages/latin_conf/tokenizer.py`

 * *Files identical despite different names*

### Comparing `loquax-0.1.3/loquax/text_processing/commons.py` & `loquax-0.1.4/loquax/text_processing/commons.py`

 * *Files identical despite different names*

### Comparing `loquax-0.1.3/loquax/text_processing/processing.py` & `loquax-0.1.4/loquax/text_processing/processing.py`

 * *Files 0% similar despite different names*

```diff
@@ -53,15 +53,15 @@
 class Document:
     """
     Class to represent a text or sequence of tokens.
     """
 
     val: str
     language: Language
-    max_line_width = 90  # change this as per your requirement
+    max_line_width: int = 90  # change this as per your requirement
 
     @property
     def tokens(self) -> List[Token]:
         return [
             Token(token, self.language)
             for token in self.language.tokenizer.tokenize(self.val)
         ]
```

### Comparing `loquax-0.1.3/loquax.egg-info/PKG-INFO` & `loquax-0.1.4/loquax.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: loquax
-Version: 0.1.3
+Version: 0.1.4
 Summary: A Classical Phonology framework
 Home-page: https://github.com/mattlianje/loquax
 Author: Matthieu Court
 Author-email: matthieu.court@protonmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: loquax Version: 0.1.3 Summary: A Classical
+Metadata-Version: 2.1 Name: loquax Version: 0.1.4 Summary: A Classical
 Phonology framework Home-page: https://github.com/mattlianje/loquax Author:
 Matthieu Court Author-email: matthieu.court@protonmail.com License: UNKNOWN
 Platform: UNKNOWN Classifier: Development Status :: 3 - Alpha Classifier:
 Intended Audience :: Science/Research Classifier: License :: OSI Approved ::
 GNU General Public License v3 (GPLv3) Classifier: Programming Language ::
 Python :: 3.10 Requires-Python: >=3.10 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `loquax-0.1.3/loquax.egg-info/SOURCES.txt` & `loquax-0.1.4/loquax.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `loquax-0.1.3/setup.py` & `loquax-0.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="loquax",
-    version="0.1.3",
+    version="0.1.4",
     author="Matthieu Court",
     author_email="matthieu.court@protonmail.com",
     description="A Classical Phonology framework",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/mattlianje/loquax",
     packages=find_packages(exclude=['tests', 'tests.*']),
```

