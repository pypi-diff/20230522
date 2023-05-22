# Comparing `tmp/scrapinglib-0.5.2.tar.gz` & `tmp/scrapinglib-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/scrapinglib-0.5.2.tar", last modified: Wed Jan 11 02:16:59 2023, max compression
+gzip compressed data, was "dist/scrapinglib-0.6.0.tar", last modified: Mon May 22 02:56:36 2023, max compression
```

## Comparing `scrapinglib-0.5.2.tar` & `scrapinglib-0.6.0.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 02:16:59.000000 scrapinglib-0.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-01-11 02:16:50.000000 scrapinglib-0.5.2/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 02:16:59.000000 scrapinglib-0.5.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 02:16:59.000000 scrapinglib-0.5.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      758 2023-01-11 02:16:50.000000 scrapinglib-0.5.2/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-01-11 02:16:50.000000 scrapinglib-0.5.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      957 2023-01-11 02:16:59.000000 scrapinglib-0.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-01-11 02:16:50.000000 scrapinglib-0.5.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 02:16:59.000000 scrapinglib-0.5.2/scrapinglib/
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-01-11 02:16:50.000000 scrapinglib-0.5.2/scrapinglib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4896 2023-01-11 02:16:50.000000 scrapinglib-0.5.2/scrapinglib/airav.py
--rw-r--r--   0 runner    (1001) docker     (123)     8725 2023-01-11 02:16:50.000000 scrapinglib-0.5.2/scrapinglib/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     3772 2023-01-11 02:16:50.000000 scrapinglib-0.5.2/scrapinglib/avsox.py
--rw-r--r--   0 runner    (1001) docker     (123)     4201 2023-01-11 02:16:50.000000 scrapinglib-0.5.2/scrapinglib/carib.py
--rw-r--r--   0 runner    (1001) docker     (123)     5149 2023-01-11 02:16:50.000000 scrapinglib-0.5.2/scrapinglib/dlsite.py
--rw-r--r--   0 runner    (1001) docker     (123)     7434 2023-01-11 02:16:50.000000 scrapinglib-0.5.2/scrapinglib/fanza.py
--rw-r--r--   0 runner    (1001) docker     (123)     2426 2023-01-11 02:16:50.000000 scrapinglib-0.5.2/scrapinglib/fc2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-01-11 02:16:50.000000 scrapinglib-0.5.2/scrapinglib/gcolle.py
--rw-r--r--   0 runner    (1001) docker     (123)     6320 2023-01-11 02:16:50.000000 scrapinglib-0.5.2/scrapinglib/getchu.py
--rw-r--r--   0 runner    (1001) docker     (123)     7832 2023-01-11 02:16:50.000000 scrapinglib-0.5.2/scrapinglib/httprequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-01-11 02:16:50.000000 scrapinglib-0.5.2/scrapinglib/imdb.py
--rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-01-11 02:16:50.000000 scrapinglib-0.5.2/scrapinglib/jav321.py
--rw-r--r--   0 runner    (1001) docker     (123)     5337 2023-01-11 02:16:50.000000 scrapinglib-0.5.2/scrapinglib/javbus.py
--rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-01-11 02:16:50.000000 scrapinglib-0.5.2/scrapinglib/javday.py
--rw-r--r--   0 runner    (1001) docker     (123)    10680 2023-01-11 02:16:50.000000 scrapinglib-0.5.2/scrapinglib/javdb.py
--rw-r--r--   0 runner    (1001) docker     (123)     3700 2023-01-11 02:16:50.000000 scrapinglib-0.5.2/scrapinglib/javlibrary.py
--rw-r--r--   0 runner    (1001) docker     (123)     2441 2023-01-11 02:16:50.000000 scrapinglib-0.5.2/scrapinglib/madou.py
--rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-01-11 02:16:50.000000 scrapinglib-0.5.2/scrapinglib/mgstage.py
--rw-r--r--   0 runner    (1001) docker     (123)    10388 2023-01-11 02:16:50.000000 scrapinglib-0.5.2/scrapinglib/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)    10980 2023-01-11 02:16:50.000000 scrapinglib-0.5.2/scrapinglib/storyline.py
--rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-01-11 02:16:50.000000 scrapinglib-0.5.2/scrapinglib/tmdb.py
--rw-r--r--   0 runner    (1001) docker     (123)      712 2023-01-11 02:16:50.000000 scrapinglib-0.5.2/scrapinglib/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3771 2023-01-11 02:16:50.000000 scrapinglib-0.5.2/scrapinglib/xcity.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 02:16:59.000000 scrapinglib-0.5.2/scrapinglib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      957 2023-01-11 02:16:58.000000 scrapinglib-0.5.2/scrapinglib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-01-11 02:16:58.000000 scrapinglib-0.5.2/scrapinglib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-11 02:16:58.000000 scrapinglib-0.5.2/scrapinglib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-01-11 02:16:58.000000 scrapinglib-0.5.2/scrapinglib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-01-11 02:16:58.000000 scrapinglib-0.5.2/scrapinglib.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-11 02:16:59.000000 scrapinglib-0.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-01-11 02:16:50.000000 scrapinglib-0.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 02:16:59.000000 scrapinglib-0.5.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     9449 2023-01-11 02:16:50.000000 scrapinglib-0.5.2/tests/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 02:56:36.000000 scrapinglib-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-22 02:56:24.000000 scrapinglib-0.6.0/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 02:56:36.000000 scrapinglib-0.6.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 02:56:36.000000 scrapinglib-0.6.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-05-22 02:56:24.000000 scrapinglib-0.6.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-05-22 02:56:24.000000 scrapinglib-0.6.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-05-22 02:56:36.000000 scrapinglib-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-05-22 02:56:24.000000 scrapinglib-0.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 02:56:36.000000 scrapinglib-0.6.0/scrapinglib/
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-05-22 02:56:24.000000 scrapinglib-0.6.0/scrapinglib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4896 2023-05-22 02:56:24.000000 scrapinglib-0.6.0/scrapinglib/airav.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7940 2023-05-22 02:56:24.000000 scrapinglib-0.6.0/scrapinglib/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3973 2023-05-22 02:56:24.000000 scrapinglib-0.6.0/scrapinglib/avsox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4201 2023-05-22 02:56:24.000000 scrapinglib-0.6.0/scrapinglib/carib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5149 2023-05-22 02:56:24.000000 scrapinglib-0.6.0/scrapinglib/dlsite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7434 2023-05-22 02:56:24.000000 scrapinglib-0.6.0/scrapinglib/fanza.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2466 2023-05-22 02:56:24.000000 scrapinglib-0.6.0/scrapinglib/fc2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-05-22 02:56:24.000000 scrapinglib-0.6.0/scrapinglib/gcolle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6320 2023-05-22 02:56:24.000000 scrapinglib-0.6.0/scrapinglib/getchu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7832 2023-05-22 02:56:24.000000 scrapinglib-0.6.0/scrapinglib/httprequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-05-22 02:56:24.000000 scrapinglib-0.6.0/scrapinglib/imdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-05-22 02:56:24.000000 scrapinglib-0.6.0/scrapinglib/jav321.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5337 2023-05-22 02:56:24.000000 scrapinglib-0.6.0/scrapinglib/javbus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-05-22 02:56:24.000000 scrapinglib-0.6.0/scrapinglib/javday.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10679 2023-05-22 02:56:24.000000 scrapinglib-0.6.0/scrapinglib/javdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3700 2023-05-22 02:56:24.000000 scrapinglib-0.6.0/scrapinglib/javlibrary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3120 2023-05-22 02:56:24.000000 scrapinglib-0.6.0/scrapinglib/madou.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2216 2023-05-22 02:56:24.000000 scrapinglib-0.6.0/scrapinglib/mgstage.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10533 2023-05-22 02:56:24.000000 scrapinglib-0.6.0/scrapinglib/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10980 2023-05-22 02:56:24.000000 scrapinglib-0.6.0/scrapinglib/storyline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-05-22 02:56:24.000000 scrapinglib-0.6.0/scrapinglib/tmdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-05-22 02:56:24.000000 scrapinglib-0.6.0/scrapinglib/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3771 2023-05-22 02:56:24.000000 scrapinglib-0.6.0/scrapinglib/xcity.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 02:56:36.000000 scrapinglib-0.6.0/scrapinglib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-05-22 02:56:36.000000 scrapinglib-0.6.0/scrapinglib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-05-22 02:56:36.000000 scrapinglib-0.6.0/scrapinglib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 02:56:36.000000 scrapinglib-0.6.0/scrapinglib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-22 02:56:36.000000 scrapinglib-0.6.0/scrapinglib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-22 02:56:36.000000 scrapinglib-0.6.0/scrapinglib.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 02:56:36.000000 scrapinglib-0.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-05-22 02:56:24.000000 scrapinglib-0.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 02:56:36.000000 scrapinglib-0.6.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     9449 2023-05-22 02:56:24.000000 scrapinglib-0.6.0/tests/test.py
```

### Comparing `scrapinglib-0.5.2/.github/workflows/release.yml` & `scrapinglib-0.6.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `scrapinglib-0.5.2/.gitignore` & `scrapinglib-0.6.0/.gitignore`

 * *Files identical despite different names*

### Comparing `scrapinglib-0.5.2/PKG-INFO` & `scrapinglib-0.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrapinglib
-Version: 0.5.2
+Version: 0.6.0
 Summary: UNKNOWN
 Home-page: https://github.com/Suwmlee/scrapinglib
 Author: suwmlee
 Author-email: suwmlee@gmail.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/Suwmlee/scrapinglib/issues
 Project-URL: Source, https://github.com/Suwmlee/scrapinglib
```

### Comparing `scrapinglib-0.5.2/scrapinglib/airav.py` & `scrapinglib-0.6.0/scrapinglib/airav.py`

 * *Files identical despite different names*

### Comparing `scrapinglib-0.5.2/scrapinglib/avsox.py` & `scrapinglib-0.6.0/scrapinglib/avsox.py`

 * *Files 8% similar despite different names*

```diff
@@ -27,20 +27,22 @@
         if 'FC2' in upnum and 'FC2-PPV' not in upnum:
             number = upnum.replace('FC2', 'FC2-PPV')
             self.number = number
         qurySiteTree = self.getHtmlTree('https://tellme.pw/avsox')
         site = self.getTreeElement(qurySiteTree, '//div[@class="container"]/div/a/@href')
         self.searchtree = self.getHtmlTree(site + '/cn/search/' + number)
         result1 = self.getTreeElement(self.searchtree, '//*[@id="waterfall"]/div/a/@href')
-        if result1 == '' or result1 == 'null' or result1 == 'None':
+        if result1 == '' or result1 == 'null' or result1 == 'None' or result1.find('movie') == -1:
             self.searchtree = self.getHtmlTree(site + '/cn/search/' + number.replace('-', '_'))
             result1 = self.getTreeElement(self.searchtree, '//*[@id="waterfall"]/div/a/@href')
-            if result1 == '' or result1 == 'null' or result1 == 'None':
+            if result1 == '' or result1 == 'null' or result1 == 'None' or result1.find('movie') == -1:
                 self.searchtree = self.getHtmlTree(site + '/cn/search/' + number.replace('_', ''))
                 result1 = self.getTreeElement(self.searchtree, '//*[@id="waterfall"]/div/a/@href')
+                if result1 == '' or result1 == 'null' or result1 == 'None' or result1.find('movie') == -1:
+                    return None
         return "https:" + result1
 
     def getNum(self, htmltree):
         new_number = self.getTreeElement(htmltree, self.expr_number)
         if new_number.upper() != self.number.upper():
             raise ValueError('number not found in ' + self.source)
         self.originalnum = new_number
```

### Comparing `scrapinglib-0.5.2/scrapinglib/carib.py` & `scrapinglib-0.6.0/scrapinglib/carib.py`

 * *Files identical despite different names*

### Comparing `scrapinglib-0.5.2/scrapinglib/dlsite.py` & `scrapinglib-0.6.0/scrapinglib/dlsite.py`

 * *Files identical despite different names*

### Comparing `scrapinglib-0.5.2/scrapinglib/fanza.py` & `scrapinglib-0.6.0/scrapinglib/fanza.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,23 +45,21 @@
             "https://www.dmm.co.jp/rental/-/detail/=/cid=",
         ]
 
         for url in fanza_urls:
             self.detailurl = url + fanza_search_number
             url = "https://www.dmm.co.jp/age_check/=/declared=yes/?"+ urlencode({"rurl": self.detailurl})
             self.htmlcode = self.getHtml(url)
-            if "Sorry! This content is not available in your region." in self.htmlcode:
-                continue
-            if self.htmlcode != 404:
+            if self.htmlcode != 404 \
+                    and 'Sorry! This content is not available in your region.' not in self.htmlcode:
                 self.htmltree = etree.HTML(self.htmlcode)
-                break
-        if self.htmlcode == 404:
-            return 404
-        result = self.dictformat(self.htmltree)
-        return result
+                if self.htmltree is not None:
+                    result = self.dictformat(self.htmltree)
+                    return result
+        return 404
 
     def getNum(self, htmltree):
         # for some old page, the input number does not match the page
         # for example, the url will be cid=test012
         # but the hinban on the page is test00012
         # so get the hinban first, and then pass it to following functions
         self.fanza_hinban = self.getFanzaString('品番：')
```

### Comparing `scrapinglib-0.5.2/scrapinglib/fc2.py` & `scrapinglib-0.6.0/scrapinglib/fc2.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,14 +18,15 @@
     expr_actor = '//*[@id="top"]/div[1]/section[1]/div/section/div[2]/ul/li[3]/a/text()'
     expr_cover = "//div[@class='items_article_MainitemThumb']/span/img/@src"
     expr_extrafanart = '//ul[@class="items_article_SampleImagesArea"]/li/a/@href'
     expr_tags = "//a[@class='tag tagTag']/text()"
 
     def extraInit(self):
         self.imagecut = 0
+        self.allow_number_change = True
 
     def search(self, number):
         self.number = number.lower().replace('fc2-ppv-', '').replace('fc2-', '')
         if self.specifiedUrl:
             self.detailurl = self.specifiedUrl
         else:
             self.detailurl = 'https://adult.contents.fc2.com/article/' + self.number + '/'
```

### Comparing `scrapinglib-0.5.2/scrapinglib/gcolle.py` & `scrapinglib-0.6.0/scrapinglib/gcolle.py`

 * *Files identical despite different names*

### Comparing `scrapinglib-0.5.2/scrapinglib/getchu.py` & `scrapinglib-0.6.0/scrapinglib/getchu.py`

 * *Files identical despite different names*

### Comparing `scrapinglib-0.5.2/scrapinglib/httprequest.py` & `scrapinglib-0.6.0/scrapinglib/httprequest.py`

 * *Files identical despite different names*

### Comparing `scrapinglib-0.5.2/scrapinglib/imdb.py` & `scrapinglib-0.6.0/scrapinglib/imdb.py`

 * *Files identical despite different names*

### Comparing `scrapinglib-0.5.2/scrapinglib/jav321.py` & `scrapinglib-0.6.0/scrapinglib/jav321.py`

 * *Files identical despite different names*

### Comparing `scrapinglib-0.5.2/scrapinglib/javbus.py` & `scrapinglib-0.6.0/scrapinglib/javbus.py`

 * *Files 0% similar despite different names*

```diff
@@ -124,15 +124,15 @@
         if self.uncensored:
             return self.getTreeElement(htmltree, self.expr_series2)
         else:
             return self.getTreeElement(htmltree, self.expr_series)
 
     def getTags(self, htmltree):
         tags = self.getTreeElement(htmltree, self.expr_tags).split(',')
-        return tags[1:]
+        return tags[2:]
 
     def getOutline(self, htmltree):
         if self.morestoryline:
             if any(caller for caller in inspect.stack() if os.path.basename(caller.filename) == 'airav.py'):
                 return ''   # 从airav.py过来的调用不计算outline直接返回，避免重复抓取数据拖慢处理速度
             from .storyline import getStoryline
             return getStoryline(self.number , uncensored = self.uncensored,
```

### Comparing `scrapinglib-0.5.2/scrapinglib/javday.py` & `scrapinglib-0.6.0/scrapinglib/javday.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 # -*- coding: utf-8 -*-
 
-import re
 from lxml import etree
-from urllib.parse import urlparse, unquote
 from .parser import Parser
 
 
 class Javday(Parser):
     source = 'javday'
 
     expr_url = '/html/head/meta[@property="og:url"]/@content'
@@ -37,7 +35,12 @@
         return result
 
     def getTitle(self, htmltree):
         title = super().getTitle(htmltree)
         # 删除番号和网站名
         result = title.replace(self.number,"").replace("- JAVDAY.TV","").strip()
         return result
+    
+    def getTags(self, htmltree) -> list:
+        tags = super().getTags(htmltree)
+        return [tag for tag in tags if 'JAVDAY.TV' not in tag]
+
```

### Comparing `scrapinglib-0.5.2/scrapinglib/javdb.py` & `scrapinglib-0.6.0/scrapinglib/javdb.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 # -*- coding: utf-8 -*-
 
-
 import re
 from urllib.parse import urljoin
 from lxml import etree
 from .httprequest import request_session
 from .parser import Parser
```

### Comparing `scrapinglib-0.5.2/scrapinglib/javlibrary.py` & `scrapinglib-0.6.0/scrapinglib/javlibrary.py`

 * *Files identical despite different names*

### Comparing `scrapinglib-0.5.2/scrapinglib/madou.py` & `scrapinglib-0.6.0/scrapinglib/madou.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,28 +2,53 @@
 
 import re
 from lxml import etree
 from urllib.parse import urlparse, unquote
 from .parser import Parser
 
 
+NUM_RULES3=[
+    r'(mmz{2,4})-?(\d{2,})(-ep\d*|-\d*)?.*',
+    r'(msd)-?(\d{2,})(-ep\d*|-\d*)?.*',
+    r'(yk)-?(\d{2,})(-ep\d*|-\d*)?.*',
+    r'(pm)-?(\d{2,})(-ep\d*|-\d*)?.*',
+    r'(mky-[a-z]{2,2})-?(\d{2,})(-ep\d*|-\d*)?.*',
+]
+
+# modou提取number
+def change_number(number):
+    number = number.lower().strip()
+    m = re.search(r'(md[a-z]{0,2})-?(\d{2,})(-ep\d*|-\d*)?.*', number, re.I)
+    if m:
+        return f'{m.group(1)}{m.group(2).zfill(4)}{m.group(3) or ""}'
+    for rules in NUM_RULES3:
+        m = re.search(rules, number, re.I)
+        if m:
+            return f'{m.group(1)}{m.group(2).zfill(3)}{m.group(3) or ""}'
+    return number
+
+
+
 class Madou(Parser):
     source = 'madou'
 
     expr_url = '//a[@class="share-weixin"]/@data-url'
     expr_title = "/html/head/title/text()"
     expr_studio = '//a[@rel="category tag"]/text()'
     expr_tags = '/html/head/meta[@name="keywords"]/@content'
 
+
+
     def extraInit(self):
-        self.imagecut = 0
+        self.imagecut = 4
         self.uncensored = True
+        self.allow_number_change = True
 
     def search(self, number):
-        self.number = number.lower().strip()
+        self.number = change_number(number)
         if self.specifiedUrl:
             self.detailurl = self.specifiedUrl
         else:
             self.detailurl = "https://madou.club/" + number + ".html"
         self.htmlcode = self.getHtml(self.detailurl)
         if self.htmlcode == 404:
             return 404
@@ -61,9 +86,9 @@
             url = str(re.findall("shareimage      : '(.*?)'", self.htmlcode)[0])
             return url.strip()
         except:
             return ''
 
     def getTags(self, htmltree):
         studio = self.getStudio(htmltree)
-        x = super().getTags(htmltree)
-        return [i.strip() for i in x if len(i.strip()) and studio not in i and '麻豆' not in i]
+        tags = super().getTags(htmltree)
+        return [tag for tag in tags if studio not in tag and '麻豆' not in tag]
```

### Comparing `scrapinglib-0.5.2/scrapinglib/mgstage.py` & `scrapinglib-0.6.0/scrapinglib/mgstage.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,22 +17,25 @@
     expr_cover = '//*[@id="EnlargeImage"]/@href'
     expr_label = '//th[contains(text(),"レーベル：")]/../td/a/text()'
     expr_tags = '//th[contains(text(),"ジャンル：")]/../td/a/text()'
     expr_tags2 = '//th[contains(text(),"ジャンル：")]/../td/text()'
     expr_series = '//th[contains(text(),"シリーズ")]/../td/a/text()'
     expr_extrafanart = '//a[@class="sample_image"]/@href'
 
+    def extraInit(self):
+        self.imagecut = 4
+
     def search(self, number):
         self.number = number.upper()
-        self.cookies = {'adc':'1'}
+        self.cookies = {'adc': '1'}
         if self.specifiedUrl:
             self.detailurl = self.specifiedUrl
         else:
-            self.detailurl = 'https://www.mgstage.com/product/product_detail/'+str(self.number)+'/'
-        htmltree =self.getHtmlTree(self.detailurl)
+            self.detailurl = 'https://www.mgstage.com/product/product_detail/' + str(self.number) + '/'
+        htmltree = self.getHtmlTree(self.detailurl)
         result = self.dictformat(htmltree)
         return result
 
     def getTitle(self, htmltree):
         return super().getTitle(htmltree).replace('/', ',').strip()
 
     def getTags(self, htmltree):
```

### Comparing `scrapinglib-0.5.2/scrapinglib/parser.py` & `scrapinglib-0.6.0/scrapinglib/parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,15 +81,15 @@
         """
         self.number = number
         if self.specifiedUrl:
             self.detailurl = self.specifiedUrl
         else:
             self.detailurl = self.queryNumberUrl(number)
         if not self.detailurl:
-            return None
+            return 404
         htmltree = self.getHtmlTree(self.detailurl)
         result = self.dictformat(htmltree)
         return result
 
     def updateCore(self, core):
         """ 从`core`内更新参数
         
@@ -206,15 +206,21 @@
         return self.getTreeElement(htmltree, self.expr_director).strip()
 
     def getActors(self, htmltree) -> list:
         return self.getTreeAll(htmltree, self.expr_actor)
 
     def getTags(self, htmltree) -> list:
         alls = self.getTreeAll(htmltree, self.expr_tags)
-        return [ x.strip() for x in alls if x.strip()]
+        tags = []
+        for t in alls:
+            for tag in t.strip().split(','):
+                tag = tag.strip()
+                if tag:
+                    tags.append(tag)
+        return tags
 
     def getStudio(self, htmltree):
         return self.getTreeElementbyExprs(htmltree, self.expr_studio, self.expr_studio2)
 
     def getLabel(self, htmltree):
         return self.getTreeElementbyExprs(htmltree, self.expr_label, self.expr_label2)
```

### Comparing `scrapinglib-0.5.2/scrapinglib/storyline.py` & `scrapinglib-0.6.0/scrapinglib/storyline.py`

 * *Files identical despite different names*

### Comparing `scrapinglib-0.5.2/scrapinglib/tmdb.py` & `scrapinglib-0.6.0/scrapinglib/tmdb.py`

 * *Files identical despite different names*

### Comparing `scrapinglib-0.5.2/scrapinglib/utils.py` & `scrapinglib-0.6.0/scrapinglib/utils.py`

 * *Files identical despite different names*

### Comparing `scrapinglib-0.5.2/scrapinglib/xcity.py` & `scrapinglib-0.6.0/scrapinglib/xcity.py`

 * *Files identical despite different names*

### Comparing `scrapinglib-0.5.2/scrapinglib.egg-info/PKG-INFO` & `scrapinglib-0.6.0/scrapinglib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrapinglib
-Version: 0.5.2
+Version: 0.6.0
 Summary: UNKNOWN
 Home-page: https://github.com/Suwmlee/scrapinglib
 Author: suwmlee
 Author-email: suwmlee@gmail.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/Suwmlee/scrapinglib/issues
 Project-URL: Source, https://github.com/Suwmlee/scrapinglib
```

### Comparing `scrapinglib-0.5.2/scrapinglib.egg-info/SOURCES.txt` & `scrapinglib-0.6.0/scrapinglib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `scrapinglib-0.5.2/setup.py` & `scrapinglib-0.6.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 ]
 
 with open("README.md", "r", "utf-8") as f:
     readme = f.read()
 
 setup(
     name='scrapinglib',
-    version='0.5.2',
+    version='0.6.0',
     author="suwmlee",
     author_email='suwmlee@gmail.com',
     url='https://github.com/Suwmlee/scrapinglib',
     long_description=readme,
     long_description_content_type="text/markdown",
     packages=["scrapinglib"],
     package_dir={'scrapinglib': 'scrapinglib'},
```

### Comparing `scrapinglib-0.5.2/tests/test.py` & `scrapinglib-0.6.0/tests/test.py`

 * *Files identical despite different names*

