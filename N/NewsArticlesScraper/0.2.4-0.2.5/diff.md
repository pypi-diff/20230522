# Comparing `tmp/NewsArticlesScraper-0.2.4.tar.gz` & `tmp/NewsArticlesScraper-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "NewsArticlesScraper-0.2.4.tar", last modified: Wed May 17 14:47:23 2023, max compression
+gzip compressed data, was "NewsArticlesScraper-0.2.5.tar", last modified: Mon May 22 21:45:56 2023, max compression
```

## Comparing `NewsArticlesScraper-0.2.4.tar` & `NewsArticlesScraper-0.2.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-17 14:47:23.141795 NewsArticlesScraper-0.2.4/
-drwxrwxrwx   0        0        0        0 2023-05-17 14:47:23.119791 NewsArticlesScraper-0.2.4/NewsArticlesScraper/
--rw-rw-rw-   0        0        0    14552 2023-05-17 14:41:40.000000 NewsArticlesScraper-0.2.4/NewsArticlesScraper/Scrapers.py
--rw-rw-rw-   0        0        0       64 2023-02-14 20:15:57.000000 NewsArticlesScraper-0.2.4/NewsArticlesScraper/__init__.py
--rw-rw-rw-   0        0        0     1074 2023-04-23 16:12:20.000000 NewsArticlesScraper-0.2.4/NewsArticlesScraper/test.py
-drwxrwxrwx   0        0        0        0 2023-05-17 14:47:23.139293 NewsArticlesScraper-0.2.4/NewsArticlesScraper.egg-info/
--rw-rw-rw-   0        0        0      648 2023-05-17 14:47:23.000000 NewsArticlesScraper-0.2.4/NewsArticlesScraper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      324 2023-05-17 14:47:23.000000 NewsArticlesScraper-0.2.4/NewsArticlesScraper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-17 14:47:23.000000 NewsArticlesScraper-0.2.4/NewsArticlesScraper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       40 2023-05-17 14:47:23.000000 NewsArticlesScraper-0.2.4/NewsArticlesScraper.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2023-05-17 14:47:23.000000 NewsArticlesScraper-0.2.4/NewsArticlesScraper.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      648 2023-05-17 14:47:23.140795 NewsArticlesScraper-0.2.4/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-02-14 20:04:13.000000 NewsArticlesScraper-0.2.4/README.md
--rw-rw-rw-   0        0        0       42 2023-05-17 14:47:23.141795 NewsArticlesScraper-0.2.4/setup.cfg
--rw-rw-rw-   0        0        0      996 2023-05-17 14:47:13.000000 NewsArticlesScraper-0.2.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-22 21:45:56.001160 NewsArticlesScraper-0.2.5/
+drwxrwxrwx   0        0        0        0 2023-05-22 21:45:55.980159 NewsArticlesScraper-0.2.5/NewsArticlesScraper/
+-rw-rw-rw-   0        0        0    14673 2023-05-22 21:42:30.000000 NewsArticlesScraper-0.2.5/NewsArticlesScraper/Scrapers.py
+-rw-rw-rw-   0        0        0       64 2023-02-14 20:15:57.000000 NewsArticlesScraper-0.2.5/NewsArticlesScraper/__init__.py
+-rw-rw-rw-   0        0        0     1074 2023-04-23 16:12:20.000000 NewsArticlesScraper-0.2.5/NewsArticlesScraper/test.py
+drwxrwxrwx   0        0        0        0 2023-05-22 21:45:55.999160 NewsArticlesScraper-0.2.5/NewsArticlesScraper.egg-info/
+-rw-rw-rw-   0        0        0      648 2023-05-22 21:45:55.000000 NewsArticlesScraper-0.2.5/NewsArticlesScraper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      324 2023-05-22 21:45:55.000000 NewsArticlesScraper-0.2.5/NewsArticlesScraper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-22 21:45:55.000000 NewsArticlesScraper-0.2.5/NewsArticlesScraper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       40 2023-05-22 21:45:55.000000 NewsArticlesScraper-0.2.5/NewsArticlesScraper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2023-05-22 21:45:55.000000 NewsArticlesScraper-0.2.5/NewsArticlesScraper.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      648 2023-05-22 21:45:56.000659 NewsArticlesScraper-0.2.5/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-02-14 20:04:13.000000 NewsArticlesScraper-0.2.5/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-22 21:45:56.001160 NewsArticlesScraper-0.2.5/setup.cfg
+-rw-rw-rw-   0        0        0      996 2023-05-22 21:45:42.000000 NewsArticlesScraper-0.2.5/setup.py
```

### Comparing `NewsArticlesScraper-0.2.4/NewsArticlesScraper/Scrapers.py` & `NewsArticlesScraper-0.2.5/NewsArticlesScraper/Scrapers.py`

 * *Files 2% similar despite different names*

```diff
@@ -189,15 +189,18 @@
         api_point = response.meta["api_point"]
         if api_point == "historic":
             articles = data["response"]["docs"]
         else:
             articles = data["results"]
         for article in articles:
             if api_point == "historic" and self.subsections_to_include is not None:
-                if article["subsection_name"] not in self.subsections_to_include:
+                subsection = article.get("subsection_name", None)
+                if subsection is None:
+                    continue
+                if subsection not in self.subsections_to_include:
                     continue
             if api_point == "recent" and self.subsections_to_include is not None:
                 if article["section"] not in self.subsections_to_include:
                     continue
             if api_point == "historic":
                 pub_date = article["pub_date"]
             else:
```

### Comparing `NewsArticlesScraper-0.2.4/NewsArticlesScraper/test.py` & `NewsArticlesScraper-0.2.5/NewsArticlesScraper/test.py`

 * *Files identical despite different names*

### Comparing `NewsArticlesScraper-0.2.4/NewsArticlesScraper.egg-info/PKG-INFO` & `NewsArticlesScraper-0.2.5/NewsArticlesScraper.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NewsArticlesScraper
-Version: 0.2.4
+Version: 0.2.5
 Summary: Scraping news articles
 Author: PySlayer (Paul Antweiler)
 Author-email: antweiler.paul@gmail.com
 Keywords: python,news,scraping,news scraping,news articles
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `NewsArticlesScraper-0.2.4/PKG-INFO` & `NewsArticlesScraper-0.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NewsArticlesScraper
-Version: 0.2.4
+Version: 0.2.5
 Summary: Scraping news articles
 Author: PySlayer (Paul Antweiler)
 Author-email: antweiler.paul@gmail.com
 Keywords: python,news,scraping,news scraping,news articles
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `NewsArticlesScraper-0.2.4/setup.py` & `NewsArticlesScraper-0.2.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.2.4'
+VERSION = '0.2.5'
 DESCRIPTION = 'Scraping news articles'
 LONG_DESCRIPTION = 'A package that allows you to scrape news articles from various news sites via scrapy.'
 
 # Setting up
 setup(
     name="NewsArticlesScraper",
     version=VERSION,
```

