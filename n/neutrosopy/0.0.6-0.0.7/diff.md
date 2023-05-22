# Comparing `tmp/neutrosopy-0.0.6.tar.gz` & `tmp/neutrosopy-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neutrosopy-0.0.6.tar", last modified: Mon May 22 03:22:34 2023, max compression
+gzip compressed data, was "neutrosopy-0.0.7.tar", last modified: Mon May 22 04:04:23 2023, max compression
```

## Comparing `neutrosopy-0.0.6.tar` & `neutrosopy-0.0.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 galen     (1000) galen     (1000)        0 2023-05-22 03:22:34.608807 neutrosopy-0.0.6/
--rw-rw-r--   0 galen     (1000) galen     (1000)    35149 2023-05-22 02:18:04.000000 neutrosopy-0.0.6/LICENSE
--rw-rw-r--   0 galen     (1000) galen     (1000)      631 2023-05-22 03:22:34.608807 neutrosopy-0.0.6/PKG-INFO
--rw-rw-r--   0 galen     (1000) galen     (1000)       67 2023-05-22 02:18:04.000000 neutrosopy-0.0.6/README.md
--rw-rw-r--   0 galen     (1000) galen     (1000)      638 2023-05-22 03:21:47.000000 neutrosopy-0.0.6/pyproject.toml
--rw-rw-r--   0 galen     (1000) galen     (1000)       38 2023-05-22 03:22:34.608807 neutrosopy-0.0.6/setup.cfg
-drwxrwxr-x   0 galen     (1000) galen     (1000)        0 2023-05-22 03:22:34.604807 neutrosopy-0.0.6/src/
-drwxrwxr-x   0 galen     (1000) galen     (1000)        0 2023-05-22 03:22:34.604807 neutrosopy-0.0.6/src/neutrosopy/
--rw-rw-r--   0 galen     (1000) galen     (1000)       28 2023-05-22 03:16:26.000000 neutrosopy-0.0.6/src/neutrosopy/__init__.py
--rw-rw-r--   0 galen     (1000) galen     (1000)    15188 2023-05-22 02:53:44.000000 neutrosopy-0.0.6/src/neutrosopy/neutrosophic.py
-drwxrwxr-x   0 galen     (1000) galen     (1000)        0 2023-05-22 03:22:34.604807 neutrosopy-0.0.6/src/neutrosopy.egg-info/
--rw-rw-r--   0 galen     (1000) galen     (1000)      631 2023-05-22 03:22:34.000000 neutrosopy-0.0.6/src/neutrosopy.egg-info/PKG-INFO
--rw-rw-r--   0 galen     (1000) galen     (1000)      276 2023-05-22 03:22:34.000000 neutrosopy-0.0.6/src/neutrosopy.egg-info/SOURCES.txt
--rw-rw-r--   0 galen     (1000) galen     (1000)        1 2023-05-22 03:22:34.000000 neutrosopy-0.0.6/src/neutrosopy.egg-info/dependency_links.txt
--rw-rw-r--   0 galen     (1000) galen     (1000)       11 2023-05-22 03:22:34.000000 neutrosopy-0.0.6/src/neutrosopy.egg-info/top_level.txt
-drwxrwxr-x   0 galen     (1000) galen     (1000)        0 2023-05-22 03:22:34.604807 neutrosopy-0.0.6/tests/
--rw-rw-r--   0 galen     (1000) galen     (1000)     1589 2023-05-22 02:29:06.000000 neutrosopy-0.0.6/tests/test_neutrosophic_number.py
+drwxrwxr-x   0 galen     (1000) galen     (1000)        0 2023-05-22 04:04:23.405627 neutrosopy-0.0.7/
+-rw-rw-r--   0 galen     (1000) galen     (1000)    35149 2023-05-22 02:18:04.000000 neutrosopy-0.0.7/LICENSE
+-rw-rw-r--   0 galen     (1000) galen     (1000)      631 2023-05-22 04:04:23.405627 neutrosopy-0.0.7/PKG-INFO
+-rw-rw-r--   0 galen     (1000) galen     (1000)       67 2023-05-22 02:18:04.000000 neutrosopy-0.0.7/README.md
+-rw-rw-r--   0 galen     (1000) galen     (1000)      638 2023-05-22 04:03:48.000000 neutrosopy-0.0.7/pyproject.toml
+-rw-rw-r--   0 galen     (1000) galen     (1000)       38 2023-05-22 04:04:23.405627 neutrosopy-0.0.7/setup.cfg
+drwxrwxr-x   0 galen     (1000) galen     (1000)        0 2023-05-22 04:04:23.393627 neutrosopy-0.0.7/src/
+drwxrwxr-x   0 galen     (1000) galen     (1000)        0 2023-05-22 04:04:23.401627 neutrosopy-0.0.7/src/neutrosopy/
+-rw-rw-r--   0 galen     (1000) galen     (1000)       28 2023-05-22 03:16:26.000000 neutrosopy-0.0.7/src/neutrosopy/__init__.py
+-rw-rw-r--   0 galen     (1000) galen     (1000)    15120 2023-05-22 03:58:35.000000 neutrosopy-0.0.7/src/neutrosopy/neutrosophic.py
+drwxrwxr-x   0 galen     (1000) galen     (1000)        0 2023-05-22 04:04:23.405627 neutrosopy-0.0.7/src/neutrosopy.egg-info/
+-rw-rw-r--   0 galen     (1000) galen     (1000)      631 2023-05-22 04:04:23.000000 neutrosopy-0.0.7/src/neutrosopy.egg-info/PKG-INFO
+-rw-rw-r--   0 galen     (1000) galen     (1000)      276 2023-05-22 04:04:23.000000 neutrosopy-0.0.7/src/neutrosopy.egg-info/SOURCES.txt
+-rw-rw-r--   0 galen     (1000) galen     (1000)        1 2023-05-22 04:04:23.000000 neutrosopy-0.0.7/src/neutrosopy.egg-info/dependency_links.txt
+-rw-rw-r--   0 galen     (1000) galen     (1000)       11 2023-05-22 04:04:23.000000 neutrosopy-0.0.7/src/neutrosopy.egg-info/top_level.txt
+drwxrwxr-x   0 galen     (1000) galen     (1000)        0 2023-05-22 04:04:23.405627 neutrosopy-0.0.7/tests/
+-rw-rw-r--   0 galen     (1000) galen     (1000)     1589 2023-05-22 02:29:06.000000 neutrosopy-0.0.7/tests/test_neutrosophic_number.py
```

### Comparing `neutrosopy-0.0.6/LICENSE` & `neutrosopy-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `neutrosopy-0.0.6/PKG-INFO` & `neutrosopy-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neutrosopy
-Version: 0.0.6
+Version: 0.0.7
 Summary: Class and utility functions for working with algebraic neutrosophic numbers.
 Author-email: Galen Seilis <galen.seilis@seilis.ca>
 Project-URL: Homepage, https://github.com/galenseilis/neutrosopy
 Project-URL: Bug Tracker, https://github.com/galenseilis/neutrosopy/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `neutrosopy-0.0.6/pyproject.toml` & `neutrosopy-0.0.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "neutrosopy"
-version = "0.0.6"
+version = "0.0.7"
 authors = [
   { name="Galen Seilis", email="galen.seilis@seilis.ca" },
 ]
 description = "Class and utility functions for working with algebraic neutrosophic numbers."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `neutrosopy-0.0.6/src/neutrosopy/neutrosophic.py` & `neutrosopy-0.0.7/src/neutrosopy/neutrosophic.py`

 * *Files 8% similar despite different names*

```diff
@@ -319,110 +319,107 @@
             Z[i] = Z[i] + NeutrosophicNumber(X[i], 0)
     else:
         for i in range(X.shape[0]):
             Z[i] = Z[i] + NeutrosophicNumber(0, X[i])
     return Z
 
 
-def nexp(x, order=10):
+def nexp(x):
     """
     Compute the neutrosophic exponential function approximation using its Maclaurin series.
 
     Parameters:
     -----------
     x : numeric
         The value at which to evaluate the neutrosophic exponential function.
 
-    order : int, optional
-        The order of the Maclaurin series used for the approximation.
-        Default is 10.
-
     Returns:
     --------
     NeutrosophicNumber
         A neutrosophic number representing the approximation of the neutrosophic exponential function.
 
     Notes:
     ------
     - The neutrosophic exponential function is approximated using its Maclaurin series.
-    - The Maclaurin series is truncated at the specified 'order'.
     - The function computes the sum of the terms in the Maclaurin series approximation.
     - The resulting sum is returned as a neutrosophic number.
     - The neutrosophic number is represented using the NeutrosophicNumber class.
 
     Examples:
     ---------
     >>> nexp(1)
     2+1I
 
-    >>> nexp(2, order=5)
+    >>> nexp(2)
     7+4.333333333333333I
     """
-    return np.sum([(x**k) / math.factorial(k) for k in range(order)])
+    result = NeutrosophicNumber(0.0, 0.0)
+    k = 0
+    while True:
+        new_result = result + (x**k) / math.factorial(k)
+        if new_result == result:
+            return result
+        else:
+            result = new_result
+            k += 1
 
 
-def nsin(x, order=10):
+def nsin(x):
     """
     Compute the neutrosophic sine function approximation using its Maclaurin series.
 
     Parameters:
     -----------
     x : numeric
         The value at which to evaluate the neutrosophic sine function.
 
-    order : int, optional
-        The order of the Maclaurin series used for the approximation.
-        Default is 10.
-
     Returns:
     --------
     NeutrosophicNumber
         A neutrosophic number representing the approximation of the neutrosophic sine function.
 
     Notes:
     ------
     - The neutrosophic sine function is approximated using its Maclaurin series.
-    - The Maclaurin series is truncated at the specified 'order'.
     - The function computes the sum of the terms in the Maclaurin series approximation.
     - The resulting sum is returned as a neutrosophic number.
     - The neutrosophic number is represented using the NeutrosophicNumber class.
 
     Examples:
     ---------
     >>> nsin(0)
     0+0I
 
     >>> nsin(1)
     1.1666666666666665+1.1752011936438014I
 
-    >>> nsin(2, order=5)
+    >>> nsin(2)
     -0.9333333333333332+3.9933992677987827I
     """
-    return np.sum(
-        [
-            (-1) ** k * (x ** (2 * k + 1)) / math.factorial(2 * k + 1)
-            for k in range(order)
-        ]
-    )
+    result = NeutrosophicNumber(0.0, 0.0)
+    k = 0
+    while True:
+        new_result = result + (-1) ** k * (x ** (2 * k + 1)) / math.factorial(2 * k + 1)
+        if new_result == result:
+            return result
+        else:
+            result = new_result
+            k += 1
 
 
-def nln(x, order=10):
+def nln(x):
     """
     Compute the neutrosophic natural logarithm function approximation using
     a series based on the area hyperbolic tangent function.
 
     Parameters:
     -----------
     x : numeric
         The value at which to evaluate the neutrosophic natural logarithm function.
 
-    order : int, optional
-        The order of the series used for the approximation.
-        Default is 10.
-
     Returns:
     --------
     NeutrosophicNumber
         A neutrosophic number representing the approximation of the neutrosophic natural logarithm function.
 
     Notes:
     ------
@@ -436,13 +433,19 @@
     ---------
     >>> nln(1)
     0+0I
 
     >>> nln(2)
     1.0986122886681098+1.5707963267948966I
 
-    >>> nln(3, order=5)
+    >>> nln(3)
     1.1752011936438014+1.5040773967762742I
     """
-    return 2 * np.sum(
-        [((x - 1) / (x + 1)) ** (2 * k + 1) / (2 * k + 1) for k in range(order)]
-    )
+    result = NeutrosophicNumber(0.0, 0.0)
+    k = 0
+    while True:
+        new_result = result + ((x - 1) / (x + 1)) ** (2 * k + 1) / (2 * k + 1)
+        if new_result == result:
+            return result
+        else:
+            result = new_result
+            k += 1
```

### Comparing `neutrosopy-0.0.6/src/neutrosopy.egg-info/PKG-INFO` & `neutrosopy-0.0.7/src/neutrosopy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neutrosopy
-Version: 0.0.6
+Version: 0.0.7
 Summary: Class and utility functions for working with algebraic neutrosophic numbers.
 Author-email: Galen Seilis <galen.seilis@seilis.ca>
 Project-URL: Homepage, https://github.com/galenseilis/neutrosopy
 Project-URL: Bug Tracker, https://github.com/galenseilis/neutrosopy/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `neutrosopy-0.0.6/tests/test_neutrosophic_number.py` & `neutrosopy-0.0.7/tests/test_neutrosophic_number.py`

 * *Files identical despite different names*

