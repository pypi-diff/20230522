# Comparing `tmp/everybeam-0.4.0.tar.gz` & `tmp/everybeam-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/loose/code/EveryBeam/dist/tmp17enyqqt/everybeam-0.4.0.tar", last modified: Fri Nov 11 15:31:05 2022, max compression
+gzip compressed data, was "/home/loose/code/EveryBeam/dist/tmpnpt5x7yr/everybeam-0.5.1.tar", last modified: Mon May 22 10:17:24 2023, max compression
```

## Comparing `everybeam-0.4.0.tar` & `everybeam-0.5.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 loose     (1025) loose     (1025)        0 2022-11-11 15:31:05.000000 everybeam-0.4.0/
--rw-rw-r--   0 loose     (1025) loose     (1025)     1999 2022-10-27 14:26:39.000000 everybeam-0.4.0/README.md
--rw-rw-r--   0 loose     (1025) loose     (1025)    35194 2022-10-27 14:26:39.000000 everybeam-0.4.0/LICENSE
--rw-rw-r--   0 loose     (1025) loose     (1025)       38 2022-11-11 15:31:05.000000 everybeam-0.4.0/setup.cfg
--rw-rw-r--   0 loose     (1025) loose     (1025)     5624 2022-11-11 15:20:17.000000 everybeam-0.4.0/setup.py
--rw-rw-r--   0 loose     (1025) loose     (1025)     2618 2022-11-11 15:31:05.000000 everybeam-0.4.0/PKG-INFO
-drwxrwxr-x   0 loose     (1025) loose     (1025)        0 2022-11-11 15:31:05.000000 everybeam-0.4.0/everybeam.egg-info/
--rw-rw-r--   0 loose     (1025) loose     (1025)        1 2022-11-10 12:56:46.000000 everybeam-0.4.0/everybeam.egg-info/not-zip-safe
--rw-rw-r--   0 loose     (1025) loose     (1025)        1 2022-11-11 15:31:05.000000 everybeam-0.4.0/everybeam.egg-info/dependency_links.txt
--rw-rw-r--   0 loose     (1025) loose     (1025)       10 2022-11-11 15:31:05.000000 everybeam-0.4.0/everybeam.egg-info/top_level.txt
--rw-rw-r--   0 loose     (1025) loose     (1025)      318 2022-11-11 15:31:05.000000 everybeam-0.4.0/everybeam.egg-info/SOURCES.txt
--rw-rw-r--   0 loose     (1025) loose     (1025)     2618 2022-11-11 15:31:05.000000 everybeam-0.4.0/everybeam.egg-info/PKG-INFO
-drwxrwxr-x   0 loose     (1025) loose     (1025)        0 2022-11-11 15:31:05.000000 everybeam-0.4.0/coeffs/
--rw-rw-r--   0 loose     (1025) loose     (1025)   112320 2022-10-27 14:26:39.000000 everybeam-0.4.0/coeffs/oskar.h5
--rw-rw-r--   0 loose     (1025) loose     (1025)     6149 2022-10-27 14:26:39.000000 everybeam-0.4.0/coeffs/element_beam_LBA.coeff
--rw-rw-r--   0 loose     (1025) loose     (1025)     4947 2022-10-27 14:26:39.000000 everybeam-0.4.0/coeffs/element_beam_HBA.coeff
--rw-rw-r--   0 loose     (1025) loose     (1025)     3648 2022-10-27 14:26:39.000000 everybeam-0.4.0/coeffs/HamakerHBACoeff.h5
--rw-rw-r--   0 loose     (1025) loose     (1025)     3648 2022-10-27 14:26:39.000000 everybeam-0.4.0/coeffs/HamakerLBACoeff.h5
+drwxrwxr-x   0 loose     (1025) loose     (1025)        0 2023-05-22 10:17:24.000000 everybeam-0.5.1/
+-rw-rw-r--   0 loose     (1025) loose     (1025)     2010 2023-05-22 08:14:36.000000 everybeam-0.5.1/README.md
+-rw-rw-r--   0 loose     (1025) loose     (1025)    35194 2022-10-27 14:26:39.000000 everybeam-0.5.1/LICENSE
+-rw-rw-r--   0 loose     (1025) loose     (1025)       38 2023-05-22 10:17:24.000000 everybeam-0.5.1/setup.cfg
+-rw-rw-r--   0 loose     (1025) loose     (1025)     5641 2023-05-22 08:14:37.000000 everybeam-0.5.1/setup.py
+-rw-rw-r--   0 loose     (1025) loose     (1025)     2645 2023-05-22 10:17:24.000000 everybeam-0.5.1/PKG-INFO
+drwxrwxr-x   0 loose     (1025) loose     (1025)        0 2023-05-22 10:17:24.000000 everybeam-0.5.1/everybeam.egg-info/
+-rw-rw-r--   0 loose     (1025) loose     (1025)        1 2023-05-22 10:17:24.000000 everybeam-0.5.1/everybeam.egg-info/not-zip-safe
+-rw-rw-r--   0 loose     (1025) loose     (1025)        1 2023-05-22 10:17:24.000000 everybeam-0.5.1/everybeam.egg-info/dependency_links.txt
+-rw-rw-r--   0 loose     (1025) loose     (1025)       10 2023-05-22 10:17:24.000000 everybeam-0.5.1/everybeam.egg-info/top_level.txt
+-rw-rw-r--   0 loose     (1025) loose     (1025)      318 2023-05-22 10:17:24.000000 everybeam-0.5.1/everybeam.egg-info/SOURCES.txt
+-rw-rw-r--   0 loose     (1025) loose     (1025)     2645 2023-05-22 10:17:24.000000 everybeam-0.5.1/everybeam.egg-info/PKG-INFO
+drwxrwxr-x   0 loose     (1025) loose     (1025)        0 2023-05-22 10:17:24.000000 everybeam-0.5.1/coeffs/
+-rw-rw-r--   0 loose     (1025) loose     (1025)   112320 2022-10-27 14:26:39.000000 everybeam-0.5.1/coeffs/oskar.h5
+-rw-rw-r--   0 loose     (1025) loose     (1025)     6149 2022-10-27 14:26:39.000000 everybeam-0.5.1/coeffs/element_beam_LBA.coeff
+-rw-rw-r--   0 loose     (1025) loose     (1025)     4947 2022-10-27 14:26:39.000000 everybeam-0.5.1/coeffs/element_beam_HBA.coeff
+-rw-rw-r--   0 loose     (1025) loose     (1025)     3648 2022-10-27 14:26:39.000000 everybeam-0.5.1/coeffs/HamakerHBACoeff.h5
+-rw-rw-r--   0 loose     (1025) loose     (1025)     3648 2022-10-27 14:26:39.000000 everybeam-0.5.1/coeffs/HamakerLBACoeff.h5
```

### Comparing `everybeam-0.4.0/README.md` & `everybeam-0.5.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 # EveryBeam library
 
 This package can be used to compute the beam response for a variety of
 radio telescopes, i.e.:
 
 * LOFAR
-* OSKAR
-* MWA
-* VLA
+* SKA/OSKAR
 * ATCA
+* GMRT
+* VLA
+* MWA
 
 This package also provides an abstract interface to a selection of beam responses for apperture arrays (LOFAR/OSKAR), and beamformed versions thereof. Currently implemented are:
 
  * Hamaker LOFAR model
  * OSKAR spherical wave model
  * OSKAR-dipole: work in progress
  * LOBEs: work in progress. A coefficient file is currently only available for a limited number of LOFAR stations. Selecting the LOBEs model defaults back to Hamaker, in case no coefficient file is available.
```

### Comparing `everybeam-0.4.0/LICENSE` & `everybeam-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `everybeam-0.4.0/setup.py` & `everybeam-0.5.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 from setuptools import Extension, setup
 from setuptools.command.build_ext import build_ext
 
 
 # Set the location where data files are to be installed
 EVERYBEAM_DATADIR = os.path.join("share", "everybeam")
 
+
 # A CMakeExtension needs a sourcedir instead of a file list.
 # The name must be the _single_ output extension from the CMake build.
 # If you need multiple extensions, see scikit-build.
 class CMakeExtension(Extension):
     def __init__(self, name, sourcedir=""):
         Extension.__init__(self, name, sources=[])
         self.sourcedir = os.path.abspath(sourcedir)
@@ -126,28 +127,28 @@
         )
     )
 
 # The information here can also be placed in setup.cfg - better separation of
 # logic and declaration, and simpler if you include description/version in a file.
 setup(
     name="everybeam",
-    version="0.4.0",
-    author="Andre Offringa",
+    version="0.5.1",
+    author="André Offringa",
     author_email="offringa@astron.nl",
     description="EveryBeam",
     long_description=open("README.md", "rt").read(),
     long_description_content_type="text/markdown",
     ext_modules=[CMakeExtension("everybeam")],
     cmdclass={"build_ext": CMakeBuild},
     zip_safe=False,
     python_requires=">=3.6",
     url="https://everybeam.readthedocs.io/",
     classifiers=[
-        "Development Status :: 4 - Beta",
+        "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Science/Research",
-        "License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)",
+        "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
         "Programming Language :: C++",
         "Programming Language :: Python :: 3",
         "Topic :: Scientific/Engineering :: Astronomy",
     ],
     data_files=data_files,
 )
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `everybeam-0.4.0/PKG-INFO` & `everybeam-0.5.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,36 +1,37 @@
 Metadata-Version: 2.1
 Name: everybeam
-Version: 0.4.0
+Version: 0.5.1
 Summary: EveryBeam
 Home-page: https://everybeam.readthedocs.io/
-Author: Andre Offringa
+Author: André Offringa
 Author-email: offringa@astron.nl
 License: UNKNOWN
 Platform: UNKNOWN
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
+Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: C++
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # EveryBeam library
 
 This package can be used to compute the beam response for a variety of
 radio telescopes, i.e.:
 
 * LOFAR
-* OSKAR
-* MWA
-* VLA
+* SKA/OSKAR
 * ATCA
+* GMRT
+* VLA
+* MWA
 
 This package also provides an abstract interface to a selection of beam responses for apperture arrays (LOFAR/OSKAR), and beamformed versions thereof. Currently implemented are:
 
  * Hamaker LOFAR model
  * OSKAR spherical wave model
  * OSKAR-dipole: work in progress
  * LOBEs: work in progress. A coefficient file is currently only available for a limited number of LOFAR stations. Selecting the LOBEs model defaults back to Hamaker, in case no coefficient file is available.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `everybeam-0.4.0/everybeam.egg-info/PKG-INFO` & `everybeam-0.5.1/everybeam.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,36 +1,37 @@
 Metadata-Version: 2.1
 Name: everybeam
-Version: 0.4.0
+Version: 0.5.1
 Summary: EveryBeam
 Home-page: https://everybeam.readthedocs.io/
-Author: Andre Offringa
+Author: André Offringa
 Author-email: offringa@astron.nl
 License: UNKNOWN
 Platform: UNKNOWN
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
+Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: C++
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # EveryBeam library
 
 This package can be used to compute the beam response for a variety of
 radio telescopes, i.e.:
 
 * LOFAR
-* OSKAR
-* MWA
-* VLA
+* SKA/OSKAR
 * ATCA
+* GMRT
+* VLA
+* MWA
 
 This package also provides an abstract interface to a selection of beam responses for apperture arrays (LOFAR/OSKAR), and beamformed versions thereof. Currently implemented are:
 
  * Hamaker LOFAR model
  * OSKAR spherical wave model
  * OSKAR-dipole: work in progress
  * LOBEs: work in progress. A coefficient file is currently only available for a limited number of LOFAR stations. Selecting the LOBEs model defaults back to Hamaker, in case no coefficient file is available.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `everybeam-0.4.0/coeffs/oskar.h5` & `everybeam-0.5.1/coeffs/oskar.h5`

 * *Files identical despite different names*

### Comparing `everybeam-0.4.0/coeffs/element_beam_LBA.coeff` & `everybeam-0.5.1/coeffs/element_beam_LBA.coeff`

 * *Files identical despite different names*

### Comparing `everybeam-0.4.0/coeffs/element_beam_HBA.coeff` & `everybeam-0.5.1/coeffs/element_beam_HBA.coeff`

 * *Files identical despite different names*

### Comparing `everybeam-0.4.0/coeffs/HamakerHBACoeff.h5` & `everybeam-0.5.1/coeffs/HamakerHBACoeff.h5`

 * *Files identical despite different names*

### Comparing `everybeam-0.4.0/coeffs/HamakerLBACoeff.h5` & `everybeam-0.5.1/coeffs/HamakerLBACoeff.h5`

 * *Files identical despite different names*

