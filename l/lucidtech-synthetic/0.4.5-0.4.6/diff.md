# Comparing `tmp/lucidtech-synthetic-0.4.5.tar.gz` & `tmp/lucidtech-synthetic-0.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lucidtech-synthetic-0.4.5.tar", last modified: Wed Dec  7 14:53:27 2022, max compression
+gzip compressed data, was "lucidtech-synthetic-0.4.6.tar", last modified: Mon May 22 13:47:28 2023, max compression
```

## Comparing `lucidtech-synthetic-0.4.5.tar` & `lucidtech-synthetic-0.4.6.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-07 14:53:27.599921 lucidtech-synthetic-0.4.5/
--rw-r--r--   0 runner    (1001) docker     (123)    11349 2022-12-07 14:53:19.000000 lucidtech-synthetic-0.4.5/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)       83 2022-12-07 14:53:19.000000 lucidtech-synthetic-0.4.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5105 2022-12-07 14:53:27.599921 lucidtech-synthetic-0.4.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4279 2022-12-07 14:53:19.000000 lucidtech-synthetic-0.4.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-07 14:53:27.595921 lucidtech-synthetic-0.4.5/lucidtech_synthetic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5105 2022-12-07 14:53:27.000000 lucidtech-synthetic-0.4.5/lucidtech_synthetic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      609 2022-12-07 14:53:27.000000 lucidtech-synthetic-0.4.5/lucidtech_synthetic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-07 14:53:27.000000 lucidtech-synthetic-0.4.5/lucidtech_synthetic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2022-12-07 14:53:27.000000 lucidtech-synthetic-0.4.5/lucidtech_synthetic.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      220 2022-12-07 14:53:27.000000 lucidtech-synthetic-0.4.5/lucidtech_synthetic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2022-12-07 14:53:27.000000 lucidtech-synthetic-0.4.5/lucidtech_synthetic.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      219 2022-12-07 14:53:19.000000 lucidtech-synthetic-0.4.5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       67 2022-12-07 14:53:27.599921 lucidtech-synthetic-0.4.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1478 2022-12-07 14:53:19.000000 lucidtech-synthetic-0.4.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-07 14:53:27.599921 lucidtech-synthetic-0.4.5/synthetic/
--rw-r--r--   0 runner    (1001) docker     (123)       78 2022-12-07 14:53:19.000000 lucidtech-synthetic-0.4.5/synthetic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4879 2022-12-07 14:53:19.000000 lucidtech-synthetic-0.4.5/synthetic/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      383 2022-12-07 14:53:19.000000 lucidtech-synthetic-0.4.5/synthetic/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-07 14:53:27.599921 lucidtech-synthetic-0.4.5/synthetic/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-07 14:53:19.000000 lucidtech-synthetic-0.4.5/synthetic/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5427 2022-12-07 14:53:19.000000 lucidtech-synthetic-0.4.5/synthetic/core/ground_truth.py
--rw-r--r--   0 runner    (1001) docker     (123)      352 2022-12-07 14:53:19.000000 lucidtech-synthetic-0.4.5/synthetic/core/synthesizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3057 2022-12-07 14:53:19.000000 lucidtech-synthetic-0.4.5/synthetic/iterdata.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-07 14:53:27.599921 lucidtech-synthetic-0.4.5/synthetic/pdf/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-07 14:53:19.000000 lucidtech-synthetic-0.4.5/synthetic/pdf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12180 2022-12-07 14:53:19.000000 lucidtech-synthetic-0.4.5/synthetic/pdf/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     4418 2022-12-07 14:53:19.000000 lucidtech-synthetic-0.4.5/synthetic/pdf/synthesizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1362 2022-12-07 14:53:19.000000 lucidtech-synthetic-0.4.5/synthetic/pdf/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:47:28.281624 lucidtech-synthetic-0.4.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    11349 2023-05-22 13:47:15.000000 lucidtech-synthetic-0.4.6/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-22 13:47:15.000000 lucidtech-synthetic-0.4.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5106 2023-05-22 13:47:28.281624 lucidtech-synthetic-0.4.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4279 2023-05-22 13:47:15.000000 lucidtech-synthetic-0.4.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:47:28.277624 lucidtech-synthetic-0.4.6/lucidtech_synthetic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5106 2023-05-22 13:47:28.000000 lucidtech-synthetic-0.4.6/lucidtech_synthetic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-05-22 13:47:28.000000 lucidtech-synthetic-0.4.6/lucidtech_synthetic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 13:47:28.000000 lucidtech-synthetic-0.4.6/lucidtech_synthetic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-22 13:47:28.000000 lucidtech-synthetic-0.4.6/lucidtech_synthetic.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-05-22 13:47:28.000000 lucidtech-synthetic-0.4.6/lucidtech_synthetic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-22 13:47:28.000000 lucidtech-synthetic-0.4.6/lucidtech_synthetic.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-05-22 13:47:15.000000 lucidtech-synthetic-0.4.6/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-22 13:47:28.281624 lucidtech-synthetic-0.4.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-05-22 13:47:15.000000 lucidtech-synthetic-0.4.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:47:28.277624 lucidtech-synthetic-0.4.6/synthetic/
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-22 13:47:15.000000 lucidtech-synthetic-0.4.6/synthetic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4879 2023-05-22 13:47:15.000000 lucidtech-synthetic-0.4.6/synthetic/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-05-22 13:47:15.000000 lucidtech-synthetic-0.4.6/synthetic/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:47:28.281624 lucidtech-synthetic-0.4.6/synthetic/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 13:47:15.000000 lucidtech-synthetic-0.4.6/synthetic/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5427 2023-05-22 13:47:15.000000 lucidtech-synthetic-0.4.6/synthetic/core/ground_truth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-05-22 13:47:15.000000 lucidtech-synthetic-0.4.6/synthetic/core/synthesizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3057 2023-05-22 13:47:15.000000 lucidtech-synthetic-0.4.6/synthetic/iterdata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:47:28.281624 lucidtech-synthetic-0.4.6/synthetic/pdf/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 13:47:15.000000 lucidtech-synthetic-0.4.6/synthetic/pdf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12195 2023-05-22 13:47:15.000000 lucidtech-synthetic-0.4.6/synthetic/pdf/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4418 2023-05-22 13:47:15.000000 lucidtech-synthetic-0.4.6/synthetic/pdf/synthesizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-05-22 13:47:15.000000 lucidtech-synthetic-0.4.6/synthetic/pdf/utils.py
```

### Comparing `lucidtech-synthetic-0.4.5/LICENSE.md` & `lucidtech-synthetic-0.4.6/LICENSE.md`

 * *Files identical despite different names*

### Comparing `lucidtech-synthetic-0.4.5/PKG-INFO` & `lucidtech-synthetic-0.4.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: lucidtech-synthetic
-Version: 0.4.5
+Version: 0.4.6
 Summary: PDF anonymizer/synthesizer for Cradl
 Home-page: https://github.com/LucidtechAI/synthetic
 Author: Lucidtech
 Author-email: hello@lucidtech.ai
 Maintainer: August Kvernmo
 Maintainer-email: august@lucidtech.ai
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
 # Image/PDF synthesizer for Cradl
 
 ![Github Actions build status](https://github.com/LucidtechAI/synthetic/actions/workflows/pipeline.yaml/badge.svg)
```

### Comparing `lucidtech-synthetic-0.4.5/README.md` & `lucidtech-synthetic-0.4.6/README.md`

 * *Files identical despite different names*

### Comparing `lucidtech-synthetic-0.4.5/lucidtech_synthetic.egg-info/PKG-INFO` & `lucidtech-synthetic-0.4.6/lucidtech_synthetic.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: lucidtech-synthetic
-Version: 0.4.5
+Version: 0.4.6
 Summary: PDF anonymizer/synthesizer for Cradl
 Home-page: https://github.com/LucidtechAI/synthetic
 Author: Lucidtech
 Author-email: hello@lucidtech.ai
 Maintainer: August Kvernmo
 Maintainer-email: august@lucidtech.ai
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
 # Image/PDF synthesizer for Cradl
 
 ![Github Actions build status](https://github.com/LucidtechAI/synthetic/actions/workflows/pipeline.yaml/badge.svg)
```

### Comparing `lucidtech-synthetic-0.4.5/lucidtech_synthetic.egg-info/SOURCES.txt` & `lucidtech-synthetic-0.4.6/lucidtech_synthetic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lucidtech-synthetic-0.4.5/setup.py` & `lucidtech-synthetic-0.4.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,14 +40,14 @@
     install_requires=install_requires,
     platforms='Posix; MacOS X; Windows',
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: Apache Software License',
         'Operating System :: OS Independent',
-        'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
         'Topic :: Internet'
     ]
 )
```

### Comparing `lucidtech-synthetic-0.4.5/synthetic/__main__.py` & `lucidtech-synthetic-0.4.6/synthetic/__main__.py`

 * *Files identical despite different names*

### Comparing `lucidtech-synthetic-0.4.5/synthetic/core/ground_truth.py` & `lucidtech-synthetic-0.4.6/synthetic/core/ground_truth.py`

 * *Files identical despite different names*

### Comparing `lucidtech-synthetic-0.4.5/synthetic/iterdata.py` & `lucidtech-synthetic-0.4.6/synthetic/iterdata.py`

 * *Files identical despite different names*

### Comparing `lucidtech-synthetic-0.4.5/synthetic/pdf/parser.py` & `lucidtech-synthetic-0.4.6/synthetic/pdf/parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -340,15 +340,15 @@
                 status = f'Successfully synthesized {name}'
             except HasFormException:
                 logger.error('Failed to get rid of forms in flattened PDF')
             except Exception as e:
                 logger.exception(e)
                 logger.error(f'Error when synthesizing {name}')
             finally:
-                flattened_pdf_file.unlink()
+                flattened_pdf_file.unlink(missing_ok=True)
     except AlreadyProcessed as e:
         logger.warning(e)
     except (FileNotFoundError, NoTextException, TooManyFontsException, TooManyPagesException, TooManySingleChars) as e:
         logger.error(e)
     except TimeoutError:
         logger.error(f'Synthesizing timed out, took longer than {timeout_in_seconds}s')
     except Exception as e:
```

### Comparing `lucidtech-synthetic-0.4.5/synthetic/pdf/synthesizer.py` & `lucidtech-synthetic-0.4.6/synthetic/pdf/synthesizer.py`

 * *Files identical despite different names*

### Comparing `lucidtech-synthetic-0.4.5/synthetic/pdf/utils.py` & `lucidtech-synthetic-0.4.6/synthetic/pdf/utils.py`

 * *Files identical despite different names*

