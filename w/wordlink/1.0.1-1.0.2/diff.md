# Comparing `tmp/wordlink-1.0.1.tar.gz` & `tmp/wordlink-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wordlink-1.0.1.tar", last modified: Mon May 22 07:07:27 2023, max compression
+gzip compressed data, was "wordlink-1.0.2.tar", last modified: Mon May 22 09:43:53 2023, max compression
```

## Comparing `wordlink-1.0.1.tar` & `wordlink-1.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 bloom      (501) staff       (20)        0 2023-05-22 07:07:27.516742 wordlink-1.0.1/
--rw-r--r--   0 bloom      (501) staff       (20)     4037 2023-05-22 07:07:27.517830 wordlink-1.0.1/PKG-INFO
--rw-r--r--   0 bloom      (501) staff       (20)     3535 2023-05-22 06:42:47.000000 wordlink-1.0.1/readme.md
--rw-r--r--   0 bloom      (501) staff       (20)      746 2023-05-22 07:07:27.518069 wordlink-1.0.1/setup.cfg
--rw-r--r--   0 bloom      (501) staff       (20)      713 2023-05-22 07:07:06.000000 wordlink-1.0.1/setup.py
-drwxr-xr-x   0 bloom      (501) staff       (20)        0 2023-05-22 07:07:27.515945 wordlink-1.0.1/wordlink/
--rw-r--r--   0 bloom      (501) staff       (20)        0 2023-05-22 06:48:08.000000 wordlink-1.0.1/wordlink/__init__.py
--rw-r--r--   0 bloom      (501) staff       (20)     3582 2023-05-22 06:48:12.000000 wordlink-1.0.1/wordlink/__main__.py
-drwxr-xr-x   0 bloom      (501) staff       (20)        0 2023-05-22 07:07:27.516660 wordlink-1.0.1/wordlink.egg-info/
--rw-r--r--   0 bloom      (501) staff       (20)     4037 2023-05-22 07:07:27.000000 wordlink-1.0.1/wordlink.egg-info/PKG-INFO
--rw-r--r--   0 bloom      (501) staff       (20)      264 2023-05-22 07:07:27.000000 wordlink-1.0.1/wordlink.egg-info/SOURCES.txt
--rw-r--r--   0 bloom      (501) staff       (20)        1 2023-05-22 07:07:27.000000 wordlink-1.0.1/wordlink.egg-info/dependency_links.txt
--rw-r--r--   0 bloom      (501) staff       (20)       43 2023-05-22 07:07:27.000000 wordlink-1.0.1/wordlink.egg-info/entry_points.txt
--rw-r--r--   0 bloom      (501) staff       (20)       24 2023-05-22 07:07:27.000000 wordlink-1.0.1/wordlink.egg-info/requires.txt
--rw-r--r--   0 bloom      (501) staff       (20)        9 2023-05-22 07:07:27.000000 wordlink-1.0.1/wordlink.egg-info/top_level.txt
+drwxr-xr-x   0 bloom      (501) staff       (20)        0 2023-05-22 09:43:53.195434 wordlink-1.0.2/
+-rw-r--r--   0 bloom      (501) staff       (20)     4117 2023-05-22 09:43:53.195495 wordlink-1.0.2/PKG-INFO
+-rw-r--r--   0 bloom      (501) staff       (20)     3615 2023-05-22 09:42:47.000000 wordlink-1.0.2/readme.md
+-rw-r--r--   0 bloom      (501) staff       (20)      746 2023-05-22 09:43:53.195739 wordlink-1.0.2/setup.cfg
+-rw-r--r--   0 bloom      (501) staff       (20)      713 2023-05-22 09:43:35.000000 wordlink-1.0.2/setup.py
+drwxr-xr-x   0 bloom      (501) staff       (20)        0 2023-05-22 09:43:53.194620 wordlink-1.0.2/wordlink/
+-rw-r--r--   0 bloom      (501) staff       (20)        0 2023-05-22 09:42:47.000000 wordlink-1.0.2/wordlink/__init__.py
+-rw-r--r--   0 bloom      (501) staff       (20)     3582 2023-05-22 09:42:47.000000 wordlink-1.0.2/wordlink/__main__.py
+drwxr-xr-x   0 bloom      (501) staff       (20)        0 2023-05-22 09:43:53.195350 wordlink-1.0.2/wordlink.egg-info/
+-rw-r--r--   0 bloom      (501) staff       (20)     4117 2023-05-22 09:43:53.000000 wordlink-1.0.2/wordlink.egg-info/PKG-INFO
+-rw-r--r--   0 bloom      (501) staff       (20)      264 2023-05-22 09:43:53.000000 wordlink-1.0.2/wordlink.egg-info/SOURCES.txt
+-rw-r--r--   0 bloom      (501) staff       (20)        1 2023-05-22 09:43:53.000000 wordlink-1.0.2/wordlink.egg-info/dependency_links.txt
+-rw-r--r--   0 bloom      (501) staff       (20)       43 2023-05-22 09:43:53.000000 wordlink-1.0.2/wordlink.egg-info/entry_points.txt
+-rw-r--r--   0 bloom      (501) staff       (20)       24 2023-05-22 09:43:53.000000 wordlink-1.0.2/wordlink.egg-info/requires.txt
+-rw-r--r--   0 bloom      (501) staff       (20)        9 2023-05-22 09:43:53.000000 wordlink-1.0.2/wordlink.egg-info/top_level.txt
```

### Comparing `wordlink-1.0.1/PKG-INFO` & `wordlink-1.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 Metadata-Version: 2.1
 Name: wordlink
-Version: 1.0.1
+Version: 1.0.2
 Summary: Word Link Generator
 Home-page: https://github.com/psibir/wordlink
 Download-URL: https://github.com/psibir/wordlink/archive/v_01.tar.gz
 Author: Trevor Bloomfield
 Author-email: bloomfieldtm@gmail.com
 Keywords: word,link,html,console
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 # wordlink
 
+![wordlink logo](/wordlink_logo.png)
+
 A Word Link Generator that searches for a given term in multiple text files within a specified directory and generates links to the matched occurrences. It provides two output options: an HTML file with clickable links or a console display using a formatted table.
 The `__main__.py` file is located in the `/wordlink/` directory.
 
 ## Prerequisites
 
 - Python 3.x
 - `argparse` library
@@ -35,15 +37,15 @@
    ```
 
 ## Usage
 
 Run the script using the following command:
 
 ```bash
-python main.py <search_term> <search_directory> [-o OUTPUT_FILE]
+python3 wordlink <search_term> <search_directory> [-o OUTPUT_FILE]
 ```
 
 - `<search_term>`: The term to search for within the text files.
 - `<search_directory>`: The directory to search for text files.
 - `-o OUTPUT_FILE` or `--output_file OUTPUT_FILE`: (Optional) Specify the output file name to save the results as an HTML file. If not provided, the results will be displayed in the console using a formatted table.
 
 **Examples:**
@@ -74,15 +76,15 @@
 
 The tool includes a test suite to ensure its functionality. The `main_test.py` file contains the unit tests. Here's a description of what each test case in `main_test.py` is testing:
 
 - `test_find_word_locations`: This test verifies that the `find_word_locations` method correctly identifies the locations of the given search term within a test file.
 - `test_generate_links_output_file`: This test checks if the `generate_links` method generates the expected output file in HTML format when an output file name is provided.
 - `test_generate_links_console`: This test validates that the `generate_links` method produces the expected console output when no output file name is provided.
 
-To run the tests, execute the following command:
+To run the tests, navigate to the `/tests/` directpry and execute the following command:
 
 ```bash
 python3 main_test.py
 ```
 
 ## Limitations
```

### Comparing `wordlink-1.0.1/readme.md` & `wordlink-1.0.2/readme.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 # wordlink
 
+![wordlink logo](/wordlink_logo.png)
+
 A Word Link Generator that searches for a given term in multiple text files within a specified directory and generates links to the matched occurrences. It provides two output options: an HTML file with clickable links or a console display using a formatted table.
 The `__main__.py` file is located in the `/wordlink/` directory.
 
 ## Prerequisites
 
 - Python 3.x
 - `argparse` library
@@ -20,15 +22,15 @@
    ```
 
 ## Usage
 
 Run the script using the following command:
 
 ```bash
-python main.py <search_term> <search_directory> [-o OUTPUT_FILE]
+python3 wordlink <search_term> <search_directory> [-o OUTPUT_FILE]
 ```
 
 - `<search_term>`: The term to search for within the text files.
 - `<search_directory>`: The directory to search for text files.
 - `-o OUTPUT_FILE` or `--output_file OUTPUT_FILE`: (Optional) Specify the output file name to save the results as an HTML file. If not provided, the results will be displayed in the console using a formatted table.
 
 **Examples:**
@@ -59,15 +61,15 @@
 
 The tool includes a test suite to ensure its functionality. The `main_test.py` file contains the unit tests. Here's a description of what each test case in `main_test.py` is testing:
 
 - `test_find_word_locations`: This test verifies that the `find_word_locations` method correctly identifies the locations of the given search term within a test file.
 - `test_generate_links_output_file`: This test checks if the `generate_links` method generates the expected output file in HTML format when an output file name is provided.
 - `test_generate_links_console`: This test validates that the `generate_links` method produces the expected console output when no output file name is provided.
 
-To run the tests, execute the following command:
+To run the tests, navigate to the `/tests/` directpry and execute the following command:
 
 ```bash
 python3 main_test.py
 ```
 
 ## Limitations
```

### Comparing `wordlink-1.0.1/setup.cfg` & `wordlink-1.0.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `wordlink-1.0.1/setup.py` & `wordlink-1.0.2/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='wordlink',
-    version='1.0.1',
+    version='1.0.2',
     author='Trevor Bloomfield',
     author_email='bloomfieldtm@gmail.com',
     description='Word Link Generator',
     py_modules=['wordlink'],
     url = 'https://github.com/psibir/wordlink',   # Provide either the link to your github or to your website
     download_url = 'https://github.com/psibir/wordlink/archive/v_01.tar.gz',    # I explain this later on
     keywords = ['word', 'link', 'html', 'console'],   # Keywords that define your package best
```

### Comparing `wordlink-1.0.1/wordlink/__main__.py` & `wordlink-1.0.2/wordlink/__main__.py`

 * *Files identical despite different names*

### Comparing `wordlink-1.0.1/wordlink.egg-info/PKG-INFO` & `wordlink-1.0.2/wordlink.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 Metadata-Version: 2.1
 Name: wordlink
-Version: 1.0.1
+Version: 1.0.2
 Summary: Word Link Generator
 Home-page: https://github.com/psibir/wordlink
 Download-URL: https://github.com/psibir/wordlink/archive/v_01.tar.gz
 Author: Trevor Bloomfield
 Author-email: bloomfieldtm@gmail.com
 Keywords: word,link,html,console
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 # wordlink
 
+![wordlink logo](/wordlink_logo.png)
+
 A Word Link Generator that searches for a given term in multiple text files within a specified directory and generates links to the matched occurrences. It provides two output options: an HTML file with clickable links or a console display using a formatted table.
 The `__main__.py` file is located in the `/wordlink/` directory.
 
 ## Prerequisites
 
 - Python 3.x
 - `argparse` library
@@ -35,15 +37,15 @@
    ```
 
 ## Usage
 
 Run the script using the following command:
 
 ```bash
-python main.py <search_term> <search_directory> [-o OUTPUT_FILE]
+python3 wordlink <search_term> <search_directory> [-o OUTPUT_FILE]
 ```
 
 - `<search_term>`: The term to search for within the text files.
 - `<search_directory>`: The directory to search for text files.
 - `-o OUTPUT_FILE` or `--output_file OUTPUT_FILE`: (Optional) Specify the output file name to save the results as an HTML file. If not provided, the results will be displayed in the console using a formatted table.
 
 **Examples:**
@@ -74,15 +76,15 @@
 
 The tool includes a test suite to ensure its functionality. The `main_test.py` file contains the unit tests. Here's a description of what each test case in `main_test.py` is testing:
 
 - `test_find_word_locations`: This test verifies that the `find_word_locations` method correctly identifies the locations of the given search term within a test file.
 - `test_generate_links_output_file`: This test checks if the `generate_links` method generates the expected output file in HTML format when an output file name is provided.
 - `test_generate_links_console`: This test validates that the `generate_links` method produces the expected console output when no output file name is provided.
 
-To run the tests, execute the following command:
+To run the tests, navigate to the `/tests/` directpry and execute the following command:
 
 ```bash
 python3 main_test.py
 ```
 
 ## Limitations
```

