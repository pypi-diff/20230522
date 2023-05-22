# Comparing `tmp/picassosr-0.6.0.tar.gz` & `tmp/picassosr-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "picassosr-0.6.0.tar", last modified: Fri Feb 17 14:51:51 2023, max compression
+gzip compressed data, was "picassosr-0.6.1.tar", last modified: Mon May 22 09:40:10 2023, max compression
```

## Comparing `picassosr-0.6.0.tar` & `picassosr-0.6.1.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 14:51:51.663369 picassosr-0.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-02-17 14:51:29.000000 picassosr-0.6.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)    10171 2023-02-17 14:51:51.663369 picassosr-0.6.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 14:51:51.659369 picassosr-0.6.0/picasso/
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-02-17 14:51:29.000000 picassosr-0.6.0/picasso/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    56760 2023-02-17 14:51:29.000000 picassosr-0.6.0/picasso/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-02-17 14:51:29.000000 picassosr-0.6.0/picasso/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4267 2023-02-17 14:51:29.000000 picassosr-0.6.0/picasso/avgroi.py
--rw-r--r--   0 runner    (1001) docker     (123)    20436 2023-02-17 14:51:29.000000 picassosr-0.6.0/picasso/clusterer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3286 2023-02-17 14:51:29.000000 picassosr-0.6.0/picasso/config_template.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4183 2023-02-17 14:51:29.000000 picassosr-0.6.0/picasso/design.py
--rw-r--r--   0 runner    (1001) docker     (123)    12374 2023-02-17 14:51:29.000000 picassosr-0.6.0/picasso/design_sequences.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 14:51:51.659369 picassosr-0.6.0/picasso/ext/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-17 14:51:29.000000 picassosr-0.6.0/picasso/ext/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12450 2023-02-17 14:51:29.000000 picassosr-0.6.0/picasso/ext/bitplane.py
--rw-r--r--   0 runner    (1001) docker     (123)     9793 2023-02-17 14:51:29.000000 picassosr-0.6.0/picasso/gausslq.py
--rw-r--r--   0 runner    (1001) docker     (123)    22088 2023-02-17 14:51:29.000000 picassosr-0.6.0/picasso/gaussmle.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 14:51:51.659369 picassosr-0.6.0/picasso/gui/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-17 14:51:29.000000 picassosr-0.6.0/picasso/gui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13913 2023-02-17 14:51:29.000000 picassosr-0.6.0/picasso/gui/average.py
--rw-r--r--   0 runner    (1001) docker     (123)    72322 2023-02-17 14:51:29.000000 picassosr-0.6.0/picasso/gui/average3.py
--rw-r--r--   0 runner    (1001) docker     (123)    52463 2023-02-17 14:51:29.000000 picassosr-0.6.0/picasso/gui/design.py
--rw-r--r--   0 runner    (1001) docker     (123)    17903 2023-02-17 14:51:29.000000 picassosr-0.6.0/picasso/gui/filter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 14:51:51.663369 picassosr-0.6.0/picasso/gui/icons/
--rw-r--r--   0 runner    (1001) docker     (123)   175462 2023-02-17 14:51:29.000000 picassosr-0.6.0/picasso/gui/icons/average.ico
--rw-r--r--   0 runner    (1001) docker     (123)   152656 2023-02-17 14:51:29.000000 picassosr-0.6.0/picasso/gui/icons/design.ico
--rw-r--r--   0 runner    (1001) docker     (123)   156571 2023-02-17 14:51:29.000000 picassosr-0.6.0/picasso/gui/icons/filter.ico
--rw-r--r--   0 runner    (1001) docker     (123)   150560 2023-02-17 14:51:29.000000 picassosr-0.6.0/picasso/gui/icons/localize.ico
--rw-r--r--   0 runner    (1001) docker     (123)   108693 2023-02-17 14:51:29.000000 picassosr-0.6.0/picasso/gui/icons/nanotron.ico
--rw-r--r--   0 runner    (1001) docker     (123)    15878 2023-02-17 14:51:29.000000 picassosr-0.6.0/picasso/gui/icons/picasso_server.png
--rw-r--r--   0 runner    (1001) docker     (123)   163812 2023-02-17 14:51:29.000000 picassosr-0.6.0/picasso/gui/icons/render.ico
--rw-r--r--   0 runner    (1001) docker     (123)   234758 2023-02-17 14:51:29.000000 picassosr-0.6.0/picasso/gui/icons/server.ico
--rw-r--r--   0 runner    (1001) docker     (123)   146322 2023-02-17 14:51:29.000000 picassosr-0.6.0/picasso/gui/icons/simulate.ico
--rw-r--r--   0 runner    (1001) docker     (123)   157098 2023-02-17 14:51:29.000000 picassosr-0.6.0/picasso/gui/icons/toraw.ico
--rw-r--r--   0 runner    (1001) docker     (123)    79250 2023-02-17 14:51:29.000000 picassosr-0.6.0/picasso/gui/localize.py
--rw-r--r--   0 runner    (1001) docker     (123)    48499 2023-02-17 14:51:29.000000 picassosr-0.6.0/picasso/gui/nanotron.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 14:51:51.663369 picassosr-0.6.0/picasso/gui/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-17 14:51:29.000000 picassosr-0.6.0/picasso/gui/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   435316 2023-02-17 14:51:29.000000 picassosr-0.6.0/picasso/gui/render.py
--rw-r--r--   0 runner    (1001) docker     (123)    86597 2023-02-17 14:51:29.000000 picassosr-0.6.0/picasso/gui/rotation.py
--rw-r--r--   0 runner    (1001) docker     (123)    86505 2023-02-17 14:51:29.000000 picassosr-0.6.0/picasso/gui/simulate.py
--rw-r--r--   0 runner    (1001) docker     (123)     5560 2023-02-17 14:51:29.000000 picassosr-0.6.0/picasso/gui/toraw.py
--rw-r--r--   0 runner    (1001) docker     (123)     3919 2023-02-17 14:51:29.000000 picassosr-0.6.0/picasso/imageprocess.py
--rw-r--r--   0 runner    (1001) docker     (123)    43608 2023-02-17 14:51:29.000000 picassosr-0.6.0/picasso/io.py
--rw-r--r--   0 runner    (1001) docker     (123)     7862 2023-02-17 14:51:29.000000 picassosr-0.6.0/picasso/lib.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    16930 2023-02-17 14:51:29.000000 picassosr-0.6.0/picasso/localize.py
--rw-r--r--   0 runner    (1001) docker     (123)     3203 2023-02-17 14:51:29.000000 picassosr-0.6.0/picasso/nanotron.py
--rw-r--r--   0 runner    (1001) docker     (123)    43142 2023-02-17 14:51:29.000000 picassosr-0.6.0/picasso/postprocess.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    29630 2023-02-17 14:51:29.000000 picassosr-0.6.0/picasso/render.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 14:51:51.663369 picassosr-0.6.0/picasso/server/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-17 14:51:29.000000 picassosr-0.6.0/picasso/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-02-17 14:51:29.000000 picassosr-0.6.0/picasso/server/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     5896 2023-02-17 14:51:29.000000 picassosr-0.6.0/picasso/server/compare.py
--rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-02-17 14:51:29.000000 picassosr-0.6.0/picasso/server/helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     8219 2023-02-17 14:51:29.000000 picassosr-0.6.0/picasso/server/history.py
--rw-r--r--   0 runner    (1001) docker     (123)     3924 2023-02-17 14:51:29.000000 picassosr-0.6.0/picasso/server/preview.py
--rw-r--r--   0 runner    (1001) docker     (123)     5947 2023-02-17 14:51:29.000000 picassosr-0.6.0/picasso/server/status.py
--rw-r--r--   0 runner    (1001) docker     (123)    14193 2023-02-17 14:51:29.000000 picassosr-0.6.0/picasso/server/watcher.py
--rw-r--r--   0 runner    (1001) docker     (123)    13023 2023-02-17 14:51:29.000000 picassosr-0.6.0/picasso/simulate.py
--rw-r--r--   0 runner    (1001) docker     (123)     9060 2023-02-17 14:51:29.000000 picassosr-0.6.0/picasso/zfit.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 14:51:51.663369 picassosr-0.6.0/picassosr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10171 2023-02-17 14:51:51.000000 picassosr-0.6.0/picassosr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-02-17 14:51:51.000000 picassosr-0.6.0/picassosr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-17 14:51:51.000000 picassosr-0.6.0/picassosr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-02-17 14:51:51.000000 picassosr-0.6.0/picassosr.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-02-17 14:51:51.000000 picassosr-0.6.0/picassosr.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-02-17 14:51:51.000000 picassosr-0.6.0/picassosr.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-17 14:51:51.663369 picassosr-0.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-02-17 14:51:29.000000 picassosr-0.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 09:40:10.158484 picassosr-0.6.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-05-22 09:39:47.000000 picassosr-0.6.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     9538 2023-05-22 09:40:10.154484 picassosr-0.6.1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 09:40:10.150484 picassosr-0.6.1/picasso/
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-05-22 09:39:47.000000 picassosr-0.6.1/picasso/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57108 2023-05-22 09:39:47.000000 picassosr-0.6.1/picasso/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-22 09:39:47.000000 picassosr-0.6.1/picasso/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4267 2023-05-22 09:39:47.000000 picassosr-0.6.1/picasso/avgroi.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20436 2023-05-22 09:39:47.000000 picassosr-0.6.1/picasso/clusterer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3286 2023-05-22 09:39:47.000000 picassosr-0.6.1/picasso/config_template.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4183 2023-05-22 09:39:47.000000 picassosr-0.6.1/picasso/design.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12374 2023-05-22 09:39:47.000000 picassosr-0.6.1/picasso/design_sequences.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 09:40:10.150484 picassosr-0.6.1/picasso/ext/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 09:39:47.000000 picassosr-0.6.1/picasso/ext/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12450 2023-05-22 09:39:47.000000 picassosr-0.6.1/picasso/ext/bitplane.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9793 2023-05-22 09:39:47.000000 picassosr-0.6.1/picasso/gausslq.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22088 2023-05-22 09:39:47.000000 picassosr-0.6.1/picasso/gaussmle.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 09:40:10.150484 picassosr-0.6.1/picasso/gui/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 09:39:47.000000 picassosr-0.6.1/picasso/gui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13913 2023-05-22 09:39:47.000000 picassosr-0.6.1/picasso/gui/average.py
+-rw-r--r--   0 runner    (1001) docker     (123)    72322 2023-05-22 09:39:47.000000 picassosr-0.6.1/picasso/gui/average3.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52463 2023-05-22 09:39:47.000000 picassosr-0.6.1/picasso/gui/design.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17903 2023-05-22 09:39:47.000000 picassosr-0.6.1/picasso/gui/filter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 09:40:10.154484 picassosr-0.6.1/picasso/gui/icons/
+-rw-r--r--   0 runner    (1001) docker     (123)   175462 2023-05-22 09:39:47.000000 picassosr-0.6.1/picasso/gui/icons/average.ico
+-rw-r--r--   0 runner    (1001) docker     (123)   152656 2023-05-22 09:39:47.000000 picassosr-0.6.1/picasso/gui/icons/design.ico
+-rw-r--r--   0 runner    (1001) docker     (123)   156571 2023-05-22 09:39:47.000000 picassosr-0.6.1/picasso/gui/icons/filter.ico
+-rw-r--r--   0 runner    (1001) docker     (123)   150560 2023-05-22 09:39:47.000000 picassosr-0.6.1/picasso/gui/icons/localize.ico
+-rw-r--r--   0 runner    (1001) docker     (123)   108693 2023-05-22 09:39:47.000000 picassosr-0.6.1/picasso/gui/icons/nanotron.ico
+-rw-r--r--   0 runner    (1001) docker     (123)    15878 2023-05-22 09:39:47.000000 picassosr-0.6.1/picasso/gui/icons/picasso_server.png
+-rw-r--r--   0 runner    (1001) docker     (123)   163812 2023-05-22 09:39:47.000000 picassosr-0.6.1/picasso/gui/icons/render.ico
+-rw-r--r--   0 runner    (1001) docker     (123)   234758 2023-05-22 09:39:47.000000 picassosr-0.6.1/picasso/gui/icons/server.ico
+-rw-r--r--   0 runner    (1001) docker     (123)   146322 2023-05-22 09:39:47.000000 picassosr-0.6.1/picasso/gui/icons/simulate.ico
+-rw-r--r--   0 runner    (1001) docker     (123)   157098 2023-05-22 09:39:47.000000 picassosr-0.6.1/picasso/gui/icons/toraw.ico
+-rw-r--r--   0 runner    (1001) docker     (123)    79626 2023-05-22 09:39:47.000000 picassosr-0.6.1/picasso/gui/localize.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48499 2023-05-22 09:39:47.000000 picassosr-0.6.1/picasso/gui/nanotron.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 09:40:10.154484 picassosr-0.6.1/picasso/gui/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 09:39:47.000000 picassosr-0.6.1/picasso/gui/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   437273 2023-05-22 09:39:47.000000 picassosr-0.6.1/picasso/gui/render.py
+-rw-r--r--   0 runner    (1001) docker     (123)    87147 2023-05-22 09:39:47.000000 picassosr-0.6.1/picasso/gui/rotation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    86505 2023-05-22 09:39:47.000000 picassosr-0.6.1/picasso/gui/simulate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5560 2023-05-22 09:39:47.000000 picassosr-0.6.1/picasso/gui/toraw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3919 2023-05-22 09:39:47.000000 picassosr-0.6.1/picasso/imageprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43588 2023-05-22 09:39:47.000000 picassosr-0.6.1/picasso/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7862 2023-05-22 09:39:47.000000 picassosr-0.6.1/picasso/lib.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16930 2023-05-22 09:39:47.000000 picassosr-0.6.1/picasso/localize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3203 2023-05-22 09:39:47.000000 picassosr-0.6.1/picasso/nanotron.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43142 2023-05-22 09:39:47.000000 picassosr-0.6.1/picasso/postprocess.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    29624 2023-05-22 09:39:47.000000 picassosr-0.6.1/picasso/render.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 09:40:10.154484 picassosr-0.6.1/picasso/server/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 09:39:47.000000 picassosr-0.6.1/picasso/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-05-22 09:39:47.000000 picassosr-0.6.1/picasso/server/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5896 2023-05-22 09:39:47.000000 picassosr-0.6.1/picasso/server/compare.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-05-22 09:39:47.000000 picassosr-0.6.1/picasso/server/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8219 2023-05-22 09:39:47.000000 picassosr-0.6.1/picasso/server/history.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3924 2023-05-22 09:39:47.000000 picassosr-0.6.1/picasso/server/preview.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5947 2023-05-22 09:39:47.000000 picassosr-0.6.1/picasso/server/status.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14193 2023-05-22 09:39:47.000000 picassosr-0.6.1/picasso/server/watcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13023 2023-05-22 09:39:47.000000 picassosr-0.6.1/picasso/simulate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9060 2023-05-22 09:39:47.000000 picassosr-0.6.1/picasso/zfit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 09:40:10.154484 picassosr-0.6.1/picassosr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9538 2023-05-22 09:40:10.000000 picassosr-0.6.1/picassosr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-05-22 09:40:10.000000 picassosr-0.6.1/picassosr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 09:40:10.000000 picassosr-0.6.1/picassosr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-22 09:40:10.000000 picassosr-0.6.1/picassosr.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-22 09:40:10.000000 picassosr-0.6.1/picassosr.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-22 09:40:10.000000 picassosr-0.6.1/picassosr.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 09:40:10.158484 picassosr-0.6.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-05-22 09:39:47.000000 picassosr-0.6.1/setup.py
```

### Comparing `picassosr-0.6.0/LICENSE.txt` & `picassosr-0.6.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `picassosr-0.6.0/PKG-INFO` & `picassosr-0.6.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: picassosr
-Version: 0.6.0
+Version: 0.6.1
 Home-page: https://github.com/jungmannlab/picasso
 Author: Joerg Schnitzbauer, Maximilian T. Strauss, Rafal Kowalewski
 Author-email: joschnitzbauer@gmail.com, straussmaximilian@gmail.com, rafalkowalewski998@gmail.com
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -32,37 +32,21 @@
    :scale: 100 %
    :alt: UML Render view
 
 A collection of tools for painting super-resolution images. The Picasso software is complemented by our `Nature Protocols publication <https://www.nature.com/nprot/journal/v12/n6/abs/nprot.2017.024.html>`__.
 A comprehensive documentation can be found here: `Read the Docs <https://picassosr.readthedocs.io/en/latest/?badge=latest>`__.
 
 
-Picasso 0.6.0
+Picasso 0.6.1
 -------------
+In previous version, the rotation window (3D Render) showed an incorrect length of the scalebar. This has been fixed.
 
-RESI (Resolution Enhancement by Sequential Imaging)
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-RESI dialog added to Picasso Render, allowing for substatial boost in spatial resolution (*to be published*).
-
-Photon conversion update
-~~~~~~~~~~~~~~~~~~~~~~~~
-The formula for conversion of raw data to photons was changed, resulting in different numbers of photons and thus **affecting the localization precision** accordingly.
-
-Until version *0.5.7*, the formula was: 
-
-*(RAW_DATA - BASELINE) x SENSITIVITY / (GAIN x QE)*, where QE is quantum efficiency of the camera. 
-
-In Picasso *0.6.0* it was changed to:
-
-*(RAW_DATA - BASELINE) x SENSITIVITY / GAIN*
-
-**i.e., quantum effiency was removed.** Thus, the estimate of the localization precision better approximates the true precision.
-
-
-For backward compatibility, quantum efficiency will be kept in Picasso Localize, however, it will have no effect on the new photon conversion formula.
+Picasso 0.6.0
+-------------
+RESI dialog added to Picasso Render, allowing for substantial boost in spatial resolution (*Reinhardt, et al., Nature, 2023.* DOI: 10.1038/s41586-023-05925-9).
 
 Picasso 0.5.0
 -------------
 Picasso has introduced many changes, including 3D rotation window and a new clustering algorithm in Render and reading of .nd2 files in Localize. Please check the `changelog <https://github.com/jungmannlab/picasso/blob/master/changelog.rst>`_ to see all modifications.
 
 Picasso 0.4.0
 -------------
@@ -173,15 +157,15 @@
 
 Contributions & Copyright
 -------------------------
 
 | Contributors: Joerg Schnitzbauer, Maximilian Strauss, Rafal Kowalewski, Adrian Przybylski, Andrey Aristov, Hiroshi Sasaki, Alexander Auer, Johanna Rahm
 | Copyright (c) 2015-2019 Jungmann Lab, Max Planck Institute of Biochemistry
 | Copyright (c) 2020-2021 Maximilian Strauss
-| Copyright (c) 2022 Rafal Kowalewski
+| Copyright (c) 2022-2023 Rafal Kowalewski
 
 Citing Picasso
 --------------
 
 If you use picasso in your research, please cite our Nature Protocols publication describing the software.
 
 | J. Schnitzbauer*, M.T. Strauss*, T. Schlichthaerle, F. Schueder, R. Jungmann
```

### Comparing `picassosr-0.6.0/picasso/__init__.py` & `picassosr-0.6.1/picasso/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
     :authors: Joerg Schnitzbauer, Maximilian Thomas Strauss, Rafal Kowalewski 2016-2023
     :copyright: Copyright (c) 2016-2018 Jungmann Lab, MPI of Biochemistry
 """
 import os.path as _ospath
 import yaml as _yaml
 
-__version__ = "0.6.0"
+__version__ = "0.6.1"
 
 _this_file = _ospath.abspath(__file__)
 _this_dir = _ospath.dirname(_this_file)
 try:
     with open(_ospath.join(_this_dir, "config.yaml"), "r") as config_file:
         CONFIG = _yaml.full_load(config_file)
     if CONFIG is None:
```

### Comparing `picassosr-0.6.0/picasso/__main__.py` & `picassosr-0.6.1/picasso/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -436,21 +436,20 @@
                 "Generated by": "Picasso Density",
                 "Radius": radius,
             }
             info.append(density_info)
             io.save_locs(base + "_density.hdf5", locs, info)
 
 
-def _dbscan(files, radius, min_density):
+def _dbscan(files, radius, min_density, pixelsize):
     import glob
 
     paths = glob.glob(files)
     if paths:
         from . import io, clusterer
-        pixelsize = int(input("Enter the camera pixelsize in nm: "))
 
         for path in paths:
             print("Loading {} ...".format(path))
             locs, info = io.load_locs(path)
             locs = clusterer.dbscan(locs, radius, min_density, pixelsize)
             clusters = clusterer.find_cluster_centers(locs, pixelsize)
             base, _ = os.path.splitext(path)
@@ -465,21 +464,20 @@
             print(
                 "Clustering executed. Results are saved in: \n"
                 f"{base}_dbscan.hdf5\n"
                 f"{base}_dbclusters.hdf5"
             )
 
 
-def _hdbscan(files, min_cluster, min_samples):
+def _hdbscan(files, min_cluster, min_samples, pixelsize):
     import glob
 
     paths = glob.glob(files)
     if paths:
         from . import io, clusterer
-        pixelsize = int(input("Enter the camera pixelsize in nm: "))
 
         for path in paths:
             print("Loading {} ...".format(path))
             locs, info = io.load_locs(path)
             locs = clusterer.hdbscan(locs, min_cluster, min_samples, pixelsize)
             clusters = clusterer.find_cluster_centers(locs, pixelsize)
             base, ext = os.path.splitext(path)
@@ -493,21 +491,22 @@
             io.save_locs(base + "_hdbclusters.hdf5", clusters, info)
             print(
                 "Clustering executed. Results are saved in: \n"
                 f"{base}_hdbscan.hdf5\n"
                 f"{base}_hdbclusters.hdf5"
             )
 
-def _smlm_clusterer(files, radius, min_locs, basic_fa=False, radius_z=None):
+def _smlm_clusterer(
+        files, radius, min_locs, pixelsize, basic_fa=False, radius_z=None
+    ):
     import glob
 
     paths = glob.glob(files)
     if paths:
         from . import io, clusterer
-        pixelsize = int(input("Enter the camera pixelsize in nm: "))
         if radius_z is not None: # 3D
             params = [radius, radius_z, min_locs, 0, basic_fa, 0]
         else: # 2D
             params = [radius, min_locs, 0, basic_fa, 0]
 
         for path in paths:
             print("Loading {} ...".format(path))
@@ -794,25 +793,25 @@
         Or NDTiffStacks where files have format file.tif, file_1.tif, etc.
         """
         files = glob(filepath + "/*.tif")
         newlist = [_ospath.abspath(file) for file in files]
         for file in files:
             path = _ospath.abspath(file)
             directory = _ospath.dirname(path)
-            if ".ome.tif" in path:
+            if "NDTiffStack" in path:
+                base, ext = _ospath.splitext(path)
+                base = _re.escape(base)
+                pattern = _re.compile(base + r"_(\d*).tif")
+            else:
                 base, ext = _ospath.splitext(
                     _ospath.splitext(path)[0]
                 )  # split two extensions as in .ome.tif
                 base = _re.escape(base)
                 # This matches the basename + an appendix of the file number
                 pattern = _re.compile(base + r"_(\d*).ome.tif")  
-            elif "NDTiffStack" in path:
-                base, ext = _ospath.splitext(path)
-                base = _re.escape(base)
-                pattern = _re.compile(base + r"_(\d*).tif")
             entries = [_.path for _ in _os.scandir(directory) if _.is_file()]
             matches = [_re.match(pattern, _) for _ in entries]
             matches = [_ for _ in matches if _ is not None]
             datafiles = [_.group(0) for _ in matches]
             if datafiles != []:
                 for element in datafiles:
                     newlist.remove(element)
@@ -1273,14 +1272,19 @@
         help=("maximal distance (camera pixels) between to localizations" " to be considered local"),
     )
     dbscan_parser.add_argument(
         "density",
         type=int,
         help=("minimum local density for localizations" " to be assigned to a cluster"),
     )
+    dbscan_parser.add_argument(
+        "pixelsize",
+        type=int,
+        help=("camera pixel size in nm (used for 3D localizations only)"),
+    )
 
     # HDBSCAN
     hdbscan_parser = subparsers.add_parser(
         "hdbscan",
         help="cluster localizations with the hdbscan clustering algorithm",
     )
     hdbscan_parser.add_argument(
@@ -1296,14 +1300,19 @@
         help=("smallest size grouping that is considered a cluster"),
     )
     hdbscan_parser.add_argument(
         "min_samples",
         type=int,
         help=("the higher the more points are considered noise"),
     )
+    hdbscan_parser.add_argument(
+        "pixelsize",
+        type=int,
+        help=("camera pixel size in nm (used for 3D localizations only)"),
+    )
 
     # SMLM clusterer
     smlm_cluster_parser = subparsers.add_parser(
         "smlm_cluster",
         help="cluster localizations with the custom SMLM clustering algorithm",
     )
     smlm_cluster_parser.add_argument(
@@ -1320,14 +1329,19 @@
     )
     smlm_cluster_parser.add_argument(
         "min_locs",
         type=int,
         help=("minimum number of localizations in a cluster"),
     )
     smlm_cluster_parser.add_argument(
+        "pixelsize",
+        type=int,
+        help=("camera pixel size in nm (used for 3D localizations only)"),
+    )
+    smlm_cluster_parser.add_argument(
         "basic_fa",
         type=bool,
         help=("whether or not perform basic frame analysis (sticking event removal)"),
         default=False,
     )
     smlm_cluster_parser.add_argument(
         "radius_z",
@@ -1688,22 +1702,23 @@
                 args.maxval,
             )
         elif args.command == "undrift":
             _undrift(args.files, args.segmentation, args.nodisplay, args.fromfile)
         elif args.command == "density":
             _density(args.files, args.radius)
         elif args.command == "dbscan":
-            _dbscan(args.files, args.radius, args.density)
+            _dbscan(args.files, args.radius, args.density, args.pixelsize)
         elif args.command == "hdbscan":
-            _hdbscan(args.files, args.min_cluster, args.min_samples)
+            _hdbscan(args.files, args.min_cluster, args.min_samples, args.pixelsize)
         elif args.command == "smlm_cluster":
             _smlm_clusterer(
                 args.files,
                 args.radius,
                 args.min_locs,
+                args.pixelsize,
                 args.basic_fa,
                 args.radius_z,
             )
         elif args.command == "nneighbor":
             _nneighbor(args.files)
         elif args.command == "dark":
             _dark(args.files)
```

### Comparing `picassosr-0.6.0/picasso/avgroi.py` & `picassosr-0.6.1/picasso/avgroi.py`

 * *Files identical despite different names*

### Comparing `picassosr-0.6.0/picasso/clusterer.py` & `picassosr-0.6.1/picasso/clusterer.py`

 * *Files identical despite different names*

### Comparing `picassosr-0.6.0/picasso/config_template.yaml` & `picassosr-0.6.1/picasso/config_template.yaml`

 * *Files identical despite different names*

### Comparing `picassosr-0.6.0/picasso/design.py` & `picassosr-0.6.1/picasso/design.py`

 * *Files identical despite different names*

### Comparing `picassosr-0.6.0/picasso/design_sequences.py` & `picassosr-0.6.1/picasso/design_sequences.py`

 * *Files identical despite different names*

### Comparing `picassosr-0.6.0/picasso/ext/bitplane.py` & `picassosr-0.6.1/picasso/ext/bitplane.py`

 * *Files identical despite different names*

### Comparing `picassosr-0.6.0/picasso/gausslq.py` & `picassosr-0.6.1/picasso/gausslq.py`

 * *Files identical despite different names*

### Comparing `picassosr-0.6.0/picasso/gaussmle.py` & `picassosr-0.6.1/picasso/gaussmle.py`

 * *Files identical despite different names*

### Comparing `picassosr-0.6.0/picasso/gui/average.py` & `picassosr-0.6.1/picasso/gui/average.py`

 * *Files identical despite different names*

### Comparing `picassosr-0.6.0/picasso/gui/average3.py` & `picassosr-0.6.1/picasso/gui/average3.py`

 * *Files identical despite different names*

### Comparing `picassosr-0.6.0/picasso/gui/design.py` & `picassosr-0.6.1/picasso/gui/design.py`

 * *Files identical despite different names*

### Comparing `picassosr-0.6.0/picasso/gui/filter.py` & `picassosr-0.6.1/picasso/gui/filter.py`

 * *Files identical despite different names*

### Comparing `picassosr-0.6.0/picasso/gui/icons/average.ico` & `picassosr-0.6.1/picasso/gui/icons/average.ico`

 * *Files identical despite different names*

### Comparing `picassosr-0.6.0/picasso/gui/icons/design.ico` & `picassosr-0.6.1/picasso/gui/icons/design.ico`

 * *Files identical despite different names*

### Comparing `picassosr-0.6.0/picasso/gui/icons/filter.ico` & `picassosr-0.6.1/picasso/gui/icons/filter.ico`

 * *Files identical despite different names*

### Comparing `picassosr-0.6.0/picasso/gui/icons/localize.ico` & `picassosr-0.6.1/picasso/gui/icons/localize.ico`

 * *Files identical despite different names*

### Comparing `picassosr-0.6.0/picasso/gui/icons/nanotron.ico` & `picassosr-0.6.1/picasso/gui/icons/nanotron.ico`

 * *Files identical despite different names*

### Comparing `picassosr-0.6.0/picasso/gui/icons/picasso_server.png` & `picassosr-0.6.1/picasso/gui/icons/picasso_server.png`

 * *Files identical despite different names*

### Comparing `picassosr-0.6.0/picasso/gui/icons/render.ico` & `picassosr-0.6.1/picasso/gui/icons/render.ico`

 * *Files identical despite different names*

### Comparing `picassosr-0.6.0/picasso/gui/icons/server.ico` & `picassosr-0.6.1/picasso/gui/icons/server.ico`

 * *Files identical despite different names*

### Comparing `picassosr-0.6.0/picasso/gui/icons/simulate.ico` & `picassosr-0.6.1/picasso/gui/icons/simulate.ico`

 * *Files identical despite different names*

### Comparing `picassosr-0.6.0/picasso/gui/icons/toraw.ico` & `picassosr-0.6.1/picasso/gui/icons/toraw.ico`

 * *Files identical despite different names*

### Comparing `picassosr-0.6.0/picasso/gui/localize.py` & `picassosr-0.6.1/picasso/gui/localize.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,31 +54,32 @@
         self.window = window
         self.setAcceptDrops(True)
         self.pan = False
         self.hscrollbar = self.horizontalScrollBar()
         self.vscrollbar = self.verticalScrollBar()
         self.rubberband = RubberBand(self)
         self.roi = None
+        self.numeric_roi = False
 
     def mousePressEvent(self, event):
-        if event.button() == QtCore.Qt.LeftButton:
+        if event.button() == QtCore.Qt.LeftButton and not self.numeric_roi:
             self.roi_origin = QtCore.QPoint(event.pos())
             self.rubberband.setGeometry(QtCore.QRect(self.roi_origin, QtCore.QSize()))
             self.rubberband.show()
         elif event.button() == QtCore.Qt.RightButton:
             self.pan = True
             self.pan_start_x = event.x()
             self.pan_start_y = event.y()
             self.setCursor(QtCore.Qt.ClosedHandCursor)
             event.accept()
         else:
             event.ignore()
 
     def mouseMoveEvent(self, event):
-        if event.buttons() == QtCore.Qt.LeftButton:
+        if event.buttons() == QtCore.Qt.LeftButton and not self.numeric_roi:
             self.rubberband.setGeometry(QtCore.QRect(self.roi_origin, event.pos()))
         if self.pan:
             self.hscrollbar.setValue(
                 self.hscrollbar.value() - event.x() + self.pan_start_x
             )
             self.vscrollbar.setValue(
                 self.vscrollbar.value() - event.y() + self.pan_start_y
@@ -86,27 +87,33 @@
             self.pan_start_x = event.x()
             self.pan_start_y = event.y()
             event.accept()
         else:
             event.ignore()
 
     def mouseReleaseEvent(self, event):
-        if event.button() == QtCore.Qt.LeftButton:
+        if event.button() == QtCore.Qt.LeftButton and not self.numeric_roi:
             self.roi_end = QtCore.QPoint(event.pos())
             dx = abs(self.roi_end.x() - self.roi_origin.x())
             dy = abs(self.roi_end.y() - self.roi_origin.y())
             if dx < 10 or dy < 10:
                 self.roi = None
                 self.rubberband.hide()
+                self.window.parameters_dialog.roi_edit.setText("")
             else:
                 roi_points = (
                     self.mapToScene(self.roi_origin),
                     self.mapToScene(self.roi_end),
                 )
-                self.roi = list([[int(_.y()), int(_.x())] for _ in roi_points])
+                self.roi = [[int(_.y()), int(_.x())] for _ in roi_points]
+                (y_min, x_min), (y_max, x_max) = self.roi
+                self.window.parameters_dialog.roi_edit.setText(
+                    f"{y_min},{x_min},{y_max},{x_max}"
+                )
+                self.numeric_roi = False
             self.window.draw_frame()
         elif event.button() == QtCore.Qt.RightButton:
             self.pan = False
             self.setCursor(QtCore.Qt.ArrowCursor)
             event.accept()
         else:
             event.ignore()
@@ -145,16 +152,16 @@
     def dragEnterEvent(self, event):
         if self.drop_has_valid_url(event):
             event.accept()
         else:
             event.ignore()
 
     def dropEvent(self, event):
-        """Loads  when dropped into the scene"""
-        path, extension = self.path_from_drop(event)
+        """Loads when dropped into the scene."""
+        path, ext = self.path_from_drop(event)
         self.window.open(path)
 
 
 class FitMarker(QtWidgets.QGraphicsItemGroup):
     def __init__(self, x, y, size, parent=None):
         super().__init__(parent)
         L = size / 2
@@ -465,28 +472,25 @@
         self.mng_max_spinbox = QtWidgets.QSpinBox()
         self.mng_max_spinbox.setKeyboardTracking(False)
         self.mng_max_spinbox.setRange(0, 999999)
         self.mng_max_spinbox.setValue(10000)
         self.mng_max_spinbox.valueChanged.connect(self.on_mng_max_changed)
         hbox.addWidget(self.mng_max_spinbox)
 
-        # # ROI
-        # identification_grid.addWidget(
-        #     QtWidgets.QLabel("ROI (y_min,x_min,y_max,x_max):"), 4, 0,
-        # )
-        # self.roi_edit = QtWidgets.QLineEdit()
-        # regex = r"\d+,\d+,\d+,\d+" # regex for 4 integers separated by commas
-        # validator = QtGui.QRegExpValidator(QtCore.QRegExp(regex))
-        # self.roi_edit.setValidator(validator)
-        # self.roi_edit.editingFinished.connect(self.on_roi_edit_finished)
-        # identification_grid.addWidget(self.roi_edit, 4, 1)
-        # #TODO: signal when roi_edit is changed: change self.roi and draw rectangle?
-        # #TODO: validate that the input numbers lie within the whole FOV
-        # #TODO: when roi is changed with mouseReleaseEvent in View, change the values displayed here!
-        # #TODO: what about nan?
+        # ROI
+        identification_grid.addWidget(
+            QtWidgets.QLabel("ROI (y_min,x_min,y_max,x_max):"), 5, 0,
+        )
+        self.roi_edit = QtWidgets.QLineEdit()
+        regex = r"\d+,\d+,\d+,\d+" # regex for 4 integers separated by commas
+        validator = QtGui.QRegExpValidator(QtCore.QRegExp(regex))
+        self.roi_edit.setValidator(validator)
+        self.roi_edit.editingFinished.connect(self.on_roi_edit_finished)
+        self.roi_edit.textChanged.connect(self.on_roi_edit_changed)
+        identification_grid.addWidget(self.roi_edit, 5, 1)
 
         self.preview_checkbox = QtWidgets.QCheckBox("Preview")
         self.preview_checkbox.setTristate(False)
         self.preview_checkbox.stateChanged.connect(self.on_preview_changed)
         identification_grid.addWidget(self.preview_checkbox, 4, 0)
         # identification_grid.addWidget(self.preview_checkbox, 5, 0)
 
@@ -666,18 +670,15 @@
         # 3D
         z_groupbox = QtWidgets.QGroupBox("3D via Astigmatism")
         vbox.addWidget(z_groupbox)
 
         z_grid = QtWidgets.QGridLayout(z_groupbox)
         z_grid.addWidget(
             QtWidgets.QLabel("Non-integrated Gaussian fitting is recommend! (LQ)"),
-            0,
-            0,
-            1,
-            2,
+            0, 0, 1, 2,
         )
         load_z_calib = QtWidgets.QPushButton("Load calibration")
         load_z_calib.setAutoDefault(False)
         load_z_calib.clicked.connect(self.load_z_calib)
         z_grid.addWidget(load_z_calib, 1, 1)
         self.fit_z_checkbox = QtWidgets.QCheckBox("Fit Z")
         self.fit_z_checkbox.setEnabled(False)
@@ -763,36 +764,44 @@
 
         self.reset_quality_check()
 
     def reset_quality_check(self):
         self.quality_check.setEnabled(False)
         self.quality_check.setVisible(True)
 
-        for idx, _ in enumerate(self.quality_grid_labels):
+        for _ in self.quality_grid_labels:
             _.setVisible(False)
 
-        for idx, _ in enumerate(self.quality_grid_values):
+        for _ in self.quality_grid_values:
             _.setVisible(False)
             _.setText("")
-    
-    # def on_roi_edit_finished(self):
-    #     from icecream import ic # TODO:delete
-    #     text = self.roi_edit.text().split(",")
-    #     y_min, x_min, y_max, x_max = [int(_) for _ in text]
-    #     # update roi
-    #     self.window.view.roi = [[y_min, x_min], [y_max, x_max]]
-    #     # draw rectangle TODO use self.window.view.rubberband
-    #     self.window.view.rubberband.setGeometry(
-    #         QtCore.QRect(x_min, y_min, x_max-x_min, y_max-y_min)
-    #     )
-    #     self.window.view.rubberband.show()
-    #     #TOOD: incorrect indeces, (wrong place for the box,)
-    #     #TODO: box dispaperast afte rcllicking on View
-    #     #TODO: use map to scene??, idk
-    #     self.window.draw_frame()
+
+    def on_roi_edit_changed(self):
+        if self.roi_edit.text() == "":
+            self.window.view.numeric_roi = False            
+            self.window.view.roi = None
+            self.window.view.rubberband.hide()
+            self.window.draw_frame()
+
+    def on_roi_edit_finished(self):
+        text = self.roi_edit.text().split(",")
+        y_min, x_min, y_max, x_max = [int(_) for _ in text]
+        # update roi
+        self.window.view.roi = [[y_min, x_min], [y_max, x_max]]
+        # draw the rectangle roi
+        topleft_xy = self.window.view.mapFromScene(x_min, y_min)
+        bottomright_xy = self.window.view.mapFromScene(x_max, y_max)
+        topleft = QtCore.QPoint(topleft_xy.x(), topleft_xy.y())
+        bottomright = QtCore.QPoint(bottomright_xy.x(), bottomright_xy.y())
+        self.window.view.rubberband.setGeometry(
+            QtCore.QRect(topleft, bottomright)
+        )
+        self.window.view.rubberband.show()
+        self.window.draw_frame()
+        self.window.view.numeric_roi = True
 
     def on_fit_method_changed(self, state):
         if self.fit_method.currentText() == "LQ, Gaussian":
             self.gpufit_checkbox.setDisabled(False)
         else:
             self.gpufit_checkbox.setChecked(False)
             self.gpufit_checkbox.setDisabled(True)
@@ -1224,17 +1233,17 @@
             dir = self.pwd
 
         path, exe = QtWidgets.QFileDialog.getOpenFileName(
             self, 
             "Open image sequence", 
             directory=dir, 
             filter=(
-                "All supported formats (*.raw *.tif *.tiff *.nd2)"
+                "All supported formats (*.raw *.tif *.tif *.nd2 *.ims)"
                 ";;Raw files (*.raw)"
-                ";;Tiff images (*.tif *.tiff)"
+                ";;Tif images (*.tif)"
                 ";;ImaRIS IMS (*.ims)"
                 ";;Nd2 files (*.nd2);;"
             )
         )
         if path:
             self.pwd = path
             self.open(path)
```

### Comparing `picassosr-0.6.0/picasso/gui/nanotron.py` & `picassosr-0.6.1/picasso/gui/nanotron.py`

 * *Files identical despite different names*

### Comparing `picassosr-0.6.0/picasso/gui/render.py` & `picassosr-0.6.1/picasso/gui/render.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,17 +53,17 @@
     from hdbscan import HDBSCAN
     HDBSCAN_IMPORTED = True
 except ModuleNotFoundError:
     HDBSCAN_IMPORTED = False
 
 if sys.platform == "darwin": # plots do not work on mac os
     matplotlib.use('agg')
-
 matplotlib.rcParams.update({"axes.titlesize": "large"})
 
+
 DEFAULT_OVERSAMPLING = 1.0
 INITIAL_REL_MAXIMUM = 0.5
 ZOOM = 9 / 7
 N_GROUP_COLORS = 8
 N_Z_COLORS = 32
 
 
@@ -83,14 +83,15 @@
         Contains tuples with rgb channels
     """
 
     hues = np.arange(0, 1, 1 / n_channels)
     colors = [colorsys.hsv_to_rgb(_, 1, 1) for _ in hues]
     return colors
 
+
 def get_render_properties_colors(n_channels, cmap='gist_rainbow'):
     """
     Creates a list with rgb channels for each of the channels used in
     rendering property using the gist_rainbow colormap, see:
     https://matplotlib.org/stable/tutorials/colors/colormaps.html
 
     Parameters
@@ -110,14 +111,15 @@
     base = plt.get_cmap(cmap)(np.arange(256))[:, :3]
     # indeces to draw from base
     idx = np.linspace(0, 255, n_channels).astype(int)
     # extract the colors of interest
     colors = base[idx]
     return colors
 
+
 def is_hexadecimal(text):
     """ 
     Checks if text represents a hexadecimal code for rgb, e.g. #ff02d4.
     
     Parameters
     ----------
     text : str
@@ -141,14 +143,15 @@
                 for char in text[1:]:
                     if char in allowed_characters:
                         sum_char += 1
                 if sum_char == 6:
                     return True
     return False
 
+
 def fit_cum_exp(data):
     """ 
     Returns an lmfit Model class fitted to a 3-parameter cumulative
     exponential.
     """
 
     data.sort()
@@ -159,29 +162,32 @@
     params = lmfit.Parameters()
     params.add("a", value=n, vary=True, min=0)
     params.add("t", value=np.mean(data), vary=True, min=data_min, max=data_max)
     params.add("c", value=data_min, vary=True, min=0)
     result = lib.CumulativeExponentialModel.fit(y, params, x=data)
     return result
 
+
 def kinetic_rate_from_fit(data):
     """ Finds the mean dark time from the lmfit fitted Model. """
 
     if len(data) > 2:
         if data.ptp() == 0:
             rate = np.nanmean(data)
         else:
             result = fit_cum_exp(data)
             rate = result.best_values["t"]
     else:
         rate = np.nanmean(data)
     return rate
 
+
 estimate_kinetic_rate = kinetic_rate_from_fit
 
+
 def check_pick(f):
     """ Decorator verifying if there is at least one pick. """
 
     def wrapper(*args):
         if len(args[0]._picks) == 0:
             QtWidgets.QMessageBox.information(
                 args[0],
@@ -189,14 +195,15 @@
                 ("No localizations picked." " Please pick first."),
             )
         else:
             return f(args[0])
 
     return wrapper
 
+
 def check_picks(f):
     """ Decorator verifying if there are at least two picks. """
 
     def wrapper(*args):
         if len(args[0]._picks) < 2:
             QtWidgets.QMessageBox.information(
                 args[0],
@@ -2331,15 +2338,15 @@
                     None,
                 ]
             else:
                 params_c = [
                     params["radius_xy"],
                     params["min_cluster_size"],
                     None,
-                    frame,
+                    params["frame_analysis"],
                     None,
                 ]
 
             locs = clusterer.cluster(locs, params_c, pixelsize)
           
         if len(locs):
             self.view.group_color = self.window.view.get_group_color(locs)
@@ -2749,17 +2756,18 @@
 
         if (
             self.dialog.display_all_locs.isChecked()
             and not self.dialog.display_centers.isChecked()
         ): # two channels, all locs and clustered locs
             channel = self.dialog.channel
             all_locs = self.dialog.window.view.picked_locs(channel)[0]
-            all_locs.z /= (
-                self.dialog.window.display_settings_dlg.pixelsize.value()
-            )
+            if hasattr(all_locs, "z"):
+                all_locs.z /= (
+                    self.dialog.window.display_settings_dlg.pixelsize.value()
+                )
             locs = [
                 all_locs,
                 self.locs,
             ]
         elif (
             not self.dialog.display_all_locs.isChecked()
             and self.dialog.display_centers.isChecked()
@@ -2770,17 +2778,18 @@
             ]
         elif (
             self.dialog.display_all_locs.isChecked()
             and self.dialog.display_centers.isChecked()
         ): # three channels, all locs, clustered locs and cluster centers
             channel = self.dialog.channel
             all_locs = self.dialog.window.view.picked_locs(channel)[0]
-            all_locs.z /= (
-                self.dialog.window.display_settings_dlg.pixelsize.value()
-            )
+            if hasattr(all_locs, "z"):
+                all_locs.z /= (
+                    self.dialog.window.display_settings_dlg.pixelsize.value()
+                )
             locs = [
                 all_locs,
                 self.locs,
                 self.centers,
             ]  
         else:
             # multiple channels, each for one group color
@@ -2985,24 +2994,24 @@
         Updates the scene in the main window and Display section of the
         Info Dialog
     """
 
     def __init__(self, window):
         super().__init__(window)
         self.window = window
-        self.setWindowTitle("Change field of view")
+        self.setWindowTitle("Change FOV")
         self.setModal(False)
         self.layout = QtWidgets.QGridLayout()
         self.setLayout(self.layout)
         self.layout.addWidget(QtWidgets.QLabel("X:"), 0, 0)
         self.x_box = QtWidgets.QDoubleSpinBox()
         self.x_box.setKeyboardTracking(False)
         self.x_box.setRange(-100, 1e6)
         self.layout.addWidget(self.x_box, 0, 1)
-        self.layout.addWidget(QtWidgets.QLabel("Y :"), 1, 0)
+        self.layout.addWidget(QtWidgets.QLabel("Y:"), 1, 0)
         self.y_box = QtWidgets.QDoubleSpinBox()
         self.y_box.setKeyboardTracking(False)
         self.y_box.setRange(-100, 1e6)
         self.layout.addWidget(self.y_box, 1, 1)
         self.layout.addWidget(QtWidgets.QLabel("Width:"), 2, 0)
         self.w_box = QtWidgets.QDoubleSpinBox()
         self.w_box.setKeyboardTracking(False)
@@ -4247,15 +4256,19 @@
             # combine resi cluster centers from all channels
             all_resi = stack_arrays(
                 resi_channels, 
                 asrecarray=True, 
                 usemask=False, 
                 autoconvert=True,
             )
-            # discard group info from resi cluster centers
+            # change the group name in all_resi
+            all_resi = all_resi.astype([
+                ("cluster_id", d[1]) if d[0]=="group" else d
+                for d in all_resi.dtype.descr
+            ])
             all_resi = lib.remove_from_rec(all_resi, "group")
             # sort like all Picasso localization lists
             all_resi.sort(kind="mergesort", order="frame")
 
             # save resi cluster centers
             io.save_locs(resi_path, all_resi, resi_info)
 
@@ -7712,48 +7725,49 @@
                         3, 1, figsize=(5, 5), constrained_layout=True
                     )
                     fig.canvas.set_window_title("Trace")
                     pick = self._picks[i]
                     locs = all_picked_locs[i]
                     locs = stack_arrays(locs, asrecarray=True, usemask=False)
 
-                    # essentialy the same plotting as in self.show_trace
-                    # ax1 = fig.add_subplot(311)
-                    # ax2 = fig.add_subplot(312, sharex=ax1)
-                    # ax3 = fig.add_subplot(313, sharex=ax1)
-
                     xvec = np.arange(n_frames)
-                    yvec = xvec[:] * 0
-                    yvec[locs["frame"]] = 1
+                    yvec = np.ones_like(xvec, dtype=float) * -1
+                    yvec[locs["frame"]] = locs["x"]
                     ax1.set_title(
                         "Scatterplot of Pick "
                         + str(i + 1)
                         + "  of: "
                         + str(len(self._picks))
                         + "."
                     )
                     ax1.set_title(
                         "Scatterplot of Pick "
                         + str(i + 1)
                         + "  of: "
                         + str(len(self._picks))
                         + "."
                     )
-                    ax1.scatter(locs["frame"], locs["x"], s=2)
+                    ax1.scatter(xvec, yvec, s=2)
                     ax1.set_ylabel("X-pos [Px]")
                     ax1.set_title("X-pos vs frame")
-
-                    ax1.set_xlim(0, n_frames)
+                    if locs.size:
+                        ax1.set_ylim(yvec[yvec>0].min(), yvec.max())
                     plt.setp(ax1.get_xticklabels(), visible=False)
 
-                    ax2.scatter(locs["frame"], locs["y"], s=2)
+                    yvec = np.ones_like(xvec, dtype=float) * -1
+                    yvec[locs["frame"]] = locs["y"]
+                    ax2.scatter(xvec, yvec, s=2)
                     ax2.set_title("Y-pos vs frame")
                     ax2.set_ylabel("Y-pos [Px]")
+                    if locs.size:
+                        ax2.set_ylim(yvec[yvec>0].min(), yvec.max())
                     plt.setp(ax2.get_xticklabels(), visible=False)
 
+                    yvec = xvec[:] * 0
+                    yvec[locs["frame"]] = 1
                     ax3.plot(xvec, yvec)
                     ax3.set_title("Localizations")
                     ax3.set_xlabel("Frames")
                     ax3.set_ylabel("ON")
                     ax3.set_yticks([0, 1])
 
                     fig.canvas.draw()
@@ -9098,28 +9112,19 @@
 
         Properties include number of locs, mean and std of all locs
         dtypes (x, y, photons, etc) and others.
         
         Parameters
         ----------
         path : str 
-            Path for saving picks' properties
+            Path for saving picks' properties.
         channel : int
-            Channel of locs to be saved
-
-        Raises
-        ------
-        NotImplementedError
-            If rectangular pick is chosen
+            Channel of locs to be saved.
         """
 
-        if self._pick_shape == "Rectangle":
-            raise NotImplementedError(
-                "Rectangular pick not implemented yet."
-            )
         picked_locs = self.picked_locs(channel)
         pick_diameter = self.window.tools_settings_dialog.pick_diameter.value()
         r_max = min(pick_diameter, 1)
         max_dark = self.window.info_dialog.max_dark_time.value()
         out_locs = []
         progress = lib.ProgressDialog(
             "Calculating kinetics", 0, len(picked_locs), self
@@ -10478,14 +10483,16 @@
     -------
     closeEvent(event)
         Changes user settings and closes all dialogs
     export_complete()
         Exports the whole field of view as .png or .tif
     export_current()
         Exports current view as .png or .tif
+    export_current_info()
+        Exports info about the current view in .yaml file
     export_multi()
         Asks the user to choose a type of export
     export_fov_ims()
         Exports current FOV to .ims
     export_ts()
         Exports locs as .csv for ThunderSTORM
     export_txt()
@@ -10905,17 +10912,62 @@
         except AttributeError:
             return
         out_path = base + ".png"
         path, ext = QtWidgets.QFileDialog.getSaveFileName(
             self, "Save image", out_path, filter="*.png;;*.tif"
         )
         if path:
+            scalebar = self.display_settings_dlg.scalebar_groupbox.isChecked()
+            if not scalebar:
+                self.display_settings_dlg.scalebar_groupbox.setChecked(True)
+                qimage_scale = self.view.draw_scalebar(self.view.qimage)
+                new_path, ext = os.path.splitext(path)
+                new_path = new_path + "_scalebar" + ext
+                qimage_scale.save(new_path)
+                self.display_settings_dlg.scalebar_groupbox.setChecked(False)
             self.view.qimage.save(path)
+            self.export_current_info(path)
         self.view.setMinimumSize(1, 1)
 
+    def export_current_info(self, path):
+        """ Exports information about the current file in .yaml 
+        format. 
+        
+        Parameters
+        ----------
+        path : str
+            Path for saving the original image with .png or .tif
+            extension
+        """
+
+        path, ext = os.path.splitext(path)
+        path = path + ".yaml"
+
+        fov_info = [
+            self.info_dialog.change_fov.x_box.value(),
+            self.info_dialog.change_fov.y_box.value(),
+            self.info_dialog.change_fov.w_box.value(),
+            self.info_dialog.change_fov.h_box.value(),
+        ]
+        d = self.display_settings_dlg
+
+        info = {
+            "FOV (X, Y, Width, Height)": fov_info,
+            "Zoom": d.zoom.value(),
+            "Display Pixel Size (nm)": d.disp_px_size.value(),
+            "Min. Density": d.minimum.value(),
+            "Max. Density": d.maximum.value(),
+            "Colormap": d.colormap.currentText(),
+            "Blur Method": d.blur_methods[d.blur_buttongroup.checkedButton()],
+            "Scalebar Length (nm)": d.scalebar.value(),
+            "Localizations Loaded": self.view.locs_paths,
+        }
+
+        io.save_info(path, [info])
+
     def export_complete(self):
         """ Exports the whole field of view as .png or .tif. """
 
         try:
             base, ext = os.path.splitext(self.view.locs_paths[0])
         except AttributeError:
             return
```

### Comparing `picassosr-0.6.0/picasso/gui/rotation.py` & `picassosr-0.6.1/picasso/gui/rotation.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,29 +9,27 @@
     :author: Rafal Kowalewski, 2021-2022
     :copyright: Copyright (c) 2021 Jungmann Lab, MPI of Biochemistry
 """
 
 import os
 import colorsys
 import re
-from time import sleep
 from functools import partial
 
-import yaml
 import numpy as np
 import matplotlib.pyplot as plt
 from moviepy.video.io.ImageSequenceClip import ImageSequenceClip
 from PyQt5 import QtCore, QtGui, QtWidgets
-from tqdm import tqdm
 
 from numpy.lib.recfunctions import stack_arrays
 
 from .. import io, render
+from ..lib import StatusDialog, ProgressDialog
 
-# from icecream import ic
+# from icecream import ic #TODO: delete
 
 DEFAULT_OVERSAMPLING = 1.0
 INITIAL_REL_MAXIMUM = 0.5
 N_GROUP_COLORS = 8
 SHIFT = 0.1
 ZOOM = 9 / 7
 
@@ -287,16 +285,16 @@
             smooth_button: "smooth",
             convolve_button: "convolve",
             gaussian_button: "gaussian",
             gaussian_iso_button: "gaussian_iso",
         }
 
         # camera
-        self.pixelsize = QtWidgets.QDoubleSpinBox()
-        self.pixelsize.setValue(130)
+        # self.pixelsize = QtWidgets.QDoubleSpinBox()
+        # self.pixelsize.setValue(130)
         
         # scalebar
         self.scalebar_groupbox = QtWidgets.QGroupBox("Scale Bar")
         self.scalebar_groupbox.setCheckable(True)
         self.scalebar_groupbox.setChecked(False)
         self.scalebar_groupbox.toggled.connect(self.render_scene)
         vbox.addWidget(self.scalebar_groupbox)
@@ -650,31 +648,35 @@
             height = self.window.view_rot.height()
             if width % 2 == 1:
                 width += 1
             if height % 2 == 1:
                 height += 1
 
             # create temporary folder to store all frames
-            base, ext = os.path.splitext(self.window.view_rot.paths[0])
-            idx = [i for i, char in enumerate(base) if char == '/'][-1]
-            path = base[:idx] + "/animation_frames"
+            base = os.path.dirname(self.window.view_rot.paths[0])
+            path = os.path.join(base, "animation_frames")
+            progress = ProgressDialog(
+                "Rendering frames", 0, len(angx), self.window
+            )
+            progress.set_value(0)
             try:
                 os.mkdir(path)
                 for i in range(len(angx)):
                     qimage = self.window.view_rot.render_scene(
                         viewport=[(ymin[i], xmin[i]), (ymax[i], xmax[i])],
                         ang=(angx[i], angy[i], angz[i]),
                         animation=True,
                     )
                     qimage = qimage.scaled(
                         width, 
                         height,
                         # QtCore.Qt.KeepAspectRatioByExpanding,
                     )
                     qimage.save(path + "/frame_{}.png".format(i+1))
+                    progress.set_value(i+1)
             except:
                 # if folder exists, ask if it should be used or deleted
                 m = QtWidgets.QMessageBox()
                 m.setWindowTitle("Frames already exist")
                 ret = m.question(
                     self,
                     "",
@@ -690,35 +692,38 @@
                             viewport=[(ymin[i], xmin[i]), (ymax[i], xmax[i])],
                             ang=(angx[i], angy[i], angz[i]),
                             animation=True,
                         )
                         qimage = qimage.scaled(
                             width,
                             height,
-                            QtCore.Qt.KeepAspectRatioByExpanding,
+                            # QtCore.Qt.KeepAspectRatioByExpanding,
                         )
                         qimage.save(path + "/frame_{}.png".format(i+1))
+                        progress.set_value(i+1)
                 elif ret == m.Yes:
                     # use old frames
-                    pass
+                    progress.set_value(len(angx))
                 
             # build a video and save it
+            status = StatusDialog("Creating the video...", self.window)
             image_files = [
                 os.path.join(path, img)
                 for img in os.listdir(path)
                 if img.endswith(".png")
             ] # paths to each frame
             image_files.sort(key=natural_keys) # sort frames
             video = ImageSequenceClip(image_files, fps=self.fps.value())
             video.write_videofile(name)
 
             # delete animation frames
             for file in os.listdir(path):
                 os.remove(os.path.join(path, file))
             os.rmdir(path)
+            status.close()
             
 
 class ViewRotation(QtWidgets.QLabel):
     """
     A class to displayed rotated super-resolution datasets.
 
     Most functions were taken from picass/gui/render.py's View class.
@@ -1169,22 +1174,22 @@
             locs = [
                 locs[self.group_color == _] for _ in range(N_GROUP_COLORS)
             ]
             return self.render_multi_channel(
                 kwargs, locs=locs, ang=ang, autoscale=autoscale
             )
 
-        if ang is None: # if build animation
+        if ang is None: # if not build animation
             n_locs, image = render.render(
                 locs, 
                 **kwargs, 
                 info=self.infos[0], 
                 ang=(self.angx, self.angy, self.angz), 
             )
-        else: # if not build animation
+        else: # if build animation
             n_locs, image = render.render(
                 locs, 
                 **kwargs, 
                 info=self.infos[0], 
                 ang=ang, 
             )
         self.n_locs = n_locs
@@ -1253,21 +1258,18 @@
         self.qimage = qimage.scaled(
             self.width(),
             self.height(),
             QtCore.Qt.KeepAspectRatioByExpanding,
         )
         # draw scalebar, legend, rotation and measuring points
         self.qimage = self.draw_scalebar(self.qimage)
-        if self.display_legend:
-            self.qimage = self.draw_legend(self.qimage)
-        if self.display_rotation:
-            self.qimage = self.draw_rotation(self.qimage)
-        if self.display_angles:
-            self.qimage = self.draw_rotation_angles(self.qimage)
-        self.qimage = self.draw_points(self.qimage)
+        self.qimage = self.draw_legend(self.qimage)
+        self.qimage = self.draw_rotation(self.qimage)
+        self.qimage = self.draw_rotation_angles(self.qimage)
+        self.qimage = self.draw_points(self.qimage)        
 
         # convert to pixmap
         self.pixmap = QtGui.QPixmap.fromImage(self.qimage)
         self.setPixmap(self.pixmap)
 
     def draw_scalebar(self, image):
         """
@@ -1281,21 +1283,20 @@
         Returns
         -------
         QImage
             Image with the drawn scalebar        
         """
 
         if self.window.display_settings_dlg.scalebar_groupbox.isChecked():
-            pixelsize = self.window.display_settings_dlg.pixelsize.value()
+            pixelsize = self.window.window.display_settings_dlg.pixelsize.value()
             scalebar = self.window.display_settings_dlg.scalebar.value()
             length_camerapxl = scalebar / pixelsize
             length_displaypxl = int(
                 round(self.width() * length_camerapxl / self.viewport_width())
             )
-            # height = max(int(round(0.15 * length_displaypxl)), 1)
             height = 10
             painter = QtGui.QPainter(image)
             painter.setPen(QtGui.QPen(QtCore.Qt.NoPen))
             painter.setBrush(QtGui.QBrush(QtGui.QColor("white")))
             if self.window.dataset_dialog.wbackground.isChecked():
                 painter.setBrush(QtGui.QBrush(QtGui.QColor("black")))
             x = self.width() - length_displaypxl - 35
@@ -1334,30 +1335,31 @@
 
         Returns
         -------
         QImage
             Image with the drawn legend
         """
 
-        n_channels = len(self.locs)
-        painter = QtGui.QPainter(image)
-        x = 12
-        y = 20
-        dy = 20
-        for i in range(n_channels):
-            if self.window.dataset_dialog.checks[i].isChecked():
-                palette = self.window.dataset_dialog.colordisp_all[i].palette()
-                color = palette.color(QtGui.QPalette.Window)
-                painter.setPen(QtGui.QColor(color))
-                font = painter.font()
-                font.setPixelSize(12)
-                painter.setFont(font)
-                text = self.window.dataset_dialog.checks[i].text()
-                painter.drawText(QtCore.QPoint(x, y), text)
-                y += dy
+        if self.display_legend:
+            n_channels = len(self.locs)
+            painter = QtGui.QPainter(image)
+            x = 12
+            y = 20
+            dy = 20
+            for i in range(n_channels):
+                if self.window.dataset_dialog.checks[i].isChecked():
+                    palette = self.window.dataset_dialog.colordisp_all[i].palette()
+                    color = palette.color(QtGui.QPalette.Window)
+                    painter.setPen(QtGui.QColor(color))
+                    font = painter.font()
+                    font.setPixelSize(12)
+                    painter.setFont(font)
+                    text = self.window.dataset_dialog.checks[i].text()
+                    painter.drawText(QtCore.QPoint(x, y), text)
+                    y += dy
         return image
 
     def draw_rotation(self, image):
         """
         Draws a small 3 axes icon that rotates with locs.
 
         Displayed in the bottom left corner.
@@ -1369,91 +1371,92 @@
 
         Returns
         -------
         QImage
             Image with the drawn legend
         """
 
-        painter = QtGui.QPainter(image)
-        length = 30
-        width = 2
-        x = 50
-        y = self.height() - 50
-        center = QtCore.QPoint(x, y)
-
-        #set the ends of the x line
-        xx = length
-        xy = 0
-        xz = 0
-
-        #set the ends of the y line
-        yx = 0
-        yy = length
-        yz = 0
-
-        #set the ends of the z line
-        zx = 0
-        zy = 0
-        zz = length
-
-        #rotate these points
-        coordinates = [[xx, xy, xz], [yx, yy, yz], [zx, zy, zz]]
-        R = render.rotation_matrix(self.angx, self.angy, self.angz)
-        coordinates = R.apply(coordinates)
-        (xx, xy, xz) = coordinates[0]
-        (yx, yy, yz) = coordinates[1]
-        (zx, zy, zz) = coordinates[2]
-
-        # translate the x and y coordinates of the end points towards 
-        # bottom right edge of the window
-        xx += x
-        xy += y
-        yx += x
-        yy += y
-        zx += x
-        zy += y
-
-        #set the points at the ends of the lines
-        point_x = QtCore.QPoint(xx, xy)
-        point_y = QtCore.QPoint(yx, yy)
-        point_z = QtCore.QPoint(zx, zy)
-        line_x = QtCore.QLine(center, point_x)
-        line_y = QtCore.QLine(center, point_y)
-        line_z = QtCore.QLine(center, point_z)
-        painter.setPen(QtGui.QPen(QtGui.QColor.fromRgbF(1, 0, 0, 1)))
-        painter.drawLine(line_x)
-        painter.setPen(QtGui.QPen(QtGui.QColor.fromRgbF(0, 1, 1, 1)))
-        painter.drawLine(line_y)
-        painter.setPen(QtGui.QPen(QtGui.QColor.fromRgbF(0, 1, 0, 1)))
-        painter.drawLine(line_z)
+        if self.display_rotation:
+            painter = QtGui.QPainter(image)
+            length = 30
+            width = 2
+            x = 50
+            y = self.height() - 50
+            center = QtCore.QPoint(x, y)
+
+            #set the ends of the x line
+            xx = length
+            xy = 0
+            xz = 0
+
+            #set the ends of the y line
+            yx = 0
+            yy = length
+            yz = 0
+
+            #set the ends of the z line
+            zx = 0
+            zy = 0
+            zz = length
+
+            #rotate these points
+            coordinates = [[xx, xy, xz], [yx, yy, yz], [zx, zy, zz]]
+            R = render.rotation_matrix(self.angx, self.angy, self.angz)
+            coordinates = R.apply(coordinates)
+            (xx, xy, xz) = coordinates[0]
+            (yx, yy, yz) = coordinates[1]
+            (zx, zy, zz) = coordinates[2]
+
+            # translate the x and y coordinates of the end points towards 
+            # bottom right edge of the window
+            xx += x
+            xy += y
+            yx += x
+            yy += y
+            zx += x
+            zy += y
+
+            #set the points at the ends of the lines
+            point_x = QtCore.QPoint(xx, xy)
+            point_y = QtCore.QPoint(yx, yy)
+            point_z = QtCore.QPoint(zx, zy)
+            line_x = QtCore.QLine(center, point_x)
+            line_y = QtCore.QLine(center, point_y)
+            line_z = QtCore.QLine(center, point_z)
+            painter.setPen(QtGui.QPen(QtGui.QColor.fromRgbF(1, 0, 0, 1)))
+            painter.drawLine(line_x)
+            painter.setPen(QtGui.QPen(QtGui.QColor.fromRgbF(0, 1, 1, 1)))
+            painter.drawLine(line_y)
+            painter.setPen(QtGui.QPen(QtGui.QColor.fromRgbF(0, 1, 0, 1)))
+            painter.drawLine(line_z)
         return image
 
     def draw_rotation_angles(self, image):
         """ 
         Draws text displaying current rotation angles in degrees. 
         """
-        
-        image = image.copy()
-        [angx, angy, angz] = [
-            int(np.round(_ * 180 / np.pi, 0)) 
-            for _ in [self.angx, self.angy, self.angz]
-        ]
-        text = f"{angx} {angy} {angz}"
-        x = self.width() - len(text) * 7.5 - 10
-        y = self.height() - 20      
-        painter = QtGui.QPainter(image)
-        font = painter.font()
-        font.setPixelSize(12)
-        painter.setFont(font)
-        painter.setPen(QtGui.QColor("white"))
-        if self.window.dataset_dialog.wbackground.isChecked():
-            painter.setPen(QtGui.QColor("black"))
-        painter.drawText(QtCore.QPoint(x, y), text)
-        return image
 
+        if self.display_angles:        
+            image = image.copy()
+            [angx, angy, angz] = [
+                int(np.round(_ * 180 / np.pi, 0)) 
+                for _ in [self.angx, self.angy, self.angz]
+            ]
+            text = f"{angx} {angy} {angz}"
+            x = self.width() - len(text) * 7.5 - 10
+            y = self.height() - 20      
+            painter = QtGui.QPainter(image)
+            font = painter.font()
+            font.setPixelSize(12)
+            painter.setFont(font)
+            painter.setPen(QtGui.QColor("white"))
+            if self.window.dataset_dialog.wbackground.isChecked():
+                painter.setPen(QtGui.QColor("black"))
+            painter.drawText(QtCore.QPoint(x, y), text)
+        return image
 
     def draw_points(self, image):
         """
         Draws points and lines and distances between them onto image.
         
         Parameters
         ----------
@@ -1473,15 +1476,15 @@
         if self.window.dataset_dialog.wbackground.isChecked():
             painter.setPen(QtGui.QColor("red"))
         cx = []
         cy = []
         ox = []
         oy = []
         oldpoint = []
-        pixelsize = self.window.display_settings_dlg.pixelsize.value()
+        pixelsize = self.window.window.display_settings_dlg.pixelsize.value()
         for point in self._points:
             if oldpoint != []:
                 ox, oy = self.map_to_view(*oldpoint)
             cx, cy = self.map_to_view(*point)
             painter.drawPoint(cx, cy)
             painter.drawLine(cx, cy, cx + d / 2, cy)
             painter.drawLine(cx, cy, cx, cy + d / 2)
@@ -2452,15 +2455,15 @@
                     self,
                     "Input Dialog",
                     "Enter suffix",
                     QtWidgets.QLineEdit.Normal,
                     f"_arotated_{angx}_{angy}_{angz}",
                 ) # get the save file suffix
                 if ok:
-                    for channel in tqdm(range(len(self.view_rot.paths))):
+                    for channel in range(len(self.view_rot.paths)):
                         base, ext = os.path.splitext(
                             self.view_rot.paths[channel]
                         )
                         out_path = base + suffix + ".hdf5"
                         info = self.view_rot.infos[channel] + new_info
                         io.save_locs(
                             out_path, self.window.view.all_locs[channel], info
```

### Comparing `picassosr-0.6.0/picasso/gui/simulate.py` & `picassosr-0.6.1/picasso/gui/simulate.py`

 * *Files identical despite different names*

### Comparing `picassosr-0.6.0/picasso/gui/toraw.py` & `picassosr-0.6.1/picasso/gui/toraw.py`

 * *Files identical despite different names*

### Comparing `picassosr-0.6.0/picasso/imageprocess.py` & `picassosr-0.6.1/picasso/imageprocess.py`

 * *Files identical despite different names*

### Comparing `picassosr-0.6.0/picasso/io.py` & `picassosr-0.6.1/picasso/io.py`

 * *Files 0% similar despite different names*

```diff
@@ -951,24 +951,24 @@
     def __init__(self, path, memmap_frames=False, verbose=False):
         super().__init__()
         self.path = _ospath.abspath(path)
         self.dir = _ospath.dirname(self.path)
         
         # This matches the basename + an appendix of the file number
         filename = _ospath.basename(self.path)
-        if ".ome." in filename: 
-            # split two extensions as in .ome.tif
-            base, ext = _ospath.splitext(_ospath.splitext(self.path)[0])  
-            base = _re.escape(base)
-            pattern = _re.compile(base + r"_(\d*).ome.tif")
-        elif "NDTiffStack" in filename:
+        if "NDTiffStack" in filename: 
             # only one extension (.tif)
             base, ext = _ospath.splitext(self.path)  
             base = _re.escape(base)
             pattern = _re.compile(base + r"_(\d*).tif")
+        else:
+            # split two extensions as in .ome.tif
+            base, ext = _ospath.splitext(_ospath.splitext(self.path)[0])  
+            base = _re.escape(base)
+            pattern = _re.compile(base + r"_(\d*).ome.tif")
         entries = [_.path for _ in _os.scandir(self.dir) if _.is_file()]
         matches = [_re.match(pattern, _) for _ in entries]
         matches = [_ for _ in matches if _ is not None]
         paths_indices = [(int(_.group(1)), _.group(0)) for _ in matches]
         self.paths = [self.path] + [path for index, path in sorted(paths_indices)]
         self.maps = [TiffMap(path, verbose=verbose) for path in self.paths]
         self.n_maps = len(self.maps)
```

### Comparing `picassosr-0.6.0/picasso/lib.py` & `picassosr-0.6.1/picasso/lib.py`

 * *Files identical despite different names*

### Comparing `picassosr-0.6.0/picasso/localize.py` & `picassosr-0.6.1/picasso/localize.py`

 * *Files identical despite different names*

### Comparing `picassosr-0.6.0/picasso/nanotron.py` & `picassosr-0.6.1/picasso/nanotron.py`

 * *Files identical despite different names*

### Comparing `picassosr-0.6.0/picasso/postprocess.py` & `picassosr-0.6.1/picasso/postprocess.py`

 * *Files identical despite different names*

### Comparing `picassosr-0.6.0/picasso/render.py` & `picassosr-0.6.1/picasso/render.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,18 +11,19 @@
 import os
 import sys
 
 import numpy as _np
 import numba as _numba
 import scipy.signal as _signal
 from scipy.spatial.transform import Rotation as _Rotation
-# from icecream import ic
+
 
 _DRAW_MAX_SIGMA = 3
 
+
 def render(
     locs,
     info=None,
     oversampling=1,
     viewport=None,
     blur_method=None,
     min_blur_width=0,
@@ -115,14 +116,15 @@
             y_min, x_min, y_max, x_max, 
             min_blur_width, 
             ang=ang, 
         )
     else:
         raise Exception("blur_method not understood.")
 
+
 @_numba.njit
 def _render_setup(
     locs, 
     oversampling, 
     y_min, x_min, y_max, x_max,
 ):
     """
@@ -167,14 +169,15 @@
     x = x[in_view]
     y = y[in_view]
     x = oversampling * (x - x_min)
     y = oversampling * (y - y_min)
     image = _np.zeros((n_pixel_y, n_pixel_x), dtype=_np.float32)
     return image, n_pixel_y, n_pixel_x, x, y, in_view
 
+
 @_numba.njit
 def _render_setup3d(
     locs, 
     oversampling, 
     y_min, x_min, y_max, x_max, z_min, z_max, 
     pixelsize,
 ):
@@ -258,14 +261,15 @@
 #     x = x[in_view]
 #     z = z[in_view]
 #     x = oversampling * (x - x_min)
 #     z = oversampling * (z - z_min)
 #     image = _np.zeros((n_pixel_x, n_pixel_z), dtype=_np.float32)
 #     return image, n_pixel_z, n_pixel_x, x, z, in_view
 
+
 @_numba.njit
 def _fill(image, x, y):
     """
     Fills image with x and y coordinates. 
     Image is not blurred.
 
     Parameters
@@ -279,14 +283,15 @@
     """
 
     x = x.astype(_np.int32)
     y = y.astype(_np.int32)
     for i, j in zip(x, y):
         image[j, i] += 1
 
+
 @_numba.njit
 def _fill3d(image, x, y, z):
     """
     Fills image with x, y and z coordinates.
     Image is not blurred.
     Used by Picasso: Average3.
 
@@ -305,14 +310,15 @@
     x = x.astype(_np.int32)
     y = y.astype(_np.int32)
     z = z.astype(_np.int32)
     z += _np.min(z) # because z takes also negative values
     for i, j, k in zip(x, y, z):
         image[j, i, k] += 1
 
+
 @_numba.njit
 def _fill_gaussian(image, x, y, sx, sy, n_pixel_x, n_pixel_y):
     """
     Fills image with blurred x and y coordinates.
     Localization precisions (sx and sy) are treated as standard
     deviations of the guassians to be rendered.
 
@@ -359,14 +365,15 @@
                 image[i, j] += _np.exp(
                     -(
                         (j - x_ + 0.5) ** 2 / (2 * sx_**2)
                         + (i - y_ + 0.5) ** 2 / (2 * sy_**2)
                     )
                 ) / (2 * _np.pi * sx_ * sy_)
 
+
 @_numba.njit
 def _fill_gaussian_rot(
     image, x, y, z, sx, sy, sz, n_pixel_x, n_pixel_y, ang
 ):
     """
     Fills image with rotated gaussian-blurred localizations.
 
@@ -479,14 +486,15 @@
                         + a*c * cri[2,0] + b*c * cri[2,1] + c*c * cri[2,2]
                     ) # Mahalanobis distance
                     image[i,j] += (
                         _np.exp(-0.5 * exponent)
                         / (((2*_np.pi) ** 3 * dcr) ** 0.5)
                     )
 
+
 @_numba.njit
 def inverse_3x3(a):
     """
     Calculates inverse of a 3x3 matrix.
 
     This function is faster than np.linalg.inv.
 
@@ -514,14 +522,15 @@
 
     c[2,0] = (a[1,0] * a[2,1] - a[1,1] * a[2,0]) / det
     c[2,1] = (a[0,1] * a[2,0] - a[0,0] * a[2,1]) / det
     c[2,2] = (a[0,0] * a[1,1] - a[0,1] * a[1,0]) / det
 
     return c    
 
+
 @_numba.njit
 def determinant_3x3(a):
     """
     Calculates determinant of a 3x3 matrix.
 
     This function is faster than np.linalg.det.
 
@@ -538,14 +547,15 @@
 
     return _np.float32(
         a[0,0] * (a[1,1] * a[2,2] - a[1,2] * a[2,1]) 
         - a[0,1] * (a[1,0] * a[2,2] - a[2,0] * a[1,2]) 
         + a[0,2] * (a[1,0] * a[2,1] - a[2,0] * a[1,1])
     )
 
+
 def render_hist(
     locs, 
     oversampling, 
     y_min, x_min, y_max, x_max, 
     ang=None, 
 ):
     """
@@ -588,22 +598,24 @@
             oversampling,
             x_min, x_max, y_min, y_max, 
             ang, 
         )
     _fill(image, x, y)
     return len(x), image
 
+
 # @_numba.jit(nopython=True, nogil=True)
 # def render_histz(locs, oversampling, x_min, z_min, x_max, z_max):
 #     image, n_pixel_z, n_pixel_x, x, z, in_view = _render_setupz(
 #         locs, oversampling, x_min, z_min, x_max, z_max
 #     )
 #     _fill(image, z, x)
 #     return len(x), image
 
+
 @_numba.jit(nopython=True, nogil=True)
 def render_hist3d(
     locs, 
     oversampling, 
     y_min, x_min, y_max, x_max, z_min, z_max, 
     pixelsize,
 ):
@@ -648,14 +660,15 @@
         oversampling, 
         y_min, x_min, y_max, x_max, z_min, z_max, 
         pixelsize,
     )
     _fill3d(image, x, y, z)
     return len(x), image
 
+
 def render_gaussian(
     locs, 
     oversampling, 
     y_min, x_min, y_max, x_max, 
     min_blur_width, 
     ang=None, 
 ):
@@ -727,14 +740,15 @@
 
         _fill_gaussian_rot(
             image, x, y, z, sx, sy, sz, n_pixel_x, n_pixel_y, ang
         )
 
     return len(x), image
 
+
 def render_gaussian_iso(
     locs, 
     oversampling, 
     y_min, x_min, y_max, x_max, 
     min_blur_width, 
     ang=None, 
 ):
@@ -806,14 +820,15 @@
 
         _fill_gaussian_rot(
             image, x, y, z, sx, sy, sz, n_pixel_x, n_pixel_y, ang
         )
 
     return len(x), image
 
+
 def render_convolve(
     locs, 
     oversampling, 
     y_min, x_min, y_max, x_max, 
     min_blur_width, 
     ang=None, 
 ):
@@ -872,14 +887,15 @@
             _np.median(locs.lpx[in_view]), min_blur_width
         )
         blur_height = oversampling * max(
             _np.median(locs.lpy[in_view]), min_blur_width
         )
         return n, _fftconvolve(image, blur_width, blur_height)
 
+
 def render_smooth(
     locs, 
     oversampling, 
     y_min, x_min, y_max, x_max, 
     ang=None, 
 ):
     """
@@ -929,14 +945,15 @@
     n = len(x)
     if n == 0:
         return 0, image
     else:
         _fill(image, x, y)
         return n, _fftconvolve(image, 1, 1)
 
+
 def _fftconvolve(image, blur_width, blur_height): 
     """
     Blurs (convolves) 2D image using fast fourier transform.
 
     Parameters
     ----------
     image : np.array
@@ -956,14 +973,15 @@
     kernel_height = 10 * int(_np.round(blur_height)) + 1
     kernel_y = _signal.gaussian(kernel_height, blur_height)
     kernel_x = _signal.gaussian(kernel_width, blur_width)
     kernel = _np.outer(kernel_y, kernel_x)
     kernel /= kernel.sum()
     return _signal.fftconvolve(image, kernel, mode="same")
 
+
 def rotation_matrix(angx, angy, angz):
     """
     Finds rotation matrix given rotation angles around axes.
 
     Parameters
     ----------
     angx : float
@@ -999,14 +1017,15 @@
             [_np.sin(angz), _np.cos(angz), 0.0],
             [0.0, 0.0, 1.0],
         ]
     ) # rotation matrix around z axis
     rot_mat = rot_mat_x @ rot_mat_y @ rot_mat_z
     return _Rotation.from_matrix(rot_mat)
 
+
 def locs_rotation(
     locs, 
     oversampling,
     x_min, x_max, y_min, y_max, 
     ang, 
 ):
     """
```

### Comparing `picassosr-0.6.0/picasso/server/app.py` & `picassosr-0.6.1/picasso/server/app.py`

 * *Files identical despite different names*

### Comparing `picassosr-0.6.0/picasso/server/compare.py` & `picassosr-0.6.1/picasso/server/compare.py`

 * *Files identical despite different names*

### Comparing `picassosr-0.6.0/picasso/server/helper.py` & `picassosr-0.6.1/picasso/server/helper.py`

 * *Files identical despite different names*

### Comparing `picassosr-0.6.0/picasso/server/history.py` & `picassosr-0.6.1/picasso/server/history.py`

 * *Files identical despite different names*

### Comparing `picassosr-0.6.0/picasso/server/preview.py` & `picassosr-0.6.1/picasso/server/preview.py`

 * *Files identical despite different names*

### Comparing `picassosr-0.6.0/picasso/server/status.py` & `picassosr-0.6.1/picasso/server/status.py`

 * *Files identical despite different names*

### Comparing `picassosr-0.6.0/picasso/server/watcher.py` & `picassosr-0.6.1/picasso/server/watcher.py`

 * *Files identical despite different names*

### Comparing `picassosr-0.6.0/picasso/simulate.py` & `picassosr-0.6.1/picasso/simulate.py`

 * *Files identical despite different names*

### Comparing `picassosr-0.6.0/picasso/zfit.py` & `picassosr-0.6.1/picasso/zfit.py`

 * *Files identical despite different names*

### Comparing `picassosr-0.6.0/picassosr.egg-info/PKG-INFO` & `picassosr-0.6.1/picassosr.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: picassosr
-Version: 0.6.0
+Version: 0.6.1
 Home-page: https://github.com/jungmannlab/picasso
 Author: Joerg Schnitzbauer, Maximilian T. Strauss, Rafal Kowalewski
 Author-email: joschnitzbauer@gmail.com, straussmaximilian@gmail.com, rafalkowalewski998@gmail.com
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -32,37 +32,21 @@
    :scale: 100 %
    :alt: UML Render view
 
 A collection of tools for painting super-resolution images. The Picasso software is complemented by our `Nature Protocols publication <https://www.nature.com/nprot/journal/v12/n6/abs/nprot.2017.024.html>`__.
 A comprehensive documentation can be found here: `Read the Docs <https://picassosr.readthedocs.io/en/latest/?badge=latest>`__.
 
 
-Picasso 0.6.0
+Picasso 0.6.1
 -------------
+In previous version, the rotation window (3D Render) showed an incorrect length of the scalebar. This has been fixed.
 
-RESI (Resolution Enhancement by Sequential Imaging)
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-RESI dialog added to Picasso Render, allowing for substatial boost in spatial resolution (*to be published*).
-
-Photon conversion update
-~~~~~~~~~~~~~~~~~~~~~~~~
-The formula for conversion of raw data to photons was changed, resulting in different numbers of photons and thus **affecting the localization precision** accordingly.
-
-Until version *0.5.7*, the formula was: 
-
-*(RAW_DATA - BASELINE) x SENSITIVITY / (GAIN x QE)*, where QE is quantum efficiency of the camera. 
-
-In Picasso *0.6.0* it was changed to:
-
-*(RAW_DATA - BASELINE) x SENSITIVITY / GAIN*
-
-**i.e., quantum effiency was removed.** Thus, the estimate of the localization precision better approximates the true precision.
-
-
-For backward compatibility, quantum efficiency will be kept in Picasso Localize, however, it will have no effect on the new photon conversion formula.
+Picasso 0.6.0
+-------------
+RESI dialog added to Picasso Render, allowing for substantial boost in spatial resolution (*Reinhardt, et al., Nature, 2023.* DOI: 10.1038/s41586-023-05925-9).
 
 Picasso 0.5.0
 -------------
 Picasso has introduced many changes, including 3D rotation window and a new clustering algorithm in Render and reading of .nd2 files in Localize. Please check the `changelog <https://github.com/jungmannlab/picasso/blob/master/changelog.rst>`_ to see all modifications.
 
 Picasso 0.4.0
 -------------
@@ -173,15 +157,15 @@
 
 Contributions & Copyright
 -------------------------
 
 | Contributors: Joerg Schnitzbauer, Maximilian Strauss, Rafal Kowalewski, Adrian Przybylski, Andrey Aristov, Hiroshi Sasaki, Alexander Auer, Johanna Rahm
 | Copyright (c) 2015-2019 Jungmann Lab, Max Planck Institute of Biochemistry
 | Copyright (c) 2020-2021 Maximilian Strauss
-| Copyright (c) 2022 Rafal Kowalewski
+| Copyright (c) 2022-2023 Rafal Kowalewski
 
 Citing Picasso
 --------------
 
 If you use picasso in your research, please cite our Nature Protocols publication describing the software.
 
 | J. Schnitzbauer*, M.T. Strauss*, T. Schlichthaerle, F. Schueder, R. Jungmann
```

### Comparing `picassosr-0.6.0/picassosr.egg-info/SOURCES.txt` & `picassosr-0.6.1/picassosr.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `picassosr-0.6.0/setup.py` & `picassosr-0.6.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     requirements = [line for line in requirements_file]
 
 with open("readme.rst", encoding="utf-8") as readme_file:
     long_description = readme_file.read()
 
 setup(
     name="picassosr",
-    version="0.6.0",
+    version="0.6.1",
     author="Joerg Schnitzbauer, Maximilian T. Strauss, Rafal Kowalewski",
     author_email=("joschnitzbauer@gmail.com, straussmaximilian@gmail.com, rafalkowalewski998@gmail.com"),
     url="https://github.com/jungmannlab/picasso",
     long_description=long_description,
     long_description_content_type="text/x-rst",
     packages=["picasso", "picasso.gui", "picasso.gui.plugins", "picasso.server", "picasso.ext"],
     entry_points={
```

