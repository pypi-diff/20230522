# Comparing `tmp/tidalapi-0.7.0rc1.tar.gz` & `tmp/tidalapi-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tidalapi-0.7.0rc1.tar", last modified: Thu Jun 30 06:17:24 2022, max compression
+gzip compressed data, was "tidalapi-0.7.1.tar", last modified: Mon May 22 20:27:54 2023, max compression
```

## Comparing `tidalapi-0.7.0rc1.tar` & `tidalapi-0.7.1.tar`

### file list

```diff
@@ -1,58 +1,50 @@
-drwxr-xr-x   0 kristian  (1000) wheel       (10)        0 2022-06-30 06:17:24.086375 tidalapi-0.7.0rc1/
--rw-r--r--   0 kristian  (1000) wheel       (10)      627 2022-06-28 04:50:03.000000 tidalapi-0.7.0rc1/.gitignore
--rw-r--r--   0 kristian  (1000) wheel       (10)     3364 2020-06-14 01:40:08.000000 tidalapi-0.7.0rc1/CODE_OF_CONDUCT.md
--rw-r--r--   0 kristian  (1000) wheel       (10)      877 2020-08-02 01:09:43.000000 tidalapi-0.7.0rc1/HISTORY.rst
--rw-r--r--   0 kristian  (1000) wheel       (10)     7651 2020-06-14 01:40:08.000000 tidalapi-0.7.0rc1/LICENSE
--rw-r--r--   0 kristian  (1000) wheel       (10)      199 2020-06-14 01:40:08.000000 tidalapi-0.7.0rc1/MANIFEST.in
--rw-r--r--   0 kristian  (1000) wheel       (10)     2803 2022-06-30 06:17:24.086375 tidalapi-0.7.0rc1/PKG-INFO
--rw-r--r--   0 kristian  (1000) wheel       (10)     1067 2022-06-30 04:35:05.000000 tidalapi-0.7.0rc1/README.rst
-drwxr-xr-x   0 kristian  (1000) wheel       (10)        0 2022-06-30 06:17:24.083042 tidalapi-0.7.0rc1/docs/
-drwxr-xr-x   0 kristian  (1000) wheel       (10)        0 2022-06-30 06:17:24.083042 tidalapi-0.7.0rc1/docs/_static/
--rw-r--r--   0 kristian  (1000) wheel       (10)       53 2020-08-02 00:41:34.000000 tidalapi-0.7.0rc1/docs/_static/style.css
-drwxr-xr-x   0 kristian  (1000) wheel       (10)        0 2022-06-30 06:17:24.083042 tidalapi-0.7.0rc1/docs/_templates/
--rw-r--r--   0 kristian  (1000) wheel       (10)      142 2020-08-02 00:41:34.000000 tidalapi-0.7.0rc1/docs/_templates/footer.html
--rw-r--r--   0 kristian  (1000) wheel       (10)      215 2020-08-02 00:54:24.000000 tidalapi-0.7.0rc1/docs/_templates/layout.html
--rw-r--r--   0 kristian  (1000) wheel       (10)     2450 2022-06-28 04:50:03.000000 tidalapi-0.7.0rc1/docs/api.rst
--rw-r--r--   0 kristian  (1000) wheel       (10)     2379 2022-06-30 04:33:32.000000 tidalapi-0.7.0rc1/docs/conf.py
--rw-r--r--   0 kristian  (1000) wheel       (10)       12 2020-08-02 00:41:34.000000 tidalapi-0.7.0rc1/docs/genindex.rst
--rw-r--r--   0 kristian  (1000) wheel       (10)       27 2020-08-02 00:41:34.000000 tidalapi-0.7.0rc1/docs/history.rst
--rw-r--r--   0 kristian  (1000) wheel       (10)      214 2022-06-28 04:50:03.000000 tidalapi-0.7.0rc1/docs/index.rst
--rw-r--r--   0 kristian  (1000) wheel       (10)     2441 2022-06-28 04:50:03.000000 tidalapi-0.7.0rc1/docs/pages.rst
--rw-r--r--   0 kristian  (1000) wheel       (10)       26 2020-08-02 00:41:34.000000 tidalapi-0.7.0rc1/docs/py-modindex.rst
--rw-r--r--   0 kristian  (1000) wheel       (10)       61 2022-06-28 04:50:03.000000 tidalapi-0.7.0rc1/docs/requirements.txt
--rw-r--r--   0 kristian  (1000) wheel       (10)        4 2020-08-02 02:05:51.000000 tidalapi-0.7.0rc1/docs/runtime.txt
--rw-r--r--   0 kristian  (1000) wheel       (10)       69 2022-06-30 03:32:25.000000 tidalapi-0.7.0rc1/netlify.toml
--rw-r--r--   0 kristian  (1000) wheel       (10)    18470 2020-08-02 21:43:19.000000 tidalapi-0.7.0rc1/pylintrc
--rw-r--r--   0 kristian  (1000) wheel       (10)      155 2022-06-30 06:17:24.086375 tidalapi-0.7.0rc1/setup.cfg
--rw-r--r--   0 kristian  (1000) wheel       (10)     1462 2022-06-30 06:08:38.000000 tidalapi-0.7.0rc1/setup.py
-drwxr-xr-x   0 kristian  (1000) wheel       (10)        0 2022-06-30 06:17:24.083042 tidalapi-0.7.0rc1/tests/
--rw-r--r--   0 kristian  (1000) wheel       (10)        0 2020-08-02 00:41:34.000000 tidalapi-0.7.0rc1/tests/__init__.py
--rw-r--r--   0 kristian  (1000) wheel       (10)     3306 2022-06-30 04:26:00.000000 tidalapi-0.7.0rc1/tests/conftest.py
--rw-r--r--   0 kristian  (1000) wheel       (10)     2880 2022-06-30 04:25:51.000000 tidalapi-0.7.0rc1/tests/cover.py
--rw-r--r--   0 kristian  (1000) wheel       (10)     3372 2022-06-30 04:25:19.000000 tidalapi-0.7.0rc1/tests/test_album.py
--rw-r--r--   0 kristian  (1000) wheel       (10)     4356 2022-06-30 04:26:55.000000 tidalapi-0.7.0rc1/tests/test_artist.py
--rw-r--r--   0 kristian  (1000) wheel       (10)     1839 2022-06-30 04:27:49.000000 tidalapi-0.7.0rc1/tests/test_genres.py
--rw-r--r--   0 kristian  (1000) wheel       (10)     5749 2022-06-30 04:25:27.000000 tidalapi-0.7.0rc1/tests/test_media.py
--rw-r--r--   0 kristian  (1000) wheel       (10)     3838 2022-06-30 03:32:25.000000 tidalapi-0.7.0rc1/tests/test_page.py
--rw-r--r--   0 kristian  (1000) wheel       (10)     4982 2022-06-30 04:26:55.000000 tidalapi-0.7.0rc1/tests/test_playlist.py
--rw-r--r--   0 kristian  (1000) wheel       (10)     4249 2022-06-30 04:26:55.000000 tidalapi-0.7.0rc1/tests/test_session.py
--rw-r--r--   0 kristian  (1000) wheel       (10)     6716 2022-06-30 04:24:13.000000 tidalapi-0.7.0rc1/tests/test_user.py
-drwxr-xr-x   0 kristian  (1000) wheel       (10)        0 2022-06-30 06:17:24.083042 tidalapi-0.7.0rc1/tidalapi/
--rw-r--r--   0 kristian  (1000) wheel       (10)      467 2022-06-30 04:34:08.000000 tidalapi-0.7.0rc1/tidalapi/__init__.py
--rw-r--r--   0 kristian  (1000) wheel       (10)     7089 2022-06-30 04:21:04.000000 tidalapi-0.7.0rc1/tidalapi/album.py
--rw-r--r--   0 kristian  (1000) wheel       (10)     6600 2022-06-30 04:21:04.000000 tidalapi-0.7.0rc1/tidalapi/artist.py
--rw-r--r--   0 kristian  (1000) wheel       (10)     2405 2022-06-30 04:27:49.000000 tidalapi-0.7.0rc1/tidalapi/genre.py
--rw-r--r--   0 kristian  (1000) wheel       (10)     8164 2022-06-30 04:19:48.000000 tidalapi-0.7.0rc1/tidalapi/media.py
--rw-r--r--   0 kristian  (1000) wheel       (10)     3472 2022-06-30 03:32:25.000000 tidalapi-0.7.0rc1/tidalapi/mix.py
--rw-r--r--   0 kristian  (1000) wheel       (10)    11356 2022-06-30 03:32:25.000000 tidalapi-0.7.0rc1/tidalapi/page.py
--rw-r--r--   0 kristian  (1000) wheel       (10)     8163 2022-06-30 04:26:17.000000 tidalapi-0.7.0rc1/tidalapi/playlist.py
--rw-r--r--   0 kristian  (1000) wheel       (10)     5986 2022-06-30 04:19:48.000000 tidalapi-0.7.0rc1/tidalapi/request.py
--rw-r--r--   0 kristian  (1000) wheel       (10)    25108 2022-06-30 04:19:26.000000 tidalapi-0.7.0rc1/tidalapi/session.py
--rw-r--r--   0 kristian  (1000) wheel       (10)    11412 2022-06-30 04:31:40.000000 tidalapi-0.7.0rc1/tidalapi/user.py
-drwxr-xr-x   0 kristian  (1000) wheel       (10)        0 2022-06-30 06:17:24.086375 tidalapi-0.7.0rc1/tidalapi.egg-info/
--rw-r--r--   0 kristian  (1000) wheel       (10)     2803 2022-06-30 06:17:23.000000 tidalapi-0.7.0rc1/tidalapi.egg-info/PKG-INFO
--rw-r--r--   0 kristian  (1000) wheel       (10)      931 2022-06-30 06:17:24.000000 tidalapi-0.7.0rc1/tidalapi.egg-info/SOURCES.txt
--rw-r--r--   0 kristian  (1000) wheel       (10)        1 2022-06-30 06:17:23.000000 tidalapi-0.7.0rc1/tidalapi.egg-info/dependency_links.txt
--rw-r--r--   0 kristian  (1000) wheel       (10)       25 2022-06-30 06:17:23.000000 tidalapi-0.7.0rc1/tidalapi.egg-info/requires.txt
--rw-r--r--   0 kristian  (1000) wheel       (10)        9 2022-06-30 06:17:23.000000 tidalapi-0.7.0rc1/tidalapi.egg-info/top_level.txt
--rw-r--r--   0 kristian  (1000) wheel       (10)      375 2022-06-30 04:32:45.000000 tidalapi-0.7.0rc1/tox.ini
+drwxrwxr-x   0 jlinde    (1000) jlinde    (1000)        0 2023-05-22 20:27:54.796436 tidalapi-0.7.1/
+-rw-rw-r--   0 jlinde    (1000) jlinde    (1000)     3554 2023-05-22 20:27:42.000000 tidalapi-0.7.1/HISTORY.rst
+-rw-rw-r--   0 jlinde    (1000) jlinde    (1000)     7651 2023-05-21 21:11:51.000000 tidalapi-0.7.1/LICENSE
+-rw-rw-r--   0 jlinde    (1000) jlinde    (1000)      199 2023-05-21 21:11:51.000000 tidalapi-0.7.1/MANIFEST.in
+-rw-rw-r--   0 jlinde    (1000) jlinde    (1000)     5548 2023-05-22 20:27:54.796436 tidalapi-0.7.1/PKG-INFO
+-rw-rw-r--   0 jlinde    (1000) jlinde    (1000)     1158 2023-05-22 20:09:13.000000 tidalapi-0.7.1/README.rst
+drwxrwxr-x   0 jlinde    (1000) jlinde    (1000)        0 2023-05-22 20:27:54.792436 tidalapi-0.7.1/docs/
+-rw-rw-r--   0 jlinde    (1000) jlinde    (1000)     2450 2023-05-21 21:11:51.000000 tidalapi-0.7.1/docs/api.rst
+-rw-rw-r--   0 jlinde    (1000) jlinde    (1000)     2464 2023-05-21 21:11:51.000000 tidalapi-0.7.1/docs/conf.py
+-rw-rw-r--   0 jlinde    (1000) jlinde    (1000)      387 2023-05-21 21:11:51.000000 tidalapi-0.7.1/docs/config.rst
+-rw-rw-r--   0 jlinde    (1000) jlinde    (1000)       12 2023-05-21 21:11:51.000000 tidalapi-0.7.1/docs/genindex.rst
+-rw-rw-r--   0 jlinde    (1000) jlinde    (1000)       27 2023-05-21 21:11:51.000000 tidalapi-0.7.1/docs/history.rst
+-rw-rw-r--   0 jlinde    (1000) jlinde    (1000)      262 2023-05-21 21:11:51.000000 tidalapi-0.7.1/docs/index.rst
+-rw-rw-r--   0 jlinde    (1000) jlinde    (1000)     2201 2023-05-21 21:11:51.000000 tidalapi-0.7.1/docs/login.rst
+-rw-rw-r--   0 jlinde    (1000) jlinde    (1000)      890 2023-05-21 21:11:51.000000 tidalapi-0.7.1/docs/migration.rst
+-rw-rw-r--   0 jlinde    (1000) jlinde    (1000)     2537 2023-05-21 21:11:51.000000 tidalapi-0.7.1/docs/pages.rst
+-rw-rw-r--   0 jlinde    (1000) jlinde    (1000)     1035 2023-05-21 21:11:51.000000 tidalapi-0.7.1/docs/playlist.rst
+-rw-rw-r--   0 jlinde    (1000) jlinde    (1000)       26 2023-05-21 21:11:51.000000 tidalapi-0.7.1/docs/py-modindex.rst
+-rw-rw-r--   0 jlinde    (1000) jlinde    (1000)      155 2023-05-22 20:27:54.796436 tidalapi-0.7.1/setup.cfg
+-rw-rw-r--   0 jlinde    (1000) jlinde    (1000)     1458 2023-05-22 19:50:46.000000 tidalapi-0.7.1/setup.py
+drwxrwxr-x   0 jlinde    (1000) jlinde    (1000)        0 2023-05-22 20:27:54.796436 tidalapi-0.7.1/tests/
+-rw-rw-r--   0 jlinde    (1000) jlinde    (1000)        0 2023-05-21 21:11:51.000000 tidalapi-0.7.1/tests/__init__.py
+-rw-rw-r--   0 jlinde    (1000) jlinde    (1000)     3306 2023-05-21 21:11:51.000000 tidalapi-0.7.1/tests/conftest.py
+-rw-rw-r--   0 jlinde    (1000) jlinde    (1000)     2880 2023-05-21 21:11:51.000000 tidalapi-0.7.1/tests/cover.py
+-rw-rw-r--   0 jlinde    (1000) jlinde    (1000)     3499 2023-05-21 21:11:51.000000 tidalapi-0.7.1/tests/test_album.py
+-rw-rw-r--   0 jlinde    (1000) jlinde    (1000)     4356 2023-05-21 21:11:51.000000 tidalapi-0.7.1/tests/test_artist.py
+-rw-rw-r--   0 jlinde    (1000) jlinde    (1000)     1839 2023-05-21 21:11:51.000000 tidalapi-0.7.1/tests/test_genres.py
+-rw-rw-r--   0 jlinde    (1000) jlinde    (1000)     5749 2023-05-21 21:11:51.000000 tidalapi-0.7.1/tests/test_media.py
+-rw-rw-r--   0 jlinde    (1000) jlinde    (1000)     3843 2023-05-21 21:11:51.000000 tidalapi-0.7.1/tests/test_page.py
+-rw-rw-r--   0 jlinde    (1000) jlinde    (1000)     4982 2023-05-21 21:11:51.000000 tidalapi-0.7.1/tests/test_playlist.py
+-rw-rw-r--   0 jlinde    (1000) jlinde    (1000)     4249 2023-05-21 21:11:51.000000 tidalapi-0.7.1/tests/test_session.py
+-rw-rw-r--   0 jlinde    (1000) jlinde    (1000)     6716 2023-05-21 21:11:51.000000 tidalapi-0.7.1/tests/test_user.py
+drwxrwxr-x   0 jlinde    (1000) jlinde    (1000)        0 2023-05-22 20:27:54.796436 tidalapi-0.7.1/tidalapi/
+-rw-rw-r--   0 jlinde    (1000) jlinde    (1000)      464 2023-05-22 20:08:43.000000 tidalapi-0.7.1/tidalapi/__init__.py
+-rw-rw-r--   0 jlinde    (1000) jlinde    (1000)     7470 2023-05-21 21:11:51.000000 tidalapi-0.7.1/tidalapi/album.py
+-rw-rw-r--   0 jlinde    (1000) jlinde    (1000)     6600 2023-05-21 21:11:51.000000 tidalapi-0.7.1/tidalapi/artist.py
+-rw-rw-r--   0 jlinde    (1000) jlinde    (1000)     2405 2023-05-21 21:11:51.000000 tidalapi-0.7.1/tidalapi/genre.py
+-rw-rw-r--   0 jlinde    (1000) jlinde    (1000)     8535 2023-05-22 20:09:13.000000 tidalapi-0.7.1/tidalapi/media.py
+-rw-rw-r--   0 jlinde    (1000) jlinde    (1000)     3472 2023-05-21 21:11:51.000000 tidalapi-0.7.1/tidalapi/mix.py
+-rw-rw-r--   0 jlinde    (1000) jlinde    (1000)    11356 2023-05-21 21:11:51.000000 tidalapi-0.7.1/tidalapi/page.py
+-rw-rw-r--   0 jlinde    (1000) jlinde    (1000)     8474 2023-05-22 20:09:13.000000 tidalapi-0.7.1/tidalapi/playlist.py
+-rw-rw-r--   0 jlinde    (1000) jlinde    (1000)     5986 2023-05-21 21:11:51.000000 tidalapi-0.7.1/tidalapi/request.py
+-rw-rw-r--   0 jlinde    (1000) jlinde    (1000)    25114 2023-05-22 20:09:13.000000 tidalapi-0.7.1/tidalapi/session.py
+-rw-rw-r--   0 jlinde    (1000) jlinde    (1000)    11906 2023-05-22 19:46:49.000000 tidalapi-0.7.1/tidalapi/user.py
+drwxrwxr-x   0 jlinde    (1000) jlinde    (1000)        0 2023-05-22 20:27:54.796436 tidalapi-0.7.1/tidalapi.egg-info/
+-rw-rw-r--   0 jlinde    (1000) jlinde    (1000)     5548 2023-05-22 20:27:54.000000 tidalapi-0.7.1/tidalapi.egg-info/PKG-INFO
+-rw-rw-r--   0 jlinde    (1000) jlinde    (1000)      821 2023-05-22 20:27:54.000000 tidalapi-0.7.1/tidalapi.egg-info/SOURCES.txt
+-rw-rw-r--   0 jlinde    (1000) jlinde    (1000)        1 2023-05-22 20:27:54.000000 tidalapi-0.7.1/tidalapi.egg-info/dependency_links.txt
+-rw-rw-r--   0 jlinde    (1000) jlinde    (1000)       25 2023-05-22 20:27:54.000000 tidalapi-0.7.1/tidalapi.egg-info/requires.txt
+-rw-rw-r--   0 jlinde    (1000) jlinde    (1000)        9 2023-05-22 20:27:54.000000 tidalapi-0.7.1/tidalapi.egg-info/top_level.txt
```

### Comparing `tidalapi-0.7.0rc1/LICENSE` & `tidalapi-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tidalapi-0.7.0rc1/docs/api.rst` & `tidalapi-0.7.1/docs/api.rst`

 * *Files identical despite different names*

### Comparing `tidalapi-0.7.0rc1/docs/conf.py` & `tidalapi-0.7.1/docs/conf.py`

 * *Files 10% similar despite different names*

```diff
@@ -18,30 +18,31 @@
 # -- Project information -----------------------------------------------------
 
 project = 'tidalapi'
 copyright = '2014-2022, Thomas Amland, morguldir'
 author = 'Thomas Amland, morguldir'
 
 # The full version, including alpha/beta/rc tags
-release = '0.7.0rc1'
+release = '0.7.0'
 
 
 # -- General configuration ---------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom ones.
 extensions = [
     'sphinx.ext.autodoc',
     'sphinx.ext.viewcode',
     'sphinx.ext.intersphinx',
     'sphinx.ext.autosectionlabel',
     'sphinx.ext.doctest'
 ]
 
-intersphinx_mapping = {'python': ('https://docs.python.org/3', None)}
+intersphinx_mapping = {'python': ('https://docs.python.org/3', None),
+                       'requests': ('https://requests.readthedocs.io/en/latest', None)}
 
 autodoc_member_order = 'bysource'
 
 # Add any paths that contain templates here, relative to this directory.
 templates_path = ['_templates']
 
 # The master toctree document.
```

### Comparing `tidalapi-0.7.0rc1/docs/pages.rst` & `tidalapi-0.7.1/docs/pages.rst`

 * *Files 7% similar despite different names*

```diff
@@ -27,43 +27,45 @@
     home.categories.extend(session.videos().categories)
 
     for category in home.categories:
         print(category.title)
 
     for category in home.categories:
         print(category.title)
+        items = []
         for item in category.items:
             if isinstance(item, PageItem):
-                print("\t" + item.short_header)
-                print("\t" + item.short_sub_header[0:50])
+                items.append("\t" + item.short_header)
+                items.append("\t" + item.short_sub_header[0:50])
                 # Call item.get() on this one, for example on click
             elif isinstance(item, PageLink):
-                print("\t" + item.title)
+                items.append("\t" + item.title)
                 # Call item.get() on this one, for example on click
             elif isinstance(item, Mix):
-                print("\t" + item.title)
+                items.append("\t" + item.title)
                 # You can optionally call item.get() to request the items() first, but it does it for you if you don't
             else:
-                print("\t" + item.name)
+                items.append("\t" + item.name)
                 # An album could be handled by session.album(item.id) for example,
                 # to get full details. Usually the relevant info is there already however
             print()
+        [print(x) for x in sorted(items)]
 
 .. testoutput::
     :hide:
     :options: +ELLIPSIS, +NORMALIZE_WHITESPACE
 
     For You...
     Recently Played...
-    Mixes For You...
-    Trending Playlists...
-    Radio Stations for You...
     Suggested New Tracks...
     Suggested New Albums...
+    Mixes For You...
+    Radio Stations for You...
     Your History...
+    Trending Playlists...
     Popular Playlists...
     TIDAL Rising...
     The Charts...
     Popular Albums...
     Podcasts...
     Radio Stations for You...
     Producers & Songwriters...
```

### Comparing `tidalapi-0.7.0rc1/setup.py` & `tidalapi-0.7.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,25 +13,25 @@
 
 long_description = ""
 with open('README.rst') as f:
     long_description += f.read()
 
 with open('HISTORY.rst') as f:
     long_description += '\n\n'
-    long_description += f.read() .replace('.. :changelog:', '')
+    long_description += f.read().replace('.. :changelog:', '')
 
 setup(
     name='tidalapi',
-    version='0.7.0rc1',
+    version='0.7.1',
     description='Unofficial API for TIDAL music streaming service.',
     long_description=long_description,
     author='Thomas Amland',
     author_email='thomas.amland@googlemail.com',
-    maintainer='morguldir',
-    maintainer_email='morguldir@protonmail.com',
+    maintainer='tehkillerbee',
+    maintainer_email='josaksel.dk@gmail.com',
     url='https://github.com/tamland/python-tidal',
     license='LGPL',
     packages=['tidalapi'],
     install_requires=required,
     keywords='',
     classifiers=[
         'Development Status :: 4 - Beta',
```

### Comparing `tidalapi-0.7.0rc1/tests/conftest.py` & `tidalapi-0.7.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `tidalapi-0.7.0rc1/tests/cover.py` & `tidalapi-0.7.1/tests/cover.py`

 * *Files identical despite different names*

### Comparing `tidalapi-0.7.0rc1/tests/test_album.py` & `tidalapi-0.7.1/tests/test_album.py`

 * *Files 3% similar despite different names*

```diff
@@ -99,7 +99,13 @@
     assert album.image(1280) == tidalapi.album.DEFAULT_ALBUM_IMAGE
 
 
 def test_similar(session):
     album = session.album(108043414)
     for alb in album.similar():
         assert isinstance(alb.similar()[0], tidalapi.Album)
+
+
+def test_review(session):
+    album = session.album(199142349)
+    review = album.review()
+    assert "Kanye West" in review
```

### Comparing `tidalapi-0.7.0rc1/tests/test_artist.py` & `tidalapi-0.7.1/tests/test_artist.py`

 * *Files identical despite different names*

### Comparing `tidalapi-0.7.0rc1/tests/test_genres.py` & `tidalapi-0.7.1/tests/test_genres.py`

 * *Files identical despite different names*

### Comparing `tidalapi-0.7.0rc1/tests/test_media.py` & `tidalapi-0.7.1/tests/test_media.py`

 * *Files identical despite different names*

### Comparing `tidalapi-0.7.0rc1/tests/test_page.py` & `tidalapi-0.7.1/tests/test_page.py`

 * *Files 2% similar despite different names*

```diff
@@ -97,15 +97,15 @@
     assert first_local != first
     assert isinstance(next(iter(first_local.get())).get(), tidalapi.Playlist)
 
 
 def test_moods(session):
     moods = session.moods()
     first = next(iter(moods))
-    assert first.title == 'Workout'
+    assert first.title == 'Music School'
     assert isinstance(next(iter(first.get())), tidalapi.Playlist)
 
 
 def test_mixes(session):
     mixes = session.mixes()
     first = next(iter(mixes))
     assert first.title == "My Daily Discovery"
```

### Comparing `tidalapi-0.7.0rc1/tests/test_playlist.py` & `tidalapi-0.7.1/tests/test_playlist.py`

 * *Files identical despite different names*

### Comparing `tidalapi-0.7.0rc1/tests/test_session.py` & `tidalapi-0.7.1/tests/test_session.py`

 * *Files identical despite different names*

### Comparing `tidalapi-0.7.0rc1/tests/test_user.py` & `tidalapi-0.7.1/tests/test_user.py`

 * *Files identical despite different names*

### Comparing `tidalapi-0.7.0rc1/tidalapi/album.py` & `tidalapi-0.7.1/tidalapi/album.py`

 * *Files 6% similar despite different names*

```diff
@@ -190,7 +190,17 @@
     def similar(self):
         """
         Retrieve albums similar to the current one
 
         :return: A :any:`list` of similar albums
         """
         return self.requests.map_request('albums/%s/similar' % self.id, parse=self.session.parse_album)
+
+    def review(self) -> str:
+        """
+        Retrieve the album review
+
+        :return: A :class:`str` containing the album review, with wimp links
+        :raises: :class:`requests.HTTPError` if there isn't a review yet
+        """
+        # morguldir: TODO: Add parsing of wimplinks?
+        return self.requests.request('GET', 'albums/%s/review' % self.id).json()['text']
```

### Comparing `tidalapi-0.7.0rc1/tidalapi/artist.py` & `tidalapi-0.7.1/tidalapi/artist.py`

 * *Files identical despite different names*

### Comparing `tidalapi-0.7.0rc1/tidalapi/genre.py` & `tidalapi-0.7.1/tidalapi/genre.py`

 * *Files identical despite different names*

### Comparing `tidalapi-0.7.0rc1/tidalapi/media.py` & `tidalapi-0.7.1/tidalapi/media.py`

 * *Files 2% similar despite different names*

```diff
@@ -168,14 +168,22 @@
         Retrieves the lyrics for a song
 
         :return: A :class:`Lyrics` object containing the lyrics
         :raises: A :class:`requests.HTTPError` if there aren't any lyrics
         """
         return self.requests.map_request('tracks/%s/lyrics' % self.id, parse=Lyrics().parse)
 
+    def get_track_radio(self):
+        """
+        Queries TIDAL for the track radio, which is a mix of tracks that are similar to this track.
+
+        :return: A list of :class:`Tracks <tidalapi.media.Track>`
+        """
+        params = {'limit': 100}
+        return self.requests.map_request('tracks/%s/radio' % self.id, params=params, parse=self.session.parse_track)
 
 class Lyrics(object):
     track_id = -1
     provider = ""
     provider_track_id = -1
     provider_lyrics_id = -1
     text = ""
```

### Comparing `tidalapi-0.7.0rc1/tidalapi/mix.py` & `tidalapi-0.7.1/tidalapi/mix.py`

 * *Files identical despite different names*

### Comparing `tidalapi-0.7.0rc1/tidalapi/page.py` & `tidalapi-0.7.1/tidalapi/page.py`

 * *Files identical despite different names*

### Comparing `tidalapi-0.7.0rc1/tidalapi/playlist.py` & `tidalapi-0.7.1/tidalapi/playlist.py`

 * *Files 6% similar despite different names*

```diff
@@ -201,14 +201,20 @@
         self.requests.request('POST', self._base_url % self.id + '/items', params=params, data=data, headers=headers)
         self._reparse()
 
     def remove_by_index(self, index):
         headers = {'If-None-Match': self._etag}
         self.requests.request('DELETE', (self._base_url + '/items/%i') % (self.id, index), headers=headers)
 
+    def remove_by_indices(self, indices):
+        headers = {'If-None-Match': self._etag}
+        track_index_string = ",".join([str(x) for x in indices])
+        self.requests.request('DELETE', (self._base_url + '/tracks/%s') % (self.id, track_index_string),
+                                 headers=headers)
+
     def _calculate_id(self, media_id):
         i = 0
         while i < self.num_tracks:
             items = self.items(100, i)
             for index, item in enumerate(items):
                 if item.id == media_id:
                     # Return the amount of items we have gone through plus the index in the last list.
```

### Comparing `tidalapi-0.7.0rc1/tidalapi/request.py` & `tidalapi-0.7.1/tidalapi/request.py`

 * *Files identical despite different names*

### Comparing `tidalapi-0.7.0rc1/tidalapi/session.py` & `tidalapi-0.7.1/tidalapi/session.py`

 * *Files 0% similar despite different names*

```diff
@@ -350,15 +350,15 @@
         json = request.json()
         executor = concurrent.futures.ThreadPoolExecutor()
         return LinkLogin(json), executor.submit(self._process_link_login, json)
 
     def _process_link_login(self, json):
         json = self._wait_for_link_login(json)
         self.access_token = json['access_token']
-        self.expiry_time = datetime.datetime.now() + datetime.timedelta(seconds=json['expires_in'])
+        self.expiry_time = datetime.datetime.utcnow() + datetime.timedelta(seconds=json['expires_in'])
         self.refresh_token = json['refresh_token']
         self.token_type = json['token_type']
         session = self.request.request('GET', 'sessions')
         json = session.json()
         self.session_id = json['sessionId']
         self.country_code = json['countryCode']
         self.user = tidalapi.User(self, user_id=json['userId']).factory()
@@ -405,15 +405,15 @@
 
         request = self.request_session.post(url, params)
         json = request.json()
         if not request.ok:
             log.warning("The refresh token has expired, a new login is required.")
             return False
         self.access_token = json['access_token']
-        self.expiry_time = datetime.datetime.now() + datetime.timedelta(seconds=json['expires_in'])
+        self.expiry_time = datetime.datetime.utcnow() + datetime.timedelta(seconds=json['expires_in'])
         self.token_type = json['token_type']
         return True
 
     def search(self, query, models=None, limit=50, offset=0):
         """
         Searches TIDAL with the specified query, you can also specify what models you want to search for.
         While you can set the offset, there aren't more than 300 items available in a search.
```

### Comparing `tidalapi-0.7.0rc1/tidalapi/user.py` & `tidalapi-0.7.1/tidalapi/user.py`

 * *Files 12% similar despite different names*

```diff
@@ -32,61 +32,65 @@
     A class containing various information about a TIDAL user.
 
     The attributes of this class are pretty varied. ID is the only attribute you can rely on being set.
     If you initialized a specific user, you will get id, first_name, last_name, and picture_id.
     If parsed as a playlist creator, you will get an ID and a name, if the creator isn't an artist, name will be 'user'.
     If the parsed user is the one logged in, for example in session.user, you will get the remaining attributes, and id.
     """
+
     id = -1
 
     def __init__(self, session, user_id):
         self.id = user_id
         self.session = session
         self.request = session.request
         self.playlist = session.playlist()
 
     def factory(self):
-        return self.request.map_request('users/%s' % self.id, parse=self.parse)
+        return self.request.map_request("users/%s" % self.id, parse=self.parse)
 
     def parse(self, json_obj):
+        if "username" in json_obj:
+            user = LoggedInUser(self.session, json_obj["id"])
 
-        if 'username' in json_obj:
-            user = LoggedInUser(self.session, json_obj['id'])
-
-        elif 'firstName' in json_obj:
-            user = FetchedUser(self.session, json_obj['id'])
+        elif "firstName" in json_obj:
+            user = FetchedUser(self.session, json_obj["id"])
 
         elif json_obj:
-            user = PlaylistCreator(self.session, json_obj['id'])
+            user = PlaylistCreator(self.session, json_obj["id"])
 
         # When searching TIDAL does not show up as a creator in the json data.
         else:
             user = PlaylistCreator(self.session, 0)
 
         return user.parse(json_obj)
 
 
 class FetchedUser(User):
     first_name = None
     last_name = None
     picture_id = None
 
     def parse(self, json_obj):
-        self.id = json_obj['id']
-        self.first_name = json_obj['firstName']
-        self.last_name = json_obj['lastName']
-        self.picture_id = json_obj['picture']
+        self.id = json_obj["id"]
+        self.first_name = json_obj["firstName"]
+        self.last_name = json_obj["lastName"]
+        self.picture_id = json_obj.get("picture", None)
 
         return copy(self)
 
     def image(self, dimensions):
         if dimensions not in [100, 210, 600]:
             raise ValueError("Invalid resolution {0} x {0}".format(dimensions))
 
-        return self.session.config.image_url % (self.picture_id.replace('-', '/'), dimensions, dimensions)
+        return self.session.config.image_url % (
+            self.picture_id.replace("-", "/"),
+            dimensions,
+            dimensions,
+        )
 
 
 class LoggedInUser(FetchedUser):
     username = None
     email = None
     created = None
     newsletter = None
@@ -98,215 +102,255 @@
 
     def __init__(self, session, user_id):
         super(LoggedInUser, self).__init__(session, user_id)
         self.favorites = Favorites(session, self.id)
 
     def parse(self, json_obj):
         super(LoggedInUser, self).parse(json_obj)
-        self.username = json_obj['username']
-        self.email = json_obj['email']
-        self.created = dateutil.parser.isoparse(json_obj['created'])
-        self.newsletter = json_obj['newsletter']
-        self.accepted_eula = json_obj['acceptedEULA']
-        self.gender = json_obj['gender']
-        self.date_of_birth = json_obj['dateOfBirth']
-        self.facebook_uid = json_obj['facebookUid']
-        self.apple_uid = json_obj['appleUid']
+        self.username = json_obj["username"]
+        self.email = json_obj["email"]
+        self.created = dateutil.parser.isoparse(json_obj["created"])
+        self.newsletter = json_obj["newsletter"]
+        self.accepted_eula = json_obj["acceptedEULA"]
+        self.gender = json_obj["gender"]
+        self.date_of_birth = json_obj["dateOfBirth"]
+        self.facebook_uid = json_obj["facebookUid"]
+        self.apple_uid = json_obj["appleUid"]
 
         return copy(self)
 
     def playlists(self):
         """
         Get the playlists created by the user.
 
         :return: Returns a list of :class:`~tidalapi.playlist.Playlist` objects containing the playlists.
         """
-        return self.request.map_request('users/%s/playlists' % self.id, parse=self.playlist.parse_factory)
+        return self.request.map_request(
+            "users/%s/playlists" % self.id, parse=self.playlist.parse_factory
+        )
 
     def playlist_and_favorite_playlists(self, offset=0):
         """
         Get the playlists created by the user, and the playlists favorited by the user.
         This function is limited to 50 by TIDAL, requiring pagination.
 
         :return: Returns a list of :class:`~tidalapi.playlist.Playlist` objects containing the playlists.
         """
-        params = {'limit': 50, 'offset': offset}
-        endpoint = 'users/%s/playlistsAndFavoritePlaylists' % self.id
-        json_obj = self.request.request('GET', endpoint, params=params).json()
+        params = {"limit": 50, "offset": offset}
+        endpoint = "users/%s/playlistsAndFavoritePlaylists" % self.id
+        json_obj = self.request.request("GET", endpoint, params=params).json()
 
         # This endpoint sorts them into favorited and created playlists, but we already do that when parsing them.
-        for index, item in enumerate(json_obj['items']):
-            item['playlist']['dateAdded'] = item['created']
-            json_obj['items'][index] = item['playlist']
+        for index, item in enumerate(json_obj["items"]):
+            item["playlist"]["dateAdded"] = item["created"]
+            json_obj["items"][index] = item["playlist"]
 
         return self.request.map_json(json_obj, parse=self.playlist.parse_factory)
 
     def create_playlist(self, title, description):
-        data = {'title': title, 'description': description}
-        json = self.request.request('POST', 'users/%s/playlists' % self.id, data=data).json()
+        data = {"title": title, "description": description}
+        json = self.request.request(
+            "POST", "users/%s/playlists" % self.id, data=data
+        ).json()
         playlist = self.session.playlist().parse(json)
         return playlist.factory()
 
 
 class PlaylistCreator(User):
     name = None
 
     def parse(self, json_obj):
         if self.id == 0:
             self.name = "TIDAL"
 
-        elif 'name' in json_obj:
-            self.name = json_obj['name']
+        elif "name" in json_obj:
+            self.name = json_obj["name"]
 
         elif self.id == self.session.user.id:
             self.name = "me"
 
         else:
             self.name = "user"
 
         return copy(self)
 
 
 class Favorites(object):
     """
     An object containing a users favourites.
     """
+
     def __init__(self, session, user_id):
         self.session = session
         self.requests = session.request
-        self.base_url = 'users/%s/favorites' % user_id
+        self.base_url = "users/%s/favorites" % user_id
 
     def add_album(self, album_id):
         """
         Adds an album to the users favorites.
 
         :param album_id: TIDAL's identifier of the album.
         :return: A boolean indicating whether the request was successful or not.
         """
-        return self.requests.request('POST', self.base_url + '/albums', data={'albumId': album_id}).ok
+        return self.requests.request(
+            "POST", self.base_url + "/albums", data={"albumId": album_id}
+        ).ok
 
     def add_artist(self, artist_id):
         """
         Adds an artist to the users favorites.
 
         :param artist_id: TIDAL's identifier of the artist
         :return: A boolean indicating whether the request was successful or not.
         """
-        return self.requests.request('POST', self.base_url + '/artists', data={'artistId': artist_id}).ok
+        return self.requests.request(
+            "POST", self.base_url + "/artists", data={"artistId": artist_id}
+        ).ok
 
     def add_playlist(self, playlist_id):
         """
         Adds a playlist to the users favorites.
 
         :param playlist_id:  TIDAL's identifier of the playlist.
         :return: A boolean indicating whether the request was successful or not.
         """
-        return self.requests.request('POST', self.base_url + '/playlists', data={'uuids': playlist_id}).ok
+        return self.requests.request(
+            "POST", self.base_url + "/playlists", data={"uuids": playlist_id}
+        ).ok
 
     def add_track(self, track_id):
         """
         Adds a track to the users favorites.
 
         :param track_id: TIDAL's identifier of the track.
         :return: A boolean indicating whether the request was successful or not.
         """
-        return self.requests.request('POST', self.base_url + '/tracks', data={'trackId': track_id}).ok
+        return self.requests.request(
+            "POST", self.base_url + "/tracks", data={"trackId": track_id}
+        ).ok
 
     def add_video(self, video_id):
         """
         Adds a video to the users favorites.
 
         :param video_id: TIDAL's identifier of the video.
         :return: A boolean indicating whether the request was successful or not.
         """
-        params = {'limit': '100'}
-        return self.requests.request('POST', self.base_url + '/videos', data={'videoIds': video_id}, params=params).ok
+        params = {"limit": "100"}
+        return self.requests.request(
+            "POST",
+            self.base_url + "/videos",
+            data={"videoIds": video_id},
+            params=params,
+        ).ok
 
     def remove_artist(self, artist_id):
         """
         Removes a track from the users favorites.
 
         :param artist_id: TIDAL's identifier of the artist.
         :return: A boolean indicating whether the request was successful or not.
         """
-        return self.requests.request('DELETE', self.base_url + '/artists/%s' % artist_id).ok
+        return self.requests.request(
+            "DELETE", self.base_url + "/artists/%s" % artist_id
+        ).ok
 
     def remove_album(self, album_id):
         """
         Removes an album from the users favorites.
 
         :param album_id: TIDAL's identifier of the album
         :return: A boolean indicating whether the request was successful or not.
         """
-        return self.requests.request('DELETE', self.base_url + '/albums/%s' % album_id).ok
+        return self.requests.request(
+            "DELETE", self.base_url + "/albums/%s" % album_id
+        ).ok
 
     def remove_playlist(self, playlist_id):
         """
         Removes a playlist from the users favorites.
 
         :param playlist_id: TIDAL's identifier of the playlist.
         :return: A boolean indicating whether the request was successful or not.
         """
-        return self.requests.request('DELETE', self.base_url + '/playlists/%s' % playlist_id).ok
+        return self.requests.request(
+            "DELETE", self.base_url + "/playlists/%s" % playlist_id
+        ).ok
 
     def remove_track(self, track_id):
         """
         Removes a track from the users favorites.
 
         :param track_id: TIDAL's identifier of the track.
         :return: A boolean indicating whether the request was successful or not.
         """
-        return self.requests.request('DELETE', self.base_url + '/tracks/%s' % track_id).ok
+        return self.requests.request(
+            "DELETE", self.base_url + "/tracks/%s" % track_id
+        ).ok
 
     def remove_video(self, video_id):
         """
         Removes a video from the users favorites.
 
         :param video_id: TIDAL's identifier of the video.
         :return: A boolean indicating whether the request was successful or not.
 
         """
-        return self.requests.request('DELETE', self.base_url + '/videos/%s' % video_id).ok
+        return self.requests.request(
+            "DELETE", self.base_url + "/videos/%s" % video_id
+        ).ok
 
     def artists(self, limit=None, offset=0):
         """
         Get the users favorite artists
 
         :return: A :class:`list` of :class:`~tidalapi.artist.Artist` objects containing the favorite artists.
         """
-        params = {'limit': limit, 'offset': offset}
-        return self.requests.map_request(self.base_url + '/artists', params=params, parse=self.session.parse_artist)
+        params = {"limit": limit, "offset": offset}
+        return self.requests.map_request(
+            self.base_url + "/artists", params=params, parse=self.session.parse_artist
+        )
 
     def albums(self, limit=None, offset=0):
         """
         Get the users favorite albums
 
         :return: A :class:`list` of :class:`~tidalapi.album.Album` objects containing the favorite albums.
         """
-        params = {'limit': limit, 'offset': offset}
-        return self.requests.map_request(self.base_url + '/albums', params=params, parse=self.session.parse_album)
+        params = {"limit": limit, "offset": offset}
+        return self.requests.map_request(
+            self.base_url + "/albums", params=params, parse=self.session.parse_album
+        )
 
     def playlists(self, limit=None, offset=0):
         """
         Get the users favorite playlists
 
         :return: A :class:`list` :class:`~tidalapi.playlist.Playlist` objects containing the favorite playlists.
         """
-        params = {'limit': limit, 'offset': offset}
-        return self.requests.map_request(self.base_url + '/playlists', params=params, parse=self.session.parse_playlist)
+        params = {"limit": limit, "offset": offset}
+        return self.requests.map_request(
+            self.base_url + "/playlists",
+            params=params,
+            parse=self.session.parse_playlist,
+        )
 
     def tracks(self, limit=None, offset=0):
         """
         Get the users favorite tracks
 
         :return: A :class:`list` of :class:`~tidalapi.track.Track` objects containing all of the favorite tracks.
         """
-        params = {'limit': limit, 'offset': offset}
-        return self.requests.map_request(self.base_url + '/tracks', params=params, parse=self.session.parse_track)
+        params = {"limit": limit, "offset": offset}
+        return self.requests.map_request(
+            self.base_url + "/tracks", params=params, parse=self.session.parse_track
+        )
 
     def videos(self):
         """
         Get the users favorite videos
 
         :return: A :class:`list` of :class:`~tidalapi.media.Video` objects containing all the favorite videos
         """
-        return self.requests.get_items(self.base_url + '/videos', parse=self.session.parse_media)
+        return self.requests.get_items(
+            self.base_url + "/videos", parse=self.session.parse_media
+        )
```

