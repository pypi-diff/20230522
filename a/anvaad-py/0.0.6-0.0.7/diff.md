# Comparing `tmp/anvaad_py-0.0.6.tar.gz` & `tmp/anvaad_py-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anvaad_py-0.0.6.tar", last modified: Sun May 21 14:34:42 2023, max compression
+gzip compressed data, was "anvaad_py-0.0.7.tar", last modified: Mon May 22 01:51:26 2023, max compression
```

## Comparing `anvaad_py-0.0.6.tar` & `anvaad_py-0.0.7.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-05-21 14:34:42.126228 anvaad_py-0.0.6/
--rw-rw-rw-   0        0        0     1103 2023-05-21 13:37:54.000000 anvaad_py-0.0.6/LICENSE
--rw-rw-rw-   0        0        0     4814 2023-05-21 14:34:42.123228 anvaad_py-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     4182 2023-05-21 14:31:33.000000 anvaad_py-0.0.6/README.md
--rw-rw-rw-   0        0        0      618 2023-05-21 14:34:25.000000 anvaad_py-0.0.6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-21 14:34:42.127233 anvaad_py-0.0.6/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-21 14:34:42.046445 anvaad_py-0.0.6/src/
-drwxrwxrwx   0        0        0        0 2023-05-21 14:34:42.096051 anvaad_py-0.0.6/src/anvaad_py/
--rw-rw-rw-   0        0        0      172 2023-05-21 14:33:37.000000 anvaad_py-0.0.6/src/anvaad_py/__init__.py
--rw-rw-rw-   0        0        0     2773 2023-05-21 14:25:30.000000 anvaad_py-0.0.6/src/anvaad_py/alphabetize.py
--rw-rw-rw-   0        0        0      328 2023-05-21 12:28:39.000000 anvaad_py-0.0.6/src/anvaad_py/ascii.py
--rw-rw-rw-   0        0        0     1372 2023-05-21 14:30:18.000000 anvaad_py-0.0.6/src/anvaad_py/firstLetters.py
--rw-rw-rw-   0        0        0     1090 2023-05-21 12:33:35.000000 anvaad_py-0.0.6/src/anvaad_py/mainLetters.py
--rw-rw-rw-   0        0        0    11156 2023-05-21 12:24:09.000000 anvaad_py-0.0.6/src/anvaad_py/unicode.py
-drwxrwxrwx   0        0        0        0 2023-05-21 14:34:42.119233 anvaad_py-0.0.6/src/anvaad_py.egg-info/
--rw-rw-rw-   0        0        0     4814 2023-05-21 14:34:42.000000 anvaad_py-0.0.6/src/anvaad_py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      342 2023-05-21 14:34:42.000000 anvaad_py-0.0.6/src/anvaad_py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-21 14:34:42.000000 anvaad_py-0.0.6/src/anvaad_py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-05-21 14:34:42.000000 anvaad_py-0.0.6/src/anvaad_py.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-22 01:51:26.916114 anvaad_py-0.0.7/
+-rw-rw-rw-   0        0        0     1103 2023-05-21 13:37:54.000000 anvaad_py-0.0.7/LICENSE
+-rw-rw-rw-   0        0        0     4990 2023-05-22 01:51:26.915103 anvaad_py-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     4358 2023-05-22 01:50:50.000000 anvaad_py-0.0.7/README.md
+-rw-rw-rw-   0        0        0      618 2023-05-22 01:51:03.000000 anvaad_py-0.0.7/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-22 01:51:26.917109 anvaad_py-0.0.7/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-22 01:51:26.880800 anvaad_py-0.0.7/src/
+drwxrwxrwx   0        0        0        0 2023-05-22 01:51:26.902343 anvaad_py-0.0.7/src/anvaad_py/
+-rw-rw-rw-   0        0        0      172 2023-05-21 14:33:37.000000 anvaad_py-0.0.7/src/anvaad_py/__init__.py
+-rw-rw-rw-   0        0        0     2773 2023-05-21 14:25:30.000000 anvaad_py-0.0.7/src/anvaad_py/alphabetize.py
+-rw-rw-rw-   0        0        0      328 2023-05-21 12:28:39.000000 anvaad_py-0.0.7/src/anvaad_py/ascii.py
+-rw-rw-rw-   0        0        0     1372 2023-05-21 14:30:18.000000 anvaad_py-0.0.7/src/anvaad_py/firstLetters.py
+-rw-rw-rw-   0        0        0     1090 2023-05-21 12:33:35.000000 anvaad_py-0.0.7/src/anvaad_py/mainLetters.py
+-rw-rw-rw-   0        0        0    11156 2023-05-21 12:24:09.000000 anvaad_py-0.0.7/src/anvaad_py/unicode.py
+drwxrwxrwx   0        0        0        0 2023-05-22 01:51:26.912081 anvaad_py-0.0.7/src/anvaad_py.egg-info/
+-rw-rw-rw-   0        0        0     4990 2023-05-22 01:51:26.000000 anvaad_py-0.0.7/src/anvaad_py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      342 2023-05-22 01:51:26.000000 anvaad_py-0.0.7/src/anvaad_py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-22 01:51:26.000000 anvaad_py-0.0.7/src/anvaad_py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-05-22 01:51:26.000000 anvaad_py-0.0.7/src/anvaad_py.egg-info/top_level.txt
```

### Comparing `anvaad_py-0.0.6/LICENSE` & `anvaad_py-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `anvaad_py-0.0.6/PKG-INFO` & `anvaad_py-0.0.7/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,34 +1,29 @@
-Metadata-Version: 2.1
-Name: anvaad_py
-Version: 0.0.6
-Summary: A Python utility to translit gurmukhi, and convert it between ascii to unicode with ease! (Python version of anvaad-js)
-Author-email: "0xharkirat (Harkirat Singh)" <info.sandhukirat23@gmail.com>
-Project-URL: Homepage, https://github.com/0xharkirat/anvaad-py
-Project-URL: Bug Tracker, https://github.com/0xharkirat/anvaad-py
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # anvaad-py :: ਅਨੁਵਾਦ-ਪੀਵਾਏ 
 
 This is python version of [anvaad-js](https://github.com/KhalisFoundation/anvaad-js) 
 
 ## Installation
 
 ```bash
 # pip
 pip install anvaad-py
 ```
 
 ## API Documentation
 
+## Usage
+
+```python
+import unicode from anvaad_py
+
+unicode('ਆਇ ਮਿਲੁ ਗੁਰਸਿਖ ਆਇ ਮਿਲੁ ਤੂ ਮੇਰੇ ਗੁਰੂ ਕੇ ਪਿਆਰੇ ॥', True)
+// => 'Awie imlu gurisK Awie imlu qU myry gurU ky ipAwry ]'
+```
+
 ### Table of Contents
 
 -   [ascii](#ascii)
 -   [firstLetters](#firstletters)
 -   [mainLetters](#mainletters)
 -   [translit](#translit)
 -   [unicode](#unicode)
@@ -36,89 +31,89 @@
 ## ascii
 
 Returns a comma-separated string of ascii codes for a
 string of Gurmukhi characters
 
 **Parameters**
 
--   `string` **[string](https://developer.mozilla.org/docs/Web/JavaScript/Reference/Global_Objects/String)** The string of letters
+-   `string` **[string](https://developer.mozilla.org/docs/Web/python/Reference/Global_Objects/String)** The string of letters
 
 **Examples**
 
-```javascript
-ascii('AmgAmqmgkp');
+```python
+ascii('AmgAmqmgkp')
 // => ',065,109,103,065,109,113,109,103,107,112,'
 ```
 
-Returns **[string](https://developer.mozilla.org/docs/Web/JavaScript/Reference/Global_Objects/String)** Returns a single string of comma-separated ascii codes
+Returns **[string](https://developer.mozilla.org/docs/Web/python/Reference/Global_Objects/String)** Returns a single string of comma-separated ascii codes
 
 
 ## firstLetters
 
 Retrieve the first letter of each word from a string
 
 **Parameters**
 
--   `words` **[string](https://developer.mozilla.org/docs/Web/JavaScript/Reference/Global_Objects/String)** The string from which to get first letters
--   `eng` **[boolean](https://developer.mozilla.org/docs/Web/JavaScript/Reference/Global_Objects/Boolean)** Whether the string is English (optional, default `false`)
--   `simplify` **[boolean](https://developer.mozilla.org/docs/Web/JavaScript/Reference/Global_Objects/Boolean)** Whether to simplify embedded vowels and other characters (eg. E to a, ^ to K)
+-   `words` **[string](https://developer.mozilla.org/docs/Web/python/Reference/Global_Objects/String)** The string from which to get first letters
+-   `eng` **[boolean](https://developer.mozilla.org/docs/Web/python/Reference/Global_Objects/Boolean)** Whether the string is English (optional, default `false`)
+-   `simplify` **[boolean](https://developer.mozilla.org/docs/Web/python/Reference/Global_Objects/Boolean)** Whether to simplify embedded vowels and other characters (eg. E to a, ^ to K)
 
 **Examples**
 
-```javascript
-firstLetters('Awie imlu gurisK Awie imlu qU myry gurU ky ipAwry ]');
+```python
+firstLetters('Awie imlu gurisK Awie imlu qU myry gurU ky ipAwry ]')
 // => 'AmgAmqmgkp'
 ```
 
-Returns **[string](https://developer.mozilla.org/docs/Web/JavaScript/Reference/Global_Objects/String)** Returns a single string of characters
+Returns **[string](https://developer.mozilla.org/docs/Web/python/Reference/Global_Objects/String)** Returns a single string of characters
 
 
 ## mainLetters
 
 Removes vowel symbols from a Gurmukhi string
 
 **Parameters**
 
--   `words` **[string](https://developer.mozilla.org/docs/Web/JavaScript/Reference/Global_Objects/String)** The string from which to get main letters
--   `simplify` **[boolean](https://developer.mozilla.org/docs/Web/JavaScript/Reference/Global_Objects/Boolean)** Whether to simplify embedded vowels/nasal sounds (eg. E to a, ^ to K)
--   `simplifyConsonants` **[boolean](https://developer.mozilla.org/docs/Web/JavaScript/Reference/Global_Objects/Boolean)** Whether to simplify half characters to full characters (eg. R to r)
+-   `words` **[string](https://developer.mozilla.org/docs/Web/python/Reference/Global_Objects/String)** The string from which to get main letters
+-   `simplify` **[boolean](https://developer.mozilla.org/docs/Web/python/Reference/Global_Objects/Boolean)** Whether to simplify embedded vowels/nasal sounds (eg. E to a, ^ to K)
+-   `simplifyConsonants` **[boolean](https://developer.mozilla.org/docs/Web/python/Reference/Global_Objects/Boolean)** Whether to simplify half characters to full characters (eg. R to r)
 
 **Examples**
 
-```javascript
-mainLetters('Awie imlu gurisK Awie imlu qU myry gurU ky ipAwry ]');
+```python
+mainLetters('Awie imlu gurisK Awie imlu qU myry gurU ky ipAwry ]')
 // => 'Ae ml grsK Ae ml q mr gr k pAr'
 ```
 
-Returns **[string](https://developer.mozilla.org/docs/Web/JavaScript/Reference/Global_Objects/String)** Returns a single string of characters
+Returns **[string](https://developer.mozilla.org/docs/Web/python/Reference/Global_Objects/String)** Returns a single string of characters
 
 
 
 ## unicode
 
 Convert Gurmukhi script to Unicode and back again.
 
 **Parameters**
 
--   `text` **[string](https://developer.mozilla.org/docs/Web/JavaScript/Reference/Global_Objects/String)** Gurbani Akhar or Unicode script to be converted
--   `reverse` **[boolean](https://developer.mozilla.org/docs/Web/JavaScript/Reference/Global_Objects/Boolean)** Whether to convert ASCII to unicode (false by default)
--   `simplify` **[boolean](https://developer.mozilla.org/docs/Web/JavaScript/Reference/Global_Objects/Boolean)** Whether to simplify extended characters to single code points (eg. sæ to ਸ਼ (u0A36), ਸ਼ (u0A38u0A3C) to S) (false by default)
+-   `text` **[string](https://developer.mozilla.org/docs/Web/python/Reference/Global_Objects/String)** Gurbani Akhar or Unicode script to be converted
+-   `reverse` **[boolean](https://developer.mozilla.org/docs/Web/python/Reference/Global_Objects/Boolean)** Whether to convert ASCII to unicode (false by default)
+-   `simplify` **[boolean](https://developer.mozilla.org/docs/Web/python/Reference/Global_Objects/Boolean)** Whether to simplify extended characters to single code points (eg. sæ to ਸ਼ (u0A36), ਸ਼ (u0A38u0A3C) to S) (false by default)
 
 
 **Examples**
 
-```javascript
-unicode('Awie imlu gurisK Awie imlu qU myry gurU ky ipAwry ]');
+```python
+unicode('Awie imlu gurisK Awie imlu qU myry gurU ky ipAwry ]')
 // => 'ਆਇ ਮਿਲੁ ਗੁਰਸਿਖ ਆਇ ਮਿਲੁ ਤੂ ਮੇਰੇ ਗੁਰੂ ਕੇ ਪਿਆਰੇ ॥'
 ```
 
-Returns **[string](https://developer.mozilla.org/docs/Web/JavaScript/Reference/Global_Objects/String)** Returns unicode text
+Returns **[string](https://developer.mozilla.org/docs/Web/python/Reference/Global_Objects/String)** Returns unicode text
 
-```javascript
- * unicode('ਆਇ ਮਿਲੁ ਗੁਰਸਿਖ ਆਇ ਮਿਲੁ ਤੂ ਮੇਰੇ ਗੁਰੂ ਕੇ ਪਿਆਰੇ ॥', true);
+```python
+ * unicode('ਆਇ ਮਿਲੁ ਗੁਰਸਿਖ ਆਇ ਮਿਲੁ ਤੂ ਮੇਰੇ ਗੁਰੂ ਕੇ ਪਿਆਰੇ ॥', True)
  * // => 'Awie imlu gurisK Awie imlu qU myry gurU ky ipAwry ]'
 ```
 
-Returns **[string](https://developer.mozilla.org/docs/Web/JavaScript/Reference/Global_Objects/String)** Returns gurbani akhar ascii text
+Returns **[string](https://developer.mozilla.org/docs/Web/python/Reference/Global_Objects/String)** Returns gurbani akhar ascii text
 
 
 a [0xharkirat](https://github.com/0xharkirat/) (Harkirat Singh) production.
```

### Comparing `anvaad_py-0.0.6/pyproject.toml` & `anvaad_py-0.0.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "anvaad_py"
-version = "0.0.6"
+version = "0.0.7"
 authors = [
   { name="0xharkirat (Harkirat Singh)", email="info.sandhukirat23@gmail.com" },
 ]
 description = "A Python utility to translit gurmukhi, and convert it between ascii to unicode with ease! (Python version of anvaad-js)"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `anvaad_py-0.0.6/src/anvaad_py/alphabetize.py` & `anvaad_py-0.0.7/src/anvaad_py/alphabetize.py`

 * *Files identical despite different names*

### Comparing `anvaad_py-0.0.6/src/anvaad_py/firstLetters.py` & `anvaad_py-0.0.7/src/anvaad_py/firstLetters.py`

 * *Files identical despite different names*

### Comparing `anvaad_py-0.0.6/src/anvaad_py/mainLetters.py` & `anvaad_py-0.0.7/src/anvaad_py/mainLetters.py`

 * *Files identical despite different names*

### Comparing `anvaad_py-0.0.6/src/anvaad_py/unicode.py` & `anvaad_py-0.0.7/src/anvaad_py/unicode.py`

 * *Files identical despite different names*

