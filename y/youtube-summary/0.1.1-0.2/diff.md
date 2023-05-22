# Comparing `tmp/youtube-summary-0.1.1.tar.gz` & `tmp/youtube-summary-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "youtube-summary-0.1.1.tar", last modified: Mon May 22 10:09:55 2023, max compression
+gzip compressed data, was "youtube-summary-0.2.tar", last modified: Mon May 22 13:22:51 2023, max compression
```

## Comparing `youtube-summary-0.1.1.tar` & `youtube-summary-0.2.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxr-xr-x   0 maorcohen   (501) staff       (20)        0 2023-05-22 10:09:55.494491 youtube-summary-0.1.1/
--rw-r--r--   0 maorcohen   (501) staff       (20)     1067 2023-05-21 10:58:12.000000 youtube-summary-0.1.1/LICENSE
--rw-r--r--   0 maorcohen   (501) staff       (20)     1560 2023-05-22 10:09:55.494303 youtube-summary-0.1.1/PKG-INFO
--rw-r--r--   0 maorcohen   (501) staff       (20)       38 2023-05-22 10:09:55.494536 youtube-summary-0.1.1/setup.cfg
--rw-r--r--   0 maorcohen   (501) staff       (20)      563 2023-05-22 10:09:08.000000 youtube-summary-0.1.1/setup.py
-drwxr-xr-x   0 maorcohen   (501) staff       (20)        0 2023-05-22 10:09:55.492836 youtube-summary-0.1.1/youtube_summary/
--rw-r--r--   0 maorcohen   (501) staff       (20)        0 2023-05-21 18:58:41.000000 youtube-summary-0.1.1/youtube_summary/__init__.py
--rw-r--r--   0 maorcohen   (501) staff       (20)     2316 2023-05-21 17:04:12.000000 youtube-summary-0.1.1/youtube_summary/main.py
-drwxr-xr-x   0 maorcohen   (501) staff       (20)        0 2023-05-22 10:09:55.494025 youtube-summary-0.1.1/youtube_summary.egg-info/
--rw-r--r--   0 maorcohen   (501) staff       (20)     1560 2023-05-22 10:09:55.000000 youtube-summary-0.1.1/youtube_summary.egg-info/PKG-INFO
--rw-r--r--   0 maorcohen   (501) staff       (20)      304 2023-05-22 10:09:55.000000 youtube-summary-0.1.1/youtube_summary.egg-info/SOURCES.txt
--rw-r--r--   0 maorcohen   (501) staff       (20)        1 2023-05-22 10:09:55.000000 youtube-summary-0.1.1/youtube_summary.egg-info/dependency_links.txt
--rw-r--r--   0 maorcohen   (501) staff       (20)       61 2023-05-22 10:09:55.000000 youtube-summary-0.1.1/youtube_summary.egg-info/entry_points.txt
--rw-r--r--   0 maorcohen   (501) staff       (20)      644 2023-05-22 10:09:55.000000 youtube-summary-0.1.1/youtube_summary.egg-info/requires.txt
--rw-r--r--   0 maorcohen   (501) staff       (20)       16 2023-05-22 10:09:55.000000 youtube-summary-0.1.1/youtube_summary.egg-info/top_level.txt
+drwxr-xr-x   0 maorcohen   (501) staff       (20)        0 2023-05-22 13:22:51.724343 youtube-summary-0.2/
+-rw-r--r--   0 maorcohen   (501) staff       (20)     1067 2023-05-21 10:58:12.000000 youtube-summary-0.2/LICENSE
+-rw-r--r--   0 maorcohen   (501) staff       (20)     1558 2023-05-22 13:22:51.724147 youtube-summary-0.2/PKG-INFO
+-rw-r--r--   0 maorcohen   (501) staff       (20)       38 2023-05-22 13:22:51.724403 youtube-summary-0.2/setup.cfg
+-rw-r--r--   0 maorcohen   (501) staff       (20)      561 2023-05-22 13:21:55.000000 youtube-summary-0.2/setup.py
+drwxr-xr-x   0 maorcohen   (501) staff       (20)        0 2023-05-22 13:22:51.722886 youtube-summary-0.2/youtube_summary/
+-rw-r--r--   0 maorcohen   (501) staff       (20)        0 2023-05-21 18:58:41.000000 youtube-summary-0.2/youtube_summary/__init__.py
+-rw-r--r--   0 maorcohen   (501) staff       (20)       29 2023-05-22 10:23:51.000000 youtube-summary-0.2/youtube_summary/__main__.py
+-rw-r--r--   0 maorcohen   (501) staff       (20)     6117 2023-05-22 13:20:54.000000 youtube-summary-0.2/youtube_summary/main.py
+drwxr-xr-x   0 maorcohen   (501) staff       (20)        0 2023-05-22 13:22:51.723851 youtube-summary-0.2/youtube_summary.egg-info/
+-rw-r--r--   0 maorcohen   (501) staff       (20)     1558 2023-05-22 13:22:51.000000 youtube-summary-0.2/youtube_summary.egg-info/PKG-INFO
+-rw-r--r--   0 maorcohen   (501) staff       (20)      332 2023-05-22 13:22:51.000000 youtube-summary-0.2/youtube_summary.egg-info/SOURCES.txt
+-rw-r--r--   0 maorcohen   (501) staff       (20)        1 2023-05-22 13:22:51.000000 youtube-summary-0.2/youtube_summary.egg-info/dependency_links.txt
+-rw-r--r--   0 maorcohen   (501) staff       (20)       61 2023-05-22 13:22:51.000000 youtube-summary-0.2/youtube_summary.egg-info/entry_points.txt
+-rw-r--r--   0 maorcohen   (501) staff       (20)      962 2023-05-22 13:22:51.000000 youtube-summary-0.2/youtube_summary.egg-info/requires.txt
+-rw-r--r--   0 maorcohen   (501) staff       (20)       16 2023-05-22 13:22:51.000000 youtube-summary-0.2/youtube_summary.egg-info/top_level.txt
```

### Comparing `youtube-summary-0.1.1/LICENSE` & `youtube-summary-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `youtube-summary-0.1.1/PKG-INFO` & `youtube-summary-0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: youtube-summary
-Version: 0.1.1
+Version: 0.2
 Home-page: https://github.com/mmaorc/youtube-summary-cli
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # YouTube Transcript Summarizer
 
 This project extracts and summarizes transcripts from YouTube videos using OpenAI GPT-3.5-turbo language model. I made it since I couldn't find any simple CLI app for this.
```

### Comparing `youtube-summary-0.1.1/setup.py` & `youtube-summary-0.2/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="youtube-summary",
-    version="0.1.1",
+    version="0.2",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=find_packages(),
     url="https://github.com/mmaorc/youtube-summary-cli",
     install_requires=[line.strip() for line in open("requirements.txt")],
     entry_points={
         "console_scripts": [
```

### Comparing `youtube-summary-0.1.1/youtube_summary.egg-info/PKG-INFO` & `youtube-summary-0.2/youtube_summary.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: youtube-summary
-Version: 0.1.1
+Version: 0.2
 Home-page: https://github.com/mmaorc/youtube-summary-cli
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # YouTube Transcript Summarizer
 
 This project extracts and summarizes transcripts from YouTube videos using OpenAI GPT-3.5-turbo language model. I made it since I couldn't find any simple CLI app for this.
```

