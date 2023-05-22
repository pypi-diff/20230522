# Comparing `tmp/PyEng-1.0.1.tar.gz` & `tmp/PyEng-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyEng-1.0.1.tar", last modified: Sat May 20 15:26:04 2023, max compression
+gzip compressed data, was "PyEng-1.0.2.tar", last modified: Mon May 22 12:57:52 2023, max compression
```

## Comparing `PyEng-1.0.1.tar` & `PyEng-1.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-20 15:26:04.727933 PyEng-1.0.1/
--rw-rw-rw-   0        0        0     1091 2023-05-16 07:22:16.000000 PyEng-1.0.1/LICENSE.txt
--rw-rw-rw-   0        0        0       76 2023-05-20 14:00:41.000000 PyEng-1.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0     2475 2023-05-20 15:26:04.726936 PyEng-1.0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-20 15:26:04.653131 PyEng-1.0.1/PyEng/
--rw-rw-rw-   0        0        0     1669 2023-05-20 14:36:30.000000 PyEng-1.0.1/PyEng/Words.py
--rw-rw-rw-   0        0        0       55 2023-05-20 14:01:19.000000 PyEng-1.0.1/PyEng/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-20 15:26:04.668093 PyEng-1.0.1/PyEng/data/
--rw-rw-rw-   0        0        0 22970019 2023-05-20 13:53:02.000000 PyEng-1.0.1/PyEng/data/dictionary.json
-drwxrwxrwx   0        0        0        0 2023-05-20 15:26:04.666098 PyEng-1.0.1/PyEng.egg-info/
--rw-rw-rw-   0        0        0     2475 2023-05-20 15:26:04.000000 PyEng-1.0.1/PyEng.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      218 2023-05-20 15:26:04.000000 PyEng-1.0.1/PyEng.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-20 15:26:04.000000 PyEng-1.0.1/PyEng.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-05-20 15:26:04.000000 PyEng-1.0.1/PyEng.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2003 2023-05-20 15:24:53.000000 PyEng-1.0.1/README.md
--rw-rw-rw-   0        0        0       42 2023-05-20 15:26:04.728929 PyEng-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      854 2023-05-20 15:24:56.000000 PyEng-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-22 12:57:52.848610 PyEng-1.0.2/
+-rw-rw-rw-   0        0        0     1091 2023-05-16 07:22:16.000000 PyEng-1.0.2/LICENSE.txt
+-rw-rw-rw-   0        0        0       76 2023-05-20 14:00:41.000000 PyEng-1.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     2480 2023-05-22 12:57:52.845618 PyEng-1.0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-22 12:57:52.533641 PyEng-1.0.2/PyEng/
+-rw-rw-rw-   0        0        0     1668 2023-05-22 12:56:48.000000 PyEng-1.0.2/PyEng/Words.py
+-rw-rw-rw-   0        0        0       55 2023-05-20 14:01:19.000000 PyEng-1.0.2/PyEng/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-22 12:57:52.574556 PyEng-1.0.2/PyEng/data/
+-rw-rw-rw-   0        0        0 22970019 2023-05-20 13:53:02.000000 PyEng-1.0.2/PyEng/data/dictionary.json
+drwxrwxrwx   0        0        0        0 2023-05-22 12:57:52.570329 PyEng-1.0.2/PyEng.egg-info/
+-rw-rw-rw-   0        0        0     2480 2023-05-22 12:57:52.000000 PyEng-1.0.2/PyEng.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      218 2023-05-22 12:57:52.000000 PyEng-1.0.2/PyEng.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-22 12:57:52.000000 PyEng-1.0.2/PyEng.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-05-22 12:57:52.000000 PyEng-1.0.2/PyEng.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2007 2023-05-22 12:54:56.000000 PyEng-1.0.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-22 12:57:52.849607 PyEng-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      855 2023-05-22 12:55:27.000000 PyEng-1.0.2/setup.py
```

### Comparing `PyEng-1.0.1/LICENSE.txt` & `PyEng-1.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `PyEng-1.0.1/PKG-INFO` & `PyEng-1.0.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 Metadata-Version: 2.1
 Name: PyEng
-Version: 1.0.1
-Summary: PyEng is a general-purpose Python module that contains functions related to the English language.
+Version: 1.0.2
+Summary: PyEng is a general-purpose Python package that contains functions related to the English language.
 Home-page: https://github.com/Anikethc/PyEng
 Download-URL: https://pypi.org/project/PyEng
 Author: Aniketh Chavare
 Author-email: anikethchavare@outlook.com
 License: MIT
 Keywords: English
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # PyEng
 
 ## Introduction
 
-PyEng is a general-purpose Python module that contains functions related to the English language.
+PyEng is a general-purpose Python package that contains functions related to the English language.
 
 Read the docs on GitBook [here](https://aniketh-chavare.gitbook.io/pyeng-docs).
 
-## Module Information
+## Package Information
 
 **Name** - PyEng</br>
-**Version** - 1.0.1</br>
-**Description** - PyEng is a general-purpose Python module that contains functions related to the English language.</br>
+**Version** - 1.0.2</br>
+**Description** - PyEng is a general-purpose Python package that contains functions related to the English language.</br>
 **Author** - Aniketh Chavare</br>
 **GitHub URL** - [https://github.com/Anikethc/PyEng](https://github.com/Anikethc/PyEng)</br>
 **Pypi.org URL** - [https://pypi.org/project/PyEng](https://pypi.org/project/PyEng)</br>
 **Docs URL** - [https://aniketh-chavare.gitbook.io/pyeng-docs](https://aniketh-chavare.gitbook.io/pyeng-docs)
 
 ## License
 
@@ -55,8 +55,8 @@
 
 ## Issues & Bugs
 
 If you encounter any issues or bugs, visit the 'Issues' tab and create an issue. I'll look into it and resolve it ASAP.
 
 ## Conclusion
 
-I hope you liked this module. Thank you!
+I hope you liked this package. Thank you!
```

### Comparing `PyEng-1.0.1/PyEng/Words.py` & `PyEng-1.0.2/PyEng/Words.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,31 +1,30 @@
 # PyEng - Words
 
-''' This is the "Words" sub-module. '''
+''' This is the "Words" module. '''
 
 # Imports
 import os
 from difflib import get_close_matches
 import json
 
 # Set Directory
-directory = os.path.dirname(os.path.realpath(__file__))
-directory = directory.replace(os.sep, "/")
+directory = os.path.dirname(os.path.realpath(__file__)).replace(os.sep, "/")
 
 # Variables
 dictionaryJSON = json.load(open(directory + "/data/dictionary.json", encoding="utf8"))
 
 # Function 1 - Meaning
 def meaning(word):
-    # Check Data Type
+    # Checking the Data Type
     if (isinstance(word, str)):
-        # Convert to Lower Case
+        # Converting to Lower Case
         word = word.lower()
 
-        # Check for Meaning
+        # Checking for Meaning
         if (word in dictionaryJSON):
             return dictionaryJSON[word]
         elif (len(get_close_matches(word, dictionaryJSON.keys())) > 0):
             return "Did you mean '{0}' instead? Try it again with the correct word.".format(get_close_matches(word, dictionaryJSON.keys())[0])
         else:
             return "The word doesn't exist. Please try again."
     else:
@@ -33,20 +32,20 @@
 
 # Function 2 - Anagram
 def anagram(string1, string2):
     # Nested Functions
     def lengthOfStrings(a, b): return len(a) == len(b)
     def sortStrings(a, b): return sorted(a) == sorted(b)
 
-    # Check Data Type
+    # Checking the Data Type
     if (isinstance(string1, str) and isinstance(string2, str)):
-        # Convert to Lower Case
+        # Converting to Lower Case
         string1 = string1.lower()
         string2 = string2.lower()
 
-        # Check if Anagram
+        # Checking if Anagram
         if (lengthOfStrings(string1, string2) and sortStrings(string1, string2)):
             return True
         else:
             return False
     else:
         raise Exception("The 'string1' and 'string2' arguments must be a string.")
```

### Comparing `PyEng-1.0.1/PyEng/data/dictionary.json` & `PyEng-1.0.2/PyEng/data/dictionary.json`

 * *Files identical despite different names*

### Comparing `PyEng-1.0.1/PyEng.egg-info/PKG-INFO` & `PyEng-1.0.2/PyEng.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 Metadata-Version: 2.1
 Name: PyEng
-Version: 1.0.1
-Summary: PyEng is a general-purpose Python module that contains functions related to the English language.
+Version: 1.0.2
+Summary: PyEng is a general-purpose Python package that contains functions related to the English language.
 Home-page: https://github.com/Anikethc/PyEng
 Download-URL: https://pypi.org/project/PyEng
 Author: Aniketh Chavare
 Author-email: anikethchavare@outlook.com
 License: MIT
 Keywords: English
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # PyEng
 
 ## Introduction
 
-PyEng is a general-purpose Python module that contains functions related to the English language.
+PyEng is a general-purpose Python package that contains functions related to the English language.
 
 Read the docs on GitBook [here](https://aniketh-chavare.gitbook.io/pyeng-docs).
 
-## Module Information
+## Package Information
 
 **Name** - PyEng</br>
-**Version** - 1.0.1</br>
-**Description** - PyEng is a general-purpose Python module that contains functions related to the English language.</br>
+**Version** - 1.0.2</br>
+**Description** - PyEng is a general-purpose Python package that contains functions related to the English language.</br>
 **Author** - Aniketh Chavare</br>
 **GitHub URL** - [https://github.com/Anikethc/PyEng](https://github.com/Anikethc/PyEng)</br>
 **Pypi.org URL** - [https://pypi.org/project/PyEng](https://pypi.org/project/PyEng)</br>
 **Docs URL** - [https://aniketh-chavare.gitbook.io/pyeng-docs](https://aniketh-chavare.gitbook.io/pyeng-docs)
 
 ## License
 
@@ -55,8 +55,8 @@
 
 ## Issues & Bugs
 
 If you encounter any issues or bugs, visit the 'Issues' tab and create an issue. I'll look into it and resolve it ASAP.
 
 ## Conclusion
 
-I hope you liked this module. Thank you!
+I hope you liked this package. Thank you!
```

### Comparing `PyEng-1.0.1/README.md` & `PyEng-1.0.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 # PyEng
 
 ## Introduction
 
-PyEng is a general-purpose Python module that contains functions related to the English language.
+PyEng is a general-purpose Python package that contains functions related to the English language.
 
 Read the docs on GitBook [here](https://aniketh-chavare.gitbook.io/pyeng-docs).
 
-## Module Information
+## Package Information
 
 **Name** - PyEng</br>
-**Version** - 1.0.1</br>
-**Description** - PyEng is a general-purpose Python module that contains functions related to the English language.</br>
+**Version** - 1.0.2</br>
+**Description** - PyEng is a general-purpose Python package that contains functions related to the English language.</br>
 **Author** - Aniketh Chavare</br>
 **GitHub URL** - [https://github.com/Anikethc/PyEng](https://github.com/Anikethc/PyEng)</br>
 **Pypi.org URL** - [https://pypi.org/project/PyEng](https://pypi.org/project/PyEng)</br>
 **Docs URL** - [https://aniketh-chavare.gitbook.io/pyeng-docs](https://aniketh-chavare.gitbook.io/pyeng-docs)
 
 ## License
 
@@ -42,8 +42,8 @@
 
 ## Issues & Bugs
 
 If you encounter any issues or bugs, visit the 'Issues' tab and create an issue. I'll look into it and resolve it ASAP.
 
 ## Conclusion
 
-I hope you liked this module. Thank you!
+I hope you liked this package. Thank you!
```

### Comparing `PyEng-1.0.1/setup.py` & `PyEng-1.0.2/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,16 +8,16 @@
 # README.md
 with open("README.md") as readme_file:
     README = readme_file.read()
 
 # Setup Arguements
 setup_args = dict (
     name="PyEng",
-    version="1.0.1",
-    description="PyEng is a general-purpose Python module that contains functions related to the English language.",
+    version="1.0.2",
+    description="PyEng is a general-purpose Python package that contains functions related to the English language.",
     long_description_content_type="text/markdown",
     long_description=README,
     license="MIT",
     packages=find_packages(),
     include_package_data=True,
     author="Aniketh Chavare",
     author_email="anikethchavare@outlook.com",
```

