# Comparing `tmp/abba_python-0.1.9.tar.gz` & `tmp/abba_python-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\nicol\Dropbox\BIOP\abba_python\dist\.tmp-o61xhnfs\abba_python-0.1.9.tar", last modified: Tue May  2 13:11:01 2023, max compression
+gzip compressed data, was "C:\Users\nicol\Dropbox\BIOP\abba_python\dist\.tmp-2ftz5zrf\abba_python-0.2.0.tar", last modified: Mon May 22 14:31:52 2023, max compression
```

## Comparing `abba_python-0.1.9.tar` & `abba_python-0.2.0.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxrwxrwx   0        0        0        0 2023-05-02 13:11:01.000000 abba_python-0.1.9/
--rw-rw-rw-   0        0        0      172 2023-03-22 13:49:35.000000 abba_python-0.1.9/AUTHORS.rst
--rw-rw-rw-   0        0        0     3575 2023-03-22 13:49:35.000000 abba_python-0.1.9/CONTRIBUTING.rst
--rw-rw-rw-   0        0        0       89 2023-03-22 13:49:35.000000 abba_python-0.1.9/HISTORY.rst
--rw-rw-rw-   0        0        0     1578 2023-03-22 13:49:35.000000 abba_python-0.1.9/LICENSE
--rw-rw-rw-   0        0        0      334 2023-03-22 14:16:42.000000 abba_python-0.1.9/MANIFEST.in
--rw-rw-rw-   0        0        0     1876 2023-05-02 13:11:01.000000 abba_python-0.1.9/PKG-INFO
--rw-rw-rw-   0        0        0      934 2023-03-22 13:49:35.000000 abba_python-0.1.9/README.rst
-drwxrwxrwx   0        0        0        0 2023-05-02 13:11:01.000000 abba_python-0.1.9/docs/
--rw-rw-rw-   0        0        0      612 2023-03-22 13:49:35.000000 abba_python-0.1.9/docs/Makefile
--rw-rw-rw-   0        0        0       28 2023-03-22 13:49:35.000000 abba_python-0.1.9/docs/authors.rst
--rw-rw-rw-   0        0        0     4860 2023-03-22 15:57:33.000000 abba_python-0.1.9/docs/conf.py
--rw-rw-rw-   0        0        0       33 2023-03-22 13:49:35.000000 abba_python-0.1.9/docs/contributing.rst
--rw-rw-rw-   0        0        0       28 2023-03-22 13:49:35.000000 abba_python-0.1.9/docs/history.rst
--rw-rw-rw-   0        0        0      308 2023-03-22 13:49:35.000000 abba_python-0.1.9/docs/index.rst
--rw-rw-rw-   0        0        0     1150 2023-03-22 13:49:35.000000 abba_python-0.1.9/docs/installation.rst
--rwxrwxrwx   0        0        0      809 2023-03-22 13:49:35.000000 abba_python-0.1.9/docs/make.bat
--rw-rw-rw-   0        0        0       27 2023-03-22 13:49:35.000000 abba_python-0.1.9/docs/readme.rst
--rw-rw-rw-   0        0        0       77 2023-03-22 13:49:35.000000 abba_python-0.1.9/docs/usage.rst
--rw-rw-rw-   0        0        0      640 2023-05-02 13:11:01.000000 abba_python-0.1.9/setup.cfg
--rw-rw-rw-   0        0        0     1406 2023-05-02 13:08:31.000000 abba_python-0.1.9/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-02 13:11:01.000000 abba_python-0.1.9/src/
-drwxrwxrwx   0        0        0        0 2023-05-02 13:11:01.000000 abba_python-0.1.9/src/abba_python/
--rw-rw-rw-   0        0        0      331 2023-05-02 13:08:31.000000 abba_python-0.1.9/src/abba_python/__init__.py
--rw-rw-rw-   0        0        0    41581 2023-05-02 13:07:37.000000 abba_python-0.1.9/src/abba_python/abba.py
-drwxrwxrwx   0        0        0        0 2023-05-02 13:11:01.000000 abba_python-0.1.9/src/abba_python/abba_private/
--rw-rw-rw-   0        0        0     1858 2023-05-01 16:24:09.000000 abba_python-0.1.9/src/abba_python/abba_private/AbbaAtlas.py
--rw-rw-rw-   0        0        0     5818 2023-02-27 12:29:23.000000 abba_python-0.1.9/src/abba_python/abba_private/AbbaMap.py
--rw-rw-rw-   0        0        0     2160 2023-02-13 22:05:24.000000 abba_python-0.1.9/src/abba_python/abba_private/AbbaOntology.py
--rw-rw-rw-   0        0        0     2307 2023-05-02 06:35:59.000000 abba_python-0.1.9/src/abba_python/abba_private/DeepSliceProcessor.py
--rw-rw-rw-   0        0        0      297 2023-05-01 16:21:57.000000 abba_python-0.1.9/src/abba_python/abba_private/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-02 13:11:01.000000 abba_python-0.1.9/src/abba_python/itk/
--rw-rw-rw-   0        0        0      169 2022-11-03 07:00:45.000000 abba_python-0.1.9/src/abba_python/itk/__init__.py
--rw-rw-rw-   0        0        0     5138 2023-03-22 15:57:33.000000 abba_python-0.1.9/src/abba_python/itk/abba_itk.py
--rw-rw-rw-   0        0        0     2820 2023-05-01 16:15:35.000000 abba_python-0.1.9/src/abba_python/run-abba-local-fiji.py
--rw-rw-rw-   0        0        0     1232 2023-05-02 06:30:49.000000 abba_python-0.1.9/src/abba_python/run-abba.py
-drwxrwxrwx   0        0        0        0 2023-05-02 13:11:01.000000 abba_python-0.1.9/src/abba_python/scijava_python_command/
--rw-rw-rw-   0        0        0      105 2023-05-01 16:12:25.000000 abba_python-0.1.9/src/abba_python/scijava_python_command/__init__.py
--rw-rw-rw-   0        0        0     6690 2022-10-18 16:35:14.000000 abba_python-0.1.9/src/abba_python/scijava_python_command/command.py
--rw-rw-rw-   0        0        0     9554 2022-11-01 21:20:40.000000 abba_python-0.1.9/src/abba_python/scijava_python_command/jupyter_ui.py
--rw-rw-rw-   0        0        0      592 2022-11-01 20:18:37.000000 abba_python-0.1.9/src/abba_python/scijava_python_command/magic.py
-drwxrwxrwx   0        0        0        0 2023-05-02 13:11:01.000000 abba_python-0.1.9/src/abba_python.egg-info/
--rw-rw-rw-   0        0        0     1876 2023-05-02 13:11:01.000000 abba_python-0.1.9/src/abba_python.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1135 2023-05-02 13:11:01.000000 abba_python-0.1.9/src/abba_python.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-02 13:11:01.000000 abba_python-0.1.9/src/abba_python.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-03-22 16:13:55.000000 abba_python-0.1.9/src/abba_python.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       51 2023-05-02 13:11:01.000000 abba_python-0.1.9/src/abba_python.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-05-02 13:11:01.000000 abba_python-0.1.9/src/abba_python.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-02 13:11:01.000000 abba_python-0.1.9/tests/
--rw-rw-rw-   0        0        0       41 2023-03-22 13:49:35.000000 abba_python-0.1.9/tests/__init__.py
--rw-rw-rw-   0        0        0      370 2023-03-22 15:57:33.000000 abba_python-0.1.9/tests/test_abba_python.py
+drwxrwxrwx   0        0        0        0 2023-05-22 14:31:52.000000 abba_python-0.2.0/
+-rw-rw-rw-   0        0        0      172 2023-03-22 13:49:35.000000 abba_python-0.2.0/AUTHORS.rst
+-rw-rw-rw-   0        0        0     2385 2023-05-03 06:42:55.000000 abba_python-0.2.0/CONTRIBUTING.rst
+-rw-rw-rw-   0        0        0      157 2023-05-03 11:04:48.000000 abba_python-0.2.0/HISTORY.rst
+-rw-rw-rw-   0        0        0     1578 2023-03-22 13:49:35.000000 abba_python-0.2.0/LICENSE
+-rw-rw-rw-   0        0        0      334 2023-03-22 14:16:42.000000 abba_python-0.2.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     2819 2023-05-22 14:31:52.000000 abba_python-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1786 2023-05-22 14:29:44.000000 abba_python-0.2.0/README.rst
+drwxrwxrwx   0        0        0        0 2023-05-22 14:31:52.000000 abba_python-0.2.0/docs/
+-rw-rw-rw-   0        0        0      612 2023-03-22 13:49:35.000000 abba_python-0.2.0/docs/Makefile
+-rw-rw-rw-   0        0        0       28 2023-03-22 13:49:35.000000 abba_python-0.2.0/docs/authors.rst
+-rw-rw-rw-   0        0        0     4860 2023-03-22 15:57:33.000000 abba_python-0.2.0/docs/conf.py
+-rw-rw-rw-   0        0        0       33 2023-03-22 13:49:35.000000 abba_python-0.2.0/docs/contributing.rst
+-rw-rw-rw-   0        0        0       28 2023-03-22 13:49:35.000000 abba_python-0.2.0/docs/history.rst
+-rw-rw-rw-   0        0        0      308 2023-03-22 13:49:35.000000 abba_python-0.2.0/docs/index.rst
+-rw-rw-rw-   0        0        0     1150 2023-03-22 13:49:35.000000 abba_python-0.2.0/docs/installation.rst
+-rwxrwxrwx   0        0        0      809 2023-03-22 13:49:35.000000 abba_python-0.2.0/docs/make.bat
+-rw-rw-rw-   0        0        0       27 2023-03-22 13:49:35.000000 abba_python-0.2.0/docs/readme.rst
+-rw-rw-rw-   0        0        0       77 2023-03-22 13:49:35.000000 abba_python-0.2.0/docs/usage.rst
+-rw-rw-rw-   0        0        0      640 2023-05-22 14:31:52.000000 abba_python-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0     1406 2023-05-22 14:29:57.000000 abba_python-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-22 14:31:52.000000 abba_python-0.2.0/src/
+drwxrwxrwx   0        0        0        0 2023-05-22 14:31:52.000000 abba_python-0.2.0/src/abba_python/
+-rw-rw-rw-   0        0        0      331 2023-05-22 14:29:57.000000 abba_python-0.2.0/src/abba_python/__init__.py
+-rw-rw-rw-   0        0        0    42230 2023-05-22 14:25:41.000000 abba_python-0.2.0/src/abba_python/abba.py
+drwxrwxrwx   0        0        0        0 2023-05-22 14:31:52.000000 abba_python-0.2.0/src/abba_python/abba_private/
+-rw-rw-rw-   0        0        0     1858 2023-05-01 16:24:09.000000 abba_python-0.2.0/src/abba_python/abba_private/AbbaAtlas.py
+-rw-rw-rw-   0        0        0     5818 2023-02-27 12:29:23.000000 abba_python-0.2.0/src/abba_python/abba_private/AbbaMap.py
+-rw-rw-rw-   0        0        0     2160 2023-02-13 22:05:24.000000 abba_python-0.2.0/src/abba_python/abba_private/AbbaOntology.py
+-rw-rw-rw-   0        0        0     2307 2023-05-02 06:35:59.000000 abba_python-0.2.0/src/abba_python/abba_private/DeepSliceProcessor.py
+-rw-rw-rw-   0        0        0      297 2023-05-01 16:21:57.000000 abba_python-0.2.0/src/abba_python/abba_private/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-22 14:31:52.000000 abba_python-0.2.0/src/abba_python/itk/
+-rw-rw-rw-   0        0        0      169 2022-11-03 07:00:45.000000 abba_python-0.2.0/src/abba_python/itk/__init__.py
+-rw-rw-rw-   0        0        0     5138 2023-03-22 15:57:33.000000 abba_python-0.2.0/src/abba_python/itk/abba_itk.py
+-rw-rw-rw-   0        0        0     2820 2023-05-01 16:15:35.000000 abba_python-0.2.0/src/abba_python/run-abba-local-fiji.py
+-rw-rw-rw-   0        0        0     1232 2023-05-02 06:30:49.000000 abba_python-0.2.0/src/abba_python/run-abba.py
+drwxrwxrwx   0        0        0        0 2023-05-22 14:31:52.000000 abba_python-0.2.0/src/abba_python/scijava_python_command/
+-rw-rw-rw-   0        0        0      105 2023-05-01 16:12:25.000000 abba_python-0.2.0/src/abba_python/scijava_python_command/__init__.py
+-rw-rw-rw-   0        0        0     6690 2022-10-18 16:35:14.000000 abba_python-0.2.0/src/abba_python/scijava_python_command/command.py
+-rw-rw-rw-   0        0        0     9554 2022-11-01 21:20:40.000000 abba_python-0.2.0/src/abba_python/scijava_python_command/jupyter_ui.py
+-rw-rw-rw-   0        0        0      592 2022-11-01 20:18:37.000000 abba_python-0.2.0/src/abba_python/scijava_python_command/magic.py
+drwxrwxrwx   0        0        0        0 2023-05-22 14:31:52.000000 abba_python-0.2.0/src/abba_python.egg-info/
+-rw-rw-rw-   0        0        0     2819 2023-05-22 14:31:52.000000 abba_python-0.2.0/src/abba_python.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1135 2023-05-22 14:31:52.000000 abba_python-0.2.0/src/abba_python.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-22 14:31:52.000000 abba_python-0.2.0/src/abba_python.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-03-22 16:13:55.000000 abba_python-0.2.0/src/abba_python.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       51 2023-05-22 14:31:52.000000 abba_python-0.2.0/src/abba_python.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-05-22 14:31:52.000000 abba_python-0.2.0/src/abba_python.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-22 14:31:52.000000 abba_python-0.2.0/tests/
+-rw-rw-rw-   0        0        0       41 2023-03-22 13:49:35.000000 abba_python-0.2.0/tests/__init__.py
+-rw-rw-rw-   0        0        0      370 2023-03-22 15:57:33.000000 abba_python-0.2.0/tests/test_abba_python.py
```

### Comparing `abba_python-0.1.9/LICENSE` & `abba_python-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `abba_python-0.1.9/docs/Makefile` & `abba_python-0.2.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `abba_python-0.1.9/docs/conf.py` & `abba_python-0.2.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `abba_python-0.1.9/docs/installation.rst` & `abba_python-0.2.0/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `abba_python-0.1.9/docs/make.bat` & `abba_python-0.2.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `abba_python-0.1.9/setup.cfg` & `abba_python-0.2.0/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 0.1.9
+current_version = 0.2.0
 commit = True
 tag = True
 
 [bumpversion:file:setup.py]
 search = version='{current_version}'
 replace = version='{new_version}'
```

### Comparing `abba_python-0.1.9/setup.py` & `abba_python-0.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,10 +35,10 @@
     include_package_data=True,
     keywords='abba_python',
     name='abba_python',
     packages=find_packages(include=['abba_python', 'abba_python.*']),
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/nicoKiaru/abba_python',
-    version='0.1.9',
+    version='0.2.0',
     zip_safe=False,
 )
```

### Comparing `abba_python-0.1.9/src/abba_python/abba.py` & `abba_python-0.2.0/src/abba_python/abba.py`

 * *Files 12% similar despite different names*

```diff
@@ -66,15 +66,15 @@
     Returns the jar files that need to be included into the classpath
     of an imagej object in order to have a functional ABBA app
     these jars should be available in https://maven.scijava.org/
     :return:
     """
     imagej_core_dep = 'net.imagej:imagej:2.9.0'
     imagej_legacy_dep = 'net.imagej:imagej-legacy:0.39.3'
-    abba_dep = 'ch.epfl.biop:ImageToAtlasRegister:0.5.3'
+    abba_dep = 'ch.epfl.biop:ImageToAtlasRegister:0.5.4'
     return [imagej_core_dep, imagej_legacy_dep, abba_dep]
 
 
 def add_brainglobe_atlases(ij):
     # TODO : check connection available or not
     try:
         check_internet_connection()
@@ -145,31 +145,22 @@
                     if str(module.getInfo().getOutput(
                         output_key).getType()) == 'class ch.epfl.biop.atlas.aligner.gui.bdv.BdvMultislicePositionerView':
                         print('MultiSlicePositionerView found')
                         view = module.getOutputs().get(output_key)
                         print(str(view.msp.getAtlas().getName()))
                         if str(view.msp.getAtlas().getName()) == 'Adult Mouse Brain - Allen Brain Atlas V3p1':
                             print('Adult Mouse Brain - Allen Brain Atlas V3p1 detected, installing DeepSlice module')
-                            print('0')
                             BdvScijavaHelper = jimport('sc.fiji.bdvpg.scijava.BdvScijavaHelper')
-                            print('1')
                             from jpype import JImplements, JOverride
-                            print('2')
                             Runnable = jimport('java.lang.Runnable')
-                            print('3')
 
                             class DSPlaceHolder(object):
                                 def __init__(self, ij):
-                                    print('ze temp')
                                     self.temp_folder = prepare_deepslice_temp_folder(self)
-                                    print('alors')
                                     self.ij = ij
-                                    print('heu')
-
-                            print('4')
 
                             @JImplements(Runnable)
                             class ExecuteDeepSlicePython(object):
 
                                 def __init__(self, dsp):
                                     self.dsp = dsp
 
@@ -181,67 +172,65 @@
                                     self.dsp.ij.command().run(RegisterSlicesDeepSliceCommand, True,
                                                               "image_name_prefix", JString('Section'),
                                                               "mp", view.msp,
                                                               "deepSliceProcessor", self.dsp._run_deep_slice,
                                                               "dataset_folder", JString(self.dsp.temp_folder)
                                                               )
 
-                            print('5')
-                            print('ij= '+str(ij))
                             dsplaceholder = DSPlaceHolder(ij)
-                            print('5A')
                             edsp = ExecuteDeepSlicePython(dsplaceholder)
-                            print('5B')
                             bdv_view = view.getBdvh()
-                            print('5C')
 
                             BdvScijavaHelper.addActionToBdvHandleMenu(bdv_view,
                                                                       "Align>ABBA - DeepSlice Registration (Python)", 0,
                                                                       edsp)
-                            print('6')
+
 
     @JImplements(Supplier)
     class IPyWidgetCommandPreprocessorSupplier(object):
         @JOverride
         def get(self):
             return IPyWidgetCommandPostProcessor()
 
     PyPostprocessor.register(IPyWidgetCommandPreprocessorSupplier())
     print('ABBA Python hooks enabled')
 
 
 def prepare_deepslice_temp_folder(self):
-    print('pdtf0')
     if not hasattr(self, '_run_deep_slice'):
-        from src.abba_python.abba_private.DeepSliceProcessor import DeepSliceProcessor
+        try:
+            from abba_python.abba_private.DeepSliceProcessor import \
+                DeepSliceProcessor  # delayed import because the jvm should be set first
+        except:
+            try:
+                from .abba_private.DeepSliceProcessor import \
+                    DeepSliceProcessor  # delayed import because the jvm should be set first
+            except:
+                print("Could not import DeepSliceProcessor because the dev do not understand python modules and submodules.")
+
         self._run_deep_slice = DeepSliceProcessor()
 
-    print('pdtf1')
     # TODO : fix potential multiple running instance issues
     temp_folder = tempfile.gettempdir() + '/temp/deepslice/'
 
-    print('pdtf2')
     # make sure that the folder exists
     if not os.path.exists(temp_folder):
         os.makedirs(temp_folder)
 
-    print('pdtf3')
     # clean folder : remove all previous files
     for filename in os.listdir(temp_folder):
-        print('pdtf3a')
         file_path = os.path.join(temp_folder, filename)
         try:
             if os.path.isfile(file_path) or os.path.islink(file_path):
                 os.unlink(file_path)
             # elif os.path.isdir(file_path):
             #    shutil.rmtree(file_path)
         except Exception as e:
-            print('pdtf3error')
             print('Failed to delete %s. Reason: %s' % (file_path, e))
-    print('pdtf4')
+
     # print('Temp folder = '+str(temp_folder))
     return temp_folder
 
 
 class Abba:
     """Abba object which can be used to register sections to a BrainGlobe atlas object
     Parameters
@@ -309,16 +298,26 @@
             elif atlas_name == 'Rat - Waxholm Sprague Dawley V4p1':
                 WaxholmSpragueDawleyRatV4Command = jimport(
                     'ch.epfl.biop.atlas.rat.waxholm.spraguedawley.v4p1.command.WaxholmSpragueDawleyRatV4p1Command')
                 atlas = ij.command().run(WaxholmSpragueDawleyRatV4Command, True).get().getOutput("ba")
                 Abba.opened_atlases[atlas_name] = atlas
             else:
                 bg_atlas = BrainGlobeAtlas(atlas_name)
-                from src.abba_python.abba_private.AbbaAtlas import \
-                    AbbaAtlas  # delayed import because the jvm should be correctly
+
+                try:
+                    from abba_python.abba_private.AbbaAtlas import \
+                        AbbaAtlas  # delayed import because the jvm should be set first
+                except:
+                    try:
+                        from .abba_private.AbbaAtlas import \
+                            AbbaAtlas  # delayed import because the jvm should be set first
+                    except:
+                        print(
+                            "Could not import DeepSliceProcessor because the dev do not understand python modules and submodules.")
+
                 # initialized
                 atlas = AbbaAtlas(bg_atlas, ij)
                 atlas.initialize(None, None)
                 Abba.opened_atlases[atlas_name] = atlas
                 ij.object().addObject(atlas, atlas_name)  # store it in java's object service
 
         self.atlas = Abba.opened_atlases[atlas_name]
@@ -378,15 +377,15 @@
         class ExecuteDeepSlicePython(object):
 
             def __init__(self, abba):
                 self.abba = abba
 
             @JOverride
             def run(self):
-                temp_folder = self.abba.prepare_deepslice_temp_folder()
+                temp_folder = prepare_deepslice_temp_folder(self)
                 RegisterSlicesDeepSliceCommand = jimport(
                     'ch.epfl.biop.atlas.aligner.command.RegisterSlicesDeepSliceCommand')
                 # Any missing input parameter will lead to a popup window asking the missing argument to the user
                 self.abba.ij.command().run(RegisterSlicesDeepSliceCommand, True,
                                            "image_name_prefix", JString('Section'),
                                            "mp", self.abba.mp,
                                            "deepSliceProcessor", self.abba._run_deep_slice,
@@ -396,38 +395,49 @@
         BdvScijavaHelper.addActionToBdvHandleMenu(self.bdv_view.getBdvh(),
                                                   "Align>ABBA - DeepSlice Registration (Python)", 0,
                                                   ExecuteDeepSlicePython(self))
 
     def get_bdv_view(self):
         return self.bdv_view
 
-    def prepare_deepslice_temp_folder(self):  # TODO : remove
-        if not hasattr(self, '_run_deep_slice'):
-            from src.abba_python.abba_private.DeepSliceProcessor import DeepSliceProcessor
-            self._run_deep_slice = DeepSliceProcessor()
-
-        # TODO : fix potential multiple running instance issues
-        temp_folder = tempfile.gettempdir() + '/temp/deepslice/'
-
-        # make sure that the folder exists
-        if not os.path.exists(temp_folder):
-            os.makedirs(temp_folder)
-
-        # clean folder : remove all previous files
-        for filename in os.listdir(temp_folder):
-            file_path = os.path.join(temp_folder, filename)
-            try:
-                if os.path.isfile(file_path) or os.path.islink(file_path):
-                    os.unlink(file_path)
-                # elif os.path.isdir(file_path):
-                #    shutil.rmtree(file_path)
-            except Exception as e:
-                print('Failed to delete %s. Reason: %s' % (file_path, e))
-        # print('Temp folder = '+str(temp_folder))
-        return temp_folder
+    # def prepare_deepslice_temp_folder(self):  # TODO : remove
+    #
+    #     if not hasattr(self, '_run_deep_slice'):
+    #         try:
+    #             from abba_python.abba_private.DeepSliceProcessor import \
+    #                 DeepSliceProcessor  # delayed import because the jvm should be set first
+    #         except:
+    #             try:
+    #                 from .abba_private.DeepSliceProcessor import \
+    #                     DeepSliceProcessor  # delayed import because the jvm should be set first
+    #             except:
+    #                 print(
+    #                     "Could not import DeepSliceProcessor because the dev do not understand python modules and submodules.")
+    #
+    #     self._run_deep_slice = DeepSliceProcessor()
+    #
+    #     # TODO : fix potential multiple running instance issues
+    #     temp_folder = tempfile.gettempdir() + '/temp/deepslice/'
+    #
+    #     # make sure that the folder exists
+    #     if not os.path.exists(temp_folder):
+    #         os.makedirs(temp_folder)
+    #
+    #     # clean folder : remove all previous files
+    #     for filename in os.listdir(temp_folder):
+    #         file_path = os.path.join(temp_folder, filename)
+    #         try:
+    #             if os.path.isfile(file_path) or os.path.islink(file_path):
+    #                 os.unlink(file_path)
+    #             # elif os.path.isdir(file_path):
+    #             #    shutil.rmtree(file_path)
+    #         except Exception as e:
+    #             print('Failed to delete %s. Reason: %s' % (file_path, e))
+    #     # print('Temp folder = '+str(temp_folder))
+    #     return temp_folder
 
     # ------------------------ IMPORT
     def import_from_files(self, filepaths, z_location=0, z_increment=0.02, split_rgb=False):
         """
 
         :param z_location:
             initial location in mm along the atlas cutting axis
@@ -496,15 +506,15 @@
             print('Deep Slice only support the Allen Brain Atlas CCFv3 in coronal slicing mode')
             return
 
         if not self.slicing_mode == 'coronal':
             print('Deep Slice only support the Allen Brain Atlas CCFv3 in coronal slicing mode')
             return
 
-        temp_folder = self.prepare_deepslice_temp_folder()
+        temp_folder = prepare_deepslice_temp_folder(self)
 
         RegisterSlicesDeepSliceCommand = jimport('ch.epfl.biop.atlas.aligner.command.RegisterSlicesDeepSliceCommand')
 
         # Any missing input parameter will lead to a popup window asking the missing argument to the user
         return self.ij.command().run(RegisterSlicesDeepSliceCommand, True,
                                      "channels", JString(','.join(map(str, channels))),
                                      "image_name_prefix", JString('Section'),
```

### Comparing `abba_python-0.1.9/src/abba_python/abba_private/AbbaAtlas.py` & `abba_python-0.2.0/src/abba_python/abba_private/AbbaAtlas.py`

 * *Files identical despite different names*

### Comparing `abba_python-0.1.9/src/abba_python/abba_private/AbbaMap.py` & `abba_python-0.2.0/src/abba_python/abba_private/AbbaMap.py`

 * *Files identical despite different names*

### Comparing `abba_python-0.1.9/src/abba_python/abba_private/AbbaOntology.py` & `abba_python-0.2.0/src/abba_python/abba_private/AbbaOntology.py`

 * *Files identical despite different names*

### Comparing `abba_python-0.1.9/src/abba_python/abba_private/DeepSliceProcessor.py` & `abba_python-0.2.0/src/abba_python/abba_private/DeepSliceProcessor.py`

 * *Files identical despite different names*

### Comparing `abba_python-0.1.9/src/abba_python/itk/abba_itk.py` & `abba_python-0.2.0/src/abba_python/itk/abba_itk.py`

 * *Files identical despite different names*

### Comparing `abba_python-0.1.9/src/abba_python/run-abba-local-fiji.py` & `abba_python-0.2.0/src/abba_python/run-abba-local-fiji.py`

 * *Files identical despite different names*

### Comparing `abba_python-0.1.9/src/abba_python/run-abba.py` & `abba_python-0.2.0/src/abba_python/run-abba.py`

 * *Files identical despite different names*

### Comparing `abba_python-0.1.9/src/abba_python/scijava_python_command/command.py` & `abba_python-0.2.0/src/abba_python/scijava_python_command/command.py`

 * *Files identical despite different names*

### Comparing `abba_python-0.1.9/src/abba_python/scijava_python_command/jupyter_ui.py` & `abba_python-0.2.0/src/abba_python/scijava_python_command/jupyter_ui.py`

 * *Files identical despite different names*

### Comparing `abba_python-0.1.9/src/abba_python/scijava_python_command/magic.py` & `abba_python-0.2.0/src/abba_python/scijava_python_command/magic.py`

 * *Files identical despite different names*

### Comparing `abba_python-0.1.9/src/abba_python.egg-info/SOURCES.txt` & `abba_python-0.2.0/src/abba_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

