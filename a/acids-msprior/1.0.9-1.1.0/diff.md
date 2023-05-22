# Comparing `tmp/acids-msprior-1.0.9.tar.gz` & `tmp/acids-msprior-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "acids-msprior-1.0.9.tar", last modified: Mon May 15 20:47:04 2023, max compression
+gzip compressed data, was "acids-msprior-1.1.0.tar", last modified: Mon May 22 12:04:36 2023, max compression
```

## Comparing `acids-msprior-1.0.9.tar` & `acids-msprior-1.1.0.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:47:04.676706 acids-msprior-1.0.9/
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-15 20:43:44.000000 acids-msprior-1.0.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-05-15 20:47:04.676706 acids-msprior-1.0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2689 2023-05-15 20:43:44.000000 acids-msprior-1.0.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:47:04.672706 acids-msprior-1.0.9/acids_msprior.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-05-15 20:47:04.000000 acids-msprior-1.0.9/acids_msprior.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-05-15 20:47:04.000000 acids-msprior-1.0.9/acids_msprior.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 20:47:04.000000 acids-msprior-1.0.9/acids_msprior.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-15 20:47:04.000000 acids-msprior-1.0.9/acids_msprior.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-05-15 20:47:04.000000 acids-msprior-1.0.9/acids_msprior.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-15 20:47:04.000000 acids-msprior-1.0.9/acids_msprior.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:47:04.672706 acids-msprior-1.0.9/msprior/
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-05-15 20:43:44.000000 acids-msprior-1.0.9/msprior/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19972 2023-05-15 20:43:44.000000 acids-msprior-1.0.9/msprior/attention.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:47:04.672706 acids-msprior-1.0.9/msprior/configs/
--rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-05-15 20:43:44.000000 acids-msprior-1.0.9/msprior/configs/decoder_only.gin
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-05-15 20:43:44.000000 acids-msprior-1.0.9/msprior/configs/encoder_decoder.gin
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-05-15 20:43:44.000000 acids-msprior-1.0.9/msprior/configs/encoder_decoder_continuous.gin
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-05-15 20:43:44.000000 acids-msprior-1.0.9/msprior/configs/recurrent.gin
--rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-05-15 20:43:44.000000 acids-msprior-1.0.9/msprior/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     4989 2023-05-15 20:43:44.000000 acids-msprior-1.0.9/msprior/preprocessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     9969 2023-05-15 20:43:44.000000 acids-msprior-1.0.9/msprior/scripted.py
--rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-05-15 20:43:44.000000 acids-msprior-1.0.9/msprior/task.py
--rw-r--r--   0 runner    (1001) docker     (123)     6325 2023-05-15 20:43:44.000000 acids-msprior-1.0.9/msprior/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:47:04.676706 acids-msprior-1.0.9/msprior_scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 20:43:44.000000 acids-msprior-1.0.9/msprior_scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-05-15 20:43:44.000000 acids-msprior-1.0.9/msprior_scripts/compact.py
--rw-r--r--   0 runner    (1001) docker     (123)      826 2023-05-15 20:43:44.000000 acids-msprior-1.0.9/msprior_scripts/export.py
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-05-15 20:43:44.000000 acids-msprior-1.0.9/msprior_scripts/main_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     6808 2023-05-15 20:43:44.000000 acids-msprior-1.0.9/msprior_scripts/preprocess.py
--rw-r--r--   0 runner    (1001) docker     (123)     4227 2023-05-15 20:43:44.000000 acids-msprior-1.0.9/msprior_scripts/train.py
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-05-15 20:43:44.000000 acids-msprior-1.0.9/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 20:47:04.676706 acids-msprior-1.0.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-05-15 20:43:44.000000 acids-msprior-1.0.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:47:04.676706 acids-msprior-1.0.9/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 20:43:44.000000 acids-msprior-1.0.9/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-05-15 20:43:44.000000 acids-msprior-1.0.9/tests/test_attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     5806 2023-05-15 20:43:44.000000 acids-msprior-1.0.9/tests/test_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-05-15 20:43:44.000000 acids-msprior-1.0.9/tests/test_configs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 12:04:36.407917 acids-msprior-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-22 12:01:21.000000 acids-msprior-1.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3318 2023-05-22 12:04:36.407917 acids-msprior-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2921 2023-05-22 12:01:21.000000 acids-msprior-1.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 12:04:36.399917 acids-msprior-1.1.0/acids_msprior.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3318 2023-05-22 12:04:36.000000 acids-msprior-1.1.0/acids_msprior.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-05-22 12:04:36.000000 acids-msprior-1.1.0/acids_msprior.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 12:04:36.000000 acids-msprior-1.1.0/acids_msprior.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-22 12:04:36.000000 acids-msprior-1.1.0/acids_msprior.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-05-22 12:04:36.000000 acids-msprior-1.1.0/acids_msprior.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-22 12:04:36.000000 acids-msprior-1.1.0/acids_msprior.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 12:04:36.403917 acids-msprior-1.1.0/msprior/
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-05-22 12:01:21.000000 acids-msprior-1.1.0/msprior/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19972 2023-05-22 12:01:21.000000 acids-msprior-1.1.0/msprior/attention.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 12:04:36.403917 acids-msprior-1.1.0/msprior/configs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-05-22 12:01:21.000000 acids-msprior-1.1.0/msprior/configs/decoder_only.gin
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-05-22 12:01:21.000000 acids-msprior-1.1.0/msprior/configs/encoder_decoder.gin
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-05-22 12:01:21.000000 acids-msprior-1.1.0/msprior/configs/encoder_decoder_continuous.gin
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-05-22 12:01:21.000000 acids-msprior-1.1.0/msprior/configs/recurrent.gin
+-rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-05-22 12:01:21.000000 acids-msprior-1.1.0/msprior/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4989 2023-05-22 12:01:21.000000 acids-msprior-1.1.0/msprior/preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10561 2023-05-22 12:01:21.000000 acids-msprior-1.1.0/msprior/scripted.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-05-22 12:01:21.000000 acids-msprior-1.1.0/msprior/task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6325 2023-05-22 12:01:21.000000 acids-msprior-1.1.0/msprior/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 12:04:36.407917 acids-msprior-1.1.0/msprior_scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 12:01:21.000000 acids-msprior-1.1.0/msprior_scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-05-22 12:01:21.000000 acids-msprior-1.1.0/msprior_scripts/compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-05-22 12:01:21.000000 acids-msprior-1.1.0/msprior_scripts/export.py
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-05-22 12:01:21.000000 acids-msprior-1.1.0/msprior_scripts/main_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6808 2023-05-22 12:01:21.000000 acids-msprior-1.1.0/msprior_scripts/preprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4227 2023-05-22 12:01:21.000000 acids-msprior-1.1.0/msprior_scripts/train.py
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-05-22 12:01:21.000000 acids-msprior-1.1.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 12:04:36.407917 acids-msprior-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-05-22 12:01:21.000000 acids-msprior-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 12:04:36.407917 acids-msprior-1.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 12:01:21.000000 acids-msprior-1.1.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-05-22 12:01:21.000000 acids-msprior-1.1.0/tests/test_attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5806 2023-05-22 12:01:21.000000 acids-msprior-1.1.0/tests/test_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-05-22 12:01:21.000000 acids-msprior-1.1.0/tests/test_configs.py
```

### Comparing `acids-msprior-1.0.9/PKG-INFO` & `acids-msprior-1.1.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: acids-msprior
-Version: 1.0.9
+Version: 1.1.0
 Summary: MSPRIOR: A multiscale prior model for realtime temporal learning
 Author: Antoine CAILLON
 Author-email: caillon@ircam.fr
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
@@ -86,14 +86,22 @@
 
 Export your model to a `.ts` file that you can load inside the [nn~ external for Max/MSP and PureData](https://github.com/acids-ircam/nn_tilde).
 
 ```bash
 msprior export --run /path/to/your/run
 ```
 
+**WARNING**
+
+If you are training on top of a *continuous* rave (i.e. anything but the `discrete` configuration), you shoud pass the `--continuous` flag during export
+
+```bash
+msprior export --run /path/to/your/run --continuous
+```
+
 ### 4. Realtime usage
 
 Once exported, you can load the model inside MaxMSP following the image below.
 
 ![Max Msp usage](docs/maxmsp_usage.png)
 
 Note that additional inputs (e.g. semantic) are only available when using seq2seq models. The last output yields the perplexity of the model.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: acids-msprior Version: 1.0.9 Summary: MSPRIOR: A
+Metadata-Version: 2.1 Name: acids-msprior Version: 1.1.0 Summary: MSPRIOR: A
 multiscale prior model for realtime temporal learning Author: Antoine CAILLON
 Author-email: caillon@ircam.fr Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: OS Independent Requires-Python: >=3.9 Description-Content-Type: text/
 markdown # MSPrior ### A multi(scale/stream) prior model for realtime temporal
 learning ## Disclaimer This is an experimental project that *will* be subject
 to lots of changes. ## Installation ```bash pip install acids-msprior ``` ##
@@ -33,11 +33,14 @@
 encoder_decoder_continuous on continuous features instead of a discrete token
                            sequence.
 The configurations `decoder_only` and `recurrent` are readily usable, the
 seq2seq variants depends on another project called `rave2vec` that will be open
 sourced in the near future. ### 3. Export Export your model to a `.ts` file
 that you can load inside the [nn~ external for Max/MSP and PureData](https://
 github.com/acids-ircam/nn_tilde). ```bash msprior export --run /path/to/your/
-run ``` ### 4. Realtime usage Once exported, you can load the model inside
-MaxMSP following the image below. ![Max Msp usage](docs/maxmsp_usage.png) Note
-that additional inputs (e.g. semantic) are only available when using seq2seq
-models. The last output yields the perplexity of the model.
+run ``` **WARNING** If you are training on top of a *continuous* rave (i.e.
+anything but the `discrete` configuration), you shoud pass the `--continuous`
+flag during export ```bash msprior export --run /path/to/your/run --continuous
+``` ### 4. Realtime usage Once exported, you can load the model inside MaxMSP
+following the image below. ![Max Msp usage](docs/maxmsp_usage.png) Note that
+additional inputs (e.g. semantic) are only available when using seq2seq models.
+The last output yields the perplexity of the model.
```

### Comparing `acids-msprior-1.0.9/README.md` & `acids-msprior-1.1.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -74,14 +74,22 @@
 
 Export your model to a `.ts` file that you can load inside the [nn~ external for Max/MSP and PureData](https://github.com/acids-ircam/nn_tilde).
 
 ```bash
 msprior export --run /path/to/your/run
 ```
 
+**WARNING**
+
+If you are training on top of a *continuous* rave (i.e. anything but the `discrete` configuration), you shoud pass the `--continuous` flag during export
+
+```bash
+msprior export --run /path/to/your/run --continuous
+```
+
 ### 4. Realtime usage
 
 Once exported, you can load the model inside MaxMSP following the image below.
 
 ![Max Msp usage](docs/maxmsp_usage.png)
 
 Note that additional inputs (e.g. semantic) are only available when using seq2seq models. The last output yields the perplexity of the model.
```

#### html2text {}

```diff
@@ -28,11 +28,14 @@
 encoder_decoder_continuous on continuous features instead of a discrete token
                            sequence.
 The configurations `decoder_only` and `recurrent` are readily usable, the
 seq2seq variants depends on another project called `rave2vec` that will be open
 sourced in the near future. ### 3. Export Export your model to a `.ts` file
 that you can load inside the [nn~ external for Max/MSP and PureData](https://
 github.com/acids-ircam/nn_tilde). ```bash msprior export --run /path/to/your/
-run ``` ### 4. Realtime usage Once exported, you can load the model inside
-MaxMSP following the image below. ![Max Msp usage](docs/maxmsp_usage.png) Note
-that additional inputs (e.g. semantic) are only available when using seq2seq
-models. The last output yields the perplexity of the model.
+run ``` **WARNING** If you are training on top of a *continuous* rave (i.e.
+anything but the `discrete` configuration), you shoud pass the `--continuous`
+flag during export ```bash msprior export --run /path/to/your/run --continuous
+``` ### 4. Realtime usage Once exported, you can load the model inside MaxMSP
+following the image below. ![Max Msp usage](docs/maxmsp_usage.png) Note that
+additional inputs (e.g. semantic) are only available when using seq2seq models.
+The last output yields the perplexity of the model.
```

### Comparing `acids-msprior-1.0.9/acids_msprior.egg-info/PKG-INFO` & `acids-msprior-1.1.0/acids_msprior.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: acids-msprior
-Version: 1.0.9
+Version: 1.1.0
 Summary: MSPRIOR: A multiscale prior model for realtime temporal learning
 Author: Antoine CAILLON
 Author-email: caillon@ircam.fr
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
@@ -86,14 +86,22 @@
 
 Export your model to a `.ts` file that you can load inside the [nn~ external for Max/MSP and PureData](https://github.com/acids-ircam/nn_tilde).
 
 ```bash
 msprior export --run /path/to/your/run
 ```
 
+**WARNING**
+
+If you are training on top of a *continuous* rave (i.e. anything but the `discrete` configuration), you shoud pass the `--continuous` flag during export
+
+```bash
+msprior export --run /path/to/your/run --continuous
+```
+
 ### 4. Realtime usage
 
 Once exported, you can load the model inside MaxMSP following the image below.
 
 ![Max Msp usage](docs/maxmsp_usage.png)
 
 Note that additional inputs (e.g. semantic) are only available when using seq2seq models. The last output yields the perplexity of the model.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: acids-msprior Version: 1.0.9 Summary: MSPRIOR: A
+Metadata-Version: 2.1 Name: acids-msprior Version: 1.1.0 Summary: MSPRIOR: A
 multiscale prior model for realtime temporal learning Author: Antoine CAILLON
 Author-email: caillon@ircam.fr Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: OS Independent Requires-Python: >=3.9 Description-Content-Type: text/
 markdown # MSPrior ### A multi(scale/stream) prior model for realtime temporal
 learning ## Disclaimer This is an experimental project that *will* be subject
 to lots of changes. ## Installation ```bash pip install acids-msprior ``` ##
@@ -33,11 +33,14 @@
 encoder_decoder_continuous on continuous features instead of a discrete token
                            sequence.
 The configurations `decoder_only` and `recurrent` are readily usable, the
 seq2seq variants depends on another project called `rave2vec` that will be open
 sourced in the near future. ### 3. Export Export your model to a `.ts` file
 that you can load inside the [nn~ external for Max/MSP and PureData](https://
 github.com/acids-ircam/nn_tilde). ```bash msprior export --run /path/to/your/
-run ``` ### 4. Realtime usage Once exported, you can load the model inside
-MaxMSP following the image below. ![Max Msp usage](docs/maxmsp_usage.png) Note
-that additional inputs (e.g. semantic) are only available when using seq2seq
-models. The last output yields the perplexity of the model.
+run ``` **WARNING** If you are training on top of a *continuous* rave (i.e.
+anything but the `discrete` configuration), you shoud pass the `--continuous`
+flag during export ```bash msprior export --run /path/to/your/run --continuous
+``` ### 4. Realtime usage Once exported, you can load the model inside MaxMSP
+following the image below. ![Max Msp usage](docs/maxmsp_usage.png) Note that
+additional inputs (e.g. semantic) are only available when using seq2seq models.
+The last output yields the perplexity of the model.
```

### Comparing `acids-msprior-1.0.9/acids_msprior.egg-info/SOURCES.txt` & `acids-msprior-1.1.0/acids_msprior.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `acids-msprior-1.0.9/msprior/attention.py` & `acids-msprior-1.1.0/msprior/attention.py`

 * *Files identical despite different names*

### Comparing `acids-msprior-1.0.9/msprior/configs/decoder_only.gin` & `acids-msprior-1.1.0/msprior/configs/decoder_only.gin`

 * *Files identical despite different names*

### Comparing `acids-msprior-1.0.9/msprior/configs/encoder_decoder.gin` & `acids-msprior-1.1.0/msprior/configs/encoder_decoder.gin`

 * *Files identical despite different names*

### Comparing `acids-msprior-1.0.9/msprior/configs/encoder_decoder_continuous.gin` & `acids-msprior-1.1.0/msprior/configs/encoder_decoder_continuous.gin`

 * *Files identical despite different names*

### Comparing `acids-msprior-1.0.9/msprior/dataset.py` & `acids-msprior-1.1.0/msprior/dataset.py`

 * *Files identical despite different names*

### Comparing `acids-msprior-1.0.9/msprior/preprocessor.py` & `acids-msprior-1.1.0/msprior/preprocessor.py`

 * *Files identical despite different names*

### Comparing `acids-msprior-1.0.9/msprior/scripted.py` & `acids-msprior-1.1.0/msprior/scripted.py`

 * *Files 7% similar despite different names*

```diff
@@ -120,15 +120,16 @@
                 1,
                 self.num_rave_quantizers,
             ),
         )
 
         self.register_attribute("temperature", 1.)
         self.register_attribute("listen", initial_listen)
-        self.register_attribute("reset", True)
+        self.register_attribute("learn_context", False)
+        self.register_attribute("reset", False)
 
         self.register_method(
             "forward",
             num_inputs,
             temporal_ratio,
             self.num_rave_quantizers + 1,
             temporal_ratio,
@@ -142,14 +143,20 @@
                 "dummy_method",
                 1,
                 self.encoder_ratio * temporal_ratio,
                 1,
                 self.encoder_ratio * temporal_ratio,
             )
 
+    def apply_full_reset(self):
+        for n, b in self.named_buffers():
+            if "_cache_length" in n or "_relative_index" in n or "_state" in n:
+                b.zero_()
+        self.set_reset(False)
+
     def forward(self, x: torch.Tensor) -> torch.Tensor:
         batch_size = x.shape[0]
         input_rave = x[:, :self.num_rave_quantizers]
 
         if self.from_continuous:
             input_rave = self.quantize(input_rave)
 
@@ -157,18 +164,15 @@
             input_rave,
             min=0,
             max=self.num_tokens,
         ).long()
         input_rave = input_rave.permute(0, 2, 1)
 
         if self.reset[0]:
-            for n, b in self.named_buffers():
-                if "_cache_length" in n or "_relative_index" in n or "_state" in n:
-                    b.zero_()
-            self.set_reset(False)
+            self.apply_full_reset()
 
         if self.has_encoder:
             assert hasattr(self, "encoder_ratio")
             if self.encoder_input_type == "discrete":
                 semantic_tokens = x[:, self.num_rave_quantizers:]
                 semantic_tokens = semantic_tokens.reshape(
                     batch_size,
@@ -186,17 +190,26 @@
                 assert self.feature_vae is not None
                 latents = x[:, self.num_rave_quantizers:]
                 latents = latents.reshape(
                     batch_size,
                     latents.shape[1],
                     -1,
                     self.encoder_ratio,
-                )[..., -1]
-                features = self.feature_vae(latents).permute(0, 2, 1)
+                )[..., -1].permute(0, 2, 1)
+
+                if self.learn_context[0]:
+                    features = self.feature_vae.decode(
+                        latents,
+                        context=input_rave,
+                    )
+                else:
+                    features = self.feature_vae.decode(latents)
+
                 encoder_out = self.encoder(features)
+
             elif self.encoder_input_type == "full":
                 features = x[:, self.num_rave_quantizers:]
                 features = features.reshape(
                     batch_size,
                     features.shape[1],
                     -1,
                     self.encoder_ratio,
@@ -288,14 +301,23 @@
 
     @torch.jit.export
     def set_listen(self, listen: bool) -> int:
         self.listen = (listen, )
         return 0
 
     @torch.jit.export
+    def get_learn_context(self) -> bool:
+        return self.learn_context[0]
+
+    @torch.jit.export
+    def set_learn_context(self, learn_context: bool) -> int:
+        self.learn_context = (learn_context, )
+        return 0
+
+    @torch.jit.export
     def get_reset(self) -> bool:
         return self.reset[0]
 
     @torch.jit.export
     def set_reset(self, reset: bool) -> int:
         self.reset = (reset, )
         return 0
```

### Comparing `acids-msprior-1.0.9/msprior/task.py` & `acids-msprior-1.1.0/msprior/task.py`

 * *Files identical despite different names*

### Comparing `acids-msprior-1.0.9/msprior/utils.py` & `acids-msprior-1.1.0/msprior/utils.py`

 * *Files identical despite different names*

### Comparing `acids-msprior-1.0.9/msprior_scripts/compact.py` & `acids-msprior-1.1.0/msprior_scripts/compact.py`

 * *Files identical despite different names*

### Comparing `acids-msprior-1.0.9/msprior_scripts/main_cli.py` & `acids-msprior-1.1.0/msprior_scripts/main_cli.py`

 * *Files identical despite different names*

### Comparing `acids-msprior-1.0.9/msprior_scripts/preprocess.py` & `acids-msprior-1.1.0/msprior_scripts/preprocess.py`

 * *Files identical despite different names*

### Comparing `acids-msprior-1.0.9/msprior_scripts/train.py` & `acids-msprior-1.1.0/msprior_scripts/train.py`

 * *Files identical despite different names*

### Comparing `acids-msprior-1.0.9/setup.py` & `acids-msprior-1.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `acids-msprior-1.0.9/tests/test_attention.py` & `acids-msprior-1.1.0/tests/test_attention.py`

 * *Files identical despite different names*

### Comparing `acids-msprior-1.0.9/tests/test_cache.py` & `acids-msprior-1.1.0/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `acids-msprior-1.0.9/tests/test_configs.py` & `acids-msprior-1.1.0/tests/test_configs.py`

 * *Files identical despite different names*

