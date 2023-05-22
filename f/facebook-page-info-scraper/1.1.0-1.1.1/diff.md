# Comparing `tmp/facebook_page_info_scraper-1.1.0.tar.gz` & `tmp/facebook_page_info_scraper-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "facebook_page_info_scraper-1.1.0.tar", last modified: Fri May 19 15:23:34 2023, max compression
+gzip compressed data, was "facebook_page_info_scraper-1.1.1.tar", last modified: Mon May 22 16:53:07 2023, max compression
```

## Comparing `facebook_page_info_scraper-1.1.0.tar` & `facebook_page_info_scraper-1.1.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 15:23:34.683388 facebook_page_info_scraper-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-19 15:23:20.000000 facebook_page_info_scraper-1.1.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 15:23:20.000000 facebook_page_info_scraper-1.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2841 2023-05-19 15:23:34.683388 facebook_page_info_scraper-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-05-19 15:23:20.000000 facebook_page_info_scraper-1.1.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 15:23:34.683388 facebook_page_info_scraper-1.1.0/facebook_page_info_scraper/
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-19 15:23:20.000000 facebook_page_info_scraper-1.1.0/facebook_page_info_scraper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19870 2023-05-19 15:23:20.000000 facebook_page_info_scraper-1.1.0/facebook_page_info_scraper/facebook_page_info_scraper.py
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-19 15:23:20.000000 facebook_page_info_scraper-1.1.0/facebook_page_info_scraper/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 15:23:34.683388 facebook_page_info_scraper-1.1.0/facebook_page_info_scraper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2841 2023-05-19 15:23:34.000000 facebook_page_info_scraper-1.1.0/facebook_page_info_scraper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-05-19 15:23:34.000000 facebook_page_info_scraper-1.1.0/facebook_page_info_scraper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 15:23:34.000000 facebook_page_info_scraper-1.1.0/facebook_page_info_scraper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-19 15:23:34.000000 facebook_page_info_scraper-1.1.0/facebook_page_info_scraper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-19 15:23:34.000000 facebook_page_info_scraper-1.1.0/facebook_page_info_scraper.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-19 15:23:20.000000 facebook_page_info_scraper-1.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-05-19 15:23:34.683388 facebook_page_info_scraper-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-19 15:23:20.000000 facebook_page_info_scraper-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:53:07.141597 facebook_page_info_scraper-1.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-22 16:52:58.000000 facebook_page_info_scraper-1.1.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 16:52:58.000000 facebook_page_info_scraper-1.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4489 2023-05-22 16:53:07.141597 facebook_page_info_scraper-1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3628 2023-05-22 16:52:58.000000 facebook_page_info_scraper-1.1.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:53:07.137597 facebook_page_info_scraper-1.1.1/facebook_page_info_scraper/
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-22 16:52:58.000000 facebook_page_info_scraper-1.1.1/facebook_page_info_scraper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19879 2023-05-22 16:52:58.000000 facebook_page_info_scraper-1.1.1/facebook_page_info_scraper/facebook_page_info_scraper.py
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-22 16:52:58.000000 facebook_page_info_scraper-1.1.1/facebook_page_info_scraper/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:53:07.141597 facebook_page_info_scraper-1.1.1/facebook_page_info_scraper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4489 2023-05-22 16:53:07.000000 facebook_page_info_scraper-1.1.1/facebook_page_info_scraper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-05-22 16:53:07.000000 facebook_page_info_scraper-1.1.1/facebook_page_info_scraper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 16:53:07.000000 facebook_page_info_scraper-1.1.1/facebook_page_info_scraper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-22 16:53:07.000000 facebook_page_info_scraper-1.1.1/facebook_page_info_scraper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-22 16:53:07.000000 facebook_page_info_scraper-1.1.1/facebook_page_info_scraper.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-22 16:52:58.000000 facebook_page_info_scraper-1.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-05-22 16:53:07.141597 facebook_page_info_scraper-1.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-22 16:52:58.000000 facebook_page_info_scraper-1.1.1/setup.py
```

### Comparing `facebook_page_info_scraper-1.1.0/LICENSE.txt` & `facebook_page_info_scraper-1.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `facebook_page_info_scraper-1.1.0/facebook_page_info_scraper/facebook_page_info_scraper.py` & `facebook_page_info_scraper-1.1.1/facebook_page_info_scraper/facebook_page_info_scraper.py`

 * *Files 1% similar despite different names*

```diff
@@ -444,16 +444,16 @@
                 "page_name": page_name,
                 "page_category": category,
                 "email": email,
                 "page_website": urls,
                 "social_media_links": links,
                 'phone_number': phone,
                 'location': location,
-                'rate_': rate,
-                'review_number': review_number
+                'page_rate': rate,
+                'page_review_number': review_number
             }
             likes_follow_followers = self.__private_fetch_follower_likes_new_layout()
             data_collected.update(likes_follow_followers)
             return data_collected
         elif layout == 'x9orja2':
             page_name = self.__private_fetch_page_name()
             print('scraping:', page_name)
```

