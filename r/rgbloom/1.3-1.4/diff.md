# Comparing `tmp/rgbloom-1.3.tar.gz` & `tmp/rgbloom-1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/cardiel/s/rgbloom/dist/.tmp-8du81lci/rgbloom-1.3.tar", last modified: Tue May  9 11:47:14 2023, max compression
+gzip compressed data, was "rgbloom-1.4.tar", last modified: Mon May 22 11:44:14 2023, max compression
```

## Comparing `rgbloom-1.3.tar` & `rgbloom-1.4.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 cardiel    (501) staff       (20)        0 2023-05-09 11:47:14.601941 rgbloom-1.3/
--rw-r--r--   0 cardiel    (501) staff       (20)    35149 2022-11-06 08:36:25.000000 rgbloom-1.3/LICENSE
--rw-r--r--   0 cardiel    (501) staff       (20)    11724 2023-05-09 11:47:14.602127 rgbloom-1.3/PKG-INFO
--rw-r--r--   0 cardiel    (501) staff       (20)    10934 2023-03-27 18:00:47.000000 rgbloom-1.3/README.md
--rw-r--r--   0 cardiel    (501) staff       (20)      100 2022-11-06 08:38:35.000000 rgbloom-1.3/pyproject.toml
-drwxr-xr-x   0 cardiel    (501) staff       (20)        0 2023-05-09 11:47:14.595991 rgbloom-1.3/rgbloom/
--rw-r--r--   0 cardiel    (501) staff       (20)       51 2022-11-06 08:39:16.000000 rgbloom-1.3/rgbloom/__init__.py
--rw-r--r--   0 cardiel    (501) staff       (20)     5613 2023-03-21 18:25:00.000000 rgbloom-1.3/rgbloom/__main__.py
-drwxr-xr-x   0 cardiel    (501) staff       (20)        0 2023-05-09 11:47:14.600376 rgbloom-1.3/rgbloom/core/
--rw-r--r--   0 cardiel    (501) staff       (20)        0 2022-11-06 08:39:16.000000 rgbloom-1.3/rgbloom/core/__init__.py
--rw-r--r--   0 cardiel    (501) staff       (20)     2487 2022-11-06 08:39:16.000000 rgbloom-1.3/rgbloom/core/step1.py
--rw-r--r--   0 cardiel    (501) staff       (20)     1844 2022-11-06 08:39:16.000000 rgbloom-1.3/rgbloom/core/step2.py
--rw-r--r--   0 cardiel    (501) staff       (20)     3128 2023-03-21 17:40:50.000000 rgbloom-1.3/rgbloom/core/step3.py
--rw-r--r--   0 cardiel    (501) staff       (20)     2560 2022-11-06 08:39:16.000000 rgbloom-1.3/rgbloom/core/step4.py
--rw-r--r--   0 cardiel    (501) staff       (20)     3007 2023-03-21 17:42:15.000000 rgbloom-1.3/rgbloom/core/step5.py
-drwxr-xr-x   0 cardiel    (501) staff       (20)        0 2023-05-09 11:47:14.601605 rgbloom-1.3/rgbloom/gui/
--rw-r--r--   0 cardiel    (501) staff       (20)        0 2022-11-06 08:39:16.000000 rgbloom-1.3/rgbloom/gui/__init__.py
--rw-r--r--   0 cardiel    (501) staff       (20)     7832 2023-03-21 18:17:15.000000 rgbloom-1.3/rgbloom/gui/step6.py
--rw-r--r--   0 cardiel    (501) staff       (20)      497 2022-11-06 08:39:16.000000 rgbloom-1.3/rgbloom/gui/style.py
--rw-r--r--   0 cardiel    (501) staff       (20)       16 2023-05-09 11:45:51.000000 rgbloom-1.3/rgbloom/version.py
-drwxr-xr-x   0 cardiel    (501) staff       (20)        0 2023-05-09 11:47:14.598030 rgbloom-1.3/rgbloom.egg-info/
--rw-r--r--   0 cardiel    (501) staff       (20)    11724 2023-05-09 11:47:14.000000 rgbloom-1.3/rgbloom.egg-info/PKG-INFO
--rw-r--r--   0 cardiel    (501) staff       (20)      499 2023-05-09 11:47:14.000000 rgbloom-1.3/rgbloom.egg-info/SOURCES.txt
--rw-r--r--   0 cardiel    (501) staff       (20)        1 2023-05-09 11:47:14.000000 rgbloom-1.3/rgbloom.egg-info/dependency_links.txt
--rw-r--r--   0 cardiel    (501) staff       (20)       50 2023-05-09 11:47:14.000000 rgbloom-1.3/rgbloom.egg-info/entry_points.txt
--rw-r--r--   0 cardiel    (501) staff       (20)       80 2023-05-09 11:47:14.000000 rgbloom-1.3/rgbloom.egg-info/requires.txt
--rw-r--r--   0 cardiel    (501) staff       (20)        8 2023-05-09 11:47:14.000000 rgbloom-1.3/rgbloom.egg-info/top_level.txt
--rw-r--r--   0 cardiel    (501) staff       (20)     1040 2023-05-09 11:47:14.602878 rgbloom-1.3/setup.cfg
--rw-r--r--   0 cardiel    (501) staff       (20)       68 2022-11-06 08:39:44.000000 rgbloom-1.3/setup.py
+drwxr-xr-x   0 cardiel    (501) staff       (20)        0 2023-05-22 11:44:14.626926 rgbloom-1.4/
+-rw-r--r--   0 cardiel    (501) staff       (20)    35149 2022-11-06 08:36:25.000000 rgbloom-1.4/LICENSE
+-rw-r--r--   0 cardiel    (501) staff       (20)    12806 2023-05-22 11:44:14.626987 rgbloom-1.4/PKG-INFO
+-rw-r--r--   0 cardiel    (501) staff       (20)    12016 2023-05-22 11:40:39.000000 rgbloom-1.4/README.md
+-rw-r--r--   0 cardiel    (501) staff       (20)      100 2022-11-06 08:38:35.000000 rgbloom-1.4/pyproject.toml
+drwxr-xr-x   0 cardiel    (501) staff       (20)        0 2023-05-22 11:44:14.624347 rgbloom-1.4/rgbloom/
+-rw-r--r--   0 cardiel    (501) staff       (20)       51 2022-11-06 08:39:16.000000 rgbloom-1.4/rgbloom/__init__.py
+-rw-r--r--   0 cardiel    (501) staff       (20)     6508 2023-05-22 11:40:39.000000 rgbloom-1.4/rgbloom/__main__.py
+drwxr-xr-x   0 cardiel    (501) staff       (20)        0 2023-05-22 11:44:14.626364 rgbloom-1.4/rgbloom/core/
+-rw-r--r--   0 cardiel    (501) staff       (20)        0 2022-11-06 08:39:16.000000 rgbloom-1.4/rgbloom/core/__init__.py
+-rw-r--r--   0 cardiel    (501) staff       (20)     2487 2022-11-06 08:39:16.000000 rgbloom-1.4/rgbloom/core/step1.py
+-rw-r--r--   0 cardiel    (501) staff       (20)     1844 2022-11-06 08:39:16.000000 rgbloom-1.4/rgbloom/core/step2.py
+-rw-r--r--   0 cardiel    (501) staff       (20)     3128 2023-03-21 17:40:50.000000 rgbloom-1.4/rgbloom/core/step3.py
+-rw-r--r--   0 cardiel    (501) staff       (20)     2560 2022-11-06 08:39:16.000000 rgbloom-1.4/rgbloom/core/step4.py
+-rw-r--r--   0 cardiel    (501) staff       (20)     3007 2023-03-21 17:42:15.000000 rgbloom-1.4/rgbloom/core/step5.py
+drwxr-xr-x   0 cardiel    (501) staff       (20)        0 2023-05-22 11:44:14.626811 rgbloom-1.4/rgbloom/gui/
+-rw-r--r--   0 cardiel    (501) staff       (20)        0 2022-11-06 08:39:16.000000 rgbloom-1.4/rgbloom/gui/__init__.py
+-rw-r--r--   0 cardiel    (501) staff       (20)    10034 2023-05-22 11:40:39.000000 rgbloom-1.4/rgbloom/gui/step6.py
+-rw-r--r--   0 cardiel    (501) staff       (20)      497 2022-11-06 08:39:16.000000 rgbloom-1.4/rgbloom/gui/style.py
+-rw-r--r--   0 cardiel    (501) staff       (20)       16 2023-05-22 11:40:39.000000 rgbloom-1.4/rgbloom/version.py
+drwxr-xr-x   0 cardiel    (501) staff       (20)        0 2023-05-22 11:44:14.625016 rgbloom-1.4/rgbloom.egg-info/
+-rw-r--r--   0 cardiel    (501) staff       (20)    12806 2023-05-22 11:44:14.000000 rgbloom-1.4/rgbloom.egg-info/PKG-INFO
+-rw-r--r--   0 cardiel    (501) staff       (20)      499 2023-05-22 11:44:14.000000 rgbloom-1.4/rgbloom.egg-info/SOURCES.txt
+-rw-r--r--   0 cardiel    (501) staff       (20)        1 2023-05-22 11:44:14.000000 rgbloom-1.4/rgbloom.egg-info/dependency_links.txt
+-rw-r--r--   0 cardiel    (501) staff       (20)       50 2023-05-22 11:44:14.000000 rgbloom-1.4/rgbloom.egg-info/entry_points.txt
+-rw-r--r--   0 cardiel    (501) staff       (20)       80 2023-05-22 11:44:14.000000 rgbloom-1.4/rgbloom.egg-info/requires.txt
+-rw-r--r--   0 cardiel    (501) staff       (20)        8 2023-05-22 11:44:14.000000 rgbloom-1.4/rgbloom.egg-info/top_level.txt
+-rw-r--r--   0 cardiel    (501) staff       (20)     1040 2023-05-22 11:44:14.627308 rgbloom-1.4/setup.cfg
+-rw-r--r--   0 cardiel    (501) staff       (20)       68 2022-11-06 08:39:44.000000 rgbloom-1.4/setup.py
```

### Comparing `rgbloom-1.3/LICENSE` & `rgbloom-1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `rgbloom-1.3/PKG-INFO` & `rgbloom-1.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rgbloom
-Version: 1.3
+Version: 1.4
 Summary: RGB from Gaia EDR3
 Home-page: https://github.com/guaix-ucm/rgbloom
 Author: Nicolás Cardiel
 Author-email: cardiel@ucm.es
 License: GPLv3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -53,31 +53,38 @@
 
 You need to have a live connection to the Internet for 
 the script to work!
 
 ## Installing the code
 
 In order to keep your current Python installation clean, it is highly 
-recommended to install a python 3 *virtual environment* first.
+recommended to first build Python 3 *virtual environment*.
 
-### Creating and activating the python virtual environment
+### Creating and activating the Python virtual environment
 
 ```bash
 $ python3 -m venv venv_rgb
 $ . venv_rgb/bin/activate
 (venv_rgb) $
 ```
 
 ### Installing the package
 
+We recommend installing the latest stable version, which is available via
+the PyPI respository:
+
 ```bash
-(venv_rgb) $ pip install git+https://github.com/guaix-ucm/rgbloom.git@main#egg=rgbloom
+(venv_rgb) $ pip install rgbloom
 ```
 
+The latest development version is available through GitHub:
 
+```bash
+(venv_rgb) $ pip install git+https://github.com/guaix-ucm/rgbloom.git@main#egg=rgbloom
+```
 
 ## Executing the program
 
 Just execute it from the command line:
 
 ```bash
 (venv_rgb) $ rgbloom 56.66 24.10 1.0 12
@@ -96,15 +103,15 @@
 recover disk space).
 
 The execution of this example should led to the following output in the
 terminal (except for the absolute path where the auxiliary downloaded files 
 are stored):
 
 ```
-        Welcome to rgbloom version 1.2
+        Welcome to rgbloom version 1.4
         ==============================
 
 Downloading data from 'http://nartex.fis.ucm.es/~ncl/rgbphot/gaiaDR3/reference_healpix8.csv' to file '/Users/cardiel/Library/Caches/pooch/635cd722cf61b23bd8eee20635e4d580-reference_healpix8.csv'.
 <STEP1> Starting cone search in Gaia DR3... (please wait)
   INFO: Query finished. [astroquery.utils.tap.core]
         --> 310 objects found
         --> 23 objects classified as VARIABLE
@@ -188,15 +195,15 @@
       - `RGB_R`: red RGB magnitude estimate
 
   The list of objects in these two files is sorted by right ascension.
 
 - Step 6: generation of a finding chart plot (in PDF format): `rgbloom.pdf`. 
   The execution of the previous example generates a cone search around 
   the [Pleiades](https://en.wikipedia.org/wiki/Pleiades) star cluster:
-  ![Pleiades plot](http://nartex.hst.ucm.es/~ncl/rgbphot/gaiaDR3/pleiades_v5.png)
+  ![Pleiades plot](http://nartex.hst.ucm.es/~ncl/rgbphot/gaiaDR3/pleiades_v6.png)
   The objects in this plot are color coded based on the *Gaia* G_BP - G_RP 
   colour. Stars brighter than a pre-defined threshold are displayed 
   with big star symbols. To facilitate the identification of each object, the
   consecutive identification numbers in the two files `rgbloom_200m.csv` and
   `rgbloom_no200m.csv` are also displayed, in red
   and black, respectively. The identification numbers corresponding to the less
   reliable sources in `rgbloom_20m.csv` (`qlflag=1`) appear inside a rectangle
@@ -216,30 +223,42 @@
 ### Additional help
 
 Some auxiliary optional arguments are also available. See description 
 invoking the script help:
 
 ```bash
 $ rgbloom --help
+usage: rgbloom [-h] [--basename BASENAME] [--brightlimit BRIGHTLIMIT] [--symbsize SYMBSIZE] [--max_symbsize MAX_SYMBSIZE]
+               [--min_symbsize MIN_SYMBSIZE] [--mag_power MAG_POWER] [--display_g_mag] [--num_fontsize NUM_FONTSIZE]
+               [--nonumbers] [--noplot] [--nocolor] [--verbose]
+               ra_center dec_center search_radius g_limit
 
-...
-...
+RGB predictions from Gaia DR3 spectrophotometry (version 1.4)
 
 positional arguments:
   ra_center             right Ascension (decimal degrees)
   dec_center            declination (decimal degrees)
   search_radius         search radius (decimal degrees)
   g_limit               limiting Gaia G magnitude
 
 optional arguments:
   -h, --help            show this help message and exit
   --basename BASENAME   file basename for output files
   --brightlimit BRIGHTLIMIT
                         objects brighter than this Gaia G limit are displayed with star symbols (default=8.0)
-  --symbsize SYMBSIZE   multiplying factor for symbol size (default=1.0)
+  --symbsize SYMBSIZE   global multiplying factor for symbol size (default=1.0)
+  --max_symbsize MAX_SYMBSIZE
+                        maximum symbol size in chart (default=1000)
+  --min_symbsize MIN_SYMBSIZE
+                        minimum symbol size in chart (default=10)
+  --mag_power MAG_POWER
+                        power to scale symbol sizes in chart (default=3)
+  --display_g_mag       display Gaia G magnitude instead of object number
+  --num_fontsize NUM_FONTSIZE
+                        font size for numbers in chart (default=5)
   --nonumbers           do not display object identification number in PDF chart
   --noplot              skip PDF chart generation
   --nocolor             do not use colors in PDF chart
   --verbose             increase program verbosity
 ```
 
 ## Citation
```

### Comparing `rgbloom-1.3/README.md` & `rgbloom-1.4/rgbloom.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,29 @@
+Metadata-Version: 2.1
+Name: rgbloom
+Version: 1.4
+Summary: RGB from Gaia EDR3
+Home-page: https://github.com/guaix-ucm/rgbloom
+Author: Nicolás Cardiel
+Author-email: cardiel@ucm.es
+License: GPLv3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Development Status :: 3 - Alpha
+Classifier: Environment :: Console
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Operating System :: OS Independent
+Classifier: Topic :: Scientific/Engineering :: Astronomy
+Description-Content-Type: text/markdown
+Provides-Extra: test
+License-File: LICENSE
+
 # rgbloom
 
 This Python script retrieves RGB magnitudes computed from low resolution
 spectra published in *Gaia* DR3, following the work described in 
 [Carrasco et al. (2023)](#3).
 These magnitudes are given in the standard system defined by
 [Cardiel et al. (2021a)](#1).
@@ -31,31 +53,38 @@
 
 You need to have a live connection to the Internet for 
 the script to work!
 
 ## Installing the code
 
 In order to keep your current Python installation clean, it is highly 
-recommended to install a python 3 *virtual environment* first.
+recommended to first build Python 3 *virtual environment*.
 
-### Creating and activating the python virtual environment
+### Creating and activating the Python virtual environment
 
 ```bash
 $ python3 -m venv venv_rgb
 $ . venv_rgb/bin/activate
 (venv_rgb) $
 ```
 
 ### Installing the package
 
+We recommend installing the latest stable version, which is available via
+the PyPI respository:
+
 ```bash
-(venv_rgb) $ pip install git+https://github.com/guaix-ucm/rgbloom.git@main#egg=rgbloom
+(venv_rgb) $ pip install rgbloom
 ```
 
+The latest development version is available through GitHub:
 
+```bash
+(venv_rgb) $ pip install git+https://github.com/guaix-ucm/rgbloom.git@main#egg=rgbloom
+```
 
 ## Executing the program
 
 Just execute it from the command line:
 
 ```bash
 (venv_rgb) $ rgbloom 56.66 24.10 1.0 12
@@ -74,15 +103,15 @@
 recover disk space).
 
 The execution of this example should led to the following output in the
 terminal (except for the absolute path where the auxiliary downloaded files 
 are stored):
 
 ```
-        Welcome to rgbloom version 1.2
+        Welcome to rgbloom version 1.4
         ==============================
 
 Downloading data from 'http://nartex.fis.ucm.es/~ncl/rgbphot/gaiaDR3/reference_healpix8.csv' to file '/Users/cardiel/Library/Caches/pooch/635cd722cf61b23bd8eee20635e4d580-reference_healpix8.csv'.
 <STEP1> Starting cone search in Gaia DR3... (please wait)
   INFO: Query finished. [astroquery.utils.tap.core]
         --> 310 objects found
         --> 23 objects classified as VARIABLE
@@ -166,15 +195,15 @@
       - `RGB_R`: red RGB magnitude estimate
 
   The list of objects in these two files is sorted by right ascension.
 
 - Step 6: generation of a finding chart plot (in PDF format): `rgbloom.pdf`. 
   The execution of the previous example generates a cone search around 
   the [Pleiades](https://en.wikipedia.org/wiki/Pleiades) star cluster:
-  ![Pleiades plot](http://nartex.hst.ucm.es/~ncl/rgbphot/gaiaDR3/pleiades_v5.png)
+  ![Pleiades plot](http://nartex.hst.ucm.es/~ncl/rgbphot/gaiaDR3/pleiades_v6.png)
   The objects in this plot are color coded based on the *Gaia* G_BP - G_RP 
   colour. Stars brighter than a pre-defined threshold are displayed 
   with big star symbols. To facilitate the identification of each object, the
   consecutive identification numbers in the two files `rgbloom_200m.csv` and
   `rgbloom_no200m.csv` are also displayed, in red
   and black, respectively. The identification numbers corresponding to the less
   reliable sources in `rgbloom_20m.csv` (`qlflag=1`) appear inside a rectangle
@@ -194,30 +223,42 @@
 ### Additional help
 
 Some auxiliary optional arguments are also available. See description 
 invoking the script help:
 
 ```bash
 $ rgbloom --help
+usage: rgbloom [-h] [--basename BASENAME] [--brightlimit BRIGHTLIMIT] [--symbsize SYMBSIZE] [--max_symbsize MAX_SYMBSIZE]
+               [--min_symbsize MIN_SYMBSIZE] [--mag_power MAG_POWER] [--display_g_mag] [--num_fontsize NUM_FONTSIZE]
+               [--nonumbers] [--noplot] [--nocolor] [--verbose]
+               ra_center dec_center search_radius g_limit
 
-...
-...
+RGB predictions from Gaia DR3 spectrophotometry (version 1.4)
 
 positional arguments:
   ra_center             right Ascension (decimal degrees)
   dec_center            declination (decimal degrees)
   search_radius         search radius (decimal degrees)
   g_limit               limiting Gaia G magnitude
 
 optional arguments:
   -h, --help            show this help message and exit
   --basename BASENAME   file basename for output files
   --brightlimit BRIGHTLIMIT
                         objects brighter than this Gaia G limit are displayed with star symbols (default=8.0)
-  --symbsize SYMBSIZE   multiplying factor for symbol size (default=1.0)
+  --symbsize SYMBSIZE   global multiplying factor for symbol size (default=1.0)
+  --max_symbsize MAX_SYMBSIZE
+                        maximum symbol size in chart (default=1000)
+  --min_symbsize MIN_SYMBSIZE
+                        minimum symbol size in chart (default=10)
+  --mag_power MAG_POWER
+                        power to scale symbol sizes in chart (default=3)
+  --display_g_mag       display Gaia G magnitude instead of object number
+  --num_fontsize NUM_FONTSIZE
+                        font size for numbers in chart (default=5)
   --nonumbers           do not display object identification number in PDF chart
   --noplot              skip PDF chart generation
   --nocolor             do not use colors in PDF chart
   --verbose             increase program verbosity
 ```
 
 ## Citation
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `rgbloom-1.3/rgbloom/__main__.py` & `rgbloom-1.4/rgbloom/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -146,16 +146,21 @@
     else:
         step6(
             r_dr3_200m,
             r_dr3_no200m,
             args.ra_center,
             args.dec_center,
             args.search_radius,
-            args.symbsize,
             args.brightlimit,
+            args.symbsize,
+            args.max_symbsize,
+            args.min_symbsize,
+            args.mag_power,
+            args.display_g_mag,
+            args.num_fontsize,
             args.nonumbers,
             args.nocolor,
             args.basename,
             version,
             args.verbose
         )
     print('End of program')
@@ -168,17 +173,28 @@
     parser.add_argument("dec_center", help="declination (decimal degrees)", type=declination)
     parser.add_argument("search_radius", help="search radius (decimal degrees)", type=search_radius)
     parser.add_argument("g_limit", help="limiting Gaia G magnitude", type=float)
     parser.add_argument("--basename", help="file basename for output files", type=str, default="rgbloom")
     parser.add_argument("--brightlimit",
                         help="objects brighter than this Gaia G limit are displayed with star symbols (default=8.0)",
                         type=float, default=8.0)
-    parser.add_argument("--symbsize", help="multiplying factor for symbol size (default=1.0)",
+    parser.add_argument("--symbsize", help="global multiplying factor for symbol size (default=1.0)",
                         type=float, default=1.0)
-    parser.add_argument("--nonumbers", help="do not display object identification number in PDF chart", action="store_true")
+    parser.add_argument("--max_symbsize", help="maximum symbol size in chart (default=1000)",
+                        type=float, default=1000)
+    parser.add_argument("--min_symbsize", help="minimum symbol size in chart (default=10)",
+                        type=float, default=10)
+    parser.add_argument("--mag_power", help="power to scale symbol sizes in chart (default=3)",
+                        type=float, default=3)
+    parser.add_argument("--display_g_mag", help="display Gaia G magnitude instead of object number",
+                        action="store_true")
+    parser.add_argument("--num_fontsize", help="font size for numbers in chart (default=5)",
+                        type=int, default=5)
+    parser.add_argument("--nonumbers", help="do not display object identification number in PDF chart",
+                        action="store_true")
     parser.add_argument("--noplot", help="skip PDF chart generation", action="store_true")
     parser.add_argument("--nocolor", help="do not use colors in PDF chart", action="store_true")
     parser.add_argument("--verbose", help="increase program verbosity", action="store_true")
 
     args = parser.parse_args()
 
     if len(sys.argv) == 1:
```

### Comparing `rgbloom-1.3/rgbloom/core/step1.py` & `rgbloom-1.4/rgbloom/core/step1.py`

 * *Files identical despite different names*

### Comparing `rgbloom-1.3/rgbloom/core/step2.py` & `rgbloom-1.4/rgbloom/core/step2.py`

 * *Files identical despite different names*

### Comparing `rgbloom-1.3/rgbloom/core/step3.py` & `rgbloom-1.4/rgbloom/core/step3.py`

 * *Files identical despite different names*

### Comparing `rgbloom-1.3/rgbloom/core/step4.py` & `rgbloom-1.4/rgbloom/core/step4.py`

 * *Files identical despite different names*

### Comparing `rgbloom-1.3/rgbloom/core/step5.py` & `rgbloom-1.4/rgbloom/core/step5.py`

 * *Files identical despite different names*

### Comparing `rgbloom-1.3/rgbloom/gui/step6.py` & `rgbloom-1.4/rgbloom/gui/step6.py`

 * *Files 25% similar despite different names*

```diff
@@ -6,29 +6,33 @@
 # License-Filename: LICENSE.txt
 #
 
 """
 Generate output PDF plot
 """
 
-import matplotlib.pyplot as plt
-import matplotlib.style
 from astropy import units as u
+from astropy.table import vstack
 from astropy.wcs import WCS
 from astropy.coordinates import SkyCoord
+import matplotlib as mpl
+import matplotlib.pyplot as plt
+import matplotlib.style
 import numpy as np
 
 from .style import mpl_style
 OUTTYPES_COLOR = {'200m': 'red', 'no200m': 'black', 'var': 'blue'}
 
 matplotlib.use('pdf')
 
 
-def step6(r_dr3_200m, r_dr3_no200m, ra_center, dec_center, search_radius, symbsize, brightlimit,
-          nonumbers, nocolor, basename, version, verbose):
+def step6(r_dr3_200m, r_dr3_no200m, ra_center, dec_center, search_radius, brightlimit,
+          symbsize, max_symbsize, min_symbsize, mag_power,
+          display_g_mag, num_fontsize, nonumbers, nocolor,
+          basename, version, verbose):
     """Perform EDR3 query
 
     Parameters
     ----------
     r_dr3_200m : astropy Table
         Objects in both the DR3 query and the 200M sample.
     r_dr3_no200m : astropy Table
@@ -37,33 +41,50 @@
         Right ascension (decimal degree) corresponding to the center
         of the field of view.
     dec_center : float
         Declination (decimal degree) corresponding to the center
         of the field of view.
     search_radius : float
         Radius (decimal degrees) of the field of view.
-    symbsize : float
-        Multiplying factor for symbol size.
     brightlimit : float
         Stars brighter than this Gaia G limit are displayed with star
         symbols.
+    symbsize : float
+        Global multiplying factor for symbol size.
+    max_symbsize : float
+        Maximum symbol size in chart.
+    min_symbsize : float
+        Minimum symbol size in chart.
+    mag_power: float
+        Power to scale symbol sizes in chart. The relative magnitude
+        difference (rescaled between 0 and 1) is raised to this power
+        to set the symbol size.
+    display_g_mag : bool
+        If True display Gaia G mag instead of object number.
+    num_fontsize : int
+        Font size for numbers in chart.
     nonumbers : bool
         If True, do not display star numbers in PDF chart.
     nocolor : bool
         If True, do not use colors in PDF chart.
     basename : str
         Base name for output files.
     version : str
         Version number.
     verbose : bool
         If True, display additional information.
 
     """
     print('<STEP6> Generating PDF plot')
 
+    # color map
+    cmap = plt.cm.get_cmap('jet')
+    cmap_vmin = -0.5
+    cmap_vmax = 2.0
+
     # define WCS
     naxis1 = 1024
     naxis2 = naxis1
     pixscale = 2 * search_radius / naxis1
 
     wcs_image = WCS(naxis=2)
     wcs_image.wcs.crpix = [naxis1 / 2, naxis2 / 2]
@@ -76,72 +97,101 @@
         print(wcs_image)
 
     matplotlib.style.use(mpl_style)
     fig = plt.figure(figsize=(13, 10))
     ax = plt.subplot(projection=wcs_image)
 
     # generate plot
-    for sample in ['200m', 'no200m']:
-        if sample == '200m':
-            r_table = r_dr3_200m
-        else:
-            r_table = r_dr3_no200m
+    if len(r_dr3_200m) > 0 and len(r_dr3_no200m) > 0:
+        r_table = vstack([r_dr3_200m, r_dr3_no200m])
+    elif len(r_dr3_200m) > 0:
+        r_table = r_dr3_200m
+    elif len(r_dr3_no200m) > 0:
+        r_table = r_dr3_no200m
+    else:
+        r_table = None
 
+    if r_table is not None:
         r_table.sort('phot_g_mean_mag')
         if verbose:
             r_table.pprint(max_width=1000)
 
-        symbol_size = symbsize * (50 / np.array(r_table['phot_g_mean_mag'])) ** 2.5
+        # define symbol size
+        min_mag = np.ma.min(r_table['phot_g_mean_mag'].value)
+        max_mag = np.ma.max(r_table['phot_g_mean_mag'].value)
+        norm_delta_mag = (np.array(r_table['phot_g_mean_mag'])-min_mag)/(max_mag - min_mag)
+        symbol_size = max_symbsize - (norm_delta_mag**(1/mag_power)) * (max_symbsize - min_symbsize)
+        symbol_size *= symbsize
+
+        # (X, Y) coordinates
         ra_array = np.array(r_table['ra'])
         dec_array = np.array(r_table['dec'])
-
         c = SkyCoord(ra=ra_array * u.degree, dec=dec_array * u.degree, frame='icrs')
         x_pix, y_pix = wcs_image.world_to_pixel(c)
 
-        iok = r_table['phot_g_mean_mag'] < brightlimit
+        iok_bool = r_table['phot_g_mean_mag'] > brightlimit
+        iok = np.arange(len(iok_bool))[iok_bool]
+        iokstar = np.arange(len(iok_bool))[~iok_bool]
         if nocolor:
-            sc = ax.scatter(x_pix[iok], y_pix[iok], marker='*', color='grey',
-                            edgecolors='black', linewidth=0.2, s=symbol_size[iok])
-            ax.scatter(x_pix[~iok], y_pix[~iok], marker='.', color='grey',
-                       edgecolors='black', linewidth=0.2, s=symbol_size[~iok])
+            for i in iokstar:
+                ax.scatter(x_pix[i], y_pix[i], marker='*', color='grey',
+                           edgecolors='white', linewidth=0.2, s=symbol_size[i], zorder=i+1)
+            for i in iok:
+                ax.scatter(x_pix[i], y_pix[i], marker='.', color='grey',
+                           edgecolors='white', linewidth=0.2, s=symbol_size[i], zorder=i+1)
         else:
-            cmap = plt.cm.get_cmap('jet')
-            sc = ax.scatter(x_pix[iok], y_pix[iok], marker='*',
-                            edgecolors='black', linewidth=0.2, s=symbol_size[iok],
-                            cmap=cmap, c=r_table[iok]['bp_rp'], vmin=-0.5, vmax=2.0)
-            ax.scatter(x_pix[~iok], y_pix[~iok], marker='.',
-                       edgecolors='black', linewidth=0.2, s=symbol_size[~iok],
-                       cmap=cmap, c=r_table[~iok]['bp_rp'], vmin=-0.5, vmax=2.0)
+            for i in iokstar:
+                ax.scatter(x_pix[i], y_pix[i], marker='*',
+                           edgecolors='black', linewidth=0.2, s=symbol_size[i], zorder=i+1,
+                           cmap=cmap, c=r_table[i]['bp_rp'], vmin=cmap_vmin, vmax=cmap_vmax)
+            for i in iok:
+                ax.scatter(x_pix[i], y_pix[i], marker='.',
+                           edgecolors='black', linewidth=0.2, s=symbol_size[i], zorder=i+1,
+                           cmap=cmap, c=r_table[i]['bp_rp'], vmin=cmap_vmin, vmax=cmap_vmax)
 
         # display numbers if requested
         if not nonumbers:
             for irow in range(len(r_table)):
-                text = r_table[irow]['number']
+                if display_g_mag:
+                    text = f'{r_table[irow]["phot_g_mean_mag"]:.2f}'
+                else:
+                    text = r_table[irow]['number']
                 if r_table[irow]['qlflag'] == 1:
                     bbox = dict(facecolor='none', edgecolor='gray', boxstyle='round, pad=0.2', lw=1, alpha=0.3)
                 else:
                     bbox = None
+                if isinstance(r_table[irow]['qlflag'], np.int64):
+                    textcolor = OUTTYPES_COLOR['200m']
+                else:
+                    textcolor = OUTTYPES_COLOR['no200m']
                 ax.text(x_pix[irow], y_pix[irow], text, bbox=bbox,
-                        color=OUTTYPES_COLOR[sample], fontsize='5',
-                        horizontalalignment='left', verticalalignment='bottom')
+                        color=textcolor, fontsize=num_fontsize,
+                        horizontalalignment='left', verticalalignment='bottom',
+                        zorder=len(r_table) + 10)
+
+    if len(r_dr3_no200m) > 0:
+        # (X, Y) coordinates
+        ra_array = np.array(r_dr3_no200m['ra'])
+        dec_array = np.array(r_dr3_no200m['dec'])
+        c = SkyCoord(ra=ra_array * u.degree, dec=dec_array * u.degree, frame='icrs')
+        x_pix, y_pix = wcs_image.world_to_pixel(c)
 
-        if sample == 'no200m':
-            # stars outside the -0.5 < G_BP - G_RP < 2.0 colour cut
-            mask_colour = np.logical_or((r_dr3_no200m['bp_rp'] <= -0.5), (r_dr3_no200m['bp_rp'] >= 2.0))
-            if np.any(mask_colour):
-                iok = np.argwhere(mask_colour)
-                ax.scatter(x_pix[iok], y_pix[iok], s=240, marker='D',
-                           facecolors='none', edgecolors='grey', linewidth=0.5)
-
-            # variable stars
-            mask_variable = r_dr3_no200m['phot_variable_flag'] == 'VARIABLE'
-            if np.any(mask_variable):
-                iok = np.argwhere(mask_variable)
-                ax.scatter(x_pix[iok], y_pix[iok], s=240, marker='s',
-                           facecolors='none', edgecolors='blue', linewidth=0.5)
+        # stars outside the -0.5 < G_BP - G_RP < 2.0 colour cut
+        mask_colour = np.logical_or((r_dr3_no200m['bp_rp'] <= -0.5), (r_dr3_no200m['bp_rp'] >= 2.0))
+        if np.any(mask_colour):
+            iok_bool = np.argwhere(mask_colour)
+            ax.scatter(x_pix[iok_bool], y_pix[iok_bool], s=240, marker='D',
+                       facecolors='none', edgecolors='grey', linewidth=0.5, zorder=0)
+
+        # variable stars
+        mask_variable = r_dr3_no200m['phot_variable_flag'] == 'VARIABLE'
+        if np.any(mask_variable):
+            iok_bool = np.argwhere(mask_variable)
+            ax.scatter(x_pix[iok_bool], y_pix[iok_bool], s=240, marker='s',
+                       facecolors='none', edgecolors=OUTTYPES_COLOR['var'], linewidth=0.5, zorder=0)
 
     # legend
     ax.scatter(0.03, 0.96, s=240, marker='s', facecolors='white',
                edgecolors=OUTTYPES_COLOR['var'], linewidth=0.5,
                transform=ax.transAxes)
     ax.text(0.06, 0.96, 'variable in Gaia DR3', fontsize=12, backgroundcolor='white',
             horizontalalignment='left', verticalalignment='center', transform=ax.transAxes)
@@ -154,17 +204,19 @@
     ax.set_xlabel('ra')
     ax.set_ylabel('dec')
 
     ax.set_aspect('equal')
 
     if not nocolor:
         cbaxes = fig.add_axes([0.683, 0.81, 0.15, 0.02])
-        cbar = plt.colorbar(sc, cax=cbaxes, orientation='horizontal', format='%1.0f')
+        norm = mpl.colors.Normalize(vmin=cmap_vmin, vmax=cmap_vmax)
+        cbar = fig.colorbar(mpl.cm.ScalarMappable(norm=norm, cmap=cmap), cax=cbaxes,
+                            orientation='horizontal', format='%1.0f')
         cbar.ax.tick_params(labelsize=12)
-        cbar.set_label(label=r'$G_{\rm BP}-G_{\rm RP}$', size=12, backgroundcolor='white')
+        cbar.set_label(label=r'$G_{\rm BP}-G_{\rm RP}$ (mag)', size=12, backgroundcolor='white')
 
     ax.text(0.98, 0.96, f'Field radius: {search_radius:.4f} degree', fontsize=12, backgroundcolor='white',
             horizontalalignment='right', verticalalignment='center', transform=ax.transAxes)
     ax.text(0.02, 0.06, r'$\alpha_{\rm center}$:', fontsize=12, backgroundcolor='white',
             horizontalalignment='left', verticalalignment='bottom', transform=ax.transAxes)
     ax.text(0.25, 0.06, f'{ra_center:.4f} degree', fontsize=12, backgroundcolor='white',
             horizontalalignment='right', verticalalignment='bottom', transform=ax.transAxes)
```

### Comparing `rgbloom-1.3/rgbloom.egg-info/PKG-INFO` & `rgbloom-1.4/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,7 @@
-Metadata-Version: 2.1
-Name: rgbloom
-Version: 1.3
-Summary: RGB from Gaia EDR3
-Home-page: https://github.com/guaix-ucm/rgbloom
-Author: Nicolás Cardiel
-Author-email: cardiel@ucm.es
-License: GPLv3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Development Status :: 3 - Alpha
-Classifier: Environment :: Console
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Operating System :: OS Independent
-Classifier: Topic :: Scientific/Engineering :: Astronomy
-Description-Content-Type: text/markdown
-Provides-Extra: test
-License-File: LICENSE
-
 # rgbloom
 
 This Python script retrieves RGB magnitudes computed from low resolution
 spectra published in *Gaia* DR3, following the work described in 
 [Carrasco et al. (2023)](#3).
 These magnitudes are given in the standard system defined by
 [Cardiel et al. (2021a)](#1).
@@ -53,31 +31,38 @@
 
 You need to have a live connection to the Internet for 
 the script to work!
 
 ## Installing the code
 
 In order to keep your current Python installation clean, it is highly 
-recommended to install a python 3 *virtual environment* first.
+recommended to first build Python 3 *virtual environment*.
 
-### Creating and activating the python virtual environment
+### Creating and activating the Python virtual environment
 
 ```bash
 $ python3 -m venv venv_rgb
 $ . venv_rgb/bin/activate
 (venv_rgb) $
 ```
 
 ### Installing the package
 
+We recommend installing the latest stable version, which is available via
+the PyPI respository:
+
 ```bash
-(venv_rgb) $ pip install git+https://github.com/guaix-ucm/rgbloom.git@main#egg=rgbloom
+(venv_rgb) $ pip install rgbloom
 ```
 
+The latest development version is available through GitHub:
 
+```bash
+(venv_rgb) $ pip install git+https://github.com/guaix-ucm/rgbloom.git@main#egg=rgbloom
+```
 
 ## Executing the program
 
 Just execute it from the command line:
 
 ```bash
 (venv_rgb) $ rgbloom 56.66 24.10 1.0 12
@@ -96,15 +81,15 @@
 recover disk space).
 
 The execution of this example should led to the following output in the
 terminal (except for the absolute path where the auxiliary downloaded files 
 are stored):
 
 ```
-        Welcome to rgbloom version 1.2
+        Welcome to rgbloom version 1.4
         ==============================
 
 Downloading data from 'http://nartex.fis.ucm.es/~ncl/rgbphot/gaiaDR3/reference_healpix8.csv' to file '/Users/cardiel/Library/Caches/pooch/635cd722cf61b23bd8eee20635e4d580-reference_healpix8.csv'.
 <STEP1> Starting cone search in Gaia DR3... (please wait)
   INFO: Query finished. [astroquery.utils.tap.core]
         --> 310 objects found
         --> 23 objects classified as VARIABLE
@@ -188,15 +173,15 @@
       - `RGB_R`: red RGB magnitude estimate
 
   The list of objects in these two files is sorted by right ascension.
 
 - Step 6: generation of a finding chart plot (in PDF format): `rgbloom.pdf`. 
   The execution of the previous example generates a cone search around 
   the [Pleiades](https://en.wikipedia.org/wiki/Pleiades) star cluster:
-  ![Pleiades plot](http://nartex.hst.ucm.es/~ncl/rgbphot/gaiaDR3/pleiades_v5.png)
+  ![Pleiades plot](http://nartex.hst.ucm.es/~ncl/rgbphot/gaiaDR3/pleiades_v6.png)
   The objects in this plot are color coded based on the *Gaia* G_BP - G_RP 
   colour. Stars brighter than a pre-defined threshold are displayed 
   with big star symbols. To facilitate the identification of each object, the
   consecutive identification numbers in the two files `rgbloom_200m.csv` and
   `rgbloom_no200m.csv` are also displayed, in red
   and black, respectively. The identification numbers corresponding to the less
   reliable sources in `rgbloom_20m.csv` (`qlflag=1`) appear inside a rectangle
@@ -216,30 +201,42 @@
 ### Additional help
 
 Some auxiliary optional arguments are also available. See description 
 invoking the script help:
 
 ```bash
 $ rgbloom --help
+usage: rgbloom [-h] [--basename BASENAME] [--brightlimit BRIGHTLIMIT] [--symbsize SYMBSIZE] [--max_symbsize MAX_SYMBSIZE]
+               [--min_symbsize MIN_SYMBSIZE] [--mag_power MAG_POWER] [--display_g_mag] [--num_fontsize NUM_FONTSIZE]
+               [--nonumbers] [--noplot] [--nocolor] [--verbose]
+               ra_center dec_center search_radius g_limit
 
-...
-...
+RGB predictions from Gaia DR3 spectrophotometry (version 1.4)
 
 positional arguments:
   ra_center             right Ascension (decimal degrees)
   dec_center            declination (decimal degrees)
   search_radius         search radius (decimal degrees)
   g_limit               limiting Gaia G magnitude
 
 optional arguments:
   -h, --help            show this help message and exit
   --basename BASENAME   file basename for output files
   --brightlimit BRIGHTLIMIT
                         objects brighter than this Gaia G limit are displayed with star symbols (default=8.0)
-  --symbsize SYMBSIZE   multiplying factor for symbol size (default=1.0)
+  --symbsize SYMBSIZE   global multiplying factor for symbol size (default=1.0)
+  --max_symbsize MAX_SYMBSIZE
+                        maximum symbol size in chart (default=1000)
+  --min_symbsize MIN_SYMBSIZE
+                        minimum symbol size in chart (default=10)
+  --mag_power MAG_POWER
+                        power to scale symbol sizes in chart (default=3)
+  --display_g_mag       display Gaia G magnitude instead of object number
+  --num_fontsize NUM_FONTSIZE
+                        font size for numbers in chart (default=5)
   --nonumbers           do not display object identification number in PDF chart
   --noplot              skip PDF chart generation
   --nocolor             do not use colors in PDF chart
   --verbose             increase program verbosity
 ```
 
 ## Citation
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `rgbloom-1.3/setup.cfg` & `rgbloom-1.4/setup.cfg`

 * *Files identical despite different names*

