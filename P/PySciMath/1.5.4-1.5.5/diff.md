# Comparing `tmp/PySciMath-1.5.4.tar.gz` & `tmp/PySciMath-1.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PySciMath-1.5.4.tar", last modified: Sat May 20 11:55:54 2023, max compression
+gzip compressed data, was "PySciMath-1.5.5.tar", last modified: Mon May 22 12:53:15 2023, max compression
```

## Comparing `PySciMath-1.5.4.tar` & `PySciMath-1.5.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-05-20 11:55:54.351907 PySciMath-1.5.4/
--rw-rw-rw-   0        0        0     1091 2023-05-10 06:48:15.000000 PySciMath-1.5.4/LICENSE.txt
--rw-rw-rw-   0        0        0       38 2023-05-14 06:30:09.000000 PySciMath-1.5.4/MANIFEST.in
--rw-rw-rw-   0        0        0     2611 2023-05-20 11:55:54.349910 PySciMath-1.5.4/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-20 11:55:54.334072 PySciMath-1.5.4/PySciMath/
--rw-rw-rw-   0        0        0     2667 2023-05-20 11:39:33.000000 PySciMath-1.5.4/PySciMath/Arithmetic.py
--rw-rw-rw-   0        0        0    22263 2023-05-20 11:31:14.000000 PySciMath-1.5.4/PySciMath/Geometry.py
--rw-rw-rw-   0        0        0      598 2023-05-12 03:54:25.000000 PySciMath-1.5.4/PySciMath/Quadratic.py
--rw-rw-rw-   0        0        0     1266 2023-05-20 11:31:27.000000 PySciMath-1.5.4/PySciMath/Statistics.py
--rw-rw-rw-   0        0        0      558 2023-05-12 06:07:57.000000 PySciMath-1.5.4/PySciMath/Trigonometry.py
--rw-rw-rw-   0        0        0       59 2023-05-10 14:22:13.000000 PySciMath-1.5.4/PySciMath/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-20 11:55:54.347916 PySciMath-1.5.4/PySciMath.egg-info/
--rw-rw-rw-   0        0        0     2611 2023-05-20 11:55:54.000000 PySciMath-1.5.4/PySciMath.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      315 2023-05-20 11:55:54.000000 PySciMath-1.5.4/PySciMath.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-20 11:55:54.000000 PySciMath-1.5.4/PySciMath.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-05-20 11:55:54.000000 PySciMath-1.5.4/PySciMath.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2077 2023-05-20 11:50:42.000000 PySciMath-1.5.4/README.md
--rw-rw-rw-   0        0        0       42 2023-05-20 11:55:54.351907 PySciMath-1.5.4/setup.cfg
--rw-rw-rw-   0        0        0      929 2023-05-20 11:54:07.000000 PySciMath-1.5.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-22 12:53:15.935040 PySciMath-1.5.5/
+-rw-rw-rw-   0        0        0     1091 2023-05-10 06:48:15.000000 PySciMath-1.5.5/LICENSE.txt
+-rw-rw-rw-   0        0        0       38 2023-05-14 06:30:09.000000 PySciMath-1.5.5/MANIFEST.in
+-rw-rw-rw-   0        0        0     2616 2023-05-22 12:53:15.933045 PySciMath-1.5.5/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-22 12:53:15.887648 PySciMath-1.5.5/PySciMath/
+-rw-rw-rw-   0        0        0     2663 2023-05-22 12:48:50.000000 PySciMath-1.5.5/PySciMath/Arithmetic.py
+-rw-rw-rw-   0        0        0    22259 2023-05-22 12:49:01.000000 PySciMath-1.5.5/PySciMath/Geometry.py
+-rw-rw-rw-   0        0        0      594 2023-05-22 12:49:09.000000 PySciMath-1.5.5/PySciMath/Quadratic.py
+-rw-rw-rw-   0        0        0     1262 2023-05-22 12:49:15.000000 PySciMath-1.5.5/PySciMath/Statistics.py
+-rw-rw-rw-   0        0        0      554 2023-05-22 12:49:19.000000 PySciMath-1.5.5/PySciMath/Trigonometry.py
+-rw-rw-rw-   0        0        0       59 2023-05-10 14:22:13.000000 PySciMath-1.5.5/PySciMath/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-22 12:53:15.930116 PySciMath-1.5.5/PySciMath.egg-info/
+-rw-rw-rw-   0        0        0     2616 2023-05-22 12:53:15.000000 PySciMath-1.5.5/PySciMath.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      315 2023-05-22 12:53:15.000000 PySciMath-1.5.5/PySciMath.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-22 12:53:15.000000 PySciMath-1.5.5/PySciMath.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-05-22 12:53:15.000000 PySciMath-1.5.5/PySciMath.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2081 2023-05-22 12:51:51.000000 PySciMath-1.5.5/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-22 12:53:15.935040 PySciMath-1.5.5/setup.cfg
+-rw-rw-rw-   0        0        0      930 2023-05-22 12:51:47.000000 PySciMath-1.5.5/setup.py
```

### Comparing `PySciMath-1.5.4/LICENSE.txt` & `PySciMath-1.5.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `PySciMath-1.5.4/PKG-INFO` & `PySciMath-1.5.5/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 Metadata-Version: 2.1
 Name: PySciMath
-Version: 1.5.4
-Summary: PySciMath is a general-purpose Python module to work on calculations and solve mathmematical and scientific problems.
+Version: 1.5.5
+Summary: PySciMath is a general-purpose Python package to work on calculations and solve mathmematical and scientific problems.
 Home-page: https://github.com/Anikethc/PySciMath
 Download-URL: https://pypi.org/project/PySciMath
 Author: Aniketh Chavare
 Author-email: anikethchavare@outlook.com
 License: MIT
 Keywords: Math,Mathematics,Science,Calculations
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # PySciMath
 
 ## Introduction
 
-PySciMath is a general-purpose Python module to work on calculations and solve mathematical and scientific problems.
+PySciMath is a general-purpose Python package to work on calculations and solve mathematical and scientific problems.
 
 Read the docs on GitBook [here](https://aniketh-chavare.gitbook.io/pyscimath-docs).
 
-## Module Information
+## Package Information
 
 **Name** - PySciMath</br>
-**Version** - 1.5.4</br>
-**Description** - PySciMath is a general-purpose Python module to work on calculations and solve mathematical and scientific problems.</br>
+**Version** - 1.5.5</br>
+**Description** - PySciMath is a general-purpose Python package to work on calculations and solve mathematical and scientific problems.</br>
 **Author** - Aniketh Chavare</br>
 **GitHub URL** - [https://github.com/Anikethc/PySciMath](https://github.com/Anikethc/PySciMath)</br>
 **Pypi.org URL** - [https://pypi.org/project/PySciMath](https://pypi.org/project/PySciMath)</br>
 **Docs URL** - [https://aniketh-chavare.gitbook.io/pyscimath-docs](https://aniketh-chavare.gitbook.io/pyscimath-docs)
 
 ## License
 
@@ -55,8 +55,8 @@
 
 ## Issues & Bugs
 
 If you encounter any issues or bugs, visit the 'Issues' tab and create an issue. I'll look into it and resolve it ASAP.
 
 ## Conclusion
 
-I hope you liked this module. Thank you!
+I hope you liked this package. Thank you!
```

### Comparing `PySciMath-1.5.4/PySciMath/Arithmetic.py` & `PySciMath-1.5.5/PySciMath/Arithmetic.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # PySciMath - Arithmetic
 
-''' This is the "Arithmetic" sub-module. '''
+''' This is the "Arithmetic" module. '''
 
 # Imports
 import cmath
 
 # Constants
 iota = "Iota is also referred to as 'i'. It's value is √-1."
```

### Comparing `PySciMath-1.5.4/PySciMath/Geometry.py` & `PySciMath-1.5.5/PySciMath/Geometry.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # PySciMath - Geometry
 
-''' This is the "Geometry" sub-module. '''
+''' This is the "Geometry" module. '''
 
 # Imports
 import Arithmetic
 
 # Constants
 pi = 3.14159
 goldenRatio = 1.61803
```

### Comparing `PySciMath-1.5.4/PySciMath/Quadratic.py` & `PySciMath-1.5.5/PySciMath/Quadratic.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # PySciMath - Quadratic
 
-''' This is the "Quadratic" sub-module. '''
+''' This is the "Quadratic" module. '''
 
 # Imports
 import Arithmetic
 
 # Function 1 - Find Discriminant
 def findDiscriminant(a, b, c):
     newA = float(a)
```

### Comparing `PySciMath-1.5.4/PySciMath/Statistics.py` & `PySciMath-1.5.5/PySciMath/Statistics.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # PySciMath - Statistics
 
-''' This is the "Statistics" sub-module. '''
+''' This is the "Statistics" module. '''
 
 # Function 1 - Mean
 def mean(data):
     if isinstance(data, (list, tuple, set)):
         if (data != None and sum(data) != 0):
             return sum(data) / len(data)
         else:
```

### Comparing `PySciMath-1.5.4/PySciMath/Trigonometry.py` & `PySciMath-1.5.5/PySciMath/Trigonometry.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # PySciMath - Trigonometry
 
-''' This is the "Trigonometry" sub-module. '''
+''' This is the "Trigonometry" module. '''
 
 # Imports
 import math
 
 # Functions - Conversions
 def degreesToRadians(degrees): return degrees * (3.14/180)
 def radiansToDegrees(radians): return radians * (180/3.14)
```

### Comparing `PySciMath-1.5.4/PySciMath.egg-info/PKG-INFO` & `PySciMath-1.5.5/PySciMath.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 Metadata-Version: 2.1
 Name: PySciMath
-Version: 1.5.4
-Summary: PySciMath is a general-purpose Python module to work on calculations and solve mathmematical and scientific problems.
+Version: 1.5.5
+Summary: PySciMath is a general-purpose Python package to work on calculations and solve mathmematical and scientific problems.
 Home-page: https://github.com/Anikethc/PySciMath
 Download-URL: https://pypi.org/project/PySciMath
 Author: Aniketh Chavare
 Author-email: anikethchavare@outlook.com
 License: MIT
 Keywords: Math,Mathematics,Science,Calculations
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # PySciMath
 
 ## Introduction
 
-PySciMath is a general-purpose Python module to work on calculations and solve mathematical and scientific problems.
+PySciMath is a general-purpose Python package to work on calculations and solve mathematical and scientific problems.
 
 Read the docs on GitBook [here](https://aniketh-chavare.gitbook.io/pyscimath-docs).
 
-## Module Information
+## Package Information
 
 **Name** - PySciMath</br>
-**Version** - 1.5.4</br>
-**Description** - PySciMath is a general-purpose Python module to work on calculations and solve mathematical and scientific problems.</br>
+**Version** - 1.5.5</br>
+**Description** - PySciMath is a general-purpose Python package to work on calculations and solve mathematical and scientific problems.</br>
 **Author** - Aniketh Chavare</br>
 **GitHub URL** - [https://github.com/Anikethc/PySciMath](https://github.com/Anikethc/PySciMath)</br>
 **Pypi.org URL** - [https://pypi.org/project/PySciMath](https://pypi.org/project/PySciMath)</br>
 **Docs URL** - [https://aniketh-chavare.gitbook.io/pyscimath-docs](https://aniketh-chavare.gitbook.io/pyscimath-docs)
 
 ## License
 
@@ -55,8 +55,8 @@
 
 ## Issues & Bugs
 
 If you encounter any issues or bugs, visit the 'Issues' tab and create an issue. I'll look into it and resolve it ASAP.
 
 ## Conclusion
 
-I hope you liked this module. Thank you!
+I hope you liked this package. Thank you!
```

### Comparing `PySciMath-1.5.4/README.md` & `PySciMath-1.5.5/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 # PySciMath
 
 ## Introduction
 
-PySciMath is a general-purpose Python module to work on calculations and solve mathematical and scientific problems.
+PySciMath is a general-purpose Python package to work on calculations and solve mathematical and scientific problems.
 
 Read the docs on GitBook [here](https://aniketh-chavare.gitbook.io/pyscimath-docs).
 
-## Module Information
+## Package Information
 
 **Name** - PySciMath</br>
-**Version** - 1.5.4</br>
-**Description** - PySciMath is a general-purpose Python module to work on calculations and solve mathematical and scientific problems.</br>
+**Version** - 1.5.5</br>
+**Description** - PySciMath is a general-purpose Python package to work on calculations and solve mathematical and scientific problems.</br>
 **Author** - Aniketh Chavare</br>
 **GitHub URL** - [https://github.com/Anikethc/PySciMath](https://github.com/Anikethc/PySciMath)</br>
 **Pypi.org URL** - [https://pypi.org/project/PySciMath](https://pypi.org/project/PySciMath)</br>
 **Docs URL** - [https://aniketh-chavare.gitbook.io/pyscimath-docs](https://aniketh-chavare.gitbook.io/pyscimath-docs)
 
 ## License
 
@@ -42,8 +42,8 @@
 
 ## Issues & Bugs
 
 If you encounter any issues or bugs, visit the 'Issues' tab and create an issue. I'll look into it and resolve it ASAP.
 
 ## Conclusion
 
-I hope you liked this module. Thank you!
+I hope you liked this package. Thank you!
```

### Comparing `PySciMath-1.5.4/setup.py` & `PySciMath-1.5.5/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,16 +8,16 @@
 # README.md
 with open("README.md") as readme_file:
     README = readme_file.read()
 
 # Setup Arguements
 setup_args = dict (
     name="PySciMath",
-    version="1.5.4",
-    description="PySciMath is a general-purpose Python module to work on calculations and solve mathmematical and scientific problems.",
+    version="1.5.5",
+    description="PySciMath is a general-purpose Python package to work on calculations and solve mathmematical and scientific problems.",
     long_description_content_type="text/markdown",
     long_description=README,
     license="MIT",
     packages=find_packages(),
     include_package_data=True,
     author="Aniketh Chavare",
     author_email="anikethchavare@outlook.com",
```

