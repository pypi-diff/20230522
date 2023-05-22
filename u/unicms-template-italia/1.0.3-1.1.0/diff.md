# Comparing `tmp/unicms_template_italia-1.0.3.tar.gz` & `tmp/unicms_template_italia-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unicms_template_italia-1.0.3.tar", last modified: Wed Dec  7 15:30:25 2022, max compression
+gzip compressed data, was "unicms_template_italia-1.1.0.tar", last modified: Mon May 22 07:34:21 2023, max compression
```

## Comparing `unicms_template_italia-1.0.3.tar` & `unicms_template_italia-1.1.0.tar`

### file list

```diff
@@ -1,70 +1,71 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-07 15:30:25.293712 unicms_template_italia-1.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2022-12-07 15:30:14.000000 unicms_template_italia-1.0.3/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2022-12-07 15:30:14.000000 unicms_template_italia-1.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      954 2022-12-07 15:30:25.293712 unicms_template_italia-1.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      123 2022-12-07 15:30:14.000000 unicms_template_italia-1.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-07 15:30:25.293712 unicms_template_italia-1.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1689 2022-12-07 15:30:14.000000 unicms_template_italia-1.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-07 15:30:25.281711 unicms_template_italia-1.0.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-07 15:30:25.285711 unicms_template_italia-1.0.3/src/unicms_template_italia/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-07 15:30:14.000000 unicms_template_italia-1.0.3/src/unicms_template_italia/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      117 2022-12-07 15:30:14.000000 unicms_template_italia-1.0.3/src/unicms_template_italia/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-07 15:30:25.281711 unicms_template_italia-1.0.3/src/unicms_template_italia/locale/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-07 15:30:25.281711 unicms_template_italia-1.0.3/src/unicms_template_italia/locale/it/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-07 15:30:25.285711 unicms_template_italia-1.0.3/src/unicms_template_italia/locale/it/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1400 2022-12-07 15:30:14.000000 unicms_template_italia-1.0.3/src/unicms_template_italia/locale/it/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)     9747 2022-12-07 15:30:14.000000 unicms_template_italia-1.0.3/src/unicms_template_italia/locale/it/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (123)     9468 2022-12-07 15:30:14.000000 unicms_template_italia-1.0.3/src/unicms_template_italia/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-07 15:30:25.281711 unicms_template_italia-1.0.3/src/unicms_template_italia/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-07 15:30:25.281711 unicms_template_italia-1.0.3/src/unicms_template_italia/static/css/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-07 15:30:25.285711 unicms_template_italia-1.0.3/src/unicms_template_italia/static/css/vendor/
--rw-r--r--   0 runner    (1001) docker     (123)     3658 2022-12-07 15:30:14.000000 unicms_template_italia-1.0.3/src/unicms_template_italia/static/css/vendor/owl.carousel.min.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-07 15:30:25.285711 unicms_template_italia-1.0.3/src/unicms_template_italia/static/js/
--rw-r--r--   0 runner    (1001) docker     (123)    26730 2022-12-07 15:30:14.000000 unicms_template_italia-1.0.3/src/unicms_template_italia/static/js/axios.1.1.3.js
--rw-r--r--   0 runner    (1001) docker     (123)   125861 2022-12-07 15:30:14.000000 unicms_template_italia-1.0.3/src/unicms_template_italia/static/js/axios.min.js.map
--rw-r--r--   0 runner    (1001) docker     (123)      298 2022-12-07 15:30:14.000000 unicms_template_italia-1.0.3/src/unicms_template_italia/static/js/deferred_iframe_src.js
--rw-r--r--   0 runner    (1001) docker     (123)      666 2022-12-07 15:30:14.000000 unicms_template_italia-1.0.3/src/unicms_template_italia/static/js/passive_listeners.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-07 15:30:25.285711 unicms_template_italia-1.0.3/src/unicms_template_italia/static/js/vendor/
--rw-r--r--   0 runner    (1001) docker     (123)    44342 2022-12-07 15:30:14.000000 unicms_template_italia-1.0.3/src/unicms_template_italia/static/js/vendor/owl.carousel.min.js
--rw-r--r--   0 runner    (1001) docker     (123)   107216 2022-12-07 15:30:14.000000 unicms_template_italia-1.0.3/src/unicms_template_italia/static/js/vue.2.7.14.js
--rw-r--r--   0 runner    (1001) docker     (123)      875 2022-12-07 15:30:14.000000 unicms_template_italia-1.0.3/src/unicms_template_italia/static/js/vue.options.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-07 15:30:25.285711 unicms_template_italia-1.0.3/src/unicms_template_italia/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-07 15:30:25.285711 unicms_template_italia-1.0.3/src/unicms_template_italia/templates/bases/
--rw-r--r--   0 runner    (1001) docker     (123)    89706 2022-12-07 15:30:14.000000 unicms_template_italia-1.0.3/src/unicms_template_italia/templates/bases/unicms_italia.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-07 15:30:25.289712 unicms_template_italia-1.0.3/src/unicms_template_italia/templates/blocks/
--rw-r--r--   0 runner    (1001) docker     (123)     3654 2022-12-07 15:30:14.000000 unicms_template_italia-1.0.3/src/unicms_template_italia/templates/blocks/italia_carousel_hero_slider.html
--rw-r--r--   0 runner    (1001) docker     (123)      341 2022-12-07 15:30:14.000000 unicms_template_italia-1.0.3/src/unicms_template_italia/templates/blocks/italia_heading.html
--rw-r--r--   0 runner    (1001) docker     (123)      413 2022-12-07 15:30:14.000000 unicms_template_italia-1.0.3/src/unicms_template_italia/templates/blocks/italia_link.html
--rw-r--r--   0 runner    (1001) docker     (123)      306 2022-12-07 15:30:14.000000 unicms_template_italia-1.0.3/src/unicms_template_italia/templates/blocks/italia_link_iframe.html
--rw-r--r--   0 runner    (1001) docker     (123)     1283 2022-12-07 15:30:14.000000 unicms_template_italia-1.0.3/src/unicms_template_italia/templates/blocks/italia_media_collection_image_grid.html
--rw-r--r--   0 runner    (1001) docker     (123)     1376 2022-12-07 15:30:14.000000 unicms_template_italia-1.0.3/src/unicms_template_italia/templates/blocks/italia_media_collection_image_slider.html
--rw-r--r--   0 runner    (1001) docker     (123)     1008 2022-12-07 15:30:14.000000 unicms_template_italia-1.0.3/src/unicms_template_italia/templates/blocks/italia_media_collection_image_slider_full.html
--rw-r--r--   0 runner    (1001) docker     (123)      885 2022-12-07 15:30:14.000000 unicms_template_italia-1.0.3/src/unicms_template_italia/templates/blocks/italia_media_collection_list.html
--rw-r--r--   0 runner    (1001) docker     (123)      188 2022-12-07 15:30:14.000000 unicms_template_italia-1.0.3/src/unicms_template_italia/templates/blocks/italia_media_image.html
--rw-r--r--   0 runner    (1001) docker     (123)     7985 2022-12-07 15:30:14.000000 unicms_template_italia-1.0.3/src/unicms_template_italia/templates/blocks/italia_menu_main.html
--rw-r--r--   0 runner    (1001) docker     (123)     2036 2022-12-07 15:30:14.000000 unicms_template_italia-1.0.3/src/unicms_template_italia/templates/blocks/italia_menu_side.html
--rw-r--r--   0 runner    (1001) docker     (123)     1328 2022-12-07 15:30:14.000000 unicms_template_italia-1.0.3/src/unicms_template_italia/templates/blocks/italia_pub_alert.html
--rw-r--r--   0 runner    (1001) docker     (123)     3183 2022-12-07 15:30:14.000000 unicms_template_italia-1.0.3/src/unicms_template_italia/templates/blocks/italia_pub_collapse.html
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2022-12-07 15:30:14.000000 unicms_template_italia-1.0.3/src/unicms_template_italia/templates/blocks/italia_pub_collapse_logo_image.html
--rw-r--r--   0 runner    (1001) docker     (123)    22369 2022-12-07 15:30:14.000000 unicms_template_italia-1.0.3/src/unicms_template_italia/templates/blocks/italia_search_engine.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-07 15:30:25.289712 unicms_template_italia-1.0.3/src/unicms_template_italia/templates/components/
--rw-r--r--   0 runner    (1001) docker     (123)     4671 2022-12-07 15:30:14.000000 unicms_template_italia-1.0.3/src/unicms_template_italia/templates/components/italia_editorialboard_frontend_menu.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-07 15:30:25.289712 unicms_template_italia-1.0.3/src/unicms_template_italia/templates/includes/
--rw-r--r--   0 runner    (1001) docker     (123)      456 2022-12-07 15:30:14.000000 unicms_template_italia-1.0.3/src/unicms_template_italia/templates/includes/edit_news.html
--rw-r--r--   0 runner    (1001) docker     (123)      468 2022-12-07 15:30:14.000000 unicms_template_italia-1.0.3/src/unicms_template_italia/templates/includes/edit_page_publication.html
--rw-r--r--   0 runner    (1001) docker     (123)     3034 2022-12-07 15:30:14.000000 unicms_template_italia-1.0.3/src/unicms_template_italia/templates/includes/social_share.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-07 15:30:25.289712 unicms_template_italia-1.0.3/src/unicms_template_italia/templates/inits/
--rw-r--r--   0 runner    (1001) docker     (123)      329 2022-12-07 15:30:14.000000 unicms_template_italia-1.0.3/src/unicms_template_italia/templates/inits/owl-carousel-init.html
--rw-r--r--   0 runner    (1001) docker     (123)      443 2022-12-07 15:30:14.000000 unicms_template_italia-1.0.3/src/unicms_template_italia/templates/inits/search-input-handler.html
--rw-r--r--   0 runner    (1001) docker     (123)      290 2022-12-07 15:30:14.000000 unicms_template_italia-1.0.3/src/unicms_template_italia/templates/inits/vue-init.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-07 15:30:25.289712 unicms_template_italia-1.0.3/src/unicms_template_italia/templates/pages/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2022-12-07 15:30:14.000000 unicms_template_italia-1.0.3/src/unicms_template_italia/templates/pages/italia.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-07 15:30:25.289712 unicms_template_italia-1.0.3/src/unicms_template_italia/templatetags/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-07 15:30:14.000000 unicms_template_italia-1.0.3/src/unicms_template_italia/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2172 2022-12-07 15:30:14.000000 unicms_template_italia-1.0.3/src/unicms_template_italia/templatetags/unicms_template_italia.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-07 15:30:25.293712 unicms_template_italia-1.0.3/unicms_template_italia.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      954 2022-12-07 15:30:25.000000 unicms_template_italia-1.0.3/unicms_template_italia.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2759 2022-12-07 15:30:25.000000 unicms_template_italia-1.0.3/unicms_template_italia.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-07 15:30:25.000000 unicms_template_italia-1.0.3/unicms_template_italia.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       37 2022-12-07 15:30:25.000000 unicms_template_italia-1.0.3/unicms_template_italia.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2022-12-07 15:30:25.000000 unicms_template_italia-1.0.3/unicms_template_italia.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 07:34:21.427257 unicms_template_italia-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-22 07:34:12.000000 unicms_template_italia-1.1.0/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-22 07:34:12.000000 unicms_template_italia-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-05-22 07:34:21.427257 unicms_template_italia-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-22 07:34:12.000000 unicms_template_italia-1.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 07:34:21.427257 unicms_template_italia-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-05-22 07:34:12.000000 unicms_template_italia-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 07:34:21.419257 unicms_template_italia-1.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 07:34:21.419257 unicms_template_italia-1.1.0/src/unicms_template_italia/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 07:34:12.000000 unicms_template_italia-1.1.0/src/unicms_template_italia/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-22 07:34:12.000000 unicms_template_italia-1.1.0/src/unicms_template_italia/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 07:34:21.419257 unicms_template_italia-1.1.0/src/unicms_template_italia/locale/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 07:34:21.419257 unicms_template_italia-1.1.0/src/unicms_template_italia/locale/it/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 07:34:21.419257 unicms_template_italia-1.1.0/src/unicms_template_italia/locale/it/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-05-22 07:34:12.000000 unicms_template_italia-1.1.0/src/unicms_template_italia/locale/it/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     9747 2023-05-22 07:34:12.000000 unicms_template_italia-1.1.0/src/unicms_template_italia/locale/it/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (123)     9297 2023-05-22 07:34:12.000000 unicms_template_italia-1.1.0/src/unicms_template_italia/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 07:34:21.419257 unicms_template_italia-1.1.0/src/unicms_template_italia/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 07:34:21.419257 unicms_template_italia-1.1.0/src/unicms_template_italia/static/css/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 07:34:21.419257 unicms_template_italia-1.1.0/src/unicms_template_italia/static/css/vendor/
+-rw-r--r--   0 runner    (1001) docker     (123)     3658 2023-05-22 07:34:12.000000 unicms_template_italia-1.1.0/src/unicms_template_italia/static/css/vendor/owl.carousel.min.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 07:34:21.423257 unicms_template_italia-1.1.0/src/unicms_template_italia/static/js/
+-rw-r--r--   0 runner    (1001) docker     (123)    26730 2023-05-22 07:34:12.000000 unicms_template_italia-1.1.0/src/unicms_template_italia/static/js/axios.1.1.3.js
+-rw-r--r--   0 runner    (1001) docker     (123)   125861 2023-05-22 07:34:12.000000 unicms_template_italia-1.1.0/src/unicms_template_italia/static/js/axios.min.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-05-22 07:34:12.000000 unicms_template_italia-1.1.0/src/unicms_template_italia/static/js/deferred_iframe_src.js
+-rw-r--r--   0 runner    (1001) docker     (123)    89947 2023-05-22 07:34:12.000000 unicms_template_italia-1.1.0/src/unicms_template_italia/static/js/jquery.3.6.3.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-05-22 07:34:12.000000 unicms_template_italia-1.1.0/src/unicms_template_italia/static/js/passive_listeners.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 07:34:21.423257 unicms_template_italia-1.1.0/src/unicms_template_italia/static/js/vendor/
+-rw-r--r--   0 runner    (1001) docker     (123)    44342 2023-05-22 07:34:12.000000 unicms_template_italia-1.1.0/src/unicms_template_italia/static/js/vendor/owl.carousel.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)   107216 2023-05-22 07:34:12.000000 unicms_template_italia-1.1.0/src/unicms_template_italia/static/js/vue.2.7.14.js
+-rw-r--r--   0 runner    (1001) docker     (123)      875 2023-05-22 07:34:12.000000 unicms_template_italia-1.1.0/src/unicms_template_italia/static/js/vue.options.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 07:34:21.419257 unicms_template_italia-1.1.0/src/unicms_template_italia/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 07:34:21.423257 unicms_template_italia-1.1.0/src/unicms_template_italia/templates/bases/
+-rw-r--r--   0 runner    (1001) docker     (123)    90865 2023-05-22 07:34:12.000000 unicms_template_italia-1.1.0/src/unicms_template_italia/templates/bases/unicms_italia.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 07:34:21.423257 unicms_template_italia-1.1.0/src/unicms_template_italia/templates/blocks/
+-rw-r--r--   0 runner    (1001) docker     (123)     3654 2023-05-22 07:34:12.000000 unicms_template_italia-1.1.0/src/unicms_template_italia/templates/blocks/italia_carousel_hero_slider.html
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-05-22 07:34:12.000000 unicms_template_italia-1.1.0/src/unicms_template_italia/templates/blocks/italia_heading.html
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-05-22 07:34:12.000000 unicms_template_italia-1.1.0/src/unicms_template_italia/templates/blocks/italia_link.html
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-05-22 07:34:12.000000 unicms_template_italia-1.1.0/src/unicms_template_italia/templates/blocks/italia_link_iframe.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-05-22 07:34:12.000000 unicms_template_italia-1.1.0/src/unicms_template_italia/templates/blocks/italia_media_collection_image_grid.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-05-22 07:34:12.000000 unicms_template_italia-1.1.0/src/unicms_template_italia/templates/blocks/italia_media_collection_image_slider.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-05-22 07:34:12.000000 unicms_template_italia-1.1.0/src/unicms_template_italia/templates/blocks/italia_media_collection_image_slider_full.html
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-05-22 07:34:12.000000 unicms_template_italia-1.1.0/src/unicms_template_italia/templates/blocks/italia_media_collection_list.html
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-22 07:34:12.000000 unicms_template_italia-1.1.0/src/unicms_template_italia/templates/blocks/italia_media_image.html
+-rw-r--r--   0 runner    (1001) docker     (123)     7985 2023-05-22 07:34:12.000000 unicms_template_italia-1.1.0/src/unicms_template_italia/templates/blocks/italia_menu_main.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-05-22 07:34:12.000000 unicms_template_italia-1.1.0/src/unicms_template_italia/templates/blocks/italia_menu_side.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-05-22 07:34:12.000000 unicms_template_italia-1.1.0/src/unicms_template_italia/templates/blocks/italia_pub_alert.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3183 2023-05-22 07:34:12.000000 unicms_template_italia-1.1.0/src/unicms_template_italia/templates/blocks/italia_pub_collapse.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-05-22 07:34:12.000000 unicms_template_italia-1.1.0/src/unicms_template_italia/templates/blocks/italia_pub_collapse_logo_image.html
+-rw-r--r--   0 runner    (1001) docker     (123)    21904 2023-05-22 07:34:12.000000 unicms_template_italia-1.1.0/src/unicms_template_italia/templates/blocks/italia_search_engine.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 07:34:21.423257 unicms_template_italia-1.1.0/src/unicms_template_italia/templates/components/
+-rw-r--r--   0 runner    (1001) docker     (123)     4671 2023-05-22 07:34:12.000000 unicms_template_italia-1.1.0/src/unicms_template_italia/templates/components/italia_editorialboard_frontend_menu.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 07:34:21.427257 unicms_template_italia-1.1.0/src/unicms_template_italia/templates/includes/
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-05-22 07:34:12.000000 unicms_template_italia-1.1.0/src/unicms_template_italia/templates/includes/edit_news.html
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-05-22 07:34:12.000000 unicms_template_italia-1.1.0/src/unicms_template_italia/templates/includes/edit_page_publication.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3034 2023-05-22 07:34:12.000000 unicms_template_italia-1.1.0/src/unicms_template_italia/templates/includes/social_share.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 07:34:21.427257 unicms_template_italia-1.1.0/src/unicms_template_italia/templates/inits/
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-05-22 07:34:12.000000 unicms_template_italia-1.1.0/src/unicms_template_italia/templates/inits/owl-carousel-init.html
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-05-22 07:34:12.000000 unicms_template_italia-1.1.0/src/unicms_template_italia/templates/inits/search-input-handler.html
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-05-22 07:34:12.000000 unicms_template_italia-1.1.0/src/unicms_template_italia/templates/inits/vue-init.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 07:34:21.427257 unicms_template_italia-1.1.0/src/unicms_template_italia/templates/pages/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-22 07:34:12.000000 unicms_template_italia-1.1.0/src/unicms_template_italia/templates/pages/italia.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 07:34:21.427257 unicms_template_italia-1.1.0/src/unicms_template_italia/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 07:34:12.000000 unicms_template_italia-1.1.0/src/unicms_template_italia/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-05-22 07:34:12.000000 unicms_template_italia-1.1.0/src/unicms_template_italia/templatetags/unicms_template_italia.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 07:34:21.427257 unicms_template_italia-1.1.0/unicms_template_italia.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-05-22 07:34:21.000000 unicms_template_italia-1.1.0/unicms_template_italia.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2816 2023-05-22 07:34:21.000000 unicms_template_italia-1.1.0/unicms_template_italia.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 07:34:21.000000 unicms_template_italia-1.1.0/unicms_template_italia.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-22 07:34:21.000000 unicms_template_italia-1.1.0/unicms_template_italia.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-22 07:34:21.000000 unicms_template_italia-1.1.0/unicms_template_italia.egg-info/top_level.txt
```

### Comparing `unicms_template_italia-1.0.3/LICENSE` & `unicms_template_italia-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `unicms_template_italia-1.0.3/PKG-INFO` & `unicms_template_italia-1.1.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unicms_template_italia
-Version: 1.0.3
+Version: 1.1.0
 Summary: uniCMS Template based on Bootstrap Italia design
 Home-page: https://github.com/UniversitaDellaCalabria/unicms-template-italia
 Author: Giuseppe De Marco, Francesco Filicetti
 Author-email: giuseppe.demarco@unical.it, francesco.filicetti@unical.it
 License: Apache License 2.0
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `unicms_template_italia-1.0.3/setup.py` & `unicms_template_italia-1.1.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 #  twine upload dist/*
 
 SRC_FOLDER = 'src'
 PKG_NAME = 'unicms_template_italia'
 
 setup(
     name=PKG_NAME,
-    version='1.0.3',
+    version='1.1.0',
 
     packages=[PKG_NAME],
     package_dir={PKG_NAME: f"{SRC_FOLDER}/{PKG_NAME}"},
 
     package_data={PKG_NAME: [i.replace(f'{SRC_FOLDER}/{PKG_NAME}/', '')
                                    for i in glob(f'{SRC_FOLDER}/{PKG_NAME}/**',
                                                  recursive=True)]
```

### Comparing `unicms_template_italia-1.0.3/src/unicms_template_italia/locale/it/LC_MESSAGES/django.mo` & `unicms_template_italia-1.1.0/src/unicms_template_italia/locale/it/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `unicms_template_italia-1.0.3/src/unicms_template_italia/locale/it/LC_MESSAGES/django.po` & `unicms_template_italia-1.1.0/src/unicms_template_italia/locale/it/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `unicms_template_italia-1.0.3/src/unicms_template_italia/settings.py` & `unicms_template_italia-1.1.0/src/unicms_template_italia/settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,21 @@
 from django.utils.translation import gettext_lazy as _
 
 CMS_TEMPLATE_BLOCK_SECTIONS = (
-                               ('pre-head', _('Pre-Head')),
-                               ('head', _('Head')),
+                               ('html-head', _('HTML Head')),
+                               ('html-bottom', _('HTML Bottom')),
 
                                ('menu-1', _('Menu-1')),
                                ('menu-2', _('Menu-2')),
                                ('menu-3', _('Menu-3')),
                                ('menu-4', _('Menu-4')),
 
                                ('banner', _('Banner')),
                                ('slider-2', _('Slider-2')),
 
-                               ('pre-footer', _('Pre-Footer')),
-                               ('footer', _('Footer')),
-                               ('post-footer', _('Post-Footer')),
-
                                # breadcrumbs
                                ('breadcrumbs', _('Breadcrumbs')),
 
                                # section 1
                                ('section-1',
                                 (
                                  ('1-top-a', _('Section 1 - Top A')),
@@ -133,8 +129,8 @@
 LINKEDIN_ENDPOINT = 'https://www.linkedin.com/shareArticle?mini=true&url='
 TELEGRAM_ENDPOINT = 'https://t.me/share/url?text=%s&url=%s'
 WHATSAPP_ENDPOINT = 'https://api.whatsapp.com/send?text='
 PINTEREST_ENDPOINT = 'https://www.pinterest.com/pin/create/button/?url='
 
 # CDN FOR STATICS
 UNICMS_TEMPLATE_ITALIA_USE_CDN = False
-UNICMS_TEMPLATE_ITALIA_CDN = 'https://cdn.jsdelivr.net/gh/UniversitaDellaCalabria/unicms-template-italia@1.0.3/src/unicms_template_italia/static'
+UNICMS_TEMPLATE_ITALIA_CDN = 'https://cdn.jsdelivr.net/gh/UniversitaDellaCalabria/unicms-template-italia@1.1.0/src/unicms_template_italia/static'
```

### Comparing `unicms_template_italia-1.0.3/src/unicms_template_italia/static/css/vendor/owl.carousel.min.css` & `unicms_template_italia-1.1.0/src/unicms_template_italia/static/css/vendor/owl.carousel.min.css`

 * *Files identical despite different names*

### Comparing `unicms_template_italia-1.0.3/src/unicms_template_italia/static/js/axios.1.1.3.js` & `unicms_template_italia-1.1.0/src/unicms_template_italia/static/js/axios.1.1.3.js`

 * *Files identical despite different names*

### Comparing `unicms_template_italia-1.0.3/src/unicms_template_italia/static/js/axios.min.js.map` & `unicms_template_italia-1.1.0/src/unicms_template_italia/static/js/axios.min.js.map`

 * *Files identical despite different names*

### Comparing `unicms_template_italia-1.0.3/src/unicms_template_italia/static/js/passive_listeners.js` & `unicms_template_italia-1.1.0/src/unicms_template_italia/static/js/passive_listeners.js`

 * *Files identical despite different names*

### Comparing `unicms_template_italia-1.0.3/src/unicms_template_italia/static/js/vendor/owl.carousel.min.js` & `unicms_template_italia-1.1.0/src/unicms_template_italia/static/js/vendor/owl.carousel.min.js`

 * *Files identical despite different names*

### Comparing `unicms_template_italia-1.0.3/src/unicms_template_italia/static/js/vue.2.7.14.js` & `unicms_template_italia-1.1.0/src/unicms_template_italia/static/js/vue.2.7.14.js`

 * *Files identical despite different names*

### Comparing `unicms_template_italia-1.0.3/src/unicms_template_italia/static/js/vue.options.js` & `unicms_template_italia-1.1.0/src/unicms_template_italia/static/js/vue.options.js`

 * *Files identical despite different names*

### Comparing `unicms_template_italia-1.0.3/src/unicms_template_italia/templates/bases/unicms_italia.html` & `unicms_template_italia-1.1.0/src/unicms_template_italia/templates/bases/unicms_italia.html`

 * *Files 2% similar despite different names*

```diff
@@ -46,5562 +46,5635 @@
 000002d0: 7b25 2065 6e64 626c 6f63 6b20 7061 6765  {% endblock page
 000002e0: 5f6d 6574 615f 726f 626f 7473 2025 7d0a  _meta_robots %}.
 000002f0: 0a3c 212d 2d20 5265 7475 726e 2074 6f20  .<!-- Return to 
 00000300: 4167 6964 206e 6174 6976 6520 7465 6d70  Agid native temp
 00000310: 6c61 7465 202d 2d3e 0a7b 2520 626c 6f63  late -->.{% bloc
 00000320: 6b20 6578 7472 615f 6865 6164 2025 7d0a  k extra_head %}.
 00000330: 2020 2020 7b7b 2062 6c6f 636b 2e73 7570      {{ block.sup
-00000340: 6572 207d 7d0a 2020 2020 7b25 2062 6c6f  er }}.    {% blo
-00000350: 636b 2068 6561 645f 696e 6974 7320 257d  ck head_inits %}
-00000360: 0a20 2020 207b 2520 696e 636c 7564 6520  .    {% include 
-00000370: 2269 6e69 7473 2f76 7565 2d69 6e69 742e  "inits/vue-init.
-00000380: 6874 6d6c 2220 257d 0a20 2020 207b 2520  html" %}.    {% 
-00000390: 696e 636c 7564 6520 2269 6e69 7473 2f6f  include "inits/o
-000003a0: 776c 2d63 6172 6f75 7365 6c2d 696e 6974  wl-carousel-init
-000003b0: 2e68 746d 6c22 2025 7d0a 2020 2020 7b25  .html" %}.    {%
-000003c0: 2065 6e64 626c 6f63 6b20 6865 6164 5f69   endblock head_i
-000003d0: 6e69 7473 2025 7d0a 0a20 2020 207b 2520  nits %}..    {% 
-000003e0: 626c 6f63 6b20 736f 6369 616c 5f74 6167  block social_tag
-000003f0: 7320 257d 7b25 2065 6e64 626c 6f63 6b20  s %}{% endblock 
-00000400: 736f 6369 616c 5f74 6167 7320 257d 0a7b  social_tags %}.{
-00000410: 2520 656e 6462 6c6f 636b 2065 7874 7261  % endblock extra
-00000420: 5f68 6561 6420 257d 0a0a 3c21 2d2d 2050  _head %}..<!-- P
-00000430: 6167 6520 5469 746c 6520 2d2d 3e0a 3c21  age Title -->.<!
-00000440: 2d2d 2050 6167 6520 5469 746c 6520 2d2d  -- Page Title --
-00000450: 3e0a 7b25 2062 6c6f 636b 2070 6167 655f  >.{% block page_
-00000460: 7469 746c 6520 257d 0a20 2020 207b 2520  title %}.    {% 
-00000470: 6966 2070 6167 6520 257d 0a20 2020 2020  if page %}.     
-00000480: 2020 207b 7b20 7061 6765 2e74 6974 6c65     {{ page.title
-00000490: 207d 7d20 2d20 7b7b 2077 6562 7369 7465   }} - {{ website
-000004a0: 2e6e 616d 6520 7d7d 0a20 2020 207b 2520  .name }}.    {% 
-000004b0: 656c 7365 2025 7d0a 2020 2020 2020 2020  else %}.        
-000004c0: 7b25 2074 7261 6e73 2022 556e 6976 6572  {% trans "Univer
-000004d0: 7369 7479 206f 6620 4361 6c61 6272 6961  sity of Calabria
-000004e0: 2220 257d 0a20 2020 207b 2520 656e 6469  " %}.    {% endi
-000004f0: 6620 257d 0a7b 2520 656e 6462 6c6f 636b  f %}.{% endblock
-00000500: 2070 6167 655f 7469 746c 6520 257d 0a0a   page_title %}..
-00000510: 3c21 2d2d 2048 6561 6465 7220 736c 696d  <!-- Header slim
-00000520: 2077 7261 7070 6572 202d 2d3e 0a7b 2520   wrapper -->.{% 
-00000530: 626c 6f63 6b20 6865 6164 6572 5f73 6c69  block header_sli
-00000540: 6d5f 746f 705f 6c65 6674 2025 7d0a 7b25  m_top_left %}.{%
-00000550: 2069 6620 7265 7175 6573 742e 7573 6572   if request.user
-00000560: 2e69 735f 7374 6166 6620 257d 0a7b 2520  .is_staff %}.{% 
-00000570: 696e 636c 7564 6520 2263 6f6d 706f 6e65  include "compone
-00000580: 6e74 732f 6974 616c 6961 5f65 6469 746f  nts/italia_edito
-00000590: 7269 616c 626f 6172 645f 6672 6f6e 7465  rialboard_fronte
-000005a0: 6e64 5f6d 656e 752e 6874 6d6c 2220 257d  nd_menu.html" %}
-000005b0: 0a7b 2520 656e 6469 6620 257d 0a7b 2520  .{% endif %}.{% 
-000005c0: 656e 6462 6c6f 636b 2068 6561 6465 725f  endblock header_
-000005d0: 736c 696d 5f74 6f70 5f6c 6566 7420 257d  slim_top_left %}
-000005e0: 0a0a 7b25 2062 6c6f 636b 2068 6561 6465  ..{% block heade
-000005f0: 725f 736c 696d 5f73 7562 5f6d 656e 7520  r_slim_sub_menu 
-00000600: 257d 0a3c 6469 7620 636c 6173 733d 226e  %}.<div class="n
-00000610: 6176 2d69 7465 6d20 6472 6f70 646f 776e  av-item dropdown
-00000620: 223e 0a20 2020 203c 6120 636c 6173 733d  ">.    <a class=
-00000630: 226e 6176 2d6c 696e 6b20 6472 6f70 646f  "nav-link dropdo
-00000640: 776e 2d74 6f67 676c 6522 0a20 2020 2020  wn-toggle".     
-00000650: 2020 6872 6566 3d22 2322 0a20 2020 2020    href="#".     
-00000660: 2020 6461 7461 2d74 6f67 676c 653d 2264    data-toggle="d
-00000670: 726f 7064 6f77 6e22 0a20 2020 2020 2020  ropdown".       
-00000680: 6172 6961 2d65 7870 616e 6465 643d 2266  aria-expanded="f
-00000690: 616c 7365 223e 0a20 2020 2020 2020 203c  alse">.        <
-000006a0: 7370 616e 3e7b 7b20 7265 7175 6573 742e  span>{{ request.
-000006b0: 4c41 4e47 5541 4745 5f43 4f44 4520 7d7d  LANGUAGE_CODE }}
-000006c0: 3c2f 7370 616e 3e0a 2020 2020 2020 2020  </span>.        
-000006d0: 3c73 7667 2063 6c61 7373 3d22 6963 6f6e  <svg class="icon
-000006e0: 2064 2d6e 6f6e 6520 642d 6c67 2d62 6c6f   d-none d-lg-blo
-000006f0: 636b 223e 0a20 2020 2020 2020 2020 2020  ck">.           
-00000700: 203c 7573 6520 786c 696e 6b3a 6872 6566   <use xlink:href
-00000710: 3d22 7b25 2073 7461 7469 6320 2773 7667  ="{% static 'svg
-00000720: 2f73 7072 6974 6573 2e73 7667 2720 257d  /sprites.svg' %}
-00000730: 2369 742d 6578 7061 6e64 223e 3c2f 7573  #it-expand"></us
-00000740: 653e 0a20 2020 2020 2020 203c 2f73 7667  e>.        </svg
-00000750: 3e0a 2020 2020 3c2f 613e 0a20 2020 203c  >.    </a>.    <
-00000760: 6469 7620 636c 6173 733d 2264 726f 7064  div class="dropd
-00000770: 6f77 6e2d 6d65 6e75 223e 0a20 2020 2020  own-menu">.     
-00000780: 2020 203c 6469 7620 636c 6173 733d 2272     <div class="r
-00000790: 6f77 223e 0a20 2020 2020 2020 2020 2020  ow">.           
-000007a0: 203c 6469 7620 636c 6173 733d 2263 6f6c   <div class="col
-000007b0: 2d31 3222 3e0a 2020 2020 2020 2020 2020  -12">.          
-000007c0: 2020 2020 2020 3c64 6976 2063 6c61 7373        <div class
-000007d0: 3d22 6c69 6e6b 2d6c 6973 742d 7772 6170  ="link-list-wrap
-000007e0: 7065 7222 3e0a 2020 2020 2020 2020 2020  per">.          
-000007f0: 2020 2020 2020 2020 2020 3c75 6c20 636c            <ul cl
-00000800: 6173 733d 226c 696e 6b2d 6c69 7374 223e  ass="link-list">
-00000810: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000820: 2020 2020 2020 2020 207b 2520 6c61 6e67           {% lang
-00000830: 7561 6765 5f6d 656e 7520 6173 206c 616e  uage_menu as lan
-00000840: 6775 6167 655f 7572 6c73 2025 7d0a 2020  guage_urls %}.  
-00000850: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000860: 2020 2020 2020 7b25 2066 6f72 2063 6f64        {% for cod
-00000870: 2c70 6172 616d 7320 696e 206c 616e 6775  ,params in langu
-00000880: 6167 655f 7572 6c73 2e69 7465 6d73 2025  age_urls.items %
-00000890: 7d0a 2020 2020 2020 2020 2020 2020 2020  }.              
-000008a0: 2020 2020 2020 2020 2020 3c6c 693e 3c61            <li><a
-000008b0: 2063 6c61 7373 3d22 6c69 7374 2d69 7465   class="list-ite
-000008c0: 6d22 2068 7265 663d 227b 7b20 7061 7261  m" href="{{ para
-000008d0: 6d73 2e31 207d 7d22 3e3c 7370 616e 3e7b  ms.1 }}"><span>{
-000008e0: 7b20 7061 7261 6d73 2e30 207d 7d3c 2f73  { params.0 }}</s
-000008f0: 7061 6e3e 3c2f 613e 3c2f 6c69 3e0a 2020  pan></a></li>.  
-00000900: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000910: 2020 2020 2020 7b25 2065 6e64 666f 7220        {% endfor 
-00000920: 257d 0a20 2020 2020 2020 2020 2020 2020  %}.             
-00000930: 2020 2020 2020 203c 2f75 6c3e 0a20 2020         </ul>.   
-00000940: 2020 2020 2020 2020 2020 2020 203c 2f64               </d
-00000950: 6976 3e0a 2020 2020 2020 2020 2020 2020  iv>.            
-00000960: 3c2f 6469 763e 0a20 2020 2020 2020 203c  </div>.        <
-00000970: 2f64 6976 3e0a 2020 2020 3c2f 6469 763e  /div>.    </div>
-00000980: 0a3c 2f64 6976 3e0a 7b25 2065 6e64 626c  .</div>.{% endbl
-00000990: 6f63 6b20 6865 6164 6572 5f73 6c69 6d5f  ock header_slim_
-000009a0: 7375 625f 6d65 6e75 2025 7d0a 0a7b 2520  sub_menu %}..{% 
-000009b0: 626c 6f63 6b20 6865 6164 6572 5f73 6c69  block header_sli
-000009c0: 6d5f 6275 7474 6f6e 7320 257d 0a3c 6469  m_buttons %}.<di
-000009d0: 7620 636c 6173 733d 2269 742d 6163 6365  v class="it-acce
-000009e0: 7373 2d74 6f70 2d77 7261 7070 6572 223e  ss-top-wrapper">
-000009f0: 0a20 2020 207b 2520 6966 2072 6571 7565  .    {% if reque
-00000a00: 7374 2e75 7365 722e 6973 5f61 7574 6865  st.user.is_authe
-00000a10: 6e74 6963 6174 6564 2025 7d0a 2020 2020  nticated %}.    
-00000a20: 3c62 7574 746f 6e20 636c 6173 733d 2262  <button class="b
-00000a30: 746e 2062 746e 2d70 7269 6d61 7279 2062  tn btn-primary b
-00000a40: 746e 2d73 6d22 2068 7265 663d 227b 2520  tn-sm" href="{% 
-00000a50: 7572 6c20 276c 6f67 6f75 7427 2025 7d22  url 'logout' %}"
-00000a60: 2074 7970 653d 2262 7574 746f 6e22 3e0a   type="button">.
-00000a70: 2020 2020 2020 2020 7b25 2074 7261 6e73          {% trans
-00000a80: 2022 4c6f 676f 7574 2220 257d 0a20 2020   "Logout" %}.   
-00000a90: 203c 2f62 7574 746f 6e3e 0a20 2020 207b   </button>.    {
-00000aa0: 2520 656c 7365 2025 7d0a 2020 2020 3c62  % else %}.    <b
-00000ab0: 7574 746f 6e20 636c 6173 733d 2262 746e  utton class="btn
-00000ac0: 2062 746e 2d70 7269 6d61 7279 2062 746e   btn-primary btn
-00000ad0: 2d73 6d22 2068 7265 663d 227b 2520 7572  -sm" href="{% ur
-00000ae0: 6c20 276c 6f67 696e 2720 257d 2220 7479  l 'login' %}" ty
-00000af0: 7065 3d22 6275 7474 6f6e 223e 0a20 2020  pe="button">.   
-00000b00: 2020 2020 207b 2520 7472 616e 7320 224c       {% trans "L
-00000b10: 6f67 696e 2220 257d 0a20 2020 203c 2f62  ogin" %}.    </b
-00000b20: 7574 746f 6e3e 0a20 2020 207b 2520 656e  utton>.    {% en
-00000b30: 6469 6620 257d 0a3c 2f64 6976 3e0a 7b25  dif %}.</div>.{%
-00000b40: 2065 6e64 626c 6f63 6b20 6865 6164 6572   endblock header
-00000b50: 5f73 6c69 6d5f 6275 7474 6f6e 7320 257d  _slim_buttons %}
-00000b60: 0a3c 212d 2d20 656e 6420 4865 6164 6572  .<!-- end Header
-00000b70: 2073 6c69 6d20 7772 6170 7065 7220 2d2d   slim wrapper --
-00000b80: 3e0a 0a3c 212d 2d20 5552 4c20 6c69 6e6b  >..<!-- URL link
-00000b90: 206c 6f67 6f20 616e 6420 6f72 6720 6e61   logo and org na
-00000ba0: 6d65 202d 2d3e 0a7b 2520 626c 6f63 6b20  me -->.{% block 
-00000bb0: 6865 6164 6572 5f63 656e 7465 725f 7572  header_center_ur
-00000bc0: 6c20 257d 0a7b 2520 7365 7474 696e 6773  l %}.{% settings
-00000bd0: 5f76 616c 7565 2022 434d 535f 5041 5448  _value "CMS_PATH
-00000be0: 5f50 5245 4649 5822 2061 7320 636d 735f  _PREFIX" as cms_
-00000bf0: 7061 7468 5f70 7265 6669 7820 257d 2f7b  path_prefix %}/{
-00000c00: 7b20 636d 735f 7061 7468 5f70 7265 6669  { cms_path_prefi
-00000c10: 7820 7d7d 0a7b 2520 656e 6462 6c6f 636b  x }}.{% endblock
-00000c20: 2068 6561 6465 725f 6365 6e74 6572 5f75   header_center_u
-00000c30: 726c 2025 7d0a 0a7b 2520 626c 6f63 6b20  rl %}..{% block 
-00000c40: 6865 6164 6572 5f6d 6f62 696c 655f 6172  header_mobile_ar
-00000c50: 726f 7720 257d 0a7b 2520 656e 6462 6c6f  row %}.{% endblo
-00000c60: 636b 2068 6561 6465 725f 6d6f 6269 6c65  ck header_mobile
-00000c70: 5f61 7272 6f77 2025 7d0a 0a7b 2520 626c  _arrow %}..{% bl
-00000c80: 6f63 6b20 6865 6164 6572 5f6d 6f62 696c  ock header_mobil
-00000c90: 655f 736c 696d 5f6d 656e 7520 257d 0a7b  e_slim_menu %}.{
-00000ca0: 2520 656e 6462 6c6f 636b 2068 6561 6465  % endblock heade
-00000cb0: 725f 6d6f 6269 6c65 5f73 6c69 6d5f 6d65  r_mobile_slim_me
-00000cc0: 6e75 2025 7d0a 0a7b 2520 626c 6f63 6b20  nu %}..{% block 
-00000cd0: 6865 6164 6572 5f73 6c69 6d5f 6d6f 6269  header_slim_mobi
-00000ce0: 6c65 5f6f 7267 5f6e 616d 6520 257d 0a7b  le_org_name %}.{
-00000cf0: 2520 656e 6462 6c6f 636b 2068 6561 6465  % endblock heade
-00000d00: 725f 736c 696d 5f6d 6f62 696c 655f 6f72  r_slim_mobile_or
-00000d10: 675f 6e61 6d65 2025 7d0a 0a7b 2520 626c  g_name %}..{% bl
-00000d20: 6f63 6b20 6865 6164 6572 5f63 656e 7465  ock header_cente
-00000d30: 725f 7772 6170 7065 725f 636f 6c75 6d6e  r_wrapper_column
-00000d40: 7320 257d 0a63 6f6c 2d31 3020 6f66 6673  s %}.col-10 offs
-00000d50: 6574 2d32 2063 6f6c 2d6c 672d 3132 206f  et-2 col-lg-12 o
-00000d60: 6666 7365 742d 6c67 2d30 0a7b 2520 656e  ffset-lg-0.{% en
-00000d70: 6462 6c6f 636b 2068 6561 6465 725f 6365  dblock header_ce
-00000d80: 6e74 6572 5f77 7261 7070 6572 5f63 6f6c  nter_wrapper_col
-00000d90: 756d 6e73 2025 7d0a 0a3c 212d 2d20 4d61  umns %}..<!-- Ma
-00000da0: 696e 204d 656e 7520 2d2d 3e0a 7b25 2062  in Menu -->.{% b
-00000db0: 6c6f 636b 206d 6169 6e5f 6d65 6e75 2025  lock main_menu %
-00000dc0: 7d0a 2020 2020 7b25 206c 6f61 645f 626c  }.    {% load_bl
-00000dd0: 6f63 6b73 2073 6563 7469 6f6e 3d27 6d65  ocks section='me
-00000de0: 6e75 2d31 2720 257d 0a7b 2520 656e 6462  nu-1' %}.{% endb
-00000df0: 6c6f 636b 206d 6169 6e5f 6d65 6e75 2025  lock main_menu %
-00000e00: 7d0a 0a3c 212d 2d20 436f 6e74 6169 6e65  }..<!-- Containe
-00000e10: 7220 2d2d 3e0a 7b25 2062 6c6f 636b 2063  r -->.{% block c
-00000e20: 6f6e 7461 696e 6572 2025 7d0a 0a20 2020  ontainer %}..   
-00000e30: 203c 212d 2d20 4d61 696e 2042 616e 6e65   <!-- Main Banne
-00000e40: 722d 2d3e 0a20 2020 207b 2520 626c 6f63  r-->.    {% bloc
-00000e50: 6b20 6261 6e6e 6572 2025 7d0a 2020 2020  k banner %}.    
-00000e60: 2020 2020 7b25 206c 6f61 645f 626c 6f63      {% load_bloc
-00000e70: 6b73 2073 6563 7469 6f6e 3d27 6261 6e6e  ks section='bann
-00000e80: 6572 2720 257d 0a20 2020 207b 2520 656e  er' %}.    {% en
-00000e90: 6462 6c6f 636b 2062 616e 6e65 7220 257d  dblock banner %}
-00000ea0: 0a20 2020 203c 212d 2d20 656e 6420 4d61  .    <!-- end Ma
-00000eb0: 696e 2042 616e 6e65 722d 2d3e 0a0a 2020  in Banner-->..  
-00000ec0: 2020 3c21 2d2d 204d 656e 7520 322d 2d3e    <!-- Menu 2-->
-00000ed0: 0a20 2020 207b 2520 626c 6f63 6b20 6d65  .    {% block me
-00000ee0: 6e75 2d32 2025 7d0a 2020 2020 2020 2020  nu-2 %}.        
-00000ef0: 7b25 206c 6f61 645f 626c 6f63 6b73 2073  {% load_blocks s
-00000f00: 6563 7469 6f6e 3d27 6d65 6e75 2d32 2720  ection='menu-2' 
-00000f10: 257d 0a20 2020 207b 2520 656e 6462 6c6f  %}.    {% endblo
-00000f20: 636b 206d 656e 752d 3220 257d 0a20 2020  ck menu-2 %}.   
-00000f30: 203c 212d 2d20 656e 6420 4d65 6e75 2032   <!-- end Menu 2
-00000f40: 2d2d 3e0a 0a20 2020 203c 212d 2d20 4272  -->..    <!-- Br
-00000f50: 6561 6463 7275 6d62 7320 2d2d 3e0a 2020  eadcrumbs -->.  
-00000f60: 2020 7b25 2062 6c6f 636b 2062 7265 6164    {% block bread
-00000f70: 6372 756d 6273 2025 7d0a 2020 2020 2020  crumbs %}.      
-00000f80: 2020 7b25 206c 6f61 645f 626c 6f63 6b73    {% load_blocks
-00000f90: 2073 6563 7469 6f6e 3d22 6272 6561 6463   section="breadc
-00000fa0: 7275 6d62 7322 2025 7d0a 2020 2020 7b25  rumbs" %}.    {%
-00000fb0: 2065 6e64 626c 6f63 6b20 6272 6561 6463   endblock breadc
-00000fc0: 7275 6d62 7320 257d 0a20 2020 203c 212d  rumbs %}.    <!-
-00000fd0: 2d20 656e 6420 4272 6561 6463 7275 6d62  - end Breadcrumb
-00000fe0: 7320 2d2d 3e0a 0a20 2020 203c 212d 2d20  s -->..    <!-- 
-00000ff0: 5365 6374 696f 6e20 3120 2d2d 3e0a 2020  Section 1 -->.  
-00001000: 2020 7b25 2062 6c6f 636b 2073 6563 7469    {% block secti
-00001010: 6f6e 5f31 2025 7d0a 2020 2020 7b25 2062  on_1 %}.    {% b
-00001020: 6c6f 636b 735f 696e 5f70 6f73 6974 696f  locks_in_positio
-00001030: 6e20 7365 6374 696f 6e3d 2273 6563 7469  n section="secti
-00001040: 6f6e 2d31 2220 6173 2073 6563 7469 6f6e  on-1" as section
-00001050: 5f31 2025 7d0a 2020 2020 7b25 2069 6620  _1 %}.    {% if 
-00001060: 7365 6374 696f 6e5f 3120 257d 0a20 2020  section_1 %}.   
-00001070: 2020 2020 207b 2520 6c6f 6164 5f62 6c6f       {% load_blo
-00001080: 636b 7320 7365 6374 696f 6e3d 2231 2d74  cks section="1-t
-00001090: 6f70 2d61 2220 6173 2031 5f74 6f70 5f61  op-a" as 1_top_a
-000010a0: 2025 7d0a 2020 2020 2020 2020 7b25 206c   %}.        {% l
-000010b0: 6f61 645f 626c 6f63 6b73 2073 6563 7469  oad_blocks secti
-000010c0: 6f6e 3d22 312d 746f 702d 6222 2061 7320  on="1-top-b" as 
-000010d0: 315f 746f 705f 6220 257d 0a20 2020 2020  1_top_b %}.     
-000010e0: 2020 207b 2520 6c6f 6164 5f62 6c6f 636b     {% load_block
-000010f0: 7320 7365 6374 696f 6e3d 2231 2d74 6f70  s section="1-top
-00001100: 2d63 2220 6173 2031 5f74 6f70 5f63 2025  -c" as 1_top_c %
-00001110: 7d0a 0a20 2020 2020 2020 207b 2520 6c6f  }..        {% lo
-00001120: 6164 5f62 6c6f 636b 7320 7365 6374 696f  ad_blocks sectio
-00001130: 6e3d 2231 2d6d 6964 2d74 6f70 2d61 2220  n="1-mid-top-a" 
-00001140: 6173 2031 5f6d 6964 5f74 6f70 5f61 2025  as 1_mid_top_a %
-00001150: 7d0a 2020 2020 2020 2020 7b25 206c 6f61  }.        {% loa
-00001160: 645f 626c 6f63 6b73 2073 6563 7469 6f6e  d_blocks section
-00001170: 3d22 312d 6d69 642d 746f 702d 6222 2061  ="1-mid-top-b" a
-00001180: 7320 315f 6d69 645f 746f 705f 6220 257d  s 1_mid_top_b %}
-00001190: 0a20 2020 2020 2020 207b 2520 6c6f 6164  .        {% load
-000011a0: 5f62 6c6f 636b 7320 7365 6374 696f 6e3d  _blocks section=
-000011b0: 2231 2d6d 6964 2d74 6f70 2d63 2220 6173  "1-mid-top-c" as
-000011c0: 2031 5f6d 6964 5f74 6f70 5f63 2025 7d0a   1_mid_top_c %}.
-000011d0: 0a20 2020 2020 2020 207b 2520 6c6f 6164  .        {% load
-000011e0: 5f62 6c6f 636b 7320 7365 6374 696f 6e3d  _blocks section=
-000011f0: 2231 2d6c 6566 742d 6122 2061 7320 315f  "1-left-a" as 1_
-00001200: 6c65 6674 5f61 2025 7d0a 2020 2020 2020  left_a %}.      
-00001210: 2020 7b25 206c 6f61 645f 626c 6f63 6b73    {% load_blocks
-00001220: 2073 6563 7469 6f6e 3d22 312d 6c65 6674   section="1-left
-00001230: 2d62 2220 6173 2031 5f6c 6566 745f 6220  -b" as 1_left_b 
-00001240: 257d 0a0a 2020 2020 2020 2020 7b25 206c  %}..        {% l
-00001250: 6f61 645f 626c 6f63 6b73 2073 6563 7469  oad_blocks secti
-00001260: 6f6e 3d22 312d 6365 6e74 6572 2d74 6f70  on="1-center-top
-00001270: 2d61 2220 6173 2031 5f63 656e 7465 725f  -a" as 1_center_
-00001280: 746f 705f 6120 257d 0a20 2020 2020 2020  top_a %}.       
-00001290: 207b 2520 6c6f 6164 5f62 6c6f 636b 7320   {% load_blocks 
-000012a0: 7365 6374 696f 6e3d 2231 2d63 656e 7465  section="1-cente
-000012b0: 722d 746f 702d 6222 2061 7320 315f 6365  r-top-b" as 1_ce
-000012c0: 6e74 6572 5f74 6f70 5f62 2025 7d0a 2020  nter_top_b %}.  
-000012d0: 2020 2020 2020 7b25 206c 6f61 645f 626c        {% load_bl
-000012e0: 6f63 6b73 2073 6563 7469 6f6e 3d22 312d  ocks section="1-
-000012f0: 6365 6e74 6572 2d74 6f70 2d63 2220 6173  center-top-c" as
-00001300: 2031 5f63 656e 7465 725f 746f 705f 6320   1_center_top_c 
-00001310: 257d 0a0a 2020 2020 2020 2020 7b25 206c  %}..        {% l
-00001320: 6f61 645f 626c 6f63 6b73 2073 6563 7469  oad_blocks secti
-00001330: 6f6e 3d22 312d 6365 6e74 6572 2d6d 6964  on="1-center-mid
-00001340: 2d74 6f70 2d61 2220 6173 2031 5f63 656e  -top-a" as 1_cen
-00001350: 7465 725f 6d69 645f 746f 705f 6120 257d  ter_mid_top_a %}
-00001360: 0a20 2020 2020 2020 207b 2520 6c6f 6164  .        {% load
-00001370: 5f62 6c6f 636b 7320 7365 6374 696f 6e3d  _blocks section=
-00001380: 2231 2d63 656e 7465 722d 6d69 642d 746f  "1-center-mid-to
-00001390: 702d 6222 2061 7320 315f 6365 6e74 6572  p-b" as 1_center
-000013a0: 5f6d 6964 5f74 6f70 5f62 2025 7d0a 2020  _mid_top_b %}.  
-000013b0: 2020 2020 2020 7b25 206c 6f61 645f 626c        {% load_bl
-000013c0: 6f63 6b73 2073 6563 7469 6f6e 3d22 312d  ocks section="1-
-000013d0: 6365 6e74 6572 2d6d 6964 2d74 6f70 2d63  center-mid-top-c
-000013e0: 2220 6173 2031 5f63 656e 7465 725f 6d69  " as 1_center_mi
-000013f0: 645f 746f 705f 6320 257d 0a0a 2020 2020  d_top_c %}..    
-00001400: 2020 2020 7b25 206c 6f61 645f 626c 6f63      {% load_bloc
-00001410: 6b73 2073 6563 7469 6f6e 3d22 312d 6365  ks section="1-ce
-00001420: 6e74 6572 2d63 6f6e 7465 6e74 2220 6173  nter-content" as
-00001430: 2031 5f63 656e 7465 725f 636f 6e74 656e   1_center_conten
-00001440: 7420 257d 0a0a 2020 2020 2020 2020 7b25  t %}..        {%
-00001450: 206c 6f61 645f 626c 6f63 6b73 2073 6563   load_blocks sec
-00001460: 7469 6f6e 3d22 312d 6365 6e74 6572 2d6d  tion="1-center-m
-00001470: 6964 2d62 6f74 746f 6d2d 6122 2061 7320  id-bottom-a" as 
-00001480: 315f 6365 6e74 6572 5f6d 6964 5f62 6f74  1_center_mid_bot
-00001490: 746f 6d5f 6120 257d 0a20 2020 2020 2020  tom_a %}.       
-000014a0: 207b 2520 6c6f 6164 5f62 6c6f 636b 7320   {% load_blocks 
-000014b0: 7365 6374 696f 6e3d 2231 2d63 656e 7465  section="1-cente
-000014c0: 722d 6d69 642d 626f 7474 6f6d 2d62 2220  r-mid-bottom-b" 
-000014d0: 6173 2031 5f63 656e 7465 725f 6d69 645f  as 1_center_mid_
-000014e0: 626f 7474 6f6d 5f62 2025 7d0a 2020 2020  bottom_b %}.    
-000014f0: 2020 2020 7b25 206c 6f61 645f 626c 6f63      {% load_bloc
-00001500: 6b73 2073 6563 7469 6f6e 3d22 312d 6365  ks section="1-ce
-00001510: 6e74 6572 2d6d 6964 2d62 6f74 746f 6d2d  nter-mid-bottom-
-00001520: 6322 2061 7320 315f 6365 6e74 6572 5f6d  c" as 1_center_m
-00001530: 6964 5f62 6f74 746f 6d5f 6320 257d 0a0a  id_bottom_c %}..
-00001540: 2020 2020 2020 2020 7b25 206c 6f61 645f          {% load_
-00001550: 626c 6f63 6b73 2073 6563 7469 6f6e 3d22  blocks section="
-00001560: 312d 6365 6e74 6572 2d62 6f74 746f 6d2d  1-center-bottom-
-00001570: 6122 2061 7320 315f 6365 6e74 6572 5f62  a" as 1_center_b
-00001580: 6f74 746f 6d5f 6120 257d 0a20 2020 2020  ottom_a %}.     
-00001590: 2020 207b 2520 6c6f 6164 5f62 6c6f 636b     {% load_block
-000015a0: 7320 7365 6374 696f 6e3d 2231 2d63 656e  s section="1-cen
-000015b0: 7465 722d 626f 7474 6f6d 2d62 2220 6173  ter-bottom-b" as
-000015c0: 2031 5f63 656e 7465 725f 626f 7474 6f6d   1_center_bottom
-000015d0: 5f62 2025 7d0a 2020 2020 2020 2020 7b25  _b %}.        {%
-000015e0: 206c 6f61 645f 626c 6f63 6b73 2073 6563   load_blocks sec
-000015f0: 7469 6f6e 3d22 312d 6365 6e74 6572 2d62  tion="1-center-b
-00001600: 6f74 746f 6d2d 6322 2061 7320 315f 6365  ottom-c" as 1_ce
-00001610: 6e74 6572 5f62 6f74 746f 6d5f 6320 257d  nter_bottom_c %}
-00001620: 0a0a 2020 2020 2020 2020 7b25 206c 6f61  ..        {% loa
-00001630: 645f 626c 6f63 6b73 2073 6563 7469 6f6e  d_blocks section
-00001640: 3d22 312d 7269 6768 742d 6122 2061 7320  ="1-right-a" as 
-00001650: 315f 7269 6768 745f 6120 257d 0a20 2020  1_right_a %}.   
-00001660: 2020 2020 207b 2520 6c6f 6164 5f62 6c6f       {% load_blo
-00001670: 636b 7320 7365 6374 696f 6e3d 2231 2d72  cks section="1-r
-00001680: 6967 6874 2d62 2220 6173 2031 5f72 6967  ight-b" as 1_rig
-00001690: 6874 5f62 2025 7d0a 0a20 2020 2020 2020  ht_b %}..       
-000016a0: 207b 2520 6c6f 6164 5f62 6c6f 636b 7320   {% load_blocks 
-000016b0: 7365 6374 696f 6e3d 2231 2d6d 6964 2d62  section="1-mid-b
-000016c0: 6f74 746f 6d2d 6122 2061 7320 315f 6d69  ottom-a" as 1_mi
-000016d0: 645f 626f 7474 6f6d 5f61 2025 7d0a 2020  d_bottom_a %}.  
-000016e0: 2020 2020 2020 7b25 206c 6f61 645f 626c        {% load_bl
-000016f0: 6f63 6b73 2073 6563 7469 6f6e 3d22 312d  ocks section="1-
-00001700: 6d69 642d 626f 7474 6f6d 2d62 2220 6173  mid-bottom-b" as
-00001710: 2031 5f6d 6964 5f62 6f74 746f 6d5f 6220   1_mid_bottom_b 
-00001720: 257d 0a20 2020 2020 2020 207b 2520 6c6f  %}.        {% lo
-00001730: 6164 5f62 6c6f 636b 7320 7365 6374 696f  ad_blocks sectio
-00001740: 6e3d 2231 2d6d 6964 2d62 6f74 746f 6d2d  n="1-mid-bottom-
-00001750: 6322 2061 7320 315f 6d69 645f 626f 7474  c" as 1_mid_bott
-00001760: 6f6d 5f63 2025 7d0a 0a20 2020 2020 2020  om_c %}..       
-00001770: 207b 2520 6c6f 6164 5f62 6c6f 636b 7320   {% load_blocks 
-00001780: 7365 6374 696f 6e3d 2231 2d62 6f74 746f  section="1-botto
-00001790: 6d2d 6122 2061 7320 315f 626f 7474 6f6d  m-a" as 1_bottom
-000017a0: 5f61 2025 7d0a 2020 2020 2020 2020 7b25  _a %}.        {%
-000017b0: 206c 6f61 645f 626c 6f63 6b73 2073 6563   load_blocks sec
-000017c0: 7469 6f6e 3d22 312d 626f 7474 6f6d 2d62  tion="1-bottom-b
-000017d0: 2220 6173 2031 5f62 6f74 746f 6d5f 6220  " as 1_bottom_b 
-000017e0: 257d 0a20 2020 2020 2020 207b 2520 6c6f  %}.        {% lo
-000017f0: 6164 5f62 6c6f 636b 7320 7365 6374 696f  ad_blocks sectio
-00001800: 6e3d 2231 2d62 6f74 746f 6d2d 6322 2061  n="1-bottom-c" a
-00001810: 7320 315f 626f 7474 6f6d 5f63 2025 7d0a  s 1_bottom_c %}.
-00001820: 0a20 2020 2020 2020 203c 6469 7620 636c  .        <div cl
-00001830: 6173 733d 227b 2520 626c 6f63 6b20 7365  ass="{% block se
-00001840: 6374 696f 6e5f 315f 636c 6173 7365 7320  ction_1_classes 
-00001850: 257d 7079 2d35 7b25 2065 6e64 626c 6f63  %}py-5{% endbloc
-00001860: 6b20 257d 223e 0a20 2020 2020 2020 2020  k %}">.         
-00001870: 2020 203c 6469 7620 636c 6173 733d 2263     <div class="c
-00001880: 6f6e 7461 696e 6572 223e 0a20 2020 2020  ontainer">.     
-00001890: 2020 2020 2020 2020 2020 203c 6469 7620             <div 
-000018a0: 636c 6173 733d 2272 6f77 206d 782d 3022  class="row mx-0"
-000018b0: 3e0a 0a20 2020 2020 2020 2020 2020 2020  >..             
-000018c0: 2020 2020 2020 203c 212d 2d20 546f 7020         <!-- Top 
-000018d0: 2d2d 3e0a 2020 2020 2020 2020 2020 2020  -->.            
-000018e0: 2020 2020 2020 2020 7b25 2069 6620 315f          {% if 1_
-000018f0: 746f 705f 6120 6f72 2031 5f74 6f70 5f62  top_a or 1_top_b
-00001900: 206f 7220 315f 746f 705f 6320 257d 0a20   or 1_top_c %}. 
-00001910: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001920: 2020 203c 6469 7620 636c 6173 733d 2263     <div class="c
-00001930: 6f6c 2d31 3222 3e0a 2020 2020 2020 2020  ol-12">.        
-00001940: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001950: 3c64 6976 2063 6c61 7373 3d22 726f 7722  <div class="row"
-00001960: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
-00001970: 2020 2020 2020 2020 2020 2020 2020 7b25                {%
-00001980: 2069 6620 315f 746f 705f 6120 616e 6420   if 1_top_a and 
-00001990: 315f 746f 705f 6220 616e 6420 315f 746f  1_top_b and 1_to
-000019a0: 705f 6320 257d 0a20 2020 2020 2020 2020  p_c %}.         
-000019b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000019c0: 2020 2020 2020 203c 6469 7620 636c 6173         <div clas
-000019d0: 733d 227b 2520 626c 6f63 6b20 315f 746f  s="{% block 1_to
-000019e0: 705f 6162 635f 6120 257d 636f 6c2d 3132  p_abc_a %}col-12
-000019f0: 2063 6f6c 2d6d 642d 347b 2520 656e 6462   col-md-4{% endb
-00001a00: 6c6f 636b 2025 7d22 3e7b 7b20 315f 746f  lock %}">{{ 1_to
-00001a10: 705f 6120 7d7d 3c2f 6469 763e 0a20 2020  p_a }}</div>.   
-00001a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001a30: 2020 2020 2020 2020 2020 2020 203c 6469               <di
-00001a40: 7620 636c 6173 733d 227b 2520 626c 6f63  v class="{% bloc
-00001a50: 6b20 315f 746f 705f 6162 635f 6220 257d  k 1_top_abc_b %}
-00001a60: 636f 6c2d 3132 2063 6f6c 2d6d 642d 347b  col-12 col-md-4{
-00001a70: 2520 656e 6462 6c6f 636b 2025 7d22 3e7b  % endblock %}">{
-00001a80: 7b20 315f 746f 705f 6220 7d7d 3c2f 6469  { 1_top_b }}</di
-00001a90: 763e 0a20 2020 2020 2020 2020 2020 2020  v>.             
-00001aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001ab0: 2020 203c 6469 7620 636c 6173 733d 227b     <div class="{
-00001ac0: 2520 626c 6f63 6b20 315f 746f 705f 6162  % block 1_top_ab
-00001ad0: 635f 6320 257d 636f 6c2d 3132 2063 6f6c  c_c %}col-12 col
-00001ae0: 2d6d 642d 347b 2520 656e 6462 6c6f 636b  -md-4{% endblock
-00001af0: 2025 7d22 3e7b 7b20 315f 746f 705f 6320   %}">{{ 1_top_c 
-00001b00: 7d7d 3c2f 6469 763e 0a20 2020 2020 2020  }}</div>.       
-00001b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001b20: 2020 2020 207b 2520 656c 6966 2031 5f74       {% elif 1_t
-00001b30: 6f70 5f61 2061 6e64 2031 5f74 6f70 5f62  op_a and 1_top_b
-00001b40: 2025 7d0a 2020 2020 2020 2020 2020 2020   %}.            
-00001b50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001b60: 2020 2020 3c64 6976 2063 6c61 7373 3d22      <div class="
-00001b70: 7b25 2062 6c6f 636b 2031 5f74 6f70 5f61  {% block 1_top_a
-00001b80: 625f 6120 257d 636f 6c2d 3132 2063 6f6c  b_a %}col-12 col
-00001b90: 2d6d 642d 387b 2520 656e 6462 6c6f 636b  -md-8{% endblock
-00001ba0: 2025 7d22 3e7b 7b20 315f 746f 705f 6120   %}">{{ 1_top_a 
-00001bb0: 7d7d 3c2f 6469 763e 0a20 2020 2020 2020  }}</div>.       
-00001bc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001bd0: 2020 2020 2020 2020 203c 6469 7620 636c           <div cl
-00001be0: 6173 733d 227b 2520 626c 6f63 6b20 315f  ass="{% block 1_
-00001bf0: 746f 705f 6162 5f62 2025 7d63 6f6c 2d31  top_ab_b %}col-1
-00001c00: 3220 636f 6c2d 6d64 2d34 7b25 2065 6e64  2 col-md-4{% end
-00001c10: 626c 6f63 6b20 257d 223e 7b7b 2031 5f74  block %}">{{ 1_t
-00001c20: 6f70 5f62 207d 7d3c 2f64 6976 3e0a 2020  op_b }}</div>.  
-00001c30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001c40: 2020 2020 2020 2020 2020 7b25 2065 6c69            {% eli
-00001c50: 6620 315f 746f 705f 6120 616e 6420 315f  f 1_top_a and 1_
-00001c60: 746f 705f 6320 257d 0a20 2020 2020 2020  top_c %}.       
-00001c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001c80: 2020 2020 2020 2020 203c 6469 7620 636c           <div cl
-00001c90: 6173 733d 227b 2520 626c 6f63 6b20 315f  ass="{% block 1_
-00001ca0: 746f 705f 6163 5f61 2025 7d63 6f6c 2d31  top_ac_a %}col-1
-00001cb0: 3220 636f 6c2d 6d64 2d36 7b25 2065 6e64  2 col-md-6{% end
-00001cc0: 626c 6f63 6b20 257d 223e 7b7b 2031 5f74  block %}">{{ 1_t
-00001cd0: 6f70 5f61 207d 7d3c 2f64 6976 3e0a 2020  op_a }}</div>.  
-00001ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001cf0: 2020 2020 2020 2020 2020 2020 2020 3c64                <d
-00001d00: 6976 2063 6c61 7373 3d22 7b25 2062 6c6f  iv class="{% blo
-00001d10: 636b 2031 5f74 6f70 5f61 635f 6320 257d  ck 1_top_ac_c %}
-00001d20: 636f 6c2d 3132 2063 6f6c 2d6d 642d 367b  col-12 col-md-6{
-00001d30: 2520 656e 6462 6c6f 636b 2025 7d22 3e7b  % endblock %}">{
-00001d40: 7b20 315f 746f 705f 6320 7d7d 3c2f 6469  { 1_top_c }}</di
-00001d50: 763e 0a20 2020 2020 2020 2020 2020 2020  v>.             
-00001d60: 2020 2020 2020 2020 2020 2020 2020 207b                 {
-00001d70: 2520 656c 6966 2031 5f74 6f70 5f62 2061  % elif 1_top_b a
-00001d80: 6e64 2031 5f74 6f70 5f63 2025 7d0a 2020  nd 1_top_c %}.  
-00001d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001da0: 2020 2020 2020 2020 2020 2020 2020 3c64                <d
-00001db0: 6976 2063 6c61 7373 3d22 7b25 2062 6c6f  iv class="{% blo
-00001dc0: 636b 2031 5f74 6f70 5f62 635f 6220 257d  ck 1_top_bc_b %}
-00001dd0: 636f 6c2d 3132 2063 6f6c 2d6d 642d 347b  col-12 col-md-4{
-00001de0: 2520 656e 6462 6c6f 636b 2025 7d22 3e7b  % endblock %}">{
-00001df0: 7b20 315f 746f 705f 6220 7d7d 3c2f 6469  { 1_top_b }}</di
-00001e00: 763e 0a20 2020 2020 2020 2020 2020 2020  v>.             
-00001e10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001e20: 2020 203c 6469 7620 636c 6173 733d 227b     <div class="{
-00001e30: 2520 626c 6f63 6b20 315f 746f 705f 6263  % block 1_top_bc
-00001e40: 5f63 2025 7d63 6f6c 2d31 3220 636f 6c2d  _c %}col-12 col-
-00001e50: 6d64 2d38 7b25 2065 6e64 626c 6f63 6b20  md-8{% endblock 
-00001e60: 257d 223e 7b7b 2031 5f74 6f70 5f63 207d  %}">{{ 1_top_c }
-00001e70: 7d3c 2f64 6976 3e0a 2020 2020 2020 2020  }</div>.        
-00001e80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001e90: 2020 2020 7b25 2065 6c73 6520 257d 0a20      {% else %}. 
+00000340: 6572 207d 7d0a 0a20 2020 207b 2520 626c  er }}..    {% bl
+00000350: 6f63 6b20 6865 6164 5f69 6e69 7473 2025  ock head_inits %
+00000360: 7d0a 2020 2020 2020 2020 7b25 2069 6e63  }.        {% inc
+00000370: 6c75 6465 2022 696e 6974 732f 7675 652d  lude "inits/vue-
+00000380: 696e 6974 2e68 746d 6c22 2025 7d0a 2020  init.html" %}.  
+00000390: 2020 2020 2020 7b25 2069 6e63 6c75 6465        {% include
+000003a0: 2022 696e 6974 732f 6f77 6c2d 6361 726f   "inits/owl-caro
+000003b0: 7573 656c 2d69 6e69 742e 6874 6d6c 2220  usel-init.html" 
+000003c0: 257d 0a20 2020 207b 2520 656e 6462 6c6f  %}.    {% endblo
+000003d0: 636b 2068 6561 645f 696e 6974 7320 257d  ck head_inits %}
+000003e0: 0a0a 2020 2020 7b25 2062 6c6f 636b 2068  ..    {% block h
+000003f0: 746d 6c5f 6865 6164 2025 7d0a 2020 2020  tml_head %}.    
+00000400: 2020 2020 7b25 206c 6f61 645f 626c 6f63      {% load_bloc
+00000410: 6b73 2073 6563 7469 6f6e 3d22 6874 6d6c  ks section="html
+00000420: 2d68 6561 6422 2061 7320 6874 6d6c 5f68  -head" as html_h
+00000430: 6561 6420 257d 0a20 2020 2020 2020 207b  ead %}.        {
+00000440: 7b20 6874 6d6c 5f68 6561 6420 7d7d 0a20  { html_head }}. 
+00000450: 2020 207b 2520 656e 6462 6c6f 636b 2068     {% endblock h
+00000460: 746d 6c5f 6865 6164 2025 7d0a 0a20 2020  tml_head %}..   
+00000470: 207b 2520 626c 6f63 6b20 736f 6369 616c   {% block social
+00000480: 5f74 6167 7320 257d 0a20 2020 203c 6d65  _tags %}.    <me
+00000490: 7461 2070 726f 7065 7274 793d 226f 673a  ta property="og:
+000004a0: 7572 6c22 2063 6f6e 7465 6e74 3d22 7b7b  url" content="{{
+000004b0: 2072 6571 7565 7374 2e62 7569 6c64 5f61   request.build_a
+000004c0: 6273 6f6c 7574 655f 7572 6920 7d7d 2220  bsolute_uri }}" 
+000004d0: 2f3e 0a20 2020 203c 6d65 7461 2070 726f  />.    <meta pro
+000004e0: 7065 7274 793d 226f 673a 7479 7065 2220  perty="og:type" 
+000004f0: 636f 6e74 656e 743d 2261 7274 6963 6c65  content="article
+00000500: 2220 2f3e 0a20 2020 203c 6d65 7461 2070  " />.    <meta p
+00000510: 726f 7065 7274 793d 226f 673a 7469 746c  roperty="og:titl
+00000520: 6522 2063 6f6e 7465 6e74 3d22 7b7b 2070  e" content="{{ p
+00000530: 6167 652e 7469 746c 6520 7d7d 2220 2f3e  age.title }}" />
+00000540: 0a20 2020 203c 6d65 7461 2070 726f 7065  .    <meta prope
+00000550: 7274 793d 226f 673a 6465 7363 7269 7074  rty="og:descript
+00000560: 696f 6e22 2063 6f6e 7465 6e74 3d22 7b7b  ion" content="{{
+00000570: 2070 6167 652e 6465 7363 7269 7074 696f   page.descriptio
+00000580: 6e20 7d7d 2220 2f3e 0a20 2020 203c 6d65  n }}" />.    <me
+00000590: 7461 2070 726f 7065 7274 793d 226f 673a  ta property="og:
+000005a0: 696d 6167 6522 2063 6f6e 7465 6e74 3d22  image" content="
+000005b0: 6874 7470 733a 2f2f 7b7b 2072 6571 7565  https://{{ reque
+000005c0: 7374 2e67 6574 5f68 6f73 7420 7d7d 2f73  st.get_host }}/s
+000005d0: 7461 7469 632f 696d 6167 6573 2f6c 6f67  tatic/images/log
+000005e0: 6f2e 706e 6722 3e0a 2020 2020 3c6d 6574  o.png">.    <met
+000005f0: 6120 7072 6f70 6572 7479 3d22 6f67 3a69  a property="og:i
+00000600: 6d61 6765 3a61 6c74 2220 636f 6e74 656e  mage:alt" conten
+00000610: 743d 227b 7b20 7061 6765 2e74 6974 6c65  t="{{ page.title
+00000620: 207d 7d22 202f 3e0a 2020 2020 3c6d 6574   }}" />.    <met
+00000630: 6120 7072 6f70 6572 7479 3d22 6f67 3a69  a property="og:i
+00000640: 6d61 6765 3a77 6964 7468 2220 636f 6e74  mage:width" cont
+00000650: 656e 743d 2233 3330 2220 2f3e 0a20 2020  ent="330" />.   
+00000660: 203c 6d65 7461 2070 726f 7065 7274 793d   <meta property=
+00000670: 226f 673a 696d 6167 653a 6865 6967 6874  "og:image:height
+00000680: 2220 636f 6e74 656e 743d 2233 3330 2220  " content="330" 
+00000690: 2f3e 0a0a 2020 2020 3c6d 6574 6120 6e61  />..    <meta na
+000006a0: 6d65 3d22 7477 6974 7465 723a 6361 7264  me="twitter:card
+000006b0: 2220 636f 6e74 656e 743d 2273 756d 6d61  " content="summa
+000006c0: 7279 5f6c 6172 6765 5f69 6d61 6765 223e  ry_large_image">
+000006d0: 0a20 2020 203c 6d65 7461 206e 616d 653d  .    <meta name=
+000006e0: 2274 7769 7474 6572 3a74 6974 6c65 2220  "twitter:title" 
+000006f0: 636f 6e74 656e 743d 227b 7b20 7061 6765  content="{{ page
+00000700: 2e74 6974 6c65 207d 7d22 3e0a 2020 2020  .title }}">.    
+00000710: 3c6d 6574 6120 6e61 6d65 3d22 7477 6974  <meta name="twit
+00000720: 7465 723a 6465 7363 7269 7074 696f 6e22  ter:description"
+00000730: 2063 6f6e 7465 6e74 3d22 7b7b 2070 6167   content="{{ pag
+00000740: 652e 6465 7363 7269 7074 696f 6e20 7d7d  e.description }}
+00000750: 223e 0a20 2020 203c 6d65 7461 206e 616d  ">.    <meta nam
+00000760: 653d 2274 7769 7474 6572 3a69 6d61 6765  e="twitter:image
+00000770: 2220 636f 6e74 656e 743d 2268 7474 7073  " content="https
+00000780: 3a2f 2f7b 7b20 7265 7175 6573 742e 6765  ://{{ request.ge
+00000790: 745f 686f 7374 207d 7d2f 7374 6174 6963  t_host }}/static
+000007a0: 2f69 6d61 6765 732f 6c6f 676f 2e70 6e67  /images/logo.png
+000007b0: 223e 0a20 2020 203c 6d65 7461 206e 616d  ">.    <meta nam
+000007c0: 653d 2274 7769 7474 6572 3a69 6d61 6765  e="twitter:image
+000007d0: 3a61 6c74 2220 636f 6e74 656e 743d 227b  :alt" content="{
+000007e0: 7b20 7061 6765 2e74 6974 6c65 207d 7d22  { page.title }}"
+000007f0: 3e0a 2020 2020 7b25 2065 6e64 626c 6f63  >.    {% endbloc
+00000800: 6b20 736f 6369 616c 5f74 6167 7320 257d  k social_tags %}
+00000810: 0a7b 2520 656e 6462 6c6f 636b 2065 7874  .{% endblock ext
+00000820: 7261 5f68 6561 6420 257d 0a0a 3c21 2d2d  ra_head %}..<!--
+00000830: 2050 6167 6520 5469 746c 6520 2d2d 3e0a   Page Title -->.
+00000840: 3c21 2d2d 2050 6167 6520 5469 746c 6520  <!-- Page Title 
+00000850: 2d2d 3e0a 7b25 2062 6c6f 636b 2070 6167  -->.{% block pag
+00000860: 655f 7469 746c 6520 257d 0a20 2020 207b  e_title %}.    {
+00000870: 2520 6966 2070 6167 6520 257d 0a20 2020  % if page %}.   
+00000880: 2020 2020 207b 7b20 7061 6765 2e74 6974       {{ page.tit
+00000890: 6c65 207d 7d20 2d20 7b7b 2077 6562 7369  le }} - {{ websi
+000008a0: 7465 2e6e 616d 6520 7d7d 0a20 2020 207b  te.name }}.    {
+000008b0: 2520 656c 7365 2025 7d0a 2020 2020 2020  % else %}.      
+000008c0: 2020 7b25 2074 7261 6e73 2022 556e 6976    {% trans "Univ
+000008d0: 6572 7369 7479 206f 6620 4361 6c61 6272  ersity of Calabr
+000008e0: 6961 2220 257d 0a20 2020 207b 2520 656e  ia" %}.    {% en
+000008f0: 6469 6620 257d 0a7b 2520 656e 6462 6c6f  dif %}.{% endblo
+00000900: 636b 2070 6167 655f 7469 746c 6520 257d  ck page_title %}
+00000910: 0a0a 3c21 2d2d 2048 6561 6465 7220 736c  ..<!-- Header sl
+00000920: 696d 2077 7261 7070 6572 202d 2d3e 0a7b  im wrapper -->.{
+00000930: 2520 626c 6f63 6b20 6865 6164 6572 5f73  % block header_s
+00000940: 6c69 6d5f 746f 705f 6c65 6674 2025 7d0a  lim_top_left %}.
+00000950: 7b25 2069 6620 7265 7175 6573 742e 7573  {% if request.us
+00000960: 6572 2e69 735f 7374 6166 6620 257d 0a7b  er.is_staff %}.{
+00000970: 2520 696e 636c 7564 6520 2263 6f6d 706f  % include "compo
+00000980: 6e65 6e74 732f 6974 616c 6961 5f65 6469  nents/italia_edi
+00000990: 746f 7269 616c 626f 6172 645f 6672 6f6e  torialboard_fron
+000009a0: 7465 6e64 5f6d 656e 752e 6874 6d6c 2220  tend_menu.html" 
+000009b0: 257d 0a7b 2520 656e 6469 6620 257d 0a7b  %}.{% endif %}.{
+000009c0: 2520 656e 6462 6c6f 636b 2068 6561 6465  % endblock heade
+000009d0: 725f 736c 696d 5f74 6f70 5f6c 6566 7420  r_slim_top_left 
+000009e0: 257d 0a0a 7b25 2062 6c6f 636b 2068 6561  %}..{% block hea
+000009f0: 6465 725f 736c 696d 5f73 7562 5f6d 656e  der_slim_sub_men
+00000a00: 7520 257d 0a3c 6469 7620 636c 6173 733d  u %}.<div class=
+00000a10: 226e 6176 2d69 7465 6d20 6472 6f70 646f  "nav-item dropdo
+00000a20: 776e 223e 0a20 2020 203c 6120 636c 6173  wn">.    <a clas
+00000a30: 733d 226e 6176 2d6c 696e 6b20 6472 6f70  s="nav-link drop
+00000a40: 646f 776e 2d74 6f67 676c 6522 0a20 2020  down-toggle".   
+00000a50: 2020 2020 6872 6566 3d22 2322 0a20 2020      href="#".   
+00000a60: 2020 2020 6461 7461 2d74 6f67 676c 653d      data-toggle=
+00000a70: 2264 726f 7064 6f77 6e22 0a20 2020 2020  "dropdown".     
+00000a80: 2020 6172 6961 2d65 7870 616e 6465 643d    aria-expanded=
+00000a90: 2266 616c 7365 223e 0a20 2020 2020 2020  "false">.       
+00000aa0: 203c 7370 616e 3e7b 7b20 7265 7175 6573   <span>{{ reques
+00000ab0: 742e 4c41 4e47 5541 4745 5f43 4f44 4520  t.LANGUAGE_CODE 
+00000ac0: 7d7d 3c2f 7370 616e 3e0a 2020 2020 2020  }}</span>.      
+00000ad0: 2020 3c73 7667 2063 6c61 7373 3d22 6963    <svg class="ic
+00000ae0: 6f6e 2064 2d6e 6f6e 6520 642d 6c67 2d62  on d-none d-lg-b
+00000af0: 6c6f 636b 223e 0a20 2020 2020 2020 2020  lock">.         
+00000b00: 2020 203c 7573 6520 786c 696e 6b3a 6872     <use xlink:hr
+00000b10: 6566 3d22 7b25 2073 7461 7469 6320 2773  ef="{% static 's
+00000b20: 7667 2f73 7072 6974 6573 2e73 7667 2720  vg/sprites.svg' 
+00000b30: 257d 2369 742d 6578 7061 6e64 223e 3c2f  %}#it-expand"></
+00000b40: 7573 653e 0a20 2020 2020 2020 203c 2f73  use>.        </s
+00000b50: 7667 3e0a 2020 2020 3c2f 613e 0a20 2020  vg>.    </a>.   
+00000b60: 203c 6469 7620 636c 6173 733d 2264 726f   <div class="dro
+00000b70: 7064 6f77 6e2d 6d65 6e75 223e 0a20 2020  pdown-menu">.   
+00000b80: 2020 2020 203c 6469 7620 636c 6173 733d       <div class=
+00000b90: 2272 6f77 223e 0a20 2020 2020 2020 2020  "row">.         
+00000ba0: 2020 203c 6469 7620 636c 6173 733d 2263     <div class="c
+00000bb0: 6f6c 2d31 3222 3e0a 2020 2020 2020 2020  ol-12">.        
+00000bc0: 2020 2020 2020 2020 3c64 6976 2063 6c61          <div cla
+00000bd0: 7373 3d22 6c69 6e6b 2d6c 6973 742d 7772  ss="link-list-wr
+00000be0: 6170 7065 7222 3e0a 2020 2020 2020 2020  apper">.        
+00000bf0: 2020 2020 2020 2020 2020 2020 3c75 6c20              <ul 
+00000c00: 636c 6173 733d 226c 696e 6b2d 6c69 7374  class="link-list
+00000c10: 223e 0a20 2020 2020 2020 2020 2020 2020  ">.             
+00000c20: 2020 2020 2020 2020 2020 207b 2520 6c61             {% la
+00000c30: 6e67 7561 6765 5f6d 656e 7520 6173 206c  nguage_menu as l
+00000c40: 616e 6775 6167 655f 7572 6c73 2025 7d0a  anguage_urls %}.
+00000c50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000c60: 2020 2020 2020 2020 7b25 2066 6f72 2063          {% for c
+00000c70: 6f64 2c70 6172 616d 7320 696e 206c 616e  od,params in lan
+00000c80: 6775 6167 655f 7572 6c73 2e69 7465 6d73  guage_urls.items
+00000c90: 2025 7d0a 2020 2020 2020 2020 2020 2020   %}.            
+00000ca0: 2020 2020 2020 2020 2020 2020 3c6c 693e              <li>
+00000cb0: 3c61 2063 6c61 7373 3d22 6c69 7374 2d69  <a class="list-i
+00000cc0: 7465 6d22 2068 7265 663d 227b 7b20 7061  tem" href="{{ pa
+00000cd0: 7261 6d73 2e31 207d 7d22 3e3c 7370 616e  rams.1 }}"><span
+00000ce0: 3e7b 7b20 7061 7261 6d73 2e30 207d 7d3c  >{{ params.0 }}<
+00000cf0: 2f73 7061 6e3e 3c2f 613e 3c2f 6c69 3e0a  /span></a></li>.
+00000d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000d10: 2020 2020 2020 2020 7b25 2065 6e64 666f          {% endfo
+00000d20: 7220 257d 0a20 2020 2020 2020 2020 2020  r %}.           
+00000d30: 2020 2020 2020 2020 203c 2f75 6c3e 0a20           </ul>. 
+00000d40: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+00000d50: 2f64 6976 3e0a 2020 2020 2020 2020 2020  /div>.          
+00000d60: 2020 3c2f 6469 763e 0a20 2020 2020 2020    </div>.       
+00000d70: 203c 2f64 6976 3e0a 2020 2020 3c2f 6469   </div>.    </di
+00000d80: 763e 0a3c 2f64 6976 3e0a 7b25 2065 6e64  v>.</div>.{% end
+00000d90: 626c 6f63 6b20 6865 6164 6572 5f73 6c69  block header_sli
+00000da0: 6d5f 7375 625f 6d65 6e75 2025 7d0a 0a7b  m_sub_menu %}..{
+00000db0: 2520 626c 6f63 6b20 6865 6164 6572 5f73  % block header_s
+00000dc0: 6c69 6d5f 6275 7474 6f6e 7320 257d 0a3c  lim_buttons %}.<
+00000dd0: 6469 7620 636c 6173 733d 2269 742d 6163  div class="it-ac
+00000de0: 6365 7373 2d74 6f70 2d77 7261 7070 6572  cess-top-wrapper
+00000df0: 223e 0a20 2020 207b 2520 6966 2072 6571  ">.    {% if req
+00000e00: 7565 7374 2e75 7365 722e 6973 5f61 7574  uest.user.is_aut
+00000e10: 6865 6e74 6963 6174 6564 2025 7d0a 2020  henticated %}.  
+00000e20: 2020 3c62 7574 746f 6e20 636c 6173 733d    <button class=
+00000e30: 2262 746e 2062 746e 2d70 7269 6d61 7279  "btn btn-primary
+00000e40: 2062 746e 2d73 6d22 2068 7265 663d 227b   btn-sm" href="{
+00000e50: 2520 7572 6c20 276c 6f67 6f75 7427 2025  % url 'logout' %
+00000e60: 7d22 2074 7970 653d 2262 7574 746f 6e22  }" type="button"
+00000e70: 3e0a 2020 2020 2020 2020 7b25 2074 7261  >.        {% tra
+00000e80: 6e73 2022 4c6f 676f 7574 2220 257d 0a20  ns "Logout" %}. 
+00000e90: 2020 203c 2f62 7574 746f 6e3e 0a20 2020     </button>.   
+00000ea0: 207b 2520 656c 7365 2025 7d0a 2020 2020   {% else %}.    
+00000eb0: 3c62 7574 746f 6e20 636c 6173 733d 2262  <button class="b
+00000ec0: 746e 2062 746e 2d70 7269 6d61 7279 2062  tn btn-primary b
+00000ed0: 746e 2d73 6d22 2068 7265 663d 227b 2520  tn-sm" href="{% 
+00000ee0: 7572 6c20 276c 6f67 696e 2720 257d 2220  url 'login' %}" 
+00000ef0: 7479 7065 3d22 6275 7474 6f6e 223e 0a20  type="button">. 
+00000f00: 2020 2020 2020 207b 2520 7472 616e 7320         {% trans 
+00000f10: 224c 6f67 696e 2220 257d 0a20 2020 203c  "Login" %}.    <
+00000f20: 2f62 7574 746f 6e3e 0a20 2020 207b 2520  /button>.    {% 
+00000f30: 656e 6469 6620 257d 0a3c 2f64 6976 3e0a  endif %}.</div>.
+00000f40: 7b25 2065 6e64 626c 6f63 6b20 6865 6164  {% endblock head
+00000f50: 6572 5f73 6c69 6d5f 6275 7474 6f6e 7320  er_slim_buttons 
+00000f60: 257d 0a3c 212d 2d20 656e 6420 4865 6164  %}.<!-- end Head
+00000f70: 6572 2073 6c69 6d20 7772 6170 7065 7220  er slim wrapper 
+00000f80: 2d2d 3e0a 0a3c 212d 2d20 5552 4c20 6c69  -->..<!-- URL li
+00000f90: 6e6b 206c 6f67 6f20 616e 6420 6f72 6720  nk logo and org 
+00000fa0: 6e61 6d65 202d 2d3e 0a7b 2520 626c 6f63  name -->.{% bloc
+00000fb0: 6b20 6865 6164 6572 5f63 656e 7465 725f  k header_center_
+00000fc0: 7572 6c20 257d 0a7b 2520 7365 7474 696e  url %}.{% settin
+00000fd0: 6773 5f76 616c 7565 2022 434d 535f 5041  gs_value "CMS_PA
+00000fe0: 5448 5f50 5245 4649 5822 2061 7320 636d  TH_PREFIX" as cm
+00000ff0: 735f 7061 7468 5f70 7265 6669 7820 257d  s_path_prefix %}
+00001000: 2f7b 7b20 636d 735f 7061 7468 5f70 7265  /{{ cms_path_pre
+00001010: 6669 7820 7d7d 0a7b 2520 656e 6462 6c6f  fix }}.{% endblo
+00001020: 636b 2068 6561 6465 725f 6365 6e74 6572  ck header_center
+00001030: 5f75 726c 2025 7d0a 0a7b 2520 626c 6f63  _url %}..{% bloc
+00001040: 6b20 6865 6164 6572 5f6d 6f62 696c 655f  k header_mobile_
+00001050: 6172 726f 7720 257d 0a7b 2520 656e 6462  arrow %}.{% endb
+00001060: 6c6f 636b 2068 6561 6465 725f 6d6f 6269  lock header_mobi
+00001070: 6c65 5f61 7272 6f77 2025 7d0a 0a7b 2520  le_arrow %}..{% 
+00001080: 626c 6f63 6b20 6865 6164 6572 5f6d 6f62  block header_mob
+00001090: 696c 655f 736c 696d 5f6d 656e 7520 257d  ile_slim_menu %}
+000010a0: 0a7b 2520 656e 6462 6c6f 636b 2068 6561  .{% endblock hea
+000010b0: 6465 725f 6d6f 6269 6c65 5f73 6c69 6d5f  der_mobile_slim_
+000010c0: 6d65 6e75 2025 7d0a 0a7b 2520 626c 6f63  menu %}..{% bloc
+000010d0: 6b20 6865 6164 6572 5f73 6c69 6d5f 6d6f  k header_slim_mo
+000010e0: 6269 6c65 5f6f 7267 5f6e 616d 6520 257d  bile_org_name %}
+000010f0: 0a7b 2520 656e 6462 6c6f 636b 2068 6561  .{% endblock hea
+00001100: 6465 725f 736c 696d 5f6d 6f62 696c 655f  der_slim_mobile_
+00001110: 6f72 675f 6e61 6d65 2025 7d0a 0a7b 2520  org_name %}..{% 
+00001120: 626c 6f63 6b20 6865 6164 6572 5f63 656e  block header_cen
+00001130: 7465 725f 7772 6170 7065 725f 636f 6c75  ter_wrapper_colu
+00001140: 6d6e 7320 257d 0a63 6f6c 2d31 3020 6f66  mns %}.col-10 of
+00001150: 6673 6574 2d32 2063 6f6c 2d6c 672d 3132  fset-2 col-lg-12
+00001160: 206f 6666 7365 742d 6c67 2d30 0a7b 2520   offset-lg-0.{% 
+00001170: 656e 6462 6c6f 636b 2068 6561 6465 725f  endblock header_
+00001180: 6365 6e74 6572 5f77 7261 7070 6572 5f63  center_wrapper_c
+00001190: 6f6c 756d 6e73 2025 7d0a 0a3c 212d 2d20  olumns %}..<!-- 
+000011a0: 4d61 696e 204d 656e 7520 2d2d 3e0a 7b25  Main Menu -->.{%
+000011b0: 2062 6c6f 636b 206d 6169 6e5f 6d65 6e75   block main_menu
+000011c0: 2025 7d0a 2020 2020 7b25 206c 6f61 645f   %}.    {% load_
+000011d0: 626c 6f63 6b73 2073 6563 7469 6f6e 3d22  blocks section="
+000011e0: 6d65 6e75 2d31 2220 257d 0a7b 2520 656e  menu-1" %}.{% en
+000011f0: 6462 6c6f 636b 206d 6169 6e5f 6d65 6e75  dblock main_menu
+00001200: 2025 7d0a 0a3c 212d 2d20 436f 6e74 6169   %}..<!-- Contai
+00001210: 6e65 7220 2d2d 3e0a 7b25 2062 6c6f 636b  ner -->.{% block
+00001220: 2063 6f6e 7461 696e 6572 2025 7d0a 0a20   container %}.. 
+00001230: 2020 203c 212d 2d20 4d61 696e 2042 616e     <!-- Main Ban
+00001240: 6e65 722d 2d3e 0a20 2020 207b 2520 626c  ner-->.    {% bl
+00001250: 6f63 6b20 6261 6e6e 6572 2025 7d0a 2020  ock banner %}.  
+00001260: 2020 2020 2020 7b25 206c 6f61 645f 626c        {% load_bl
+00001270: 6f63 6b73 2073 6563 7469 6f6e 3d22 6261  ocks section="ba
+00001280: 6e6e 6572 2220 257d 0a20 2020 207b 2520  nner" %}.    {% 
+00001290: 656e 6462 6c6f 636b 2062 616e 6e65 7220  endblock banner 
+000012a0: 257d 0a20 2020 203c 212d 2d20 656e 6420  %}.    <!-- end 
+000012b0: 4d61 696e 2042 616e 6e65 722d 2d3e 0a0a  Main Banner-->..
+000012c0: 2020 2020 3c21 2d2d 204d 656e 7520 322d      <!-- Menu 2-
+000012d0: 2d3e 0a20 2020 207b 2520 626c 6f63 6b20  ->.    {% block 
+000012e0: 6d65 6e75 2d32 2025 7d0a 2020 2020 2020  menu-2 %}.      
+000012f0: 2020 7b25 206c 6f61 645f 626c 6f63 6b73    {% load_blocks
+00001300: 2073 6563 7469 6f6e 3d22 6d65 6e75 2d32   section="menu-2
+00001310: 2220 257d 0a20 2020 207b 2520 656e 6462  " %}.    {% endb
+00001320: 6c6f 636b 206d 656e 752d 3220 257d 0a20  lock menu-2 %}. 
+00001330: 2020 203c 212d 2d20 656e 6420 4d65 6e75     <!-- end Menu
+00001340: 2032 2d2d 3e0a 0a20 2020 203c 212d 2d20   2-->..    <!-- 
+00001350: 4272 6561 6463 7275 6d62 7320 2d2d 3e0a  Breadcrumbs -->.
+00001360: 2020 2020 7b25 2062 6c6f 636b 2062 7265      {% block bre
+00001370: 6164 6372 756d 6273 2025 7d0a 2020 2020  adcrumbs %}.    
+00001380: 2020 2020 7b25 206c 6f61 645f 626c 6f63      {% load_bloc
+00001390: 6b73 2073 6563 7469 6f6e 3d22 6272 6561  ks section="brea
+000013a0: 6463 7275 6d62 7322 2025 7d0a 2020 2020  dcrumbs" %}.    
+000013b0: 7b25 2065 6e64 626c 6f63 6b20 6272 6561  {% endblock brea
+000013c0: 6463 7275 6d62 7320 257d 0a20 2020 203c  dcrumbs %}.    <
+000013d0: 212d 2d20 656e 6420 4272 6561 6463 7275  !-- end Breadcru
+000013e0: 6d62 7320 2d2d 3e0a 0a20 2020 203c 212d  mbs -->..    <!-
+000013f0: 2d20 5365 6374 696f 6e20 3120 2d2d 3e0a  - Section 1 -->.
+00001400: 2020 2020 7b25 2062 6c6f 636b 2073 6563      {% block sec
+00001410: 7469 6f6e 5f31 2025 7d0a 2020 2020 7b25  tion_1 %}.    {%
+00001420: 2062 6c6f 636b 735f 696e 5f70 6f73 6974   blocks_in_posit
+00001430: 696f 6e20 7365 6374 696f 6e3d 2273 6563  ion section="sec
+00001440: 7469 6f6e 2d31 2220 6173 2073 6563 7469  tion-1" as secti
+00001450: 6f6e 5f31 2025 7d0a 2020 2020 7b25 2069  on_1 %}.    {% i
+00001460: 6620 7365 6374 696f 6e5f 3120 257d 0a20  f section_1 %}. 
+00001470: 2020 2020 2020 207b 2520 6c6f 6164 5f62         {% load_b
+00001480: 6c6f 636b 7320 7365 6374 696f 6e3d 2231  locks section="1
+00001490: 2d74 6f70 2d61 2220 6173 2031 5f74 6f70  -top-a" as 1_top
+000014a0: 5f61 2025 7d0a 2020 2020 2020 2020 7b25  _a %}.        {%
+000014b0: 206c 6f61 645f 626c 6f63 6b73 2073 6563   load_blocks sec
+000014c0: 7469 6f6e 3d22 312d 746f 702d 6222 2061  tion="1-top-b" a
+000014d0: 7320 315f 746f 705f 6220 257d 0a20 2020  s 1_top_b %}.   
+000014e0: 2020 2020 207b 2520 6c6f 6164 5f62 6c6f       {% load_blo
+000014f0: 636b 7320 7365 6374 696f 6e3d 2231 2d74  cks section="1-t
+00001500: 6f70 2d63 2220 6173 2031 5f74 6f70 5f63  op-c" as 1_top_c
+00001510: 2025 7d0a 0a20 2020 2020 2020 207b 2520   %}..        {% 
+00001520: 6c6f 6164 5f62 6c6f 636b 7320 7365 6374  load_blocks sect
+00001530: 696f 6e3d 2231 2d6d 6964 2d74 6f70 2d61  ion="1-mid-top-a
+00001540: 2220 6173 2031 5f6d 6964 5f74 6f70 5f61  " as 1_mid_top_a
+00001550: 2025 7d0a 2020 2020 2020 2020 7b25 206c   %}.        {% l
+00001560: 6f61 645f 626c 6f63 6b73 2073 6563 7469  oad_blocks secti
+00001570: 6f6e 3d22 312d 6d69 642d 746f 702d 6222  on="1-mid-top-b"
+00001580: 2061 7320 315f 6d69 645f 746f 705f 6220   as 1_mid_top_b 
+00001590: 257d 0a20 2020 2020 2020 207b 2520 6c6f  %}.        {% lo
+000015a0: 6164 5f62 6c6f 636b 7320 7365 6374 696f  ad_blocks sectio
+000015b0: 6e3d 2231 2d6d 6964 2d74 6f70 2d63 2220  n="1-mid-top-c" 
+000015c0: 6173 2031 5f6d 6964 5f74 6f70 5f63 2025  as 1_mid_top_c %
+000015d0: 7d0a 0a20 2020 2020 2020 207b 2520 6c6f  }..        {% lo
+000015e0: 6164 5f62 6c6f 636b 7320 7365 6374 696f  ad_blocks sectio
+000015f0: 6e3d 2231 2d6c 6566 742d 6122 2061 7320  n="1-left-a" as 
+00001600: 315f 6c65 6674 5f61 2025 7d0a 2020 2020  1_left_a %}.    
+00001610: 2020 2020 7b25 206c 6f61 645f 626c 6f63      {% load_bloc
+00001620: 6b73 2073 6563 7469 6f6e 3d22 312d 6c65  ks section="1-le
+00001630: 6674 2d62 2220 6173 2031 5f6c 6566 745f  ft-b" as 1_left_
+00001640: 6220 257d 0a0a 2020 2020 2020 2020 7b25  b %}..        {%
+00001650: 206c 6f61 645f 626c 6f63 6b73 2073 6563   load_blocks sec
+00001660: 7469 6f6e 3d22 312d 6365 6e74 6572 2d74  tion="1-center-t
+00001670: 6f70 2d61 2220 6173 2031 5f63 656e 7465  op-a" as 1_cente
+00001680: 725f 746f 705f 6120 257d 0a20 2020 2020  r_top_a %}.     
+00001690: 2020 207b 2520 6c6f 6164 5f62 6c6f 636b     {% load_block
+000016a0: 7320 7365 6374 696f 6e3d 2231 2d63 656e  s section="1-cen
+000016b0: 7465 722d 746f 702d 6222 2061 7320 315f  ter-top-b" as 1_
+000016c0: 6365 6e74 6572 5f74 6f70 5f62 2025 7d0a  center_top_b %}.
+000016d0: 2020 2020 2020 2020 7b25 206c 6f61 645f          {% load_
+000016e0: 626c 6f63 6b73 2073 6563 7469 6f6e 3d22  blocks section="
+000016f0: 312d 6365 6e74 6572 2d74 6f70 2d63 2220  1-center-top-c" 
+00001700: 6173 2031 5f63 656e 7465 725f 746f 705f  as 1_center_top_
+00001710: 6320 257d 0a0a 2020 2020 2020 2020 7b25  c %}..        {%
+00001720: 206c 6f61 645f 626c 6f63 6b73 2073 6563   load_blocks sec
+00001730: 7469 6f6e 3d22 312d 6365 6e74 6572 2d6d  tion="1-center-m
+00001740: 6964 2d74 6f70 2d61 2220 6173 2031 5f63  id-top-a" as 1_c
+00001750: 656e 7465 725f 6d69 645f 746f 705f 6120  enter_mid_top_a 
+00001760: 257d 0a20 2020 2020 2020 207b 2520 6c6f  %}.        {% lo
+00001770: 6164 5f62 6c6f 636b 7320 7365 6374 696f  ad_blocks sectio
+00001780: 6e3d 2231 2d63 656e 7465 722d 6d69 642d  n="1-center-mid-
+00001790: 746f 702d 6222 2061 7320 315f 6365 6e74  top-b" as 1_cent
+000017a0: 6572 5f6d 6964 5f74 6f70 5f62 2025 7d0a  er_mid_top_b %}.
+000017b0: 2020 2020 2020 2020 7b25 206c 6f61 645f          {% load_
+000017c0: 626c 6f63 6b73 2073 6563 7469 6f6e 3d22  blocks section="
+000017d0: 312d 6365 6e74 6572 2d6d 6964 2d74 6f70  1-center-mid-top
+000017e0: 2d63 2220 6173 2031 5f63 656e 7465 725f  -c" as 1_center_
+000017f0: 6d69 645f 746f 705f 6320 257d 0a0a 2020  mid_top_c %}..  
+00001800: 2020 2020 2020 7b25 206c 6f61 645f 626c        {% load_bl
+00001810: 6f63 6b73 2073 6563 7469 6f6e 3d22 312d  ocks section="1-
+00001820: 6365 6e74 6572 2d63 6f6e 7465 6e74 2220  center-content" 
+00001830: 6173 2031 5f63 656e 7465 725f 636f 6e74  as 1_center_cont
+00001840: 656e 7420 257d 0a0a 2020 2020 2020 2020  ent %}..        
+00001850: 7b25 206c 6f61 645f 626c 6f63 6b73 2073  {% load_blocks s
+00001860: 6563 7469 6f6e 3d22 312d 6365 6e74 6572  ection="1-center
+00001870: 2d6d 6964 2d62 6f74 746f 6d2d 6122 2061  -mid-bottom-a" a
+00001880: 7320 315f 6365 6e74 6572 5f6d 6964 5f62  s 1_center_mid_b
+00001890: 6f74 746f 6d5f 6120 257d 0a20 2020 2020  ottom_a %}.     
+000018a0: 2020 207b 2520 6c6f 6164 5f62 6c6f 636b     {% load_block
+000018b0: 7320 7365 6374 696f 6e3d 2231 2d63 656e  s section="1-cen
+000018c0: 7465 722d 6d69 642d 626f 7474 6f6d 2d62  ter-mid-bottom-b
+000018d0: 2220 6173 2031 5f63 656e 7465 725f 6d69  " as 1_center_mi
+000018e0: 645f 626f 7474 6f6d 5f62 2025 7d0a 2020  d_bottom_b %}.  
+000018f0: 2020 2020 2020 7b25 206c 6f61 645f 626c        {% load_bl
+00001900: 6f63 6b73 2073 6563 7469 6f6e 3d22 312d  ocks section="1-
+00001910: 6365 6e74 6572 2d6d 6964 2d62 6f74 746f  center-mid-botto
+00001920: 6d2d 6322 2061 7320 315f 6365 6e74 6572  m-c" as 1_center
+00001930: 5f6d 6964 5f62 6f74 746f 6d5f 6320 257d  _mid_bottom_c %}
+00001940: 0a0a 2020 2020 2020 2020 7b25 206c 6f61  ..        {% loa
+00001950: 645f 626c 6f63 6b73 2073 6563 7469 6f6e  d_blocks section
+00001960: 3d22 312d 6365 6e74 6572 2d62 6f74 746f  ="1-center-botto
+00001970: 6d2d 6122 2061 7320 315f 6365 6e74 6572  m-a" as 1_center
+00001980: 5f62 6f74 746f 6d5f 6120 257d 0a20 2020  _bottom_a %}.   
+00001990: 2020 2020 207b 2520 6c6f 6164 5f62 6c6f       {% load_blo
+000019a0: 636b 7320 7365 6374 696f 6e3d 2231 2d63  cks section="1-c
+000019b0: 656e 7465 722d 626f 7474 6f6d 2d62 2220  enter-bottom-b" 
+000019c0: 6173 2031 5f63 656e 7465 725f 626f 7474  as 1_center_bott
+000019d0: 6f6d 5f62 2025 7d0a 2020 2020 2020 2020  om_b %}.        
+000019e0: 7b25 206c 6f61 645f 626c 6f63 6b73 2073  {% load_blocks s
+000019f0: 6563 7469 6f6e 3d22 312d 6365 6e74 6572  ection="1-center
+00001a00: 2d62 6f74 746f 6d2d 6322 2061 7320 315f  -bottom-c" as 1_
+00001a10: 6365 6e74 6572 5f62 6f74 746f 6d5f 6320  center_bottom_c 
+00001a20: 257d 0a0a 2020 2020 2020 2020 7b25 206c  %}..        {% l
+00001a30: 6f61 645f 626c 6f63 6b73 2073 6563 7469  oad_blocks secti
+00001a40: 6f6e 3d22 312d 7269 6768 742d 6122 2061  on="1-right-a" a
+00001a50: 7320 315f 7269 6768 745f 6120 257d 0a20  s 1_right_a %}. 
+00001a60: 2020 2020 2020 207b 2520 6c6f 6164 5f62         {% load_b
+00001a70: 6c6f 636b 7320 7365 6374 696f 6e3d 2231  locks section="1
+00001a80: 2d72 6967 6874 2d62 2220 6173 2031 5f72  -right-b" as 1_r
+00001a90: 6967 6874 5f62 2025 7d0a 0a20 2020 2020  ight_b %}..     
+00001aa0: 2020 207b 2520 6c6f 6164 5f62 6c6f 636b     {% load_block
+00001ab0: 7320 7365 6374 696f 6e3d 2231 2d6d 6964  s section="1-mid
+00001ac0: 2d62 6f74 746f 6d2d 6122 2061 7320 315f  -bottom-a" as 1_
+00001ad0: 6d69 645f 626f 7474 6f6d 5f61 2025 7d0a  mid_bottom_a %}.
+00001ae0: 2020 2020 2020 2020 7b25 206c 6f61 645f          {% load_
+00001af0: 626c 6f63 6b73 2073 6563 7469 6f6e 3d22  blocks section="
+00001b00: 312d 6d69 642d 626f 7474 6f6d 2d62 2220  1-mid-bottom-b" 
+00001b10: 6173 2031 5f6d 6964 5f62 6f74 746f 6d5f  as 1_mid_bottom_
+00001b20: 6220 257d 0a20 2020 2020 2020 207b 2520  b %}.        {% 
+00001b30: 6c6f 6164 5f62 6c6f 636b 7320 7365 6374  load_blocks sect
+00001b40: 696f 6e3d 2231 2d6d 6964 2d62 6f74 746f  ion="1-mid-botto
+00001b50: 6d2d 6322 2061 7320 315f 6d69 645f 626f  m-c" as 1_mid_bo
+00001b60: 7474 6f6d 5f63 2025 7d0a 0a20 2020 2020  ttom_c %}..     
+00001b70: 2020 207b 2520 6c6f 6164 5f62 6c6f 636b     {% load_block
+00001b80: 7320 7365 6374 696f 6e3d 2231 2d62 6f74  s section="1-bot
+00001b90: 746f 6d2d 6122 2061 7320 315f 626f 7474  tom-a" as 1_bott
+00001ba0: 6f6d 5f61 2025 7d0a 2020 2020 2020 2020  om_a %}.        
+00001bb0: 7b25 206c 6f61 645f 626c 6f63 6b73 2073  {% load_blocks s
+00001bc0: 6563 7469 6f6e 3d22 312d 626f 7474 6f6d  ection="1-bottom
+00001bd0: 2d62 2220 6173 2031 5f62 6f74 746f 6d5f  -b" as 1_bottom_
+00001be0: 6220 257d 0a20 2020 2020 2020 207b 2520  b %}.        {% 
+00001bf0: 6c6f 6164 5f62 6c6f 636b 7320 7365 6374  load_blocks sect
+00001c00: 696f 6e3d 2231 2d62 6f74 746f 6d2d 6322  ion="1-bottom-c"
+00001c10: 2061 7320 315f 626f 7474 6f6d 5f63 2025   as 1_bottom_c %
+00001c20: 7d0a 0a20 2020 2020 2020 203c 6469 7620  }..        <div 
+00001c30: 636c 6173 733d 227b 2520 626c 6f63 6b20  class="{% block 
+00001c40: 7365 6374 696f 6e5f 315f 636c 6173 7365  section_1_classe
+00001c50: 7320 257d 7079 2d35 7b25 2065 6e64 626c  s %}py-5{% endbl
+00001c60: 6f63 6b20 257d 223e 0a20 2020 2020 2020  ock %}">.       
+00001c70: 2020 2020 203c 6469 7620 636c 6173 733d       <div class=
+00001c80: 2263 6f6e 7461 696e 6572 223e 0a20 2020  "container">.   
+00001c90: 2020 2020 2020 2020 2020 2020 203c 6469               <di
+00001ca0: 7620 636c 6173 733d 2272 6f77 206d 782d  v class="row mx-
+00001cb0: 3022 3e0a 0a20 2020 2020 2020 2020 2020  0">..           
+00001cc0: 2020 2020 2020 2020 203c 212d 2d20 546f           <!-- To
+00001cd0: 7020 2d2d 3e0a 2020 2020 2020 2020 2020  p -->.          
+00001ce0: 2020 2020 2020 2020 2020 7b25 2069 6620            {% if 
+00001cf0: 315f 746f 705f 6120 6f72 2031 5f74 6f70  1_top_a or 1_top
+00001d00: 5f62 206f 7220 315f 746f 705f 6320 257d  _b or 1_top_c %}
+00001d10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00001d20: 2020 2020 203c 6469 7620 636c 6173 733d       <div class=
+00001d30: 2263 6f6c 2d31 3222 3e0a 2020 2020 2020  "col-12">.      
+00001d40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001d50: 2020 3c64 6976 2063 6c61 7373 3d22 726f    <div class="ro
+00001d60: 7722 3e0a 2020 2020 2020 2020 2020 2020  w">.            
+00001d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001d80: 7b25 2069 6620 315f 746f 705f 6120 616e  {% if 1_top_a an
+00001d90: 6420 315f 746f 705f 6220 616e 6420 315f  d 1_top_b and 1_
+00001da0: 746f 705f 6320 257d 0a20 2020 2020 2020  top_c %}.       
+00001db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001dc0: 2020 2020 2020 2020 203c 6469 7620 636c           <div cl
+00001dd0: 6173 733d 227b 2520 626c 6f63 6b20 315f  ass="{% block 1_
+00001de0: 746f 705f 6162 635f 6120 257d 636f 6c2d  top_abc_a %}col-
+00001df0: 3132 2063 6f6c 2d6d 642d 347b 2520 656e  12 col-md-4{% en
+00001e00: 6462 6c6f 636b 2025 7d22 3e7b 7b20 315f  dblock %}">{{ 1_
+00001e10: 746f 705f 6120 7d7d 3c2f 6469 763e 0a20  top_a }}</div>. 
+00001e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001e30: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+00001e40: 6469 7620 636c 6173 733d 227b 2520 626c  div class="{% bl
+00001e50: 6f63 6b20 315f 746f 705f 6162 635f 6220  ock 1_top_abc_b 
+00001e60: 257d 636f 6c2d 3132 2063 6f6c 2d6d 642d  %}col-12 col-md-
+00001e70: 347b 2520 656e 6462 6c6f 636b 2025 7d22  4{% endblock %}"
+00001e80: 3e7b 7b20 315f 746f 705f 6220 7d7d 3c2f  >{{ 1_top_b }}</
+00001e90: 6469 763e 0a20 2020 2020 2020 2020 2020  div>.           
 00001ea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001eb0: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-00001ec0: 6469 7620 636c 6173 733d 2263 6f6c 2d31  div class="col-1
-00001ed0: 3222 3e7b 7b20 315f 746f 705f 6120 7d7d  2">{{ 1_top_a }}
-00001ee0: 7b7b 2031 5f74 6f70 5f62 207d 7d7b 7b20  {{ 1_top_b }}{{ 
-00001ef0: 315f 746f 705f 6320 7d7d 3c2f 6469 763e  1_top_c }}</div>
-00001f00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001f10: 2020 2020 2020 2020 2020 2020 207b 2520               {% 
-00001f20: 656e 6469 6620 257d 0a20 2020 2020 2020  endif %}.       
-00001f30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001f40: 203c 2f64 6976 3e0a 2020 2020 2020 2020   </div>.        
-00001f50: 2020 2020 2020 2020 2020 2020 3c2f 6469              </di
-00001f60: 763e 0a20 2020 2020 2020 2020 2020 2020  v>.             
-00001f70: 2020 2020 2020 207b 2520 656e 6469 6620         {% endif 
-00001f80: 257d 0a20 2020 2020 2020 2020 2020 2020  %}.             
-00001f90: 2020 2020 2020 203c 212d 2d20 656e 6420         <!-- end 
-00001fa0: 546f 7020 2d2d 3e0a 0a20 2020 2020 2020  Top -->..       
-00001fb0: 2020 2020 2020 2020 2020 2020 203c 212d               <!-
-00001fc0: 2d20 4d69 6464 6c65 2054 6f70 202d 2d3e  - Middle Top -->
-00001fd0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001fe0: 2020 2020 207b 2520 6966 2031 5f6d 6964       {% if 1_mid
-00001ff0: 5f74 6f70 5f61 206f 7220 315f 6d69 645f  _top_a or 1_mid_
-00002000: 746f 705f 6220 6f72 2031 5f6d 6964 5f74  top_b or 1_mid_t
-00002010: 6f70 5f63 2025 7d0a 2020 2020 2020 2020  op_c %}.        
-00002020: 2020 2020 2020 2020 2020 2020 3c64 6976              <div
-00002030: 2063 6c61 7373 3d22 636f 6c2d 3132 223e   class="col-12">
-00002040: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002050: 2020 2020 2020 2020 203c 6469 7620 636c           <div cl
-00002060: 6173 733d 2272 6f77 223e 0a20 2020 2020  ass="row">.     
+00001eb0: 2020 2020 203c 6469 7620 636c 6173 733d       <div class=
+00001ec0: 227b 2520 626c 6f63 6b20 315f 746f 705f  "{% block 1_top_
+00001ed0: 6162 635f 6320 257d 636f 6c2d 3132 2063  abc_c %}col-12 c
+00001ee0: 6f6c 2d6d 642d 347b 2520 656e 6462 6c6f  ol-md-4{% endblo
+00001ef0: 636b 2025 7d22 3e7b 7b20 315f 746f 705f  ck %}">{{ 1_top_
+00001f00: 6320 7d7d 3c2f 6469 763e 0a20 2020 2020  c }}</div>.     
+00001f10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001f20: 2020 2020 2020 207b 2520 656c 6966 2031         {% elif 1
+00001f30: 5f74 6f70 5f61 2061 6e64 2031 5f74 6f70  _top_a and 1_top
+00001f40: 5f62 2025 7d0a 2020 2020 2020 2020 2020  _b %}.          
+00001f50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001f60: 2020 2020 2020 3c64 6976 2063 6c61 7373        <div class
+00001f70: 3d22 7b25 2062 6c6f 636b 2031 5f74 6f70  ="{% block 1_top
+00001f80: 5f61 625f 6120 257d 636f 6c2d 3132 2063  _ab_a %}col-12 c
+00001f90: 6f6c 2d6d 642d 387b 2520 656e 6462 6c6f  ol-md-8{% endblo
+00001fa0: 636b 2025 7d22 3e7b 7b20 315f 746f 705f  ck %}">{{ 1_top_
+00001fb0: 6120 7d7d 3c2f 6469 763e 0a20 2020 2020  a }}</div>.     
+00001fc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001fd0: 2020 2020 2020 2020 2020 203c 6469 7620             <div 
+00001fe0: 636c 6173 733d 227b 2520 626c 6f63 6b20  class="{% block 
+00001ff0: 315f 746f 705f 6162 5f62 2025 7d63 6f6c  1_top_ab_b %}col
+00002000: 2d31 3220 636f 6c2d 6d64 2d34 7b25 2065  -12 col-md-4{% e
+00002010: 6e64 626c 6f63 6b20 257d 223e 7b7b 2031  ndblock %}">{{ 1
+00002020: 5f74 6f70 5f62 207d 7d3c 2f64 6976 3e0a  _top_b }}</div>.
+00002030: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002040: 2020 2020 2020 2020 2020 2020 7b25 2065              {% e
+00002050: 6c69 6620 315f 746f 705f 6120 616e 6420  lif 1_top_a and 
+00002060: 315f 746f 705f 6320 257d 0a20 2020 2020  1_top_c %}.     
 00002070: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002080: 2020 2020 2020 207b 2520 6966 2031 5f6d         {% if 1_m
-00002090: 6964 5f74 6f70 5f61 2061 6e64 2031 5f6d  id_top_a and 1_m
-000020a0: 6964 5f74 6f70 5f62 2061 6e64 2031 5f6d  id_top_b and 1_m
-000020b0: 6964 5f74 6f70 5f63 2025 7d0a 2020 2020  id_top_c %}.    
-000020c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000020d0: 2020 2020 2020 2020 2020 2020 3c64 6976              <div
-000020e0: 2063 6c61 7373 3d22 7b25 2062 6c6f 636b   class="{% block
-000020f0: 2031 5f6d 6964 5f74 6f70 5f61 6263 5f61   1_mid_top_abc_a
-00002100: 2025 7d63 6f6c 2d31 3220 636f 6c2d 6d64   %}col-12 col-md
-00002110: 2d34 7b25 2065 6e64 626c 6f63 6b20 257d  -4{% endblock %}
-00002120: 223e 7b7b 2031 5f6d 6964 5f74 6f70 5f61  ">{{ 1_mid_top_a
-00002130: 207d 7d3c 2f64 6976 3e0a 2020 2020 2020   }}</div>.      
-00002140: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002150: 2020 2020 2020 2020 2020 3c64 6976 2063            <div c
-00002160: 6c61 7373 3d22 7b25 2062 6c6f 636b 2031  lass="{% block 1
-00002170: 5f6d 6964 5f74 6f70 5f61 6263 5f62 2025  _mid_top_abc_b %
-00002180: 7d63 6f6c 2d31 3220 636f 6c2d 6d64 2d34  }col-12 col-md-4
-00002190: 7b25 2065 6e64 626c 6f63 6b20 257d 223e  {% endblock %}">
-000021a0: 7b7b 2031 5f6d 6964 5f74 6f70 5f62 207d  {{ 1_mid_top_b }
-000021b0: 7d3c 2f64 6976 3e0a 2020 2020 2020 2020  }</div>.        
-000021c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000021d0: 2020 2020 2020 2020 3c64 6976 2063 6c61          <div cla
-000021e0: 7373 3d22 7b25 2062 6c6f 636b 2031 5f6d  ss="{% block 1_m
-000021f0: 6964 5f74 6f70 5f61 6263 5f63 2025 7d63  id_top_abc_c %}c
-00002200: 6f6c 2d31 3220 636f 6c2d 6d64 2d34 7b25  ol-12 col-md-4{%
-00002210: 2065 6e64 626c 6f63 6b20 257d 223e 7b7b   endblock %}">{{
-00002220: 2031 5f6d 6964 5f74 6f70 5f63 207d 7d3c   1_mid_top_c }}<
-00002230: 2f64 6976 3e0a 2020 2020 2020 2020 2020  /div>.          
-00002240: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002250: 2020 7b25 2065 6c69 6620 315f 6d69 645f    {% elif 1_mid_
-00002260: 746f 705f 6120 616e 6420 315f 6d69 645f  top_a and 1_mid_
-00002270: 746f 705f 6220 257d 0a20 2020 2020 2020  top_b %}.       
+00002080: 2020 2020 2020 2020 2020 203c 6469 7620             <div 
+00002090: 636c 6173 733d 227b 2520 626c 6f63 6b20  class="{% block 
+000020a0: 315f 746f 705f 6163 5f61 2025 7d63 6f6c  1_top_ac_a %}col
+000020b0: 2d31 3220 636f 6c2d 6d64 2d36 7b25 2065  -12 col-md-6{% e
+000020c0: 6e64 626c 6f63 6b20 257d 223e 7b7b 2031  ndblock %}">{{ 1
+000020d0: 5f74 6f70 5f61 207d 7d3c 2f64 6976 3e0a  _top_a }}</div>.
+000020e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000020f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002100: 3c64 6976 2063 6c61 7373 3d22 7b25 2062  <div class="{% b
+00002110: 6c6f 636b 2031 5f74 6f70 5f61 635f 6320  lock 1_top_ac_c 
+00002120: 257d 636f 6c2d 3132 2063 6f6c 2d6d 642d  %}col-12 col-md-
+00002130: 367b 2520 656e 6462 6c6f 636b 2025 7d22  6{% endblock %}"
+00002140: 3e7b 7b20 315f 746f 705f 6320 7d7d 3c2f  >{{ 1_top_c }}</
+00002150: 6469 763e 0a20 2020 2020 2020 2020 2020  div>.           
+00002160: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002170: 207b 2520 656c 6966 2031 5f74 6f70 5f62   {% elif 1_top_b
+00002180: 2061 6e64 2031 5f74 6f70 5f63 2025 7d0a   and 1_top_c %}.
+00002190: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000021a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000021b0: 3c64 6976 2063 6c61 7373 3d22 7b25 2062  <div class="{% b
+000021c0: 6c6f 636b 2031 5f74 6f70 5f62 635f 6220  lock 1_top_bc_b 
+000021d0: 257d 636f 6c2d 3132 2063 6f6c 2d6d 642d  %}col-12 col-md-
+000021e0: 347b 2520 656e 6462 6c6f 636b 2025 7d22  4{% endblock %}"
+000021f0: 3e7b 7b20 315f 746f 705f 6220 7d7d 3c2f  >{{ 1_top_b }}</
+00002200: 6469 763e 0a20 2020 2020 2020 2020 2020  div>.           
+00002210: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002220: 2020 2020 203c 6469 7620 636c 6173 733d       <div class=
+00002230: 227b 2520 626c 6f63 6b20 315f 746f 705f  "{% block 1_top_
+00002240: 6263 5f63 2025 7d63 6f6c 2d31 3220 636f  bc_c %}col-12 co
+00002250: 6c2d 6d64 2d38 7b25 2065 6e64 626c 6f63  l-md-8{% endbloc
+00002260: 6b20 257d 223e 7b7b 2031 5f74 6f70 5f63  k %}">{{ 1_top_c
+00002270: 207d 7d3c 2f64 6976 3e0a 2020 2020 2020   }}</div>.      
 00002280: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002290: 2020 2020 2020 2020 203c 6469 7620 636c           <div cl
-000022a0: 6173 733d 227b 2520 626c 6f63 6b20 315f  ass="{% block 1_
-000022b0: 6d69 645f 746f 705f 6162 5f61 2025 7d63  mid_top_ab_a %}c
-000022c0: 6f6c 2d31 3220 636f 6c2d 6d64 2d38 7b25  ol-12 col-md-8{%
-000022d0: 2065 6e64 626c 6f63 6b20 257d 223e 7b7b   endblock %}">{{
-000022e0: 2031 5f6d 6964 5f74 6f70 5f61 207d 7d3c   1_mid_top_a }}<
-000022f0: 2f64 6976 3e0a 2020 2020 2020 2020 2020  /div>.          
-00002300: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002310: 2020 2020 2020 3c64 6976 2063 6c61 7373        <div class
-00002320: 3d22 7b25 2062 6c6f 636b 2031 5f6d 6964  ="{% block 1_mid
-00002330: 5f74 6f70 5f61 625f 6220 257d 636f 6c2d  _top_ab_b %}col-
-00002340: 3132 2063 6f6c 2d6d 642d 347b 2520 656e  12 col-md-4{% en
-00002350: 6462 6c6f 636b 2025 7d22 3e7b 7b20 315f  dblock %}">{{ 1_
-00002360: 6d69 645f 746f 705f 6220 7d7d 3c2f 6469  mid_top_b }}</di
-00002370: 763e 0a20 2020 2020 2020 2020 2020 2020  v>.             
-00002380: 2020 2020 2020 2020 2020 2020 2020 207b                 {
-00002390: 2520 656c 6966 2031 5f6d 6964 5f74 6f70  % elif 1_mid_top
-000023a0: 5f61 2061 6e64 2031 5f6d 6964 5f74 6f70  _a and 1_mid_top
-000023b0: 5f63 2025 7d0a 2020 2020 2020 2020 2020  _c %}.          
-000023c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000023d0: 2020 2020 2020 3c64 6976 2063 6c61 7373        <div class
-000023e0: 3d22 7b25 2062 6c6f 636b 2031 5f6d 6964  ="{% block 1_mid
-000023f0: 5f74 6f70 5f61 635f 6120 257d 636f 6c2d  _top_ac_a %}col-
-00002400: 3132 2063 6f6c 2d6d 642d 367b 2520 656e  12 col-md-6{% en
-00002410: 6462 6c6f 636b 2025 7d22 3e7b 7b20 315f  dblock %}">{{ 1_
-00002420: 6d69 645f 746f 705f 6120 7d7d 3c2f 6469  mid_top_a }}</di
-00002430: 763e 0a20 2020 2020 2020 2020 2020 2020  v>.             
-00002440: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002450: 2020 203c 6469 7620 636c 6173 733d 227b     <div class="{
-00002460: 2520 626c 6f63 6b20 315f 6d69 645f 746f  % block 1_mid_to
-00002470: 705f 6163 5f63 2025 7d63 6f6c 2d31 3220  p_ac_c %}col-12 
-00002480: 636f 6c2d 6d64 2d36 7b25 2065 6e64 626c  col-md-6{% endbl
-00002490: 6f63 6b20 257d 223e 7b7b 2031 5f6d 6964  ock %}">{{ 1_mid
-000024a0: 5f74 6f70 5f63 207d 7d3c 2f64 6976 3e0a  _top_c }}</div>.
-000024b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000024c0: 2020 2020 2020 2020 2020 2020 7b25 2065              {% e
-000024d0: 6c69 6620 315f 6d69 645f 746f 705f 6220  lif 1_mid_top_b 
-000024e0: 616e 6420 315f 6d69 645f 746f 705f 6320  and 1_mid_top_c 
-000024f0: 257d 0a20 2020 2020 2020 2020 2020 2020  %}.             
-00002500: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002510: 2020 203c 6469 7620 636c 6173 733d 227b     <div class="{
-00002520: 2520 626c 6f63 6b20 315f 6d69 645f 746f  % block 1_mid_to
-00002530: 705f 6263 5f62 2025 7d63 6f6c 2d31 3220  p_bc_b %}col-12 
-00002540: 636f 6c2d 6d64 2d34 7b25 2065 6e64 626c  col-md-4{% endbl
-00002550: 6f63 6b20 257d 223e 7b7b 2031 5f6d 6964  ock %}">{{ 1_mid
-00002560: 5f74 6f70 5f62 207d 7d3c 2f64 6976 3e0a  _top_b }}</div>.
-00002570: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002580: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002590: 3c64 6976 2063 6c61 7373 3d22 7b25 2062  <div class="{% b
-000025a0: 6c6f 636b 2031 5f6d 6964 5f74 6f70 5f62  lock 1_mid_top_b
-000025b0: 635f 6320 257d 636f 6c2d 3132 2063 6f6c  c_c %}col-12 col
-000025c0: 2d6d 642d 387b 2520 656e 6462 6c6f 636b  -md-8{% endblock
-000025d0: 2025 7d22 3e7b 7b20 315f 6d69 645f 746f   %}">{{ 1_mid_to
-000025e0: 705f 6320 7d7d 3c2f 6469 763e 0a20 2020  p_c }}</div>.   
-000025f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002600: 2020 2020 2020 2020 207b 2520 656c 7365           {% else
-00002610: 2025 7d0a 2020 2020 2020 2020 2020 2020   %}.            
-00002620: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002630: 2020 2020 3c64 6976 2063 6c61 7373 3d22      <div class="
-00002640: 636f 6c2d 3132 223e 7b7b 2031 5f6d 6964  col-12">{{ 1_mid
-00002650: 5f74 6f70 5f61 207d 7d7b 7b20 315f 6d69  _top_a }}{{ 1_mi
-00002660: 645f 746f 705f 6220 7d7d 7b7b 2031 5f6d  d_top_b }}{{ 1_m
-00002670: 6964 5f74 6f70 5f63 207d 7d3c 2f64 6976  id_top_c }}</div
-00002680: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
-00002690: 2020 2020 2020 2020 2020 2020 2020 7b25                {%
-000026a0: 2065 6e64 6966 2025 7d0a 2020 2020 2020   endif %}.      
-000026b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000026c0: 2020 3c2f 6469 763e 0a20 2020 2020 2020    </div>.       
-000026d0: 2020 2020 2020 2020 2020 2020 203c 2f64               </d
-000026e0: 6976 3e0a 2020 2020 2020 2020 2020 2020  iv>.            
-000026f0: 2020 2020 2020 2020 7b25 2065 6e64 6966          {% endif
-00002700: 2025 7d0a 2020 2020 2020 2020 2020 2020   %}.            
-00002710: 2020 2020 2020 2020 3c21 2d2d 2065 6e64          <!-- end
-00002720: 204d 6964 646c 6520 546f 7020 2d2d 3e0a   Middle Top -->.
-00002730: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002740: 2020 2020 203c 212d 2d20 426c 6f63 6b73       <!-- Blocks
-00002750: 2069 6e20 6365 6e74 6572 2070 6f73 6974   in center posit
-00002760: 696f 6e73 202d 2d3e 0a20 2020 2020 2020  ions -->.       
-00002770: 2020 2020 2020 2020 2020 2020 207b 2520               {% 
-00002780: 6966 2031 5f63 656e 7465 725f 746f 705f  if 1_center_top_
-00002790: 6120 6f72 2031 5f63 656e 7465 725f 746f  a or 1_center_to
-000027a0: 705f 6220 6f72 2031 5f63 656e 7465 725f  p_b or 1_center_
-000027b0: 746f 705f 6320 6f72 2031 5f63 656e 7465  top_c or 1_cente
-000027c0: 725f 6d69 645f 746f 705f 6120 6f72 2031  r_mid_top_a or 1
-000027d0: 5f63 656e 7465 725f 6d69 645f 746f 705f  _center_mid_top_
-000027e0: 6220 6f72 2031 5f63 656e 7465 725f 6d69  b or 1_center_mi
-000027f0: 645f 746f 705f 6320 6f72 2031 5f63 656e  d_top_c or 1_cen
-00002800: 7465 725f 636f 6e74 656e 7420 6f72 2031  ter_content or 1
-00002810: 5f63 656e 7465 725f 6d69 645f 626f 7474  _center_mid_bott
-00002820: 6f6d 5f61 206f 7220 315f 6365 6e74 6572  om_a or 1_center
-00002830: 5f6d 6964 5f62 6f74 746f 6d5f 6220 6f72  _mid_bottom_b or
-00002840: 2031 5f63 656e 7465 725f 6d69 645f 626f   1_center_mid_bo
-00002850: 7474 6f6d 5f63 206f 7220 315f 6365 6e74  ttom_c or 1_cent
-00002860: 6572 5f62 6f74 746f 6d5f 6120 6f72 2031  er_bottom_a or 1
-00002870: 5f63 656e 7465 725f 626f 7474 6f6d 5f62  _center_bottom_b
-00002880: 206f 7220 315f 6365 6e74 6572 5f62 6f74   or 1_center_bot
-00002890: 746f 6d5f 6320 257d 0a0a 2020 2020 2020  tom_c %}..      
-000028a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000028b0: 2020 3c21 2d2d 2042 6c6f 636b 7320 696e    <!-- Blocks in
-000028c0: 206c 6566 7420 636f 6c75 6d6e 202d 2d3e   left column -->
-000028d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000028e0: 2020 2020 2020 2020 207b 2520 6966 2031           {% if 1
-000028f0: 5f6c 6566 745f 6120 6f72 2031 5f6c 6566  _left_a or 1_lef
-00002900: 745f 6220 257d 0a20 2020 2020 2020 2020  t_b %}.         
-00002910: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002920: 2020 207b 2520 6966 2031 5f6c 6566 745f     {% if 1_left_
-00002930: 6120 616e 6420 315f 6c65 6674 5f62 2025  a and 1_left_b %
-00002940: 7d0a 2020 2020 2020 2020 2020 2020 2020  }.              
-00002950: 2020 2020 2020 2020 2020 2020 2020 3c64                <d
-00002960: 6976 2063 6c61 7373 3d22 7b25 2062 6c6f  iv class="{% blo
-00002970: 636b 2031 5f6c 6566 745f 6162 2025 7d63  ck 1_left_ab %}c
-00002980: 6f6c 2d31 3220 636f 6c2d 6c67 2d34 206d  ol-12 col-lg-4 m
-00002990: 622d 3520 6d62 2d6c 672d 307b 2520 656e  b-5 mb-lg-0{% en
-000029a0: 6462 6c6f 636b 2025 7d22 3e0a 2020 2020  dblock %}">.    
-000029b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000029c0: 2020 2020 2020 2020 7b25 2065 6c69 6620          {% elif 
-000029d0: 315f 6c65 6674 5f61 2025 7d0a 2020 2020  1_left_a %}.    
-000029e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000029f0: 2020 2020 2020 2020 3c64 6976 2063 6c61          <div cla
-00002a00: 7373 3d22 7b25 2062 6c6f 636b 2031 5f6c  ss="{% block 1_l
-00002a10: 6566 745f 6120 257d 636f 6c2d 3132 2063  eft_a %}col-12 c
-00002a20: 6f6c 2d6c 672d 3320 6d62 2d35 206d 622d  ol-lg-3 mb-5 mb-
-00002a30: 6c67 2d30 7b25 2065 6e64 626c 6f63 6b20  lg-0{% endblock 
-00002a40: 257d 223e 0a20 2020 2020 2020 2020 2020  %}">.           
-00002a50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002a60: 207b 2520 656c 7365 2025 7d0a 2020 2020   {% else %}.    
-00002a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002a80: 2020 2020 2020 2020 3c64 6976 2063 6c61          <div cla
-00002a90: 7373 3d22 7b25 2062 6c6f 636b 2031 5f6c  ss="{% block 1_l
-00002aa0: 6566 745f 6220 257d 636f 6c2d 3132 2063  eft_b %}col-12 c
-00002ab0: 6f6c 2d6c 672d 3320 6d62 2d35 206d 622d  ol-lg-3 mb-5 mb-
-00002ac0: 6c67 2d30 7b25 2065 6e64 626c 6f63 6b20  lg-0{% endblock 
-00002ad0: 257d 223e 0a20 2020 2020 2020 2020 2020  %}">.           
-00002ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002af0: 207b 2520 656e 6469 6620 257d 0a20 2020   {% endif %}.   
-00002b00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002b10: 2020 2020 2020 2020 2020 2020 203c 6469               <di
-00002b20: 7620 636c 6173 733d 2272 6f77 223e 0a20  v class="row">. 
-00002b30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002b40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002b50: 2020 207b 2520 6966 2031 5f6c 6566 745f     {% if 1_left_
-00002b60: 6120 616e 6420 315f 6c65 6674 5f62 2025  a and 1_left_b %
-00002b70: 7d0a 2020 2020 2020 2020 2020 2020 2020  }.              
-00002b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002b90: 2020 2020 2020 3c64 6976 2063 6c61 7373        <div class
-00002ba0: 3d22 7b25 2062 6c6f 636b 2031 5f6c 6566  ="{% block 1_lef
-00002bb0: 745f 6162 5f61 2025 7d63 6f6c 2d31 3220  t_ab_a %}col-12 
-00002bc0: 636f 6c2d 6c67 2d36 7b25 2065 6e64 626c  col-lg-6{% endbl
-00002bd0: 6f63 6b20 257d 223e 7b7b 2031 5f6c 6566  ock %}">{{ 1_lef
-00002be0: 745f 6120 7d7d 3c2f 6469 763e 0a20 2020  t_a }}</div>.   
-00002bf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002c10: 203c 6469 7620 636c 6173 733d 227b 2520   <div class="{% 
-00002c20: 626c 6f63 6b20 315f 6c65 6674 5f61 625f  block 1_left_ab_
-00002c30: 6220 257d 636f 6c2d 3132 2063 6f6c 2d6c  b %}col-12 col-l
-00002c40: 672d 367b 2520 656e 6462 6c6f 636b 2025  g-6{% endblock %
-00002c50: 7d22 3e7b 7b20 315f 6c65 6674 5f62 207d  }">{{ 1_left_b }
-00002c60: 7d3c 2f64 6976 3e0a 2020 2020 2020 2020  }</div>.        
-00002c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002c80: 2020 2020 2020 2020 2020 2020 7b25 2065              {% e
-00002c90: 6c69 6620 315f 6c65 6674 5f61 2025 7d0a  lif 1_left_a %}.
+00002290: 2020 2020 2020 7b25 2065 6c73 6520 257d        {% else %}
+000022a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000022b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000022c0: 203c 6469 7620 636c 6173 733d 2263 6f6c   <div class="col
+000022d0: 2d31 3222 3e7b 7b20 315f 746f 705f 6120  -12">{{ 1_top_a 
+000022e0: 7d7d 7b7b 2031 5f74 6f70 5f62 207d 7d7b  }}{{ 1_top_b }}{
+000022f0: 7b20 315f 746f 705f 6320 7d7d 3c2f 6469  { 1_top_c }}</di
+00002300: 763e 0a20 2020 2020 2020 2020 2020 2020  v>.             
+00002310: 2020 2020 2020 2020 2020 2020 2020 207b                 {
+00002320: 2520 656e 6469 6620 257d 0a20 2020 2020  % endif %}.     
+00002330: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002340: 2020 203c 2f64 6976 3e0a 2020 2020 2020     </div>.      
+00002350: 2020 2020 2020 2020 2020 2020 2020 3c2f                </
+00002360: 6469 763e 0a20 2020 2020 2020 2020 2020  div>.           
+00002370: 2020 2020 2020 2020 207b 2520 656e 6469           {% endi
+00002380: 6620 257d 0a20 2020 2020 2020 2020 2020  f %}.           
+00002390: 2020 2020 2020 2020 203c 212d 2d20 656e           <!-- en
+000023a0: 6420 546f 7020 2d2d 3e0a 0a20 2020 2020  d Top -->..     
+000023b0: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+000023c0: 212d 2d20 4d69 6464 6c65 2054 6f70 202d  !-- Middle Top -
+000023d0: 2d3e 0a20 2020 2020 2020 2020 2020 2020  ->.             
+000023e0: 2020 2020 2020 207b 2520 6966 2031 5f6d         {% if 1_m
+000023f0: 6964 5f74 6f70 5f61 206f 7220 315f 6d69  id_top_a or 1_mi
+00002400: 645f 746f 705f 6220 6f72 2031 5f6d 6964  d_top_b or 1_mid
+00002410: 5f74 6f70 5f63 2025 7d0a 2020 2020 2020  _top_c %}.      
+00002420: 2020 2020 2020 2020 2020 2020 2020 3c64                <d
+00002430: 6976 2063 6c61 7373 3d22 636f 6c2d 3132  iv class="col-12
+00002440: 223e 0a20 2020 2020 2020 2020 2020 2020  ">.             
+00002450: 2020 2020 2020 2020 2020 203c 6469 7620             <div 
+00002460: 636c 6173 733d 2272 6f77 223e 0a20 2020  class="row">.   
+00002470: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002480: 2020 2020 2020 2020 207b 2520 6966 2031           {% if 1
+00002490: 5f6d 6964 5f74 6f70 5f61 2061 6e64 2031  _mid_top_a and 1
+000024a0: 5f6d 6964 5f74 6f70 5f62 2061 6e64 2031  _mid_top_b and 1
+000024b0: 5f6d 6964 5f74 6f70 5f63 2025 7d0a 2020  _mid_top_c %}.  
+000024c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000024d0: 2020 2020 2020 2020 2020 2020 2020 3c64                <d
+000024e0: 6976 2063 6c61 7373 3d22 7b25 2062 6c6f  iv class="{% blo
+000024f0: 636b 2031 5f6d 6964 5f74 6f70 5f61 6263  ck 1_mid_top_abc
+00002500: 5f61 2025 7d63 6f6c 2d31 3220 636f 6c2d  _a %}col-12 col-
+00002510: 6d64 2d34 7b25 2065 6e64 626c 6f63 6b20  md-4{% endblock 
+00002520: 257d 223e 7b7b 2031 5f6d 6964 5f74 6f70  %}">{{ 1_mid_top
+00002530: 5f61 207d 7d3c 2f64 6976 3e0a 2020 2020  _a }}</div>.    
+00002540: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002550: 2020 2020 2020 2020 2020 2020 3c64 6976              <div
+00002560: 2063 6c61 7373 3d22 7b25 2062 6c6f 636b   class="{% block
+00002570: 2031 5f6d 6964 5f74 6f70 5f61 6263 5f62   1_mid_top_abc_b
+00002580: 2025 7d63 6f6c 2d31 3220 636f 6c2d 6d64   %}col-12 col-md
+00002590: 2d34 7b25 2065 6e64 626c 6f63 6b20 257d  -4{% endblock %}
+000025a0: 223e 7b7b 2031 5f6d 6964 5f74 6f70 5f62  ">{{ 1_mid_top_b
+000025b0: 207d 7d3c 2f64 6976 3e0a 2020 2020 2020   }}</div>.      
+000025c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000025d0: 2020 2020 2020 2020 2020 3c64 6976 2063            <div c
+000025e0: 6c61 7373 3d22 7b25 2062 6c6f 636b 2031  lass="{% block 1
+000025f0: 5f6d 6964 5f74 6f70 5f61 6263 5f63 2025  _mid_top_abc_c %
+00002600: 7d63 6f6c 2d31 3220 636f 6c2d 6d64 2d34  }col-12 col-md-4
+00002610: 7b25 2065 6e64 626c 6f63 6b20 257d 223e  {% endblock %}">
+00002620: 7b7b 2031 5f6d 6964 5f74 6f70 5f63 207d  {{ 1_mid_top_c }
+00002630: 7d3c 2f64 6976 3e0a 2020 2020 2020 2020  }</div>.        
+00002640: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002650: 2020 2020 7b25 2065 6c69 6620 315f 6d69      {% elif 1_mi
+00002660: 645f 746f 705f 6120 616e 6420 315f 6d69  d_top_a and 1_mi
+00002670: 645f 746f 705f 6220 257d 0a20 2020 2020  d_top_b %}.     
+00002680: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002690: 2020 2020 2020 2020 2020 203c 6469 7620             <div 
+000026a0: 636c 6173 733d 227b 2520 626c 6f63 6b20  class="{% block 
+000026b0: 315f 6d69 645f 746f 705f 6162 5f61 2025  1_mid_top_ab_a %
+000026c0: 7d63 6f6c 2d31 3220 636f 6c2d 6d64 2d38  }col-12 col-md-8
+000026d0: 7b25 2065 6e64 626c 6f63 6b20 257d 223e  {% endblock %}">
+000026e0: 7b7b 2031 5f6d 6964 5f74 6f70 5f61 207d  {{ 1_mid_top_a }
+000026f0: 7d3c 2f64 6976 3e0a 2020 2020 2020 2020  }</div>.        
+00002700: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002710: 2020 2020 2020 2020 3c64 6976 2063 6c61          <div cla
+00002720: 7373 3d22 7b25 2062 6c6f 636b 2031 5f6d  ss="{% block 1_m
+00002730: 6964 5f74 6f70 5f61 625f 6220 257d 636f  id_top_ab_b %}co
+00002740: 6c2d 3132 2063 6f6c 2d6d 642d 347b 2520  l-12 col-md-4{% 
+00002750: 656e 6462 6c6f 636b 2025 7d22 3e7b 7b20  endblock %}">{{ 
+00002760: 315f 6d69 645f 746f 705f 6220 7d7d 3c2f  1_mid_top_b }}</
+00002770: 6469 763e 0a20 2020 2020 2020 2020 2020  div>.           
+00002780: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002790: 207b 2520 656c 6966 2031 5f6d 6964 5f74   {% elif 1_mid_t
+000027a0: 6f70 5f61 2061 6e64 2031 5f6d 6964 5f74  op_a and 1_mid_t
+000027b0: 6f70 5f63 2025 7d0a 2020 2020 2020 2020  op_c %}.        
+000027c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000027d0: 2020 2020 2020 2020 3c64 6976 2063 6c61          <div cla
+000027e0: 7373 3d22 7b25 2062 6c6f 636b 2031 5f6d  ss="{% block 1_m
+000027f0: 6964 5f74 6f70 5f61 635f 6120 257d 636f  id_top_ac_a %}co
+00002800: 6c2d 3132 2063 6f6c 2d6d 642d 367b 2520  l-12 col-md-6{% 
+00002810: 656e 6462 6c6f 636b 2025 7d22 3e7b 7b20  endblock %}">{{ 
+00002820: 315f 6d69 645f 746f 705f 6120 7d7d 3c2f  1_mid_top_a }}</
+00002830: 6469 763e 0a20 2020 2020 2020 2020 2020  div>.           
+00002840: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002850: 2020 2020 203c 6469 7620 636c 6173 733d       <div class=
+00002860: 227b 2520 626c 6f63 6b20 315f 6d69 645f  "{% block 1_mid_
+00002870: 746f 705f 6163 5f63 2025 7d63 6f6c 2d31  top_ac_c %}col-1
+00002880: 3220 636f 6c2d 6d64 2d36 7b25 2065 6e64  2 col-md-6{% end
+00002890: 626c 6f63 6b20 257d 223e 7b7b 2031 5f6d  block %}">{{ 1_m
+000028a0: 6964 5f74 6f70 5f63 207d 7d3c 2f64 6976  id_top_c }}</div
+000028b0: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
+000028c0: 2020 2020 2020 2020 2020 2020 2020 7b25                {%
+000028d0: 2065 6c69 6620 315f 6d69 645f 746f 705f   elif 1_mid_top_
+000028e0: 6220 616e 6420 315f 6d69 645f 746f 705f  b and 1_mid_top_
+000028f0: 6320 257d 0a20 2020 2020 2020 2020 2020  c %}.           
+00002900: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002910: 2020 2020 203c 6469 7620 636c 6173 733d       <div class=
+00002920: 227b 2520 626c 6f63 6b20 315f 6d69 645f  "{% block 1_mid_
+00002930: 746f 705f 6263 5f62 2025 7d63 6f6c 2d31  top_bc_b %}col-1
+00002940: 3220 636f 6c2d 6d64 2d34 7b25 2065 6e64  2 col-md-4{% end
+00002950: 626c 6f63 6b20 257d 223e 7b7b 2031 5f6d  block %}">{{ 1_m
+00002960: 6964 5f74 6f70 5f62 207d 7d3c 2f64 6976  id_top_b }}</div
+00002970: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
+00002980: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002990: 2020 3c64 6976 2063 6c61 7373 3d22 7b25    <div class="{%
+000029a0: 2062 6c6f 636b 2031 5f6d 6964 5f74 6f70   block 1_mid_top
+000029b0: 5f62 635f 6320 257d 636f 6c2d 3132 2063  _bc_c %}col-12 c
+000029c0: 6f6c 2d6d 642d 387b 2520 656e 6462 6c6f  ol-md-8{% endblo
+000029d0: 636b 2025 7d22 3e7b 7b20 315f 6d69 645f  ck %}">{{ 1_mid_
+000029e0: 746f 705f 6320 7d7d 3c2f 6469 763e 0a20  top_c }}</div>. 
+000029f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002a00: 2020 2020 2020 2020 2020 207b 2520 656c             {% el
+00002a10: 7365 2025 7d0a 2020 2020 2020 2020 2020  se %}.          
+00002a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002a30: 2020 2020 2020 3c64 6976 2063 6c61 7373        <div class
+00002a40: 3d22 636f 6c2d 3132 223e 7b7b 2031 5f6d  ="col-12">{{ 1_m
+00002a50: 6964 5f74 6f70 5f61 207d 7d7b 7b20 315f  id_top_a }}{{ 1_
+00002a60: 6d69 645f 746f 705f 6220 7d7d 7b7b 2031  mid_top_b }}{{ 1
+00002a70: 5f6d 6964 5f74 6f70 5f63 207d 7d3c 2f64  _mid_top_c }}</d
+00002a80: 6976 3e0a 2020 2020 2020 2020 2020 2020  iv>.            
+00002a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002aa0: 7b25 2065 6e64 6966 2025 7d0a 2020 2020  {% endif %}.    
+00002ab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002ac0: 2020 2020 3c2f 6469 763e 0a20 2020 2020      </div>.     
+00002ad0: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+00002ae0: 2f64 6976 3e0a 2020 2020 2020 2020 2020  /div>.          
+00002af0: 2020 2020 2020 2020 2020 7b25 2065 6e64            {% end
+00002b00: 6966 2025 7d0a 2020 2020 2020 2020 2020  if %}.          
+00002b10: 2020 2020 2020 2020 2020 3c21 2d2d 2065            <!-- e
+00002b20: 6e64 204d 6964 646c 6520 546f 7020 2d2d  nd Middle Top --
+00002b30: 3e0a 0a20 2020 2020 2020 2020 2020 2020  >..             
+00002b40: 2020 2020 2020 203c 212d 2d20 426c 6f63         <!-- Bloc
+00002b50: 6b73 2069 6e20 6365 6e74 6572 2070 6f73  ks in center pos
+00002b60: 6974 696f 6e73 202d 2d3e 0a20 2020 2020  itions -->.     
+00002b70: 2020 2020 2020 2020 2020 2020 2020 207b                 {
+00002b80: 2520 6966 2031 5f63 656e 7465 725f 746f  % if 1_center_to
+00002b90: 705f 6120 6f72 2031 5f63 656e 7465 725f  p_a or 1_center_
+00002ba0: 746f 705f 6220 6f72 2031 5f63 656e 7465  top_b or 1_cente
+00002bb0: 725f 746f 705f 6320 6f72 2031 5f63 656e  r_top_c or 1_cen
+00002bc0: 7465 725f 6d69 645f 746f 705f 6120 6f72  ter_mid_top_a or
+00002bd0: 2031 5f63 656e 7465 725f 6d69 645f 746f   1_center_mid_to
+00002be0: 705f 6220 6f72 2031 5f63 656e 7465 725f  p_b or 1_center_
+00002bf0: 6d69 645f 746f 705f 6320 6f72 2031 5f63  mid_top_c or 1_c
+00002c00: 656e 7465 725f 636f 6e74 656e 7420 6f72  enter_content or
+00002c10: 2031 5f63 656e 7465 725f 6d69 645f 626f   1_center_mid_bo
+00002c20: 7474 6f6d 5f61 206f 7220 315f 6365 6e74  ttom_a or 1_cent
+00002c30: 6572 5f6d 6964 5f62 6f74 746f 6d5f 6220  er_mid_bottom_b 
+00002c40: 6f72 2031 5f63 656e 7465 725f 6d69 645f  or 1_center_mid_
+00002c50: 626f 7474 6f6d 5f63 206f 7220 315f 6365  bottom_c or 1_ce
+00002c60: 6e74 6572 5f62 6f74 746f 6d5f 6120 6f72  nter_bottom_a or
+00002c70: 2031 5f63 656e 7465 725f 626f 7474 6f6d   1_center_bottom
+00002c80: 5f62 206f 7220 315f 6365 6e74 6572 5f62  _b or 1_center_b
+00002c90: 6f74 746f 6d5f 6320 257d 0a0a 2020 2020  ottom_c %}..    
 00002ca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002cc0: 2020 2020 3c64 6976 2063 6c61 7373 3d22      <div class="
-00002cd0: 636f 6c2d 3132 223e 7b7b 2031 5f6c 6566  col-12">{{ 1_lef
-00002ce0: 745f 6120 7d7d 3c2f 6469 763e 0a20 2020  t_a }}</div>.   
-00002cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002d10: 207b 2520 656c 7365 2025 7d0a 2020 2020   {% else %}.    
-00002d20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002d40: 3c64 6976 2063 6c61 7373 3d22 636f 6c2d  <div class="col-
-00002d50: 3132 223e 7b7b 2031 5f6c 6566 745f 6220  12">{{ 1_left_b 
-00002d60: 7d7d 3c2f 6469 763e 0a20 2020 2020 2020  }}</div>.       
-00002d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002d80: 2020 2020 2020 2020 2020 2020 207b 2520               {% 
-00002d90: 656e 6469 6620 257d 0a20 2020 2020 2020  endif %}.       
-00002da0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002db0: 2020 2020 2020 2020 203c 2f64 6976 3e0a           </div>.
-00002dc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002dd0: 2020 2020 2020 2020 2020 2020 3c2f 6469              </di
-00002de0: 763e 0a20 2020 2020 2020 2020 2020 2020  v>.             
-00002df0: 2020 2020 2020 2020 2020 207b 2520 656e             {% en
-00002e00: 6469 6620 257d 0a20 2020 2020 2020 2020  dif %}.         
-00002e10: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-00002e20: 212d 2d20 656e 6420 426c 6f63 6b73 2069  !-- end Blocks i
-00002e30: 6e20 6c65 6674 2063 6f6c 756d 6e20 2d2d  n left column --
-00002e40: 3e0a 0a20 2020 2020 2020 2020 2020 2020  >..             
-00002e50: 2020 2020 2020 2020 2020 203c 212d 2d20             <!-- 
-00002e60: 426c 6f63 6b73 2069 6e20 4365 6e74 6572  Blocks in Center
-00002e70: 2063 6f6c 756d 6e20 2874 616b 6573 2061   column (takes a
-00002e80: 7661 696c 6162 6c65 2073 7061 6365 2920  vailable space) 
-00002e90: 2d2d 3e0a 2020 2020 2020 2020 2020 2020  -->.            
-00002ea0: 2020 2020 2020 2020 2020 2020 7b25 2069              {% i
-00002eb0: 6620 315f 6c65 6674 5f61 2061 6e64 2031  f 1_left_a and 1
-00002ec0: 5f6c 6566 745f 6220 616e 6420 315f 7269  _left_b and 1_ri
-00002ed0: 6768 745f 6120 616e 6420 315f 7269 6768  ght_a and 1_righ
-00002ee0: 745f 6220 257d 0a20 2020 2020 2020 2020  t_b %}.         
-00002ef0: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-00002f00: 6469 7620 636c 6173 733d 227b 2520 626c  div class="{% bl
-00002f10: 6f63 6b20 315f 6365 6e74 6572 5f6c 6566  ock 1_center_lef
-00002f20: 745f 6162 5f72 6967 6874 5f61 6220 257d  t_ab_right_ab %}
-00002f30: 636f 6c2d 3132 2063 6f6c 2d6c 672d 347b  col-12 col-lg-4{
-00002f40: 2520 656e 6462 6c6f 636b 2025 7d22 3e0a  % endblock %}">.
-00002f50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002f60: 2020 2020 2020 2020 7b25 2065 6c69 6620          {% elif 
-00002f70: 315f 6c65 6674 5f61 2061 6e64 2031 5f6c  1_left_a and 1_l
-00002f80: 6566 745f 6220 616e 6420 315f 7269 6768  eft_b and 1_righ
-00002f90: 745f 6120 257d 0a20 2020 2020 2020 2020  t_a %}.         
-00002fa0: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-00002fb0: 6469 7620 636c 6173 733d 227b 2520 626c  div class="{% bl
-00002fc0: 6f63 6b20 315f 6365 6e74 6572 5f6c 6566  ock 1_center_lef
-00002fd0: 745f 6162 5f72 6967 6874 5f61 2025 7d63  t_ab_right_a %}c
-00002fe0: 6f6c 2d31 3220 636f 6c2d 6c67 2d35 7b25  ol-12 col-lg-5{%
-00002ff0: 2065 6e64 626c 6f63 6b20 257d 223e 0a20   endblock %}">. 
+00002cb0: 2020 2020 3c21 2d2d 2042 6c6f 636b 7320      <!-- Blocks 
+00002cc0: 696e 206c 6566 7420 636f 6c75 6d6e 202d  in left column -
+00002cd0: 2d3e 0a20 2020 2020 2020 2020 2020 2020  ->.             
+00002ce0: 2020 2020 2020 2020 2020 207b 2520 6966             {% if
+00002cf0: 2031 5f6c 6566 745f 6120 6f72 2031 5f6c   1_left_a or 1_l
+00002d00: 6566 745f 6220 257d 0a20 2020 2020 2020  eft_b %}.       
+00002d10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002d20: 2020 2020 207b 2520 6966 2031 5f6c 6566       {% if 1_lef
+00002d30: 745f 6120 616e 6420 315f 6c65 6674 5f62  t_a and 1_left_b
+00002d40: 2025 7d0a 2020 2020 2020 2020 2020 2020   %}.            
+00002d50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002d60: 3c64 6976 2063 6c61 7373 3d22 7b25 2062  <div class="{% b
+00002d70: 6c6f 636b 2031 5f6c 6566 745f 6162 2025  lock 1_left_ab %
+00002d80: 7d63 6f6c 2d31 3220 636f 6c2d 6c67 2d34  }col-12 col-lg-4
+00002d90: 206d 622d 3520 6d62 2d6c 672d 307b 2520   mb-5 mb-lg-0{% 
+00002da0: 656e 6462 6c6f 636b 2025 7d22 3e0a 2020  endblock %}">.  
+00002db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002dc0: 2020 2020 2020 2020 2020 7b25 2065 6c69            {% eli
+00002dd0: 6620 315f 6c65 6674 5f61 2025 7d0a 2020  f 1_left_a %}.  
+00002de0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002df0: 2020 2020 2020 2020 2020 3c64 6976 2063            <div c
+00002e00: 6c61 7373 3d22 7b25 2062 6c6f 636b 2031  lass="{% block 1
+00002e10: 5f6c 6566 745f 6120 257d 636f 6c2d 3132  _left_a %}col-12
+00002e20: 2063 6f6c 2d6c 672d 3320 6d62 2d35 206d   col-lg-3 mb-5 m
+00002e30: 622d 6c67 2d30 7b25 2065 6e64 626c 6f63  b-lg-0{% endbloc
+00002e40: 6b20 257d 223e 0a20 2020 2020 2020 2020  k %}">.         
+00002e50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002e60: 2020 207b 2520 656c 7365 2025 7d0a 2020     {% else %}.  
+00002e70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002e80: 2020 2020 2020 2020 2020 3c64 6976 2063            <div c
+00002e90: 6c61 7373 3d22 7b25 2062 6c6f 636b 2031  lass="{% block 1
+00002ea0: 5f6c 6566 745f 6220 257d 636f 6c2d 3132  _left_b %}col-12
+00002eb0: 2063 6f6c 2d6c 672d 3320 6d62 2d35 206d   col-lg-3 mb-5 m
+00002ec0: 622d 6c67 2d30 7b25 2065 6e64 626c 6f63  b-lg-0{% endbloc
+00002ed0: 6b20 257d 223e 0a20 2020 2020 2020 2020  k %}">.         
+00002ee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002ef0: 2020 207b 2520 656e 6469 6620 257d 0a20     {% endif %}. 
+00002f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002f10: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+00002f20: 6469 7620 636c 6173 733d 2272 6f77 223e  div class="row">
+00002f30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002f40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002f50: 2020 2020 207b 2520 6966 2031 5f6c 6566       {% if 1_lef
+00002f60: 745f 6120 616e 6420 315f 6c65 6674 5f62  t_a and 1_left_b
+00002f70: 2025 7d0a 2020 2020 2020 2020 2020 2020   %}.            
+00002f80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002f90: 2020 2020 2020 2020 3c64 6976 2063 6c61          <div cla
+00002fa0: 7373 3d22 7b25 2062 6c6f 636b 2031 5f6c  ss="{% block 1_l
+00002fb0: 6566 745f 6162 5f61 2025 7d63 6f6c 2d31  eft_ab_a %}col-1
+00002fc0: 3220 636f 6c2d 6c67 2d36 7b25 2065 6e64  2 col-lg-6{% end
+00002fd0: 626c 6f63 6b20 257d 223e 7b7b 2031 5f6c  block %}">{{ 1_l
+00002fe0: 6566 745f 6120 7d7d 3c2f 6469 763e 0a20  eft_a }}</div>. 
+00002ff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00003000: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003010: 2020 2020 2020 207b 2520 656c 6966 2031         {% elif 1
-00003020: 5f6c 6566 745f 6120 616e 6420 315f 6c65  _left_a and 1_le
-00003030: 6674 5f62 2061 6e64 2031 5f72 6967 6874  ft_b and 1_right
-00003040: 5f62 2025 7d0a 2020 2020 2020 2020 2020  _b %}.          
-00003050: 2020 2020 2020 2020 2020 2020 2020 3c64                <d
-00003060: 6976 2063 6c61 7373 3d22 7b25 2062 6c6f  iv class="{% blo
-00003070: 636b 2031 5f63 656e 7465 725f 6c65 6674  ck 1_center_left
-00003080: 5f61 625f 7269 6768 745f 6220 257d 636f  _ab_right_b %}co
-00003090: 6c2d 3132 2063 6f6c 2d6c 672d 347b 2520  l-12 col-lg-4{% 
-000030a0: 656e 6462 6c6f 636b 2025 7d22 3e0a 2020  endblock %}">.  
+00003010: 2020 203c 6469 7620 636c 6173 733d 227b     <div class="{
+00003020: 2520 626c 6f63 6b20 315f 6c65 6674 5f61  % block 1_left_a
+00003030: 625f 6220 257d 636f 6c2d 3132 2063 6f6c  b_b %}col-12 col
+00003040: 2d6c 672d 367b 2520 656e 6462 6c6f 636b  -lg-6{% endblock
+00003050: 2025 7d22 3e7b 7b20 315f 6c65 6674 5f62   %}">{{ 1_left_b
+00003060: 207d 7d3c 2f64 6976 3e0a 2020 2020 2020   }}</div>.      
+00003070: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003080: 2020 2020 2020 2020 2020 2020 2020 7b25                {%
+00003090: 2065 6c69 6620 315f 6c65 6674 5f61 2025   elif 1_left_a %
+000030a0: 7d0a 2020 2020 2020 2020 2020 2020 2020  }.              
 000030b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000030c0: 2020 2020 2020 7b25 2065 6c69 6620 315f        {% elif 1_
-000030d0: 6c65 6674 5f61 2061 6e64 2031 5f72 6967  left_a and 1_rig
-000030e0: 6874 5f61 2061 6e64 2031 5f72 6967 6874  ht_a and 1_right
-000030f0: 5f62 2025 7d0a 2020 2020 2020 2020 2020  _b %}.          
-00003100: 2020 2020 2020 2020 2020 2020 2020 3c64                <d
-00003110: 6976 2063 6c61 7373 3d22 7b25 2062 6c6f  iv class="{% blo
-00003120: 636b 2031 5f63 656e 7465 725f 6c65 6674  ck 1_center_left
-00003130: 5f61 5f72 6967 6874 5f61 6220 257d 636f  _a_right_ab %}co
-00003140: 6c2d 3132 2063 6f6c 2d6c 672d 357b 2520  l-12 col-lg-5{% 
-00003150: 656e 6462 6c6f 636b 2025 7d22 3e0a 2020  endblock %}">.  
-00003160: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003170: 2020 2020 2020 7b25 2065 6c69 6620 315f        {% elif 1_
-00003180: 6c65 6674 5f61 2061 6e64 2031 5f72 6967  left_a and 1_rig
-00003190: 6874 5f61 2025 7d0a 2020 2020 2020 2020  ht_a %}.        
+000030c0: 2020 2020 2020 3c64 6976 2063 6c61 7373        <div class
+000030d0: 3d22 636f 6c2d 3132 223e 7b7b 2031 5f6c  ="col-12">{{ 1_l
+000030e0: 6566 745f 6120 7d7d 3c2f 6469 763e 0a20  eft_a }}</div>. 
+000030f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003100: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003110: 2020 207b 2520 656c 7365 2025 7d0a 2020     {% else %}.  
+00003120: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003130: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003140: 2020 3c64 6976 2063 6c61 7373 3d22 636f    <div class="co
+00003150: 6c2d 3132 223e 7b7b 2031 5f6c 6566 745f  l-12">{{ 1_left_
+00003160: 6220 7d7d 3c2f 6469 763e 0a20 2020 2020  b }}</div>.     
+00003170: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003180: 2020 2020 2020 2020 2020 2020 2020 207b                 {
+00003190: 2520 656e 6469 6620 257d 0a20 2020 2020  % endif %}.     
 000031a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000031b0: 3c64 6976 2063 6c61 7373 3d22 7b25 2062  <div class="{% b
-000031c0: 6c6f 636b 2031 5f63 656e 7465 725f 6c65  lock 1_center_le
-000031d0: 6674 5f61 5f72 6967 6874 5f61 2025 7d63  ft_a_right_a %}c
-000031e0: 6f6c 2d31 3220 636f 6c2d 6c67 2d36 7b25  ol-12 col-lg-6{%
-000031f0: 2065 6e64 626c 6f63 6b20 257d 223e 0a20   endblock %}">. 
-00003200: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003210: 2020 2020 2020 207b 2520 656c 6966 2031         {% elif 1
-00003220: 5f6c 6566 745f 6120 616e 6420 315f 7269  _left_a and 1_ri
-00003230: 6768 745f 6220 257d 0a20 2020 2020 2020  ght_b %}.       
-00003240: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003250: 203c 6469 7620 636c 6173 733d 227b 2520   <div class="{% 
-00003260: 626c 6f63 6b20 315f 6365 6e74 6572 5f6c  block 1_center_l
-00003270: 6566 745f 615f 7269 6768 745f 6220 257d  eft_a_right_b %}
-00003280: 636f 6c2d 3132 2063 6f6c 2d6c 672d 357b  col-12 col-lg-5{
-00003290: 2520 656e 6462 6c6f 636b 2025 7d22 3e0a  % endblock %}">.
-000032a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000032b0: 2020 2020 2020 2020 7b25 2065 6c69 6620          {% elif 
-000032c0: 315f 6c65 6674 5f62 2061 6e64 2031 5f72  1_left_b and 1_r
-000032d0: 6967 6874 5f61 2061 6e64 2031 5f72 6967  ight_a and 1_rig
-000032e0: 6874 5f62 2025 7d0a 2020 2020 2020 2020  ht_b %}.        
+000031b0: 2020 2020 2020 2020 2020 203c 2f64 6976             </div
+000031c0: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
+000031d0: 2020 2020 2020 2020 2020 2020 2020 3c2f                </
+000031e0: 6469 763e 0a20 2020 2020 2020 2020 2020  div>.           
+000031f0: 2020 2020 2020 2020 2020 2020 207b 2520               {% 
+00003200: 656e 6469 6620 257d 0a20 2020 2020 2020  endif %}.       
+00003210: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003220: 203c 212d 2d20 656e 6420 426c 6f63 6b73   <!-- end Blocks
+00003230: 2069 6e20 6c65 6674 2063 6f6c 756d 6e20   in left column 
+00003240: 2d2d 3e0a 0a20 2020 2020 2020 2020 2020  -->..           
+00003250: 2020 2020 2020 2020 2020 2020 203c 212d               <!-
+00003260: 2d20 426c 6f63 6b73 2069 6e20 4365 6e74  - Blocks in Cent
+00003270: 6572 2063 6f6c 756d 6e20 2874 616b 6573  er column (takes
+00003280: 2061 7661 696c 6162 6c65 2073 7061 6365   available space
+00003290: 2920 2d2d 3e0a 2020 2020 2020 2020 2020  ) -->.          
+000032a0: 2020 2020 2020 2020 2020 2020 2020 7b25                {%
+000032b0: 2069 6620 315f 6c65 6674 5f61 2061 6e64   if 1_left_a and
+000032c0: 2031 5f6c 6566 745f 6220 616e 6420 315f   1_left_b and 1_
+000032d0: 7269 6768 745f 6120 616e 6420 315f 7269  right_a and 1_ri
+000032e0: 6768 745f 6220 257d 0a20 2020 2020 2020  ght_b %}.       
 000032f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003300: 3c64 6976 2063 6c61 7373 3d22 7b25 2062  <div class="{% b
-00003310: 6c6f 636b 2031 5f63 656e 7465 725f 6c65  lock 1_center_le
-00003320: 6674 5f62 5f72 6967 6874 5f61 6220 257d  ft_b_right_ab %}
-00003330: 636f 6c2d 3132 2063 6f6c 2d6c 672d 3420  col-12 col-lg-4 
-00003340: 6f66 6673 6574 2d6c 672d 317b 2520 656e  offset-lg-1{% en
-00003350: 6462 6c6f 636b 2025 7d22 3e0a 2020 2020  dblock %}">.    
-00003360: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003370: 2020 2020 7b25 2065 6c69 6620 315f 6c65      {% elif 1_le
-00003380: 6674 5f62 2061 6e64 2031 5f72 6967 6874  ft_b and 1_right
-00003390: 5f61 2025 7d0a 2020 2020 2020 2020 2020  _a %}.          
-000033a0: 2020 2020 2020 2020 2020 2020 2020 3c64                <d
-000033b0: 6976 2063 6c61 7373 3d22 7b25 2062 6c6f  iv class="{% blo
-000033c0: 636b 2031 5f63 656e 7465 725f 6c65 6674  ck 1_center_left
-000033d0: 5f62 5f72 6967 6874 5f61 2025 7d63 6f6c  _b_right_a %}col
-000033e0: 2d31 3220 636f 6c2d 6c67 2d35 206f 6666  -12 col-lg-5 off
-000033f0: 7365 742d 6c67 2d31 7b25 2065 6e64 626c  set-lg-1{% endbl
-00003400: 6f63 6b20 257d 223e 0a20 2020 2020 2020  ock %}">.       
-00003410: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003420: 207b 2520 656c 6966 2031 5f6c 6566 745f   {% elif 1_left_
-00003430: 6220 616e 6420 315f 7269 6768 745f 6220  b and 1_right_b 
-00003440: 257d 0a20 2020 2020 2020 2020 2020 2020  %}.             
-00003450: 2020 2020 2020 2020 2020 203c 6469 7620             <div 
-00003460: 636c 6173 733d 227b 2520 626c 6f63 6b20  class="{% block 
-00003470: 315f 6365 6e74 6572 5f6c 6566 745f 625f  1_center_left_b_
-00003480: 7269 6768 745f 6220 257d 636f 6c2d 3132  right_b %}col-12
-00003490: 2063 6f6c 2d6c 672d 3420 6f66 6673 6574   col-lg-4 offset
-000034a0: 2d6c 672d 317b 2520 656e 6462 6c6f 636b  -lg-1{% endblock
-000034b0: 2025 7d22 3e0a 2020 2020 2020 2020 2020   %}">.          
-000034c0: 2020 2020 2020 2020 2020 2020 2020 7b25                {%
-000034d0: 2065 6c69 6620 315f 6c65 6674 5f61 2061   elif 1_left_a a
-000034e0: 6e64 2031 5f6c 6566 745f 6220 257d 0a20  nd 1_left_b %}. 
-000034f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003500: 2020 2020 2020 203c 6469 7620 636c 6173         <div clas
-00003510: 733d 227b 2520 626c 6f63 6b20 315f 6365  s="{% block 1_ce
-00003520: 6e74 6572 5f6c 6566 745f 6162 2025 7d63  nter_left_ab %}c
-00003530: 6f6c 2d31 3220 636f 6c2d 6c67 2d38 7b25  ol-12 col-lg-8{%
-00003540: 2065 6e64 626c 6f63 6b20 257d 223e 0a20   endblock %}">. 
-00003550: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003560: 2020 2020 2020 207b 2520 656c 6966 2031         {% elif 1
-00003570: 5f6c 6566 745f 6120 257d 0a20 2020 2020  _left_a %}.     
-00003580: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003590: 2020 203c 6469 7620 636c 6173 733d 227b     <div class="{
-000035a0: 2520 626c 6f63 6b20 315f 6365 6e74 6572  % block 1_center
-000035b0: 5f6c 6566 745f 6120 257d 636f 6c2d 3132  _left_a %}col-12
-000035c0: 2063 6f6c 2d6c 672d 397b 2520 656e 6462   col-lg-9{% endb
-000035d0: 6c6f 636b 2025 7d22 3e0a 2020 2020 2020  lock %}">.      
-000035e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000035f0: 2020 7b25 2065 6c69 6620 315f 6c65 6674    {% elif 1_left
-00003600: 5f62 2025 7d0a 2020 2020 2020 2020 2020  _b %}.          
-00003610: 2020 2020 2020 2020 2020 2020 2020 3c64                <d
-00003620: 6976 2063 6c61 7373 3d22 7b25 2062 6c6f  iv class="{% blo
-00003630: 636b 2031 5f63 656e 7465 725f 6c65 6674  ck 1_center_left
-00003640: 5f62 2025 7d63 6f6c 2d31 3220 636f 6c2d  _b %}col-12 col-
-00003650: 6c67 2d38 206f 6666 7365 742d 6c67 2d31  lg-8 offset-lg-1
-00003660: 7b25 2065 6e64 626c 6f63 6b20 257d 223e  {% endblock %}">
-00003670: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00003680: 2020 2020 2020 2020 207b 2520 656c 6966           {% elif
-00003690: 2031 5f72 6967 6874 5f61 2061 6e64 2031   1_right_a and 1
-000036a0: 5f72 6967 6874 5f62 2025 7d0a 2020 2020  _right_b %}.    
-000036b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000036c0: 2020 2020 3c64 6976 2063 6c61 7373 3d22      <div class="
-000036d0: 7b25 2062 6c6f 636b 2031 5f63 656e 7465  {% block 1_cente
-000036e0: 725f 7269 6768 745f 6162 2025 7d63 6f6c  r_right_ab %}col
-000036f0: 2d31 3220 636f 6c2d 6c67 2d38 7b25 2065  -12 col-lg-8{% e
-00003700: 6e64 626c 6f63 6b20 257d 223e 0a20 2020  ndblock %}">.   
-00003710: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003720: 2020 2020 207b 2520 656c 6966 2031 5f72       {% elif 1_r
-00003730: 6967 6874 5f61 2025 7d0a 2020 2020 2020  ight_a %}.      
-00003740: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003750: 2020 3c64 6976 2063 6c61 7373 3d22 7b25    <div class="{%
-00003760: 2062 6c6f 636b 2031 5f63 656e 7465 725f   block 1_center_
-00003770: 7269 6768 745f 6120 257d 636f 6c2d 3132  right_a %}col-12
-00003780: 2063 6f6c 2d6c 672d 397b 2520 656e 6462   col-lg-9{% endb
-00003790: 6c6f 636b 2025 7d22 3e0a 2020 2020 2020  lock %}">.      
+00003300: 203c 6469 7620 636c 6173 733d 227b 2520   <div class="{% 
+00003310: 626c 6f63 6b20 315f 6365 6e74 6572 5f6c  block 1_center_l
+00003320: 6566 745f 6162 5f72 6967 6874 5f61 6220  eft_ab_right_ab 
+00003330: 257d 636f 6c2d 3132 2063 6f6c 2d6c 672d  %}col-12 col-lg-
+00003340: 347b 2520 656e 6462 6c6f 636b 2025 7d22  4{% endblock %}"
+00003350: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
+00003360: 2020 2020 2020 2020 2020 7b25 2065 6c69            {% eli
+00003370: 6620 315f 6c65 6674 5f61 2061 6e64 2031  f 1_left_a and 1
+00003380: 5f6c 6566 745f 6220 616e 6420 315f 7269  _left_b and 1_ri
+00003390: 6768 745f 6120 257d 0a20 2020 2020 2020  ght_a %}.       
+000033a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000033b0: 203c 6469 7620 636c 6173 733d 227b 2520   <div class="{% 
+000033c0: 626c 6f63 6b20 315f 6365 6e74 6572 5f6c  block 1_center_l
+000033d0: 6566 745f 6162 5f72 6967 6874 5f61 2025  eft_ab_right_a %
+000033e0: 7d63 6f6c 2d31 3220 636f 6c2d 6c67 2d35  }col-12 col-lg-5
+000033f0: 7b25 2065 6e64 626c 6f63 6b20 257d 223e  {% endblock %}">
+00003400: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00003410: 2020 2020 2020 2020 207b 2520 656c 6966           {% elif
+00003420: 2031 5f6c 6566 745f 6120 616e 6420 315f   1_left_a and 1_
+00003430: 6c65 6674 5f62 2061 6e64 2031 5f72 6967  left_b and 1_rig
+00003440: 6874 5f62 2025 7d0a 2020 2020 2020 2020  ht_b %}.        
+00003450: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003460: 3c64 6976 2063 6c61 7373 3d22 7b25 2062  <div class="{% b
+00003470: 6c6f 636b 2031 5f63 656e 7465 725f 6c65  lock 1_center_le
+00003480: 6674 5f61 625f 7269 6768 745f 6220 257d  ft_ab_right_b %}
+00003490: 636f 6c2d 3132 2063 6f6c 2d6c 672d 347b  col-12 col-lg-4{
+000034a0: 2520 656e 6462 6c6f 636b 2025 7d22 3e0a  % endblock %}">.
+000034b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000034c0: 2020 2020 2020 2020 7b25 2065 6c69 6620          {% elif 
+000034d0: 315f 6c65 6674 5f61 2061 6e64 2031 5f72  1_left_a and 1_r
+000034e0: 6967 6874 5f61 2061 6e64 2031 5f72 6967  ight_a and 1_rig
+000034f0: 6874 5f62 2025 7d0a 2020 2020 2020 2020  ht_b %}.        
+00003500: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003510: 3c64 6976 2063 6c61 7373 3d22 7b25 2062  <div class="{% b
+00003520: 6c6f 636b 2031 5f63 656e 7465 725f 6c65  lock 1_center_le
+00003530: 6674 5f61 5f72 6967 6874 5f61 6220 257d  ft_a_right_ab %}
+00003540: 636f 6c2d 3132 2063 6f6c 2d6c 672d 357b  col-12 col-lg-5{
+00003550: 2520 656e 6462 6c6f 636b 2025 7d22 3e0a  % endblock %}">.
+00003560: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003570: 2020 2020 2020 2020 7b25 2065 6c69 6620          {% elif 
+00003580: 315f 6c65 6674 5f61 2061 6e64 2031 5f72  1_left_a and 1_r
+00003590: 6967 6874 5f61 2025 7d0a 2020 2020 2020  ight_a %}.      
+000035a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000035b0: 2020 3c64 6976 2063 6c61 7373 3d22 7b25    <div class="{%
+000035c0: 2062 6c6f 636b 2031 5f63 656e 7465 725f   block 1_center_
+000035d0: 6c65 6674 5f61 5f72 6967 6874 5f61 2025  left_a_right_a %
+000035e0: 7d63 6f6c 2d31 3220 636f 6c2d 6c67 2d36  }col-12 col-lg-6
+000035f0: 7b25 2065 6e64 626c 6f63 6b20 257d 223e  {% endblock %}">
+00003600: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00003610: 2020 2020 2020 2020 207b 2520 656c 6966           {% elif
+00003620: 2031 5f6c 6566 745f 6120 616e 6420 315f   1_left_a and 1_
+00003630: 7269 6768 745f 6220 257d 0a20 2020 2020  right_b %}.     
+00003640: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003650: 2020 203c 6469 7620 636c 6173 733d 227b     <div class="{
+00003660: 2520 626c 6f63 6b20 315f 6365 6e74 6572  % block 1_center
+00003670: 5f6c 6566 745f 615f 7269 6768 745f 6220  _left_a_right_b 
+00003680: 257d 636f 6c2d 3132 2063 6f6c 2d6c 672d  %}col-12 col-lg-
+00003690: 357b 2520 656e 6462 6c6f 636b 2025 7d22  5{% endblock %}"
+000036a0: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
+000036b0: 2020 2020 2020 2020 2020 7b25 2065 6c69            {% eli
+000036c0: 6620 315f 6c65 6674 5f62 2061 6e64 2031  f 1_left_b and 1
+000036d0: 5f72 6967 6874 5f61 2061 6e64 2031 5f72  _right_a and 1_r
+000036e0: 6967 6874 5f62 2025 7d0a 2020 2020 2020  ight_b %}.      
+000036f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003700: 2020 3c64 6976 2063 6c61 7373 3d22 7b25    <div class="{%
+00003710: 2062 6c6f 636b 2031 5f63 656e 7465 725f   block 1_center_
+00003720: 6c65 6674 5f62 5f72 6967 6874 5f61 6220  left_b_right_ab 
+00003730: 257d 636f 6c2d 3132 2063 6f6c 2d6c 672d  %}col-12 col-lg-
+00003740: 3420 6f66 6673 6574 2d6c 672d 317b 2520  4 offset-lg-1{% 
+00003750: 656e 6462 6c6f 636b 2025 7d22 3e0a 2020  endblock %}">.  
+00003760: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003770: 2020 2020 2020 7b25 2065 6c69 6620 315f        {% elif 1_
+00003780: 6c65 6674 5f62 2061 6e64 2031 5f72 6967  left_b and 1_rig
+00003790: 6874 5f61 2025 7d0a 2020 2020 2020 2020  ht_a %}.        
 000037a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000037b0: 2020 7b25 2065 6c69 6620 315f 7269 6768    {% elif 1_righ
-000037c0: 745f 6220 257d 0a20 2020 2020 2020 2020  t_b %}.         
-000037d0: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-000037e0: 6469 7620 636c 6173 733d 227b 2520 626c  div class="{% bl
-000037f0: 6f63 6b20 315f 6365 6e74 6572 5f72 6967  ock 1_center_rig
-00003800: 6874 5f62 2025 7d63 6f6c 2d31 3220 636f  ht_b %}col-12 co
-00003810: 6c2d 6c67 2d38 7b25 2065 6e64 626c 6f63  l-lg-8{% endbloc
-00003820: 6b20 257d 223e 0a20 2020 2020 2020 2020  k %}">.         
-00003830: 2020 2020 2020 2020 2020 2020 2020 207b                 {
-00003840: 2520 656c 7365 2025 7d0a 2020 2020 2020  % else %}.      
-00003850: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003860: 2020 3c64 6976 2063 6c61 7373 3d22 7b25    <div class="{%
-00003870: 2062 6c6f 636b 2031 5f63 656e 7465 7220   block 1_center 
-00003880: 257d 636f 6c2d 3132 7b25 2065 6e64 626c  %}col-12{% endbl
-00003890: 6f63 6b20 257d 223e 0a20 2020 2020 2020  ock %}">.       
-000038a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000038b0: 207b 2520 656e 6469 6620 257d 0a20 2020   {% endif %}.   
+000037b0: 3c64 6976 2063 6c61 7373 3d22 7b25 2062  <div class="{% b
+000037c0: 6c6f 636b 2031 5f63 656e 7465 725f 6c65  lock 1_center_le
+000037d0: 6674 5f62 5f72 6967 6874 5f61 2025 7d63  ft_b_right_a %}c
+000037e0: 6f6c 2d31 3220 636f 6c2d 6c67 2d35 206f  ol-12 col-lg-5 o
+000037f0: 6666 7365 742d 6c67 2d31 7b25 2065 6e64  ffset-lg-1{% end
+00003800: 626c 6f63 6b20 257d 223e 0a20 2020 2020  block %}">.     
+00003810: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003820: 2020 207b 2520 656c 6966 2031 5f6c 6566     {% elif 1_lef
+00003830: 745f 6220 616e 6420 315f 7269 6768 745f  t_b and 1_right_
+00003840: 6220 257d 0a20 2020 2020 2020 2020 2020  b %}.           
+00003850: 2020 2020 2020 2020 2020 2020 203c 6469               <di
+00003860: 7620 636c 6173 733d 227b 2520 626c 6f63  v class="{% bloc
+00003870: 6b20 315f 6365 6e74 6572 5f6c 6566 745f  k 1_center_left_
+00003880: 625f 7269 6768 745f 6220 257d 636f 6c2d  b_right_b %}col-
+00003890: 3132 2063 6f6c 2d6c 672d 3420 6f66 6673  12 col-lg-4 offs
+000038a0: 6574 2d6c 672d 317b 2520 656e 6462 6c6f  et-lg-1{% endblo
+000038b0: 636b 2025 7d22 3e0a 2020 2020 2020 2020  ck %}">.        
 000038c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000038d0: 2020 2020 203c 212d 2d20 456e 6420 426c       <!-- End Bl
-000038e0: 6f63 6b73 2069 6e20 4365 6e74 6572 2063  ocks in Center c
-000038f0: 6f6c 756d 6e20 2874 616b 6573 2061 7661  olumn (takes ava
-00003900: 696c 6162 6c65 2073 7061 6365 2920 2d2d  ilable space) --
-00003910: 3e0a 0a20 2020 2020 2020 2020 2020 2020  >..             
-00003920: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-00003930: 212d 2d20 4365 6e74 6572 2074 6f70 202d  !-- Center top -
-00003940: 2d3e 0a20 2020 2020 2020 2020 2020 2020  ->.             
-00003950: 2020 2020 2020 2020 2020 2020 2020 207b                 {
-00003960: 2520 6966 2031 5f63 656e 7465 725f 746f  % if 1_center_to
-00003970: 705f 6120 6f72 2031 5f63 656e 7465 725f  p_a or 1_center_
-00003980: 746f 705f 6220 6f72 2031 5f63 656e 7465  top_b or 1_cente
-00003990: 725f 746f 705f 6320 257d 0a20 2020 2020  r_top_c %}.     
-000039a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000039b0: 2020 2020 2020 203c 6469 7620 636c 6173         <div clas
-000039c0: 733d 2272 6f77 223e 0a20 2020 2020 2020  s="row">.       
-000039d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000039e0: 2020 2020 2020 2020 207b 2520 6966 2031           {% if 1
-000039f0: 5f63 656e 7465 725f 746f 705f 6120 616e  _center_top_a an
-00003a00: 6420 315f 6365 6e74 6572 5f74 6f70 5f62  d 1_center_top_b
-00003a10: 2061 6e64 2031 5f63 656e 7465 725f 746f   and 1_center_to
-00003a20: 705f 6320 257d 0a20 2020 2020 2020 2020  p_c %}.         
-00003a30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003a40: 2020 2020 2020 2020 2020 203c 6469 7620             <div 
-00003a50: 636c 6173 733d 227b 2520 626c 6f63 6b20  class="{% block 
-00003a60: 315f 6365 6e74 6572 5f74 6f70 5f61 6263  1_center_top_abc
-00003a70: 5f61 2025 7d63 6f6c 2d31 3220 636f 6c2d  _a %}col-12 col-
-00003a80: 6d64 2d34 7b25 2065 6e64 626c 6f63 6b20  md-4{% endblock 
-00003a90: 257d 223e 7b7b 2031 5f63 656e 7465 725f  %}">{{ 1_center_
-00003aa0: 746f 705f 6120 7d7d 3c2f 6469 763e 0a20  top_a }}</div>. 
+000038d0: 7b25 2065 6c69 6620 315f 6c65 6674 5f61  {% elif 1_left_a
+000038e0: 2061 6e64 2031 5f6c 6566 745f 6220 257d   and 1_left_b %}
+000038f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00003900: 2020 2020 2020 2020 203c 6469 7620 636c           <div cl
+00003910: 6173 733d 227b 2520 626c 6f63 6b20 315f  ass="{% block 1_
+00003920: 6365 6e74 6572 5f6c 6566 745f 6162 2025  center_left_ab %
+00003930: 7d63 6f6c 2d31 3220 636f 6c2d 6c67 2d38  }col-12 col-lg-8
+00003940: 7b25 2065 6e64 626c 6f63 6b20 257d 223e  {% endblock %}">
+00003950: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00003960: 2020 2020 2020 2020 207b 2520 656c 6966           {% elif
+00003970: 2031 5f6c 6566 745f 6120 257d 0a20 2020   1_left_a %}.   
+00003980: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003990: 2020 2020 203c 6469 7620 636c 6173 733d       <div class=
+000039a0: 227b 2520 626c 6f63 6b20 315f 6365 6e74  "{% block 1_cent
+000039b0: 6572 5f6c 6566 745f 6120 257d 636f 6c2d  er_left_a %}col-
+000039c0: 3132 2063 6f6c 2d6c 672d 397b 2520 656e  12 col-lg-9{% en
+000039d0: 6462 6c6f 636b 2025 7d22 3e0a 2020 2020  dblock %}">.    
+000039e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000039f0: 2020 2020 7b25 2065 6c69 6620 315f 6c65      {% elif 1_le
+00003a00: 6674 5f62 2025 7d0a 2020 2020 2020 2020  ft_b %}.        
+00003a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003a20: 3c64 6976 2063 6c61 7373 3d22 7b25 2062  <div class="{% b
+00003a30: 6c6f 636b 2031 5f63 656e 7465 725f 6c65  lock 1_center_le
+00003a40: 6674 5f62 2025 7d63 6f6c 2d31 3220 636f  ft_b %}col-12 co
+00003a50: 6c2d 6c67 2d38 206f 6666 7365 742d 6c67  l-lg-8 offset-lg
+00003a60: 2d31 7b25 2065 6e64 626c 6f63 6b20 257d  -1{% endblock %}
+00003a70: 223e 0a20 2020 2020 2020 2020 2020 2020  ">.             
+00003a80: 2020 2020 2020 2020 2020 207b 2520 656c             {% el
+00003a90: 6966 2031 5f72 6967 6874 5f61 2061 6e64  if 1_right_a and
+00003aa0: 2031 5f72 6967 6874 5f62 2025 7d0a 2020   1_right_b %}.  
 00003ab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003ad0: 2020 203c 6469 7620 636c 6173 733d 227b     <div class="{
-00003ae0: 2520 626c 6f63 6b20 315f 6365 6e74 6572  % block 1_center
-00003af0: 5f74 6f70 5f61 6263 5f62 2025 7d63 6f6c  _top_abc_b %}col
-00003b00: 2d31 3220 636f 6c2d 6d64 2d34 7b25 2065  -12 col-md-4{% e
-00003b10: 6e64 626c 6f63 6b20 257d 223e 7b7b 2031  ndblock %}">{{ 1
-00003b20: 5f63 656e 7465 725f 746f 705f 6220 7d7d  _center_top_b }}
-00003b30: 3c2f 6469 763e 0a20 2020 2020 2020 2020  </div>.         
+00003ac0: 2020 2020 2020 3c64 6976 2063 6c61 7373        <div class
+00003ad0: 3d22 7b25 2062 6c6f 636b 2031 5f63 656e  ="{% block 1_cen
+00003ae0: 7465 725f 7269 6768 745f 6162 2025 7d63  ter_right_ab %}c
+00003af0: 6f6c 2d31 3220 636f 6c2d 6c67 2d38 7b25  ol-12 col-lg-8{%
+00003b00: 2065 6e64 626c 6f63 6b20 257d 223e 0a20   endblock %}">. 
+00003b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003b20: 2020 2020 2020 207b 2520 656c 6966 2031         {% elif 1
+00003b30: 5f72 6967 6874 5f61 2025 7d0a 2020 2020  _right_a %}.    
 00003b40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003b50: 2020 2020 2020 2020 2020 203c 6469 7620             <div 
-00003b60: 636c 6173 733d 227b 2520 626c 6f63 6b20  class="{% block 
-00003b70: 315f 6365 6e74 6572 5f74 6f70 5f61 6263  1_center_top_abc
-00003b80: 5f63 2025 7d63 6f6c 2d31 3220 636f 6c2d  _c %}col-12 col-
-00003b90: 6d64 2d34 7b25 2065 6e64 626c 6f63 6b20  md-4{% endblock 
-00003ba0: 257d 223e 7b7b 2031 5f63 656e 7465 725f  %}">{{ 1_center_
-00003bb0: 746f 705f 6320 7d7d 3c2f 6469 763e 0a20  top_c }}</div>. 
-00003bc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003bd0: 2020 2020 2020 2020 2020 2020 2020 207b                 {
-00003be0: 2520 656c 6966 2031 5f63 656e 7465 725f  % elif 1_center_
-00003bf0: 746f 705f 6120 616e 6420 315f 6365 6e74  top_a and 1_cent
-00003c00: 6572 5f74 6f70 5f62 2025 7d0a 2020 2020  er_top_b %}.    
-00003c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003c30: 3c64 6976 2063 6c61 7373 3d22 7b25 2062  <div class="{% b
-00003c40: 6c6f 636b 2031 5f63 656e 7465 725f 746f  lock 1_center_to
-00003c50: 705f 6162 5f61 2025 7d63 6f6c 2d31 3220  p_ab_a %}col-12 
-00003c60: 636f 6c2d 6d64 2d38 7b25 2065 6e64 626c  col-md-8{% endbl
-00003c70: 6f63 6b20 257d 223e 7b7b 2031 5f63 656e  ock %}">{{ 1_cen
-00003c80: 7465 725f 746f 705f 6120 7d7d 3c2f 6469  ter_top_a }}</di
-00003c90: 763e 0a20 2020 2020 2020 2020 2020 2020  v>.             
+00003b50: 2020 2020 3c64 6976 2063 6c61 7373 3d22      <div class="
+00003b60: 7b25 2062 6c6f 636b 2031 5f63 656e 7465  {% block 1_cente
+00003b70: 725f 7269 6768 745f 6120 257d 636f 6c2d  r_right_a %}col-
+00003b80: 3132 2063 6f6c 2d6c 672d 397b 2520 656e  12 col-lg-9{% en
+00003b90: 6462 6c6f 636b 2025 7d22 3e0a 2020 2020  dblock %}">.    
+00003ba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003bb0: 2020 2020 7b25 2065 6c69 6620 315f 7269      {% elif 1_ri
+00003bc0: 6768 745f 6220 257d 0a20 2020 2020 2020  ght_b %}.       
+00003bd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003be0: 203c 6469 7620 636c 6173 733d 227b 2520   <div class="{% 
+00003bf0: 626c 6f63 6b20 315f 6365 6e74 6572 5f72  block 1_center_r
+00003c00: 6967 6874 5f62 2025 7d63 6f6c 2d31 3220  ight_b %}col-12 
+00003c10: 636f 6c2d 6c67 2d38 7b25 2065 6e64 626c  col-lg-8{% endbl
+00003c20: 6f63 6b20 257d 223e 0a20 2020 2020 2020  ock %}">.       
+00003c30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003c40: 207b 2520 656c 7365 2025 7d0a 2020 2020   {% else %}.    
+00003c50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003c60: 2020 2020 3c64 6976 2063 6c61 7373 3d22      <div class="
+00003c70: 7b25 2062 6c6f 636b 2031 5f63 656e 7465  {% block 1_cente
+00003c80: 7220 257d 636f 6c2d 3132 7b25 2065 6e64  r %}col-12{% end
+00003c90: 626c 6f63 6b20 257d 223e 0a20 2020 2020  block %}">.     
 00003ca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003cb0: 2020 2020 2020 203c 6469 7620 636c 6173         <div clas
-00003cc0: 733d 227b 2520 626c 6f63 6b20 315f 6365  s="{% block 1_ce
-00003cd0: 6e74 6572 5f74 6f70 5f61 625f 6220 257d  nter_top_ab_b %}
-00003ce0: 636f 6c2d 3132 2063 6f6c 2d6d 642d 347b  col-12 col-md-4{
-00003cf0: 2520 656e 6462 6c6f 636b 2025 7d22 3e7b  % endblock %}">{
-00003d00: 7b20 315f 6365 6e74 6572 5f74 6f70 5f62  { 1_center_top_b
-00003d10: 207d 7d3c 2f64 6976 3e0a 2020 2020 2020   }}</div>.      
+00003cb0: 2020 207b 2520 656e 6469 6620 257d 0a20     {% endif %}. 
+00003cc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003cd0: 2020 2020 2020 203c 212d 2d20 456e 6420         <!-- End 
+00003ce0: 426c 6f63 6b73 2069 6e20 4365 6e74 6572  Blocks in Center
+00003cf0: 2063 6f6c 756d 6e20 2874 616b 6573 2061   column (takes a
+00003d00: 7661 696c 6162 6c65 2073 7061 6365 2920  vailable space) 
+00003d10: 2d2d 3e0a 0a20 2020 2020 2020 2020 2020  -->..           
 00003d20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003d30: 2020 2020 2020 2020 2020 7b25 2065 6c69            {% eli
-00003d40: 6620 315f 6365 6e74 6572 5f74 6f70 5f61  f 1_center_top_a
-00003d50: 2061 6e64 2031 5f63 656e 7465 725f 746f   and 1_center_to
-00003d60: 705f 6320 257d 0a20 2020 2020 2020 2020  p_c %}.         
-00003d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003d80: 2020 2020 2020 2020 2020 203c 6469 7620             <div 
-00003d90: 636c 6173 733d 227b 2520 626c 6f63 6b20  class="{% block 
-00003da0: 315f 6365 6e74 6572 5f74 6f70 5f61 635f  1_center_top_ac_
-00003db0: 6120 257d 636f 6c2d 3132 2063 6f6c 2d6d  a %}col-12 col-m
-00003dc0: 642d 367b 2520 656e 6462 6c6f 636b 2025  d-6{% endblock %
-00003dd0: 7d22 3e7b 7b20 315f 6365 6e74 6572 5f74  }">{{ 1_center_t
-00003de0: 6f70 5f61 207d 7d3c 2f64 6976 3e0a 2020  op_a }}</div>.  
-00003df0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003e00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003e10: 2020 3c64 6976 2063 6c61 7373 3d22 7b25    <div class="{%
-00003e20: 2062 6c6f 636b 2031 5f63 656e 7465 725f   block 1_center_
-00003e30: 746f 705f 6163 5f63 2025 7d63 6f6c 2d31  top_ac_c %}col-1
-00003e40: 3220 636f 6c2d 6d64 2d36 7b25 2065 6e64  2 col-md-6{% end
-00003e50: 626c 6f63 6b20 257d 223e 7b7b 2031 5f63  block %}">{{ 1_c
-00003e60: 656e 7465 725f 746f 705f 6320 7d7d 3c2f  enter_top_c }}</
-00003e70: 6469 763e 0a20 2020 2020 2020 2020 2020  div>.           
-00003e80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003e90: 2020 2020 207b 2520 656c 6966 2031 5f63       {% elif 1_c
-00003ea0: 656e 7465 725f 746f 705f 6220 616e 6420  enter_top_b and 
-00003eb0: 315f 6365 6e74 6572 5f74 6f70 5f63 2025  1_center_top_c %
-00003ec0: 7d0a 2020 2020 2020 2020 2020 2020 2020  }.              
-00003ed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003ee0: 2020 2020 2020 3c64 6976 2063 6c61 7373        <div class
-00003ef0: 3d22 7b25 2062 6c6f 636b 2031 5f63 656e  ="{% block 1_cen
-00003f00: 7465 725f 746f 705f 6263 5f62 2025 7d63  ter_top_bc_b %}c
-00003f10: 6f6c 2d31 3220 636f 6c2d 6d64 2d34 7b25  ol-12 col-md-4{%
-00003f20: 2065 6e64 626c 6f63 6b20 257d 223e 7b7b   endblock %}">{{
-00003f30: 2031 5f63 656e 7465 725f 746f 705f 6220   1_center_top_b 
-00003f40: 7d7d 3c2f 6469 763e 0a20 2020 2020 2020  }}</div>.       
-00003f50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003f60: 2020 2020 2020 2020 2020 2020 203c 6469               <di
-00003f70: 7620 636c 6173 733d 227b 2520 626c 6f63  v class="{% bloc
-00003f80: 6b20 315f 6365 6e74 6572 5f74 6f70 5f62  k 1_center_top_b
-00003f90: 635f 6320 257d 636f 6c2d 3132 2063 6f6c  c_c %}col-12 col
-00003fa0: 2d6d 642d 387b 2520 656e 6462 6c6f 636b  -md-8{% endblock
-00003fb0: 2025 7d22 3e7b 7b20 315f 6365 6e74 6572   %}">{{ 1_center
-00003fc0: 5f74 6f70 5f63 207d 7d3c 2f64 6976 3e0a  _top_c }}</div>.
+00003d30: 203c 212d 2d20 4365 6e74 6572 2074 6f70   <!-- Center top
+00003d40: 202d 2d3e 0a20 2020 2020 2020 2020 2020   -->.           
+00003d50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003d60: 207b 2520 6966 2031 5f63 656e 7465 725f   {% if 1_center_
+00003d70: 746f 705f 6120 6f72 2031 5f63 656e 7465  top_a or 1_cente
+00003d80: 725f 746f 705f 6220 6f72 2031 5f63 656e  r_top_b or 1_cen
+00003d90: 7465 725f 746f 705f 6320 257d 0a20 2020  ter_top_c %}.   
+00003da0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003db0: 2020 2020 2020 2020 203c 6469 7620 636c           <div cl
+00003dc0: 6173 733d 2272 6f77 223e 0a20 2020 2020  ass="row">.     
+00003dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003de0: 2020 2020 2020 2020 2020 207b 2520 6966             {% if
+00003df0: 2031 5f63 656e 7465 725f 746f 705f 6120   1_center_top_a 
+00003e00: 616e 6420 315f 6365 6e74 6572 5f74 6f70  and 1_center_top
+00003e10: 5f62 2061 6e64 2031 5f63 656e 7465 725f  _b and 1_center_
+00003e20: 746f 705f 6320 257d 0a20 2020 2020 2020  top_c %}.       
+00003e30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003e40: 2020 2020 2020 2020 2020 2020 203c 6469               <di
+00003e50: 7620 636c 6173 733d 227b 2520 626c 6f63  v class="{% bloc
+00003e60: 6b20 315f 6365 6e74 6572 5f74 6f70 5f61  k 1_center_top_a
+00003e70: 6263 5f61 2025 7d63 6f6c 2d31 3220 636f  bc_a %}col-12 co
+00003e80: 6c2d 6d64 2d34 7b25 2065 6e64 626c 6f63  l-md-4{% endbloc
+00003e90: 6b20 257d 223e 7b7b 2031 5f63 656e 7465  k %}">{{ 1_cente
+00003ea0: 725f 746f 705f 6120 7d7d 3c2f 6469 763e  r_top_a }}</div>
+00003eb0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00003ec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003ed0: 2020 2020 203c 6469 7620 636c 6173 733d       <div class=
+00003ee0: 227b 2520 626c 6f63 6b20 315f 6365 6e74  "{% block 1_cent
+00003ef0: 6572 5f74 6f70 5f61 6263 5f62 2025 7d63  er_top_abc_b %}c
+00003f00: 6f6c 2d31 3220 636f 6c2d 6d64 2d34 7b25  ol-12 col-md-4{%
+00003f10: 2065 6e64 626c 6f63 6b20 257d 223e 7b7b   endblock %}">{{
+00003f20: 2031 5f63 656e 7465 725f 746f 705f 6220   1_center_top_b 
+00003f30: 7d7d 3c2f 6469 763e 0a20 2020 2020 2020  }}</div>.       
+00003f40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003f50: 2020 2020 2020 2020 2020 2020 203c 6469               <di
+00003f60: 7620 636c 6173 733d 227b 2520 626c 6f63  v class="{% bloc
+00003f70: 6b20 315f 6365 6e74 6572 5f74 6f70 5f61  k 1_center_top_a
+00003f80: 6263 5f63 2025 7d63 6f6c 2d31 3220 636f  bc_c %}col-12 co
+00003f90: 6c2d 6d64 2d34 7b25 2065 6e64 626c 6f63  l-md-4{% endbloc
+00003fa0: 6b20 257d 223e 7b7b 2031 5f63 656e 7465  k %}">{{ 1_cente
+00003fb0: 725f 746f 705f 6320 7d7d 3c2f 6469 763e  r_top_c }}</div>
+00003fc0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
 00003fd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003fe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003ff0: 7b25 2065 6c73 6520 257d 0a20 2020 2020  {% else %}.     
-00004000: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004010: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-00004020: 6469 7620 636c 6173 733d 2263 6f6c 2d31  div class="col-1
-00004030: 3222 3e7b 7b20 315f 6365 6e74 6572 5f74  2">{{ 1_center_t
-00004040: 6f70 5f61 207d 7d7b 7b20 315f 6365 6e74  op_a }}{{ 1_cent
-00004050: 6572 5f74 6f70 5f62 207d 7d7b 7b20 315f  er_top_b }}{{ 1_
-00004060: 6365 6e74 6572 5f74 6f70 5f63 207d 7d3c  center_top_c }}<
-00004070: 2f64 6976 3e0a 2020 2020 2020 2020 2020  /div>.          
-00004080: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004090: 2020 2020 2020 7b25 2065 6e64 6966 2025        {% endif %
-000040a0: 7d0a 2020 2020 2020 2020 2020 2020 2020  }.              
-000040b0: 2020 2020 2020 2020 2020 2020 2020 3c2f                </
-000040c0: 6469 763e 0a20 2020 2020 2020 2020 2020  div>.           
-000040d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000040e0: 207b 2520 656e 6469 6620 257d 0a20 2020   {% endif %}.   
-000040f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004100: 2020 2020 2020 2020 203c 212d 2d20 454e           <!-- EN
-00004110: 4420 4365 6e74 6572 2074 6f70 202d 2d3e  D Center top -->
-00004120: 0a0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00004130: 2020 2020 2020 2020 2020 2020 2020 3c21                <!
-00004140: 2d2d 2043 656e 7465 7220 6d69 642d 746f  -- Center mid-to
-00004150: 7020 2d2d 3e0a 2020 2020 2020 2020 2020  p -->.          
-00004160: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004170: 2020 7b25 2069 6620 315f 6365 6e74 6572    {% if 1_center
-00004180: 5f6d 6964 5f74 6f70 5f61 206f 7220 315f  _mid_top_a or 1_
-00004190: 6365 6e74 6572 5f6d 6964 5f74 6f70 5f62  center_mid_top_b
-000041a0: 206f 7220 315f 6365 6e74 6572 5f74 6f70   or 1_center_top
-000041b0: 5f63 2025 7d0a 2020 2020 2020 2020 2020  _c %}.          
-000041c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000041d0: 2020 3c64 6976 2063 6c61 7373 3d22 726f    <div class="ro
-000041e0: 7722 3e0a 2020 2020 2020 2020 2020 2020  w">.            
+00003fe0: 207b 2520 656c 6966 2031 5f63 656e 7465   {% elif 1_cente
+00003ff0: 725f 746f 705f 6120 616e 6420 315f 6365  r_top_a and 1_ce
+00004000: 6e74 6572 5f74 6f70 5f62 2025 7d0a 2020  nter_top_b %}.  
+00004010: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004020: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004030: 2020 3c64 6976 2063 6c61 7373 3d22 7b25    <div class="{%
+00004040: 2062 6c6f 636b 2031 5f63 656e 7465 725f   block 1_center_
+00004050: 746f 705f 6162 5f61 2025 7d63 6f6c 2d31  top_ab_a %}col-1
+00004060: 3220 636f 6c2d 6d64 2d38 7b25 2065 6e64  2 col-md-8{% end
+00004070: 626c 6f63 6b20 257d 223e 7b7b 2031 5f63  block %}">{{ 1_c
+00004080: 656e 7465 725f 746f 705f 6120 7d7d 3c2f  enter_top_a }}</
+00004090: 6469 763e 0a20 2020 2020 2020 2020 2020  div>.           
+000040a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000040b0: 2020 2020 2020 2020 203c 6469 7620 636c           <div cl
+000040c0: 6173 733d 227b 2520 626c 6f63 6b20 315f  ass="{% block 1_
+000040d0: 6365 6e74 6572 5f74 6f70 5f61 625f 6220  center_top_ab_b 
+000040e0: 257d 636f 6c2d 3132 2063 6f6c 2d6d 642d  %}col-12 col-md-
+000040f0: 347b 2520 656e 6462 6c6f 636b 2025 7d22  4{% endblock %}"
+00004100: 3e7b 7b20 315f 6365 6e74 6572 5f74 6f70  >{{ 1_center_top
+00004110: 5f62 207d 7d3c 2f64 6976 3e0a 2020 2020  _b }}</div>.    
+00004120: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004130: 2020 2020 2020 2020 2020 2020 7b25 2065              {% e
+00004140: 6c69 6620 315f 6365 6e74 6572 5f74 6f70  lif 1_center_top
+00004150: 5f61 2061 6e64 2031 5f63 656e 7465 725f  _a and 1_center_
+00004160: 746f 705f 6320 257d 0a20 2020 2020 2020  top_c %}.       
+00004170: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004180: 2020 2020 2020 2020 2020 2020 203c 6469               <di
+00004190: 7620 636c 6173 733d 227b 2520 626c 6f63  v class="{% bloc
+000041a0: 6b20 315f 6365 6e74 6572 5f74 6f70 5f61  k 1_center_top_a
+000041b0: 635f 6120 257d 636f 6c2d 3132 2063 6f6c  c_a %}col-12 col
+000041c0: 2d6d 642d 367b 2520 656e 6462 6c6f 636b  -md-6{% endblock
+000041d0: 2025 7d22 3e7b 7b20 315f 6365 6e74 6572   %}">{{ 1_center
+000041e0: 5f74 6f70 5f61 207d 7d3c 2f64 6976 3e0a  _top_a }}</div>.
 000041f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004200: 2020 2020 7b25 2069 6620 315f 6365 6e74      {% if 1_cent
-00004210: 6572 5f6d 6964 5f74 6f70 5f61 2061 6e64  er_mid_top_a and
-00004220: 2031 5f63 656e 7465 725f 6d69 645f 746f   1_center_mid_to
-00004230: 705f 6220 616e 6420 315f 6365 6e74 6572  p_b and 1_center
-00004240: 5f6d 6964 5f74 6f70 5f63 2025 7d0a 2020  _mid_top_c %}.  
-00004250: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004260: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004270: 2020 3c64 6976 2063 6c61 7373 3d22 7b25    <div class="{%
-00004280: 2062 6c6f 636b 2031 5f63 656e 7465 725f   block 1_center_
-00004290: 6d69 645f 746f 705f 6162 635f 6120 257d  mid_top_abc_a %}
-000042a0: 636f 6c2d 3132 2063 6f6c 2d6d 642d 347b  col-12 col-md-4{
-000042b0: 2520 656e 6462 6c6f 636b 2025 7d22 3e7b  % endblock %}">{
-000042c0: 7b20 315f 6365 6e74 6572 5f6d 6964 5f74  { 1_center_mid_t
-000042d0: 6f70 5f61 207d 7d3c 2f64 6976 3e0a 2020  op_a }}</div>.  
-000042e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000042f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004300: 2020 3c64 6976 2063 6c61 7373 3d22 7b25    <div class="{%
-00004310: 2062 6c6f 636b 2031 5f63 656e 7465 725f   block 1_center_
-00004320: 6d69 645f 746f 705f 6162 635f 6220 257d  mid_top_abc_b %}
-00004330: 636f 6c2d 3132 2063 6f6c 2d6d 642d 347b  col-12 col-md-4{
-00004340: 2520 656e 6462 6c6f 636b 2025 7d22 3e7b  % endblock %}">{
-00004350: 7b20 315f 6365 6e74 6572 5f6d 6964 5f74  { 1_center_mid_t
-00004360: 6f70 5f62 207d 7d3c 2f64 6976 3e0a 2020  op_b }}</div>.  
-00004370: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004380: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004390: 2020 3c64 6976 2063 6c61 7373 3d22 7b25    <div class="{%
-000043a0: 2062 6c6f 636b 2031 5f63 656e 7465 725f   block 1_center_
-000043b0: 6d69 645f 746f 705f 6162 635f 6320 257d  mid_top_abc_c %}
-000043c0: 636f 6c2d 3132 2063 6f6c 2d6d 642d 347b  col-12 col-md-4{
-000043d0: 2520 656e 6462 6c6f 636b 2025 7d22 3e7b  % endblock %}">{
-000043e0: 7b20 315f 6365 6e74 6572 5f6d 6964 5f74  { 1_center_mid_t
-000043f0: 6f70 5f63 207d 7d3c 2f64 6976 3e0a 2020  op_c }}</div>.  
+00004200: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004210: 2020 2020 3c64 6976 2063 6c61 7373 3d22      <div class="
+00004220: 7b25 2062 6c6f 636b 2031 5f63 656e 7465  {% block 1_cente
+00004230: 725f 746f 705f 6163 5f63 2025 7d63 6f6c  r_top_ac_c %}col
+00004240: 2d31 3220 636f 6c2d 6d64 2d36 7b25 2065  -12 col-md-6{% e
+00004250: 6e64 626c 6f63 6b20 257d 223e 7b7b 2031  ndblock %}">{{ 1
+00004260: 5f63 656e 7465 725f 746f 705f 6320 7d7d  _center_top_c }}
+00004270: 3c2f 6469 763e 0a20 2020 2020 2020 2020  </div>.         
+00004280: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004290: 2020 2020 2020 207b 2520 656c 6966 2031         {% elif 1
+000042a0: 5f63 656e 7465 725f 746f 705f 6220 616e  _center_top_b an
+000042b0: 6420 315f 6365 6e74 6572 5f74 6f70 5f63  d 1_center_top_c
+000042c0: 2025 7d0a 2020 2020 2020 2020 2020 2020   %}.            
+000042d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000042e0: 2020 2020 2020 2020 3c64 6976 2063 6c61          <div cla
+000042f0: 7373 3d22 7b25 2062 6c6f 636b 2031 5f63  ss="{% block 1_c
+00004300: 656e 7465 725f 746f 705f 6263 5f62 2025  enter_top_bc_b %
+00004310: 7d63 6f6c 2d31 3220 636f 6c2d 6d64 2d34  }col-12 col-md-4
+00004320: 7b25 2065 6e64 626c 6f63 6b20 257d 223e  {% endblock %}">
+00004330: 7b7b 2031 5f63 656e 7465 725f 746f 705f  {{ 1_center_top_
+00004340: 6220 7d7d 3c2f 6469 763e 0a20 2020 2020  b }}</div>.     
+00004350: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004360: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+00004370: 6469 7620 636c 6173 733d 227b 2520 626c  div class="{% bl
+00004380: 6f63 6b20 315f 6365 6e74 6572 5f74 6f70  ock 1_center_top
+00004390: 5f62 635f 6320 257d 636f 6c2d 3132 2063  _bc_c %}col-12 c
+000043a0: 6f6c 2d6d 642d 387b 2520 656e 6462 6c6f  ol-md-8{% endblo
+000043b0: 636b 2025 7d22 3e7b 7b20 315f 6365 6e74  ck %}">{{ 1_cent
+000043c0: 6572 5f74 6f70 5f63 207d 7d3c 2f64 6976  er_top_c }}</div
+000043d0: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
+000043e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000043f0: 2020 7b25 2065 6c73 6520 257d 0a20 2020    {% else %}.   
 00004400: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004410: 2020 2020 2020 2020 2020 2020 2020 7b25                {%
-00004420: 2065 6c69 6620 315f 6365 6e74 6572 5f6d   elif 1_center_m
-00004430: 6964 5f74 6f70 5f61 2061 6e64 2031 5f63  id_top_a and 1_c
-00004440: 656e 7465 725f 6d69 645f 746f 705f 6220  enter_mid_top_b 
-00004450: 257d 0a20 2020 2020 2020 2020 2020 2020  %}.             
-00004460: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004470: 2020 2020 2020 203c 6469 7620 636c 6173         <div clas
-00004480: 733d 227b 2520 626c 6f63 6b20 315f 6365  s="{% block 1_ce
-00004490: 6e74 6572 5f6d 6964 5f74 6f70 5f61 625f  nter_mid_top_ab_
-000044a0: 6120 257d 636f 6c2d 3132 2063 6f6c 2d6d  a %}col-12 col-m
-000044b0: 642d 387b 2520 656e 6462 6c6f 636b 2025  d-8{% endblock %
-000044c0: 7d22 3e7b 7b20 315f 6365 6e74 6572 5f6d  }">{{ 1_center_m
-000044d0: 6964 5f74 6f70 5f61 207d 7d3c 2f64 6976  id_top_a }}</div
-000044e0: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
+00004410: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004420: 203c 6469 7620 636c 6173 733d 2263 6f6c   <div class="col
+00004430: 2d31 3222 3e7b 7b20 315f 6365 6e74 6572  -12">{{ 1_center
+00004440: 5f74 6f70 5f61 207d 7d7b 7b20 315f 6365  _top_a }}{{ 1_ce
+00004450: 6e74 6572 5f74 6f70 5f62 207d 7d7b 7b20  nter_top_b }}{{ 
+00004460: 315f 6365 6e74 6572 5f74 6f70 5f63 207d  1_center_top_c }
+00004470: 7d3c 2f64 6976 3e0a 2020 2020 2020 2020  }</div>.        
+00004480: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004490: 2020 2020 2020 2020 7b25 2065 6e64 6966          {% endif
+000044a0: 2025 7d0a 2020 2020 2020 2020 2020 2020   %}.            
+000044b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000044c0: 3c2f 6469 763e 0a20 2020 2020 2020 2020  </div>.         
+000044d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000044e0: 2020 207b 2520 656e 6469 6620 257d 0a20     {% endif %}. 
 000044f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004500: 2020 2020 2020 3c64 6976 2063 6c61 7373        <div class
-00004510: 3d22 7b25 2062 6c6f 636b 2031 5f63 656e  ="{% block 1_cen
-00004520: 7465 725f 6d69 645f 746f 705f 6162 5f62  ter_mid_top_ab_b
-00004530: 2025 7d63 6f6c 2d31 3220 636f 6c2d 6d64   %}col-12 col-md
-00004540: 2d34 7b25 2065 6e64 626c 6f63 6b20 257d  -4{% endblock %}
-00004550: 223e 7b7b 2031 5f63 656e 7465 725f 6d69  ">{{ 1_center_mi
-00004560: 645f 746f 705f 6220 7d7d 3c2f 6469 763e  d_top_b }}</div>
-00004570: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00004580: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004590: 207b 2520 656c 6966 2031 5f63 656e 7465   {% elif 1_cente
-000045a0: 725f 6d69 645f 746f 705f 6120 616e 6420  r_mid_top_a and 
-000045b0: 315f 6365 6e74 6572 5f6d 6964 5f74 6f70  1_center_mid_top
-000045c0: 5f63 2025 7d0a 2020 2020 2020 2020 2020  _c %}.          
-000045d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000045e0: 2020 2020 2020 2020 2020 3c64 6976 2063            <div c
-000045f0: 6c61 7373 3d22 7b25 2062 6c6f 636b 2031  lass="{% block 1
-00004600: 5f63 656e 7465 725f 6d69 645f 746f 705f  _center_mid_top_
-00004610: 6163 5f61 2025 7d63 6f6c 2d31 3220 636f  ac_a %}col-12 co
-00004620: 6c2d 6d64 2d36 7b25 2065 6e64 626c 6f63  l-md-6{% endbloc
-00004630: 6b20 257d 223e 7b7b 2031 5f63 656e 7465  k %}">{{ 1_cente
-00004640: 725f 6d69 645f 746f 705f 6120 7d7d 3c2f  r_mid_top_a }}</
-00004650: 6469 763e 0a20 2020 2020 2020 2020 2020  div>.           
+00004500: 2020 2020 2020 2020 2020 203c 212d 2d20             <!-- 
+00004510: 454e 4420 4365 6e74 6572 2074 6f70 202d  END Center top -
+00004520: 2d3e 0a0a 2020 2020 2020 2020 2020 2020  ->..            
+00004530: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004540: 3c21 2d2d 2043 656e 7465 7220 6d69 642d  <!-- Center mid-
+00004550: 746f 7020 2d2d 3e0a 2020 2020 2020 2020  top -->.        
+00004560: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004570: 2020 2020 7b25 2069 6620 315f 6365 6e74      {% if 1_cent
+00004580: 6572 5f6d 6964 5f74 6f70 5f61 206f 7220  er_mid_top_a or 
+00004590: 315f 6365 6e74 6572 5f6d 6964 5f74 6f70  1_center_mid_top
+000045a0: 5f62 206f 7220 315f 6365 6e74 6572 5f74  _b or 1_center_t
+000045b0: 6f70 5f63 2025 7d0a 2020 2020 2020 2020  op_c %}.        
+000045c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000045d0: 2020 2020 3c64 6976 2063 6c61 7373 3d22      <div class="
+000045e0: 726f 7722 3e0a 2020 2020 2020 2020 2020  row">.          
+000045f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004600: 2020 2020 2020 7b25 2069 6620 315f 6365        {% if 1_ce
+00004610: 6e74 6572 5f6d 6964 5f74 6f70 5f61 2061  nter_mid_top_a a
+00004620: 6e64 2031 5f63 656e 7465 725f 6d69 645f  nd 1_center_mid_
+00004630: 746f 705f 6220 616e 6420 315f 6365 6e74  top_b and 1_cent
+00004640: 6572 5f6d 6964 5f74 6f70 5f63 2025 7d0a  er_mid_top_c %}.
+00004650: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00004660: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004670: 2020 2020 2020 2020 203c 6469 7620 636c           <div cl
-00004680: 6173 733d 227b 2520 626c 6f63 6b20 315f  ass="{% block 1_
-00004690: 6365 6e74 6572 5f6d 6964 5f74 6f70 5f61  center_mid_top_a
-000046a0: 635f 6320 257d 636f 6c2d 3132 2063 6f6c  c_c %}col-12 col
-000046b0: 2d6d 642d 367b 2520 656e 6462 6c6f 636b  -md-6{% endblock
-000046c0: 2025 7d22 3e7b 7b20 315f 6365 6e74 6572   %}">{{ 1_center
-000046d0: 5f6d 6964 5f74 6f70 5f63 207d 7d3c 2f64  _mid_top_c }}</d
-000046e0: 6976 3e0a 2020 2020 2020 2020 2020 2020  iv>.            
+00004670: 2020 2020 3c64 6976 2063 6c61 7373 3d22      <div class="
+00004680: 7b25 2062 6c6f 636b 2031 5f63 656e 7465  {% block 1_cente
+00004690: 725f 6d69 645f 746f 705f 6162 635f 6120  r_mid_top_abc_a 
+000046a0: 257d 636f 6c2d 3132 2063 6f6c 2d6d 642d  %}col-12 col-md-
+000046b0: 347b 2520 656e 6462 6c6f 636b 2025 7d22  4{% endblock %}"
+000046c0: 3e7b 7b20 315f 6365 6e74 6572 5f6d 6964  >{{ 1_center_mid
+000046d0: 5f74 6f70 5f61 207d 7d3c 2f64 6976 3e0a  _top_a }}</div>.
+000046e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000046f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004700: 2020 2020 7b25 2065 6c69 6620 315f 6365      {% elif 1_ce
-00004710: 6e74 6572 5f6d 6964 5f74 6f70 5f62 2061  nter_mid_top_b a
-00004720: 6e64 2031 5f63 656e 7465 725f 6d69 645f  nd 1_center_mid_
-00004730: 746f 705f 6320 257d 0a20 2020 2020 2020  top_c %}.       
-00004740: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004750: 2020 2020 2020 2020 2020 2020 203c 6469               <di
-00004760: 7620 636c 6173 733d 227b 2520 626c 6f63  v class="{% bloc
-00004770: 6b20 315f 6365 6e74 6572 5f6d 6964 5f74  k 1_center_mid_t
-00004780: 6f70 5f62 635f 6220 257d 636f 6c2d 3132  op_bc_b %}col-12
-00004790: 2063 6f6c 2d6d 642d 347b 2520 656e 6462   col-md-4{% endb
-000047a0: 6c6f 636b 2025 7d22 3e7b 7b20 315f 6365  lock %}">{{ 1_ce
-000047b0: 6e74 6572 5f6d 6964 5f74 6f70 5f62 207d  nter_mid_top_b }
-000047c0: 7d3c 2f64 6976 3e0a 2020 2020 2020 2020  }</div>.        
-000047d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000047e0: 2020 2020 2020 2020 2020 2020 3c64 6976              <div
-000047f0: 2063 6c61 7373 3d22 7b25 2062 6c6f 636b   class="{% block
-00004800: 2031 5f63 656e 7465 725f 6d69 645f 746f   1_center_mid_to
-00004810: 705f 6263 5f63 2025 7d63 6f6c 2d31 3220  p_bc_c %}col-12 
-00004820: 636f 6c2d 6d64 2d38 7b25 2065 6e64 626c  col-md-8{% endbl
-00004830: 6f63 6b20 257d 223e 7b7b 2031 5f63 656e  ock %}">{{ 1_cen
-00004840: 7465 725f 6d69 645f 746f 705f 6320 7d7d  ter_mid_top_c }}
-00004850: 3c2f 6469 763e 0a20 2020 2020 2020 2020  </div>.         
+00004700: 2020 2020 3c64 6976 2063 6c61 7373 3d22      <div class="
+00004710: 7b25 2062 6c6f 636b 2031 5f63 656e 7465  {% block 1_cente
+00004720: 725f 6d69 645f 746f 705f 6162 635f 6220  r_mid_top_abc_b 
+00004730: 257d 636f 6c2d 3132 2063 6f6c 2d6d 642d  %}col-12 col-md-
+00004740: 347b 2520 656e 6462 6c6f 636b 2025 7d22  4{% endblock %}"
+00004750: 3e7b 7b20 315f 6365 6e74 6572 5f6d 6964  >{{ 1_center_mid
+00004760: 5f74 6f70 5f62 207d 7d3c 2f64 6976 3e0a  _top_b }}</div>.
+00004770: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004780: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004790: 2020 2020 3c64 6976 2063 6c61 7373 3d22      <div class="
+000047a0: 7b25 2062 6c6f 636b 2031 5f63 656e 7465  {% block 1_cente
+000047b0: 725f 6d69 645f 746f 705f 6162 635f 6320  r_mid_top_abc_c 
+000047c0: 257d 636f 6c2d 3132 2063 6f6c 2d6d 642d  %}col-12 col-md-
+000047d0: 347b 2520 656e 6462 6c6f 636b 2025 7d22  4{% endblock %}"
+000047e0: 3e7b 7b20 315f 6365 6e74 6572 5f6d 6964  >{{ 1_center_mid
+000047f0: 5f74 6f70 5f63 207d 7d3c 2f64 6976 3e0a  _top_c }}</div>.
+00004800: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004810: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004820: 7b25 2065 6c69 6620 315f 6365 6e74 6572  {% elif 1_center
+00004830: 5f6d 6964 5f74 6f70 5f61 2061 6e64 2031  _mid_top_a and 1
+00004840: 5f63 656e 7465 725f 6d69 645f 746f 705f  _center_mid_top_
+00004850: 6220 257d 0a20 2020 2020 2020 2020 2020  b %}.           
 00004860: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004870: 2020 2020 2020 207b 2520 656c 7365 2025         {% else %
-00004880: 7d0a 2020 2020 2020 2020 2020 2020 2020  }.              
-00004890: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000048a0: 2020 2020 2020 3c64 6976 2063 6c61 7373        <div class
-000048b0: 3d22 636f 6c2d 3132 223e 7b7b 2031 5f63  ="col-12">{{ 1_c
-000048c0: 656e 7465 725f 6d69 645f 746f 705f 6120  enter_mid_top_a 
-000048d0: 7d7d 7b7b 2031 5f63 656e 7465 725f 6d69  }}{{ 1_center_mi
-000048e0: 645f 746f 705f 6220 7d7d 7b7b 2031 5f63  d_top_b }}{{ 1_c
-000048f0: 656e 7465 725f 6d69 645f 746f 705f 6320  enter_mid_top_c 
-00004900: 7d7d 3c2f 6469 763e 0a20 2020 2020 2020  }}</div>.       
-00004910: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004920: 2020 2020 2020 2020 207b 2520 656e 6469           {% endi
-00004930: 6620 257d 0a20 2020 2020 2020 2020 2020  f %}.           
-00004940: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004950: 203c 2f64 6976 3e0a 2020 2020 2020 2020   </div>.        
-00004960: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004970: 2020 2020 7b25 2065 6e64 6966 2025 7d0a      {% endif %}.
+00004870: 2020 2020 2020 2020 203c 6469 7620 636c           <div cl
+00004880: 6173 733d 227b 2520 626c 6f63 6b20 315f  ass="{% block 1_
+00004890: 6365 6e74 6572 5f6d 6964 5f74 6f70 5f61  center_mid_top_a
+000048a0: 625f 6120 257d 636f 6c2d 3132 2063 6f6c  b_a %}col-12 col
+000048b0: 2d6d 642d 387b 2520 656e 6462 6c6f 636b  -md-8{% endblock
+000048c0: 2025 7d22 3e7b 7b20 315f 6365 6e74 6572   %}">{{ 1_center
+000048d0: 5f6d 6964 5f74 6f70 5f61 207d 7d3c 2f64  _mid_top_a }}</d
+000048e0: 6976 3e0a 2020 2020 2020 2020 2020 2020  iv>.            
+000048f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004900: 2020 2020 2020 2020 3c64 6976 2063 6c61          <div cla
+00004910: 7373 3d22 7b25 2062 6c6f 636b 2031 5f63  ss="{% block 1_c
+00004920: 656e 7465 725f 6d69 645f 746f 705f 6162  enter_mid_top_ab
+00004930: 5f62 2025 7d63 6f6c 2d31 3220 636f 6c2d  _b %}col-12 col-
+00004940: 6d64 2d34 7b25 2065 6e64 626c 6f63 6b20  md-4{% endblock 
+00004950: 257d 223e 7b7b 2031 5f63 656e 7465 725f  %}">{{ 1_center_
+00004960: 6d69 645f 746f 705f 6220 7d7d 3c2f 6469  mid_top_b }}</di
+00004970: 763e 0a20 2020 2020 2020 2020 2020 2020  v>.             
 00004980: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004990: 2020 2020 2020 2020 2020 2020 3c21 2d2d              <!--
-000049a0: 2045 4e44 2043 656e 7465 7220 6d69 642d   END Center mid-
-000049b0: 746f 7020 2d2d 3e0a 0a20 2020 2020 2020  top -->..       
-000049c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000049d0: 2020 2020 203c 212d 2d20 4365 6e74 6572       <!-- Center
-000049e0: 2063 6f6e 7465 6e74 202d 2d3e 0a20 2020   content -->.   
-000049f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004a00: 2020 2020 2020 2020 207b 2520 6966 2031           {% if 1
-00004a10: 5f63 656e 7465 725f 636f 6e74 656e 7420  _center_content 
-00004a20: 257d 0a20 2020 2020 2020 2020 2020 2020  %}.             
-00004a30: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-00004a40: 6469 7620 636c 6173 733d 2272 6f77 223e  div class="row">
-00004a50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00004990: 2020 207b 2520 656c 6966 2031 5f63 656e     {% elif 1_cen
+000049a0: 7465 725f 6d69 645f 746f 705f 6120 616e  ter_mid_top_a an
+000049b0: 6420 315f 6365 6e74 6572 5f6d 6964 5f74  d 1_center_mid_t
+000049c0: 6f70 5f63 2025 7d0a 2020 2020 2020 2020  op_c %}.        
+000049d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000049e0: 2020 2020 2020 2020 2020 2020 3c64 6976              <div
+000049f0: 2063 6c61 7373 3d22 7b25 2062 6c6f 636b   class="{% block
+00004a00: 2031 5f63 656e 7465 725f 6d69 645f 746f   1_center_mid_to
+00004a10: 705f 6163 5f61 2025 7d63 6f6c 2d31 3220  p_ac_a %}col-12 
+00004a20: 636f 6c2d 6d64 2d36 7b25 2065 6e64 626c  col-md-6{% endbl
+00004a30: 6f63 6b20 257d 223e 7b7b 2031 5f63 656e  ock %}">{{ 1_cen
+00004a40: 7465 725f 6d69 645f 746f 705f 6120 7d7d  ter_mid_top_a }}
+00004a50: 3c2f 6469 763e 0a20 2020 2020 2020 2020  </div>.         
 00004a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004a70: 203c 6469 7620 636c 6173 733d 2263 6f6c   <div class="col
-00004a80: 223e 0a20 2020 2020 2020 2020 2020 2020  ">.             
-00004a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004aa0: 2020 2020 2020 207b 7b20 315f 6365 6e74         {{ 1_cent
-00004ab0: 6572 5f63 6f6e 7465 6e74 207d 7d0a 2020  er_content }}.  
-00004ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004ad0: 2020 2020 2020 2020 2020 2020 2020 3c2f                </
-00004ae0: 6469 763e 0a20 2020 2020 2020 2020 2020  div>.           
+00004a70: 2020 2020 2020 2020 2020 203c 6469 7620             <div 
+00004a80: 636c 6173 733d 227b 2520 626c 6f63 6b20  class="{% block 
+00004a90: 315f 6365 6e74 6572 5f6d 6964 5f74 6f70  1_center_mid_top
+00004aa0: 5f61 635f 6320 257d 636f 6c2d 3132 2063  _ac_c %}col-12 c
+00004ab0: 6f6c 2d6d 642d 367b 2520 656e 6462 6c6f  ol-md-6{% endblo
+00004ac0: 636b 2025 7d22 3e7b 7b20 315f 6365 6e74  ck %}">{{ 1_cent
+00004ad0: 6572 5f6d 6964 5f74 6f70 5f63 207d 7d3c  er_mid_top_c }}<
+00004ae0: 2f64 6976 3e0a 2020 2020 2020 2020 2020  /div>.          
 00004af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004b00: 203c 2f64 6976 3e0a 2020 2020 2020 2020   </div>.        
-00004b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004b20: 2020 2020 7b25 2065 6e64 6966 2025 7d0a      {% endif %}.
-00004b30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004b40: 2020 2020 2020 2020 2020 2020 3c21 2d2d              <!--
-00004b50: 2045 4e44 2043 656e 7465 7220 636f 6e74   END Center cont
-00004b60: 656e 7420 2d2d 3e0a 0a20 2020 2020 2020  ent -->..       
-00004b70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004b80: 2020 2020 203c 212d 2d20 4365 6e74 6572       <!-- Center
-00004b90: 206d 6964 2d62 6f74 746f 6d20 2d2d 3e0a   mid-bottom -->.
-00004ba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004bb0: 2020 2020 2020 2020 2020 2020 7b25 2069              {% i
-00004bc0: 6620 315f 6365 6e74 6572 5f6d 6964 5f62  f 1_center_mid_b
-00004bd0: 6f74 746f 6d5f 6120 6f72 2031 5f63 656e  ottom_a or 1_cen
-00004be0: 7465 725f 6d69 645f 626f 7474 6f6d 5f62  ter_mid_bottom_b
-00004bf0: 206f 7220 315f 6365 6e74 6572 5f6d 6964   or 1_center_mid
-00004c00: 5f62 6f74 746f 6d5f 6320 257d 0a20 2020  _bottom_c %}.   
-00004c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004c20: 2020 2020 2020 2020 203c 6469 7620 636c           <div cl
-00004c30: 6173 733d 2272 6f77 223e 0a20 2020 2020  ass="row">.     
-00004c40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004c50: 2020 2020 2020 2020 2020 207b 2520 6966             {% if
-00004c60: 2031 5f63 656e 7465 725f 6d69 645f 626f   1_center_mid_bo
-00004c70: 7474 6f6d 5f61 2061 6e64 2031 5f63 656e  ttom_a and 1_cen
-00004c80: 7465 725f 6d69 645f 626f 7474 6f6d 5f62  ter_mid_bottom_b
-00004c90: 2061 6e64 2031 5f63 656e 7465 725f 6d69   and 1_center_mi
-00004ca0: 645f 626f 7474 6f6d 5f63 2025 7d0a 2020  d_bottom_c %}.  
-00004cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004cc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004cd0: 2020 3c64 6976 2063 6c61 7373 3d22 7b25    <div class="{%
-00004ce0: 2062 6c6f 636b 2031 5f63 656e 7465 725f   block 1_center_
-00004cf0: 6d69 645f 626f 7474 6f6d 5f61 6263 5f61  mid_bottom_abc_a
-00004d00: 2025 7d63 6f6c 2d31 3220 636f 6c2d 6d64   %}col-12 col-md
-00004d10: 2d34 7b25 2065 6e64 626c 6f63 6b20 257d  -4{% endblock %}
-00004d20: 223e 7b7b 2031 5f63 656e 7465 725f 6d69  ">{{ 1_center_mi
-00004d30: 645f 626f 7474 6f6d 5f61 207d 7d3c 2f64  d_bottom_a }}</d
-00004d40: 6976 3e0a 2020 2020 2020 2020 2020 2020  iv>.            
-00004d50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004d60: 2020 2020 2020 2020 3c64 6976 2063 6c61          <div cla
-00004d70: 7373 3d22 7b25 2062 6c6f 636b 2031 5f63  ss="{% block 1_c
-00004d80: 656e 7465 725f 6d69 645f 626f 7474 6f6d  enter_mid_bottom
-00004d90: 5f61 6263 5f62 2025 7d63 6f6c 2d31 3220  _abc_b %}col-12 
-00004da0: 636f 6c2d 6d64 2d34 7b25 2065 6e64 626c  col-md-4{% endbl
-00004db0: 6f63 6b20 257d 223e 7b7b 2031 5f63 656e  ock %}">{{ 1_cen
-00004dc0: 7465 725f 6d69 645f 626f 7474 6f6d 5f62  ter_mid_bottom_b
-00004dd0: 207d 7d3c 2f64 6976 3e0a 2020 2020 2020   }}</div>.      
-00004de0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004df0: 2020 2020 2020 2020 2020 2020 2020 3c64                <d
-00004e00: 6976 2063 6c61 7373 3d22 7b25 2062 6c6f  iv class="{% blo
-00004e10: 636b 2031 5f63 656e 7465 725f 6d69 645f  ck 1_center_mid_
-00004e20: 626f 7474 6f6d 5f61 6263 5f63 2025 7d63  bottom_abc_c %}c
-00004e30: 6f6c 2d31 3220 636f 6c2d 6d64 2d34 7b25  ol-12 col-md-4{%
-00004e40: 2065 6e64 626c 6f63 6b20 257d 223e 7b7b   endblock %}">{{
-00004e50: 2031 5f63 656e 7465 725f 6d69 645f 626f   1_center_mid_bo
-00004e60: 7474 6f6d 5f63 207d 7d3c 2f64 6976 3e0a  ttom_c }}</div>.
-00004e70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004e80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004e90: 7b25 2065 6c69 6620 315f 6365 6e74 6572  {% elif 1_center
-00004ea0: 5f6d 6964 5f62 6f74 746f 6d5f 6120 616e  _mid_bottom_a an
-00004eb0: 6420 315f 6365 6e74 6572 5f6d 6964 5f62  d 1_center_mid_b
-00004ec0: 6f74 746f 6d5f 6220 257d 0a20 2020 2020  ottom_b %}.     
+00004b00: 2020 2020 2020 7b25 2065 6c69 6620 315f        {% elif 1_
+00004b10: 6365 6e74 6572 5f6d 6964 5f74 6f70 5f62  center_mid_top_b
+00004b20: 2061 6e64 2031 5f63 656e 7465 725f 6d69   and 1_center_mi
+00004b30: 645f 746f 705f 6320 257d 0a20 2020 2020  d_top_c %}.     
+00004b40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004b50: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+00004b60: 6469 7620 636c 6173 733d 227b 2520 626c  div class="{% bl
+00004b70: 6f63 6b20 315f 6365 6e74 6572 5f6d 6964  ock 1_center_mid
+00004b80: 5f74 6f70 5f62 635f 6220 257d 636f 6c2d  _top_bc_b %}col-
+00004b90: 3132 2063 6f6c 2d6d 642d 347b 2520 656e  12 col-md-4{% en
+00004ba0: 6462 6c6f 636b 2025 7d22 3e7b 7b20 315f  dblock %}">{{ 1_
+00004bb0: 6365 6e74 6572 5f6d 6964 5f74 6f70 5f62  center_mid_top_b
+00004bc0: 207d 7d3c 2f64 6976 3e0a 2020 2020 2020   }}</div>.      
+00004bd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004be0: 2020 2020 2020 2020 2020 2020 2020 3c64                <d
+00004bf0: 6976 2063 6c61 7373 3d22 7b25 2062 6c6f  iv class="{% blo
+00004c00: 636b 2031 5f63 656e 7465 725f 6d69 645f  ck 1_center_mid_
+00004c10: 746f 705f 6263 5f63 2025 7d63 6f6c 2d31  top_bc_c %}col-1
+00004c20: 3220 636f 6c2d 6d64 2d38 7b25 2065 6e64  2 col-md-8{% end
+00004c30: 626c 6f63 6b20 257d 223e 7b7b 2031 5f63  block %}">{{ 1_c
+00004c40: 656e 7465 725f 6d69 645f 746f 705f 6320  enter_mid_top_c 
+00004c50: 7d7d 3c2f 6469 763e 0a20 2020 2020 2020  }}</div>.       
+00004c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004c70: 2020 2020 2020 2020 207b 2520 656c 7365           {% else
+00004c80: 2025 7d0a 2020 2020 2020 2020 2020 2020   %}.            
+00004c90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004ca0: 2020 2020 2020 2020 3c64 6976 2063 6c61          <div cla
+00004cb0: 7373 3d22 636f 6c2d 3132 223e 7b7b 2031  ss="col-12">{{ 1
+00004cc0: 5f63 656e 7465 725f 6d69 645f 746f 705f  _center_mid_top_
+00004cd0: 6120 7d7d 7b7b 2031 5f63 656e 7465 725f  a }}{{ 1_center_
+00004ce0: 6d69 645f 746f 705f 6220 7d7d 7b7b 2031  mid_top_b }}{{ 1
+00004cf0: 5f63 656e 7465 725f 6d69 645f 746f 705f  _center_mid_top_
+00004d00: 6320 7d7d 3c2f 6469 763e 0a20 2020 2020  c }}</div>.     
+00004d10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004d20: 2020 2020 2020 2020 2020 207b 2520 656e             {% en
+00004d30: 6469 6620 257d 0a20 2020 2020 2020 2020  dif %}.         
+00004d40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004d50: 2020 203c 2f64 6976 3e0a 2020 2020 2020     </div>.      
+00004d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004d70: 2020 2020 2020 7b25 2065 6e64 6966 2025        {% endif %
+00004d80: 7d0a 2020 2020 2020 2020 2020 2020 2020  }.              
+00004d90: 2020 2020 2020 2020 2020 2020 2020 3c21                <!
+00004da0: 2d2d 2045 4e44 2043 656e 7465 7220 6d69  -- END Center mi
+00004db0: 642d 746f 7020 2d2d 3e0a 0a20 2020 2020  d-top -->..     
+00004dc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004dd0: 2020 2020 2020 203c 212d 2d20 4365 6e74         <!-- Cent
+00004de0: 6572 2063 6f6e 7465 6e74 202d 2d3e 0a20  er content -->. 
+00004df0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004e00: 2020 2020 2020 2020 2020 207b 2520 6966             {% if
+00004e10: 2031 5f63 656e 7465 725f 636f 6e74 656e   1_center_conten
+00004e20: 7420 257d 0a20 2020 2020 2020 2020 2020  t %}.           
+00004e30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004e40: 203c 6469 7620 636c 6173 733d 2272 6f77   <div class="row
+00004e50: 223e 0a20 2020 2020 2020 2020 2020 2020  ">.             
+00004e60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004e70: 2020 203c 6469 7620 636c 6173 733d 2263     <div class="c
+00004e80: 6f6c 223e 0a20 2020 2020 2020 2020 2020  ol">.           
+00004e90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004ea0: 2020 2020 2020 2020 207b 7b20 315f 6365           {{ 1_ce
+00004eb0: 6e74 6572 5f63 6f6e 7465 6e74 207d 7d0a  nter_content }}.
+00004ec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00004ed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004ee0: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-00004ef0: 6469 7620 636c 6173 733d 227b 2520 626c  div class="{% bl
-00004f00: 6f63 6b20 315f 6365 6e74 6572 5f6d 6964  ock 1_center_mid
-00004f10: 5f62 6f74 746f 6d5f 6162 5f61 2025 7d63  _bottom_ab_a %}c
-00004f20: 6f6c 2d31 3220 636f 6c2d 6d64 2d38 7b25  ol-12 col-md-8{%
-00004f30: 2065 6e64 626c 6f63 6b20 257d 223e 7b7b   endblock %}">{{
-00004f40: 2031 5f63 656e 7465 725f 6d69 645f 626f   1_center_mid_bo
-00004f50: 7474 6f6d 5f61 207d 7d3c 2f64 6976 3e0a  ttom_a }}</div>.
-00004f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004ee0: 3c2f 6469 763e 0a20 2020 2020 2020 2020  </div>.         
+00004ef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004f00: 2020 203c 2f64 6976 3e0a 2020 2020 2020     </div>.      
+00004f10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004f20: 2020 2020 2020 7b25 2065 6e64 6966 2025        {% endif %
+00004f30: 7d0a 2020 2020 2020 2020 2020 2020 2020  }.              
+00004f40: 2020 2020 2020 2020 2020 2020 2020 3c21                <!
+00004f50: 2d2d 2045 4e44 2043 656e 7465 7220 636f  -- END Center co
+00004f60: 6e74 656e 7420 2d2d 3e0a 0a20 2020 2020  ntent -->..     
 00004f70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004f80: 2020 2020 3c64 6976 2063 6c61 7373 3d22      <div class="
-00004f90: 7b25 2062 6c6f 636b 2031 5f63 656e 7465  {% block 1_cente
-00004fa0: 725f 6d69 645f 626f 7474 6f6d 5f61 625f  r_mid_bottom_ab_
-00004fb0: 6220 257d 636f 6c2d 3132 2063 6f6c 2d6d  b %}col-12 col-m
-00004fc0: 642d 347b 2520 656e 6462 6c6f 636b 2025  d-4{% endblock %
-00004fd0: 7d22 3e7b 7b20 315f 6365 6e74 6572 5f6d  }">{{ 1_center_m
-00004fe0: 6964 5f62 6f74 746f 6d5f 6220 7d7d 3c2f  id_bottom_b }}</
-00004ff0: 6469 763e 0a20 2020 2020 2020 2020 2020  div>.           
-00005000: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005010: 2020 2020 207b 2520 656c 6966 2031 5f63       {% elif 1_c
-00005020: 656e 7465 725f 6d69 645f 626f 7474 6f6d  enter_mid_bottom
-00005030: 5f61 2061 6e64 2031 5f63 656e 7465 725f  _a and 1_center_
-00005040: 6d69 645f 626f 7474 6f6d 5f63 2025 7d0a  mid_bottom_c %}.
-00005050: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005060: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005070: 2020 2020 3c64 6976 2063 6c61 7373 3d22      <div class="
-00005080: 7b25 2062 6c6f 636b 2031 5f63 656e 7465  {% block 1_cente
-00005090: 725f 6d69 645f 626f 7474 6f6d 5f61 635f  r_mid_bottom_ac_
-000050a0: 6120 257d 636f 6c2d 3132 2063 6f6c 2d6d  a %}col-12 col-m
-000050b0: 642d 367b 2520 656e 6462 6c6f 636b 2025  d-6{% endblock %
-000050c0: 7d22 3e7b 7b20 315f 6365 6e74 6572 5f6d  }">{{ 1_center_m
-000050d0: 6964 5f62 6f74 746f 6d5f 6120 7d7d 3c2f  id_bottom_a }}</
-000050e0: 6469 763e 0a20 2020 2020 2020 2020 2020  div>.           
-000050f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005100: 2020 2020 2020 2020 203c 6469 7620 636c           <div cl
-00005110: 6173 733d 227b 2520 626c 6f63 6b20 315f  ass="{% block 1_
-00005120: 6365 6e74 6572 5f6d 6964 5f62 6f74 746f  center_mid_botto
-00005130: 6d5f 6163 5f63 2025 7d63 6f6c 2d31 3220  m_ac_c %}col-12 
-00005140: 636f 6c2d 6d64 2d36 7b25 2065 6e64 626c  col-md-6{% endbl
-00005150: 6f63 6b20 257d 223e 7b7b 2031 5f63 656e  ock %}">{{ 1_cen
-00005160: 7465 725f 6d69 645f 626f 7474 6f6d 5f63  ter_mid_bottom_c
-00005170: 207d 7d3c 2f64 6976 3e0a 2020 2020 2020   }}</div>.      
-00005180: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005190: 2020 2020 2020 2020 2020 7b25 2065 6c69            {% eli
-000051a0: 6620 315f 6365 6e74 6572 5f6d 6964 5f62  f 1_center_mid_b
-000051b0: 6f74 746f 6d5f 6220 616e 6420 315f 6365  ottom_b and 1_ce
-000051c0: 6e74 6572 5f6d 6964 5f62 6f74 746f 6d5f  nter_mid_bottom_
-000051d0: 6320 257d 0a20 2020 2020 2020 2020 2020  c %}.           
+00004f80: 2020 2020 2020 203c 212d 2d20 4365 6e74         <!-- Cent
+00004f90: 6572 206d 6964 2d62 6f74 746f 6d20 2d2d  er mid-bottom --
+00004fa0: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
+00004fb0: 2020 2020 2020 2020 2020 2020 2020 7b25                {%
+00004fc0: 2069 6620 315f 6365 6e74 6572 5f6d 6964   if 1_center_mid
+00004fd0: 5f62 6f74 746f 6d5f 6120 6f72 2031 5f63  _bottom_a or 1_c
+00004fe0: 656e 7465 725f 6d69 645f 626f 7474 6f6d  enter_mid_bottom
+00004ff0: 5f62 206f 7220 315f 6365 6e74 6572 5f6d  _b or 1_center_m
+00005000: 6964 5f62 6f74 746f 6d5f 6320 257d 0a20  id_bottom_c %}. 
+00005010: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005020: 2020 2020 2020 2020 2020 203c 6469 7620             <div 
+00005030: 636c 6173 733d 2272 6f77 223e 0a20 2020  class="row">.   
+00005040: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005050: 2020 2020 2020 2020 2020 2020 207b 2520               {% 
+00005060: 6966 2031 5f63 656e 7465 725f 6d69 645f  if 1_center_mid_
+00005070: 626f 7474 6f6d 5f61 2061 6e64 2031 5f63  bottom_a and 1_c
+00005080: 656e 7465 725f 6d69 645f 626f 7474 6f6d  enter_mid_bottom
+00005090: 5f62 2061 6e64 2031 5f63 656e 7465 725f  _b and 1_center_
+000050a0: 6d69 645f 626f 7474 6f6d 5f63 2025 7d0a  mid_bottom_c %}.
+000050b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000050c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000050d0: 2020 2020 3c64 6976 2063 6c61 7373 3d22      <div class="
+000050e0: 7b25 2062 6c6f 636b 2031 5f63 656e 7465  {% block 1_cente
+000050f0: 725f 6d69 645f 626f 7474 6f6d 5f61 6263  r_mid_bottom_abc
+00005100: 5f61 2025 7d63 6f6c 2d31 3220 636f 6c2d  _a %}col-12 col-
+00005110: 6d64 2d34 7b25 2065 6e64 626c 6f63 6b20  md-4{% endblock 
+00005120: 257d 223e 7b7b 2031 5f63 656e 7465 725f  %}">{{ 1_center_
+00005130: 6d69 645f 626f 7474 6f6d 5f61 207d 7d3c  mid_bottom_a }}<
+00005140: 2f64 6976 3e0a 2020 2020 2020 2020 2020  /div>.          
+00005150: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005160: 2020 2020 2020 2020 2020 3c64 6976 2063            <div c
+00005170: 6c61 7373 3d22 7b25 2062 6c6f 636b 2031  lass="{% block 1
+00005180: 5f63 656e 7465 725f 6d69 645f 626f 7474  _center_mid_bott
+00005190: 6f6d 5f61 6263 5f62 2025 7d63 6f6c 2d31  om_abc_b %}col-1
+000051a0: 3220 636f 6c2d 6d64 2d34 7b25 2065 6e64  2 col-md-4{% end
+000051b0: 626c 6f63 6b20 257d 223e 7b7b 2031 5f63  block %}">{{ 1_c
+000051c0: 656e 7465 725f 6d69 645f 626f 7474 6f6d  enter_mid_bottom
+000051d0: 5f62 207d 7d3c 2f64 6976 3e0a 2020 2020  _b }}</div>.    
 000051e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000051f0: 2020 2020 2020 2020 203c 6469 7620 636c           <div cl
-00005200: 6173 733d 227b 2520 626c 6f63 6b20 315f  ass="{% block 1_
-00005210: 6365 6e74 6572 5f6d 6964 5f62 6f74 746f  center_mid_botto
-00005220: 6d5f 6263 5f62 2025 7d63 6f6c 2d31 3220  m_bc_b %}col-12 
-00005230: 636f 6c2d 6d64 2d34 7b25 2065 6e64 626c  col-md-4{% endbl
-00005240: 6f63 6b20 257d 223e 7b7b 2031 5f63 656e  ock %}">{{ 1_cen
-00005250: 7465 725f 6d69 645f 626f 7474 6f6d 5f62  ter_mid_bottom_b
-00005260: 207d 7d3c 2f64 6976 3e0a 2020 2020 2020   }}</div>.      
-00005270: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005280: 2020 2020 2020 2020 2020 2020 2020 3c64                <d
-00005290: 6976 2063 6c61 7373 3d22 7b25 2062 6c6f  iv class="{% blo
-000052a0: 636b 2031 5f63 656e 7465 725f 6d69 645f  ck 1_center_mid_
-000052b0: 626f 7474 6f6d 5f62 635f 6320 257d 636f  bottom_bc_c %}co
-000052c0: 6c2d 3132 2063 6f6c 2d6d 642d 387b 2520  l-12 col-md-8{% 
-000052d0: 656e 6462 6c6f 636b 2025 7d22 3e7b 7b20  endblock %}">{{ 
-000052e0: 315f 6365 6e74 6572 5f6d 6964 5f62 6f74  1_center_mid_bot
-000052f0: 746f 6d5f 6320 7d7d 3c2f 6469 763e 0a20  tom_c }}</div>. 
-00005300: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005310: 2020 2020 2020 2020 2020 2020 2020 207b                 {
-00005320: 2520 656c 7365 2025 7d0a 2020 2020 2020  % else %}.      
-00005330: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005340: 2020 2020 2020 2020 2020 2020 2020 3c64                <d
-00005350: 6976 2063 6c61 7373 3d22 636f 6c2d 3132  iv class="col-12
-00005360: 223e 7b7b 2031 5f63 656e 7465 725f 6d69  ">{{ 1_center_mi
-00005370: 645f 626f 7474 6f6d 5f61 207d 7d7b 7b20  d_bottom_a }}{{ 
-00005380: 315f 6365 6e74 6572 5f6d 6964 5f62 6f74  1_center_mid_bot
-00005390: 746f 6d5f 6220 7d7d 7b7b 2031 5f63 656e  tom_b }}{{ 1_cen
-000053a0: 7465 725f 6d69 645f 626f 7474 6f6d 5f63  ter_mid_bottom_c
-000053b0: 207d 7d3c 2f64 6976 3e0a 2020 2020 2020   }}</div>.      
-000053c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000053d0: 2020 2020 2020 2020 2020 7b25 2065 6e64            {% end
-000053e0: 6966 2025 7d0a 2020 2020 2020 2020 2020  if %}.          
-000053f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005400: 2020 3c2f 6469 763e 0a20 2020 2020 2020    </div>.       
-00005410: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005420: 2020 2020 207b 2520 656e 6469 6620 257d       {% endif %}
-00005430: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00005440: 2020 2020 2020 2020 2020 2020 203c 212d               <!-
-00005450: 2d20 454e 4420 4365 6e74 6572 206d 6964  - END Center mid
-00005460: 2d62 6f74 746f 6d20 2d2d 3e0a 0a20 2020  -bottom -->..   
-00005470: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005480: 2020 2020 2020 2020 203c 212d 2d20 4365           <!-- Ce
-00005490: 6e74 6572 2062 6f74 746f 6d20 2d2d 3e0a  nter bottom -->.
-000054a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000054b0: 2020 2020 2020 2020 2020 2020 7b25 2069              {% i
-000054c0: 6620 315f 6365 6e74 6572 5f62 6f74 746f  f 1_center_botto
-000054d0: 6d5f 6120 6f72 2031 5f63 656e 7465 725f  m_a or 1_center_
-000054e0: 626f 7474 6f6d 5f62 206f 7220 315f 6365  bottom_b or 1_ce
-000054f0: 6e74 6572 5f62 6f74 746f 6d5f 6320 257d  nter_bottom_c %}
-00005500: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00005510: 2020 2020 2020 2020 2020 2020 203c 6469               <di
-00005520: 7620 636c 6173 733d 2272 6f77 223e 0a20  v class="row">. 
-00005530: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005540: 2020 2020 2020 2020 2020 2020 2020 207b                 {
-00005550: 2520 6966 2031 5f63 656e 7465 725f 626f  % if 1_center_bo
-00005560: 7474 6f6d 5f61 2061 6e64 2031 5f63 656e  ttom_a and 1_cen
-00005570: 7465 725f 626f 7474 6f6d 5f62 2061 6e64  ter_bottom_b and
-00005580: 2031 5f63 656e 7465 725f 626f 7474 6f6d   1_center_bottom
-00005590: 5f63 2025 7d0a 2020 2020 2020 2020 2020  _c %}.          
-000055a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000055b0: 2020 2020 2020 2020 2020 3c64 6976 2063            <div c
-000055c0: 6c61 7373 3d22 7b25 2062 6c6f 636b 2031  lass="{% block 1
-000055d0: 5f63 656e 7465 725f 626f 7474 6f6d 5f61  _center_bottom_a
-000055e0: 6263 5f61 2025 7d63 6f6c 2d31 3220 636f  bc_a %}col-12 co
-000055f0: 6c2d 6d64 2d34 7b25 2065 6e64 626c 6f63  l-md-4{% endbloc
-00005600: 6b20 257d 223e 7b7b 2031 5f63 656e 7465  k %}">{{ 1_cente
-00005610: 725f 626f 7474 6f6d 5f61 207d 7d3c 2f64  r_bottom_a }}</d
-00005620: 6976 3e0a 2020 2020 2020 2020 2020 2020  iv>.            
-00005630: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005640: 2020 2020 2020 2020 3c64 6976 2063 6c61          <div cla
-00005650: 7373 3d22 7b25 2062 6c6f 636b 2031 5f63  ss="{% block 1_c
-00005660: 656e 7465 725f 626f 7474 6f6d 5f61 6263  enter_bottom_abc
-00005670: 5f62 2025 7d63 6f6c 2d31 3220 636f 6c2d  _b %}col-12 col-
-00005680: 6d64 2d34 7b25 2065 6e64 626c 6f63 6b20  md-4{% endblock 
-00005690: 257d 223e 7b7b 2031 5f63 656e 7465 725f  %}">{{ 1_center_
-000056a0: 626f 7474 6f6d 5f62 207d 7d3c 2f64 6976  bottom_b }}</div
-000056b0: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
-000056c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000056d0: 2020 2020 2020 3c64 6976 2063 6c61 7373        <div class
-000056e0: 3d22 7b25 2062 6c6f 636b 2031 5f63 656e  ="{% block 1_cen
-000056f0: 7465 725f 626f 7474 6f6d 5f61 6263 5f63  ter_bottom_abc_c
-00005700: 2025 7d63 6f6c 2d31 3220 636f 6c2d 6d64   %}col-12 col-md
-00005710: 2d34 7b25 2065 6e64 626c 6f63 6b20 257d  -4{% endblock %}
-00005720: 223e 7b7b 2031 5f63 656e 7465 725f 626f  ">{{ 1_center_bo
-00005730: 7474 6f6d 5f63 207d 7d3c 2f64 6976 3e0a  ttom_c }}</div>.
+000051f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005200: 3c64 6976 2063 6c61 7373 3d22 7b25 2062  <div class="{% b
+00005210: 6c6f 636b 2031 5f63 656e 7465 725f 6d69  lock 1_center_mi
+00005220: 645f 626f 7474 6f6d 5f61 6263 5f63 2025  d_bottom_abc_c %
+00005230: 7d63 6f6c 2d31 3220 636f 6c2d 6d64 2d34  }col-12 col-md-4
+00005240: 7b25 2065 6e64 626c 6f63 6b20 257d 223e  {% endblock %}">
+00005250: 7b7b 2031 5f63 656e 7465 725f 6d69 645f  {{ 1_center_mid_
+00005260: 626f 7474 6f6d 5f63 207d 7d3c 2f64 6976  bottom_c }}</div
+00005270: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
+00005280: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005290: 2020 7b25 2065 6c69 6620 315f 6365 6e74    {% elif 1_cent
+000052a0: 6572 5f6d 6964 5f62 6f74 746f 6d5f 6120  er_mid_bottom_a 
+000052b0: 616e 6420 315f 6365 6e74 6572 5f6d 6964  and 1_center_mid
+000052c0: 5f62 6f74 746f 6d5f 6220 257d 0a20 2020  _bottom_b %}.   
+000052d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000052e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000052f0: 203c 6469 7620 636c 6173 733d 227b 2520   <div class="{% 
+00005300: 626c 6f63 6b20 315f 6365 6e74 6572 5f6d  block 1_center_m
+00005310: 6964 5f62 6f74 746f 6d5f 6162 5f61 2025  id_bottom_ab_a %
+00005320: 7d63 6f6c 2d31 3220 636f 6c2d 6d64 2d38  }col-12 col-md-8
+00005330: 7b25 2065 6e64 626c 6f63 6b20 257d 223e  {% endblock %}">
+00005340: 7b7b 2031 5f63 656e 7465 725f 6d69 645f  {{ 1_center_mid_
+00005350: 626f 7474 6f6d 5f61 207d 7d3c 2f64 6976  bottom_a }}</div
+00005360: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
+00005370: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005380: 2020 2020 2020 3c64 6976 2063 6c61 7373        <div class
+00005390: 3d22 7b25 2062 6c6f 636b 2031 5f63 656e  ="{% block 1_cen
+000053a0: 7465 725f 6d69 645f 626f 7474 6f6d 5f61  ter_mid_bottom_a
+000053b0: 625f 6220 257d 636f 6c2d 3132 2063 6f6c  b_b %}col-12 col
+000053c0: 2d6d 642d 347b 2520 656e 6462 6c6f 636b  -md-4{% endblock
+000053d0: 2025 7d22 3e7b 7b20 315f 6365 6e74 6572   %}">{{ 1_center
+000053e0: 5f6d 6964 5f62 6f74 746f 6d5f 6220 7d7d  _mid_bottom_b }}
+000053f0: 3c2f 6469 763e 0a20 2020 2020 2020 2020  </div>.         
+00005400: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005410: 2020 2020 2020 207b 2520 656c 6966 2031         {% elif 1
+00005420: 5f63 656e 7465 725f 6d69 645f 626f 7474  _center_mid_bott
+00005430: 6f6d 5f61 2061 6e64 2031 5f63 656e 7465  om_a and 1_cente
+00005440: 725f 6d69 645f 626f 7474 6f6d 5f63 2025  r_mid_bottom_c %
+00005450: 7d0a 2020 2020 2020 2020 2020 2020 2020  }.              
+00005460: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005470: 2020 2020 2020 3c64 6976 2063 6c61 7373        <div class
+00005480: 3d22 7b25 2062 6c6f 636b 2031 5f63 656e  ="{% block 1_cen
+00005490: 7465 725f 6d69 645f 626f 7474 6f6d 5f61  ter_mid_bottom_a
+000054a0: 635f 6120 257d 636f 6c2d 3132 2063 6f6c  c_a %}col-12 col
+000054b0: 2d6d 642d 367b 2520 656e 6462 6c6f 636b  -md-6{% endblock
+000054c0: 2025 7d22 3e7b 7b20 315f 6365 6e74 6572   %}">{{ 1_center
+000054d0: 5f6d 6964 5f62 6f74 746f 6d5f 6120 7d7d  _mid_bottom_a }}
+000054e0: 3c2f 6469 763e 0a20 2020 2020 2020 2020  </div>.         
+000054f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005500: 2020 2020 2020 2020 2020 203c 6469 7620             <div 
+00005510: 636c 6173 733d 227b 2520 626c 6f63 6b20  class="{% block 
+00005520: 315f 6365 6e74 6572 5f6d 6964 5f62 6f74  1_center_mid_bot
+00005530: 746f 6d5f 6163 5f63 2025 7d63 6f6c 2d31  tom_ac_c %}col-1
+00005540: 3220 636f 6c2d 6d64 2d36 7b25 2065 6e64  2 col-md-6{% end
+00005550: 626c 6f63 6b20 257d 223e 7b7b 2031 5f63  block %}">{{ 1_c
+00005560: 656e 7465 725f 6d69 645f 626f 7474 6f6d  enter_mid_bottom
+00005570: 5f63 207d 7d3c 2f64 6976 3e0a 2020 2020  _c }}</div>.    
+00005580: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005590: 2020 2020 2020 2020 2020 2020 7b25 2065              {% e
+000055a0: 6c69 6620 315f 6365 6e74 6572 5f6d 6964  lif 1_center_mid
+000055b0: 5f62 6f74 746f 6d5f 6220 616e 6420 315f  _bottom_b and 1_
+000055c0: 6365 6e74 6572 5f6d 6964 5f62 6f74 746f  center_mid_botto
+000055d0: 6d5f 6320 257d 0a20 2020 2020 2020 2020  m_c %}.         
+000055e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000055f0: 2020 2020 2020 2020 2020 203c 6469 7620             <div 
+00005600: 636c 6173 733d 227b 2520 626c 6f63 6b20  class="{% block 
+00005610: 315f 6365 6e74 6572 5f6d 6964 5f62 6f74  1_center_mid_bot
+00005620: 746f 6d5f 6263 5f62 2025 7d63 6f6c 2d31  tom_bc_b %}col-1
+00005630: 3220 636f 6c2d 6d64 2d34 7b25 2065 6e64  2 col-md-4{% end
+00005640: 626c 6f63 6b20 257d 223e 7b7b 2031 5f63  block %}">{{ 1_c
+00005650: 656e 7465 725f 6d69 645f 626f 7474 6f6d  enter_mid_bottom
+00005660: 5f62 207d 7d3c 2f64 6976 3e0a 2020 2020  _b }}</div>.    
+00005670: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005680: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005690: 3c64 6976 2063 6c61 7373 3d22 7b25 2062  <div class="{% b
+000056a0: 6c6f 636b 2031 5f63 656e 7465 725f 6d69  lock 1_center_mi
+000056b0: 645f 626f 7474 6f6d 5f62 635f 6320 257d  d_bottom_bc_c %}
+000056c0: 636f 6c2d 3132 2063 6f6c 2d6d 642d 387b  col-12 col-md-8{
+000056d0: 2520 656e 6462 6c6f 636b 2025 7d22 3e7b  % endblock %}">{
+000056e0: 7b20 315f 6365 6e74 6572 5f6d 6964 5f62  { 1_center_mid_b
+000056f0: 6f74 746f 6d5f 6320 7d7d 3c2f 6469 763e  ottom_c }}</div>
+00005700: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00005710: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005720: 207b 2520 656c 7365 2025 7d0a 2020 2020   {% else %}.    
+00005730: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00005740: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005750: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005760: 7b25 2065 6c69 6620 315f 6365 6e74 6572  {% elif 1_center
-00005770: 5f62 6f74 746f 6d5f 6120 616e 6420 315f  _bottom_a and 1_
-00005780: 6365 6e74 6572 5f62 6f74 746f 6d5f 6220  center_bottom_b 
-00005790: 257d 0a20 2020 2020 2020 2020 2020 2020  %}.             
-000057a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000057b0: 2020 2020 2020 203c 6469 7620 636c 6173         <div clas
-000057c0: 733d 227b 2520 626c 6f63 6b20 315f 6365  s="{% block 1_ce
-000057d0: 6e74 6572 5f62 6f74 746f 6d5f 6162 5f61  nter_bottom_ab_a
-000057e0: 2025 7d63 6f6c 2d31 3220 636f 6c2d 6d64   %}col-12 col-md
-000057f0: 2d38 7b25 2065 6e64 626c 6f63 6b20 257d  -8{% endblock %}
-00005800: 223e 7b7b 2031 5f63 656e 7465 725f 626f  ">{{ 1_center_bo
-00005810: 7474 6f6d 5f61 207d 7d3c 2f64 6976 3e0a  ttom_a }}</div>.
-00005820: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005830: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005840: 2020 2020 3c64 6976 2063 6c61 7373 3d22      <div class="
-00005850: 7b25 2062 6c6f 636b 2031 5f63 656e 7465  {% block 1_cente
-00005860: 725f 626f 7474 6f6d 5f61 625f 6220 257d  r_bottom_ab_b %}
-00005870: 636f 6c2d 3132 2063 6f6c 2d6d 642d 347b  col-12 col-md-4{
-00005880: 2520 656e 6462 6c6f 636b 2025 7d22 3e7b  % endblock %}">{
-00005890: 7b20 315f 6365 6e74 6572 5f62 6f74 746f  { 1_center_botto
-000058a0: 6d5f 6220 7d7d 3c2f 6469 763e 0a20 2020  m_b }}</div>.   
-000058b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000058c0: 2020 2020 2020 2020 2020 2020 207b 2520               {% 
-000058d0: 656c 6966 2031 5f63 656e 7465 725f 626f  elif 1_center_bo
-000058e0: 7474 6f6d 5f61 2061 6e64 2031 5f63 656e  ttom_a and 1_cen
-000058f0: 7465 725f 626f 7474 6f6d 5f63 2025 7d0a  ter_bottom_c %}.
-00005900: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005910: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005920: 2020 2020 3c64 6976 2063 6c61 7373 3d22      <div class="
-00005930: 7b25 2062 6c6f 636b 2031 5f63 656e 7465  {% block 1_cente
-00005940: 725f 626f 7474 6f6d 5f61 635f 6120 257d  r_bottom_ac_a %}
-00005950: 636f 6c2d 3132 2063 6f6c 2d6d 642d 367b  col-12 col-md-6{
-00005960: 2520 656e 6462 6c6f 636b 2025 7d22 3e7b  % endblock %}">{
-00005970: 7b20 315f 6365 6e74 6572 5f62 6f74 746f  { 1_center_botto
-00005980: 6d5f 6120 7d7d 3c2f 6469 763e 0a20 2020  m_a }}</div>.   
-00005990: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005750: 3c64 6976 2063 6c61 7373 3d22 636f 6c2d  <div class="col-
+00005760: 3132 223e 7b7b 2031 5f63 656e 7465 725f  12">{{ 1_center_
+00005770: 6d69 645f 626f 7474 6f6d 5f61 207d 7d7b  mid_bottom_a }}{
+00005780: 7b20 315f 6365 6e74 6572 5f6d 6964 5f62  { 1_center_mid_b
+00005790: 6f74 746f 6d5f 6220 7d7d 7b7b 2031 5f63  ottom_b }}{{ 1_c
+000057a0: 656e 7465 725f 6d69 645f 626f 7474 6f6d  enter_mid_bottom
+000057b0: 5f63 207d 7d3c 2f64 6976 3e0a 2020 2020  _c }}</div>.    
+000057c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000057d0: 2020 2020 2020 2020 2020 2020 7b25 2065              {% e
+000057e0: 6e64 6966 2025 7d0a 2020 2020 2020 2020  ndif %}.        
+000057f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005800: 2020 2020 3c2f 6469 763e 0a20 2020 2020      </div>.     
+00005810: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005820: 2020 2020 2020 207b 2520 656e 6469 6620         {% endif 
+00005830: 257d 0a20 2020 2020 2020 2020 2020 2020  %}.             
+00005840: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+00005850: 212d 2d20 454e 4420 4365 6e74 6572 206d  !-- END Center m
+00005860: 6964 2d62 6f74 746f 6d20 2d2d 3e0a 0a20  id-bottom -->.. 
+00005870: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005880: 2020 2020 2020 2020 2020 203c 212d 2d20             <!-- 
+00005890: 4365 6e74 6572 2062 6f74 746f 6d20 2d2d  Center bottom --
+000058a0: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
+000058b0: 2020 2020 2020 2020 2020 2020 2020 7b25                {%
+000058c0: 2069 6620 315f 6365 6e74 6572 5f62 6f74   if 1_center_bot
+000058d0: 746f 6d5f 6120 6f72 2031 5f63 656e 7465  tom_a or 1_cente
+000058e0: 725f 626f 7474 6f6d 5f62 206f 7220 315f  r_bottom_b or 1_
+000058f0: 6365 6e74 6572 5f62 6f74 746f 6d5f 6320  center_bottom_c 
+00005900: 257d 0a20 2020 2020 2020 2020 2020 2020  %}.             
+00005910: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+00005920: 6469 7620 636c 6173 733d 2272 6f77 223e  div class="row">
+00005930: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00005940: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005950: 207b 2520 6966 2031 5f63 656e 7465 725f   {% if 1_center_
+00005960: 626f 7474 6f6d 5f61 2061 6e64 2031 5f63  bottom_a and 1_c
+00005970: 656e 7465 725f 626f 7474 6f6d 5f62 2061  enter_bottom_b a
+00005980: 6e64 2031 5f63 656e 7465 725f 626f 7474  nd 1_center_bott
+00005990: 6f6d 5f63 2025 7d0a 2020 2020 2020 2020  om_c %}.        
 000059a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000059b0: 203c 6469 7620 636c 6173 733d 227b 2520   <div class="{% 
-000059c0: 626c 6f63 6b20 315f 6365 6e74 6572 5f62  block 1_center_b
-000059d0: 6f74 746f 6d5f 6163 5f63 2025 7d63 6f6c  ottom_ac_c %}col
-000059e0: 2d31 3220 636f 6c2d 6d64 2d36 7b25 2065  -12 col-md-6{% e
-000059f0: 6e64 626c 6f63 6b20 257d 223e 7b7b 2031  ndblock %}">{{ 1
-00005a00: 5f63 656e 7465 725f 626f 7474 6f6d 5f63  _center_bottom_c
-00005a10: 207d 7d3c 2f64 6976 3e0a 2020 2020 2020   }}</div>.      
-00005a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005a30: 2020 2020 2020 2020 2020 7b25 2065 6c69            {% eli
-00005a40: 6620 315f 6365 6e74 6572 5f62 6f74 746f  f 1_center_botto
-00005a50: 6d5f 6220 616e 6420 315f 6365 6e74 6572  m_b and 1_center
-00005a60: 5f62 6f74 746f 6d5f 6320 257d 0a20 2020  _bottom_c %}.   
-00005a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005a90: 203c 6469 7620 636c 6173 733d 227b 2520   <div class="{% 
-00005aa0: 626c 6f63 6b20 315f 6365 6e74 6572 5f62  block 1_center_b
-00005ab0: 6f74 746f 6d5f 6263 5f62 2025 7d63 6f6c  ottom_bc_b %}col
-00005ac0: 2d31 3220 636f 6c2d 6d64 2d34 7b25 2065  -12 col-md-4{% e
-00005ad0: 6e64 626c 6f63 6b20 257d 223e 7b7b 2031  ndblock %}">{{ 1
-00005ae0: 5f63 656e 7465 725f 626f 7474 6f6d 5f62  _center_bottom_b
-00005af0: 207d 7d3c 2f64 6976 3e0a 2020 2020 2020   }}</div>.      
-00005b00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005b10: 2020 2020 2020 2020 2020 2020 2020 3c64                <d
-00005b20: 6976 2063 6c61 7373 3d22 7b25 2062 6c6f  iv class="{% blo
-00005b30: 636b 2031 5f63 656e 7465 725f 626f 7474  ck 1_center_bott
-00005b40: 6f6d 5f62 635f 6320 257d 636f 6c2d 3132  om_bc_c %}col-12
-00005b50: 2063 6f6c 2d6d 642d 387b 2520 656e 6462   col-md-8{% endb
-00005b60: 6c6f 636b 2025 7d22 3e7b 7b20 315f 6365  lock %}">{{ 1_ce
-00005b70: 6e74 6572 5f62 6f74 746f 6d5f 6320 7d7d  nter_bottom_c }}
-00005b80: 3c2f 6469 763e 0a20 2020 2020 2020 2020  </div>.         
-00005b90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005ba0: 2020 2020 2020 207b 2520 656c 7365 2025         {% else %
-00005bb0: 7d0a 2020 2020 2020 2020 2020 2020 2020  }.              
-00005bc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005bd0: 2020 2020 2020 3c64 6976 2063 6c61 7373        <div class
-00005be0: 3d22 636f 6c2d 3132 223e 7b7b 2031 5f63  ="col-12">{{ 1_c
-00005bf0: 656e 7465 725f 626f 7474 6f6d 5f61 207d  enter_bottom_a }
-00005c00: 7d7b 7b20 315f 6365 6e74 6572 5f62 6f74  }{{ 1_center_bot
-00005c10: 746f 6d5f 6220 7d7d 7b7b 2031 5f63 656e  tom_b }}{{ 1_cen
-00005c20: 7465 725f 626f 7474 6f6d 5f63 207d 7d3c  ter_bottom_c }}<
-00005c30: 2f64 6976 3e0a 2020 2020 2020 2020 2020  /div>.          
-00005c40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005c50: 2020 2020 2020 7b25 2065 6e64 6966 2025        {% endif %
-00005c60: 7d0a 2020 2020 2020 2020 2020 2020 2020  }.              
-00005c70: 2020 2020 2020 2020 2020 2020 2020 3c2f                </
-00005c80: 6469 763e 0a20 2020 2020 2020 2020 2020  div>.           
-00005c90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005ca0: 207b 2520 656e 6469 6620 257d 0a20 2020   {% endif %}.   
+000059b0: 2020 2020 2020 2020 2020 2020 3c64 6976              <div
+000059c0: 2063 6c61 7373 3d22 7b25 2062 6c6f 636b   class="{% block
+000059d0: 2031 5f63 656e 7465 725f 626f 7474 6f6d   1_center_bottom
+000059e0: 5f61 6263 5f61 2025 7d63 6f6c 2d31 3220  _abc_a %}col-12 
+000059f0: 636f 6c2d 6d64 2d34 7b25 2065 6e64 626c  col-md-4{% endbl
+00005a00: 6f63 6b20 257d 223e 7b7b 2031 5f63 656e  ock %}">{{ 1_cen
+00005a10: 7465 725f 626f 7474 6f6d 5f61 207d 7d3c  ter_bottom_a }}<
+00005a20: 2f64 6976 3e0a 2020 2020 2020 2020 2020  /div>.          
+00005a30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005a40: 2020 2020 2020 2020 2020 3c64 6976 2063            <div c
+00005a50: 6c61 7373 3d22 7b25 2062 6c6f 636b 2031  lass="{% block 1
+00005a60: 5f63 656e 7465 725f 626f 7474 6f6d 5f61  _center_bottom_a
+00005a70: 6263 5f62 2025 7d63 6f6c 2d31 3220 636f  bc_b %}col-12 co
+00005a80: 6c2d 6d64 2d34 7b25 2065 6e64 626c 6f63  l-md-4{% endbloc
+00005a90: 6b20 257d 223e 7b7b 2031 5f63 656e 7465  k %}">{{ 1_cente
+00005aa0: 725f 626f 7474 6f6d 5f62 207d 7d3c 2f64  r_bottom_b }}</d
+00005ab0: 6976 3e0a 2020 2020 2020 2020 2020 2020  iv>.            
+00005ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005ad0: 2020 2020 2020 2020 3c64 6976 2063 6c61          <div cla
+00005ae0: 7373 3d22 7b25 2062 6c6f 636b 2031 5f63  ss="{% block 1_c
+00005af0: 656e 7465 725f 626f 7474 6f6d 5f61 6263  enter_bottom_abc
+00005b00: 5f63 2025 7d63 6f6c 2d31 3220 636f 6c2d  _c %}col-12 col-
+00005b10: 6d64 2d34 7b25 2065 6e64 626c 6f63 6b20  md-4{% endblock 
+00005b20: 257d 223e 7b7b 2031 5f63 656e 7465 725f  %}">{{ 1_center_
+00005b30: 626f 7474 6f6d 5f63 207d 7d3c 2f64 6976  bottom_c }}</div
+00005b40: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
+00005b50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005b60: 2020 7b25 2065 6c69 6620 315f 6365 6e74    {% elif 1_cent
+00005b70: 6572 5f62 6f74 746f 6d5f 6120 616e 6420  er_bottom_a and 
+00005b80: 315f 6365 6e74 6572 5f62 6f74 746f 6d5f  1_center_bottom_
+00005b90: 6220 257d 0a20 2020 2020 2020 2020 2020  b %}.           
+00005ba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005bb0: 2020 2020 2020 2020 203c 6469 7620 636c           <div cl
+00005bc0: 6173 733d 227b 2520 626c 6f63 6b20 315f  ass="{% block 1_
+00005bd0: 6365 6e74 6572 5f62 6f74 746f 6d5f 6162  center_bottom_ab
+00005be0: 5f61 2025 7d63 6f6c 2d31 3220 636f 6c2d  _a %}col-12 col-
+00005bf0: 6d64 2d38 7b25 2065 6e64 626c 6f63 6b20  md-8{% endblock 
+00005c00: 257d 223e 7b7b 2031 5f63 656e 7465 725f  %}">{{ 1_center_
+00005c10: 626f 7474 6f6d 5f61 207d 7d3c 2f64 6976  bottom_a }}</div
+00005c20: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
+00005c30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005c40: 2020 2020 2020 3c64 6976 2063 6c61 7373        <div class
+00005c50: 3d22 7b25 2062 6c6f 636b 2031 5f63 656e  ="{% block 1_cen
+00005c60: 7465 725f 626f 7474 6f6d 5f61 625f 6220  ter_bottom_ab_b 
+00005c70: 257d 636f 6c2d 3132 2063 6f6c 2d6d 642d  %}col-12 col-md-
+00005c80: 347b 2520 656e 6462 6c6f 636b 2025 7d22  4{% endblock %}"
+00005c90: 3e7b 7b20 315f 6365 6e74 6572 5f62 6f74  >{{ 1_center_bot
+00005ca0: 746f 6d5f 6220 7d7d 3c2f 6469 763e 0a20  tom_b }}</div>. 
 00005cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005cc0: 2020 2020 2020 2020 203c 212d 2d20 454e           <!-- EN
-00005cd0: 4420 4365 6e74 6572 2062 6f74 746f 6d20  D Center bottom 
-00005ce0: 2d2d 3e0a 0a20 2020 2020 2020 2020 2020  -->..           
-00005cf0: 2020 2020 2020 2020 2020 2020 203c 2f64               </d
-00005d00: 6976 3e0a 2020 2020 2020 2020 2020 2020  iv>.            
-00005d10: 2020 2020 2020 2020 2020 2020 3c21 2d2d              <!--
-00005d20: 2045 6e64 2043 656e 7465 7220 636f 6c75   End Center colu
-00005d30: 6d6e 202d 2d3e 0a0a 2020 2020 2020 2020  mn -->..        
-00005d40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005d50: 3c21 2d2d 2042 7569 6c64 2072 6967 6874  <!-- Build right
-00005d60: 2063 6f6c 756d 6e20 2d2d 3e0a 2020 2020   column -->.    
-00005d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005d80: 2020 2020 7b25 2069 6620 315f 7269 6768      {% if 1_righ
-00005d90: 745f 6120 6f72 2031 5f72 6967 6874 5f62  t_a or 1_right_b
-00005da0: 2025 7d0a 2020 2020 2020 2020 2020 2020   %}.            
-00005db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005dc0: 7b25 2069 6620 315f 7269 6768 745f 6120  {% if 1_right_a 
-00005dd0: 616e 6420 315f 7269 6768 745f 6220 257d  and 1_right_b %}
-00005de0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00005df0: 2020 2020 2020 2020 2020 2020 203c 6469               <di
-00005e00: 7620 636c 6173 733d 227b 2520 626c 6f63  v class="{% bloc
-00005e10: 6b20 315f 7269 6768 745f 6162 2025 7d63  k 1_right_ab %}c
-00005e20: 6f6c 2d31 3220 636f 6c2d 6c67 2d34 206d  ol-12 col-lg-4 m
-00005e30: 742d 3520 6d74 2d6c 672d 307b 2520 656e  t-5 mt-lg-0{% en
-00005e40: 6462 6c6f 636b 2025 7d22 3e0a 2020 2020  dblock %}">.    
-00005e50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005e60: 2020 2020 2020 2020 7b25 2065 6c69 6620          {% elif 
-00005e70: 315f 7269 6768 745f 6120 257d 0a20 2020  1_right_a %}.   
+00005cc0: 2020 2020 2020 2020 2020 2020 2020 207b                 {
+00005cd0: 2520 656c 6966 2031 5f63 656e 7465 725f  % elif 1_center_
+00005ce0: 626f 7474 6f6d 5f61 2061 6e64 2031 5f63  bottom_a and 1_c
+00005cf0: 656e 7465 725f 626f 7474 6f6d 5f63 2025  enter_bottom_c %
+00005d00: 7d0a 2020 2020 2020 2020 2020 2020 2020  }.              
+00005d10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005d20: 2020 2020 2020 3c64 6976 2063 6c61 7373        <div class
+00005d30: 3d22 7b25 2062 6c6f 636b 2031 5f63 656e  ="{% block 1_cen
+00005d40: 7465 725f 626f 7474 6f6d 5f61 635f 6120  ter_bottom_ac_a 
+00005d50: 257d 636f 6c2d 3132 2063 6f6c 2d6d 642d  %}col-12 col-md-
+00005d60: 367b 2520 656e 6462 6c6f 636b 2025 7d22  6{% endblock %}"
+00005d70: 3e7b 7b20 315f 6365 6e74 6572 5f62 6f74  >{{ 1_center_bot
+00005d80: 746f 6d5f 6120 7d7d 3c2f 6469 763e 0a20  tom_a }}</div>. 
+00005d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005da0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005db0: 2020 203c 6469 7620 636c 6173 733d 227b     <div class="{
+00005dc0: 2520 626c 6f63 6b20 315f 6365 6e74 6572  % block 1_center
+00005dd0: 5f62 6f74 746f 6d5f 6163 5f63 2025 7d63  _bottom_ac_c %}c
+00005de0: 6f6c 2d31 3220 636f 6c2d 6d64 2d36 7b25  ol-12 col-md-6{%
+00005df0: 2065 6e64 626c 6f63 6b20 257d 223e 7b7b   endblock %}">{{
+00005e00: 2031 5f63 656e 7465 725f 626f 7474 6f6d   1_center_bottom
+00005e10: 5f63 207d 7d3c 2f64 6976 3e0a 2020 2020  _c }}</div>.    
+00005e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005e30: 2020 2020 2020 2020 2020 2020 7b25 2065              {% e
+00005e40: 6c69 6620 315f 6365 6e74 6572 5f62 6f74  lif 1_center_bot
+00005e50: 746f 6d5f 6220 616e 6420 315f 6365 6e74  tom_b and 1_cent
+00005e60: 6572 5f62 6f74 746f 6d5f 6320 257d 0a20  er_bottom_c %}. 
+00005e70: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00005e80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005e90: 2020 2020 2020 2020 203c 6469 7620 636c           <div cl
-00005ea0: 6173 733d 227b 2520 626c 6f63 6b20 315f  ass="{% block 1_
-00005eb0: 7269 6768 745f 6120 257d 636f 6c2d 3132  right_a %}col-12
-00005ec0: 2063 6f6c 2d6c 672d 3320 6d74 2d35 206d   col-lg-3 mt-5 m
-00005ed0: 742d 6c67 2d30 7b25 2065 6e64 626c 6f63  t-lg-0{% endbloc
-00005ee0: 6b20 257d 223e 0a20 2020 2020 2020 2020  k %}">.         
-00005ef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005f00: 2020 207b 2520 656c 7365 2025 7d0a 2020     {% else %}.  
+00005e90: 2020 203c 6469 7620 636c 6173 733d 227b     <div class="{
+00005ea0: 2520 626c 6f63 6b20 315f 6365 6e74 6572  % block 1_center
+00005eb0: 5f62 6f74 746f 6d5f 6263 5f62 2025 7d63  _bottom_bc_b %}c
+00005ec0: 6f6c 2d31 3220 636f 6c2d 6d64 2d34 7b25  ol-12 col-md-4{%
+00005ed0: 2065 6e64 626c 6f63 6b20 257d 223e 7b7b   endblock %}">{{
+00005ee0: 2031 5f63 656e 7465 725f 626f 7474 6f6d   1_center_bottom
+00005ef0: 5f62 207d 7d3c 2f64 6976 3e0a 2020 2020  _b }}</div>.    
+00005f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00005f10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005f20: 2020 2020 2020 2020 2020 3c64 6976 2063            <div c
-00005f30: 6c61 7373 3d22 7b25 2062 6c6f 636b 2031  lass="{% block 1
-00005f40: 5f72 6967 6874 5f62 2025 7d63 6f6c 2d31  _right_b %}col-1
-00005f50: 3220 636f 6c2d 6c67 2d33 206f 6666 7365  2 col-lg-3 offse
-00005f60: 742d 6c67 2d31 206d 742d 3520 6d74 2d6c  t-lg-1 mt-5 mt-l
-00005f70: 672d 307b 2520 656e 6462 6c6f 636b 2025  g-0{% endblock %
-00005f80: 7d22 3e0a 2020 2020 2020 2020 2020 2020  }">.            
+00005f20: 3c64 6976 2063 6c61 7373 3d22 7b25 2062  <div class="{% b
+00005f30: 6c6f 636b 2031 5f63 656e 7465 725f 626f  lock 1_center_bo
+00005f40: 7474 6f6d 5f62 635f 6320 257d 636f 6c2d  ttom_bc_c %}col-
+00005f50: 3132 2063 6f6c 2d6d 642d 387b 2520 656e  12 col-md-8{% en
+00005f60: 6462 6c6f 636b 2025 7d22 3e7b 7b20 315f  dblock %}">{{ 1_
+00005f70: 6365 6e74 6572 5f62 6f74 746f 6d5f 6320  center_bottom_c 
+00005f80: 7d7d 3c2f 6469 763e 0a20 2020 2020 2020  }}</div>.       
 00005f90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005fa0: 7b25 2065 6e64 6966 2025 7d0a 2020 2020  {% endif %}.    
-00005fb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005fc0: 2020 2020 2020 2020 2020 2020 3c64 6976              <div
-00005fd0: 2063 6c61 7373 3d22 726f 7722 3e0a 2020   class="row">.  
-00005fe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005ff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006000: 2020 7b25 2069 6620 315f 7269 6768 745f    {% if 1_right_
-00006010: 6120 616e 6420 315f 7269 6768 745f 6220  a and 1_right_b 
-00006020: 257d 0a20 2020 2020 2020 2020 2020 2020  %}.             
-00006030: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006040: 2020 2020 2020 203c 6469 7620 636c 6173         <div clas
-00006050: 733d 227b 2520 626c 6f63 6b20 315f 7269  s="{% block 1_ri
-00006060: 6768 745f 6162 5f61 2025 7d63 6f6c 2d31  ght_ab_a %}col-1
-00006070: 3220 636f 6c2d 6c67 2d36 7b25 2065 6e64  2 col-lg-6{% end
-00006080: 626c 6f63 6b20 257d 223e 7b7b 2031 5f72  block %}">{{ 1_r
-00006090: 6967 6874 5f61 207d 7d3c 2f64 6976 3e0a  ight_a }}</div>.
-000060a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005fa0: 2020 2020 2020 2020 207b 2520 656c 7365           {% else
+00005fb0: 2025 7d0a 2020 2020 2020 2020 2020 2020   %}.            
+00005fc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005fd0: 2020 2020 2020 2020 3c64 6976 2063 6c61          <div cla
+00005fe0: 7373 3d22 636f 6c2d 3132 223e 7b7b 2031  ss="col-12">{{ 1
+00005ff0: 5f63 656e 7465 725f 626f 7474 6f6d 5f61  _center_bottom_a
+00006000: 207d 7d7b 7b20 315f 6365 6e74 6572 5f62   }}{{ 1_center_b
+00006010: 6f74 746f 6d5f 6220 7d7d 7b7b 2031 5f63  ottom_b }}{{ 1_c
+00006020: 656e 7465 725f 626f 7474 6f6d 5f63 207d  enter_bottom_c }
+00006030: 7d3c 2f64 6976 3e0a 2020 2020 2020 2020  }</div>.        
+00006040: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006050: 2020 2020 2020 2020 7b25 2065 6e64 6966          {% endif
+00006060: 2025 7d0a 2020 2020 2020 2020 2020 2020   %}.            
+00006070: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006080: 3c2f 6469 763e 0a20 2020 2020 2020 2020  </div>.         
+00006090: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000060a0: 2020 207b 2520 656e 6469 6620 257d 0a20     {% endif %}. 
 000060b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000060c0: 2020 2020 3c64 6976 2063 6c61 7373 3d22      <div class="
-000060d0: 7b25 2062 6c6f 636b 2031 5f72 6967 6874  {% block 1_right
-000060e0: 5f61 625f 6220 257d 636f 6c2d 3132 2063  _ab_b %}col-12 c
-000060f0: 6f6c 2d6c 672d 367b 2520 656e 6462 6c6f  ol-lg-6{% endblo
-00006100: 636b 2025 7d22 3e7b 7b20 315f 7269 6768  ck %}">{{ 1_righ
-00006110: 745f 6220 7d7d 3c2f 6469 763e 0a20 2020  t_b }}</div>.   
-00006120: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006130: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006140: 207b 2520 656c 6966 2031 5f72 6967 6874   {% elif 1_right
-00006150: 5f61 2025 7d0a 2020 2020 2020 2020 2020  _a %}.          
-00006160: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006170: 2020 2020 2020 2020 2020 3c64 6976 2063            <div c
-00006180: 6c61 7373 3d22 636f 6c2d 3132 223e 7b7b  lass="col-12">{{
-00006190: 2031 5f72 6967 6874 5f61 207d 7d3c 2f64   1_right_a }}</d
-000061a0: 6976 3e0a 2020 2020 2020 2020 2020 2020  iv>.            
+000060c0: 2020 2020 2020 2020 2020 203c 212d 2d20             <!-- 
+000060d0: 454e 4420 4365 6e74 6572 2062 6f74 746f  END Center botto
+000060e0: 6d20 2d2d 3e0a 0a20 2020 2020 2020 2020  m -->..         
+000060f0: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+00006100: 2f64 6976 3e0a 2020 2020 2020 2020 2020  /div>.          
+00006110: 2020 2020 2020 2020 2020 2020 2020 3c21                <!
+00006120: 2d2d 2045 6e64 2043 656e 7465 7220 636f  -- End Center co
+00006130: 6c75 6d6e 202d 2d3e 0a0a 2020 2020 2020  lumn -->..      
+00006140: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006150: 2020 3c21 2d2d 2042 7569 6c64 2072 6967    <!-- Build rig
+00006160: 6874 2063 6f6c 756d 6e20 2d2d 3e0a 2020  ht column -->.  
+00006170: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006180: 2020 2020 2020 7b25 2069 6620 315f 7269        {% if 1_ri
+00006190: 6768 745f 6120 6f72 2031 5f72 6967 6874  ght_a or 1_right
+000061a0: 5f62 2025 7d0a 2020 2020 2020 2020 2020  _b %}.          
 000061b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000061c0: 2020 2020 2020 2020 7b25 2065 6c73 6520          {% else 
-000061d0: 257d 0a20 2020 2020 2020 2020 2020 2020  %}.             
-000061e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000061f0: 2020 2020 2020 203c 6469 7620 636c 6173         <div clas
-00006200: 733d 2263 6f6c 2d31 3222 3e7b 7b20 315f  s="col-12">{{ 1_
-00006210: 7269 6768 745f 6220 7d7d 3c2f 6469 763e  right_b }}</div>
-00006220: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00006230: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006240: 2020 2020 207b 2520 656e 6469 6620 257d       {% endif %}
-00006250: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00006260: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006270: 203c 2f64 6976 3e0a 2020 2020 2020 2020   </div>.        
+000061c0: 2020 7b25 2069 6620 315f 7269 6768 745f    {% if 1_right_
+000061d0: 6120 616e 6420 315f 7269 6768 745f 6220  a and 1_right_b 
+000061e0: 257d 0a20 2020 2020 2020 2020 2020 2020  %}.             
+000061f0: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+00006200: 6469 7620 636c 6173 733d 227b 2520 626c  div class="{% bl
+00006210: 6f63 6b20 315f 7269 6768 745f 6162 2025  ock 1_right_ab %
+00006220: 7d63 6f6c 2d31 3220 636f 6c2d 6c67 2d34  }col-12 col-lg-4
+00006230: 206d 742d 3520 6d74 2d6c 672d 307b 2520   mt-5 mt-lg-0{% 
+00006240: 656e 6462 6c6f 636b 2025 7d22 3e0a 2020  endblock %}">.  
+00006250: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006260: 2020 2020 2020 2020 2020 7b25 2065 6c69            {% eli
+00006270: 6620 315f 7269 6768 745f 6120 257d 0a20  f 1_right_a %}. 
 00006280: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006290: 2020 2020 3c2f 6469 763e 0a20 2020 2020      </div>.     
-000062a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000062b0: 2020 207b 2520 656e 6469 6620 257d 0a0a     {% endif %}..
-000062c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000062d0: 2020 2020 3c21 2d2d 204e 6f20 626c 6f63      <!-- No bloc
-000062e0: 6b73 2069 6e20 6365 6e74 6572 2070 6f73  ks in center pos
-000062f0: 6974 696f 6e73 202d 2d3e 0a20 2020 2020  itions -->.     
-00006300: 2020 2020 2020 2020 2020 2020 2020 207b                 {
-00006310: 2520 656c 7365 2025 7d0a 2020 2020 2020  % else %}.      
-00006320: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006330: 2020 7b25 2069 6620 315f 6c65 6674 5f61    {% if 1_left_a
-00006340: 206f 7220 315f 6c65 6674 5f62 2025 7d0a   or 1_left_b %}.
-00006350: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006360: 2020 2020 2020 2020 2020 2020 7b25 2069              {% i
-00006370: 6620 315f 6c65 6674 5f61 2061 6e64 2031  f 1_left_a and 1
-00006380: 5f6c 6566 745f 6220 257d 0a20 2020 2020  _left_b %}.     
+00006290: 2020 2020 2020 2020 2020 203c 6469 7620             <div 
+000062a0: 636c 6173 733d 227b 2520 626c 6f63 6b20  class="{% block 
+000062b0: 315f 7269 6768 745f 6120 257d 636f 6c2d  1_right_a %}col-
+000062c0: 3132 2063 6f6c 2d6c 672d 3320 6d74 2d35  12 col-lg-3 mt-5
+000062d0: 206d 742d 6c67 2d30 7b25 2065 6e64 626c   mt-lg-0{% endbl
+000062e0: 6f63 6b20 257d 223e 0a20 2020 2020 2020  ock %}">.       
+000062f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006300: 2020 2020 207b 2520 656c 7365 2025 7d0a       {% else %}.
+00006310: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006320: 2020 2020 2020 2020 2020 2020 3c64 6976              <div
+00006330: 2063 6c61 7373 3d22 7b25 2062 6c6f 636b   class="{% block
+00006340: 2031 5f72 6967 6874 5f62 2025 7d63 6f6c   1_right_b %}col
+00006350: 2d31 3220 636f 6c2d 6c67 2d33 206f 6666  -12 col-lg-3 off
+00006360: 7365 742d 6c67 2d31 206d 742d 3520 6d74  set-lg-1 mt-5 mt
+00006370: 2d6c 672d 307b 2520 656e 6462 6c6f 636b  -lg-0{% endblock
+00006380: 2025 7d22 3e0a 2020 2020 2020 2020 2020   %}">.          
 00006390: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000063a0: 2020 2020 2020 203c 6469 7620 636c 6173         <div clas
-000063b0: 733d 227b 2520 626c 6f63 6b20 315f 6c65  s="{% block 1_le
-000063c0: 6674 5f6e 6f5f 6365 6e74 6572 5f61 6220  ft_no_center_ab 
-000063d0: 257d 636f 6c2d 3132 2063 6f6c 2d6d 642d  %}col-12 col-md-
-000063e0: 367b 2520 656e 6462 6c6f 636b 2025 7d22  6{% endblock %}"
-000063f0: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
-00006400: 2020 2020 2020 2020 2020 2020 2020 7b25                {%
-00006410: 2065 6c69 6620 315f 6c65 6674 5f61 2025   elif 1_left_a %
-00006420: 7d0a 2020 2020 2020 2020 2020 2020 2020  }.              
-00006430: 2020 2020 2020 2020 2020 2020 2020 3c64                <d
-00006440: 6976 2063 6c61 7373 3d22 7b25 2062 6c6f  iv class="{% blo
-00006450: 636b 2031 5f6c 6566 745f 6e6f 5f63 656e  ck 1_left_no_cen
-00006460: 7465 725f 6120 257d 636f 6c2d 3132 2063  ter_a %}col-12 c
-00006470: 6f6c 2d6d 642d 367b 2520 656e 6462 6c6f  ol-md-6{% endblo
-00006480: 636b 2025 7d22 3e0a 2020 2020 2020 2020  ck %}">.        
-00006490: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000064a0: 2020 2020 7b25 2065 6c69 6620 315f 6c65      {% elif 1_le
-000064b0: 6674 5f62 2025 7d0a 2020 2020 2020 2020  ft_b %}.        
-000064c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000064d0: 2020 2020 3c64 6976 2063 6c61 7373 3d22      <div class="
-000064e0: 7b25 2062 6c6f 636b 2031 5f6c 6566 745f  {% block 1_left_
-000064f0: 6e6f 5f63 656e 7465 725f 6220 257d 636f  no_center_b %}co
-00006500: 6c2d 3132 2063 6f6c 2d6d 642d 367b 2520  l-12 col-md-6{% 
-00006510: 656e 6462 6c6f 636b 2025 7d22 3e0a 2020  endblock %}">.  
+000063a0: 2020 7b25 2065 6e64 6966 2025 7d0a 2020    {% endif %}.  
+000063b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000063c0: 2020 2020 2020 2020 2020 2020 2020 3c64                <d
+000063d0: 6976 2063 6c61 7373 3d22 726f 7722 3e0a  iv class="row">.
+000063e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000063f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006400: 2020 2020 7b25 2069 6620 315f 7269 6768      {% if 1_righ
+00006410: 745f 6120 616e 6420 315f 7269 6768 745f  t_a and 1_right_
+00006420: 6220 257d 0a20 2020 2020 2020 2020 2020  b %}.           
+00006430: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006440: 2020 2020 2020 2020 203c 6469 7620 636c           <div cl
+00006450: 6173 733d 227b 2520 626c 6f63 6b20 315f  ass="{% block 1_
+00006460: 7269 6768 745f 6162 5f61 2025 7d63 6f6c  right_ab_a %}col
+00006470: 2d31 3220 636f 6c2d 6c67 2d36 7b25 2065  -12 col-lg-6{% e
+00006480: 6e64 626c 6f63 6b20 257d 223e 7b7b 2031  ndblock %}">{{ 1
+00006490: 5f72 6967 6874 5f61 207d 7d3c 2f64 6976  _right_a }}</div
+000064a0: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
+000064b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000064c0: 2020 2020 2020 3c64 6976 2063 6c61 7373        <div class
+000064d0: 3d22 7b25 2062 6c6f 636b 2031 5f72 6967  ="{% block 1_rig
+000064e0: 6874 5f61 625f 6220 257d 636f 6c2d 3132  ht_ab_b %}col-12
+000064f0: 2063 6f6c 2d6c 672d 367b 2520 656e 6462   col-lg-6{% endb
+00006500: 6c6f 636b 2025 7d22 3e7b 7b20 315f 7269  lock %}">{{ 1_ri
+00006510: 6768 745f 6220 7d7d 3c2f 6469 763e 0a20  ght_b }}</div>. 
 00006520: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006530: 2020 2020 2020 2020 2020 7b25 2065 6e64            {% end
-00006540: 6966 2025 7d0a 2020 2020 2020 2020 2020  if %}.          
-00006550: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006560: 2020 2020 2020 3c64 6976 2063 6c61 7373        <div class
-00006570: 3d22 726f 7722 3e0a 2020 2020 2020 2020  ="row">.        
-00006580: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006590: 2020 2020 2020 2020 2020 2020 7b25 2069              {% i
-000065a0: 6620 315f 6c65 6674 5f61 2061 6e64 2031  f 1_left_a and 1
-000065b0: 5f6c 6566 745f 6220 257d 0a20 2020 2020  _left_b %}.     
-000065c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000065d0: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-000065e0: 6469 7620 636c 6173 733d 227b 2520 626c  div class="{% bl
-000065f0: 6f63 6b20 315f 6c65 6674 5f6e 6f5f 6365  ock 1_left_no_ce
-00006600: 6e74 6572 5f61 625f 6120 257d 636f 6c2d  nter_ab_a %}col-
-00006610: 3132 2063 6f6c 2d6d 642d 367b 2520 656e  12 col-md-6{% en
-00006620: 6462 6c6f 636b 2025 7d22 3e7b 7b20 315f  dblock %}">{{ 1_
-00006630: 6c65 6674 5f61 207d 7d3c 2f64 6976 3e0a  left_a }}</div>.
-00006640: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006650: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006660: 2020 2020 3c64 6976 2063 6c61 7373 3d22      <div class="
-00006670: 7b25 2062 6c6f 636b 2031 5f6c 6566 745f  {% block 1_left_
-00006680: 6e6f 5f63 656e 7465 725f 6162 5f62 2025  no_center_ab_b %
-00006690: 7d63 6f6c 2d31 3220 636f 6c2d 6d64 2d36  }col-12 col-md-6
-000066a0: 7b25 2065 6e64 626c 6f63 6b20 257d 223e  {% endblock %}">
-000066b0: 7b7b 2031 5f6c 6566 745f 6220 7d7d 3c2f  {{ 1_left_b }}</
-000066c0: 6469 763e 0a20 2020 2020 2020 2020 2020  div>.           
-000066d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000066e0: 2020 2020 2020 2020 207b 2520 656c 6966           {% elif
-000066f0: 2031 5f6c 6566 745f 6120 257d 0a20 2020   1_left_a %}.   
+00006530: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006540: 2020 207b 2520 656c 6966 2031 5f72 6967     {% elif 1_rig
+00006550: 6874 5f61 2025 7d0a 2020 2020 2020 2020  ht_a %}.        
+00006560: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006570: 2020 2020 2020 2020 2020 2020 3c64 6976              <div
+00006580: 2063 6c61 7373 3d22 636f 6c2d 3132 223e   class="col-12">
+00006590: 7b7b 2031 5f72 6967 6874 5f61 207d 7d3c  {{ 1_right_a }}<
+000065a0: 2f64 6976 3e0a 2020 2020 2020 2020 2020  /div>.          
+000065b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000065c0: 2020 2020 2020 2020 2020 7b25 2065 6c73            {% els
+000065d0: 6520 257d 0a20 2020 2020 2020 2020 2020  e %}.           
+000065e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000065f0: 2020 2020 2020 2020 203c 6469 7620 636c           <div cl
+00006600: 6173 733d 2263 6f6c 2d31 3222 3e7b 7b20  ass="col-12">{{ 
+00006610: 315f 7269 6768 745f 6220 7d7d 3c2f 6469  1_right_b }}</di
+00006620: 763e 0a20 2020 2020 2020 2020 2020 2020  v>.             
+00006630: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006640: 2020 2020 2020 207b 2520 656e 6469 6620         {% endif 
+00006650: 257d 0a20 2020 2020 2020 2020 2020 2020  %}.             
+00006660: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006670: 2020 203c 2f64 6976 3e0a 2020 2020 2020     </div>.      
+00006680: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006690: 2020 2020 2020 3c2f 6469 763e 0a20 2020        </div>.   
+000066a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000066b0: 2020 2020 207b 2520 656e 6469 6620 257d       {% endif %}
+000066c0: 0a0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000066d0: 2020 2020 2020 3c21 2d2d 204e 6f20 626c        <!-- No bl
+000066e0: 6f63 6b73 2069 6e20 6365 6e74 6572 2070  ocks in center p
+000066f0: 6f73 6974 696f 6e73 202d 2d3e 0a20 2020  ositions -->.   
 00006700: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006710: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006720: 203c 6469 7620 636c 6173 733d 2263 6f6c   <div class="col
-00006730: 2d31 3222 3e7b 7b20 315f 6c65 6674 5f61  -12">{{ 1_left_a
-00006740: 207d 7d3c 2f64 6976 3e0a 2020 2020 2020   }}</div>.      
-00006750: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006710: 207b 2520 656c 7365 2025 7d0a 2020 2020   {% else %}.    
+00006720: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006730: 2020 2020 7b25 2069 6620 315f 6c65 6674      {% if 1_left
+00006740: 5f61 206f 7220 315f 6c65 6674 5f62 2025  _a or 1_left_b %
+00006750: 7d0a 2020 2020 2020 2020 2020 2020 2020  }.              
 00006760: 2020 2020 2020 2020 2020 2020 2020 7b25                {%
-00006770: 2065 6c73 6520 257d 0a20 2020 2020 2020   else %}.       
-00006780: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006790: 2020 2020 2020 2020 2020 2020 203c 6469               <di
-000067a0: 7620 636c 6173 733d 2263 6f6c 2d31 3222  v class="col-12"
-000067b0: 3e7b 7b20 315f 6c65 6674 5f62 207d 7d3c  >{{ 1_left_b }}<
-000067c0: 2f64 6976 3e0a 2020 2020 2020 2020 2020  /div>.          
-000067d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000067e0: 2020 2020 2020 2020 2020 7b25 2065 6e64            {% end
-000067f0: 6966 2025 7d0a 2020 2020 2020 2020 2020  if %}.          
+00006770: 2069 6620 315f 6c65 6674 5f61 2061 6e64   if 1_left_a and
+00006780: 2031 5f6c 6566 745f 6220 257d 0a20 2020   1_left_b %}.   
+00006790: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000067a0: 2020 2020 2020 2020 203c 6469 7620 636c           <div cl
+000067b0: 6173 733d 227b 2520 626c 6f63 6b20 315f  ass="{% block 1_
+000067c0: 6c65 6674 5f6e 6f5f 6365 6e74 6572 5f61  left_no_center_a
+000067d0: 6220 257d 636f 6c2d 3132 2063 6f6c 2d6d  b %}col-12 col-m
+000067e0: 642d 367b 2520 656e 6462 6c6f 636b 2025  d-6{% endblock %
+000067f0: 7d22 3e0a 2020 2020 2020 2020 2020 2020  }">.            
 00006800: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006810: 2020 2020 2020 3c2f 6469 763e 0a20 2020        </div>.   
-00006820: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006830: 2020 2020 2020 2020 203c 2f64 6976 3e0a           </div>.
-00006840: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006850: 2020 2020 2020 2020 7b25 2065 6e64 6966          {% endif
-00006860: 2025 7d0a 0a20 2020 2020 2020 2020 2020   %}..           
-00006870: 2020 2020 2020 2020 2020 2020 207b 2520               {% 
-00006880: 6966 2031 5f72 6967 6874 5f61 206f 7220  if 1_right_a or 
-00006890: 315f 7269 6768 745f 6220 257d 0a20 2020  1_right_b %}.   
-000068a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000068b0: 2020 2020 2020 2020 207b 2520 6966 2031           {% if 1
-000068c0: 5f72 6967 6874 5f61 2061 6e64 2031 5f72  _right_a and 1_r
-000068d0: 6967 6874 5f62 2025 7d0a 2020 2020 2020  ight_b %}.      
-000068e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000068f0: 2020 2020 2020 3c64 6976 2063 6c61 7373        <div class
-00006900: 3d22 7b25 2062 6c6f 636b 2031 5f72 6967  ="{% block 1_rig
-00006910: 6874 5f6e 6f5f 6365 6e74 6572 5f61 6220  ht_no_center_ab 
-00006920: 257d 636f 6c2d 3132 2063 6f6c 2d6d 642d  %}col-12 col-md-
-00006930: 367b 2520 656e 6462 6c6f 636b 2025 7d22  6{% endblock %}"
-00006940: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
-00006950: 2020 2020 2020 2020 2020 2020 2020 7b25                {%
-00006960: 2065 6c69 6620 315f 7269 6768 745f 6120   elif 1_right_a 
-00006970: 257d 0a20 2020 2020 2020 2020 2020 2020  %}.             
-00006980: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-00006990: 6469 7620 636c 6173 733d 227b 2520 626c  div class="{% bl
-000069a0: 6f63 6b20 315f 7269 6768 745f 6e6f 5f63  ock 1_right_no_c
-000069b0: 656e 7465 725f 6120 257d 636f 6c2d 3132  enter_a %}col-12
-000069c0: 2063 6f6c 2d6d 642d 367b 2520 656e 6462   col-md-6{% endb
-000069d0: 6c6f 636b 2025 7d22 3e0a 2020 2020 2020  lock %}">.      
-000069e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000069f0: 2020 2020 2020 7b25 2065 6c69 6620 315f        {% elif 1_
-00006a00: 7269 6768 745f 6220 257d 0a20 2020 2020  right_b %}.     
-00006a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006a20: 2020 2020 2020 203c 6469 7620 636c 6173         <div clas
-00006a30: 733d 227b 2520 626c 6f63 6b20 315f 7269  s="{% block 1_ri
-00006a40: 6768 745f 6e6f 5f63 656e 7465 725f 6220  ght_no_center_b 
-00006a50: 257d 636f 6c2d 3132 2063 6f6c 2d6d 642d  %}col-12 col-md-
-00006a60: 367b 2520 656e 6462 6c6f 636b 2025 7d22  6{% endblock %}"
-00006a70: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
-00006a80: 2020 2020 2020 2020 2020 2020 2020 7b25                {%
-00006a90: 2065 6e64 6966 2025 7d0a 2020 2020 2020   endif %}.      
-00006aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006ab0: 2020 2020 2020 2020 2020 3c64 6976 2063            <div c
-00006ac0: 6c61 7373 3d22 726f 7722 3e0a 2020 2020  lass="row">.    
+00006810: 7b25 2065 6c69 6620 315f 6c65 6674 5f61  {% elif 1_left_a
+00006820: 2025 7d0a 2020 2020 2020 2020 2020 2020   %}.            
+00006830: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006840: 3c64 6976 2063 6c61 7373 3d22 7b25 2062  <div class="{% b
+00006850: 6c6f 636b 2031 5f6c 6566 745f 6e6f 5f63  lock 1_left_no_c
+00006860: 656e 7465 725f 6120 257d 636f 6c2d 3132  enter_a %}col-12
+00006870: 2063 6f6c 2d6d 642d 367b 2520 656e 6462   col-md-6{% endb
+00006880: 6c6f 636b 2025 7d22 3e0a 2020 2020 2020  lock %}">.      
+00006890: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000068a0: 2020 2020 2020 7b25 2065 6c69 6620 315f        {% elif 1_
+000068b0: 6c65 6674 5f62 2025 7d0a 2020 2020 2020  left_b %}.      
+000068c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000068d0: 2020 2020 2020 3c64 6976 2063 6c61 7373        <div class
+000068e0: 3d22 7b25 2062 6c6f 636b 2031 5f6c 6566  ="{% block 1_lef
+000068f0: 745f 6e6f 5f63 656e 7465 725f 6220 257d  t_no_center_b %}
+00006900: 636f 6c2d 3132 2063 6f6c 2d6d 642d 367b  col-12 col-md-6{
+00006910: 2520 656e 6462 6c6f 636b 2025 7d22 3e0a  % endblock %}">.
+00006920: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006930: 2020 2020 2020 2020 2020 2020 7b25 2065              {% e
+00006940: 6e64 6966 2025 7d0a 2020 2020 2020 2020  ndif %}.        
+00006950: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006960: 2020 2020 2020 2020 3c64 6976 2063 6c61          <div cla
+00006970: 7373 3d22 726f 7722 3e0a 2020 2020 2020  ss="row">.      
+00006980: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006990: 2020 2020 2020 2020 2020 2020 2020 7b25                {%
+000069a0: 2069 6620 315f 6c65 6674 5f61 2061 6e64   if 1_left_a and
+000069b0: 2031 5f6c 6566 745f 6220 257d 0a20 2020   1_left_b %}.   
+000069c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000069d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000069e0: 203c 6469 7620 636c 6173 733d 227b 2520   <div class="{% 
+000069f0: 626c 6f63 6b20 315f 6c65 6674 5f6e 6f5f  block 1_left_no_
+00006a00: 6365 6e74 6572 5f61 625f 6120 257d 636f  center_ab_a %}co
+00006a10: 6c2d 3132 2063 6f6c 2d6d 642d 367b 2520  l-12 col-md-6{% 
+00006a20: 656e 6462 6c6f 636b 2025 7d22 3e7b 7b20  endblock %}">{{ 
+00006a30: 315f 6c65 6674 5f61 207d 7d3c 2f64 6976  1_left_a }}</div
+00006a40: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
+00006a50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006a60: 2020 2020 2020 3c64 6976 2063 6c61 7373        <div class
+00006a70: 3d22 7b25 2062 6c6f 636b 2031 5f6c 6566  ="{% block 1_lef
+00006a80: 745f 6e6f 5f63 656e 7465 725f 6162 5f62  t_no_center_ab_b
+00006a90: 2025 7d63 6f6c 2d31 3220 636f 6c2d 6d64   %}col-12 col-md
+00006aa0: 2d36 7b25 2065 6e64 626c 6f63 6b20 257d  -6{% endblock %}
+00006ab0: 223e 7b7b 2031 5f6c 6566 745f 6220 7d7d  ">{{ 1_left_b }}
+00006ac0: 3c2f 6469 763e 0a20 2020 2020 2020 2020  </div>.         
 00006ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006af0: 7b25 2069 6620 315f 7269 6768 745f 6120  {% if 1_right_a 
-00006b00: 616e 6420 315f 7269 6768 745f 6220 257d  and 1_right_b %}
-00006b10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00006b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006b30: 2020 2020 203c 6469 7620 636c 6173 733d       <div class=
-00006b40: 227b 2520 626c 6f63 6b20 315f 7269 6768  "{% block 1_righ
-00006b50: 745f 6e6f 5f63 656e 7465 725f 6162 5f61  t_no_center_ab_a
-00006b60: 2025 7d63 6f6c 2d31 3220 636f 6c2d 6d64   %}col-12 col-md
-00006b70: 2d36 7b25 2065 6e64 626c 6f63 6b20 257d  -6{% endblock %}
-00006b80: 223e 7b7b 2031 5f72 6967 6874 5f61 207d  ">{{ 1_right_a }
-00006b90: 7d3c 2f64 6976 3e0a 2020 2020 2020 2020  }</div>.        
-00006ba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006bb0: 2020 2020 2020 2020 2020 2020 3c64 6976              <div
-00006bc0: 2063 6c61 7373 3d22 7b25 2062 6c6f 636b   class="{% block
-00006bd0: 2031 5f72 6967 6874 5f6e 6f5f 6365 6e74   1_right_no_cent
-00006be0: 6572 5f61 625f 6220 257d 636f 6c2d 3132  er_ab_b %}col-12
-00006bf0: 2063 6f6c 2d6d 642d 367b 2520 656e 6462   col-md-6{% endb
-00006c00: 6c6f 636b 2025 7d22 3e7b 7b20 315f 7269  lock %}">{{ 1_ri
-00006c10: 6768 745f 6220 7d7d 2f64 6976 3e0a 2020  ght_b }}/div>.  
+00006ae0: 2020 2020 2020 2020 2020 207b 2520 656c             {% el
+00006af0: 6966 2031 5f6c 6566 745f 6120 257d 0a20  if 1_left_a %}. 
+00006b00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006b20: 2020 203c 6469 7620 636c 6173 733d 2263     <div class="c
+00006b30: 6f6c 2d31 3222 3e7b 7b20 315f 6c65 6674  ol-12">{{ 1_left
+00006b40: 5f61 207d 7d3c 2f64 6976 3e0a 2020 2020  _a }}</div>.    
+00006b50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006b60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006b70: 7b25 2065 6c73 6520 257d 0a20 2020 2020  {% else %}.     
+00006b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006b90: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+00006ba0: 6469 7620 636c 6173 733d 2263 6f6c 2d31  div class="col-1
+00006bb0: 3222 3e7b 7b20 315f 6c65 6674 5f62 207d  2">{{ 1_left_b }
+00006bc0: 7d3c 2f64 6976 3e0a 2020 2020 2020 2020  }</div>.        
+00006bd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006be0: 2020 2020 2020 2020 2020 2020 7b25 2065              {% e
+00006bf0: 6e64 6966 2025 7d0a 2020 2020 2020 2020  ndif %}.        
+00006c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006c10: 2020 2020 2020 2020 3c2f 6469 763e 0a20          </div>. 
 00006c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006c30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006c40: 2020 7b25 2065 6c69 6620 315f 7269 6768    {% elif 1_righ
-00006c50: 745f 6120 257d 0a20 2020 2020 2020 2020  t_a %}.         
-00006c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006c70: 2020 2020 2020 2020 2020 203c 6469 7620             <div 
-00006c80: 636c 6173 733d 2263 6f6c 2d31 3222 3e7b  class="col-12">{
-00006c90: 7b20 315f 7269 6768 745f 6120 7d7d 3c2f  { 1_right_a }}</
-00006ca0: 6469 763e 0a20 2020 2020 2020 2020 2020  div>.           
-00006cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006cc0: 2020 2020 2020 2020 207b 2520 656c 7365           {% else
-00006cd0: 2025 7d0a 2020 2020 2020 2020 2020 2020   %}.            
+00006c30: 2020 2020 2020 2020 2020 203c 2f64 6976             </div
+00006c40: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
+00006c50: 2020 2020 2020 2020 2020 7b25 2065 6e64            {% end
+00006c60: 6966 2025 7d0a 0a20 2020 2020 2020 2020  if %}..         
+00006c70: 2020 2020 2020 2020 2020 2020 2020 207b                 {
+00006c80: 2520 6966 2031 5f72 6967 6874 5f61 206f  % if 1_right_a o
+00006c90: 7220 315f 7269 6768 745f 6220 257d 0a20  r 1_right_b %}. 
+00006ca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006cb0: 2020 2020 2020 2020 2020 207b 2520 6966             {% if
+00006cc0: 2031 5f72 6967 6874 5f61 2061 6e64 2031   1_right_a and 1
+00006cd0: 5f72 6967 6874 5f62 2025 7d0a 2020 2020  _right_b %}.    
 00006ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00006cf0: 2020 2020 2020 2020 3c64 6976 2063 6c61          <div cla
-00006d00: 7373 3d22 636f 6c2d 3132 223e 7b7b 2031  ss="col-12">{{ 1
-00006d10: 5f72 6967 6874 5f62 207d 7d3c 2f64 6976  _right_b }}</div
-00006d20: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
-00006d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006d40: 2020 2020 2020 7b25 2065 6e64 6966 2025        {% endif %
-00006d50: 7d0a 2020 2020 2020 2020 2020 2020 2020  }.              
-00006d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006d70: 2020 3c2f 6469 763e 0a20 2020 2020 2020    </div>.       
+00006d00: 7373 3d22 7b25 2062 6c6f 636b 2031 5f72  ss="{% block 1_r
+00006d10: 6967 6874 5f6e 6f5f 6365 6e74 6572 5f61  ight_no_center_a
+00006d20: 6220 257d 636f 6c2d 3132 2063 6f6c 2d6d  b %}col-12 col-m
+00006d30: 642d 367b 2520 656e 6462 6c6f 636b 2025  d-6{% endblock %
+00006d40: 7d22 3e0a 2020 2020 2020 2020 2020 2020  }">.            
+00006d50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006d60: 7b25 2065 6c69 6620 315f 7269 6768 745f  {% elif 1_right_
+00006d70: 6120 257d 0a20 2020 2020 2020 2020 2020  a %}.           
 00006d80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006d90: 2020 2020 203c 2f64 6976 3e0a 2020 2020       </div>.    
-00006da0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006db0: 2020 2020 7b25 2065 6e64 6966 2025 7d0a      {% endif %}.
-00006dc0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00006dd0: 2020 2020 207b 2520 656e 6469 6620 257d       {% endif %}
-00006de0: 0a0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00006df0: 2020 2020 2020 3c21 2d2d 2042 6c6f 636b        <!-- Block
-00006e00: 7320 696e 206d 6964 646c 6520 626f 7474  s in middle bott
-00006e10: 6f6d 2070 6f73 6974 696f 6e20 2d2d 3e0a  om position -->.
-00006e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006e30: 2020 2020 7b25 2069 6620 315f 6d69 645f      {% if 1_mid_
-00006e40: 626f 7474 6f6d 5f61 206f 7220 315f 6d69  bottom_a or 1_mi
-00006e50: 645f 626f 7474 6f6d 5f62 206f 7220 315f  d_bottom_b or 1_
-00006e60: 6d69 645f 626f 7474 6f6d 5f63 2025 7d0a  mid_bottom_c %}.
-00006e70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006e80: 2020 2020 3c64 6976 2063 6c61 7373 3d22      <div class="
-00006e90: 636f 6c2d 3132 223e 0a20 2020 2020 2020  col-12">.       
+00006d90: 203c 6469 7620 636c 6173 733d 227b 2520   <div class="{% 
+00006da0: 626c 6f63 6b20 315f 7269 6768 745f 6e6f  block 1_right_no
+00006db0: 5f63 656e 7465 725f 6120 257d 636f 6c2d  _center_a %}col-
+00006dc0: 3132 2063 6f6c 2d6d 642d 367b 2520 656e  12 col-md-6{% en
+00006dd0: 6462 6c6f 636b 2025 7d22 3e0a 2020 2020  dblock %}">.    
+00006de0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006df0: 2020 2020 2020 2020 7b25 2065 6c69 6620          {% elif 
+00006e00: 315f 7269 6768 745f 6220 257d 0a20 2020  1_right_b %}.   
+00006e10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006e20: 2020 2020 2020 2020 203c 6469 7620 636c           <div cl
+00006e30: 6173 733d 227b 2520 626c 6f63 6b20 315f  ass="{% block 1_
+00006e40: 7269 6768 745f 6e6f 5f63 656e 7465 725f  right_no_center_
+00006e50: 6220 257d 636f 6c2d 3132 2063 6f6c 2d6d  b %}col-12 col-m
+00006e60: 642d 367b 2520 656e 6462 6c6f 636b 2025  d-6{% endblock %
+00006e70: 7d22 3e0a 2020 2020 2020 2020 2020 2020  }">.            
+00006e80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006e90: 7b25 2065 6e64 6966 2025 7d0a 2020 2020  {% endif %}.    
 00006ea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006eb0: 203c 6469 7620 636c 6173 733d 2272 6f77   <div class="row
-00006ec0: 223e 0a20 2020 2020 2020 2020 2020 2020  ">.             
-00006ed0: 2020 2020 2020 2020 2020 2020 2020 207b                 {
-00006ee0: 2520 6966 2031 5f6d 6964 5f62 6f74 746f  % if 1_mid_botto
-00006ef0: 6d5f 6120 616e 6420 315f 6d69 645f 626f  m_a and 1_mid_bo
-00006f00: 7474 6f6d 5f62 2061 6e64 2031 5f6d 6964  ttom_b and 1_mid
-00006f10: 5f62 6f74 746f 6d5f 6320 257d 0a20 2020  _bottom_c %}.   
+00006eb0: 2020 2020 2020 2020 2020 2020 3c64 6976              <div
+00006ec0: 2063 6c61 7373 3d22 726f 7722 3e0a 2020   class="row">.  
+00006ed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006ee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006ef0: 2020 7b25 2069 6620 315f 7269 6768 745f    {% if 1_right_
+00006f00: 6120 616e 6420 315f 7269 6768 745f 6220  a and 1_right_b 
+00006f10: 257d 0a20 2020 2020 2020 2020 2020 2020  %}.             
 00006f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006f30: 2020 2020 2020 2020 2020 2020 203c 6469               <di
-00006f40: 7620 636c 6173 733d 227b 2520 626c 6f63  v class="{% bloc
-00006f50: 6b20 315f 6d69 645f 626f 7474 6f6d 5f61  k 1_mid_bottom_a
-00006f60: 6263 5f61 2025 7d63 6f6c 2d31 3220 636f  bc_a %}col-12 co
-00006f70: 6c2d 6d64 2d34 7b25 2065 6e64 626c 6f63  l-md-4{% endbloc
-00006f80: 6b20 257d 223e 7b7b 2031 5f6d 6964 5f62  k %}">{{ 1_mid_b
-00006f90: 6f74 746f 6d5f 6120 7d7d 3c2f 6469 763e  ottom_a }}</div>
-00006fa0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00006fb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006fc0: 203c 6469 7620 636c 6173 733d 227b 2520   <div class="{% 
-00006fd0: 626c 6f63 6b20 315f 6d69 645f 626f 7474  block 1_mid_bott
-00006fe0: 6f6d 5f61 6263 5f62 2025 7d63 6f6c 2d31  om_abc_b %}col-1
-00006ff0: 3220 636f 6c2d 6d64 2d34 7b25 2065 6e64  2 col-md-4{% end
-00007000: 626c 6f63 6b20 257d 223e 7b7b 2031 5f6d  block %}">{{ 1_m
-00007010: 6964 5f62 6f74 746f 6d5f 6220 7d7d 3c2f  id_bottom_b }}</
-00007020: 6469 763e 0a20 2020 2020 2020 2020 2020  div>.           
+00006f30: 2020 2020 2020 203c 6469 7620 636c 6173         <div clas
+00006f40: 733d 227b 2520 626c 6f63 6b20 315f 7269  s="{% block 1_ri
+00006f50: 6768 745f 6e6f 5f63 656e 7465 725f 6162  ght_no_center_ab
+00006f60: 5f61 2025 7d63 6f6c 2d31 3220 636f 6c2d  _a %}col-12 col-
+00006f70: 6d64 2d36 7b25 2065 6e64 626c 6f63 6b20  md-6{% endblock 
+00006f80: 257d 223e 7b7b 2031 5f72 6967 6874 5f61  %}">{{ 1_right_a
+00006f90: 207d 7d3c 2f64 6976 3e0a 2020 2020 2020   }}</div>.      
+00006fa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006fb0: 2020 2020 2020 2020 2020 2020 2020 3c64                <d
+00006fc0: 6976 2063 6c61 7373 3d22 7b25 2062 6c6f  iv class="{% blo
+00006fd0: 636b 2031 5f72 6967 6874 5f6e 6f5f 6365  ck 1_right_no_ce
+00006fe0: 6e74 6572 5f61 625f 6220 257d 636f 6c2d  nter_ab_b %}col-
+00006ff0: 3132 2063 6f6c 2d6d 642d 367b 2520 656e  12 col-md-6{% en
+00007000: 6462 6c6f 636b 2025 7d22 3e7b 7b20 315f  dblock %}">{{ 1_
+00007010: 7269 6768 745f 6220 7d7d 2f64 6976 3e0a  right_b }}/div>.
+00007020: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00007030: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007040: 2020 2020 203c 6469 7620 636c 6173 733d       <div class=
-00007050: 227b 2520 626c 6f63 6b20 315f 6d69 645f  "{% block 1_mid_
-00007060: 626f 7474 6f6d 5f61 6263 5f63 2025 7d63  bottom_abc_c %}c
-00007070: 6f6c 2d31 3220 636f 6c2d 6d64 2d34 7b25  ol-12 col-md-4{%
-00007080: 2065 6e64 626c 6f63 6b20 257d 223e 7b7b   endblock %}">{{
-00007090: 2031 5f6d 6964 5f62 6f74 746f 6d5f 6320   1_mid_bottom_c 
-000070a0: 7d7d 3c2f 6469 763e 0a20 2020 2020 2020  }}</div>.       
+00007040: 2020 2020 7b25 2065 6c69 6620 315f 7269      {% elif 1_ri
+00007050: 6768 745f 6120 257d 0a20 2020 2020 2020  ght_a %}.       
+00007060: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007070: 2020 2020 2020 2020 2020 2020 203c 6469               <di
+00007080: 7620 636c 6173 733d 2263 6f6c 2d31 3222  v class="col-12"
+00007090: 3e7b 7b20 315f 7269 6768 745f 6120 7d7d  >{{ 1_right_a }}
+000070a0: 3c2f 6469 763e 0a20 2020 2020 2020 2020  </div>.         
 000070b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000070c0: 2020 2020 207b 2520 656c 6966 2031 5f6d       {% elif 1_m
-000070d0: 6964 5f62 6f74 746f 6d5f 6120 616e 6420  id_bottom_a and 
-000070e0: 315f 6d69 645f 626f 7474 6f6d 5f62 2025  1_mid_bottom_b %
-000070f0: 7d0a 2020 2020 2020 2020 2020 2020 2020  }.              
-00007100: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007110: 2020 3c64 6976 2063 6c61 7373 3d22 7b25    <div class="{%
-00007120: 2062 6c6f 636b 2031 5f6d 6964 5f62 6f74   block 1_mid_bot
-00007130: 746f 6d5f 6162 5f61 2025 7d63 6f6c 2d31  tom_ab_a %}col-1
-00007140: 3220 636f 6c2d 6d64 2d38 7b25 2065 6e64  2 col-md-8{% end
-00007150: 626c 6f63 6b20 257d 223e 7b7b 2031 5f6d  block %}">{{ 1_m
-00007160: 6964 5f62 6f74 746f 6d5f 6120 7d7d 3c2f  id_bottom_a }}</
-00007170: 6469 763e 0a20 2020 2020 2020 2020 2020  div>.           
+000070c0: 2020 2020 2020 2020 2020 207b 2520 656c             {% el
+000070d0: 7365 2025 7d0a 2020 2020 2020 2020 2020  se %}.          
+000070e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000070f0: 2020 2020 2020 2020 2020 3c64 6976 2063            <div c
+00007100: 6c61 7373 3d22 636f 6c2d 3132 223e 7b7b  lass="col-12">{{
+00007110: 2031 5f72 6967 6874 5f62 207d 7d3c 2f64   1_right_b }}</d
+00007120: 6976 3e0a 2020 2020 2020 2020 2020 2020  iv>.            
+00007130: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007140: 2020 2020 2020 2020 7b25 2065 6e64 6966          {% endif
+00007150: 2025 7d0a 2020 2020 2020 2020 2020 2020   %}.            
+00007160: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007170: 2020 2020 3c2f 6469 763e 0a20 2020 2020      </div>.     
 00007180: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007190: 2020 2020 203c 6469 7620 636c 6173 733d       <div class=
-000071a0: 227b 2520 626c 6f63 6b20 315f 6d69 645f  "{% block 1_mid_
-000071b0: 626f 7474 6f6d 5f61 625f 6220 257d 636f  bottom_ab_b %}co
-000071c0: 6c2d 3132 2063 6f6c 2d6d 642d 347b 2520  l-12 col-md-4{% 
-000071d0: 656e 6462 6c6f 636b 2025 7d22 3e7b 7b20  endblock %}">{{ 
-000071e0: 315f 6d69 645f 626f 7474 6f6d 5f62 207d  1_mid_bottom_b }
-000071f0: 7d3c 2f64 6976 3e0a 2020 2020 2020 2020  }</div>.        
-00007200: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007210: 2020 2020 7b25 2065 6c69 6620 315f 6d69      {% elif 1_mi
-00007220: 645f 626f 7474 6f6d 5f61 2061 6e64 2031  d_bottom_a and 1
-00007230: 5f6d 6964 5f62 6f74 746f 6d5f 6320 257d  _mid_bottom_c %}
-00007240: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00007250: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007260: 203c 6469 7620 636c 6173 733d 227b 2520   <div class="{% 
-00007270: 626c 6f63 6b20 315f 6d69 645f 626f 7474  block 1_mid_bott
-00007280: 6f6d 5f61 635f 6120 257d 636f 6c2d 3132  om_ac_a %}col-12
-00007290: 2063 6f6c 2d6d 642d 367b 2520 656e 6462   col-md-6{% endb
-000072a0: 6c6f 636b 2025 7d22 3e7b 7b20 315f 6d69  lock %}">{{ 1_mi
-000072b0: 645f 626f 7474 6f6d 5f61 207d 7d3c 2f64  d_bottom_a }}</d
-000072c0: 6976 3e0a 2020 2020 2020 2020 2020 2020  iv>.            
+00007190: 2020 2020 2020 203c 2f64 6976 3e0a 2020         </div>.  
+000071a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000071b0: 2020 2020 2020 7b25 2065 6e64 6966 2025        {% endif %
+000071c0: 7d0a 0a20 2020 2020 2020 2020 2020 2020  }..             
+000071d0: 2020 2020 2020 207b 2520 656e 6469 6620         {% endif 
+000071e0: 257d 0a0a 2020 2020 2020 2020 2020 2020  %}..            
+000071f0: 2020 2020 2020 2020 3c21 2d2d 2042 6c6f          <!-- Blo
+00007200: 636b 7320 696e 206d 6964 646c 6520 626f  cks in middle bo
+00007210: 7474 6f6d 2070 6f73 6974 696f 6e20 2d2d  ttom position --
+00007220: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
+00007230: 2020 2020 2020 7b25 2069 6620 315f 6d69        {% if 1_mi
+00007240: 645f 626f 7474 6f6d 5f61 206f 7220 315f  d_bottom_a or 1_
+00007250: 6d69 645f 626f 7474 6f6d 5f62 206f 7220  mid_bottom_b or 
+00007260: 315f 6d69 645f 626f 7474 6f6d 5f63 2025  1_mid_bottom_c %
+00007270: 7d0a 2020 2020 2020 2020 2020 2020 2020  }.              
+00007280: 2020 2020 2020 3c64 6976 2063 6c61 7373        <div class
+00007290: 3d22 636f 6c2d 3132 223e 0a20 2020 2020  ="col-12">.     
+000072a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000072b0: 2020 203c 6469 7620 636c 6173 733d 2272     <div class="r
+000072c0: 6f77 223e 0a20 2020 2020 2020 2020 2020  ow">.           
 000072d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000072e0: 2020 2020 3c64 6976 2063 6c61 7373 3d22      <div class="
-000072f0: 7b25 2062 6c6f 636b 2031 5f6d 6964 5f62  {% block 1_mid_b
-00007300: 6f74 746f 6d5f 6163 5f63 2025 7d63 6f6c  ottom_ac_c %}col
-00007310: 2d31 3220 636f 6c2d 6d64 2d36 7b25 2065  -12 col-md-6{% e
-00007320: 6e64 626c 6f63 6b20 257d 223e 7b7b 2031  ndblock %}">{{ 1
-00007330: 5f6d 6964 5f62 6f74 746f 6d5f 6320 7d7d  _mid_bottom_c }}
-00007340: 3c2f 6469 763e 0a20 2020 2020 2020 2020  </div>.         
-00007350: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007360: 2020 207b 2520 656c 6966 2031 5f6d 6964     {% elif 1_mid
-00007370: 5f62 6f74 746f 6d5f 6220 616e 6420 315f  _bottom_b and 1_
-00007380: 6d69 645f 626f 7474 6f6d 5f63 2025 7d0a  mid_bottom_c %}.
-00007390: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000073a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000073b0: 3c64 6976 2063 6c61 7373 3d22 7b25 2062  <div class="{% b
-000073c0: 6c6f 636b 2031 5f6d 6964 5f62 6f74 746f  lock 1_mid_botto
-000073d0: 6d5f 6263 5f62 2025 7d63 6f6c 2d31 3220  m_bc_b %}col-12 
-000073e0: 636f 6c2d 6d64 2d34 7b25 2065 6e64 626c  col-md-4{% endbl
-000073f0: 6f63 6b20 257d 223e 7b7b 2031 5f6d 6964  ock %}">{{ 1_mid
-00007400: 5f62 6f74 746f 6d5f 6220 7d7d 3c2f 6469  _bottom_b }}</di
-00007410: 763e 0a20 2020 2020 2020 2020 2020 2020  v>.             
-00007420: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007430: 2020 203c 6469 7620 636c 6173 733d 227b     <div class="{
-00007440: 2520 626c 6f63 6b20 315f 6d69 645f 626f  % block 1_mid_bo
-00007450: 7474 6f6d 5f62 635f 6320 257d 636f 6c2d  ttom_bc_c %}col-
-00007460: 3132 2063 6f6c 2d6d 642d 387b 2520 656e  12 col-md-8{% en
-00007470: 6462 6c6f 636b 2025 7d22 3e7b 7b20 315f  dblock %}">{{ 1_
-00007480: 6d69 645f 626f 7474 6f6d 5f63 207d 7d3c  mid_bottom_c }}<
-00007490: 2f64 6976 3e0a 2020 2020 2020 2020 2020  /div>.          
-000074a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000074b0: 2020 7b25 2065 6c73 6520 257d 0a20 2020    {% else %}.   
-000074c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000074d0: 2020 2020 2020 2020 2020 2020 203c 6469               <di
-000074e0: 7620 636c 6173 733d 2263 6f6c 2d31 3222  v class="col-12"
-000074f0: 3e7b 7b20 315f 6d69 645f 626f 7474 6f6d  >{{ 1_mid_bottom
-00007500: 5f61 207d 7d7b 7b20 315f 6d69 645f 626f  _a }}{{ 1_mid_bo
-00007510: 7474 6f6d 5f62 207d 7d7b 7b20 315f 6d69  ttom_b }}{{ 1_mi
-00007520: 645f 626f 7474 6f6d 5f63 207d 7d3c 2f64  d_bottom_c }}</d
-00007530: 6976 3e0a 2020 2020 2020 2020 2020 2020  iv>.            
-00007540: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007550: 7b25 2065 6e64 6966 2025 7d0a 2020 2020  {% endif %}.    
-00007560: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007570: 2020 2020 3c2f 6469 763e 0a20 2020 2020      </div>.     
-00007580: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-00007590: 2f64 6976 3e0a 2020 2020 2020 2020 2020  /div>.          
-000075a0: 2020 2020 2020 2020 2020 7b25 2065 6e64            {% end
-000075b0: 6966 2025 7d0a 0a20 2020 2020 2020 2020  if %}..         
-000075c0: 2020 2020 2020 2020 2020 203c 212d 2d20             <!-- 
-000075d0: 426c 6f63 6b73 2069 6e20 626f 7474 6f6d  Blocks in bottom
-000075e0: 2070 6f73 6974 696f 6e20 2d2d 3e0a 2020   position -->.  
-000075f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007600: 2020 7b25 2069 6620 315f 626f 7474 6f6d    {% if 1_bottom
-00007610: 5f61 206f 7220 315f 626f 7474 6f6d 5f62  _a or 1_bottom_b
-00007620: 206f 7220 315f 626f 7474 6f6d 5f63 2025   or 1_bottom_c %
-00007630: 7d0a 2020 2020 2020 2020 2020 2020 2020  }.              
-00007640: 2020 2020 2020 3c64 6976 2063 6c61 7373        <div class
-00007650: 3d22 636f 6c2d 3132 223e 0a20 2020 2020  ="col-12">.     
-00007660: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007670: 2020 203c 6469 7620 636c 6173 733d 2272     <div class="r
-00007680: 6f77 223e 0a20 2020 2020 2020 2020 2020  ow">.           
-00007690: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000076a0: 207b 2520 6966 2031 5f62 6f74 746f 6d5f   {% if 1_bottom_
-000076b0: 6120 616e 6420 315f 626f 7474 6f6d 5f62  a and 1_bottom_b
-000076c0: 2061 6e64 2031 5f62 6f74 746f 6d5f 6320   and 1_bottom_c 
-000076d0: 257d 0a20 2020 2020 2020 2020 2020 2020  %}.             
-000076e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000076f0: 2020 203c 6469 7620 636c 6173 733d 227b     <div class="{
-00007700: 2520 626c 6f63 6b20 315f 626f 7474 6f6d  % block 1_bottom
-00007710: 5f61 6263 5f61 2025 7d63 6f6c 2d31 3220  _abc_a %}col-12 
-00007720: 636f 6c2d 6d64 2d34 7b25 2065 6e64 626c  col-md-4{% endbl
-00007730: 6f63 6b20 257d 223e 7b7b 2031 5f62 6f74  ock %}">{{ 1_bot
-00007740: 746f 6d5f 6120 7d7d 3c2f 6469 763e 0a20  tom_a }}</div>. 
+000072e0: 207b 2520 6966 2031 5f6d 6964 5f62 6f74   {% if 1_mid_bot
+000072f0: 746f 6d5f 6120 616e 6420 315f 6d69 645f  tom_a and 1_mid_
+00007300: 626f 7474 6f6d 5f62 2061 6e64 2031 5f6d  bottom_b and 1_m
+00007310: 6964 5f62 6f74 746f 6d5f 6320 257d 0a20  id_bottom_c %}. 
+00007320: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007330: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+00007340: 6469 7620 636c 6173 733d 227b 2520 626c  div class="{% bl
+00007350: 6f63 6b20 315f 6d69 645f 626f 7474 6f6d  ock 1_mid_bottom
+00007360: 5f61 6263 5f61 2025 7d63 6f6c 2d31 3220  _abc_a %}col-12 
+00007370: 636f 6c2d 6d64 2d34 7b25 2065 6e64 626c  col-md-4{% endbl
+00007380: 6f63 6b20 257d 223e 7b7b 2031 5f6d 6964  ock %}">{{ 1_mid
+00007390: 5f62 6f74 746f 6d5f 6120 7d7d 3c2f 6469  _bottom_a }}</di
+000073a0: 763e 0a20 2020 2020 2020 2020 2020 2020  v>.             
+000073b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000073c0: 2020 203c 6469 7620 636c 6173 733d 227b     <div class="{
+000073d0: 2520 626c 6f63 6b20 315f 6d69 645f 626f  % block 1_mid_bo
+000073e0: 7474 6f6d 5f61 6263 5f62 2025 7d63 6f6c  ttom_abc_b %}col
+000073f0: 2d31 3220 636f 6c2d 6d64 2d34 7b25 2065  -12 col-md-4{% e
+00007400: 6e64 626c 6f63 6b20 257d 223e 7b7b 2031  ndblock %}">{{ 1
+00007410: 5f6d 6964 5f62 6f74 746f 6d5f 6220 7d7d  _mid_bottom_b }}
+00007420: 3c2f 6469 763e 0a20 2020 2020 2020 2020  </div>.         
+00007430: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007440: 2020 2020 2020 203c 6469 7620 636c 6173         <div clas
+00007450: 733d 227b 2520 626c 6f63 6b20 315f 6d69  s="{% block 1_mi
+00007460: 645f 626f 7474 6f6d 5f61 6263 5f63 2025  d_bottom_abc_c %
+00007470: 7d63 6f6c 2d31 3220 636f 6c2d 6d64 2d34  }col-12 col-md-4
+00007480: 7b25 2065 6e64 626c 6f63 6b20 257d 223e  {% endblock %}">
+00007490: 7b7b 2031 5f6d 6964 5f62 6f74 746f 6d5f  {{ 1_mid_bottom_
+000074a0: 6320 7d7d 3c2f 6469 763e 0a20 2020 2020  c }}</div>.     
+000074b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000074c0: 2020 2020 2020 207b 2520 656c 6966 2031         {% elif 1
+000074d0: 5f6d 6964 5f62 6f74 746f 6d5f 6120 616e  _mid_bottom_a an
+000074e0: 6420 315f 6d69 645f 626f 7474 6f6d 5f62  d 1_mid_bottom_b
+000074f0: 2025 7d0a 2020 2020 2020 2020 2020 2020   %}.            
+00007500: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007510: 2020 2020 3c64 6976 2063 6c61 7373 3d22      <div class="
+00007520: 7b25 2062 6c6f 636b 2031 5f6d 6964 5f62  {% block 1_mid_b
+00007530: 6f74 746f 6d5f 6162 5f61 2025 7d63 6f6c  ottom_ab_a %}col
+00007540: 2d31 3220 636f 6c2d 6d64 2d38 7b25 2065  -12 col-md-8{% e
+00007550: 6e64 626c 6f63 6b20 257d 223e 7b7b 2031  ndblock %}">{{ 1
+00007560: 5f6d 6964 5f62 6f74 746f 6d5f 6120 7d7d  _mid_bottom_a }}
+00007570: 3c2f 6469 763e 0a20 2020 2020 2020 2020  </div>.         
+00007580: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007590: 2020 2020 2020 203c 6469 7620 636c 6173         <div clas
+000075a0: 733d 227b 2520 626c 6f63 6b20 315f 6d69  s="{% block 1_mi
+000075b0: 645f 626f 7474 6f6d 5f61 625f 6220 257d  d_bottom_ab_b %}
+000075c0: 636f 6c2d 3132 2063 6f6c 2d6d 642d 347b  col-12 col-md-4{
+000075d0: 2520 656e 6462 6c6f 636b 2025 7d22 3e7b  % endblock %}">{
+000075e0: 7b20 315f 6d69 645f 626f 7474 6f6d 5f62  { 1_mid_bottom_b
+000075f0: 207d 7d3c 2f64 6976 3e0a 2020 2020 2020   }}</div>.      
+00007600: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007610: 2020 2020 2020 7b25 2065 6c69 6620 315f        {% elif 1_
+00007620: 6d69 645f 626f 7474 6f6d 5f61 2061 6e64  mid_bottom_a and
+00007630: 2031 5f6d 6964 5f62 6f74 746f 6d5f 6320   1_mid_bottom_c 
+00007640: 257d 0a20 2020 2020 2020 2020 2020 2020  %}.             
+00007650: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007660: 2020 203c 6469 7620 636c 6173 733d 227b     <div class="{
+00007670: 2520 626c 6f63 6b20 315f 6d69 645f 626f  % block 1_mid_bo
+00007680: 7474 6f6d 5f61 635f 6120 257d 636f 6c2d  ttom_ac_a %}col-
+00007690: 3132 2063 6f6c 2d6d 642d 367b 2520 656e  12 col-md-6{% en
+000076a0: 6462 6c6f 636b 2025 7d22 3e7b 7b20 315f  dblock %}">{{ 1_
+000076b0: 6d69 645f 626f 7474 6f6d 5f61 207d 7d3c  mid_bottom_a }}<
+000076c0: 2f64 6976 3e0a 2020 2020 2020 2020 2020  /div>.          
+000076d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000076e0: 2020 2020 2020 3c64 6976 2063 6c61 7373        <div class
+000076f0: 3d22 7b25 2062 6c6f 636b 2031 5f6d 6964  ="{% block 1_mid
+00007700: 5f62 6f74 746f 6d5f 6163 5f63 2025 7d63  _bottom_ac_c %}c
+00007710: 6f6c 2d31 3220 636f 6c2d 6d64 2d36 7b25  ol-12 col-md-6{%
+00007720: 2065 6e64 626c 6f63 6b20 257d 223e 7b7b   endblock %}">{{
+00007730: 2031 5f6d 6964 5f62 6f74 746f 6d5f 6320   1_mid_bottom_c 
+00007740: 7d7d 3c2f 6469 763e 0a20 2020 2020 2020  }}</div>.       
 00007750: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007760: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-00007770: 6469 7620 636c 6173 733d 227b 2520 626c  div class="{% bl
-00007780: 6f63 6b20 315f 626f 7474 6f6d 5f61 6263  ock 1_bottom_abc
-00007790: 5f62 2025 7d63 6f6c 2d31 3220 636f 6c2d  _b %}col-12 col-
-000077a0: 6d64 2d34 7b25 2065 6e64 626c 6f63 6b20  md-4{% endblock 
-000077b0: 257d 223e 7b7b 2031 5f62 6f74 746f 6d5f  %}">{{ 1_bottom_
-000077c0: 6220 7d7d 3c2f 6469 763e 0a20 2020 2020  b }}</div>.     
-000077d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000077e0: 2020 2020 2020 2020 2020 203c 6469 7620             <div 
-000077f0: 636c 6173 733d 227b 2520 626c 6f63 6b20  class="{% block 
-00007800: 315f 626f 7474 6f6d 5f61 6263 5f63 2025  1_bottom_abc_c %
-00007810: 7d63 6f6c 2d31 3220 636f 6c2d 6d64 2d34  }col-12 col-md-4
-00007820: 7b25 2065 6e64 626c 6f63 6b20 257d 223e  {% endblock %}">
-00007830: 7b7b 2031 5f62 6f74 746f 6d5f 6320 7d7d  {{ 1_bottom_c }}
-00007840: 3c2f 6469 763e 0a20 2020 2020 2020 2020  </div>.         
-00007850: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007860: 2020 207b 2520 656c 6966 2031 5f62 6f74     {% elif 1_bot
-00007870: 746f 6d5f 6120 616e 6420 315f 626f 7474  tom_a and 1_bott
-00007880: 6f6d 5f62 2025 7d0a 2020 2020 2020 2020  om_b %}.        
-00007890: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000078a0: 2020 2020 2020 2020 3c64 6976 2063 6c61          <div cla
-000078b0: 7373 3d22 7b25 2062 6c6f 636b 2031 5f62  ss="{% block 1_b
-000078c0: 6f74 746f 6d5f 6162 5f61 2025 7d63 6f6c  ottom_ab_a %}col
-000078d0: 2d31 3220 636f 6c2d 6d64 2d38 7b25 2065  -12 col-md-8{% e
-000078e0: 6e64 626c 6f63 6b20 257d 223e 7b7b 2031  ndblock %}">{{ 1
-000078f0: 5f62 6f74 746f 6d5f 6120 7d7d 3c2f 6469  _bottom_a }}</di
-00007900: 763e 0a20 2020 2020 2020 2020 2020 2020  v>.             
-00007910: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007920: 2020 203c 6469 7620 636c 6173 733d 227b     <div class="{
-00007930: 2520 626c 6f63 6b20 315f 626f 7474 6f6d  % block 1_bottom
-00007940: 5f61 625f 6220 257d 636f 6c2d 3132 2063  _ab_b %}col-12 c
-00007950: 6f6c 2d6d 642d 347b 2520 656e 6462 6c6f  ol-md-4{% endblo
-00007960: 636b 2025 7d22 3e7b 7b20 315f 626f 7474  ck %}">{{ 1_bott
-00007970: 6f6d 5f62 207d 7d3c 2f64 6976 3e0a 2020  om_b }}</div>.  
+00007760: 2020 2020 207b 2520 656c 6966 2031 5f6d       {% elif 1_m
+00007770: 6964 5f62 6f74 746f 6d5f 6220 616e 6420  id_bottom_b and 
+00007780: 315f 6d69 645f 626f 7474 6f6d 5f63 2025  1_mid_bottom_c %
+00007790: 7d0a 2020 2020 2020 2020 2020 2020 2020  }.              
+000077a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000077b0: 2020 3c64 6976 2063 6c61 7373 3d22 7b25    <div class="{%
+000077c0: 2062 6c6f 636b 2031 5f6d 6964 5f62 6f74   block 1_mid_bot
+000077d0: 746f 6d5f 6263 5f62 2025 7d63 6f6c 2d31  tom_bc_b %}col-1
+000077e0: 3220 636f 6c2d 6d64 2d34 7b25 2065 6e64  2 col-md-4{% end
+000077f0: 626c 6f63 6b20 257d 223e 7b7b 2031 5f6d  block %}">{{ 1_m
+00007800: 6964 5f62 6f74 746f 6d5f 6220 7d7d 3c2f  id_bottom_b }}</
+00007810: 6469 763e 0a20 2020 2020 2020 2020 2020  div>.           
+00007820: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007830: 2020 2020 203c 6469 7620 636c 6173 733d       <div class=
+00007840: 227b 2520 626c 6f63 6b20 315f 6d69 645f  "{% block 1_mid_
+00007850: 626f 7474 6f6d 5f62 635f 6320 257d 636f  bottom_bc_c %}co
+00007860: 6c2d 3132 2063 6f6c 2d6d 642d 387b 2520  l-12 col-md-8{% 
+00007870: 656e 6462 6c6f 636b 2025 7d22 3e7b 7b20  endblock %}">{{ 
+00007880: 315f 6d69 645f 626f 7474 6f6d 5f63 207d  1_mid_bottom_c }
+00007890: 7d3c 2f64 6976 3e0a 2020 2020 2020 2020  }</div>.        
+000078a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000078b0: 2020 2020 7b25 2065 6c73 6520 257d 0a20      {% else %}. 
+000078c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000078d0: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+000078e0: 6469 7620 636c 6173 733d 2263 6f6c 2d31  div class="col-1
+000078f0: 3222 3e7b 7b20 315f 6d69 645f 626f 7474  2">{{ 1_mid_bott
+00007900: 6f6d 5f61 207d 7d7b 7b20 315f 6d69 645f  om_a }}{{ 1_mid_
+00007910: 626f 7474 6f6d 5f62 207d 7d7b 7b20 315f  bottom_b }}{{ 1_
+00007920: 6d69 645f 626f 7474 6f6d 5f63 207d 7d3c  mid_bottom_c }}<
+00007930: 2f64 6976 3e0a 2020 2020 2020 2020 2020  /div>.          
+00007940: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007950: 2020 7b25 2065 6e64 6966 2025 7d0a 2020    {% endif %}.  
+00007960: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007970: 2020 2020 2020 3c2f 6469 763e 0a20 2020        </div>.   
 00007980: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007990: 2020 2020 2020 2020 2020 7b25 2065 6c69            {% eli
-000079a0: 6620 315f 626f 7474 6f6d 5f61 2061 6e64  f 1_bottom_a and
-000079b0: 2031 5f62 6f74 746f 6d5f 6320 257d 0a20   1_bottom_c %}. 
-000079c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000079d0: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-000079e0: 6469 7620 636c 6173 733d 227b 2520 626c  div class="{% bl
-000079f0: 6f63 6b20 315f 626f 7474 6f6d 5f61 635f  ock 1_bottom_ac_
-00007a00: 6120 257d 636f 6c2d 3132 2063 6f6c 2d6d  a %}col-12 col-m
-00007a10: 642d 367b 2520 656e 6462 6c6f 636b 2025  d-6{% endblock %
-00007a20: 7d22 3e7b 7b20 315f 626f 7474 6f6d 5f61  }">{{ 1_bottom_a
-00007a30: 207d 7d3c 2f64 6976 3e0a 2020 2020 2020   }}</div>.      
-00007a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007a50: 2020 2020 2020 2020 2020 3c64 6976 2063            <div c
-00007a60: 6c61 7373 3d22 7b25 2062 6c6f 636b 2031  lass="{% block 1
-00007a70: 5f62 6f74 746f 6d5f 6163 5f63 2025 7d63  _bottom_ac_c %}c
-00007a80: 6f6c 2d31 3220 636f 6c2d 6d64 2d36 7b25  ol-12 col-md-6{%
-00007a90: 2065 6e64 626c 6f63 6b20 257d 223e 7b7b   endblock %}">{{
-00007aa0: 2031 5f62 6f74 746f 6d5f 6320 7d7d 3c2f   1_bottom_c }}</
-00007ab0: 6469 763e 0a20 2020 2020 2020 2020 2020  div>.           
-00007ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007ad0: 207b 2520 656c 6966 2031 5f62 6f74 746f   {% elif 1_botto
-00007ae0: 6d5f 6220 616e 6420 315f 626f 7474 6f6d  m_b and 1_bottom
-00007af0: 5f63 2025 7d0a 2020 2020 2020 2020 2020  _c %}.          
-00007b00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007b10: 2020 2020 2020 3c64 6976 2063 6c61 7373        <div class
-00007b20: 3d22 7b25 2062 6c6f 636b 2031 5f62 6f74  ="{% block 1_bot
-00007b30: 746f 6d5f 6263 5f62 2025 7d63 6f6c 2d31  tom_bc_b %}col-1
-00007b40: 3220 636f 6c2d 6d64 2d34 7b25 2065 6e64  2 col-md-4{% end
-00007b50: 626c 6f63 6b20 257d 223e 7b7b 2031 5f62  block %}">{{ 1_b
-00007b60: 6f74 746f 6d5f 6220 7d7d 3c2f 6469 763e  ottom_b }}</div>
-00007b70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00007b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007b90: 203c 6469 7620 636c 6173 733d 227b 2520   <div class="{% 
-00007ba0: 626c 6f63 6b20 315f 626f 7474 6f6d 5f62  block 1_bottom_b
-00007bb0: 635f 6320 257d 636f 6c2d 3132 2063 6f6c  c_c %}col-12 col
-00007bc0: 2d6d 642d 387b 2520 656e 6462 6c6f 636b  -md-8{% endblock
-00007bd0: 2025 7d22 3e7b 7b20 315f 626f 7474 6f6d   %}">{{ 1_bottom
-00007be0: 5f63 207d 7d3c 2f64 6976 3e0a 2020 2020  _c }}</div>.    
-00007bf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007c00: 2020 2020 2020 2020 7b25 2065 6c73 6520          {% else 
-00007c10: 257d 0a20 2020 2020 2020 2020 2020 2020  %}.             
-00007c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007c30: 2020 203c 6469 7620 636c 6173 733d 2263     <div class="c
-00007c40: 6f6c 2d31 3222 3e7b 7b20 315f 626f 7474  ol-12">{{ 1_bott
-00007c50: 6f6d 5f61 207d 7d7b 7b20 315f 626f 7474  om_a }}{{ 1_bott
-00007c60: 6f6d 5f62 207d 7d7b 7b20 315f 626f 7474  om_b }}{{ 1_bott
-00007c70: 6f6d 5f63 207d 7d3c 2f64 6976 3e0a 2020  om_c }}</div>.  
-00007c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007c90: 2020 2020 2020 2020 2020 7b25 2065 6e64            {% end
-00007ca0: 6966 2025 7d0a 2020 2020 2020 2020 2020  if %}.          
-00007cb0: 2020 2020 2020 2020 2020 2020 2020 3c2f                </
-00007cc0: 6469 763e 0a20 2020 2020 2020 2020 2020  div>.           
-00007cd0: 2020 2020 2020 2020 203c 2f64 6976 3e0a           </div>.
-00007ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007cf0: 2020 2020 7b25 2065 6e64 6966 2025 7d0a      {% endif %}.
-00007d00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00007d10: 203c 2f64 6976 3e0a 2020 2020 2020 2020   </div>.        
-00007d20: 2020 2020 3c2f 6469 763e 0a20 2020 2020      </div>.     
-00007d30: 2020 203c 2f64 6976 3e0a 2020 2020 7b25     </div>.    {%
-00007d40: 2065 6e64 6966 2025 7d0a 2020 2020 7b25   endif %}.    {%
-00007d50: 2065 6e64 626c 6f63 6b20 7365 6374 696f   endblock sectio
-00007d60: 6e5f 3120 257d 0a20 2020 203c 212d 2d20  n_1 %}.    <!-- 
-00007d70: 656e 6420 5365 6374 696f 6e20 3120 2d2d  end Section 1 --
-00007d80: 3e0a 0a20 2020 203c 212d 2d2d 2d2d 2d2d  >..    <!-------
-00007d90: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00007da0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00007db0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00007dc0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 3e0a  -------------->.
-00007dd0: 0a20 2020 203c 212d 2d20 5365 6374 696f  .    <!-- Sectio
-00007de0: 6e20 3220 2d2d 3e0a 2020 2020 7b25 2062  n 2 -->.    {% b
-00007df0: 6c6f 636b 2073 6563 7469 6f6e 5f32 2025  lock section_2 %
-00007e00: 7d0a 2020 2020 7b25 2062 6c6f 636b 735f  }.    {% blocks_
-00007e10: 696e 5f70 6f73 6974 696f 6e20 7365 6374  in_position sect
-00007e20: 696f 6e3d 2273 6563 7469 6f6e 2d32 2220  ion="section-2" 
-00007e30: 6173 2073 6563 7469 6f6e 5f32 2025 7d0a  as section_2 %}.
-00007e40: 2020 2020 7b25 2069 6620 7365 6374 696f      {% if sectio
-00007e50: 6e5f 3220 257d 0a20 2020 2020 2020 207b  n_2 %}.        {
-00007e60: 2520 6c6f 6164 5f62 6c6f 636b 7320 7365  % load_blocks se
-00007e70: 6374 696f 6e3d 2232 2d74 6f70 2d61 2220  ction="2-top-a" 
-00007e80: 6173 2032 5f74 6f70 5f61 2025 7d0a 2020  as 2_top_a %}.  
-00007e90: 2020 2020 2020 7b25 206c 6f61 645f 626c        {% load_bl
-00007ea0: 6f63 6b73 2073 6563 7469 6f6e 3d22 322d  ocks section="2-
-00007eb0: 746f 702d 6222 2061 7320 325f 746f 705f  top-b" as 2_top_
-00007ec0: 6220 257d 0a20 2020 2020 2020 207b 2520  b %}.        {% 
-00007ed0: 6c6f 6164 5f62 6c6f 636b 7320 7365 6374  load_blocks sect
-00007ee0: 696f 6e3d 2232 2d74 6f70 2d63 2220 6173  ion="2-top-c" as
-00007ef0: 2032 5f74 6f70 5f63 2025 7d0a 0a20 2020   2_top_c %}..   
-00007f00: 2020 2020 207b 2520 6c6f 6164 5f62 6c6f       {% load_blo
-00007f10: 636b 7320 7365 6374 696f 6e3d 2232 2d6d  cks section="2-m
-00007f20: 6964 2d74 6f70 2d61 2220 6173 2032 5f6d  id-top-a" as 2_m
-00007f30: 6964 5f74 6f70 5f61 2025 7d0a 2020 2020  id_top_a %}.    
-00007f40: 2020 2020 7b25 206c 6f61 645f 626c 6f63      {% load_bloc
-00007f50: 6b73 2073 6563 7469 6f6e 3d22 322d 6d69  ks section="2-mi
-00007f60: 642d 746f 702d 6222 2061 7320 325f 6d69  d-top-b" as 2_mi
-00007f70: 645f 746f 705f 6220 257d 0a20 2020 2020  d_top_b %}.     
-00007f80: 2020 207b 2520 6c6f 6164 5f62 6c6f 636b     {% load_block
-00007f90: 7320 7365 6374 696f 6e3d 2232 2d6d 6964  s section="2-mid
-00007fa0: 2d74 6f70 2d63 2220 6173 2032 5f6d 6964  -top-c" as 2_mid
-00007fb0: 5f74 6f70 5f63 2025 7d0a 0a20 2020 2020  _top_c %}..     
-00007fc0: 2020 207b 2520 6c6f 6164 5f62 6c6f 636b     {% load_block
-00007fd0: 7320 7365 6374 696f 6e3d 2232 2d6c 6566  s section="2-lef
-00007fe0: 742d 6122 2061 7320 325f 6c65 6674 5f61  t-a" as 2_left_a
-00007ff0: 2025 7d0a 2020 2020 2020 2020 7b25 206c   %}.        {% l
-00008000: 6f61 645f 626c 6f63 6b73 2073 6563 7469  oad_blocks secti
-00008010: 6f6e 3d22 322d 6c65 6674 2d62 2220 6173  on="2-left-b" as
-00008020: 2032 5f6c 6566 745f 6220 257d 0a0a 2020   2_left_b %}..  
-00008030: 2020 2020 2020 7b25 206c 6f61 645f 626c        {% load_bl
-00008040: 6f63 6b73 2073 6563 7469 6f6e 3d22 322d  ocks section="2-
-00008050: 6365 6e74 6572 2d74 6f70 2d61 2220 6173  center-top-a" as
-00008060: 2032 5f63 656e 7465 725f 746f 705f 6120   2_center_top_a 
-00008070: 257d 0a20 2020 2020 2020 207b 2520 6c6f  %}.        {% lo
-00008080: 6164 5f62 6c6f 636b 7320 7365 6374 696f  ad_blocks sectio
-00008090: 6e3d 2232 2d63 656e 7465 722d 746f 702d  n="2-center-top-
-000080a0: 6222 2061 7320 325f 6365 6e74 6572 5f74  b" as 2_center_t
-000080b0: 6f70 5f62 2025 7d0a 2020 2020 2020 2020  op_b %}.        
-000080c0: 7b25 206c 6f61 645f 626c 6f63 6b73 2073  {% load_blocks s
-000080d0: 6563 7469 6f6e 3d22 322d 6365 6e74 6572  ection="2-center
-000080e0: 2d74 6f70 2d63 2220 6173 2032 5f63 656e  -top-c" as 2_cen
-000080f0: 7465 725f 746f 705f 6320 257d 0a0a 2020  ter_top_c %}..  
-00008100: 2020 2020 2020 7b25 206c 6f61 645f 626c        {% load_bl
-00008110: 6f63 6b73 2073 6563 7469 6f6e 3d22 322d  ocks section="2-
-00008120: 6365 6e74 6572 2d6d 6964 2d74 6f70 2d61  center-mid-top-a
-00008130: 2220 6173 2032 5f63 656e 7465 725f 6d69  " as 2_center_mi
-00008140: 645f 746f 705f 6120 257d 0a20 2020 2020  d_top_a %}.     
-00008150: 2020 207b 2520 6c6f 6164 5f62 6c6f 636b     {% load_block
-00008160: 7320 7365 6374 696f 6e3d 2232 2d63 656e  s section="2-cen
-00008170: 7465 722d 6d69 642d 746f 702d 6222 2061  ter-mid-top-b" a
-00008180: 7320 325f 6365 6e74 6572 5f6d 6964 5f74  s 2_center_mid_t
-00008190: 6f70 5f62 2025 7d0a 2020 2020 2020 2020  op_b %}.        
-000081a0: 7b25 206c 6f61 645f 626c 6f63 6b73 2073  {% load_blocks s
-000081b0: 6563 7469 6f6e 3d22 322d 6365 6e74 6572  ection="2-center
-000081c0: 2d6d 6964 2d74 6f70 2d63 2220 6173 2032  -mid-top-c" as 2
-000081d0: 5f63 656e 7465 725f 6d69 645f 746f 705f  _center_mid_top_
-000081e0: 6320 257d 0a0a 2020 2020 2020 2020 7b25  c %}..        {%
-000081f0: 206c 6f61 645f 626c 6f63 6b73 2073 6563   load_blocks sec
-00008200: 7469 6f6e 3d22 322d 6365 6e74 6572 2d63  tion="2-center-c
-00008210: 6f6e 7465 6e74 2220 6173 2032 5f63 656e  ontent" as 2_cen
-00008220: 7465 725f 636f 6e74 656e 7420 257d 0a0a  ter_content %}..
-00008230: 2020 2020 2020 2020 7b25 206c 6f61 645f          {% load_
-00008240: 626c 6f63 6b73 2073 6563 7469 6f6e 3d22  blocks section="
-00008250: 322d 6365 6e74 6572 2d6d 6964 2d62 6f74  2-center-mid-bot
-00008260: 746f 6d2d 6122 2061 7320 325f 6365 6e74  tom-a" as 2_cent
-00008270: 6572 5f6d 6964 5f62 6f74 746f 6d5f 6120  er_mid_bottom_a 
-00008280: 257d 0a20 2020 2020 2020 207b 2520 6c6f  %}.        {% lo
-00008290: 6164 5f62 6c6f 636b 7320 7365 6374 696f  ad_blocks sectio
-000082a0: 6e3d 2232 2d63 656e 7465 722d 6d69 642d  n="2-center-mid-
-000082b0: 626f 7474 6f6d 2d62 2220 6173 2032 5f63  bottom-b" as 2_c
-000082c0: 656e 7465 725f 6d69 645f 626f 7474 6f6d  enter_mid_bottom
-000082d0: 5f62 2025 7d0a 2020 2020 2020 2020 7b25  _b %}.        {%
-000082e0: 206c 6f61 645f 626c 6f63 6b73 2073 6563   load_blocks sec
-000082f0: 7469 6f6e 3d22 322d 6365 6e74 6572 2d6d  tion="2-center-m
-00008300: 6964 2d62 6f74 746f 6d2d 6322 2061 7320  id-bottom-c" as 
-00008310: 325f 6365 6e74 6572 5f6d 6964 5f62 6f74  2_center_mid_bot
-00008320: 746f 6d5f 6320 257d 0a0a 2020 2020 2020  tom_c %}..      
-00008330: 2020 7b25 206c 6f61 645f 626c 6f63 6b73    {% load_blocks
-00008340: 2073 6563 7469 6f6e 3d22 322d 6365 6e74   section="2-cent
-00008350: 6572 2d62 6f74 746f 6d2d 6122 2061 7320  er-bottom-a" as 
-00008360: 325f 6365 6e74 6572 5f62 6f74 746f 6d5f  2_center_bottom_
-00008370: 6120 257d 0a20 2020 2020 2020 207b 2520  a %}.        {% 
-00008380: 6c6f 6164 5f62 6c6f 636b 7320 7365 6374  load_blocks sect
-00008390: 696f 6e3d 2232 2d63 656e 7465 722d 626f  ion="2-center-bo
-000083a0: 7474 6f6d 2d62 2220 6173 2032 5f63 656e  ttom-b" as 2_cen
-000083b0: 7465 725f 626f 7474 6f6d 5f62 2025 7d0a  ter_bottom_b %}.
-000083c0: 2020 2020 2020 2020 7b25 206c 6f61 645f          {% load_
-000083d0: 626c 6f63 6b73 2073 6563 7469 6f6e 3d22  blocks section="
-000083e0: 322d 6365 6e74 6572 2d62 6f74 746f 6d2d  2-center-bottom-
-000083f0: 6322 2061 7320 325f 6365 6e74 6572 5f62  c" as 2_center_b
-00008400: 6f74 746f 6d5f 6320 257d 0a0a 2020 2020  ottom_c %}..    
-00008410: 2020 2020 7b25 206c 6f61 645f 626c 6f63      {% load_bloc
-00008420: 6b73 2073 6563 7469 6f6e 3d22 322d 7269  ks section="2-ri
-00008430: 6768 742d 6122 2061 7320 325f 7269 6768  ght-a" as 2_righ
-00008440: 745f 6120 257d 0a20 2020 2020 2020 207b  t_a %}.        {
-00008450: 2520 6c6f 6164 5f62 6c6f 636b 7320 7365  % load_blocks se
-00008460: 6374 696f 6e3d 2232 2d72 6967 6874 2d62  ction="2-right-b
-00008470: 2220 6173 2032 5f72 6967 6874 5f62 2025  " as 2_right_b %
-00008480: 7d0a 0a20 2020 2020 2020 207b 2520 6c6f  }..        {% lo
-00008490: 6164 5f62 6c6f 636b 7320 7365 6374 696f  ad_blocks sectio
-000084a0: 6e3d 2232 2d6d 6964 2d62 6f74 746f 6d2d  n="2-mid-bottom-
-000084b0: 6122 2061 7320 325f 6d69 645f 626f 7474  a" as 2_mid_bott
-000084c0: 6f6d 5f61 2025 7d0a 2020 2020 2020 2020  om_a %}.        
-000084d0: 7b25 206c 6f61 645f 626c 6f63 6b73 2073  {% load_blocks s
-000084e0: 6563 7469 6f6e 3d22 322d 6d69 642d 626f  ection="2-mid-bo
-000084f0: 7474 6f6d 2d62 2220 6173 2032 5f6d 6964  ttom-b" as 2_mid
-00008500: 5f62 6f74 746f 6d5f 6220 257d 0a20 2020  _bottom_b %}.   
-00008510: 2020 2020 207b 2520 6c6f 6164 5f62 6c6f       {% load_blo
-00008520: 636b 7320 7365 6374 696f 6e3d 2232 2d6d  cks section="2-m
-00008530: 6964 2d62 6f74 746f 6d2d 6322 2061 7320  id-bottom-c" as 
-00008540: 325f 6d69 645f 626f 7474 6f6d 5f63 2025  2_mid_bottom_c %
-00008550: 7d0a 0a20 2020 2020 2020 207b 2520 6c6f  }..        {% lo
-00008560: 6164 5f62 6c6f 636b 7320 7365 6374 696f  ad_blocks sectio
-00008570: 6e3d 2232 2d62 6f74 746f 6d2d 6122 2061  n="2-bottom-a" a
-00008580: 7320 325f 626f 7474 6f6d 5f61 2025 7d0a  s 2_bottom_a %}.
-00008590: 2020 2020 2020 2020 7b25 206c 6f61 645f          {% load_
-000085a0: 626c 6f63 6b73 2073 6563 7469 6f6e 3d22  blocks section="
-000085b0: 322d 626f 7474 6f6d 2d62 2220 6173 2032  2-bottom-b" as 2
-000085c0: 5f62 6f74 746f 6d5f 6220 257d 0a20 2020  _bottom_b %}.   
-000085d0: 2020 2020 207b 2520 6c6f 6164 5f62 6c6f       {% load_blo
-000085e0: 636b 7320 7365 6374 696f 6e3d 2232 2d62  cks section="2-b
-000085f0: 6f74 746f 6d2d 6322 2061 7320 325f 626f  ottom-c" as 2_bo
-00008600: 7474 6f6d 5f63 2025 7d0a 0a20 2020 2020  ttom_c %}..     
-00008610: 2020 203c 6469 7620 636c 6173 733d 227b     <div class="{
-00008620: 2520 626c 6f63 6b20 7365 6374 696f 6e5f  % block section_
-00008630: 325f 636c 6173 7365 7320 257d 7079 2d35  2_classes %}py-5
-00008640: 206e 6575 7472 616c 2d32 2d62 677b 2520   neutral-2-bg{% 
-00008650: 656e 6462 6c6f 636b 2025 7d22 3e0a 2020  endblock %}">.  
-00008660: 2020 2020 2020 2020 2020 3c64 6976 2063            <div c
-00008670: 6c61 7373 3d22 636f 6e74 6169 6e65 7222  lass="container"
-00008680: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
-00008690: 2020 3c64 6976 2063 6c61 7373 3d22 726f    <div class="ro
-000086a0: 7720 6d78 2d30 223e 0a0a 2020 2020 2020  w mx-0">..      
-000086b0: 2020 2020 2020 2020 2020 2020 2020 3c21                <!
-000086c0: 2d2d 2054 6f70 202d 2d3e 0a20 2020 2020  -- Top -->.     
-000086d0: 2020 2020 2020 2020 2020 2020 2020 207b                 {
-000086e0: 2520 6966 2032 5f74 6f70 5f61 206f 7220  % if 2_top_a or 
-000086f0: 325f 746f 705f 6220 6f72 2032 5f74 6f70  2_top_b or 2_top
-00008700: 5f63 2025 7d0a 2020 2020 2020 2020 2020  _c %}.          
-00008710: 2020 2020 2020 2020 2020 3c64 6976 2063            <div c
-00008720: 6c61 7373 3d22 636f 6c2d 3132 223e 0a20  lass="col-12">. 
-00008730: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008740: 2020 2020 2020 203c 6469 7620 636c 6173         <div clas
-00008750: 733d 2272 6f77 223e 0a20 2020 2020 2020  s="row">.       
-00008760: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008770: 2020 2020 207b 2520 6966 2032 5f74 6f70       {% if 2_top
-00008780: 5f61 2061 6e64 2032 5f74 6f70 5f62 2061  _a and 2_top_b a
-00008790: 6e64 2032 5f74 6f70 5f63 2025 7d0a 2020  nd 2_top_c %}.  
-000087a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000087b0: 2020 2020 2020 2020 2020 2020 2020 3c64                <d
-000087c0: 6976 2063 6c61 7373 3d22 7b25 2062 6c6f  iv class="{% blo
-000087d0: 636b 2032 5f74 6f70 5f61 6263 5f61 2025  ck 2_top_abc_a %
-000087e0: 7d63 6f6c 2d31 3220 636f 6c2d 6d64 2d34  }col-12 col-md-4
-000087f0: 7b25 2065 6e64 626c 6f63 6b20 257d 223e  {% endblock %}">
-00008800: 7b7b 2032 5f74 6f70 5f61 207d 7d3c 2f64  {{ 2_top_a }}</d
-00008810: 6976 3e0a 2020 2020 2020 2020 2020 2020  iv>.            
-00008820: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008830: 2020 2020 3c64 6976 2063 6c61 7373 3d22      <div class="
-00008840: 7b25 2062 6c6f 636b 2032 5f74 6f70 5f61  {% block 2_top_a
-00008850: 6263 5f62 2025 7d63 6f6c 2d31 3220 636f  bc_b %}col-12 co
-00008860: 6c2d 6d64 2d34 7b25 2065 6e64 626c 6f63  l-md-4{% endbloc
-00008870: 6b20 257d 223e 7b7b 2032 5f74 6f70 5f62  k %}">{{ 2_top_b
-00008880: 207d 7d3c 2f64 6976 3e0a 2020 2020 2020   }}</div>.      
-00008890: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000088a0: 2020 2020 2020 2020 2020 3c64 6976 2063            <div c
-000088b0: 6c61 7373 3d22 7b25 2062 6c6f 636b 2032  lass="{% block 2
-000088c0: 5f74 6f70 5f61 6263 5f63 2025 7d63 6f6c  _top_abc_c %}col
-000088d0: 2d31 3220 636f 6c2d 6d64 2d34 7b25 2065  -12 col-md-4{% e
-000088e0: 6e64 626c 6f63 6b20 257d 223e 7b7b 2032  ndblock %}">{{ 2
-000088f0: 5f74 6f70 5f63 207d 7d3c 2f64 6976 3e0a  _top_c }}</div>.
-00008900: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008910: 2020 2020 2020 2020 2020 2020 7b25 2065              {% e
-00008920: 6c69 6620 325f 746f 705f 6120 616e 6420  lif 2_top_a and 
-00008930: 325f 746f 705f 6220 257d 0a20 2020 2020  2_top_b %}.     
-00008940: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008950: 2020 2020 2020 2020 2020 203c 6469 7620             <div 
-00008960: 636c 6173 733d 227b 2520 626c 6f63 6b20  class="{% block 
-00008970: 325f 746f 705f 6162 5f61 2025 7d63 6f6c  2_top_ab_a %}col
-00008980: 2d31 3220 636f 6c2d 6d64 2d38 7b25 2065  -12 col-md-8{% e
-00008990: 6e64 626c 6f63 6b20 257d 223e 7b7b 2032  ndblock %}">{{ 2
-000089a0: 5f74 6f70 5f61 207d 7d3c 2f64 6976 3e0a  _top_a }}</div>.
-000089b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000089c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000089d0: 3c64 6976 2063 6c61 7373 3d22 7b25 2062  <div class="{% b
-000089e0: 6c6f 636b 2032 5f74 6f70 5f61 625f 6220  lock 2_top_ab_b 
-000089f0: 257d 636f 6c2d 3132 2063 6f6c 2d6d 642d  %}col-12 col-md-
-00008a00: 347b 2520 656e 6462 6c6f 636b 2025 7d22  4{% endblock %}"
-00008a10: 3e7b 7b20 325f 746f 705f 6220 7d7d 3c2f  >{{ 2_top_b }}</
-00008a20: 6469 763e 0a20 2020 2020 2020 2020 2020  div>.           
-00008a30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008a40: 207b 2520 656c 6966 2032 5f74 6f70 5f61   {% elif 2_top_a
-00008a50: 2061 6e64 2032 5f74 6f70 5f63 2025 7d0a   and 2_top_c %}.
-00008a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008a80: 3c64 6976 2063 6c61 7373 3d22 7b25 2062  <div class="{% b
-00008a90: 6c6f 636b 2032 5f74 6f70 5f61 635f 6120  lock 2_top_ac_a 
-00008aa0: 257d 636f 6c2d 3132 2063 6f6c 2d6d 642d  %}col-12 col-md-
-00008ab0: 367b 2520 656e 6462 6c6f 636b 2025 7d22  6{% endblock %}"
-00008ac0: 3e7b 7b20 325f 746f 705f 6120 7d7d 3c2f  >{{ 2_top_a }}</
-00008ad0: 6469 763e 0a20 2020 2020 2020 2020 2020  div>.           
-00008ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008af0: 2020 2020 203c 6469 7620 636c 6173 733d       <div class=
-00008b00: 227b 2520 626c 6f63 6b20 325f 746f 705f  "{% block 2_top_
-00008b10: 6163 5f63 2025 7d63 6f6c 2d31 3220 636f  ac_c %}col-12 co
-00008b20: 6c2d 6d64 2d36 7b25 2065 6e64 626c 6f63  l-md-6{% endbloc
-00008b30: 6b20 257d 223e 7b7b 2032 5f74 6f70 5f63  k %}">{{ 2_top_c
-00008b40: 207d 7d3c 2f64 6976 3e0a 2020 2020 2020   }}</div>.      
-00008b50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008b60: 2020 2020 2020 7b25 2065 6c69 6620 325f        {% elif 2_
-00008b70: 746f 705f 6220 616e 6420 325f 746f 705f  top_b and 2_top_
-00008b80: 6320 257d 0a20 2020 2020 2020 2020 2020  c %}.           
-00008b90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008ba0: 2020 2020 203c 6469 7620 636c 6173 733d       <div class=
-00008bb0: 227b 2520 626c 6f63 6b20 325f 746f 705f  "{% block 2_top_
-00008bc0: 6263 5f62 2025 7d63 6f6c 2d31 3220 636f  bc_b %}col-12 co
-00008bd0: 6c2d 6d64 2d34 7b25 2065 6e64 626c 6f63  l-md-4{% endbloc
-00008be0: 6b20 257d 223e 7b7b 2032 5f74 6f70 5f62  k %}">{{ 2_top_b
-00008bf0: 207d 7d3c 2f64 6976 3e0a 2020 2020 2020   }}</div>.      
-00008c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008c10: 2020 2020 2020 2020 2020 3c64 6976 2063            <div c
-00008c20: 6c61 7373 3d22 7b25 2062 6c6f 636b 2032  lass="{% block 2
-00008c30: 5f74 6f70 5f62 635f 6320 257d 636f 6c2d  _top_bc_c %}col-
-00008c40: 3132 2063 6f6c 2d6d 642d 387b 2520 656e  12 col-md-8{% en
-00008c50: 6462 6c6f 636b 2025 7d22 3e7b 7b20 325f  dblock %}">{{ 2_
-00008c60: 746f 705f 6320 7d7d 3c2f 6469 763e 0a20  top_c }}</div>. 
-00008c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008c80: 2020 2020 2020 2020 2020 207b 2520 656c             {% el
-00008c90: 7365 2025 7d0a 2020 2020 2020 2020 2020  se %}.          
-00008ca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008cb0: 2020 2020 2020 3c64 6976 2063 6c61 7373        <div class
-00008cc0: 3d22 636f 6c2d 3132 223e 7b7b 2032 5f74  ="col-12">{{ 2_t
-00008cd0: 6f70 5f61 207d 7d7b 7b20 325f 746f 705f  op_a }}{{ 2_top_
-00008ce0: 6220 7d7d 7b7b 2032 5f74 6f70 5f63 207d  b }}{{ 2_top_c }
-00008cf0: 7d3c 2f64 6976 3e0a 2020 2020 2020 2020  }</div>.        
-00008d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008d10: 2020 2020 7b25 2065 6e64 6966 2025 7d0a      {% endif %}.
-00008d20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008d30: 2020 2020 2020 2020 3c2f 6469 763e 0a20          </div>. 
+00007990: 203c 2f64 6976 3e0a 2020 2020 2020 2020   </div>.        
+000079a0: 2020 2020 2020 2020 2020 2020 7b25 2065              {% e
+000079b0: 6e64 6966 2025 7d0a 0a20 2020 2020 2020  ndif %}..       
+000079c0: 2020 2020 2020 2020 2020 2020 203c 212d               <!-
+000079d0: 2d20 426c 6f63 6b73 2069 6e20 626f 7474  - Blocks in bott
+000079e0: 6f6d 2070 6f73 6974 696f 6e20 2d2d 3e0a  om position -->.
+000079f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007a00: 2020 2020 7b25 2069 6620 315f 626f 7474      {% if 1_bott
+00007a10: 6f6d 5f61 206f 7220 315f 626f 7474 6f6d  om_a or 1_bottom
+00007a20: 5f62 206f 7220 315f 626f 7474 6f6d 5f63  _b or 1_bottom_c
+00007a30: 2025 7d0a 2020 2020 2020 2020 2020 2020   %}.            
+00007a40: 2020 2020 2020 2020 3c64 6976 2063 6c61          <div cla
+00007a50: 7373 3d22 636f 6c2d 3132 223e 0a20 2020  ss="col-12">.   
+00007a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007a70: 2020 2020 203c 6469 7620 636c 6173 733d       <div class=
+00007a80: 2272 6f77 223e 0a20 2020 2020 2020 2020  "row">.         
+00007a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007aa0: 2020 207b 2520 6966 2031 5f62 6f74 746f     {% if 1_botto
+00007ab0: 6d5f 6120 616e 6420 315f 626f 7474 6f6d  m_a and 1_bottom
+00007ac0: 5f62 2061 6e64 2031 5f62 6f74 746f 6d5f  _b and 1_bottom_
+00007ad0: 6320 257d 0a20 2020 2020 2020 2020 2020  c %}.           
+00007ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007af0: 2020 2020 203c 6469 7620 636c 6173 733d       <div class=
+00007b00: 227b 2520 626c 6f63 6b20 315f 626f 7474  "{% block 1_bott
+00007b10: 6f6d 5f61 6263 5f61 2025 7d63 6f6c 2d31  om_abc_a %}col-1
+00007b20: 3220 636f 6c2d 6d64 2d34 7b25 2065 6e64  2 col-md-4{% end
+00007b30: 626c 6f63 6b20 257d 223e 7b7b 2031 5f62  block %}">{{ 1_b
+00007b40: 6f74 746f 6d5f 6120 7d7d 3c2f 6469 763e  ottom_a }}</div>
+00007b50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00007b60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007b70: 203c 6469 7620 636c 6173 733d 227b 2520   <div class="{% 
+00007b80: 626c 6f63 6b20 315f 626f 7474 6f6d 5f61  block 1_bottom_a
+00007b90: 6263 5f62 2025 7d63 6f6c 2d31 3220 636f  bc_b %}col-12 co
+00007ba0: 6c2d 6d64 2d34 7b25 2065 6e64 626c 6f63  l-md-4{% endbloc
+00007bb0: 6b20 257d 223e 7b7b 2031 5f62 6f74 746f  k %}">{{ 1_botto
+00007bc0: 6d5f 6220 7d7d 3c2f 6469 763e 0a20 2020  m_b }}</div>.   
+00007bd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007be0: 2020 2020 2020 2020 2020 2020 203c 6469               <di
+00007bf0: 7620 636c 6173 733d 227b 2520 626c 6f63  v class="{% bloc
+00007c00: 6b20 315f 626f 7474 6f6d 5f61 6263 5f63  k 1_bottom_abc_c
+00007c10: 2025 7d63 6f6c 2d31 3220 636f 6c2d 6d64   %}col-12 col-md
+00007c20: 2d34 7b25 2065 6e64 626c 6f63 6b20 257d  -4{% endblock %}
+00007c30: 223e 7b7b 2031 5f62 6f74 746f 6d5f 6320  ">{{ 1_bottom_c 
+00007c40: 7d7d 3c2f 6469 763e 0a20 2020 2020 2020  }}</div>.       
+00007c50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007c60: 2020 2020 207b 2520 656c 6966 2031 5f62       {% elif 1_b
+00007c70: 6f74 746f 6d5f 6120 616e 6420 315f 626f  ottom_a and 1_bo
+00007c80: 7474 6f6d 5f62 2025 7d0a 2020 2020 2020  ttom_b %}.      
+00007c90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007ca0: 2020 2020 2020 2020 2020 3c64 6976 2063            <div c
+00007cb0: 6c61 7373 3d22 7b25 2062 6c6f 636b 2031  lass="{% block 1
+00007cc0: 5f62 6f74 746f 6d5f 6162 5f61 2025 7d63  _bottom_ab_a %}c
+00007cd0: 6f6c 2d31 3220 636f 6c2d 6d64 2d38 7b25  ol-12 col-md-8{%
+00007ce0: 2065 6e64 626c 6f63 6b20 257d 223e 7b7b   endblock %}">{{
+00007cf0: 2031 5f62 6f74 746f 6d5f 6120 7d7d 3c2f   1_bottom_a }}</
+00007d00: 6469 763e 0a20 2020 2020 2020 2020 2020  div>.           
+00007d10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007d20: 2020 2020 203c 6469 7620 636c 6173 733d       <div class=
+00007d30: 227b 2520 626c 6f63 6b20 315f 626f 7474  "{% block 1_bott
+00007d40: 6f6d 5f61 625f 6220 257d 636f 6c2d 3132  om_ab_b %}col-12
+00007d50: 2063 6f6c 2d6d 642d 347b 2520 656e 6462   col-md-4{% endb
+00007d60: 6c6f 636b 2025 7d22 3e7b 7b20 315f 626f  lock %}">{{ 1_bo
+00007d70: 7474 6f6d 5f62 207d 7d3c 2f64 6976 3e0a  ttom_b }}</div>.
+00007d80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007d90: 2020 2020 2020 2020 2020 2020 7b25 2065              {% e
+00007da0: 6c69 6620 315f 626f 7474 6f6d 5f61 2061  lif 1_bottom_a a
+00007db0: 6e64 2031 5f62 6f74 746f 6d5f 6320 257d  nd 1_bottom_c %}
+00007dc0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00007dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007de0: 203c 6469 7620 636c 6173 733d 227b 2520   <div class="{% 
+00007df0: 626c 6f63 6b20 315f 626f 7474 6f6d 5f61  block 1_bottom_a
+00007e00: 635f 6120 257d 636f 6c2d 3132 2063 6f6c  c_a %}col-12 col
+00007e10: 2d6d 642d 367b 2520 656e 6462 6c6f 636b  -md-6{% endblock
+00007e20: 2025 7d22 3e7b 7b20 315f 626f 7474 6f6d   %}">{{ 1_bottom
+00007e30: 5f61 207d 7d3c 2f64 6976 3e0a 2020 2020  _a }}</div>.    
+00007e40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007e50: 2020 2020 2020 2020 2020 2020 3c64 6976              <div
+00007e60: 2063 6c61 7373 3d22 7b25 2062 6c6f 636b   class="{% block
+00007e70: 2031 5f62 6f74 746f 6d5f 6163 5f63 2025   1_bottom_ac_c %
+00007e80: 7d63 6f6c 2d31 3220 636f 6c2d 6d64 2d36  }col-12 col-md-6
+00007e90: 7b25 2065 6e64 626c 6f63 6b20 257d 223e  {% endblock %}">
+00007ea0: 7b7b 2031 5f62 6f74 746f 6d5f 6320 7d7d  {{ 1_bottom_c }}
+00007eb0: 3c2f 6469 763e 0a20 2020 2020 2020 2020  </div>.         
+00007ec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007ed0: 2020 207b 2520 656c 6966 2031 5f62 6f74     {% elif 1_bot
+00007ee0: 746f 6d5f 6220 616e 6420 315f 626f 7474  tom_b and 1_bott
+00007ef0: 6f6d 5f63 2025 7d0a 2020 2020 2020 2020  om_c %}.        
+00007f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007f10: 2020 2020 2020 2020 3c64 6976 2063 6c61          <div cla
+00007f20: 7373 3d22 7b25 2062 6c6f 636b 2031 5f62  ss="{% block 1_b
+00007f30: 6f74 746f 6d5f 6263 5f62 2025 7d63 6f6c  ottom_bc_b %}col
+00007f40: 2d31 3220 636f 6c2d 6d64 2d34 7b25 2065  -12 col-md-4{% e
+00007f50: 6e64 626c 6f63 6b20 257d 223e 7b7b 2031  ndblock %}">{{ 1
+00007f60: 5f62 6f74 746f 6d5f 6220 7d7d 3c2f 6469  _bottom_b }}</di
+00007f70: 763e 0a20 2020 2020 2020 2020 2020 2020  v>.             
+00007f80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007f90: 2020 203c 6469 7620 636c 6173 733d 227b     <div class="{
+00007fa0: 2520 626c 6f63 6b20 315f 626f 7474 6f6d  % block 1_bottom
+00007fb0: 5f62 635f 6320 257d 636f 6c2d 3132 2063  _bc_c %}col-12 c
+00007fc0: 6f6c 2d6d 642d 387b 2520 656e 6462 6c6f  ol-md-8{% endblo
+00007fd0: 636b 2025 7d22 3e7b 7b20 315f 626f 7474  ck %}">{{ 1_bott
+00007fe0: 6f6d 5f63 207d 7d3c 2f64 6976 3e0a 2020  om_c }}</div>.  
+00007ff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008000: 2020 2020 2020 2020 2020 7b25 2065 6c73            {% els
+00008010: 6520 257d 0a20 2020 2020 2020 2020 2020  e %}.           
+00008020: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008030: 2020 2020 203c 6469 7620 636c 6173 733d       <div class=
+00008040: 2263 6f6c 2d31 3222 3e7b 7b20 315f 626f  "col-12">{{ 1_bo
+00008050: 7474 6f6d 5f61 207d 7d7b 7b20 315f 626f  ttom_a }}{{ 1_bo
+00008060: 7474 6f6d 5f62 207d 7d7b 7b20 315f 626f  ttom_b }}{{ 1_bo
+00008070: 7474 6f6d 5f63 207d 7d3c 2f64 6976 3e0a  ttom_c }}</div>.
+00008080: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008090: 2020 2020 2020 2020 2020 2020 7b25 2065              {% e
+000080a0: 6e64 6966 2025 7d0a 2020 2020 2020 2020  ndif %}.        
+000080b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000080c0: 3c2f 6469 763e 0a20 2020 2020 2020 2020  </div>.         
+000080d0: 2020 2020 2020 2020 2020 203c 2f64 6976             </div
+000080e0: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
+000080f0: 2020 2020 2020 7b25 2065 6e64 6966 2025        {% endif %
+00008100: 7d0a 0a20 2020 2020 2020 2020 2020 2020  }..             
+00008110: 2020 203c 2f64 6976 3e0a 2020 2020 2020     </div>.      
+00008120: 2020 2020 2020 3c2f 6469 763e 0a20 2020        </div>.   
+00008130: 2020 2020 203c 2f64 6976 3e0a 2020 2020       </div>.    
+00008140: 7b25 2065 6e64 6966 2025 7d0a 2020 2020  {% endif %}.    
+00008150: 7b25 2065 6e64 626c 6f63 6b20 7365 6374  {% endblock sect
+00008160: 696f 6e5f 3120 257d 0a20 2020 203c 212d  ion_1 %}.    <!-
+00008170: 2d20 656e 6420 5365 6374 696f 6e20 3120  - end Section 1 
+00008180: 2d2d 3e0a 0a20 2020 203c 212d 2d2d 2d2d  -->..    <!-----
+00008190: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000081a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000081b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000081c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000081d0: 3e0a 0a20 2020 203c 212d 2d20 5365 6374  >..    <!-- Sect
+000081e0: 696f 6e20 3220 2d2d 3e0a 2020 2020 7b25  ion 2 -->.    {%
+000081f0: 2062 6c6f 636b 2073 6563 7469 6f6e 5f32   block section_2
+00008200: 2025 7d0a 2020 2020 7b25 2062 6c6f 636b   %}.    {% block
+00008210: 735f 696e 5f70 6f73 6974 696f 6e20 7365  s_in_position se
+00008220: 6374 696f 6e3d 2273 6563 7469 6f6e 2d32  ction="section-2
+00008230: 2220 6173 2073 6563 7469 6f6e 5f32 2025  " as section_2 %
+00008240: 7d0a 2020 2020 7b25 2069 6620 7365 6374  }.    {% if sect
+00008250: 696f 6e5f 3220 257d 0a20 2020 2020 2020  ion_2 %}.       
+00008260: 207b 2520 6c6f 6164 5f62 6c6f 636b 7320   {% load_blocks 
+00008270: 7365 6374 696f 6e3d 2232 2d74 6f70 2d61  section="2-top-a
+00008280: 2220 6173 2032 5f74 6f70 5f61 2025 7d0a  " as 2_top_a %}.
+00008290: 2020 2020 2020 2020 7b25 206c 6f61 645f          {% load_
+000082a0: 626c 6f63 6b73 2073 6563 7469 6f6e 3d22  blocks section="
+000082b0: 322d 746f 702d 6222 2061 7320 325f 746f  2-top-b" as 2_to
+000082c0: 705f 6220 257d 0a20 2020 2020 2020 207b  p_b %}.        {
+000082d0: 2520 6c6f 6164 5f62 6c6f 636b 7320 7365  % load_blocks se
+000082e0: 6374 696f 6e3d 2232 2d74 6f70 2d63 2220  ction="2-top-c" 
+000082f0: 6173 2032 5f74 6f70 5f63 2025 7d0a 0a20  as 2_top_c %}.. 
+00008300: 2020 2020 2020 207b 2520 6c6f 6164 5f62         {% load_b
+00008310: 6c6f 636b 7320 7365 6374 696f 6e3d 2232  locks section="2
+00008320: 2d6d 6964 2d74 6f70 2d61 2220 6173 2032  -mid-top-a" as 2
+00008330: 5f6d 6964 5f74 6f70 5f61 2025 7d0a 2020  _mid_top_a %}.  
+00008340: 2020 2020 2020 7b25 206c 6f61 645f 626c        {% load_bl
+00008350: 6f63 6b73 2073 6563 7469 6f6e 3d22 322d  ocks section="2-
+00008360: 6d69 642d 746f 702d 6222 2061 7320 325f  mid-top-b" as 2_
+00008370: 6d69 645f 746f 705f 6220 257d 0a20 2020  mid_top_b %}.   
+00008380: 2020 2020 207b 2520 6c6f 6164 5f62 6c6f       {% load_blo
+00008390: 636b 7320 7365 6374 696f 6e3d 2232 2d6d  cks section="2-m
+000083a0: 6964 2d74 6f70 2d63 2220 6173 2032 5f6d  id-top-c" as 2_m
+000083b0: 6964 5f74 6f70 5f63 2025 7d0a 0a20 2020  id_top_c %}..   
+000083c0: 2020 2020 207b 2520 6c6f 6164 5f62 6c6f       {% load_blo
+000083d0: 636b 7320 7365 6374 696f 6e3d 2232 2d6c  cks section="2-l
+000083e0: 6566 742d 6122 2061 7320 325f 6c65 6674  eft-a" as 2_left
+000083f0: 5f61 2025 7d0a 2020 2020 2020 2020 7b25  _a %}.        {%
+00008400: 206c 6f61 645f 626c 6f63 6b73 2073 6563   load_blocks sec
+00008410: 7469 6f6e 3d22 322d 6c65 6674 2d62 2220  tion="2-left-b" 
+00008420: 6173 2032 5f6c 6566 745f 6220 257d 0a0a  as 2_left_b %}..
+00008430: 2020 2020 2020 2020 7b25 206c 6f61 645f          {% load_
+00008440: 626c 6f63 6b73 2073 6563 7469 6f6e 3d22  blocks section="
+00008450: 322d 6365 6e74 6572 2d74 6f70 2d61 2220  2-center-top-a" 
+00008460: 6173 2032 5f63 656e 7465 725f 746f 705f  as 2_center_top_
+00008470: 6120 257d 0a20 2020 2020 2020 207b 2520  a %}.        {% 
+00008480: 6c6f 6164 5f62 6c6f 636b 7320 7365 6374  load_blocks sect
+00008490: 696f 6e3d 2232 2d63 656e 7465 722d 746f  ion="2-center-to
+000084a0: 702d 6222 2061 7320 325f 6365 6e74 6572  p-b" as 2_center
+000084b0: 5f74 6f70 5f62 2025 7d0a 2020 2020 2020  _top_b %}.      
+000084c0: 2020 7b25 206c 6f61 645f 626c 6f63 6b73    {% load_blocks
+000084d0: 2073 6563 7469 6f6e 3d22 322d 6365 6e74   section="2-cent
+000084e0: 6572 2d74 6f70 2d63 2220 6173 2032 5f63  er-top-c" as 2_c
+000084f0: 656e 7465 725f 746f 705f 6320 257d 0a0a  enter_top_c %}..
+00008500: 2020 2020 2020 2020 7b25 206c 6f61 645f          {% load_
+00008510: 626c 6f63 6b73 2073 6563 7469 6f6e 3d22  blocks section="
+00008520: 322d 6365 6e74 6572 2d6d 6964 2d74 6f70  2-center-mid-top
+00008530: 2d61 2220 6173 2032 5f63 656e 7465 725f  -a" as 2_center_
+00008540: 6d69 645f 746f 705f 6120 257d 0a20 2020  mid_top_a %}.   
+00008550: 2020 2020 207b 2520 6c6f 6164 5f62 6c6f       {% load_blo
+00008560: 636b 7320 7365 6374 696f 6e3d 2232 2d63  cks section="2-c
+00008570: 656e 7465 722d 6d69 642d 746f 702d 6222  enter-mid-top-b"
+00008580: 2061 7320 325f 6365 6e74 6572 5f6d 6964   as 2_center_mid
+00008590: 5f74 6f70 5f62 2025 7d0a 2020 2020 2020  _top_b %}.      
+000085a0: 2020 7b25 206c 6f61 645f 626c 6f63 6b73    {% load_blocks
+000085b0: 2073 6563 7469 6f6e 3d22 322d 6365 6e74   section="2-cent
+000085c0: 6572 2d6d 6964 2d74 6f70 2d63 2220 6173  er-mid-top-c" as
+000085d0: 2032 5f63 656e 7465 725f 6d69 645f 746f   2_center_mid_to
+000085e0: 705f 6320 257d 0a0a 2020 2020 2020 2020  p_c %}..        
+000085f0: 7b25 206c 6f61 645f 626c 6f63 6b73 2073  {% load_blocks s
+00008600: 6563 7469 6f6e 3d22 322d 6365 6e74 6572  ection="2-center
+00008610: 2d63 6f6e 7465 6e74 2220 6173 2032 5f63  -content" as 2_c
+00008620: 656e 7465 725f 636f 6e74 656e 7420 257d  enter_content %}
+00008630: 0a0a 2020 2020 2020 2020 7b25 206c 6f61  ..        {% loa
+00008640: 645f 626c 6f63 6b73 2073 6563 7469 6f6e  d_blocks section
+00008650: 3d22 322d 6365 6e74 6572 2d6d 6964 2d62  ="2-center-mid-b
+00008660: 6f74 746f 6d2d 6122 2061 7320 325f 6365  ottom-a" as 2_ce
+00008670: 6e74 6572 5f6d 6964 5f62 6f74 746f 6d5f  nter_mid_bottom_
+00008680: 6120 257d 0a20 2020 2020 2020 207b 2520  a %}.        {% 
+00008690: 6c6f 6164 5f62 6c6f 636b 7320 7365 6374  load_blocks sect
+000086a0: 696f 6e3d 2232 2d63 656e 7465 722d 6d69  ion="2-center-mi
+000086b0: 642d 626f 7474 6f6d 2d62 2220 6173 2032  d-bottom-b" as 2
+000086c0: 5f63 656e 7465 725f 6d69 645f 626f 7474  _center_mid_bott
+000086d0: 6f6d 5f62 2025 7d0a 2020 2020 2020 2020  om_b %}.        
+000086e0: 7b25 206c 6f61 645f 626c 6f63 6b73 2073  {% load_blocks s
+000086f0: 6563 7469 6f6e 3d22 322d 6365 6e74 6572  ection="2-center
+00008700: 2d6d 6964 2d62 6f74 746f 6d2d 6322 2061  -mid-bottom-c" a
+00008710: 7320 325f 6365 6e74 6572 5f6d 6964 5f62  s 2_center_mid_b
+00008720: 6f74 746f 6d5f 6320 257d 0a0a 2020 2020  ottom_c %}..    
+00008730: 2020 2020 7b25 206c 6f61 645f 626c 6f63      {% load_bloc
+00008740: 6b73 2073 6563 7469 6f6e 3d22 322d 6365  ks section="2-ce
+00008750: 6e74 6572 2d62 6f74 746f 6d2d 6122 2061  nter-bottom-a" a
+00008760: 7320 325f 6365 6e74 6572 5f62 6f74 746f  s 2_center_botto
+00008770: 6d5f 6120 257d 0a20 2020 2020 2020 207b  m_a %}.        {
+00008780: 2520 6c6f 6164 5f62 6c6f 636b 7320 7365  % load_blocks se
+00008790: 6374 696f 6e3d 2232 2d63 656e 7465 722d  ction="2-center-
+000087a0: 626f 7474 6f6d 2d62 2220 6173 2032 5f63  bottom-b" as 2_c
+000087b0: 656e 7465 725f 626f 7474 6f6d 5f62 2025  enter_bottom_b %
+000087c0: 7d0a 2020 2020 2020 2020 7b25 206c 6f61  }.        {% loa
+000087d0: 645f 626c 6f63 6b73 2073 6563 7469 6f6e  d_blocks section
+000087e0: 3d22 322d 6365 6e74 6572 2d62 6f74 746f  ="2-center-botto
+000087f0: 6d2d 6322 2061 7320 325f 6365 6e74 6572  m-c" as 2_center
+00008800: 5f62 6f74 746f 6d5f 6320 257d 0a0a 2020  _bottom_c %}..  
+00008810: 2020 2020 2020 7b25 206c 6f61 645f 626c        {% load_bl
+00008820: 6f63 6b73 2073 6563 7469 6f6e 3d22 322d  ocks section="2-
+00008830: 7269 6768 742d 6122 2061 7320 325f 7269  right-a" as 2_ri
+00008840: 6768 745f 6120 257d 0a20 2020 2020 2020  ght_a %}.       
+00008850: 207b 2520 6c6f 6164 5f62 6c6f 636b 7320   {% load_blocks 
+00008860: 7365 6374 696f 6e3d 2232 2d72 6967 6874  section="2-right
+00008870: 2d62 2220 6173 2032 5f72 6967 6874 5f62  -b" as 2_right_b
+00008880: 2025 7d0a 0a20 2020 2020 2020 207b 2520   %}..        {% 
+00008890: 6c6f 6164 5f62 6c6f 636b 7320 7365 6374  load_blocks sect
+000088a0: 696f 6e3d 2232 2d6d 6964 2d62 6f74 746f  ion="2-mid-botto
+000088b0: 6d2d 6122 2061 7320 325f 6d69 645f 626f  m-a" as 2_mid_bo
+000088c0: 7474 6f6d 5f61 2025 7d0a 2020 2020 2020  ttom_a %}.      
+000088d0: 2020 7b25 206c 6f61 645f 626c 6f63 6b73    {% load_blocks
+000088e0: 2073 6563 7469 6f6e 3d22 322d 6d69 642d   section="2-mid-
+000088f0: 626f 7474 6f6d 2d62 2220 6173 2032 5f6d  bottom-b" as 2_m
+00008900: 6964 5f62 6f74 746f 6d5f 6220 257d 0a20  id_bottom_b %}. 
+00008910: 2020 2020 2020 207b 2520 6c6f 6164 5f62         {% load_b
+00008920: 6c6f 636b 7320 7365 6374 696f 6e3d 2232  locks section="2
+00008930: 2d6d 6964 2d62 6f74 746f 6d2d 6322 2061  -mid-bottom-c" a
+00008940: 7320 325f 6d69 645f 626f 7474 6f6d 5f63  s 2_mid_bottom_c
+00008950: 2025 7d0a 0a20 2020 2020 2020 207b 2520   %}..        {% 
+00008960: 6c6f 6164 5f62 6c6f 636b 7320 7365 6374  load_blocks sect
+00008970: 696f 6e3d 2232 2d62 6f74 746f 6d2d 6122  ion="2-bottom-a"
+00008980: 2061 7320 325f 626f 7474 6f6d 5f61 2025   as 2_bottom_a %
+00008990: 7d0a 2020 2020 2020 2020 7b25 206c 6f61  }.        {% loa
+000089a0: 645f 626c 6f63 6b73 2073 6563 7469 6f6e  d_blocks section
+000089b0: 3d22 322d 626f 7474 6f6d 2d62 2220 6173  ="2-bottom-b" as
+000089c0: 2032 5f62 6f74 746f 6d5f 6220 257d 0a20   2_bottom_b %}. 
+000089d0: 2020 2020 2020 207b 2520 6c6f 6164 5f62         {% load_b
+000089e0: 6c6f 636b 7320 7365 6374 696f 6e3d 2232  locks section="2
+000089f0: 2d62 6f74 746f 6d2d 6322 2061 7320 325f  -bottom-c" as 2_
+00008a00: 626f 7474 6f6d 5f63 2025 7d0a 0a20 2020  bottom_c %}..   
+00008a10: 2020 2020 203c 6469 7620 636c 6173 733d       <div class=
+00008a20: 227b 2520 626c 6f63 6b20 7365 6374 696f  "{% block sectio
+00008a30: 6e5f 325f 636c 6173 7365 7320 257d 7079  n_2_classes %}py
+00008a40: 2d35 206e 6575 7472 616c 2d32 2d62 677b  -5 neutral-2-bg{
+00008a50: 2520 656e 6462 6c6f 636b 2025 7d22 3e0a  % endblock %}">.
+00008a60: 2020 2020 2020 2020 2020 2020 3c64 6976              <div
+00008a70: 2063 6c61 7373 3d22 636f 6e74 6169 6e65   class="containe
+00008a80: 7222 3e0a 2020 2020 2020 2020 2020 2020  r">.            
+00008a90: 2020 2020 3c64 6976 2063 6c61 7373 3d22      <div class="
+00008aa0: 726f 7720 6d78 2d30 223e 0a0a 2020 2020  row mx-0">..    
+00008ab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008ac0: 3c21 2d2d 2054 6f70 202d 2d3e 0a20 2020  <!-- Top -->.   
+00008ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008ae0: 207b 2520 6966 2032 5f74 6f70 5f61 206f   {% if 2_top_a o
+00008af0: 7220 325f 746f 705f 6220 6f72 2032 5f74  r 2_top_b or 2_t
+00008b00: 6f70 5f63 2025 7d0a 2020 2020 2020 2020  op_c %}.        
+00008b10: 2020 2020 2020 2020 2020 2020 3c64 6976              <div
+00008b20: 2063 6c61 7373 3d22 636f 6c2d 3132 223e   class="col-12">
+00008b30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00008b40: 2020 2020 2020 2020 203c 6469 7620 636c           <div cl
+00008b50: 6173 733d 2272 6f77 223e 0a20 2020 2020  ass="row">.     
+00008b60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008b70: 2020 2020 2020 207b 2520 6966 2032 5f74         {% if 2_t
+00008b80: 6f70 5f61 2061 6e64 2032 5f74 6f70 5f62  op_a and 2_top_b
+00008b90: 2061 6e64 2032 5f74 6f70 5f63 2025 7d0a   and 2_top_c %}.
+00008ba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008bb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008bc0: 3c64 6976 2063 6c61 7373 3d22 7b25 2062  <div class="{% b
+00008bd0: 6c6f 636b 2032 5f74 6f70 5f61 6263 5f61  lock 2_top_abc_a
+00008be0: 2025 7d63 6f6c 2d31 3220 636f 6c2d 6d64   %}col-12 col-md
+00008bf0: 2d34 7b25 2065 6e64 626c 6f63 6b20 257d  -4{% endblock %}
+00008c00: 223e 7b7b 2032 5f74 6f70 5f61 207d 7d3c  ">{{ 2_top_a }}<
+00008c10: 2f64 6976 3e0a 2020 2020 2020 2020 2020  /div>.          
+00008c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008c30: 2020 2020 2020 3c64 6976 2063 6c61 7373        <div class
+00008c40: 3d22 7b25 2062 6c6f 636b 2032 5f74 6f70  ="{% block 2_top
+00008c50: 5f61 6263 5f62 2025 7d63 6f6c 2d31 3220  _abc_b %}col-12 
+00008c60: 636f 6c2d 6d64 2d34 7b25 2065 6e64 626c  col-md-4{% endbl
+00008c70: 6f63 6b20 257d 223e 7b7b 2032 5f74 6f70  ock %}">{{ 2_top
+00008c80: 5f62 207d 7d3c 2f64 6976 3e0a 2020 2020  _b }}</div>.    
+00008c90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008ca0: 2020 2020 2020 2020 2020 2020 3c64 6976              <div
+00008cb0: 2063 6c61 7373 3d22 7b25 2062 6c6f 636b   class="{% block
+00008cc0: 2032 5f74 6f70 5f61 6263 5f63 2025 7d63   2_top_abc_c %}c
+00008cd0: 6f6c 2d31 3220 636f 6c2d 6d64 2d34 7b25  ol-12 col-md-4{%
+00008ce0: 2065 6e64 626c 6f63 6b20 257d 223e 7b7b   endblock %}">{{
+00008cf0: 2032 5f74 6f70 5f63 207d 7d3c 2f64 6976   2_top_c }}</div
+00008d00: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
+00008d10: 2020 2020 2020 2020 2020 2020 2020 7b25                {%
+00008d20: 2065 6c69 6620 325f 746f 705f 6120 616e   elif 2_top_a an
+00008d30: 6420 325f 746f 705f 6220 257d 0a20 2020  d 2_top_b %}.   
 00008d40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008d50: 2020 203c 2f64 6976 3e0a 2020 2020 2020     </div>.      
-00008d60: 2020 2020 2020 2020 2020 2020 2020 7b25                {%
-00008d70: 2065 6e64 6966 2025 7d0a 2020 2020 2020   endif %}.      
-00008d80: 2020 2020 2020 2020 2020 2020 2020 3c21                <!
-00008d90: 2d2d 2065 6e64 2054 6f70 202d 2d3e 0a0a  -- end Top -->..
-00008da0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008db0: 2020 2020 3c21 2d2d 204d 6964 646c 6520      <!-- Middle 
-00008dc0: 546f 7020 2d2d 3e0a 2020 2020 2020 2020  Top -->.        
-00008dd0: 2020 2020 2020 2020 2020 2020 7b25 2069              {% i
-00008de0: 6620 325f 6d69 645f 746f 705f 6120 6f72  f 2_mid_top_a or
-00008df0: 2032 5f6d 6964 5f74 6f70 5f62 206f 7220   2_mid_top_b or 
-00008e00: 325f 6d69 645f 746f 705f 6320 257d 0a20  2_mid_top_c %}. 
-00008e10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008e20: 2020 203c 6469 7620 636c 6173 733d 2263     <div class="c
-00008e30: 6f6c 2d31 3222 3e0a 2020 2020 2020 2020  ol-12">.        
-00008e40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008e50: 3c64 6976 2063 6c61 7373 3d22 726f 7722  <div class="row"
-00008e60: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
-00008e70: 2020 2020 2020 2020 2020 2020 2020 7b25                {%
-00008e80: 2069 6620 325f 6d69 645f 746f 705f 6120   if 2_mid_top_a 
-00008e90: 616e 6420 325f 6d69 645f 746f 705f 6220  and 2_mid_top_b 
-00008ea0: 616e 6420 325f 6d69 645f 746f 705f 6320  and 2_mid_top_c 
-00008eb0: 257d 0a20 2020 2020 2020 2020 2020 2020  %}.             
-00008ec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008ed0: 2020 203c 6469 7620 636c 6173 733d 227b     <div class="{
-00008ee0: 2520 626c 6f63 6b20 325f 6d69 645f 746f  % block 2_mid_to
-00008ef0: 705f 6162 635f 6120 257d 636f 6c2d 3132  p_abc_a %}col-12
-00008f00: 2063 6f6c 2d6d 642d 347b 2520 656e 6462   col-md-4{% endb
-00008f10: 6c6f 636b 2025 7d22 3e7b 7b20 325f 6d69  lock %}">{{ 2_mi
-00008f20: 645f 746f 705f 6120 7d7d 3c2f 6469 763e  d_top_a }}</div>
-00008f30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00008f40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008f50: 203c 6469 7620 636c 6173 733d 227b 2520   <div class="{% 
-00008f60: 626c 6f63 6b20 325f 6d69 645f 746f 705f  block 2_mid_top_
-00008f70: 6162 635f 6220 257d 636f 6c2d 3132 2063  abc_b %}col-12 c
-00008f80: 6f6c 2d6d 642d 347b 2520 656e 6462 6c6f  ol-md-4{% endblo
-00008f90: 636b 2025 7d22 3e7b 7b20 325f 6d69 645f  ck %}">{{ 2_mid_
-00008fa0: 746f 705f 6220 7d7d 3c2f 6469 763e 0a20  top_b }}</div>. 
-00008fb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008fc0: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-00008fd0: 6469 7620 636c 6173 733d 227b 2520 626c  div class="{% bl
-00008fe0: 6f63 6b20 325f 6d69 645f 746f 705f 6162  ock 2_mid_top_ab
-00008ff0: 635f 6320 257d 636f 6c2d 3132 2063 6f6c  c_c %}col-12 col
-00009000: 2d6d 642d 347b 2520 656e 6462 6c6f 636b  -md-4{% endblock
-00009010: 2025 7d22 3e7b 7b20 325f 6d69 645f 746f   %}">{{ 2_mid_to
-00009020: 705f 6320 7d7d 3c2f 6469 763e 0a20 2020  p_c }}</div>.   
-00009030: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009040: 2020 2020 2020 2020 207b 2520 656c 6966           {% elif
-00009050: 2032 5f6d 6964 5f74 6f70 5f61 2061 6e64   2_mid_top_a and
-00009060: 2032 5f6d 6964 5f74 6f70 5f62 2025 7d0a   2_mid_top_b %}.
-00009070: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009080: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009090: 3c64 6976 2063 6c61 7373 3d22 7b25 2062  <div class="{% b
-000090a0: 6c6f 636b 2032 5f6d 6964 5f74 6f70 5f61  lock 2_mid_top_a
-000090b0: 625f 6120 257d 636f 6c2d 3132 2063 6f6c  b_a %}col-12 col
-000090c0: 2d6d 642d 387b 2520 656e 6462 6c6f 636b  -md-8{% endblock
-000090d0: 2025 7d22 3e7b 7b20 325f 6d69 645f 746f   %}">{{ 2_mid_to
-000090e0: 705f 6120 7d7d 3c2f 6469 763e 0a20 2020  p_a }}</div>.   
-000090f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009100: 2020 2020 2020 2020 2020 2020 203c 6469               <di
-00009110: 7620 636c 6173 733d 227b 2520 626c 6f63  v class="{% bloc
-00009120: 6b20 325f 6d69 645f 746f 705f 6162 5f62  k 2_mid_top_ab_b
-00009130: 2025 7d63 6f6c 2d31 3220 636f 6c2d 6d64   %}col-12 col-md
-00009140: 2d34 7b25 2065 6e64 626c 6f63 6b20 257d  -4{% endblock %}
-00009150: 223e 7b7b 2032 5f6d 6964 5f74 6f70 5f62  ">{{ 2_mid_top_b
-00009160: 207d 7d3c 2f64 6976 3e0a 2020 2020 2020   }}</div>.      
-00009170: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009180: 2020 2020 2020 7b25 2065 6c69 6620 325f        {% elif 2_
-00009190: 6d69 645f 746f 705f 6120 616e 6420 325f  mid_top_a and 2_
-000091a0: 6d69 645f 746f 705f 6320 257d 0a20 2020  mid_top_c %}.   
-000091b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000091c0: 2020 2020 2020 2020 2020 2020 203c 6469               <di
-000091d0: 7620 636c 6173 733d 227b 2520 626c 6f63  v class="{% bloc
-000091e0: 6b20 325f 6d69 645f 746f 705f 6163 5f61  k 2_mid_top_ac_a
-000091f0: 2025 7d63 6f6c 2d31 3220 636f 6c2d 6d64   %}col-12 col-md
-00009200: 2d36 7b25 2065 6e64 626c 6f63 6b20 257d  -6{% endblock %}
-00009210: 223e 7b7b 2032 5f6d 6964 5f74 6f70 5f61  ">{{ 2_mid_top_a
-00009220: 207d 7d3c 2f64 6976 3e0a 2020 2020 2020   }}</div>.      
-00009230: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009240: 2020 2020 2020 2020 2020 3c64 6976 2063            <div c
-00009250: 6c61 7373 3d22 7b25 2062 6c6f 636b 2032  lass="{% block 2
-00009260: 5f6d 6964 5f74 6f70 5f61 635f 6320 257d  _mid_top_ac_c %}
-00009270: 636f 6c2d 3132 2063 6f6c 2d6d 642d 367b  col-12 col-md-6{
-00009280: 2520 656e 6462 6c6f 636b 2025 7d22 3e7b  % endblock %}">{
-00009290: 7b20 325f 6d69 645f 746f 705f 6320 7d7d  { 2_mid_top_c }}
-000092a0: 3c2f 6469 763e 0a20 2020 2020 2020 2020  </div>.         
-000092b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000092c0: 2020 207b 2520 656c 6966 2032 5f6d 6964     {% elif 2_mid
-000092d0: 5f74 6f70 5f62 2061 6e64 2032 5f6d 6964  _top_b and 2_mid
-000092e0: 5f74 6f70 5f63 2025 7d0a 2020 2020 2020  _top_c %}.      
-000092f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009300: 2020 2020 2020 2020 2020 3c64 6976 2063            <div c
-00009310: 6c61 7373 3d22 7b25 2062 6c6f 636b 2032  lass="{% block 2
-00009320: 5f6d 6964 5f74 6f70 5f62 635f 6220 257d  _mid_top_bc_b %}
-00009330: 636f 6c2d 3132 2063 6f6c 2d6d 642d 347b  col-12 col-md-4{
-00009340: 2520 656e 6462 6c6f 636b 2025 7d22 3e7b  % endblock %}">{
-00009350: 7b20 325f 6d69 645f 746f 705f 6220 7d7d  { 2_mid_top_b }}
-00009360: 3c2f 6469 763e 0a20 2020 2020 2020 2020  </div>.         
-00009370: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009380: 2020 2020 2020 203c 6469 7620 636c 6173         <div clas
-00009390: 733d 227b 2520 626c 6f63 6b20 325f 6d69  s="{% block 2_mi
-000093a0: 645f 746f 705f 6263 5f63 2025 7d63 6f6c  d_top_bc_c %}col
-000093b0: 2d31 3220 636f 6c2d 6d64 2d38 7b25 2065  -12 col-md-8{% e
-000093c0: 6e64 626c 6f63 6b20 257d 223e 7b7b 2032  ndblock %}">{{ 2
-000093d0: 5f6d 6964 5f74 6f70 5f63 207d 7d3c 2f64  _mid_top_c }}</d
-000093e0: 6976 3e0a 2020 2020 2020 2020 2020 2020  iv>.            
-000093f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009400: 7b25 2065 6c73 6520 257d 0a20 2020 2020  {% else %}.     
-00009410: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009420: 2020 2020 2020 2020 2020 203c 6469 7620             <div 
-00009430: 636c 6173 733d 2263 6f6c 2d31 3222 3e7b  class="col-12">{
-00009440: 7b20 325f 6d69 645f 746f 705f 6120 7d7d  { 2_mid_top_a }}
-00009450: 7b7b 2032 5f6d 6964 5f74 6f70 5f62 207d  {{ 2_mid_top_b }
-00009460: 7d7b 7b20 325f 6d69 645f 746f 705f 6320  }{{ 2_mid_top_c 
-00009470: 7d7d 3c2f 6469 763e 0a20 2020 2020 2020  }}</div>.       
+00008d50: 2020 2020 2020 2020 2020 2020 203c 6469               <di
+00008d60: 7620 636c 6173 733d 227b 2520 626c 6f63  v class="{% bloc
+00008d70: 6b20 325f 746f 705f 6162 5f61 2025 7d63  k 2_top_ab_a %}c
+00008d80: 6f6c 2d31 3220 636f 6c2d 6d64 2d38 7b25  ol-12 col-md-8{%
+00008d90: 2065 6e64 626c 6f63 6b20 257d 223e 7b7b   endblock %}">{{
+00008da0: 2032 5f74 6f70 5f61 207d 7d3c 2f64 6976   2_top_a }}</div
+00008db0: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
+00008dc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008dd0: 2020 3c64 6976 2063 6c61 7373 3d22 7b25    <div class="{%
+00008de0: 2062 6c6f 636b 2032 5f74 6f70 5f61 625f   block 2_top_ab_
+00008df0: 6220 257d 636f 6c2d 3132 2063 6f6c 2d6d  b %}col-12 col-m
+00008e00: 642d 347b 2520 656e 6462 6c6f 636b 2025  d-4{% endblock %
+00008e10: 7d22 3e7b 7b20 325f 746f 705f 6220 7d7d  }">{{ 2_top_b }}
+00008e20: 3c2f 6469 763e 0a20 2020 2020 2020 2020  </div>.         
+00008e30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008e40: 2020 207b 2520 656c 6966 2032 5f74 6f70     {% elif 2_top
+00008e50: 5f61 2061 6e64 2032 5f74 6f70 5f63 2025  _a and 2_top_c %
+00008e60: 7d0a 2020 2020 2020 2020 2020 2020 2020  }.              
+00008e70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008e80: 2020 3c64 6976 2063 6c61 7373 3d22 7b25    <div class="{%
+00008e90: 2062 6c6f 636b 2032 5f74 6f70 5f61 635f   block 2_top_ac_
+00008ea0: 6120 257d 636f 6c2d 3132 2063 6f6c 2d6d  a %}col-12 col-m
+00008eb0: 642d 367b 2520 656e 6462 6c6f 636b 2025  d-6{% endblock %
+00008ec0: 7d22 3e7b 7b20 325f 746f 705f 6120 7d7d  }">{{ 2_top_a }}
+00008ed0: 3c2f 6469 763e 0a20 2020 2020 2020 2020  </div>.         
+00008ee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008ef0: 2020 2020 2020 203c 6469 7620 636c 6173         <div clas
+00008f00: 733d 227b 2520 626c 6f63 6b20 325f 746f  s="{% block 2_to
+00008f10: 705f 6163 5f63 2025 7d63 6f6c 2d31 3220  p_ac_c %}col-12 
+00008f20: 636f 6c2d 6d64 2d36 7b25 2065 6e64 626c  col-md-6{% endbl
+00008f30: 6f63 6b20 257d 223e 7b7b 2032 5f74 6f70  ock %}">{{ 2_top
+00008f40: 5f63 207d 7d3c 2f64 6976 3e0a 2020 2020  _c }}</div>.    
+00008f50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008f60: 2020 2020 2020 2020 7b25 2065 6c69 6620          {% elif 
+00008f70: 325f 746f 705f 6220 616e 6420 325f 746f  2_top_b and 2_to
+00008f80: 705f 6320 257d 0a20 2020 2020 2020 2020  p_c %}.         
+00008f90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008fa0: 2020 2020 2020 203c 6469 7620 636c 6173         <div clas
+00008fb0: 733d 227b 2520 626c 6f63 6b20 325f 746f  s="{% block 2_to
+00008fc0: 705f 6263 5f62 2025 7d63 6f6c 2d31 3220  p_bc_b %}col-12 
+00008fd0: 636f 6c2d 6d64 2d34 7b25 2065 6e64 626c  col-md-4{% endbl
+00008fe0: 6f63 6b20 257d 223e 7b7b 2032 5f74 6f70  ock %}">{{ 2_top
+00008ff0: 5f62 207d 7d3c 2f64 6976 3e0a 2020 2020  _b }}</div>.    
+00009000: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009010: 2020 2020 2020 2020 2020 2020 3c64 6976              <div
+00009020: 2063 6c61 7373 3d22 7b25 2062 6c6f 636b   class="{% block
+00009030: 2032 5f74 6f70 5f62 635f 6320 257d 636f   2_top_bc_c %}co
+00009040: 6c2d 3132 2063 6f6c 2d6d 642d 387b 2520  l-12 col-md-8{% 
+00009050: 656e 6462 6c6f 636b 2025 7d22 3e7b 7b20  endblock %}">{{ 
+00009060: 325f 746f 705f 6320 7d7d 3c2f 6469 763e  2_top_c }}</div>
+00009070: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00009080: 2020 2020 2020 2020 2020 2020 207b 2520               {% 
+00009090: 656c 7365 2025 7d0a 2020 2020 2020 2020  else %}.        
+000090a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000090b0: 2020 2020 2020 2020 3c64 6976 2063 6c61          <div cla
+000090c0: 7373 3d22 636f 6c2d 3132 223e 7b7b 2032  ss="col-12">{{ 2
+000090d0: 5f74 6f70 5f61 207d 7d7b 7b20 325f 746f  _top_a }}{{ 2_to
+000090e0: 705f 6220 7d7d 7b7b 2032 5f74 6f70 5f63  p_b }}{{ 2_top_c
+000090f0: 207d 7d3c 2f64 6976 3e0a 2020 2020 2020   }}</div>.      
+00009100: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009110: 2020 2020 2020 7b25 2065 6e64 6966 2025        {% endif %
+00009120: 7d0a 2020 2020 2020 2020 2020 2020 2020  }.              
+00009130: 2020 2020 2020 2020 2020 3c2f 6469 763e            </div>
+00009140: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00009150: 2020 2020 203c 2f64 6976 3e0a 2020 2020       </div>.    
+00009160: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009170: 7b25 2065 6e64 6966 2025 7d0a 2020 2020  {% endif %}.    
+00009180: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009190: 3c21 2d2d 2065 6e64 2054 6f70 202d 2d3e  <!-- end Top -->
+000091a0: 0a0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000091b0: 2020 2020 2020 3c21 2d2d 204d 6964 646c        <!-- Middl
+000091c0: 6520 546f 7020 2d2d 3e0a 2020 2020 2020  e Top -->.      
+000091d0: 2020 2020 2020 2020 2020 2020 2020 7b25                {%
+000091e0: 2069 6620 325f 6d69 645f 746f 705f 6120   if 2_mid_top_a 
+000091f0: 6f72 2032 5f6d 6964 5f74 6f70 5f62 206f  or 2_mid_top_b o
+00009200: 7220 325f 6d69 645f 746f 705f 6320 257d  r 2_mid_top_c %}
+00009210: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00009220: 2020 2020 203c 6469 7620 636c 6173 733d       <div class=
+00009230: 2263 6f6c 2d31 3222 3e0a 2020 2020 2020  "col-12">.      
+00009240: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009250: 2020 3c64 6976 2063 6c61 7373 3d22 726f    <div class="ro
+00009260: 7722 3e0a 2020 2020 2020 2020 2020 2020  w">.            
+00009270: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009280: 7b25 2069 6620 325f 6d69 645f 746f 705f  {% if 2_mid_top_
+00009290: 6120 616e 6420 325f 6d69 645f 746f 705f  a and 2_mid_top_
+000092a0: 6220 616e 6420 325f 6d69 645f 746f 705f  b and 2_mid_top_
+000092b0: 6320 257d 0a20 2020 2020 2020 2020 2020  c %}.           
+000092c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000092d0: 2020 2020 203c 6469 7620 636c 6173 733d       <div class=
+000092e0: 227b 2520 626c 6f63 6b20 325f 6d69 645f  "{% block 2_mid_
+000092f0: 746f 705f 6162 635f 6120 257d 636f 6c2d  top_abc_a %}col-
+00009300: 3132 2063 6f6c 2d6d 642d 347b 2520 656e  12 col-md-4{% en
+00009310: 6462 6c6f 636b 2025 7d22 3e7b 7b20 325f  dblock %}">{{ 2_
+00009320: 6d69 645f 746f 705f 6120 7d7d 3c2f 6469  mid_top_a }}</di
+00009330: 763e 0a20 2020 2020 2020 2020 2020 2020  v>.             
+00009340: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009350: 2020 203c 6469 7620 636c 6173 733d 227b     <div class="{
+00009360: 2520 626c 6f63 6b20 325f 6d69 645f 746f  % block 2_mid_to
+00009370: 705f 6162 635f 6220 257d 636f 6c2d 3132  p_abc_b %}col-12
+00009380: 2063 6f6c 2d6d 642d 347b 2520 656e 6462   col-md-4{% endb
+00009390: 6c6f 636b 2025 7d22 3e7b 7b20 325f 6d69  lock %}">{{ 2_mi
+000093a0: 645f 746f 705f 6220 7d7d 3c2f 6469 763e  d_top_b }}</div>
+000093b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000093c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000093d0: 203c 6469 7620 636c 6173 733d 227b 2520   <div class="{% 
+000093e0: 626c 6f63 6b20 325f 6d69 645f 746f 705f  block 2_mid_top_
+000093f0: 6162 635f 6320 257d 636f 6c2d 3132 2063  abc_c %}col-12 c
+00009400: 6f6c 2d6d 642d 347b 2520 656e 6462 6c6f  ol-md-4{% endblo
+00009410: 636b 2025 7d22 3e7b 7b20 325f 6d69 645f  ck %}">{{ 2_mid_
+00009420: 746f 705f 6320 7d7d 3c2f 6469 763e 0a20  top_c }}</div>. 
+00009430: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009440: 2020 2020 2020 2020 2020 207b 2520 656c             {% el
+00009450: 6966 2032 5f6d 6964 5f74 6f70 5f61 2061  if 2_mid_top_a a
+00009460: 6e64 2032 5f6d 6964 5f74 6f70 5f62 2025  nd 2_mid_top_b %
+00009470: 7d0a 2020 2020 2020 2020 2020 2020 2020  }.              
 00009480: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009490: 2020 2020 207b 2520 656e 6469 6620 257d       {% endif %}
-000094a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000094b0: 2020 2020 2020 2020 203c 2f64 6976 3e0a           </div>.
-000094c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000094d0: 2020 2020 3c2f 6469 763e 0a20 2020 2020      </div>.     
-000094e0: 2020 2020 2020 2020 2020 2020 2020 207b                 {
-000094f0: 2520 656e 6469 6620 257d 0a20 2020 2020  % endif %}.     
+00009490: 2020 3c64 6976 2063 6c61 7373 3d22 7b25    <div class="{%
+000094a0: 2062 6c6f 636b 2032 5f6d 6964 5f74 6f70   block 2_mid_top
+000094b0: 5f61 625f 6120 257d 636f 6c2d 3132 2063  _ab_a %}col-12 c
+000094c0: 6f6c 2d6d 642d 387b 2520 656e 6462 6c6f  ol-md-8{% endblo
+000094d0: 636b 2025 7d22 3e7b 7b20 325f 6d69 645f  ck %}">{{ 2_mid_
+000094e0: 746f 705f 6120 7d7d 3c2f 6469 763e 0a20  top_a }}</div>. 
+000094f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00009500: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-00009510: 212d 2d20 656e 6420 4d69 6464 6c65 2054  !-- end Middle T
-00009520: 6f70 202d 2d3e 0a0a 2020 2020 2020 2020  op -->..        
-00009530: 2020 2020 2020 2020 2020 2020 3c21 2d2d              <!--
-00009540: 2042 6c6f 636b 7320 696e 2063 656e 7465   Blocks in cente
-00009550: 7220 706f 7369 7469 6f6e 7320 2d2d 3e0a  r positions -->.
-00009560: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009570: 2020 2020 7b25 2069 6620 325f 6365 6e74      {% if 2_cent
-00009580: 6572 5f74 6f70 5f61 206f 7220 325f 6365  er_top_a or 2_ce
-00009590: 6e74 6572 5f74 6f70 5f62 206f 7220 325f  nter_top_b or 2_
-000095a0: 6365 6e74 6572 5f74 6f70 5f63 206f 7220  center_top_c or 
-000095b0: 325f 6365 6e74 6572 5f6d 6964 5f74 6f70  2_center_mid_top
-000095c0: 5f61 206f 7220 325f 6365 6e74 6572 5f6d  _a or 2_center_m
-000095d0: 6964 5f74 6f70 5f62 206f 7220 325f 6365  id_top_b or 2_ce
-000095e0: 6e74 6572 5f6d 6964 5f74 6f70 5f63 206f  nter_mid_top_c o
-000095f0: 7220 325f 6365 6e74 6572 5f63 6f6e 7465  r 2_center_conte
-00009600: 6e74 206f 7220 325f 6365 6e74 6572 5f6d  nt or 2_center_m
-00009610: 6964 5f62 6f74 746f 6d5f 6120 6f72 2032  id_bottom_a or 2
-00009620: 5f63 656e 7465 725f 6d69 645f 626f 7474  _center_mid_bott
-00009630: 6f6d 5f62 206f 7220 325f 6365 6e74 6572  om_b or 2_center
-00009640: 5f6d 6964 5f62 6f74 746f 6d5f 6320 6f72  _mid_bottom_c or
-00009650: 2032 5f63 656e 7465 725f 626f 7474 6f6d   2_center_bottom
-00009660: 5f61 206f 7220 325f 6365 6e74 6572 5f62  _a or 2_center_b
-00009670: 6f74 746f 6d5f 6220 6f72 2032 5f63 656e  ottom_b or 2_cen
-00009680: 7465 725f 626f 7474 6f6d 5f63 2025 7d0a  ter_bottom_c %}.
-00009690: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000096a0: 2020 2020 2020 2020 203c 212d 2d20 426c           <!-- Bl
-000096b0: 6f63 6b73 2069 6e20 6c65 6674 2063 6f6c  ocks in left col
-000096c0: 756d 6e20 2d2d 3e0a 2020 2020 2020 2020  umn -->.        
-000096d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000096e0: 7b25 2069 6620 325f 6c65 6674 5f61 206f  {% if 2_left_a o
-000096f0: 7220 325f 6c65 6674 5f62 2025 7d0a 2020  r 2_left_b %}.  
-00009700: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009710: 2020 2020 2020 2020 2020 7b25 2069 6620            {% if 
-00009720: 325f 6c65 6674 5f61 2061 6e64 2032 5f6c  2_left_a and 2_l
-00009730: 6566 745f 6220 257d 0a20 2020 2020 2020  eft_b %}.       
-00009740: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009750: 2020 2020 203c 6469 7620 636c 6173 733d       <div class=
-00009760: 227b 2520 626c 6f63 6b20 325f 6c65 6674  "{% block 2_left
-00009770: 5f61 6220 257d 636f 6c2d 3132 2063 6f6c  _ab %}col-12 col
-00009780: 2d6c 672d 3420 6d62 2d35 206d 622d 6c67  -lg-4 mb-5 mb-lg
-00009790: 2d30 7b25 2065 6e64 626c 6f63 6b20 257d  -0{% endblock %}
-000097a0: 223e 0a20 2020 2020 2020 2020 2020 2020  ">.             
-000097b0: 2020 2020 2020 2020 2020 2020 2020 207b                 {
-000097c0: 2520 656c 6966 2032 5f6c 6566 745f 6120  % elif 2_left_a 
-000097d0: 257d 0a20 2020 2020 2020 2020 2020 2020  %}.             
-000097e0: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-000097f0: 6469 7620 636c 6173 733d 227b 2520 626c  div class="{% bl
-00009800: 6f63 6b20 325f 6c65 6674 5f61 2025 7d63  ock 2_left_a %}c
-00009810: 6f6c 2d31 3220 636f 6c2d 6c67 2d33 206d  ol-12 col-lg-3 m
-00009820: 622d 3520 6d62 2d6c 672d 307b 2520 656e  b-5 mb-lg-0{% en
-00009830: 6462 6c6f 636b 2025 7d22 3e0a 2020 2020  dblock %}">.    
-00009840: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009850: 2020 2020 2020 2020 7b25 2065 6c73 6520          {% else 
-00009860: 257d 0a20 2020 2020 2020 2020 2020 2020  %}.             
-00009870: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-00009880: 6469 7620 636c 6173 733d 227b 2520 626c  div class="{% bl
-00009890: 6f63 6b20 325f 6c65 6674 5f62 2025 7d63  ock 2_left_b %}c
-000098a0: 6f6c 2d31 3220 636f 6c2d 6c67 2d33 206d  ol-12 col-lg-3 m
-000098b0: 622d 3520 6d62 2d6c 672d 307b 2520 656e  b-5 mb-lg-0{% en
-000098c0: 6462 6c6f 636b 2025 7d22 3e0a 2020 2020  dblock %}">.    
-000098d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000098e0: 2020 2020 2020 2020 7b25 2065 6e64 6966          {% endif
-000098f0: 2025 7d0a 2020 2020 2020 2020 2020 2020   %}.            
+00009510: 6469 7620 636c 6173 733d 227b 2520 626c  div class="{% bl
+00009520: 6f63 6b20 325f 6d69 645f 746f 705f 6162  ock 2_mid_top_ab
+00009530: 5f62 2025 7d63 6f6c 2d31 3220 636f 6c2d  _b %}col-12 col-
+00009540: 6d64 2d34 7b25 2065 6e64 626c 6f63 6b20  md-4{% endblock 
+00009550: 257d 223e 7b7b 2032 5f6d 6964 5f74 6f70  %}">{{ 2_mid_top
+00009560: 5f62 207d 7d3c 2f64 6976 3e0a 2020 2020  _b }}</div>.    
+00009570: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009580: 2020 2020 2020 2020 7b25 2065 6c69 6620          {% elif 
+00009590: 325f 6d69 645f 746f 705f 6120 616e 6420  2_mid_top_a and 
+000095a0: 325f 6d69 645f 746f 705f 6320 257d 0a20  2_mid_top_c %}. 
+000095b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000095c0: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+000095d0: 6469 7620 636c 6173 733d 227b 2520 626c  div class="{% bl
+000095e0: 6f63 6b20 325f 6d69 645f 746f 705f 6163  ock 2_mid_top_ac
+000095f0: 5f61 2025 7d63 6f6c 2d31 3220 636f 6c2d  _a %}col-12 col-
+00009600: 6d64 2d36 7b25 2065 6e64 626c 6f63 6b20  md-6{% endblock 
+00009610: 257d 223e 7b7b 2032 5f6d 6964 5f74 6f70  %}">{{ 2_mid_top
+00009620: 5f61 207d 7d3c 2f64 6976 3e0a 2020 2020  _a }}</div>.    
+00009630: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009640: 2020 2020 2020 2020 2020 2020 3c64 6976              <div
+00009650: 2063 6c61 7373 3d22 7b25 2062 6c6f 636b   class="{% block
+00009660: 2032 5f6d 6964 5f74 6f70 5f61 635f 6320   2_mid_top_ac_c 
+00009670: 257d 636f 6c2d 3132 2063 6f6c 2d6d 642d  %}col-12 col-md-
+00009680: 367b 2520 656e 6462 6c6f 636b 2025 7d22  6{% endblock %}"
+00009690: 3e7b 7b20 325f 6d69 645f 746f 705f 6320  >{{ 2_mid_top_c 
+000096a0: 7d7d 3c2f 6469 763e 0a20 2020 2020 2020  }}</div>.       
+000096b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000096c0: 2020 2020 207b 2520 656c 6966 2032 5f6d       {% elif 2_m
+000096d0: 6964 5f74 6f70 5f62 2061 6e64 2032 5f6d  id_top_b and 2_m
+000096e0: 6964 5f74 6f70 5f63 2025 7d0a 2020 2020  id_top_c %}.    
+000096f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009700: 2020 2020 2020 2020 2020 2020 3c64 6976              <div
+00009710: 2063 6c61 7373 3d22 7b25 2062 6c6f 636b   class="{% block
+00009720: 2032 5f6d 6964 5f74 6f70 5f62 635f 6220   2_mid_top_bc_b 
+00009730: 257d 636f 6c2d 3132 2063 6f6c 2d6d 642d  %}col-12 col-md-
+00009740: 347b 2520 656e 6462 6c6f 636b 2025 7d22  4{% endblock %}"
+00009750: 3e7b 7b20 325f 6d69 645f 746f 705f 6220  >{{ 2_mid_top_b 
+00009760: 7d7d 3c2f 6469 763e 0a20 2020 2020 2020  }}</div>.       
+00009770: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009780: 2020 2020 2020 2020 203c 6469 7620 636c           <div cl
+00009790: 6173 733d 227b 2520 626c 6f63 6b20 325f  ass="{% block 2_
+000097a0: 6d69 645f 746f 705f 6263 5f63 2025 7d63  mid_top_bc_c %}c
+000097b0: 6f6c 2d31 3220 636f 6c2d 6d64 2d38 7b25  ol-12 col-md-8{%
+000097c0: 2065 6e64 626c 6f63 6b20 257d 223e 7b7b   endblock %}">{{
+000097d0: 2032 5f6d 6964 5f74 6f70 5f63 207d 7d3c   2_mid_top_c }}<
+000097e0: 2f64 6976 3e0a 2020 2020 2020 2020 2020  /div>.          
+000097f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009800: 2020 7b25 2065 6c73 6520 257d 0a20 2020    {% else %}.   
+00009810: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009820: 2020 2020 2020 2020 2020 2020 203c 6469               <di
+00009830: 7620 636c 6173 733d 2263 6f6c 2d31 3222  v class="col-12"
+00009840: 3e7b 7b20 325f 6d69 645f 746f 705f 6120  >{{ 2_mid_top_a 
+00009850: 7d7d 7b7b 2032 5f6d 6964 5f74 6f70 5f62  }}{{ 2_mid_top_b
+00009860: 207d 7d7b 7b20 325f 6d69 645f 746f 705f   }}{{ 2_mid_top_
+00009870: 6320 7d7d 3c2f 6469 763e 0a20 2020 2020  c }}</div>.     
+00009880: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009890: 2020 2020 2020 207b 2520 656e 6469 6620         {% endif 
+000098a0: 257d 0a20 2020 2020 2020 2020 2020 2020  %}.             
+000098b0: 2020 2020 2020 2020 2020 203c 2f64 6976             </div
+000098c0: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
+000098d0: 2020 2020 2020 3c2f 6469 763e 0a20 2020        </div>.   
+000098e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000098f0: 207b 2520 656e 6469 6620 257d 0a20 2020   {% endif %}.   
 00009900: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009910: 2020 2020 3c64 6976 2063 6c61 7373 3d22      <div class="
-00009920: 726f 7722 3e0a 2020 2020 2020 2020 2020  row">.          
-00009930: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009940: 2020 2020 2020 2020 2020 7b25 2069 6620            {% if 
-00009950: 325f 6c65 6674 5f61 2061 6e64 2032 5f6c  2_left_a and 2_l
-00009960: 6566 745f 6220 257d 0a20 2020 2020 2020  eft_b %}.       
-00009970: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009980: 2020 2020 2020 2020 2020 2020 203c 6469               <di
-00009990: 7620 636c 6173 733d 227b 2520 626c 6f63  v class="{% bloc
-000099a0: 6b20 325f 6c65 6674 5f61 625f 6120 257d  k 2_left_ab_a %}
-000099b0: 636f 6c2d 3132 2063 6f6c 2d6c 672d 367b  col-12 col-lg-6{
-000099c0: 2520 656e 6462 6c6f 636b 2025 7d22 3e7b  % endblock %}">{
-000099d0: 7b20 325f 6c65 6674 5f61 207d 7d3c 2f64  { 2_left_a }}</d
-000099e0: 6976 3e0a 2020 2020 2020 2020 2020 2020  iv>.            
-000099f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009a00: 2020 2020 2020 2020 3c64 6976 2063 6c61          <div cla
-00009a10: 7373 3d22 7b25 2062 6c6f 636b 2032 5f6c  ss="{% block 2_l
-00009a20: 6566 745f 6162 5f62 2025 7d63 6f6c 2d31  eft_ab_b %}col-1
-00009a30: 3220 636f 6c2d 6c67 2d36 7b25 2065 6e64  2 col-lg-6{% end
-00009a40: 626c 6f63 6b20 257d 223e 7b7b 2032 5f6c  block %}">{{ 2_l
-00009a50: 6566 745f 6220 7d7d 3c2f 6469 763e 0a20  eft_b }}</div>. 
-00009a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009a80: 2020 207b 2520 656c 6966 2032 5f6c 6566     {% elif 2_lef
-00009a90: 745f 6120 257d 0a20 2020 2020 2020 2020  t_a %}.         
-00009aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009ab0: 2020 2020 2020 2020 2020 203c 6469 7620             <div 
-00009ac0: 636c 6173 733d 2263 6f6c 2d31 3222 3e7b  class="col-12">{
-00009ad0: 7b20 325f 6c65 6674 5f61 207d 7d3c 2f64  { 2_left_a }}</d
-00009ae0: 6976 3e0a 2020 2020 2020 2020 2020 2020  iv>.            
-00009af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009b00: 2020 2020 2020 2020 7b25 2065 6c73 6520          {% else 
-00009b10: 257d 0a20 2020 2020 2020 2020 2020 2020  %}.             
-00009b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009b30: 2020 2020 2020 203c 6469 7620 636c 6173         <div clas
-00009b40: 733d 2263 6f6c 2d31 3222 3e7b 7b20 325f  s="col-12">{{ 2_
-00009b50: 6c65 6674 5f62 207d 7d3c 2f64 6976 3e0a  left_b }}</div>.
-00009b60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009b70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009b80: 2020 2020 7b25 2065 6e64 6966 2025 7d0a      {% endif %}.
-00009b90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009ba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009bb0: 3c2f 6469 763e 0a20 2020 2020 2020 2020  </div>.         
-00009bc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009bd0: 2020 203c 2f64 6976 3e0a 2020 2020 2020     </div>.      
+00009910: 203c 212d 2d20 656e 6420 4d69 6464 6c65   <!-- end Middle
+00009920: 2054 6f70 202d 2d3e 0a0a 2020 2020 2020   Top -->..      
+00009930: 2020 2020 2020 2020 2020 2020 2020 3c21                <!
+00009940: 2d2d 2042 6c6f 636b 7320 696e 2063 656e  -- Blocks in cen
+00009950: 7465 7220 706f 7369 7469 6f6e 7320 2d2d  ter positions --
+00009960: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
+00009970: 2020 2020 2020 7b25 2069 6620 325f 6365        {% if 2_ce
+00009980: 6e74 6572 5f74 6f70 5f61 206f 7220 325f  nter_top_a or 2_
+00009990: 6365 6e74 6572 5f74 6f70 5f62 206f 7220  center_top_b or 
+000099a0: 325f 6365 6e74 6572 5f74 6f70 5f63 206f  2_center_top_c o
+000099b0: 7220 325f 6365 6e74 6572 5f6d 6964 5f74  r 2_center_mid_t
+000099c0: 6f70 5f61 206f 7220 325f 6365 6e74 6572  op_a or 2_center
+000099d0: 5f6d 6964 5f74 6f70 5f62 206f 7220 325f  _mid_top_b or 2_
+000099e0: 6365 6e74 6572 5f6d 6964 5f74 6f70 5f63  center_mid_top_c
+000099f0: 206f 7220 325f 6365 6e74 6572 5f63 6f6e   or 2_center_con
+00009a00: 7465 6e74 206f 7220 325f 6365 6e74 6572  tent or 2_center
+00009a10: 5f6d 6964 5f62 6f74 746f 6d5f 6120 6f72  _mid_bottom_a or
+00009a20: 2032 5f63 656e 7465 725f 6d69 645f 626f   2_center_mid_bo
+00009a30: 7474 6f6d 5f62 206f 7220 325f 6365 6e74  ttom_b or 2_cent
+00009a40: 6572 5f6d 6964 5f62 6f74 746f 6d5f 6320  er_mid_bottom_c 
+00009a50: 6f72 2032 5f63 656e 7465 725f 626f 7474  or 2_center_bott
+00009a60: 6f6d 5f61 206f 7220 325f 6365 6e74 6572  om_a or 2_center
+00009a70: 5f62 6f74 746f 6d5f 6220 6f72 2032 5f63  _bottom_b or 2_c
+00009a80: 656e 7465 725f 626f 7474 6f6d 5f63 2025  enter_bottom_c %
+00009a90: 7d0a 0a20 2020 2020 2020 2020 2020 2020  }..             
+00009aa0: 2020 2020 2020 2020 2020 203c 212d 2d20             <!-- 
+00009ab0: 426c 6f63 6b73 2069 6e20 6c65 6674 2063  Blocks in left c
+00009ac0: 6f6c 756d 6e20 2d2d 3e0a 2020 2020 2020  olumn -->.      
+00009ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009ae0: 2020 7b25 2069 6620 325f 6c65 6674 5f61    {% if 2_left_a
+00009af0: 206f 7220 325f 6c65 6674 5f62 2025 7d0a   or 2_left_b %}.
+00009b00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009b10: 2020 2020 2020 2020 2020 2020 7b25 2069              {% i
+00009b20: 6620 325f 6c65 6674 5f61 2061 6e64 2032  f 2_left_a and 2
+00009b30: 5f6c 6566 745f 6220 257d 0a20 2020 2020  _left_b %}.     
+00009b40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009b50: 2020 2020 2020 203c 6469 7620 636c 6173         <div clas
+00009b60: 733d 227b 2520 626c 6f63 6b20 325f 6c65  s="{% block 2_le
+00009b70: 6674 5f61 6220 257d 636f 6c2d 3132 2063  ft_ab %}col-12 c
+00009b80: 6f6c 2d6c 672d 3420 6d62 2d35 206d 622d  ol-lg-4 mb-5 mb-
+00009b90: 6c67 2d30 7b25 2065 6e64 626c 6f63 6b20  lg-0{% endblock 
+00009ba0: 257d 223e 0a20 2020 2020 2020 2020 2020  %}">.           
+00009bb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009bc0: 207b 2520 656c 6966 2032 5f6c 6566 745f   {% elif 2_left_
+00009bd0: 6120 257d 0a20 2020 2020 2020 2020 2020  a %}.           
 00009be0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009bf0: 2020 7b25 2065 6e64 6966 2025 7d0a 2020    {% endif %}.  
-00009c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009c10: 2020 2020 2020 3c21 2d2d 2065 6e64 2042        <!-- end B
-00009c20: 6c6f 636b 7320 696e 206c 6566 7420 636f  locks in left co
-00009c30: 6c75 6d6e 202d 2d3e 0a0a 2020 2020 2020  lumn -->..      
+00009bf0: 203c 6469 7620 636c 6173 733d 227b 2520   <div class="{% 
+00009c00: 626c 6f63 6b20 325f 6c65 6674 5f61 2025  block 2_left_a %
+00009c10: 7d63 6f6c 2d31 3220 636f 6c2d 6c67 2d33  }col-12 col-lg-3
+00009c20: 206d 622d 3520 6d62 2d6c 672d 307b 2520   mb-5 mb-lg-0{% 
+00009c30: 656e 6462 6c6f 636b 2025 7d22 3e0a 2020  endblock %}">.  
 00009c40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009c50: 2020 3c21 2d2d 2042 6c6f 636b 7320 696e    <!-- Blocks in
-00009c60: 2043 656e 7465 7220 636f 6c75 6d6e 2028   Center column (
-00009c70: 7461 6b65 7320 6176 6169 6c61 626c 6520  takes available 
-00009c80: 7370 6163 6529 202d 2d3e 0a20 2020 2020  space) -->.     
-00009c90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009ca0: 2020 207b 2520 6966 2032 5f6c 6566 745f     {% if 2_left_
-00009cb0: 6120 616e 6420 325f 6c65 6674 5f62 2061  a and 2_left_b a
-00009cc0: 6e64 2032 5f72 6967 6874 5f61 2061 6e64  nd 2_right_a and
-00009cd0: 2032 5f72 6967 6874 5f62 2025 7d0a 2020   2_right_b %}.  
-00009ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009cf0: 2020 2020 2020 3c64 6976 2063 6c61 7373        <div class
-00009d00: 3d22 7b25 2062 6c6f 636b 2032 5f63 656e  ="{% block 2_cen
-00009d10: 7465 725f 6c65 6674 5f61 625f 7269 6768  ter_left_ab_righ
-00009d20: 745f 6162 2025 7d63 6f6c 2d31 3220 636f  t_ab %}col-12 co
-00009d30: 6c2d 6c67 2d34 7b25 2065 6e64 626c 6f63  l-lg-4{% endbloc
-00009d40: 6b20 257d 223e 0a20 2020 2020 2020 2020  k %}">.         
-00009d50: 2020 2020 2020 2020 2020 2020 2020 207b                 {
-00009d60: 2520 656c 6966 2032 5f6c 6566 745f 6120  % elif 2_left_a 
-00009d70: 616e 6420 325f 6c65 6674 5f62 2061 6e64  and 2_left_b and
-00009d80: 2032 5f72 6967 6874 5f61 2025 7d0a 2020   2_right_a %}.  
-00009d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009da0: 2020 2020 2020 3c64 6976 2063 6c61 7373        <div class
-00009db0: 3d22 7b25 2062 6c6f 636b 2032 5f63 656e  ="{% block 2_cen
-00009dc0: 7465 725f 6c65 6674 5f61 625f 7269 6768  ter_left_ab_righ
-00009dd0: 745f 6120 257d 636f 6c2d 3132 2063 6f6c  t_a %}col-12 col
-00009de0: 2d6c 672d 357b 2520 656e 6462 6c6f 636b  -lg-5{% endblock
-00009df0: 2025 7d22 3e0a 2020 2020 2020 2020 2020   %}">.          
-00009e00: 2020 2020 2020 2020 2020 2020 2020 7b25                {%
-00009e10: 2065 6c69 6620 325f 6c65 6674 5f61 2061   elif 2_left_a a
-00009e20: 6e64 2032 5f6c 6566 745f 6220 616e 6420  nd 2_left_b and 
-00009e30: 325f 7269 6768 745f 6220 257d 0a20 2020  2_right_b %}.   
-00009e40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009e50: 2020 2020 203c 6469 7620 636c 6173 733d       <div class=
-00009e60: 227b 2520 626c 6f63 6b20 325f 6365 6e74  "{% block 2_cent
-00009e70: 6572 5f6c 6566 745f 6162 5f72 6967 6874  er_left_ab_right
-00009e80: 5f62 2025 7d63 6f6c 2d31 3220 636f 6c2d  _b %}col-12 col-
-00009e90: 6c67 2d34 7b25 2065 6e64 626c 6f63 6b20  lg-4{% endblock 
-00009ea0: 257d 223e 0a20 2020 2020 2020 2020 2020  %}">.           
-00009eb0: 2020 2020 2020 2020 2020 2020 207b 2520               {% 
-00009ec0: 656c 6966 2032 5f6c 6566 745f 6120 616e  elif 2_left_a an
-00009ed0: 6420 325f 7269 6768 745f 6120 616e 6420  d 2_right_a and 
-00009ee0: 325f 7269 6768 745f 6220 257d 0a20 2020  2_right_b %}.   
+00009c50: 2020 2020 2020 2020 2020 7b25 2065 6c73            {% els
+00009c60: 6520 257d 0a20 2020 2020 2020 2020 2020  e %}.           
+00009c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009c80: 203c 6469 7620 636c 6173 733d 227b 2520   <div class="{% 
+00009c90: 626c 6f63 6b20 325f 6c65 6674 5f62 2025  block 2_left_b %
+00009ca0: 7d63 6f6c 2d31 3220 636f 6c2d 6c67 2d33  }col-12 col-lg-3
+00009cb0: 206d 622d 3520 6d62 2d6c 672d 307b 2520   mb-5 mb-lg-0{% 
+00009cc0: 656e 6462 6c6f 636b 2025 7d22 3e0a 2020  endblock %}">.  
+00009cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009ce0: 2020 2020 2020 2020 2020 7b25 2065 6e64            {% end
+00009cf0: 6966 2025 7d0a 2020 2020 2020 2020 2020  if %}.          
+00009d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009d10: 2020 2020 2020 3c64 6976 2063 6c61 7373        <div class
+00009d20: 3d22 726f 7722 3e0a 2020 2020 2020 2020  ="row">.        
+00009d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009d40: 2020 2020 2020 2020 2020 2020 7b25 2069              {% i
+00009d50: 6620 325f 6c65 6674 5f61 2061 6e64 2032  f 2_left_a and 2
+00009d60: 5f6c 6566 745f 6220 257d 0a20 2020 2020  _left_b %}.     
+00009d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009d80: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+00009d90: 6469 7620 636c 6173 733d 227b 2520 626c  div class="{% bl
+00009da0: 6f63 6b20 325f 6c65 6674 5f61 625f 6120  ock 2_left_ab_a 
+00009db0: 257d 636f 6c2d 3132 2063 6f6c 2d6c 672d  %}col-12 col-lg-
+00009dc0: 367b 2520 656e 6462 6c6f 636b 2025 7d22  6{% endblock %}"
+00009dd0: 3e7b 7b20 325f 6c65 6674 5f61 207d 7d3c  >{{ 2_left_a }}<
+00009de0: 2f64 6976 3e0a 2020 2020 2020 2020 2020  /div>.          
+00009df0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009e00: 2020 2020 2020 2020 2020 3c64 6976 2063            <div c
+00009e10: 6c61 7373 3d22 7b25 2062 6c6f 636b 2032  lass="{% block 2
+00009e20: 5f6c 6566 745f 6162 5f62 2025 7d63 6f6c  _left_ab_b %}col
+00009e30: 2d31 3220 636f 6c2d 6c67 2d36 7b25 2065  -12 col-lg-6{% e
+00009e40: 6e64 626c 6f63 6b20 257d 223e 7b7b 2032  ndblock %}">{{ 2
+00009e50: 5f6c 6566 745f 6220 7d7d 3c2f 6469 763e  _left_b }}</div>
+00009e60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00009e70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009e80: 2020 2020 207b 2520 656c 6966 2032 5f6c       {% elif 2_l
+00009e90: 6566 745f 6120 257d 0a20 2020 2020 2020  eft_a %}.       
+00009ea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009eb0: 2020 2020 2020 2020 2020 2020 203c 6469               <di
+00009ec0: 7620 636c 6173 733d 2263 6f6c 2d31 3222  v class="col-12"
+00009ed0: 3e7b 7b20 325f 6c65 6674 5f61 207d 7d3c  >{{ 2_left_a }}<
+00009ee0: 2f64 6976 3e0a 2020 2020 2020 2020 2020  /div>.          
 00009ef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009f00: 2020 2020 203c 6469 7620 636c 6173 733d       <div class=
-00009f10: 227b 2520 626c 6f63 6b20 325f 6365 6e74  "{% block 2_cent
-00009f20: 6572 5f6c 6566 745f 615f 7269 6768 745f  er_left_a_right_
-00009f30: 6162 2025 7d63 6f6c 2d31 3220 636f 6c2d  ab %}col-12 col-
-00009f40: 6c67 2d35 7b25 2065 6e64 626c 6f63 6b20  lg-5{% endblock 
-00009f50: 257d 223e 0a20 2020 2020 2020 2020 2020  %}">.           
-00009f60: 2020 2020 2020 2020 2020 2020 207b 2520               {% 
-00009f70: 656c 6966 2032 5f6c 6566 745f 6120 616e  elif 2_left_a an
-00009f80: 6420 325f 7269 6768 745f 6120 257d 0a20  d 2_right_a %}. 
-00009f90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009fa0: 2020 2020 2020 203c 6469 7620 636c 6173         <div clas
-00009fb0: 733d 227b 2520 626c 6f63 6b20 325f 6365  s="{% block 2_ce
-00009fc0: 6e74 6572 5f6c 6566 745f 615f 7269 6768  nter_left_a_righ
-00009fd0: 745f 6120 257d 636f 6c2d 3132 2063 6f6c  t_a %}col-12 col
-00009fe0: 2d6c 672d 367b 2520 656e 6462 6c6f 636b  -lg-6{% endblock
-00009ff0: 2025 7d22 3e0a 2020 2020 2020 2020 2020   %}">.          
-0000a000: 2020 2020 2020 2020 2020 2020 2020 7b25                {%
-0000a010: 2065 6c69 6620 325f 6c65 6674 5f61 2061   elif 2_left_a a
-0000a020: 6e64 2032 5f72 6967 6874 5f62 2025 7d0a  nd 2_right_b %}.
-0000a030: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a040: 2020 2020 2020 2020 3c64 6976 2063 6c61          <div cla
-0000a050: 7373 3d22 7b25 2062 6c6f 636b 2032 5f63  ss="{% block 2_c
-0000a060: 656e 7465 725f 6c65 6674 5f61 5f72 6967  enter_left_a_rig
-0000a070: 6874 5f62 2025 7d63 6f6c 2d31 3220 636f  ht_b %}col-12 co
-0000a080: 6c2d 6c67 2d35 7b25 2065 6e64 626c 6f63  l-lg-5{% endbloc
-0000a090: 6b20 257d 223e 0a20 2020 2020 2020 2020  k %}">.         
-0000a0a0: 2020 2020 2020 2020 2020 2020 2020 207b                 {
-0000a0b0: 2520 656c 6966 2032 5f6c 6566 745f 6220  % elif 2_left_b 
-0000a0c0: 616e 6420 325f 7269 6768 745f 6120 616e  and 2_right_a an
-0000a0d0: 6420 325f 7269 6768 745f 6220 257d 0a20  d 2_right_b %}. 
+00009f00: 2020 2020 2020 2020 2020 7b25 2065 6c73            {% els
+00009f10: 6520 257d 0a20 2020 2020 2020 2020 2020  e %}.           
+00009f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009f30: 2020 2020 2020 2020 203c 6469 7620 636c           <div cl
+00009f40: 6173 733d 2263 6f6c 2d31 3222 3e7b 7b20  ass="col-12">{{ 
+00009f50: 325f 6c65 6674 5f62 207d 7d3c 2f64 6976  2_left_b }}</div
+00009f60: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
+00009f70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009f80: 2020 2020 2020 7b25 2065 6e64 6966 2025        {% endif %
+00009f90: 7d0a 2020 2020 2020 2020 2020 2020 2020  }.              
+00009fa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009fb0: 2020 3c2f 6469 763e 0a20 2020 2020 2020    </div>.       
+00009fc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009fd0: 2020 2020 203c 2f64 6976 3e0a 2020 2020       </div>.    
+00009fe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009ff0: 2020 2020 7b25 2065 6e64 6966 2025 7d0a      {% endif %}.
+0000a000: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a010: 2020 2020 2020 2020 3c21 2d2d 2065 6e64          <!-- end
+0000a020: 2042 6c6f 636b 7320 696e 206c 6566 7420   Blocks in left 
+0000a030: 636f 6c75 6d6e 202d 2d3e 0a0a 2020 2020  column -->..    
+0000a040: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a050: 2020 2020 3c21 2d2d 2042 6c6f 636b 7320      <!-- Blocks 
+0000a060: 696e 2043 656e 7465 7220 636f 6c75 6d6e  in Center column
+0000a070: 2028 7461 6b65 7320 6176 6169 6c61 626c   (takes availabl
+0000a080: 6520 7370 6163 6529 202d 2d3e 0a20 2020  e space) -->.   
+0000a090: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a0a0: 2020 2020 207b 2520 6966 2032 5f6c 6566       {% if 2_lef
+0000a0b0: 745f 6120 616e 6420 325f 6c65 6674 5f62  t_a and 2_left_b
+0000a0c0: 2061 6e64 2032 5f72 6967 6874 5f61 2061   and 2_right_a a
+0000a0d0: 6e64 2032 5f72 6967 6874 5f62 2025 7d0a  nd 2_right_b %}.
 0000a0e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a0f0: 2020 2020 2020 203c 6469 7620 636c 6173         <div clas
-0000a100: 733d 227b 2520 626c 6f63 6b20 325f 6365  s="{% block 2_ce
-0000a110: 6e74 6572 5f6c 6566 745f 625f 7269 6768  nter_left_b_righ
-0000a120: 745f 6162 2025 7d63 6f6c 2d31 3220 636f  t_ab %}col-12 co
-0000a130: 6c2d 6c67 2d34 206f 6666 7365 742d 6c67  l-lg-4 offset-lg
-0000a140: 2d31 7b25 2065 6e64 626c 6f63 6b20 257d  -1{% endblock %}
-0000a150: 223e 0a20 2020 2020 2020 2020 2020 2020  ">.             
-0000a160: 2020 2020 2020 2020 2020 207b 2520 656c             {% el
-0000a170: 6966 2032 5f6c 6566 745f 6220 616e 6420  if 2_left_b and 
-0000a180: 325f 7269 6768 745f 6120 257d 0a20 2020  2_right_a %}.   
+0000a0f0: 2020 2020 2020 2020 3c64 6976 2063 6c61          <div cla
+0000a100: 7373 3d22 7b25 2062 6c6f 636b 2032 5f63  ss="{% block 2_c
+0000a110: 656e 7465 725f 6c65 6674 5f61 625f 7269  enter_left_ab_ri
+0000a120: 6768 745f 6162 2025 7d63 6f6c 2d31 3220  ght_ab %}col-12 
+0000a130: 636f 6c2d 6c67 2d34 7b25 2065 6e64 626c  col-lg-4{% endbl
+0000a140: 6f63 6b20 257d 223e 0a20 2020 2020 2020  ock %}">.       
+0000a150: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a160: 207b 2520 656c 6966 2032 5f6c 6566 745f   {% elif 2_left_
+0000a170: 6120 616e 6420 325f 6c65 6674 5f62 2061  a and 2_left_b a
+0000a180: 6e64 2032 5f72 6967 6874 5f61 2025 7d0a  nd 2_right_a %}.
 0000a190: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a1a0: 2020 2020 203c 6469 7620 636c 6173 733d       <div class=
-0000a1b0: 227b 2520 626c 6f63 6b20 325f 6365 6e74  "{% block 2_cent
-0000a1c0: 6572 5f6c 6566 745f 625f 7269 6768 745f  er_left_b_right_
-0000a1d0: 6120 257d 636f 6c2d 3132 2063 6f6c 2d6c  a %}col-12 col-l
-0000a1e0: 672d 3520 6f66 6673 6574 2d6c 672d 317b  g-5 offset-lg-1{
-0000a1f0: 2520 656e 6462 6c6f 636b 2025 7d22 3e0a  % endblock %}">.
+0000a1a0: 2020 2020 2020 2020 3c64 6976 2063 6c61          <div cla
+0000a1b0: 7373 3d22 7b25 2062 6c6f 636b 2032 5f63  ss="{% block 2_c
+0000a1c0: 656e 7465 725f 6c65 6674 5f61 625f 7269  enter_left_ab_ri
+0000a1d0: 6768 745f 6120 257d 636f 6c2d 3132 2063  ght_a %}col-12 c
+0000a1e0: 6f6c 2d6c 672d 357b 2520 656e 6462 6c6f  ol-lg-5{% endblo
+0000a1f0: 636b 2025 7d22 3e0a 2020 2020 2020 2020  ck %}">.        
 0000a200: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a210: 2020 2020 2020 2020 7b25 2065 6c69 6620          {% elif 
-0000a220: 325f 6c65 6674 5f62 2061 6e64 2032 5f72  2_left_b and 2_r
-0000a230: 6967 6874 5f62 2025 7d0a 2020 2020 2020  ight_b %}.      
+0000a210: 7b25 2065 6c69 6620 325f 6c65 6674 5f61  {% elif 2_left_a
+0000a220: 2061 6e64 2032 5f6c 6566 745f 6220 616e   and 2_left_b an
+0000a230: 6420 325f 7269 6768 745f 6220 257d 0a20  d 2_right_b %}. 
 0000a240: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a250: 2020 3c64 6976 2063 6c61 7373 3d22 7b25    <div class="{%
-0000a260: 2062 6c6f 636b 2032 5f63 656e 7465 725f   block 2_center_
-0000a270: 6c65 6674 5f62 5f72 6967 6874 5f62 2025  left_b_right_b %
-0000a280: 7d63 6f6c 2d31 3220 636f 6c2d 6c67 2d34  }col-12 col-lg-4
-0000a290: 206f 6666 7365 742d 6c67 2d31 7b25 2065   offset-lg-1{% e
-0000a2a0: 6e64 626c 6f63 6b20 257d 223e 0a20 2020  ndblock %}">.   
-0000a2b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a2c0: 2020 2020 207b 2520 656c 6966 2032 5f6c       {% elif 2_l
-0000a2d0: 6566 745f 6120 616e 6420 325f 6c65 6674  eft_a and 2_left
-0000a2e0: 5f62 2025 7d0a 2020 2020 2020 2020 2020  _b %}.          
-0000a2f0: 2020 2020 2020 2020 2020 2020 2020 3c64                <d
-0000a300: 6976 2063 6c61 7373 3d22 7b25 2062 6c6f  iv class="{% blo
-0000a310: 636b 2032 5f63 656e 7465 725f 6c65 6674  ck 2_center_left
-0000a320: 5f61 6220 257d 636f 6c2d 3132 2063 6f6c  _ab %}col-12 col
-0000a330: 2d6c 672d 387b 2520 656e 6462 6c6f 636b  -lg-8{% endblock
-0000a340: 2025 7d22 3e0a 2020 2020 2020 2020 2020   %}">.          
-0000a350: 2020 2020 2020 2020 2020 2020 2020 7b25                {%
-0000a360: 2065 6c69 6620 325f 6c65 6674 5f61 2025   elif 2_left_a %
-0000a370: 7d0a 2020 2020 2020 2020 2020 2020 2020  }.              
-0000a380: 2020 2020 2020 2020 2020 3c64 6976 2063            <div c
-0000a390: 6c61 7373 3d22 7b25 2062 6c6f 636b 2032  lass="{% block 2
-0000a3a0: 5f63 656e 7465 725f 6c65 6674 5f61 2025  _center_left_a %
-0000a3b0: 7d63 6f6c 2d31 3220 636f 6c2d 6c67 2d39  }col-12 col-lg-9
-0000a3c0: 7b25 2065 6e64 626c 6f63 6b20 257d 223e  {% endblock %}">
-0000a3d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000a3e0: 2020 2020 2020 2020 207b 2520 656c 6966           {% elif
-0000a3f0: 2032 5f6c 6566 745f 6220 257d 0a20 2020   2_left_b %}.   
+0000a250: 2020 2020 2020 203c 6469 7620 636c 6173         <div clas
+0000a260: 733d 227b 2520 626c 6f63 6b20 325f 6365  s="{% block 2_ce
+0000a270: 6e74 6572 5f6c 6566 745f 6162 5f72 6967  nter_left_ab_rig
+0000a280: 6874 5f62 2025 7d63 6f6c 2d31 3220 636f  ht_b %}col-12 co
+0000a290: 6c2d 6c67 2d34 7b25 2065 6e64 626c 6f63  l-lg-4{% endbloc
+0000a2a0: 6b20 257d 223e 0a20 2020 2020 2020 2020  k %}">.         
+0000a2b0: 2020 2020 2020 2020 2020 2020 2020 207b                 {
+0000a2c0: 2520 656c 6966 2032 5f6c 6566 745f 6120  % elif 2_left_a 
+0000a2d0: 616e 6420 325f 7269 6768 745f 6120 616e  and 2_right_a an
+0000a2e0: 6420 325f 7269 6768 745f 6220 257d 0a20  d 2_right_b %}. 
+0000a2f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a300: 2020 2020 2020 203c 6469 7620 636c 6173         <div clas
+0000a310: 733d 227b 2520 626c 6f63 6b20 325f 6365  s="{% block 2_ce
+0000a320: 6e74 6572 5f6c 6566 745f 615f 7269 6768  nter_left_a_righ
+0000a330: 745f 6162 2025 7d63 6f6c 2d31 3220 636f  t_ab %}col-12 co
+0000a340: 6c2d 6c67 2d35 7b25 2065 6e64 626c 6f63  l-lg-5{% endbloc
+0000a350: 6b20 257d 223e 0a20 2020 2020 2020 2020  k %}">.         
+0000a360: 2020 2020 2020 2020 2020 2020 2020 207b                 {
+0000a370: 2520 656c 6966 2032 5f6c 6566 745f 6120  % elif 2_left_a 
+0000a380: 616e 6420 325f 7269 6768 745f 6120 257d  and 2_right_a %}
+0000a390: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000a3a0: 2020 2020 2020 2020 203c 6469 7620 636c           <div cl
+0000a3b0: 6173 733d 227b 2520 626c 6f63 6b20 325f  ass="{% block 2_
+0000a3c0: 6365 6e74 6572 5f6c 6566 745f 615f 7269  center_left_a_ri
+0000a3d0: 6768 745f 6120 257d 636f 6c2d 3132 2063  ght_a %}col-12 c
+0000a3e0: 6f6c 2d6c 672d 367b 2520 656e 6462 6c6f  ol-lg-6{% endblo
+0000a3f0: 636b 2025 7d22 3e0a 2020 2020 2020 2020  ck %}">.        
 0000a400: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a410: 2020 2020 203c 6469 7620 636c 6173 733d       <div class=
-0000a420: 227b 2520 626c 6f63 6b20 325f 6365 6e74  "{% block 2_cent
-0000a430: 6572 5f6c 6566 745f 6220 257d 636f 6c2d  er_left_b %}col-
-0000a440: 3132 2063 6f6c 2d6c 672d 3820 6f66 6673  12 col-lg-8 offs
-0000a450: 6574 2d6c 672d 317b 2520 656e 6462 6c6f  et-lg-1{% endblo
-0000a460: 636b 2025 7d22 3e0a 2020 2020 2020 2020  ck %}">.        
-0000a470: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a480: 7b25 2065 6c69 6620 325f 7269 6768 745f  {% elif 2_right_
-0000a490: 6120 616e 6420 325f 7269 6768 745f 6220  a and 2_right_b 
-0000a4a0: 257d 0a20 2020 2020 2020 2020 2020 2020  %}.             
-0000a4b0: 2020 2020 2020 2020 2020 203c 6469 7620             <div 
-0000a4c0: 636c 6173 733d 227b 2520 626c 6f63 6b20  class="{% block 
-0000a4d0: 325f 6365 6e74 6572 5f72 6967 6874 5f61  2_center_right_a
-0000a4e0: 6220 257d 636f 6c2d 3132 2063 6f6c 2d6c  b %}col-12 col-l
-0000a4f0: 672d 387b 2520 656e 6462 6c6f 636b 2025  g-8{% endblock %
-0000a500: 7d22 3e0a 2020 2020 2020 2020 2020 2020  }">.            
-0000a510: 2020 2020 2020 2020 2020 2020 7b25 2065              {% e
-0000a520: 6c69 6620 325f 7269 6768 745f 6120 257d  lif 2_right_a %}
-0000a530: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000a540: 2020 2020 2020 2020 203c 6469 7620 636c           <div cl
-0000a550: 6173 733d 227b 2520 626c 6f63 6b20 325f  ass="{% block 2_
-0000a560: 6365 6e74 6572 5f72 6967 6874 5f61 2025  center_right_a %
-0000a570: 7d63 6f6c 2d31 3220 636f 6c2d 6c67 2d39  }col-12 col-lg-9
-0000a580: 7b25 2065 6e64 626c 6f63 6b20 257d 223e  {% endblock %}">
-0000a590: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000a5a0: 2020 2020 2020 2020 207b 2520 656c 6966           {% elif
-0000a5b0: 2032 5f72 6967 6874 5f62 2025 7d0a 2020   2_right_b %}.  
-0000a5c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a5d0: 2020 2020 2020 3c64 6976 2063 6c61 7373        <div class
-0000a5e0: 3d22 7b25 2062 6c6f 636b 2032 5f63 656e  ="{% block 2_cen
-0000a5f0: 7465 725f 7269 6768 745f 6220 257d 636f  ter_right_b %}co
-0000a600: 6c2d 3132 2063 6f6c 2d6c 672d 387b 2520  l-12 col-lg-8{% 
-0000a610: 656e 6462 6c6f 636b 2025 7d22 3e0a 2020  endblock %}">.  
-0000a620: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a630: 2020 2020 2020 7b25 2065 6c73 6520 257d        {% else %}
-0000a640: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000a650: 2020 2020 2020 2020 203c 6469 7620 636c           <div cl
-0000a660: 6173 733d 227b 2520 626c 6f63 6b20 325f  ass="{% block 2_
-0000a670: 6365 6e74 6572 2025 7d63 6f6c 2d31 327b  center %}col-12{
-0000a680: 2520 656e 6462 6c6f 636b 2025 7d22 3e0a  % endblock %}">.
-0000a690: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a6a0: 2020 2020 2020 2020 7b25 2065 6e64 6966          {% endif
-0000a6b0: 2025 7d0a 2020 2020 2020 2020 2020 2020   %}.            
-0000a6c0: 2020 2020 2020 2020 2020 2020 3c21 2d2d              <!--
-0000a6d0: 2045 6e64 2042 6c6f 636b 7320 696e 2043   End Blocks in C
-0000a6e0: 656e 7465 7220 636f 6c75 6d6e 2028 7461  enter column (ta
-0000a6f0: 6b65 7320 6176 6169 6c61 626c 6520 7370  kes available sp
-0000a700: 6163 6529 202d 2d3e 0a0a 2020 2020 2020  ace) -->..      
-0000a710: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a720: 2020 2020 2020 3c21 2d2d 2043 656e 7465        <!-- Cente
-0000a730: 7220 746f 7020 2d2d 3e0a 2020 2020 2020  r top -->.      
-0000a740: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a750: 2020 2020 2020 7b25 2069 6620 325f 6365        {% if 2_ce
-0000a760: 6e74 6572 5f74 6f70 5f61 206f 7220 325f  nter_top_a or 2_
-0000a770: 6365 6e74 6572 5f74 6f70 5f62 206f 7220  center_top_b or 
-0000a780: 325f 6365 6e74 6572 5f74 6f70 5f63 2025  2_center_top_c %
-0000a790: 7d0a 2020 2020 2020 2020 2020 2020 2020  }.              
-0000a7a0: 2020 2020 2020 2020 2020 2020 2020 3c64                <d
-0000a7b0: 6976 2063 6c61 7373 3d22 726f 7722 3e0a  iv class="row">.
-0000a7c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a7d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a7e0: 7b25 2069 6620 325f 6365 6e74 6572 5f74  {% if 2_center_t
-0000a7f0: 6f70 5f61 2061 6e64 2032 5f63 656e 7465  op_a and 2_cente
-0000a800: 725f 746f 705f 6220 616e 6420 325f 6365  r_top_b and 2_ce
-0000a810: 6e74 6572 5f74 6f70 5f63 2025 7d0a 2020  nter_top_c %}.  
-0000a820: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a830: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a840: 2020 3c64 6976 2063 6c61 7373 3d22 7b25    <div class="{%
-0000a850: 2062 6c6f 636b 2032 5f63 656e 7465 725f   block 2_center_
-0000a860: 746f 705f 6162 635f 6120 257d 636f 6c2d  top_abc_a %}col-
-0000a870: 3132 2063 6f6c 2d6d 642d 347b 2520 656e  12 col-md-4{% en
-0000a880: 6462 6c6f 636b 2025 7d22 3e7b 7b20 325f  dblock %}">{{ 2_
-0000a890: 6365 6e74 6572 5f74 6f70 5f61 207d 7d3c  center_top_a }}<
-0000a8a0: 2f64 6976 3e0a 2020 2020 2020 2020 2020  /div>.          
-0000a8b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a8c0: 2020 2020 2020 2020 2020 3c64 6976 2063            <div c
-0000a8d0: 6c61 7373 3d22 7b25 2062 6c6f 636b 2032  lass="{% block 2
-0000a8e0: 5f63 656e 7465 725f 746f 705f 6162 635f  _center_top_abc_
-0000a8f0: 6220 257d 636f 6c2d 3132 2063 6f6c 2d6d  b %}col-12 col-m
-0000a900: 642d 347b 2520 656e 6462 6c6f 636b 2025  d-4{% endblock %
-0000a910: 7d22 3e7b 7b20 325f 6365 6e74 6572 5f74  }">{{ 2_center_t
-0000a920: 6f70 5f62 207d 7d3c 2f64 6976 3e0a 2020  op_b }}</div>.  
-0000a930: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a940: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a950: 2020 3c64 6976 2063 6c61 7373 3d22 7b25    <div class="{%
-0000a960: 2062 6c6f 636b 2032 5f63 656e 7465 725f   block 2_center_
-0000a970: 746f 705f 6162 635f 6320 257d 636f 6c2d  top_abc_c %}col-
-0000a980: 3132 2063 6f6c 2d6d 642d 347b 2520 656e  12 col-md-4{% en
-0000a990: 6462 6c6f 636b 2025 7d22 3e7b 7b20 325f  dblock %}">{{ 2_
-0000a9a0: 6365 6e74 6572 5f74 6f70 5f63 207d 7d3c  center_top_c }}<
-0000a9b0: 2f64 6976 3e0a 2020 2020 2020 2020 2020  /div>.          
+0000a410: 7b25 2065 6c69 6620 325f 6c65 6674 5f61  {% elif 2_left_a
+0000a420: 2061 6e64 2032 5f72 6967 6874 5f62 2025   and 2_right_b %
+0000a430: 7d0a 2020 2020 2020 2020 2020 2020 2020  }.              
+0000a440: 2020 2020 2020 2020 2020 3c64 6976 2063            <div c
+0000a450: 6c61 7373 3d22 7b25 2062 6c6f 636b 2032  lass="{% block 2
+0000a460: 5f63 656e 7465 725f 6c65 6674 5f61 5f72  _center_left_a_r
+0000a470: 6967 6874 5f62 2025 7d63 6f6c 2d31 3220  ight_b %}col-12 
+0000a480: 636f 6c2d 6c67 2d35 7b25 2065 6e64 626c  col-lg-5{% endbl
+0000a490: 6f63 6b20 257d 223e 0a20 2020 2020 2020  ock %}">.       
+0000a4a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a4b0: 207b 2520 656c 6966 2032 5f6c 6566 745f   {% elif 2_left_
+0000a4c0: 6220 616e 6420 325f 7269 6768 745f 6120  b and 2_right_a 
+0000a4d0: 616e 6420 325f 7269 6768 745f 6220 257d  and 2_right_b %}
+0000a4e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000a4f0: 2020 2020 2020 2020 203c 6469 7620 636c           <div cl
+0000a500: 6173 733d 227b 2520 626c 6f63 6b20 325f  ass="{% block 2_
+0000a510: 6365 6e74 6572 5f6c 6566 745f 625f 7269  center_left_b_ri
+0000a520: 6768 745f 6162 2025 7d63 6f6c 2d31 3220  ght_ab %}col-12 
+0000a530: 636f 6c2d 6c67 2d34 206f 6666 7365 742d  col-lg-4 offset-
+0000a540: 6c67 2d31 7b25 2065 6e64 626c 6f63 6b20  lg-1{% endblock 
+0000a550: 257d 223e 0a20 2020 2020 2020 2020 2020  %}">.           
+0000a560: 2020 2020 2020 2020 2020 2020 207b 2520               {% 
+0000a570: 656c 6966 2032 5f6c 6566 745f 6220 616e  elif 2_left_b an
+0000a580: 6420 325f 7269 6768 745f 6120 257d 0a20  d 2_right_a %}. 
+0000a590: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a5a0: 2020 2020 2020 203c 6469 7620 636c 6173         <div clas
+0000a5b0: 733d 227b 2520 626c 6f63 6b20 325f 6365  s="{% block 2_ce
+0000a5c0: 6e74 6572 5f6c 6566 745f 625f 7269 6768  nter_left_b_righ
+0000a5d0: 745f 6120 257d 636f 6c2d 3132 2063 6f6c  t_a %}col-12 col
+0000a5e0: 2d6c 672d 3520 6f66 6673 6574 2d6c 672d  -lg-5 offset-lg-
+0000a5f0: 317b 2520 656e 6462 6c6f 636b 2025 7d22  1{% endblock %}"
+0000a600: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
+0000a610: 2020 2020 2020 2020 2020 7b25 2065 6c69            {% eli
+0000a620: 6620 325f 6c65 6674 5f62 2061 6e64 2032  f 2_left_b and 2
+0000a630: 5f72 6967 6874 5f62 2025 7d0a 2020 2020  _right_b %}.    
+0000a640: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a650: 2020 2020 3c64 6976 2063 6c61 7373 3d22      <div class="
+0000a660: 7b25 2062 6c6f 636b 2032 5f63 656e 7465  {% block 2_cente
+0000a670: 725f 6c65 6674 5f62 5f72 6967 6874 5f62  r_left_b_right_b
+0000a680: 2025 7d63 6f6c 2d31 3220 636f 6c2d 6c67   %}col-12 col-lg
+0000a690: 2d34 206f 6666 7365 742d 6c67 2d31 7b25  -4 offset-lg-1{%
+0000a6a0: 2065 6e64 626c 6f63 6b20 257d 223e 0a20   endblock %}">. 
+0000a6b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a6c0: 2020 2020 2020 207b 2520 656c 6966 2032         {% elif 2
+0000a6d0: 5f6c 6566 745f 6120 616e 6420 325f 6c65  _left_a and 2_le
+0000a6e0: 6674 5f62 2025 7d0a 2020 2020 2020 2020  ft_b %}.        
+0000a6f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a700: 3c64 6976 2063 6c61 7373 3d22 7b25 2062  <div class="{% b
+0000a710: 6c6f 636b 2032 5f63 656e 7465 725f 6c65  lock 2_center_le
+0000a720: 6674 5f61 6220 257d 636f 6c2d 3132 2063  ft_ab %}col-12 c
+0000a730: 6f6c 2d6c 672d 387b 2520 656e 6462 6c6f  ol-lg-8{% endblo
+0000a740: 636b 2025 7d22 3e0a 2020 2020 2020 2020  ck %}">.        
+0000a750: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a760: 7b25 2065 6c69 6620 325f 6c65 6674 5f61  {% elif 2_left_a
+0000a770: 2025 7d0a 2020 2020 2020 2020 2020 2020   %}.            
+0000a780: 2020 2020 2020 2020 2020 2020 3c64 6976              <div
+0000a790: 2063 6c61 7373 3d22 7b25 2062 6c6f 636b   class="{% block
+0000a7a0: 2032 5f63 656e 7465 725f 6c65 6674 5f61   2_center_left_a
+0000a7b0: 2025 7d63 6f6c 2d31 3220 636f 6c2d 6c67   %}col-12 col-lg
+0000a7c0: 2d39 7b25 2065 6e64 626c 6f63 6b20 257d  -9{% endblock %}
+0000a7d0: 223e 0a20 2020 2020 2020 2020 2020 2020  ">.             
+0000a7e0: 2020 2020 2020 2020 2020 207b 2520 656c             {% el
+0000a7f0: 6966 2032 5f6c 6566 745f 6220 257d 0a20  if 2_left_b %}. 
+0000a800: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a810: 2020 2020 2020 203c 6469 7620 636c 6173         <div clas
+0000a820: 733d 227b 2520 626c 6f63 6b20 325f 6365  s="{% block 2_ce
+0000a830: 6e74 6572 5f6c 6566 745f 6220 257d 636f  nter_left_b %}co
+0000a840: 6c2d 3132 2063 6f6c 2d6c 672d 3820 6f66  l-12 col-lg-8 of
+0000a850: 6673 6574 2d6c 672d 317b 2520 656e 6462  fset-lg-1{% endb
+0000a860: 6c6f 636b 2025 7d22 3e0a 2020 2020 2020  lock %}">.      
+0000a870: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a880: 2020 7b25 2065 6c69 6620 325f 7269 6768    {% elif 2_righ
+0000a890: 745f 6120 616e 6420 325f 7269 6768 745f  t_a and 2_right_
+0000a8a0: 6220 257d 0a20 2020 2020 2020 2020 2020  b %}.           
+0000a8b0: 2020 2020 2020 2020 2020 2020 203c 6469               <di
+0000a8c0: 7620 636c 6173 733d 227b 2520 626c 6f63  v class="{% bloc
+0000a8d0: 6b20 325f 6365 6e74 6572 5f72 6967 6874  k 2_center_right
+0000a8e0: 5f61 6220 257d 636f 6c2d 3132 2063 6f6c  _ab %}col-12 col
+0000a8f0: 2d6c 672d 387b 2520 656e 6462 6c6f 636b  -lg-8{% endblock
+0000a900: 2025 7d22 3e0a 2020 2020 2020 2020 2020   %}">.          
+0000a910: 2020 2020 2020 2020 2020 2020 2020 7b25                {%
+0000a920: 2065 6c69 6620 325f 7269 6768 745f 6120   elif 2_right_a 
+0000a930: 257d 0a20 2020 2020 2020 2020 2020 2020  %}.             
+0000a940: 2020 2020 2020 2020 2020 203c 6469 7620             <div 
+0000a950: 636c 6173 733d 227b 2520 626c 6f63 6b20  class="{% block 
+0000a960: 325f 6365 6e74 6572 5f72 6967 6874 5f61  2_center_right_a
+0000a970: 2025 7d63 6f6c 2d31 3220 636f 6c2d 6c67   %}col-12 col-lg
+0000a980: 2d39 7b25 2065 6e64 626c 6f63 6b20 257d  -9{% endblock %}
+0000a990: 223e 0a20 2020 2020 2020 2020 2020 2020  ">.             
+0000a9a0: 2020 2020 2020 2020 2020 207b 2520 656c             {% el
+0000a9b0: 6966 2032 5f72 6967 6874 5f62 2025 7d0a  if 2_right_b %}.
 0000a9c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a9d0: 2020 2020 2020 7b25 2065 6c69 6620 325f        {% elif 2_
-0000a9e0: 6365 6e74 6572 5f74 6f70 5f61 2061 6e64  center_top_a and
-0000a9f0: 2032 5f63 656e 7465 725f 746f 705f 6220   2_center_top_b 
-0000aa00: 257d 0a20 2020 2020 2020 2020 2020 2020  %}.             
-0000aa10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000aa20: 2020 2020 2020 203c 6469 7620 636c 6173         <div clas
-0000aa30: 733d 227b 2520 626c 6f63 6b20 325f 6365  s="{% block 2_ce
-0000aa40: 6e74 6572 5f74 6f70 5f61 625f 6120 257d  nter_top_ab_a %}
-0000aa50: 636f 6c2d 3132 2063 6f6c 2d6d 642d 387b  col-12 col-md-8{
-0000aa60: 2520 656e 6462 6c6f 636b 2025 7d22 3e7b  % endblock %}">{
-0000aa70: 7b20 325f 6365 6e74 6572 5f74 6f70 5f61  { 2_center_top_a
-0000aa80: 207d 7d3c 2f64 6976 3e0a 2020 2020 2020   }}</div>.      
-0000aa90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000aaa0: 2020 2020 2020 2020 2020 2020 2020 3c64                <d
-0000aab0: 6976 2063 6c61 7373 3d22 7b25 2062 6c6f  iv class="{% blo
-0000aac0: 636b 2032 5f63 656e 7465 725f 746f 705f  ck 2_center_top_
-0000aad0: 6162 5f62 2025 7d63 6f6c 2d31 3220 636f  ab_b %}col-12 co
-0000aae0: 6c2d 6d64 2d34 7b25 2065 6e64 626c 6f63  l-md-4{% endbloc
-0000aaf0: 6b20 257d 223e 7b7b 2032 5f63 656e 7465  k %}">{{ 2_cente
-0000ab00: 725f 746f 705f 6220 7d7d 3c2f 6469 763e  r_top_b }}</div>
-0000ab10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000ab20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ab30: 207b 2520 656c 6966 2032 5f63 656e 7465   {% elif 2_cente
-0000ab40: 725f 746f 705f 6120 616e 6420 325f 6365  r_top_a and 2_ce
-0000ab50: 6e74 6572 5f74 6f70 5f63 2025 7d0a 2020  nter_top_c %}.  
-0000ab60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ab70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ab80: 2020 3c64 6976 2063 6c61 7373 3d22 7b25    <div class="{%
-0000ab90: 2062 6c6f 636b 2032 5f63 656e 7465 725f   block 2_center_
-0000aba0: 746f 705f 6163 5f61 2025 7d63 6f6c 2d31  top_ac_a %}col-1
-0000abb0: 3220 636f 6c2d 6d64 2d36 7b25 2065 6e64  2 col-md-6{% end
-0000abc0: 626c 6f63 6b20 257d 223e 7b7b 2032 5f63  block %}">{{ 2_c
-0000abd0: 656e 7465 725f 746f 705f 6120 7d7d 3c2f  enter_top_a }}</
-0000abe0: 6469 763e 0a20 2020 2020 2020 2020 2020  div>.           
-0000abf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ac00: 2020 2020 2020 2020 203c 6469 7620 636c           <div cl
-0000ac10: 6173 733d 227b 2520 626c 6f63 6b20 325f  ass="{% block 2_
-0000ac20: 6365 6e74 6572 5f74 6f70 5f61 635f 6320  center_top_ac_c 
-0000ac30: 257d 636f 6c2d 3132 2063 6f6c 2d6d 642d  %}col-12 col-md-
-0000ac40: 367b 2520 656e 6462 6c6f 636b 2025 7d22  6{% endblock %}"
-0000ac50: 3e7b 7b20 325f 6365 6e74 6572 5f74 6f70  >{{ 2_center_top
-0000ac60: 5f63 207d 7d3c 2f64 6976 3e0a 2020 2020  _c }}</div>.    
-0000ac70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ac80: 2020 2020 2020 2020 2020 2020 7b25 2065              {% e
-0000ac90: 6c69 6620 325f 6365 6e74 6572 5f74 6f70  lif 2_center_top
-0000aca0: 5f62 2061 6e64 2032 5f63 656e 7465 725f  _b and 2_center_
-0000acb0: 746f 705f 6320 257d 0a20 2020 2020 2020  top_c %}.       
-0000acc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000acd0: 2020 2020 2020 2020 2020 2020 203c 6469               <di
-0000ace0: 7620 636c 6173 733d 227b 2520 626c 6f63  v class="{% bloc
-0000acf0: 6b20 325f 6365 6e74 6572 5f74 6f70 5f62  k 2_center_top_b
-0000ad00: 635f 6220 257d 636f 6c2d 3132 2063 6f6c  c_b %}col-12 col
-0000ad10: 2d6d 642d 347b 2520 656e 6462 6c6f 636b  -md-4{% endblock
-0000ad20: 2025 7d22 3e7b 7b20 325f 6365 6e74 6572   %}">{{ 2_center
-0000ad30: 5f74 6f70 5f62 207d 7d3c 2f64 6976 3e0a  _top_b }}</div>.
+0000a9d0: 2020 2020 2020 2020 3c64 6976 2063 6c61          <div cla
+0000a9e0: 7373 3d22 7b25 2062 6c6f 636b 2032 5f63  ss="{% block 2_c
+0000a9f0: 656e 7465 725f 7269 6768 745f 6220 257d  enter_right_b %}
+0000aa00: 636f 6c2d 3132 2063 6f6c 2d6c 672d 387b  col-12 col-lg-8{
+0000aa10: 2520 656e 6462 6c6f 636b 2025 7d22 3e0a  % endblock %}">.
+0000aa20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000aa30: 2020 2020 2020 2020 7b25 2065 6c73 6520          {% else 
+0000aa40: 257d 0a20 2020 2020 2020 2020 2020 2020  %}.             
+0000aa50: 2020 2020 2020 2020 2020 203c 6469 7620             <div 
+0000aa60: 636c 6173 733d 227b 2520 626c 6f63 6b20  class="{% block 
+0000aa70: 325f 6365 6e74 6572 2025 7d63 6f6c 2d31  2_center %}col-1
+0000aa80: 327b 2520 656e 6462 6c6f 636b 2025 7d22  2{% endblock %}"
+0000aa90: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
+0000aaa0: 2020 2020 2020 2020 2020 7b25 2065 6e64            {% end
+0000aab0: 6966 2025 7d0a 2020 2020 2020 2020 2020  if %}.          
+0000aac0: 2020 2020 2020 2020 2020 2020 2020 3c21                <!
+0000aad0: 2d2d 2045 6e64 2042 6c6f 636b 7320 696e  -- End Blocks in
+0000aae0: 2043 656e 7465 7220 636f 6c75 6d6e 2028   Center column (
+0000aaf0: 7461 6b65 7320 6176 6169 6c61 626c 6520  takes available 
+0000ab00: 7370 6163 6529 202d 2d3e 0a0a 2020 2020  space) -->..    
+0000ab10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ab20: 2020 2020 2020 2020 3c21 2d2d 2043 656e          <!-- Cen
+0000ab30: 7465 7220 746f 7020 2d2d 3e0a 2020 2020  ter top -->.    
+0000ab40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ab50: 2020 2020 2020 2020 7b25 2069 6620 325f          {% if 2_
+0000ab60: 6365 6e74 6572 5f74 6f70 5f61 206f 7220  center_top_a or 
+0000ab70: 325f 6365 6e74 6572 5f74 6f70 5f62 206f  2_center_top_b o
+0000ab80: 7220 325f 6365 6e74 6572 5f74 6f70 5f63  r 2_center_top_c
+0000ab90: 2025 7d0a 2020 2020 2020 2020 2020 2020   %}.            
+0000aba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000abb0: 3c64 6976 2063 6c61 7373 3d22 726f 7722  <div class="row"
+0000abc0: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
+0000abd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000abe0: 2020 7b25 2069 6620 325f 6365 6e74 6572    {% if 2_center
+0000abf0: 5f74 6f70 5f61 2061 6e64 2032 5f63 656e  _top_a and 2_cen
+0000ac00: 7465 725f 746f 705f 6220 616e 6420 325f  ter_top_b and 2_
+0000ac10: 6365 6e74 6572 5f74 6f70 5f63 2025 7d0a  center_top_c %}.
+0000ac20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ac30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ac40: 2020 2020 3c64 6976 2063 6c61 7373 3d22      <div class="
+0000ac50: 7b25 2062 6c6f 636b 2032 5f63 656e 7465  {% block 2_cente
+0000ac60: 725f 746f 705f 6162 635f 6120 257d 636f  r_top_abc_a %}co
+0000ac70: 6c2d 3132 2063 6f6c 2d6d 642d 347b 2520  l-12 col-md-4{% 
+0000ac80: 656e 6462 6c6f 636b 2025 7d22 3e7b 7b20  endblock %}">{{ 
+0000ac90: 325f 6365 6e74 6572 5f74 6f70 5f61 207d  2_center_top_a }
+0000aca0: 7d3c 2f64 6976 3e0a 2020 2020 2020 2020  }</div>.        
+0000acb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000acc0: 2020 2020 2020 2020 2020 2020 3c64 6976              <div
+0000acd0: 2063 6c61 7373 3d22 7b25 2062 6c6f 636b   class="{% block
+0000ace0: 2032 5f63 656e 7465 725f 746f 705f 6162   2_center_top_ab
+0000acf0: 635f 6220 257d 636f 6c2d 3132 2063 6f6c  c_b %}col-12 col
+0000ad00: 2d6d 642d 347b 2520 656e 6462 6c6f 636b  -md-4{% endblock
+0000ad10: 2025 7d22 3e7b 7b20 325f 6365 6e74 6572   %}">{{ 2_center
+0000ad20: 5f74 6f70 5f62 207d 7d3c 2f64 6976 3e0a  _top_b }}</div>.
+0000ad30: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000ad40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ad50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ad60: 2020 2020 3c64 6976 2063 6c61 7373 3d22      <div class="
-0000ad70: 7b25 2062 6c6f 636b 2032 5f63 656e 7465  {% block 2_cente
-0000ad80: 725f 746f 705f 6263 5f63 2025 7d63 6f6c  r_top_bc_c %}col
-0000ad90: 2d31 3220 636f 6c2d 6d64 2d38 7b25 2065  -12 col-md-8{% e
-0000ada0: 6e64 626c 6f63 6b20 257d 223e 7b7b 2032  ndblock %}">{{ 2
-0000adb0: 5f63 656e 7465 725f 746f 705f 6320 7d7d  _center_top_c }}
-0000adc0: 3c2f 6469 763e 0a20 2020 2020 2020 2020  </div>.         
-0000add0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ade0: 2020 2020 2020 207b 2520 656c 7365 2025         {% else %
-0000adf0: 7d0a 2020 2020 2020 2020 2020 2020 2020  }.              
-0000ae00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ae10: 2020 2020 2020 3c64 6976 2063 6c61 7373        <div class
-0000ae20: 3d22 636f 6c2d 3132 223e 7b7b 2032 5f63  ="col-12">{{ 2_c
-0000ae30: 656e 7465 725f 746f 705f 6120 7d7d 7b7b  enter_top_a }}{{
-0000ae40: 2032 5f63 656e 7465 725f 746f 705f 6220   2_center_top_b 
-0000ae50: 7d7d 7b7b 2032 5f63 656e 7465 725f 746f  }}{{ 2_center_to
-0000ae60: 705f 6320 7d7d 3c2f 6469 763e 0a20 2020  p_c }}</div>.   
-0000ae70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ae80: 2020 2020 2020 2020 2020 2020 207b 2520               {% 
-0000ae90: 656e 6469 6620 257d 0a20 2020 2020 2020  endif %}.       
+0000ad50: 2020 2020 3c64 6976 2063 6c61 7373 3d22      <div class="
+0000ad60: 7b25 2062 6c6f 636b 2032 5f63 656e 7465  {% block 2_cente
+0000ad70: 725f 746f 705f 6162 635f 6320 257d 636f  r_top_abc_c %}co
+0000ad80: 6c2d 3132 2063 6f6c 2d6d 642d 347b 2520  l-12 col-md-4{% 
+0000ad90: 656e 6462 6c6f 636b 2025 7d22 3e7b 7b20  endblock %}">{{ 
+0000ada0: 325f 6365 6e74 6572 5f74 6f70 5f63 207d  2_center_top_c }
+0000adb0: 7d3c 2f64 6976 3e0a 2020 2020 2020 2020  }</div>.        
+0000adc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000add0: 2020 2020 2020 2020 7b25 2065 6c69 6620          {% elif 
+0000ade0: 325f 6365 6e74 6572 5f74 6f70 5f61 2061  2_center_top_a a
+0000adf0: 6e64 2032 5f63 656e 7465 725f 746f 705f  nd 2_center_top_
+0000ae00: 6220 257d 0a20 2020 2020 2020 2020 2020  b %}.           
+0000ae10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ae20: 2020 2020 2020 2020 203c 6469 7620 636c           <div cl
+0000ae30: 6173 733d 227b 2520 626c 6f63 6b20 325f  ass="{% block 2_
+0000ae40: 6365 6e74 6572 5f74 6f70 5f61 625f 6120  center_top_ab_a 
+0000ae50: 257d 636f 6c2d 3132 2063 6f6c 2d6d 642d  %}col-12 col-md-
+0000ae60: 387b 2520 656e 6462 6c6f 636b 2025 7d22  8{% endblock %}"
+0000ae70: 3e7b 7b20 325f 6365 6e74 6572 5f74 6f70  >{{ 2_center_top
+0000ae80: 5f61 207d 7d3c 2f64 6976 3e0a 2020 2020  _a }}</div>.    
+0000ae90: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000aea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000aeb0: 2020 2020 203c 2f64 6976 3e0a 2020 2020       </div>.    
-0000aec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000aed0: 2020 2020 2020 2020 7b25 2065 6e64 6966          {% endif
-0000aee0: 2025 7d0a 2020 2020 2020 2020 2020 2020   %}.            
-0000aef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000af00: 3c21 2d2d 2045 4e44 2043 656e 7465 7220  <!-- END Center 
-0000af10: 746f 7020 2d2d 3e0a 0a20 2020 2020 2020  top -->..       
+0000aeb0: 3c64 6976 2063 6c61 7373 3d22 7b25 2062  <div class="{% b
+0000aec0: 6c6f 636b 2032 5f63 656e 7465 725f 746f  lock 2_center_to
+0000aed0: 705f 6162 5f62 2025 7d63 6f6c 2d31 3220  p_ab_b %}col-12 
+0000aee0: 636f 6c2d 6d64 2d34 7b25 2065 6e64 626c  col-md-4{% endbl
+0000aef0: 6f63 6b20 257d 223e 7b7b 2032 5f63 656e  ock %}">{{ 2_cen
+0000af00: 7465 725f 746f 705f 6220 7d7d 3c2f 6469  ter_top_b }}</di
+0000af10: 763e 0a20 2020 2020 2020 2020 2020 2020  v>.             
 0000af20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000af30: 2020 2020 203c 212d 2d20 4365 6e74 6572       <!-- Center
-0000af40: 206d 6964 2d74 6f70 202d 2d3e 0a20 2020   mid-top -->.   
-0000af50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000af60: 2020 2020 2020 2020 207b 2520 6966 2032           {% if 2
-0000af70: 5f63 656e 7465 725f 6d69 645f 746f 705f  _center_mid_top_
-0000af80: 6120 6f72 2032 5f63 656e 7465 725f 6d69  a or 2_center_mi
-0000af90: 645f 746f 705f 6220 6f72 2032 5f63 656e  d_top_b or 2_cen
-0000afa0: 7465 725f 746f 705f 6320 257d 0a20 2020  ter_top_c %}.   
-0000afb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000afc0: 2020 2020 2020 2020 203c 6469 7620 636c           <div cl
-0000afd0: 6173 733d 2272 6f77 223e 0a20 2020 2020  ass="row">.     
-0000afe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000aff0: 2020 2020 2020 2020 2020 207b 2520 6966             {% if
-0000b000: 2032 5f63 656e 7465 725f 6d69 645f 746f   2_center_mid_to
-0000b010: 705f 6120 616e 6420 325f 6365 6e74 6572  p_a and 2_center
-0000b020: 5f6d 6964 5f74 6f70 5f62 2061 6e64 2032  _mid_top_b and 2
-0000b030: 5f63 656e 7465 725f 6d69 645f 746f 705f  _center_mid_top_
-0000b040: 6320 257d 0a20 2020 2020 2020 2020 2020  c %}.           
-0000b050: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b060: 2020 2020 2020 2020 203c 6469 7620 636c           <div cl
-0000b070: 6173 733d 227b 2520 626c 6f63 6b20 325f  ass="{% block 2_
-0000b080: 6365 6e74 6572 5f6d 6964 5f74 6f70 5f61  center_mid_top_a
-0000b090: 6263 5f61 2025 7d63 6f6c 2d31 3220 636f  bc_a %}col-12 co
-0000b0a0: 6c2d 6d64 2d34 7b25 2065 6e64 626c 6f63  l-md-4{% endbloc
-0000b0b0: 6b20 257d 223e 7b7b 2032 5f63 656e 7465  k %}">{{ 2_cente
-0000b0c0: 725f 6d69 645f 746f 705f 6120 7d7d 3c2f  r_mid_top_a }}</
-0000b0d0: 6469 763e 0a20 2020 2020 2020 2020 2020  div>.           
-0000b0e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b0f0: 2020 2020 2020 2020 203c 6469 7620 636c           <div cl
-0000b100: 6173 733d 227b 2520 626c 6f63 6b20 325f  ass="{% block 2_
-0000b110: 6365 6e74 6572 5f6d 6964 5f74 6f70 5f61  center_mid_top_a
-0000b120: 6263 5f62 2025 7d63 6f6c 2d31 3220 636f  bc_b %}col-12 co
-0000b130: 6c2d 6d64 2d34 7b25 2065 6e64 626c 6f63  l-md-4{% endbloc
-0000b140: 6b20 257d 223e 7b7b 2032 5f63 656e 7465  k %}">{{ 2_cente
-0000b150: 725f 6d69 645f 746f 705f 6220 7d7d 3c2f  r_mid_top_b }}</
-0000b160: 6469 763e 0a20 2020 2020 2020 2020 2020  div>.           
-0000b170: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b180: 2020 2020 2020 2020 203c 6469 7620 636c           <div cl
-0000b190: 6173 733d 227b 2520 626c 6f63 6b20 325f  ass="{% block 2_
-0000b1a0: 6365 6e74 6572 5f6d 6964 5f74 6f70 5f61  center_mid_top_a
-0000b1b0: 6263 5f63 2025 7d63 6f6c 2d31 3220 636f  bc_c %}col-12 co
-0000b1c0: 6c2d 6d64 2d34 7b25 2065 6e64 626c 6f63  l-md-4{% endbloc
-0000b1d0: 6b20 257d 223e 7b7b 2032 5f63 656e 7465  k %}">{{ 2_cente
-0000b1e0: 725f 6d69 645f 746f 705f 6320 7d7d 3c2f  r_mid_top_c }}</
-0000b1f0: 6469 763e 0a20 2020 2020 2020 2020 2020  div>.           
+0000af30: 2020 207b 2520 656c 6966 2032 5f63 656e     {% elif 2_cen
+0000af40: 7465 725f 746f 705f 6120 616e 6420 325f  ter_top_a and 2_
+0000af50: 6365 6e74 6572 5f74 6f70 5f63 2025 7d0a  center_top_c %}.
+0000af60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000af70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000af80: 2020 2020 3c64 6976 2063 6c61 7373 3d22      <div class="
+0000af90: 7b25 2062 6c6f 636b 2032 5f63 656e 7465  {% block 2_cente
+0000afa0: 725f 746f 705f 6163 5f61 2025 7d63 6f6c  r_top_ac_a %}col
+0000afb0: 2d31 3220 636f 6c2d 6d64 2d36 7b25 2065  -12 col-md-6{% e
+0000afc0: 6e64 626c 6f63 6b20 257d 223e 7b7b 2032  ndblock %}">{{ 2
+0000afd0: 5f63 656e 7465 725f 746f 705f 6120 7d7d  _center_top_a }}
+0000afe0: 3c2f 6469 763e 0a20 2020 2020 2020 2020  </div>.         
+0000aff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b000: 2020 2020 2020 2020 2020 203c 6469 7620             <div 
+0000b010: 636c 6173 733d 227b 2520 626c 6f63 6b20  class="{% block 
+0000b020: 325f 6365 6e74 6572 5f74 6f70 5f61 635f  2_center_top_ac_
+0000b030: 6320 257d 636f 6c2d 3132 2063 6f6c 2d6d  c %}col-12 col-m
+0000b040: 642d 367b 2520 656e 6462 6c6f 636b 2025  d-6{% endblock %
+0000b050: 7d22 3e7b 7b20 325f 6365 6e74 6572 5f74  }">{{ 2_center_t
+0000b060: 6f70 5f63 207d 7d3c 2f64 6976 3e0a 2020  op_c }}</div>.  
+0000b070: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b080: 2020 2020 2020 2020 2020 2020 2020 7b25                {%
+0000b090: 2065 6c69 6620 325f 6365 6e74 6572 5f74   elif 2_center_t
+0000b0a0: 6f70 5f62 2061 6e64 2032 5f63 656e 7465  op_b and 2_cente
+0000b0b0: 725f 746f 705f 6320 257d 0a20 2020 2020  r_top_c %}.     
+0000b0c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b0d0: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+0000b0e0: 6469 7620 636c 6173 733d 227b 2520 626c  div class="{% bl
+0000b0f0: 6f63 6b20 325f 6365 6e74 6572 5f74 6f70  ock 2_center_top
+0000b100: 5f62 635f 6220 257d 636f 6c2d 3132 2063  _bc_b %}col-12 c
+0000b110: 6f6c 2d6d 642d 347b 2520 656e 6462 6c6f  ol-md-4{% endblo
+0000b120: 636b 2025 7d22 3e7b 7b20 325f 6365 6e74  ck %}">{{ 2_cent
+0000b130: 6572 5f74 6f70 5f62 207d 7d3c 2f64 6976  er_top_b }}</div
+0000b140: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
+0000b150: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b160: 2020 2020 2020 3c64 6976 2063 6c61 7373        <div class
+0000b170: 3d22 7b25 2062 6c6f 636b 2032 5f63 656e  ="{% block 2_cen
+0000b180: 7465 725f 746f 705f 6263 5f63 2025 7d63  ter_top_bc_c %}c
+0000b190: 6f6c 2d31 3220 636f 6c2d 6d64 2d38 7b25  ol-12 col-md-8{%
+0000b1a0: 2065 6e64 626c 6f63 6b20 257d 223e 7b7b   endblock %}">{{
+0000b1b0: 2032 5f63 656e 7465 725f 746f 705f 6320   2_center_top_c 
+0000b1c0: 7d7d 3c2f 6469 763e 0a20 2020 2020 2020  }}</div>.       
+0000b1d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b1e0: 2020 2020 2020 2020 207b 2520 656c 7365           {% else
+0000b1f0: 2025 7d0a 2020 2020 2020 2020 2020 2020   %}.            
 0000b200: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b210: 2020 2020 207b 2520 656c 6966 2032 5f63       {% elif 2_c
-0000b220: 656e 7465 725f 6d69 645f 746f 705f 6120  enter_mid_top_a 
-0000b230: 616e 6420 325f 6365 6e74 6572 5f6d 6964  and 2_center_mid
-0000b240: 5f74 6f70 5f62 2025 7d0a 2020 2020 2020  _top_b %}.      
-0000b250: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b260: 2020 2020 2020 2020 2020 2020 2020 3c64                <d
-0000b270: 6976 2063 6c61 7373 3d22 7b25 2062 6c6f  iv class="{% blo
-0000b280: 636b 2032 5f63 656e 7465 725f 6d69 645f  ck 2_center_mid_
-0000b290: 746f 705f 6162 5f61 2025 7d63 6f6c 2d31  top_ab_a %}col-1
-0000b2a0: 3220 636f 6c2d 6d64 2d38 7b25 2065 6e64  2 col-md-8{% end
-0000b2b0: 626c 6f63 6b20 257d 223e 7b7b 2032 5f63  block %}">{{ 2_c
-0000b2c0: 656e 7465 725f 6d69 645f 746f 705f 6120  enter_mid_top_a 
-0000b2d0: 7d7d 3c2f 6469 763e 0a20 2020 2020 2020  }}</div>.       
-0000b2e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b2f0: 2020 2020 2020 2020 2020 2020 203c 6469               <di
-0000b300: 7620 636c 6173 733d 227b 2520 626c 6f63  v class="{% bloc
-0000b310: 6b20 325f 6365 6e74 6572 5f6d 6964 5f74  k 2_center_mid_t
-0000b320: 6f70 5f61 625f 6220 257d 636f 6c2d 3132  op_ab_b %}col-12
-0000b330: 2063 6f6c 2d6d 642d 347b 2520 656e 6462   col-md-4{% endb
-0000b340: 6c6f 636b 2025 7d22 3e7b 7b20 325f 6365  lock %}">{{ 2_ce
-0000b350: 6e74 6572 5f6d 6964 5f74 6f70 5f62 207d  nter_mid_top_b }
-0000b360: 7d3c 2f64 6976 3e0a 2020 2020 2020 2020  }</div>.        
-0000b370: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b380: 2020 2020 2020 2020 7b25 2065 6c69 6620          {% elif 
-0000b390: 325f 6365 6e74 6572 5f6d 6964 5f74 6f70  2_center_mid_top
-0000b3a0: 5f61 2061 6e64 2032 5f63 656e 7465 725f  _a and 2_center_
-0000b3b0: 6d69 645f 746f 705f 6320 257d 0a20 2020  mid_top_c %}.   
-0000b3c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b3d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b3e0: 203c 6469 7620 636c 6173 733d 227b 2520   <div class="{% 
-0000b3f0: 626c 6f63 6b20 325f 6365 6e74 6572 5f6d  block 2_center_m
-0000b400: 6964 5f74 6f70 5f61 635f 6120 257d 636f  id_top_ac_a %}co
-0000b410: 6c2d 3132 2063 6f6c 2d6d 642d 367b 2520  l-12 col-md-6{% 
-0000b420: 656e 6462 6c6f 636b 2025 7d22 3e7b 7b20  endblock %}">{{ 
-0000b430: 325f 6365 6e74 6572 5f6d 6964 5f74 6f70  2_center_mid_top
-0000b440: 5f61 207d 7d3c 2f64 6976 3e0a 2020 2020  _a }}</div>.    
+0000b210: 2020 2020 2020 2020 3c64 6976 2063 6c61          <div cla
+0000b220: 7373 3d22 636f 6c2d 3132 223e 7b7b 2032  ss="col-12">{{ 2
+0000b230: 5f63 656e 7465 725f 746f 705f 6120 7d7d  _center_top_a }}
+0000b240: 7b7b 2032 5f63 656e 7465 725f 746f 705f  {{ 2_center_top_
+0000b250: 6220 7d7d 7b7b 2032 5f63 656e 7465 725f  b }}{{ 2_center_
+0000b260: 746f 705f 6320 7d7d 3c2f 6469 763e 0a20  top_c }}</div>. 
+0000b270: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b280: 2020 2020 2020 2020 2020 2020 2020 207b                 {
+0000b290: 2520 656e 6469 6620 257d 0a20 2020 2020  % endif %}.     
+0000b2a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b2b0: 2020 2020 2020 203c 2f64 6976 3e0a 2020         </div>.  
+0000b2c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b2d0: 2020 2020 2020 2020 2020 7b25 2065 6e64            {% end
+0000b2e0: 6966 2025 7d0a 2020 2020 2020 2020 2020  if %}.          
+0000b2f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b300: 2020 3c21 2d2d 2045 4e44 2043 656e 7465    <!-- END Cente
+0000b310: 7220 746f 7020 2d2d 3e0a 0a20 2020 2020  r top -->..     
+0000b320: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b330: 2020 2020 2020 203c 212d 2d20 4365 6e74         <!-- Cent
+0000b340: 6572 206d 6964 2d74 6f70 202d 2d3e 0a20  er mid-top -->. 
+0000b350: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b360: 2020 2020 2020 2020 2020 207b 2520 6966             {% if
+0000b370: 2032 5f63 656e 7465 725f 6d69 645f 746f   2_center_mid_to
+0000b380: 705f 6120 6f72 2032 5f63 656e 7465 725f  p_a or 2_center_
+0000b390: 6d69 645f 746f 705f 6220 6f72 2032 5f63  mid_top_b or 2_c
+0000b3a0: 656e 7465 725f 746f 705f 6320 257d 0a20  enter_top_c %}. 
+0000b3b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b3c0: 2020 2020 2020 2020 2020 203c 6469 7620             <div 
+0000b3d0: 636c 6173 733d 2272 6f77 223e 0a20 2020  class="row">.   
+0000b3e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b3f0: 2020 2020 2020 2020 2020 2020 207b 2520               {% 
+0000b400: 6966 2032 5f63 656e 7465 725f 6d69 645f  if 2_center_mid_
+0000b410: 746f 705f 6120 616e 6420 325f 6365 6e74  top_a and 2_cent
+0000b420: 6572 5f6d 6964 5f74 6f70 5f62 2061 6e64  er_mid_top_b and
+0000b430: 2032 5f63 656e 7465 725f 6d69 645f 746f   2_center_mid_to
+0000b440: 705f 6320 257d 0a20 2020 2020 2020 2020  p_c %}.         
 0000b450: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b460: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b470: 3c64 6976 2063 6c61 7373 3d22 7b25 2062  <div class="{% b
-0000b480: 6c6f 636b 2032 5f63 656e 7465 725f 6d69  lock 2_center_mi
-0000b490: 645f 746f 705f 6163 5f63 2025 7d63 6f6c  d_top_ac_c %}col
-0000b4a0: 2d31 3220 636f 6c2d 6d64 2d36 7b25 2065  -12 col-md-6{% e
-0000b4b0: 6e64 626c 6f63 6b20 257d 223e 7b7b 2032  ndblock %}">{{ 2
-0000b4c0: 5f63 656e 7465 725f 6d69 645f 746f 705f  _center_mid_top_
-0000b4d0: 6320 7d7d 3c2f 6469 763e 0a20 2020 2020  c }}</div>.     
+0000b460: 2020 2020 2020 2020 2020 203c 6469 7620             <div 
+0000b470: 636c 6173 733d 227b 2520 626c 6f63 6b20  class="{% block 
+0000b480: 325f 6365 6e74 6572 5f6d 6964 5f74 6f70  2_center_mid_top
+0000b490: 5f61 6263 5f61 2025 7d63 6f6c 2d31 3220  _abc_a %}col-12 
+0000b4a0: 636f 6c2d 6d64 2d34 7b25 2065 6e64 626c  col-md-4{% endbl
+0000b4b0: 6f63 6b20 257d 223e 7b7b 2032 5f63 656e  ock %}">{{ 2_cen
+0000b4c0: 7465 725f 6d69 645f 746f 705f 6120 7d7d  ter_mid_top_a }}
+0000b4d0: 3c2f 6469 763e 0a20 2020 2020 2020 2020  </div>.         
 0000b4e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b4f0: 2020 2020 2020 2020 2020 207b 2520 656c             {% el
-0000b500: 6966 2032 5f63 656e 7465 725f 6d69 645f  if 2_center_mid_
-0000b510: 746f 705f 6220 616e 6420 325f 6365 6e74  top_b and 2_cent
-0000b520: 6572 5f6d 6964 5f74 6f70 5f63 2025 7d0a  er_mid_top_c %}.
-0000b530: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b540: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b550: 2020 2020 3c64 6976 2063 6c61 7373 3d22      <div class="
-0000b560: 7b25 2062 6c6f 636b 2032 5f63 656e 7465  {% block 2_cente
-0000b570: 725f 6d69 645f 746f 705f 6263 5f62 2025  r_mid_top_bc_b %
-0000b580: 7d63 6f6c 2d31 3220 636f 6c2d 6d64 2d34  }col-12 col-md-4
-0000b590: 7b25 2065 6e64 626c 6f63 6b20 257d 223e  {% endblock %}">
-0000b5a0: 7b7b 2032 5f63 656e 7465 725f 6d69 645f  {{ 2_center_mid_
-0000b5b0: 746f 705f 6220 7d7d 3c2f 6469 763e 0a20  top_b }}</div>. 
-0000b5c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b5d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b5e0: 2020 203c 6469 7620 636c 6173 733d 227b     <div class="{
-0000b5f0: 2520 626c 6f63 6b20 325f 6365 6e74 6572  % block 2_center
-0000b600: 5f6d 6964 5f74 6f70 5f62 635f 6320 257d  _mid_top_bc_c %}
-0000b610: 636f 6c2d 3132 2063 6f6c 2d6d 642d 387b  col-12 col-md-8{
-0000b620: 2520 656e 6462 6c6f 636b 2025 7d22 3e7b  % endblock %}">{
-0000b630: 7b20 325f 6365 6e74 6572 5f6d 6964 5f74  { 2_center_mid_t
-0000b640: 6f70 5f63 207d 7d3c 2f64 6976 3e0a 2020  op_c }}</div>.  
+0000b4f0: 2020 2020 2020 2020 2020 203c 6469 7620             <div 
+0000b500: 636c 6173 733d 227b 2520 626c 6f63 6b20  class="{% block 
+0000b510: 325f 6365 6e74 6572 5f6d 6964 5f74 6f70  2_center_mid_top
+0000b520: 5f61 6263 5f62 2025 7d63 6f6c 2d31 3220  _abc_b %}col-12 
+0000b530: 636f 6c2d 6d64 2d34 7b25 2065 6e64 626c  col-md-4{% endbl
+0000b540: 6f63 6b20 257d 223e 7b7b 2032 5f63 656e  ock %}">{{ 2_cen
+0000b550: 7465 725f 6d69 645f 746f 705f 6220 7d7d  ter_mid_top_b }}
+0000b560: 3c2f 6469 763e 0a20 2020 2020 2020 2020  </div>.         
+0000b570: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b580: 2020 2020 2020 2020 2020 203c 6469 7620             <div 
+0000b590: 636c 6173 733d 227b 2520 626c 6f63 6b20  class="{% block 
+0000b5a0: 325f 6365 6e74 6572 5f6d 6964 5f74 6f70  2_center_mid_top
+0000b5b0: 5f61 6263 5f63 2025 7d63 6f6c 2d31 3220  _abc_c %}col-12 
+0000b5c0: 636f 6c2d 6d64 2d34 7b25 2065 6e64 626c  col-md-4{% endbl
+0000b5d0: 6f63 6b20 257d 223e 7b7b 2032 5f63 656e  ock %}">{{ 2_cen
+0000b5e0: 7465 725f 6d69 645f 746f 705f 6320 7d7d  ter_mid_top_c }}
+0000b5f0: 3c2f 6469 763e 0a20 2020 2020 2020 2020  </div>.         
+0000b600: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b610: 2020 2020 2020 207b 2520 656c 6966 2032         {% elif 2
+0000b620: 5f63 656e 7465 725f 6d69 645f 746f 705f  _center_mid_top_
+0000b630: 6120 616e 6420 325f 6365 6e74 6572 5f6d  a and 2_center_m
+0000b640: 6964 5f74 6f70 5f62 2025 7d0a 2020 2020  id_top_b %}.    
 0000b650: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b660: 2020 2020 2020 2020 2020 2020 2020 7b25                {%
-0000b670: 2065 6c73 6520 257d 0a20 2020 2020 2020   else %}.       
-0000b680: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b690: 2020 2020 2020 2020 2020 2020 203c 6469               <di
-0000b6a0: 7620 636c 6173 733d 2263 6f6c 2d31 3222  v class="col-12"
-0000b6b0: 3e7b 7b20 325f 6365 6e74 6572 5f6d 6964  >{{ 2_center_mid
-0000b6c0: 5f74 6f70 5f61 207d 7d7b 7b20 325f 6365  _top_a }}{{ 2_ce
-0000b6d0: 6e74 6572 5f6d 6964 5f74 6f70 5f62 207d  nter_mid_top_b }
-0000b6e0: 7d7b 7b20 325f 6365 6e74 6572 5f6d 6964  }{{ 2_center_mid
-0000b6f0: 5f74 6f70 5f63 207d 7d3c 2f64 6976 3e0a  _top_c }}</div>.
-0000b700: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b710: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b720: 7b25 2065 6e64 6966 2025 7d0a 2020 2020  {% endif %}.    
-0000b730: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b740: 2020 2020 2020 2020 3c2f 6469 763e 0a20          </div>. 
-0000b750: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b760: 2020 2020 2020 2020 2020 207b 2520 656e             {% en
-0000b770: 6469 6620 257d 0a20 2020 2020 2020 2020  dif %}.         
-0000b780: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b790: 2020 203c 212d 2d20 454e 4420 4365 6e74     <!-- END Cent
-0000b7a0: 6572 206d 6964 2d74 6f70 202d 2d3e 0a0a  er mid-top -->..
-0000b7b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b7c0: 2020 2020 2020 2020 2020 2020 3c21 2d2d              <!--
-0000b7d0: 2043 656e 7465 7220 636f 6e74 656e 7420   Center content 
-0000b7e0: 2d2d 3e0a 2020 2020 2020 2020 2020 2020  -->.            
-0000b7f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b800: 7b25 2069 6620 325f 6365 6e74 6572 5f63  {% if 2_center_c
-0000b810: 6f6e 7465 6e74 2025 7d0a 2020 2020 2020  ontent %}.      
-0000b820: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b830: 2020 2020 2020 3c64 6976 2063 6c61 7373        <div class
-0000b840: 3d22 726f 7722 3e0a 2020 2020 2020 2020  ="row">.        
+0000b660: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b670: 3c64 6976 2063 6c61 7373 3d22 7b25 2062  <div class="{% b
+0000b680: 6c6f 636b 2032 5f63 656e 7465 725f 6d69  lock 2_center_mi
+0000b690: 645f 746f 705f 6162 5f61 2025 7d63 6f6c  d_top_ab_a %}col
+0000b6a0: 2d31 3220 636f 6c2d 6d64 2d38 7b25 2065  -12 col-md-8{% e
+0000b6b0: 6e64 626c 6f63 6b20 257d 223e 7b7b 2032  ndblock %}">{{ 2
+0000b6c0: 5f63 656e 7465 725f 6d69 645f 746f 705f  _center_mid_top_
+0000b6d0: 6120 7d7d 3c2f 6469 763e 0a20 2020 2020  a }}</div>.     
+0000b6e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b6f0: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+0000b700: 6469 7620 636c 6173 733d 227b 2520 626c  div class="{% bl
+0000b710: 6f63 6b20 325f 6365 6e74 6572 5f6d 6964  ock 2_center_mid
+0000b720: 5f74 6f70 5f61 625f 6220 257d 636f 6c2d  _top_ab_b %}col-
+0000b730: 3132 2063 6f6c 2d6d 642d 347b 2520 656e  12 col-md-4{% en
+0000b740: 6462 6c6f 636b 2025 7d22 3e7b 7b20 325f  dblock %}">{{ 2_
+0000b750: 6365 6e74 6572 5f6d 6964 5f74 6f70 5f62  center_mid_top_b
+0000b760: 207d 7d3c 2f64 6976 3e0a 2020 2020 2020   }}</div>.      
+0000b770: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b780: 2020 2020 2020 2020 2020 7b25 2065 6c69            {% eli
+0000b790: 6620 325f 6365 6e74 6572 5f6d 6964 5f74  f 2_center_mid_t
+0000b7a0: 6f70 5f61 2061 6e64 2032 5f63 656e 7465  op_a and 2_cente
+0000b7b0: 725f 6d69 645f 746f 705f 6320 257d 0a20  r_mid_top_c %}. 
+0000b7c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b7d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b7e0: 2020 203c 6469 7620 636c 6173 733d 227b     <div class="{
+0000b7f0: 2520 626c 6f63 6b20 325f 6365 6e74 6572  % block 2_center
+0000b800: 5f6d 6964 5f74 6f70 5f61 635f 6120 257d  _mid_top_ac_a %}
+0000b810: 636f 6c2d 3132 2063 6f6c 2d6d 642d 367b  col-12 col-md-6{
+0000b820: 2520 656e 6462 6c6f 636b 2025 7d22 3e7b  % endblock %}">{
+0000b830: 7b20 325f 6365 6e74 6572 5f6d 6964 5f74  { 2_center_mid_t
+0000b840: 6f70 5f61 207d 7d3c 2f64 6976 3e0a 2020  op_a }}</div>.  
 0000b850: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b860: 2020 2020 2020 2020 3c64 6976 2063 6c61          <div cla
-0000b870: 7373 3d22 636f 6c22 3e0a 2020 2020 2020  ss="col">.      
-0000b880: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b890: 2020 2020 2020 2020 2020 2020 2020 7b7b                {{
-0000b8a0: 2032 5f63 656e 7465 725f 636f 6e74 656e   2_center_conten
-0000b8b0: 7420 7d7d 0a20 2020 2020 2020 2020 2020  t }}.           
-0000b8c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b8d0: 2020 2020 203c 2f64 6976 3e0a 2020 2020       </div>.    
+0000b860: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b870: 2020 3c64 6976 2063 6c61 7373 3d22 7b25    <div class="{%
+0000b880: 2062 6c6f 636b 2032 5f63 656e 7465 725f   block 2_center_
+0000b890: 6d69 645f 746f 705f 6163 5f63 2025 7d63  mid_top_ac_c %}c
+0000b8a0: 6f6c 2d31 3220 636f 6c2d 6d64 2d36 7b25  ol-12 col-md-6{%
+0000b8b0: 2065 6e64 626c 6f63 6b20 257d 223e 7b7b   endblock %}">{{
+0000b8c0: 2032 5f63 656e 7465 725f 6d69 645f 746f   2_center_mid_to
+0000b8d0: 705f 6320 7d7d 3c2f 6469 763e 0a20 2020  p_c }}</div>.   
 0000b8e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b8f0: 2020 2020 2020 2020 3c2f 6469 763e 0a20          </div>. 
-0000b900: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b910: 2020 2020 2020 2020 2020 207b 2520 656e             {% en
-0000b920: 6469 6620 257d 0a20 2020 2020 2020 2020  dif %}.         
-0000b930: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b940: 2020 203c 212d 2d20 454e 4420 4365 6e74     <!-- END Cent
-0000b950: 6572 2063 6f6e 7465 6e74 202d 2d3e 0a0a  er content -->..
-0000b960: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b970: 2020 2020 2020 2020 2020 2020 3c21 2d2d              <!--
-0000b980: 2043 656e 7465 7220 6d69 642d 626f 7474   Center mid-bott
-0000b990: 6f6d 202d 2d3e 0a20 2020 2020 2020 2020  om -->.         
-0000b9a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b9b0: 2020 207b 2520 6966 2032 5f63 656e 7465     {% if 2_cente
-0000b9c0: 725f 6d69 645f 626f 7474 6f6d 5f61 206f  r_mid_bottom_a o
-0000b9d0: 7220 325f 6365 6e74 6572 5f6d 6964 5f62  r 2_center_mid_b
-0000b9e0: 6f74 746f 6d5f 6220 6f72 2032 5f63 656e  ottom_b or 2_cen
-0000b9f0: 7465 725f 6d69 645f 626f 7474 6f6d 5f63  ter_mid_bottom_c
-0000ba00: 2025 7d0a 2020 2020 2020 2020 2020 2020   %}.            
-0000ba10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ba20: 3c64 6976 2063 6c61 7373 3d22 726f 7722  <div class="row"
-0000ba30: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
-0000ba40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ba50: 2020 7b25 2069 6620 325f 6365 6e74 6572    {% if 2_center
-0000ba60: 5f6d 6964 5f62 6f74 746f 6d5f 6120 616e  _mid_bottom_a an
-0000ba70: 6420 325f 6365 6e74 6572 5f6d 6964 5f62  d 2_center_mid_b
-0000ba80: 6f74 746f 6d5f 6220 616e 6420 325f 6365  ottom_b and 2_ce
-0000ba90: 6e74 6572 5f6d 6964 5f62 6f74 746f 6d5f  nter_mid_bottom_
-0000baa0: 6320 257d 0a20 2020 2020 2020 2020 2020  c %}.           
-0000bab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bac0: 2020 2020 2020 2020 203c 6469 7620 636c           <div cl
-0000bad0: 6173 733d 227b 2520 626c 6f63 6b20 325f  ass="{% block 2_
-0000bae0: 6365 6e74 6572 5f6d 6964 5f62 6f74 746f  center_mid_botto
-0000baf0: 6d5f 6162 635f 6120 257d 636f 6c2d 3132  m_abc_a %}col-12
-0000bb00: 2063 6f6c 2d6d 642d 347b 2520 656e 6462   col-md-4{% endb
-0000bb10: 6c6f 636b 2025 7d22 3e7b 7b20 325f 6365  lock %}">{{ 2_ce
-0000bb20: 6e74 6572 5f6d 6964 5f62 6f74 746f 6d5f  nter_mid_bottom_
-0000bb30: 6120 7d7d 3c2f 6469 763e 0a20 2020 2020  a }}</div>.     
-0000bb40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bb50: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-0000bb60: 6469 7620 636c 6173 733d 227b 2520 626c  div class="{% bl
-0000bb70: 6f63 6b20 325f 6365 6e74 6572 5f6d 6964  ock 2_center_mid
-0000bb80: 5f62 6f74 746f 6d5f 6162 635f 6220 257d  _bottom_abc_b %}
-0000bb90: 636f 6c2d 3132 2063 6f6c 2d6d 642d 347b  col-12 col-md-4{
-0000bba0: 2520 656e 6462 6c6f 636b 2025 7d22 3e7b  % endblock %}">{
-0000bbb0: 7b20 325f 6365 6e74 6572 5f6d 6964 5f62  { 2_center_mid_b
-0000bbc0: 6f74 746f 6d5f 6220 7d7d 3c2f 6469 763e  ottom_b }}</div>
-0000bbd0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000bbe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bbf0: 2020 2020 203c 6469 7620 636c 6173 733d       <div class=
-0000bc00: 227b 2520 626c 6f63 6b20 325f 6365 6e74  "{% block 2_cent
-0000bc10: 6572 5f6d 6964 5f62 6f74 746f 6d5f 6162  er_mid_bottom_ab
-0000bc20: 635f 6320 257d 636f 6c2d 3132 2063 6f6c  c_c %}col-12 col
-0000bc30: 2d6d 642d 347b 2520 656e 6462 6c6f 636b  -md-4{% endblock
-0000bc40: 2025 7d22 3e7b 7b20 325f 6365 6e74 6572   %}">{{ 2_center
-0000bc50: 5f6d 6964 5f62 6f74 746f 6d5f 6320 7d7d  _mid_bottom_c }}
-0000bc60: 3c2f 6469 763e 0a20 2020 2020 2020 2020  </div>.         
-0000bc70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bc80: 2020 2020 2020 207b 2520 656c 6966 2032         {% elif 2
-0000bc90: 5f63 656e 7465 725f 6d69 645f 626f 7474  _center_mid_bott
-0000bca0: 6f6d 5f61 2061 6e64 2032 5f63 656e 7465  om_a and 2_cente
-0000bcb0: 725f 6d69 645f 626f 7474 6f6d 5f62 2025  r_mid_bottom_b %
-0000bcc0: 7d0a 2020 2020 2020 2020 2020 2020 2020  }.              
-0000bcd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bce0: 2020 2020 2020 3c64 6976 2063 6c61 7373        <div class
-0000bcf0: 3d22 7b25 2062 6c6f 636b 2032 5f63 656e  ="{% block 2_cen
-0000bd00: 7465 725f 6d69 645f 626f 7474 6f6d 5f61  ter_mid_bottom_a
-0000bd10: 625f 6120 257d 636f 6c2d 3132 2063 6f6c  b_a %}col-12 col
-0000bd20: 2d6d 642d 387b 2520 656e 6462 6c6f 636b  -md-8{% endblock
-0000bd30: 2025 7d22 3e7b 7b20 325f 6365 6e74 6572   %}">{{ 2_center
-0000bd40: 5f6d 6964 5f62 6f74 746f 6d5f 6120 7d7d  _mid_bottom_a }}
-0000bd50: 3c2f 6469 763e 0a20 2020 2020 2020 2020  </div>.         
-0000bd60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bd70: 2020 2020 2020 2020 2020 203c 6469 7620             <div 
-0000bd80: 636c 6173 733d 227b 2520 626c 6f63 6b20  class="{% block 
-0000bd90: 325f 6365 6e74 6572 5f6d 6964 5f62 6f74  2_center_mid_bot
-0000bda0: 746f 6d5f 6162 5f62 2025 7d63 6f6c 2d31  tom_ab_b %}col-1
-0000bdb0: 3220 636f 6c2d 6d64 2d34 7b25 2065 6e64  2 col-md-4{% end
-0000bdc0: 626c 6f63 6b20 257d 223e 7b7b 2032 5f63  block %}">{{ 2_c
-0000bdd0: 656e 7465 725f 6d69 645f 626f 7474 6f6d  enter_mid_bottom
-0000bde0: 5f62 207d 7d3c 2f64 6976 3e0a 2020 2020  _b }}</div>.    
-0000bdf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000be00: 2020 2020 2020 2020 2020 2020 7b25 2065              {% e
-0000be10: 6c69 6620 325f 6365 6e74 6572 5f6d 6964  lif 2_center_mid
-0000be20: 5f62 6f74 746f 6d5f 6120 616e 6420 325f  _bottom_a and 2_
-0000be30: 6365 6e74 6572 5f6d 6964 5f62 6f74 746f  center_mid_botto
-0000be40: 6d5f 6320 257d 0a20 2020 2020 2020 2020  m_c %}.         
-0000be50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000be60: 2020 2020 2020 2020 2020 203c 6469 7620             <div 
-0000be70: 636c 6173 733d 227b 2520 626c 6f63 6b20  class="{% block 
-0000be80: 325f 6365 6e74 6572 5f6d 6964 5f62 6f74  2_center_mid_bot
-0000be90: 746f 6d5f 6163 5f61 2025 7d63 6f6c 2d31  tom_ac_a %}col-1
-0000bea0: 3220 636f 6c2d 6d64 2d36 7b25 2065 6e64  2 col-md-6{% end
-0000beb0: 626c 6f63 6b20 257d 223e 7b7b 2032 5f63  block %}">{{ 2_c
-0000bec0: 656e 7465 725f 6d69 645f 626f 7474 6f6d  enter_mid_bottom
-0000bed0: 5f61 207d 7d3c 2f64 6976 3e0a 2020 2020  _a }}</div>.    
-0000bee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bf00: 3c64 6976 2063 6c61 7373 3d22 7b25 2062  <div class="{% b
-0000bf10: 6c6f 636b 2032 5f63 656e 7465 725f 6d69  lock 2_center_mi
-0000bf20: 645f 626f 7474 6f6d 5f61 635f 6320 257d  d_bottom_ac_c %}
-0000bf30: 636f 6c2d 3132 2063 6f6c 2d6d 642d 367b  col-12 col-md-6{
-0000bf40: 2520 656e 6462 6c6f 636b 2025 7d22 3e7b  % endblock %}">{
-0000bf50: 7b20 325f 6365 6e74 6572 5f6d 6964 5f62  { 2_center_mid_b
-0000bf60: 6f74 746f 6d5f 6320 7d7d 3c2f 6469 763e  ottom_c }}</div>
-0000bf70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000bf80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bf90: 207b 2520 656c 6966 2032 5f63 656e 7465   {% elif 2_cente
-0000bfa0: 725f 6d69 645f 626f 7474 6f6d 5f62 2061  r_mid_bottom_b a
-0000bfb0: 6e64 2032 5f63 656e 7465 725f 6d69 645f  nd 2_center_mid_
-0000bfc0: 626f 7474 6f6d 5f63 2025 7d0a 2020 2020  bottom_c %}.    
-0000bfd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b8f0: 2020 2020 2020 2020 2020 2020 207b 2520               {% 
+0000b900: 656c 6966 2032 5f63 656e 7465 725f 6d69  elif 2_center_mi
+0000b910: 645f 746f 705f 6220 616e 6420 325f 6365  d_top_b and 2_ce
+0000b920: 6e74 6572 5f6d 6964 5f74 6f70 5f63 2025  nter_mid_top_c %
+0000b930: 7d0a 2020 2020 2020 2020 2020 2020 2020  }.              
+0000b940: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b950: 2020 2020 2020 3c64 6976 2063 6c61 7373        <div class
+0000b960: 3d22 7b25 2062 6c6f 636b 2032 5f63 656e  ="{% block 2_cen
+0000b970: 7465 725f 6d69 645f 746f 705f 6263 5f62  ter_mid_top_bc_b
+0000b980: 2025 7d63 6f6c 2d31 3220 636f 6c2d 6d64   %}col-12 col-md
+0000b990: 2d34 7b25 2065 6e64 626c 6f63 6b20 257d  -4{% endblock %}
+0000b9a0: 223e 7b7b 2032 5f63 656e 7465 725f 6d69  ">{{ 2_center_mi
+0000b9b0: 645f 746f 705f 6220 7d7d 3c2f 6469 763e  d_top_b }}</div>
+0000b9c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000b9d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b9e0: 2020 2020 203c 6469 7620 636c 6173 733d       <div class=
+0000b9f0: 227b 2520 626c 6f63 6b20 325f 6365 6e74  "{% block 2_cent
+0000ba00: 6572 5f6d 6964 5f74 6f70 5f62 635f 6320  er_mid_top_bc_c 
+0000ba10: 257d 636f 6c2d 3132 2063 6f6c 2d6d 642d  %}col-12 col-md-
+0000ba20: 387b 2520 656e 6462 6c6f 636b 2025 7d22  8{% endblock %}"
+0000ba30: 3e7b 7b20 325f 6365 6e74 6572 5f6d 6964  >{{ 2_center_mid
+0000ba40: 5f74 6f70 5f63 207d 7d3c 2f64 6976 3e0a  _top_c }}</div>.
+0000ba50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ba60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ba70: 7b25 2065 6c73 6520 257d 0a20 2020 2020  {% else %}.     
+0000ba80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ba90: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+0000baa0: 6469 7620 636c 6173 733d 2263 6f6c 2d31  div class="col-1
+0000bab0: 3222 3e7b 7b20 325f 6365 6e74 6572 5f6d  2">{{ 2_center_m
+0000bac0: 6964 5f74 6f70 5f61 207d 7d7b 7b20 325f  id_top_a }}{{ 2_
+0000bad0: 6365 6e74 6572 5f6d 6964 5f74 6f70 5f62  center_mid_top_b
+0000bae0: 207d 7d7b 7b20 325f 6365 6e74 6572 5f6d   }}{{ 2_center_m
+0000baf0: 6964 5f74 6f70 5f63 207d 7d3c 2f64 6976  id_top_c }}</div
+0000bb00: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
+0000bb10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bb20: 2020 7b25 2065 6e64 6966 2025 7d0a 2020    {% endif %}.  
+0000bb30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bb40: 2020 2020 2020 2020 2020 3c2f 6469 763e            </div>
+0000bb50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000bb60: 2020 2020 2020 2020 2020 2020 207b 2520               {% 
+0000bb70: 656e 6469 6620 257d 0a20 2020 2020 2020  endif %}.       
+0000bb80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bb90: 2020 2020 203c 212d 2d20 454e 4420 4365       <!-- END Ce
+0000bba0: 6e74 6572 206d 6964 2d74 6f70 202d 2d3e  nter mid-top -->
+0000bbb0: 0a0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000bbc0: 2020 2020 2020 2020 2020 2020 2020 3c21                <!
+0000bbd0: 2d2d 2043 656e 7465 7220 636f 6e74 656e  -- Center conten
+0000bbe0: 7420 2d2d 3e0a 2020 2020 2020 2020 2020  t -->.          
+0000bbf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bc00: 2020 7b25 2069 6620 325f 6365 6e74 6572    {% if 2_center
+0000bc10: 5f63 6f6e 7465 6e74 2025 7d0a 2020 2020  _content %}.    
+0000bc20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bc30: 2020 2020 2020 2020 3c64 6976 2063 6c61          <div cla
+0000bc40: 7373 3d22 726f 7722 3e0a 2020 2020 2020  ss="row">.      
+0000bc50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bc60: 2020 2020 2020 2020 2020 3c64 6976 2063            <div c
+0000bc70: 6c61 7373 3d22 636f 6c22 3e0a 2020 2020  lass="col">.    
+0000bc80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bc90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bca0: 7b7b 2032 5f63 656e 7465 725f 636f 6e74  {{ 2_center_cont
+0000bcb0: 656e 7420 7d7d 0a20 2020 2020 2020 2020  ent }}.         
+0000bcc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bcd0: 2020 2020 2020 203c 2f64 6976 3e0a 2020         </div>.  
+0000bce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bcf0: 2020 2020 2020 2020 2020 3c2f 6469 763e            </div>
+0000bd00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000bd10: 2020 2020 2020 2020 2020 2020 207b 2520               {% 
+0000bd20: 656e 6469 6620 257d 0a20 2020 2020 2020  endif %}.       
+0000bd30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bd40: 2020 2020 203c 212d 2d20 454e 4420 4365       <!-- END Ce
+0000bd50: 6e74 6572 2063 6f6e 7465 6e74 202d 2d3e  nter content -->
+0000bd60: 0a0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000bd70: 2020 2020 2020 2020 2020 2020 2020 3c21                <!
+0000bd80: 2d2d 2043 656e 7465 7220 6d69 642d 626f  -- Center mid-bo
+0000bd90: 7474 6f6d 202d 2d3e 0a20 2020 2020 2020  ttom -->.       
+0000bda0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bdb0: 2020 2020 207b 2520 6966 2032 5f63 656e       {% if 2_cen
+0000bdc0: 7465 725f 6d69 645f 626f 7474 6f6d 5f61  ter_mid_bottom_a
+0000bdd0: 206f 7220 325f 6365 6e74 6572 5f6d 6964   or 2_center_mid
+0000bde0: 5f62 6f74 746f 6d5f 6220 6f72 2032 5f63  _bottom_b or 2_c
+0000bdf0: 656e 7465 725f 6d69 645f 626f 7474 6f6d  enter_mid_bottom
+0000be00: 5f63 2025 7d0a 2020 2020 2020 2020 2020  _c %}.          
+0000be10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000be20: 2020 3c64 6976 2063 6c61 7373 3d22 726f    <div class="ro
+0000be30: 7722 3e0a 2020 2020 2020 2020 2020 2020  w">.            
+0000be40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000be50: 2020 2020 7b25 2069 6620 325f 6365 6e74      {% if 2_cent
+0000be60: 6572 5f6d 6964 5f62 6f74 746f 6d5f 6120  er_mid_bottom_a 
+0000be70: 616e 6420 325f 6365 6e74 6572 5f6d 6964  and 2_center_mid
+0000be80: 5f62 6f74 746f 6d5f 6220 616e 6420 325f  _bottom_b and 2_
+0000be90: 6365 6e74 6572 5f6d 6964 5f62 6f74 746f  center_mid_botto
+0000bea0: 6d5f 6320 257d 0a20 2020 2020 2020 2020  m_c %}.         
+0000beb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bec0: 2020 2020 2020 2020 2020 203c 6469 7620             <div 
+0000bed0: 636c 6173 733d 227b 2520 626c 6f63 6b20  class="{% block 
+0000bee0: 325f 6365 6e74 6572 5f6d 6964 5f62 6f74  2_center_mid_bot
+0000bef0: 746f 6d5f 6162 635f 6120 257d 636f 6c2d  tom_abc_a %}col-
+0000bf00: 3132 2063 6f6c 2d6d 642d 347b 2520 656e  12 col-md-4{% en
+0000bf10: 6462 6c6f 636b 2025 7d22 3e7b 7b20 325f  dblock %}">{{ 2_
+0000bf20: 6365 6e74 6572 5f6d 6964 5f62 6f74 746f  center_mid_botto
+0000bf30: 6d5f 6120 7d7d 3c2f 6469 763e 0a20 2020  m_a }}</div>.   
+0000bf40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bf50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bf60: 203c 6469 7620 636c 6173 733d 227b 2520   <div class="{% 
+0000bf70: 626c 6f63 6b20 325f 6365 6e74 6572 5f6d  block 2_center_m
+0000bf80: 6964 5f62 6f74 746f 6d5f 6162 635f 6220  id_bottom_abc_b 
+0000bf90: 257d 636f 6c2d 3132 2063 6f6c 2d6d 642d  %}col-12 col-md-
+0000bfa0: 347b 2520 656e 6462 6c6f 636b 2025 7d22  4{% endblock %}"
+0000bfb0: 3e7b 7b20 325f 6365 6e74 6572 5f6d 6964  >{{ 2_center_mid
+0000bfc0: 5f62 6f74 746f 6d5f 6220 7d7d 3c2f 6469  _bottom_b }}</di
+0000bfd0: 763e 0a20 2020 2020 2020 2020 2020 2020  v>.             
 0000bfe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bff0: 3c64 6976 2063 6c61 7373 3d22 7b25 2062  <div class="{% b
-0000c000: 6c6f 636b 2032 5f63 656e 7465 725f 6d69  lock 2_center_mi
-0000c010: 645f 626f 7474 6f6d 5f62 635f 6220 257d  d_bottom_bc_b %}
-0000c020: 636f 6c2d 3132 2063 6f6c 2d6d 642d 347b  col-12 col-md-4{
-0000c030: 2520 656e 6462 6c6f 636b 2025 7d22 3e7b  % endblock %}">{
-0000c040: 7b20 325f 6365 6e74 6572 5f6d 6964 5f62  { 2_center_mid_b
-0000c050: 6f74 746f 6d5f 6220 7d7d 3c2f 6469 763e  ottom_b }}</div>
-0000c060: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000bff0: 2020 2020 2020 203c 6469 7620 636c 6173         <div clas
+0000c000: 733d 227b 2520 626c 6f63 6b20 325f 6365  s="{% block 2_ce
+0000c010: 6e74 6572 5f6d 6964 5f62 6f74 746f 6d5f  nter_mid_bottom_
+0000c020: 6162 635f 6320 257d 636f 6c2d 3132 2063  abc_c %}col-12 c
+0000c030: 6f6c 2d6d 642d 347b 2520 656e 6462 6c6f  ol-md-4{% endblo
+0000c040: 636b 2025 7d22 3e7b 7b20 325f 6365 6e74  ck %}">{{ 2_cent
+0000c050: 6572 5f6d 6964 5f62 6f74 746f 6d5f 6320  er_mid_bottom_c 
+0000c060: 7d7d 3c2f 6469 763e 0a20 2020 2020 2020  }}</div>.       
 0000c070: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c080: 2020 2020 203c 6469 7620 636c 6173 733d       <div class=
-0000c090: 227b 2520 626c 6f63 6b20 325f 6365 6e74  "{% block 2_cent
-0000c0a0: 6572 5f6d 6964 5f62 6f74 746f 6d5f 6263  er_mid_bottom_bc
-0000c0b0: 5f63 2025 7d63 6f6c 2d31 3220 636f 6c2d  _c %}col-12 col-
-0000c0c0: 6d64 2d38 7b25 2065 6e64 626c 6f63 6b20  md-8{% endblock 
-0000c0d0: 257d 223e 7b7b 2032 5f63 656e 7465 725f  %}">{{ 2_center_
-0000c0e0: 6d69 645f 626f 7474 6f6d 5f63 207d 7d3c  mid_bottom_c }}<
-0000c0f0: 2f64 6976 3e0a 2020 2020 2020 2020 2020  /div>.          
-0000c100: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c110: 2020 2020 2020 7b25 2065 6c73 6520 257d        {% else %}
-0000c120: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000c130: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c140: 2020 2020 203c 6469 7620 636c 6173 733d       <div class=
-0000c150: 2263 6f6c 2d31 3222 3e7b 7b20 325f 6365  "col-12">{{ 2_ce
-0000c160: 6e74 6572 5f6d 6964 5f62 6f74 746f 6d5f  nter_mid_bottom_
-0000c170: 6120 7d7d 7b7b 2032 5f63 656e 7465 725f  a }}{{ 2_center_
-0000c180: 6d69 645f 626f 7474 6f6d 5f62 207d 7d7b  mid_bottom_b }}{
-0000c190: 7b20 325f 6365 6e74 6572 5f6d 6964 5f62  { 2_center_mid_b
-0000c1a0: 6f74 746f 6d5f 6320 7d7d 3c2f 6469 763e  ottom_c }}</div>
-0000c1b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000c1c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c1d0: 207b 2520 656e 6469 6620 257d 0a20 2020   {% endif %}.   
-0000c1e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c1f0: 2020 2020 2020 2020 203c 2f64 6976 3e0a           </div>.
-0000c200: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c210: 2020 2020 2020 2020 2020 2020 7b25 2065              {% e
-0000c220: 6e64 6966 2025 7d0a 2020 2020 2020 2020  ndif %}.        
-0000c230: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c240: 2020 2020 3c21 2d2d 2045 4e44 2043 656e      <!-- END Cen
-0000c250: 7465 7220 6d69 642d 626f 7474 6f6d 202d  ter mid-bottom -
-0000c260: 2d3e 0a0a 2020 2020 2020 2020 2020 2020  ->..            
-0000c270: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c280: 3c21 2d2d 2043 656e 7465 7220 626f 7474  <!-- Center bott
-0000c290: 6f6d 202d 2d3e 0a20 2020 2020 2020 2020  om -->.         
-0000c2a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c2b0: 2020 207b 2520 6966 2032 5f63 656e 7465     {% if 2_cente
-0000c2c0: 725f 626f 7474 6f6d 5f61 206f 7220 325f  r_bottom_a or 2_
-0000c2d0: 6365 6e74 6572 5f62 6f74 746f 6d5f 6220  center_bottom_b 
-0000c2e0: 6f72 2032 5f63 656e 7465 725f 626f 7474  or 2_center_bott
-0000c2f0: 6f6d 5f63 2025 7d0a 2020 2020 2020 2020  om_c %}.        
-0000c300: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c310: 2020 2020 3c64 6976 2063 6c61 7373 3d22      <div class="
-0000c320: 726f 7722 3e0a 2020 2020 2020 2020 2020  row">.          
-0000c330: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c340: 2020 2020 2020 7b25 2069 6620 325f 6365        {% if 2_ce
-0000c350: 6e74 6572 5f62 6f74 746f 6d5f 6120 616e  nter_bottom_a an
-0000c360: 6420 325f 6365 6e74 6572 5f62 6f74 746f  d 2_center_botto
-0000c370: 6d5f 6220 616e 6420 325f 6365 6e74 6572  m_b and 2_center
-0000c380: 5f62 6f74 746f 6d5f 6320 257d 0a20 2020  _bottom_c %}.   
-0000c390: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c3a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c3b0: 203c 6469 7620 636c 6173 733d 227b 2520   <div class="{% 
-0000c3c0: 626c 6f63 6b20 325f 6365 6e74 6572 5f62  block 2_center_b
-0000c3d0: 6f74 746f 6d5f 6162 635f 6120 257d 636f  ottom_abc_a %}co
-0000c3e0: 6c2d 3132 2063 6f6c 2d6d 642d 347b 2520  l-12 col-md-4{% 
-0000c3f0: 656e 6462 6c6f 636b 2025 7d22 3e7b 7b20  endblock %}">{{ 
-0000c400: 325f 6365 6e74 6572 5f62 6f74 746f 6d5f  2_center_bottom_
-0000c410: 6120 7d7d 3c2f 6469 763e 0a20 2020 2020  a }}</div>.     
-0000c420: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c430: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-0000c440: 6469 7620 636c 6173 733d 227b 2520 626c  div class="{% bl
-0000c450: 6f63 6b20 325f 6365 6e74 6572 5f62 6f74  ock 2_center_bot
-0000c460: 746f 6d5f 6162 635f 6220 257d 636f 6c2d  tom_abc_b %}col-
-0000c470: 3132 2063 6f6c 2d6d 642d 347b 2520 656e  12 col-md-4{% en
-0000c480: 6462 6c6f 636b 2025 7d22 3e7b 7b20 325f  dblock %}">{{ 2_
-0000c490: 6365 6e74 6572 5f62 6f74 746f 6d5f 6220  center_bottom_b 
-0000c4a0: 7d7d 3c2f 6469 763e 0a20 2020 2020 2020  }}</div>.       
-0000c4b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c4c0: 2020 2020 2020 2020 2020 2020 203c 6469               <di
-0000c4d0: 7620 636c 6173 733d 227b 2520 626c 6f63  v class="{% bloc
-0000c4e0: 6b20 325f 6365 6e74 6572 5f62 6f74 746f  k 2_center_botto
-0000c4f0: 6d5f 6162 635f 6320 257d 636f 6c2d 3132  m_abc_c %}col-12
-0000c500: 2063 6f6c 2d6d 642d 347b 2520 656e 6462   col-md-4{% endb
-0000c510: 6c6f 636b 2025 7d22 3e7b 7b20 325f 6365  lock %}">{{ 2_ce
-0000c520: 6e74 6572 5f62 6f74 746f 6d5f 6320 7d7d  nter_bottom_c }}
-0000c530: 3c2f 6469 763e 0a20 2020 2020 2020 2020  </div>.         
-0000c540: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c550: 2020 2020 2020 207b 2520 656c 6966 2032         {% elif 2
-0000c560: 5f63 656e 7465 725f 626f 7474 6f6d 5f61  _center_bottom_a
-0000c570: 2061 6e64 2032 5f63 656e 7465 725f 626f   and 2_center_bo
-0000c580: 7474 6f6d 5f62 2025 7d0a 2020 2020 2020  ttom_b %}.      
-0000c590: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c5a0: 2020 2020 2020 2020 2020 2020 2020 3c64                <d
-0000c5b0: 6976 2063 6c61 7373 3d22 7b25 2062 6c6f  iv class="{% blo
-0000c5c0: 636b 2032 5f63 656e 7465 725f 626f 7474  ck 2_center_bott
-0000c5d0: 6f6d 5f61 625f 6120 257d 636f 6c2d 3132  om_ab_a %}col-12
-0000c5e0: 2063 6f6c 2d6d 642d 387b 2520 656e 6462   col-md-8{% endb
-0000c5f0: 6c6f 636b 2025 7d22 3e7b 7b20 325f 6365  lock %}">{{ 2_ce
-0000c600: 6e74 6572 5f62 6f74 746f 6d5f 6120 7d7d  nter_bottom_a }}
-0000c610: 3c2f 6469 763e 0a20 2020 2020 2020 2020  </div>.         
-0000c620: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c630: 2020 2020 2020 2020 2020 203c 6469 7620             <div 
-0000c640: 636c 6173 733d 227b 2520 626c 6f63 6b20  class="{% block 
-0000c650: 325f 6365 6e74 6572 5f62 6f74 746f 6d5f  2_center_bottom_
-0000c660: 6162 5f62 2025 7d63 6f6c 2d31 3220 636f  ab_b %}col-12 co
-0000c670: 6c2d 6d64 2d34 7b25 2065 6e64 626c 6f63  l-md-4{% endbloc
-0000c680: 6b20 257d 223e 7b7b 2032 5f63 656e 7465  k %}">{{ 2_cente
-0000c690: 725f 626f 7474 6f6d 5f62 207d 7d3c 2f64  r_bottom_b }}</d
-0000c6a0: 6976 3e0a 2020 2020 2020 2020 2020 2020  iv>.            
-0000c6b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c6c0: 2020 2020 7b25 2065 6c69 6620 325f 6365      {% elif 2_ce
-0000c6d0: 6e74 6572 5f62 6f74 746f 6d5f 6120 616e  nter_bottom_a an
-0000c6e0: 6420 325f 6365 6e74 6572 5f62 6f74 746f  d 2_center_botto
-0000c6f0: 6d5f 6320 257d 0a20 2020 2020 2020 2020  m_c %}.         
+0000c080: 2020 2020 2020 2020 207b 2520 656c 6966           {% elif
+0000c090: 2032 5f63 656e 7465 725f 6d69 645f 626f   2_center_mid_bo
+0000c0a0: 7474 6f6d 5f61 2061 6e64 2032 5f63 656e  ttom_a and 2_cen
+0000c0b0: 7465 725f 6d69 645f 626f 7474 6f6d 5f62  ter_mid_bottom_b
+0000c0c0: 2025 7d0a 2020 2020 2020 2020 2020 2020   %}.            
+0000c0d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c0e0: 2020 2020 2020 2020 3c64 6976 2063 6c61          <div cla
+0000c0f0: 7373 3d22 7b25 2062 6c6f 636b 2032 5f63  ss="{% block 2_c
+0000c100: 656e 7465 725f 6d69 645f 626f 7474 6f6d  enter_mid_bottom
+0000c110: 5f61 625f 6120 257d 636f 6c2d 3132 2063  _ab_a %}col-12 c
+0000c120: 6f6c 2d6d 642d 387b 2520 656e 6462 6c6f  ol-md-8{% endblo
+0000c130: 636b 2025 7d22 3e7b 7b20 325f 6365 6e74  ck %}">{{ 2_cent
+0000c140: 6572 5f6d 6964 5f62 6f74 746f 6d5f 6120  er_mid_bottom_a 
+0000c150: 7d7d 3c2f 6469 763e 0a20 2020 2020 2020  }}</div>.       
+0000c160: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c170: 2020 2020 2020 2020 2020 2020 203c 6469               <di
+0000c180: 7620 636c 6173 733d 227b 2520 626c 6f63  v class="{% bloc
+0000c190: 6b20 325f 6365 6e74 6572 5f6d 6964 5f62  k 2_center_mid_b
+0000c1a0: 6f74 746f 6d5f 6162 5f62 2025 7d63 6f6c  ottom_ab_b %}col
+0000c1b0: 2d31 3220 636f 6c2d 6d64 2d34 7b25 2065  -12 col-md-4{% e
+0000c1c0: 6e64 626c 6f63 6b20 257d 223e 7b7b 2032  ndblock %}">{{ 2
+0000c1d0: 5f63 656e 7465 725f 6d69 645f 626f 7474  _center_mid_bott
+0000c1e0: 6f6d 5f62 207d 7d3c 2f64 6976 3e0a 2020  om_b }}</div>.  
+0000c1f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c200: 2020 2020 2020 2020 2020 2020 2020 7b25                {%
+0000c210: 2065 6c69 6620 325f 6365 6e74 6572 5f6d   elif 2_center_m
+0000c220: 6964 5f62 6f74 746f 6d5f 6120 616e 6420  id_bottom_a and 
+0000c230: 325f 6365 6e74 6572 5f6d 6964 5f62 6f74  2_center_mid_bot
+0000c240: 746f 6d5f 6320 257d 0a20 2020 2020 2020  tom_c %}.       
+0000c250: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c260: 2020 2020 2020 2020 2020 2020 203c 6469               <di
+0000c270: 7620 636c 6173 733d 227b 2520 626c 6f63  v class="{% bloc
+0000c280: 6b20 325f 6365 6e74 6572 5f6d 6964 5f62  k 2_center_mid_b
+0000c290: 6f74 746f 6d5f 6163 5f61 2025 7d63 6f6c  ottom_ac_a %}col
+0000c2a0: 2d31 3220 636f 6c2d 6d64 2d36 7b25 2065  -12 col-md-6{% e
+0000c2b0: 6e64 626c 6f63 6b20 257d 223e 7b7b 2032  ndblock %}">{{ 2
+0000c2c0: 5f63 656e 7465 725f 6d69 645f 626f 7474  _center_mid_bott
+0000c2d0: 6f6d 5f61 207d 7d3c 2f64 6976 3e0a 2020  om_a }}</div>.  
+0000c2e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c2f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c300: 2020 3c64 6976 2063 6c61 7373 3d22 7b25    <div class="{%
+0000c310: 2062 6c6f 636b 2032 5f63 656e 7465 725f   block 2_center_
+0000c320: 6d69 645f 626f 7474 6f6d 5f61 635f 6320  mid_bottom_ac_c 
+0000c330: 257d 636f 6c2d 3132 2063 6f6c 2d6d 642d  %}col-12 col-md-
+0000c340: 367b 2520 656e 6462 6c6f 636b 2025 7d22  6{% endblock %}"
+0000c350: 3e7b 7b20 325f 6365 6e74 6572 5f6d 6964  >{{ 2_center_mid
+0000c360: 5f62 6f74 746f 6d5f 6320 7d7d 3c2f 6469  _bottom_c }}</di
+0000c370: 763e 0a20 2020 2020 2020 2020 2020 2020  v>.             
+0000c380: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c390: 2020 207b 2520 656c 6966 2032 5f63 656e     {% elif 2_cen
+0000c3a0: 7465 725f 6d69 645f 626f 7474 6f6d 5f62  ter_mid_bottom_b
+0000c3b0: 2061 6e64 2032 5f63 656e 7465 725f 6d69   and 2_center_mi
+0000c3c0: 645f 626f 7474 6f6d 5f63 2025 7d0a 2020  d_bottom_c %}.  
+0000c3d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c3e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c3f0: 2020 3c64 6976 2063 6c61 7373 3d22 7b25    <div class="{%
+0000c400: 2062 6c6f 636b 2032 5f63 656e 7465 725f   block 2_center_
+0000c410: 6d69 645f 626f 7474 6f6d 5f62 635f 6220  mid_bottom_bc_b 
+0000c420: 257d 636f 6c2d 3132 2063 6f6c 2d6d 642d  %}col-12 col-md-
+0000c430: 347b 2520 656e 6462 6c6f 636b 2025 7d22  4{% endblock %}"
+0000c440: 3e7b 7b20 325f 6365 6e74 6572 5f6d 6964  >{{ 2_center_mid
+0000c450: 5f62 6f74 746f 6d5f 6220 7d7d 3c2f 6469  _bottom_b }}</di
+0000c460: 763e 0a20 2020 2020 2020 2020 2020 2020  v>.             
+0000c470: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c480: 2020 2020 2020 203c 6469 7620 636c 6173         <div clas
+0000c490: 733d 227b 2520 626c 6f63 6b20 325f 6365  s="{% block 2_ce
+0000c4a0: 6e74 6572 5f6d 6964 5f62 6f74 746f 6d5f  nter_mid_bottom_
+0000c4b0: 6263 5f63 2025 7d63 6f6c 2d31 3220 636f  bc_c %}col-12 co
+0000c4c0: 6c2d 6d64 2d38 7b25 2065 6e64 626c 6f63  l-md-8{% endbloc
+0000c4d0: 6b20 257d 223e 7b7b 2032 5f63 656e 7465  k %}">{{ 2_cente
+0000c4e0: 725f 6d69 645f 626f 7474 6f6d 5f63 207d  r_mid_bottom_c }
+0000c4f0: 7d3c 2f64 6976 3e0a 2020 2020 2020 2020  }</div>.        
+0000c500: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c510: 2020 2020 2020 2020 7b25 2065 6c73 6520          {% else 
+0000c520: 257d 0a20 2020 2020 2020 2020 2020 2020  %}.             
+0000c530: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c540: 2020 2020 2020 203c 6469 7620 636c 6173         <div clas
+0000c550: 733d 2263 6f6c 2d31 3222 3e7b 7b20 325f  s="col-12">{{ 2_
+0000c560: 6365 6e74 6572 5f6d 6964 5f62 6f74 746f  center_mid_botto
+0000c570: 6d5f 6120 7d7d 7b7b 2032 5f63 656e 7465  m_a }}{{ 2_cente
+0000c580: 725f 6d69 645f 626f 7474 6f6d 5f62 207d  r_mid_bottom_b }
+0000c590: 7d7b 7b20 325f 6365 6e74 6572 5f6d 6964  }{{ 2_center_mid
+0000c5a0: 5f62 6f74 746f 6d5f 6320 7d7d 3c2f 6469  _bottom_c }}</di
+0000c5b0: 763e 0a20 2020 2020 2020 2020 2020 2020  v>.             
+0000c5c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c5d0: 2020 207b 2520 656e 6469 6620 257d 0a20     {% endif %}. 
+0000c5e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c5f0: 2020 2020 2020 2020 2020 203c 2f64 6976             </div
+0000c600: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
+0000c610: 2020 2020 2020 2020 2020 2020 2020 7b25                {%
+0000c620: 2065 6e64 6966 2025 7d0a 2020 2020 2020   endif %}.      
+0000c630: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c640: 2020 2020 2020 3c21 2d2d 2045 4e44 2043        <!-- END C
+0000c650: 656e 7465 7220 6d69 642d 626f 7474 6f6d  enter mid-bottom
+0000c660: 202d 2d3e 0a0a 2020 2020 2020 2020 2020   -->..          
+0000c670: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c680: 2020 3c21 2d2d 2043 656e 7465 7220 626f    <!-- Center bo
+0000c690: 7474 6f6d 202d 2d3e 0a20 2020 2020 2020  ttom -->.       
+0000c6a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c6b0: 2020 2020 207b 2520 6966 2032 5f63 656e       {% if 2_cen
+0000c6c0: 7465 725f 626f 7474 6f6d 5f61 206f 7220  ter_bottom_a or 
+0000c6d0: 325f 6365 6e74 6572 5f62 6f74 746f 6d5f  2_center_bottom_
+0000c6e0: 6220 6f72 2032 5f63 656e 7465 725f 626f  b or 2_center_bo
+0000c6f0: 7474 6f6d 5f63 2025 7d0a 2020 2020 2020  ttom_c %}.      
 0000c700: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c710: 2020 2020 2020 2020 2020 203c 6469 7620             <div 
-0000c720: 636c 6173 733d 227b 2520 626c 6f63 6b20  class="{% block 
-0000c730: 325f 6365 6e74 6572 5f62 6f74 746f 6d5f  2_center_bottom_
-0000c740: 6163 5f61 2025 7d63 6f6c 2d31 3220 636f  ac_a %}col-12 co
-0000c750: 6c2d 6d64 2d36 7b25 2065 6e64 626c 6f63  l-md-6{% endbloc
-0000c760: 6b20 257d 223e 7b7b 2032 5f63 656e 7465  k %}">{{ 2_cente
-0000c770: 725f 626f 7474 6f6d 5f61 207d 7d3c 2f64  r_bottom_a }}</d
-0000c780: 6976 3e0a 2020 2020 2020 2020 2020 2020  iv>.            
+0000c710: 2020 2020 2020 3c64 6976 2063 6c61 7373        <div class
+0000c720: 3d22 726f 7722 3e0a 2020 2020 2020 2020  ="row">.        
+0000c730: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c740: 2020 2020 2020 2020 7b25 2069 6620 325f          {% if 2_
+0000c750: 6365 6e74 6572 5f62 6f74 746f 6d5f 6120  center_bottom_a 
+0000c760: 616e 6420 325f 6365 6e74 6572 5f62 6f74  and 2_center_bot
+0000c770: 746f 6d5f 6220 616e 6420 325f 6365 6e74  tom_b and 2_cent
+0000c780: 6572 5f62 6f74 746f 6d5f 6320 257d 0a20  er_bottom_c %}. 
 0000c790: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c7a0: 2020 2020 2020 2020 3c64 6976 2063 6c61          <div cla
-0000c7b0: 7373 3d22 7b25 2062 6c6f 636b 2032 5f63  ss="{% block 2_c
-0000c7c0: 656e 7465 725f 626f 7474 6f6d 5f61 635f  enter_bottom_ac_
-0000c7d0: 6320 257d 636f 6c2d 3132 2063 6f6c 2d6d  c %}col-12 col-m
-0000c7e0: 642d 367b 2520 656e 6462 6c6f 636b 2025  d-6{% endblock %
-0000c7f0: 7d22 3e7b 7b20 325f 6365 6e74 6572 5f62  }">{{ 2_center_b
-0000c800: 6f74 746f 6d5f 6320 7d7d 3c2f 6469 763e  ottom_c }}</div>
-0000c810: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000c7a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c7b0: 2020 203c 6469 7620 636c 6173 733d 227b     <div class="{
+0000c7c0: 2520 626c 6f63 6b20 325f 6365 6e74 6572  % block 2_center
+0000c7d0: 5f62 6f74 746f 6d5f 6162 635f 6120 257d  _bottom_abc_a %}
+0000c7e0: 636f 6c2d 3132 2063 6f6c 2d6d 642d 347b  col-12 col-md-4{
+0000c7f0: 2520 656e 6462 6c6f 636b 2025 7d22 3e7b  % endblock %}">{
+0000c800: 7b20 325f 6365 6e74 6572 5f62 6f74 746f  { 2_center_botto
+0000c810: 6d5f 6120 7d7d 3c2f 6469 763e 0a20 2020  m_a }}</div>.   
 0000c820: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c830: 207b 2520 656c 6966 2032 5f63 656e 7465   {% elif 2_cente
-0000c840: 725f 626f 7474 6f6d 5f62 2061 6e64 2032  r_bottom_b and 2
-0000c850: 5f63 656e 7465 725f 626f 7474 6f6d 5f63  _center_bottom_c
-0000c860: 2025 7d0a 2020 2020 2020 2020 2020 2020   %}.            
-0000c870: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c880: 2020 2020 2020 2020 3c64 6976 2063 6c61          <div cla
-0000c890: 7373 3d22 7b25 2062 6c6f 636b 2032 5f63  ss="{% block 2_c
-0000c8a0: 656e 7465 725f 626f 7474 6f6d 5f62 635f  enter_bottom_bc_
-0000c8b0: 6220 257d 636f 6c2d 3132 2063 6f6c 2d6d  b %}col-12 col-m
-0000c8c0: 642d 347b 2520 656e 6462 6c6f 636b 2025  d-4{% endblock %
-0000c8d0: 7d22 3e7b 7b20 325f 6365 6e74 6572 5f62  }">{{ 2_center_b
-0000c8e0: 6f74 746f 6d5f 6220 7d7d 3c2f 6469 763e  ottom_b }}</div>
-0000c8f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000c900: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c910: 2020 2020 203c 6469 7620 636c 6173 733d       <div class=
-0000c920: 227b 2520 626c 6f63 6b20 325f 6365 6e74  "{% block 2_cent
-0000c930: 6572 5f62 6f74 746f 6d5f 6263 5f63 2025  er_bottom_bc_c %
-0000c940: 7d63 6f6c 2d31 3220 636f 6c2d 6d64 2d38  }col-12 col-md-8
-0000c950: 7b25 2065 6e64 626c 6f63 6b20 257d 223e  {% endblock %}">
-0000c960: 7b7b 2032 5f63 656e 7465 725f 626f 7474  {{ 2_center_bott
-0000c970: 6f6d 5f63 207d 7d3c 2f64 6976 3e0a 2020  om_c }}</div>.  
-0000c980: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c990: 2020 2020 2020 2020 2020 2020 2020 7b25                {%
-0000c9a0: 2065 6c73 6520 257d 0a20 2020 2020 2020   else %}.       
-0000c9b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c9c0: 2020 2020 2020 2020 2020 2020 203c 6469               <di
-0000c9d0: 7620 636c 6173 733d 2263 6f6c 2d31 3222  v class="col-12"
-0000c9e0: 3e7b 7b20 325f 6365 6e74 6572 5f62 6f74  >{{ 2_center_bot
-0000c9f0: 746f 6d5f 6120 7d7d 7b7b 2032 5f63 656e  tom_a }}{{ 2_cen
-0000ca00: 7465 725f 626f 7474 6f6d 5f62 207d 7d7b  ter_bottom_b }}{
-0000ca10: 7b20 325f 6365 6e74 6572 5f62 6f74 746f  { 2_center_botto
-0000ca20: 6d5f 6320 7d7d 3c2f 6469 763e 0a20 2020  m_c }}</div>.   
-0000ca30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ca40: 2020 2020 2020 2020 2020 2020 207b 2520               {% 
-0000ca50: 656e 6469 6620 257d 0a20 2020 2020 2020  endif %}.       
-0000ca60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ca70: 2020 2020 203c 2f64 6976 3e0a 2020 2020       </div>.    
-0000ca80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ca90: 2020 2020 2020 2020 7b25 2065 6e64 6966          {% endif
-0000caa0: 2025 7d0a 0a20 2020 2020 2020 2020 2020   %}..           
-0000cab0: 2020 2020 2020 2020 2020 2020 203c 2f64               </d
-0000cac0: 6976 3e0a 2020 2020 2020 2020 2020 2020  iv>.            
-0000cad0: 2020 2020 2020 2020 2020 2020 3c21 2d2d              <!--
-0000cae0: 2045 6e64 2043 656e 7465 7220 636f 6c75   End Center colu
-0000caf0: 6d6e 202d 2d3e 0a0a 2020 2020 2020 2020  mn -->..        
+0000c830: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c840: 203c 6469 7620 636c 6173 733d 227b 2520   <div class="{% 
+0000c850: 626c 6f63 6b20 325f 6365 6e74 6572 5f62  block 2_center_b
+0000c860: 6f74 746f 6d5f 6162 635f 6220 257d 636f  ottom_abc_b %}co
+0000c870: 6c2d 3132 2063 6f6c 2d6d 642d 347b 2520  l-12 col-md-4{% 
+0000c880: 656e 6462 6c6f 636b 2025 7d22 3e7b 7b20  endblock %}">{{ 
+0000c890: 325f 6365 6e74 6572 5f62 6f74 746f 6d5f  2_center_bottom_
+0000c8a0: 6220 7d7d 3c2f 6469 763e 0a20 2020 2020  b }}</div>.     
+0000c8b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c8c0: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+0000c8d0: 6469 7620 636c 6173 733d 227b 2520 626c  div class="{% bl
+0000c8e0: 6f63 6b20 325f 6365 6e74 6572 5f62 6f74  ock 2_center_bot
+0000c8f0: 746f 6d5f 6162 635f 6320 257d 636f 6c2d  tom_abc_c %}col-
+0000c900: 3132 2063 6f6c 2d6d 642d 347b 2520 656e  12 col-md-4{% en
+0000c910: 6462 6c6f 636b 2025 7d22 3e7b 7b20 325f  dblock %}">{{ 2_
+0000c920: 6365 6e74 6572 5f62 6f74 746f 6d5f 6320  center_bottom_c 
+0000c930: 7d7d 3c2f 6469 763e 0a20 2020 2020 2020  }}</div>.       
+0000c940: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c950: 2020 2020 2020 2020 207b 2520 656c 6966           {% elif
+0000c960: 2032 5f63 656e 7465 725f 626f 7474 6f6d   2_center_bottom
+0000c970: 5f61 2061 6e64 2032 5f63 656e 7465 725f  _a and 2_center_
+0000c980: 626f 7474 6f6d 5f62 2025 7d0a 2020 2020  bottom_b %}.    
+0000c990: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c9a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c9b0: 3c64 6976 2063 6c61 7373 3d22 7b25 2062  <div class="{% b
+0000c9c0: 6c6f 636b 2032 5f63 656e 7465 725f 626f  lock 2_center_bo
+0000c9d0: 7474 6f6d 5f61 625f 6120 257d 636f 6c2d  ttom_ab_a %}col-
+0000c9e0: 3132 2063 6f6c 2d6d 642d 387b 2520 656e  12 col-md-8{% en
+0000c9f0: 6462 6c6f 636b 2025 7d22 3e7b 7b20 325f  dblock %}">{{ 2_
+0000ca00: 6365 6e74 6572 5f62 6f74 746f 6d5f 6120  center_bottom_a 
+0000ca10: 7d7d 3c2f 6469 763e 0a20 2020 2020 2020  }}</div>.       
+0000ca20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ca30: 2020 2020 2020 2020 2020 2020 203c 6469               <di
+0000ca40: 7620 636c 6173 733d 227b 2520 626c 6f63  v class="{% bloc
+0000ca50: 6b20 325f 6365 6e74 6572 5f62 6f74 746f  k 2_center_botto
+0000ca60: 6d5f 6162 5f62 2025 7d63 6f6c 2d31 3220  m_ab_b %}col-12 
+0000ca70: 636f 6c2d 6d64 2d34 7b25 2065 6e64 626c  col-md-4{% endbl
+0000ca80: 6f63 6b20 257d 223e 7b7b 2032 5f63 656e  ock %}">{{ 2_cen
+0000ca90: 7465 725f 626f 7474 6f6d 5f62 207d 7d3c  ter_bottom_b }}<
+0000caa0: 2f64 6976 3e0a 2020 2020 2020 2020 2020  /div>.          
+0000cab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cac0: 2020 2020 2020 7b25 2065 6c69 6620 325f        {% elif 2_
+0000cad0: 6365 6e74 6572 5f62 6f74 746f 6d5f 6120  center_bottom_a 
+0000cae0: 616e 6420 325f 6365 6e74 6572 5f62 6f74  and 2_center_bot
+0000caf0: 746f 6d5f 6320 257d 0a20 2020 2020 2020  tom_c %}.       
 0000cb00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cb10: 3c21 2d2d 2042 7569 6c64 2072 6967 6874  <!-- Build right
-0000cb20: 2063 6f6c 756d 6e20 2d2d 3e0a 2020 2020   column -->.    
-0000cb30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cb40: 2020 2020 7b25 2069 6620 325f 7269 6768      {% if 2_righ
-0000cb50: 745f 6120 6f72 2032 5f72 6967 6874 5f62  t_a or 2_right_b
-0000cb60: 2025 7d0a 2020 2020 2020 2020 2020 2020   %}.            
-0000cb70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cb80: 7b25 2069 6620 325f 7269 6768 745f 6120  {% if 2_right_a 
-0000cb90: 616e 6420 325f 7269 6768 745f 6220 257d  and 2_right_b %}
-0000cba0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000cbb0: 2020 2020 2020 2020 2020 2020 203c 6469               <di
-0000cbc0: 7620 636c 6173 733d 227b 2520 626c 6f63  v class="{% bloc
-0000cbd0: 6b20 325f 7269 6768 745f 6162 2025 7d63  k 2_right_ab %}c
-0000cbe0: 6f6c 2d31 3220 636f 6c2d 6c67 2d34 206d  ol-12 col-lg-4 m
-0000cbf0: 742d 3520 6d74 2d6c 672d 307b 2520 656e  t-5 mt-lg-0{% en
-0000cc00: 6462 6c6f 636b 2025 7d22 3e0a 2020 2020  dblock %}">.    
-0000cc10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cc20: 2020 2020 2020 2020 7b25 2065 6c69 6620          {% elif 
-0000cc30: 325f 7269 6768 745f 6120 257d 0a20 2020  2_right_a %}.   
-0000cc40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cc50: 2020 2020 2020 2020 203c 6469 7620 636c           <div cl
-0000cc60: 6173 733d 227b 2520 626c 6f63 6b20 325f  ass="{% block 2_
-0000cc70: 7269 6768 745f 6120 257d 636f 6c2d 3132  right_a %}col-12
-0000cc80: 2063 6f6c 2d6c 672d 3320 6d74 2d35 206d   col-lg-3 mt-5 m
-0000cc90: 742d 6c67 2d30 7b25 2065 6e64 626c 6f63  t-lg-0{% endbloc
-0000cca0: 6b20 257d 223e 0a20 2020 2020 2020 2020  k %}">.         
-0000ccb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ccc0: 2020 207b 2520 656c 7365 2025 7d0a 2020     {% else %}.  
-0000ccd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cce0: 2020 2020 2020 2020 2020 3c64 6976 2063            <div c
-0000ccf0: 6c61 7373 3d22 7b25 2062 6c6f 636b 2032  lass="{% block 2
-0000cd00: 5f72 6967 6874 5f62 2025 7d63 6f6c 2d31  _right_b %}col-1
-0000cd10: 3220 636f 6c2d 6c67 2d33 206f 6666 7365  2 col-lg-3 offse
-0000cd20: 742d 6c67 2d31 206d 742d 3520 6d74 2d6c  t-lg-1 mt-5 mt-l
-0000cd30: 672d 307b 2520 656e 6462 6c6f 636b 2025  g-0{% endblock %
-0000cd40: 7d22 3e0a 2020 2020 2020 2020 2020 2020  }">.            
-0000cd50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cd60: 7b25 2065 6e64 6966 2025 7d0a 2020 2020  {% endif %}.    
-0000cd70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cd80: 2020 2020 2020 2020 2020 2020 3c64 6976              <div
-0000cd90: 2063 6c61 7373 3d22 726f 7722 3e0a 2020   class="row">.  
-0000cda0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cb10: 2020 2020 2020 2020 2020 2020 203c 6469               <di
+0000cb20: 7620 636c 6173 733d 227b 2520 626c 6f63  v class="{% bloc
+0000cb30: 6b20 325f 6365 6e74 6572 5f62 6f74 746f  k 2_center_botto
+0000cb40: 6d5f 6163 5f61 2025 7d63 6f6c 2d31 3220  m_ac_a %}col-12 
+0000cb50: 636f 6c2d 6d64 2d36 7b25 2065 6e64 626c  col-md-6{% endbl
+0000cb60: 6f63 6b20 257d 223e 7b7b 2032 5f63 656e  ock %}">{{ 2_cen
+0000cb70: 7465 725f 626f 7474 6f6d 5f61 207d 7d3c  ter_bottom_a }}<
+0000cb80: 2f64 6976 3e0a 2020 2020 2020 2020 2020  /div>.          
+0000cb90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cba0: 2020 2020 2020 2020 2020 3c64 6976 2063            <div c
+0000cbb0: 6c61 7373 3d22 7b25 2062 6c6f 636b 2032  lass="{% block 2
+0000cbc0: 5f63 656e 7465 725f 626f 7474 6f6d 5f61  _center_bottom_a
+0000cbd0: 635f 6320 257d 636f 6c2d 3132 2063 6f6c  c_c %}col-12 col
+0000cbe0: 2d6d 642d 367b 2520 656e 6462 6c6f 636b  -md-6{% endblock
+0000cbf0: 2025 7d22 3e7b 7b20 325f 6365 6e74 6572   %}">{{ 2_center
+0000cc00: 5f62 6f74 746f 6d5f 6320 7d7d 3c2f 6469  _bottom_c }}</di
+0000cc10: 763e 0a20 2020 2020 2020 2020 2020 2020  v>.             
+0000cc20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cc30: 2020 207b 2520 656c 6966 2032 5f63 656e     {% elif 2_cen
+0000cc40: 7465 725f 626f 7474 6f6d 5f62 2061 6e64  ter_bottom_b and
+0000cc50: 2032 5f63 656e 7465 725f 626f 7474 6f6d   2_center_bottom
+0000cc60: 5f63 2025 7d0a 2020 2020 2020 2020 2020  _c %}.          
+0000cc70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cc80: 2020 2020 2020 2020 2020 3c64 6976 2063            <div c
+0000cc90: 6c61 7373 3d22 7b25 2062 6c6f 636b 2032  lass="{% block 2
+0000cca0: 5f63 656e 7465 725f 626f 7474 6f6d 5f62  _center_bottom_b
+0000ccb0: 635f 6220 257d 636f 6c2d 3132 2063 6f6c  c_b %}col-12 col
+0000ccc0: 2d6d 642d 347b 2520 656e 6462 6c6f 636b  -md-4{% endblock
+0000ccd0: 2025 7d22 3e7b 7b20 325f 6365 6e74 6572   %}">{{ 2_center
+0000cce0: 5f62 6f74 746f 6d5f 6220 7d7d 3c2f 6469  _bottom_b }}</di
+0000ccf0: 763e 0a20 2020 2020 2020 2020 2020 2020  v>.             
+0000cd00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cd10: 2020 2020 2020 203c 6469 7620 636c 6173         <div clas
+0000cd20: 733d 227b 2520 626c 6f63 6b20 325f 6365  s="{% block 2_ce
+0000cd30: 6e74 6572 5f62 6f74 746f 6d5f 6263 5f63  nter_bottom_bc_c
+0000cd40: 2025 7d63 6f6c 2d31 3220 636f 6c2d 6d64   %}col-12 col-md
+0000cd50: 2d38 7b25 2065 6e64 626c 6f63 6b20 257d  -8{% endblock %}
+0000cd60: 223e 7b7b 2032 5f63 656e 7465 725f 626f  ">{{ 2_center_bo
+0000cd70: 7474 6f6d 5f63 207d 7d3c 2f64 6976 3e0a  ttom_c }}</div>.
+0000cd80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cd90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cda0: 7b25 2065 6c73 6520 257d 0a20 2020 2020  {% else %}.     
 0000cdb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cdc0: 2020 7b25 2069 6620 325f 7269 6768 745f    {% if 2_right_
-0000cdd0: 6120 616e 6420 325f 7269 6768 745f 6220  a and 2_right_b 
-0000cde0: 257d 0a20 2020 2020 2020 2020 2020 2020  %}.             
-0000cdf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ce00: 2020 2020 2020 203c 6469 7620 636c 6173         <div clas
-0000ce10: 733d 227b 2520 626c 6f63 6b20 325f 7269  s="{% block 2_ri
-0000ce20: 6768 745f 6162 5f61 2025 7d63 6f6c 2d31  ght_ab_a %}col-1
-0000ce30: 3220 636f 6c2d 6c67 2d36 7b25 2065 6e64  2 col-lg-6{% end
-0000ce40: 626c 6f63 6b20 257d 223e 7b7b 2032 5f72  block %}">{{ 2_r
-0000ce50: 6967 6874 5f61 207d 7d3c 2f64 6976 3e0a  ight_a }}</div>.
+0000cdc0: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+0000cdd0: 6469 7620 636c 6173 733d 2263 6f6c 2d31  div class="col-1
+0000cde0: 3222 3e7b 7b20 325f 6365 6e74 6572 5f62  2">{{ 2_center_b
+0000cdf0: 6f74 746f 6d5f 6120 7d7d 7b7b 2032 5f63  ottom_a }}{{ 2_c
+0000ce00: 656e 7465 725f 626f 7474 6f6d 5f62 207d  enter_bottom_b }
+0000ce10: 7d7b 7b20 325f 6365 6e74 6572 5f62 6f74  }{{ 2_center_bot
+0000ce20: 746f 6d5f 6320 7d7d 3c2f 6469 763e 0a20  tom_c }}</div>. 
+0000ce30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ce40: 2020 2020 2020 2020 2020 2020 2020 207b                 {
+0000ce50: 2520 656e 6469 6620 257d 0a20 2020 2020  % endif %}.     
 0000ce60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ce70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ce80: 2020 2020 3c64 6976 2063 6c61 7373 3d22      <div class="
-0000ce90: 7b25 2062 6c6f 636b 2032 5f72 6967 6874  {% block 2_right
-0000cea0: 5f61 625f 6220 257d 636f 6c2d 3132 2063  _ab_b %}col-12 c
-0000ceb0: 6f6c 2d6c 672d 367b 2520 656e 6462 6c6f  ol-lg-6{% endblo
-0000cec0: 636b 2025 7d22 3e7b 7b20 325f 7269 6768  ck %}">{{ 2_righ
-0000ced0: 745f 6220 7d7d 3c2f 6469 763e 0a20 2020  t_b }}</div>.   
-0000cee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cf00: 207b 2520 656c 6966 2032 5f72 6967 6874   {% elif 2_right
-0000cf10: 5f61 2025 7d0a 2020 2020 2020 2020 2020  _a %}.          
-0000cf20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cf30: 2020 2020 2020 2020 2020 3c64 6976 2063            <div c
-0000cf40: 6c61 7373 3d22 636f 6c2d 3132 223e 7b7b  lass="col-12">{{
-0000cf50: 2032 5f72 6967 6874 5f61 207d 7d3c 2f64   2_right_a }}</d
-0000cf60: 6976 3e0a 2020 2020 2020 2020 2020 2020  iv>.            
+0000ce70: 2020 2020 2020 203c 2f64 6976 3e0a 2020         </div>.  
+0000ce80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ce90: 2020 2020 2020 2020 2020 7b25 2065 6e64            {% end
+0000cea0: 6966 2025 7d0a 0a20 2020 2020 2020 2020  if %}..         
+0000ceb0: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+0000cec0: 2f64 6976 3e0a 2020 2020 2020 2020 2020  /div>.          
+0000ced0: 2020 2020 2020 2020 2020 2020 2020 3c21                <!
+0000cee0: 2d2d 2045 6e64 2043 656e 7465 7220 636f  -- End Center co
+0000cef0: 6c75 6d6e 202d 2d3e 0a0a 2020 2020 2020  lumn -->..      
+0000cf00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cf10: 2020 3c21 2d2d 2042 7569 6c64 2072 6967    <!-- Build rig
+0000cf20: 6874 2063 6f6c 756d 6e20 2d2d 3e0a 2020  ht column -->.  
+0000cf30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cf40: 2020 2020 2020 7b25 2069 6620 325f 7269        {% if 2_ri
+0000cf50: 6768 745f 6120 6f72 2032 5f72 6967 6874  ght_a or 2_right
+0000cf60: 5f62 2025 7d0a 2020 2020 2020 2020 2020  _b %}.          
 0000cf70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cf80: 2020 2020 2020 2020 7b25 2065 6c73 6520          {% else 
-0000cf90: 257d 0a20 2020 2020 2020 2020 2020 2020  %}.             
-0000cfa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cfb0: 2020 2020 2020 203c 6469 7620 636c 6173         <div clas
-0000cfc0: 733d 2263 6f6c 2d31 3222 3e7b 7b20 325f  s="col-12">{{ 2_
-0000cfd0: 7269 6768 745f 6220 7d7d 3c2f 6469 763e  right_b }}</div>
-0000cfe0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000cff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d000: 2020 2020 207b 2520 656e 6469 6620 257d       {% endif %}
-0000d010: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000d020: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d030: 203c 2f64 6976 3e0a 2020 2020 2020 2020   </div>.        
+0000cf80: 2020 7b25 2069 6620 325f 7269 6768 745f    {% if 2_right_
+0000cf90: 6120 616e 6420 325f 7269 6768 745f 6220  a and 2_right_b 
+0000cfa0: 257d 0a20 2020 2020 2020 2020 2020 2020  %}.             
+0000cfb0: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+0000cfc0: 6469 7620 636c 6173 733d 227b 2520 626c  div class="{% bl
+0000cfd0: 6f63 6b20 325f 7269 6768 745f 6162 2025  ock 2_right_ab %
+0000cfe0: 7d63 6f6c 2d31 3220 636f 6c2d 6c67 2d34  }col-12 col-lg-4
+0000cff0: 206d 742d 3520 6d74 2d6c 672d 307b 2520   mt-5 mt-lg-0{% 
+0000d000: 656e 6462 6c6f 636b 2025 7d22 3e0a 2020  endblock %}">.  
+0000d010: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d020: 2020 2020 2020 2020 2020 7b25 2065 6c69            {% eli
+0000d030: 6620 325f 7269 6768 745f 6120 257d 0a20  f 2_right_a %}. 
 0000d040: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d050: 2020 2020 3c2f 6469 763e 0a20 2020 2020      </div>.     
-0000d060: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d070: 2020 207b 2520 656e 6469 6620 257d 0a0a     {% endif %}..
-0000d080: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d090: 2020 2020 3c21 2d2d 204e 6f20 626c 6f63      <!-- No bloc
-0000d0a0: 6b73 2069 6e20 6365 6e74 6572 2070 6f73  ks in center pos
-0000d0b0: 6974 696f 6e73 202d 2d3e 0a20 2020 2020  itions -->.     
-0000d0c0: 2020 2020 2020 2020 2020 2020 2020 207b                 {
-0000d0d0: 2520 656c 7365 2025 7d0a 2020 2020 2020  % else %}.      
-0000d0e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d0f0: 2020 7b25 2069 6620 325f 6c65 6674 5f61    {% if 2_left_a
-0000d100: 206f 7220 325f 6c65 6674 5f62 2025 7d0a   or 2_left_b %}.
-0000d110: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d120: 2020 2020 2020 2020 2020 2020 7b25 2069              {% i
-0000d130: 6620 325f 6c65 6674 5f61 2061 6e64 2032  f 2_left_a and 2
-0000d140: 5f6c 6566 745f 6220 257d 0a20 2020 2020  _left_b %}.     
+0000d050: 2020 2020 2020 2020 2020 203c 6469 7620             <div 
+0000d060: 636c 6173 733d 227b 2520 626c 6f63 6b20  class="{% block 
+0000d070: 325f 7269 6768 745f 6120 257d 636f 6c2d  2_right_a %}col-
+0000d080: 3132 2063 6f6c 2d6c 672d 3320 6d74 2d35  12 col-lg-3 mt-5
+0000d090: 206d 742d 6c67 2d30 7b25 2065 6e64 626c   mt-lg-0{% endbl
+0000d0a0: 6f63 6b20 257d 223e 0a20 2020 2020 2020  ock %}">.       
+0000d0b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d0c0: 2020 2020 207b 2520 656c 7365 2025 7d0a       {% else %}.
+0000d0d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d0e0: 2020 2020 2020 2020 2020 2020 3c64 6976              <div
+0000d0f0: 2063 6c61 7373 3d22 7b25 2062 6c6f 636b   class="{% block
+0000d100: 2032 5f72 6967 6874 5f62 2025 7d63 6f6c   2_right_b %}col
+0000d110: 2d31 3220 636f 6c2d 6c67 2d33 206f 6666  -12 col-lg-3 off
+0000d120: 7365 742d 6c67 2d31 206d 742d 3520 6d74  set-lg-1 mt-5 mt
+0000d130: 2d6c 672d 307b 2520 656e 6462 6c6f 636b  -lg-0{% endblock
+0000d140: 2025 7d22 3e0a 2020 2020 2020 2020 2020   %}">.          
 0000d150: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d160: 2020 2020 2020 203c 6469 7620 636c 6173         <div clas
-0000d170: 733d 227b 2520 626c 6f63 6b20 325f 6c65  s="{% block 2_le
-0000d180: 6674 5f6e 6f5f 6365 6e74 6572 5f61 6220  ft_no_center_ab 
-0000d190: 257d 636f 6c2d 3132 2063 6f6c 2d6d 642d  %}col-12 col-md-
-0000d1a0: 367b 2520 656e 6462 6c6f 636b 2025 7d22  6{% endblock %}"
-0000d1b0: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
-0000d1c0: 2020 2020 2020 2020 2020 2020 2020 7b25                {%
-0000d1d0: 2065 6c69 6620 325f 6c65 6674 5f61 2025   elif 2_left_a %
-0000d1e0: 7d0a 2020 2020 2020 2020 2020 2020 2020  }.              
-0000d1f0: 2020 2020 2020 2020 2020 2020 2020 3c64                <d
-0000d200: 6976 2063 6c61 7373 3d22 7b25 2062 6c6f  iv class="{% blo
-0000d210: 636b 2032 5f6c 6566 745f 6e6f 5f63 656e  ck 2_left_no_cen
-0000d220: 7465 725f 6120 257d 636f 6c2d 3132 2063  ter_a %}col-12 c
-0000d230: 6f6c 2d6d 642d 367b 2520 656e 6462 6c6f  ol-md-6{% endblo
-0000d240: 636b 2025 7d22 3e0a 2020 2020 2020 2020  ck %}">.        
-0000d250: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d260: 2020 2020 7b25 2065 6c69 6620 325f 6c65      {% elif 2_le
-0000d270: 6674 5f62 2025 7d0a 2020 2020 2020 2020  ft_b %}.        
-0000d280: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d290: 2020 2020 3c64 6976 2063 6c61 7373 3d22      <div class="
-0000d2a0: 7b25 2062 6c6f 636b 2032 5f6c 6566 745f  {% block 2_left_
-0000d2b0: 6e6f 5f63 656e 7465 725f 6220 257d 636f  no_center_b %}co
-0000d2c0: 6c2d 3132 2063 6f6c 2d6d 642d 367b 2520  l-12 col-md-6{% 
-0000d2d0: 656e 6462 6c6f 636b 2025 7d22 3e0a 2020  endblock %}">.  
+0000d160: 2020 7b25 2065 6e64 6966 2025 7d0a 2020    {% endif %}.  
+0000d170: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d180: 2020 2020 2020 2020 2020 2020 2020 3c64                <d
+0000d190: 6976 2063 6c61 7373 3d22 726f 7722 3e0a  iv class="row">.
+0000d1a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d1b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d1c0: 2020 2020 7b25 2069 6620 325f 7269 6768      {% if 2_righ
+0000d1d0: 745f 6120 616e 6420 325f 7269 6768 745f  t_a and 2_right_
+0000d1e0: 6220 257d 0a20 2020 2020 2020 2020 2020  b %}.           
+0000d1f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d200: 2020 2020 2020 2020 203c 6469 7620 636c           <div cl
+0000d210: 6173 733d 227b 2520 626c 6f63 6b20 325f  ass="{% block 2_
+0000d220: 7269 6768 745f 6162 5f61 2025 7d63 6f6c  right_ab_a %}col
+0000d230: 2d31 3220 636f 6c2d 6c67 2d36 7b25 2065  -12 col-lg-6{% e
+0000d240: 6e64 626c 6f63 6b20 257d 223e 7b7b 2032  ndblock %}">{{ 2
+0000d250: 5f72 6967 6874 5f61 207d 7d3c 2f64 6976  _right_a }}</div
+0000d260: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
+0000d270: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d280: 2020 2020 2020 3c64 6976 2063 6c61 7373        <div class
+0000d290: 3d22 7b25 2062 6c6f 636b 2032 5f72 6967  ="{% block 2_rig
+0000d2a0: 6874 5f61 625f 6220 257d 636f 6c2d 3132  ht_ab_b %}col-12
+0000d2b0: 2063 6f6c 2d6c 672d 367b 2520 656e 6462   col-lg-6{% endb
+0000d2c0: 6c6f 636b 2025 7d22 3e7b 7b20 325f 7269  lock %}">{{ 2_ri
+0000d2d0: 6768 745f 6220 7d7d 3c2f 6469 763e 0a20  ght_b }}</div>. 
 0000d2e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d2f0: 2020 2020 2020 2020 2020 7b25 2065 6e64            {% end
-0000d300: 6966 2025 7d0a 2020 2020 2020 2020 2020  if %}.          
-0000d310: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d320: 2020 2020 2020 3c64 6976 2063 6c61 7373        <div class
-0000d330: 3d22 726f 7722 3e0a 2020 2020 2020 2020  ="row">.        
-0000d340: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d350: 2020 2020 2020 2020 2020 2020 7b25 2069              {% i
-0000d360: 6620 325f 6c65 6674 5f61 2061 6e64 2032  f 2_left_a and 2
-0000d370: 5f6c 6566 745f 6220 257d 0a20 2020 2020  _left_b %}.     
-0000d380: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d390: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-0000d3a0: 6469 7620 636c 6173 733d 227b 2520 626c  div class="{% bl
-0000d3b0: 6f63 6b20 325f 6c65 6674 5f6e 6f5f 6365  ock 2_left_no_ce
-0000d3c0: 6e74 6572 5f61 625f 6120 257d 636f 6c2d  nter_ab_a %}col-
-0000d3d0: 3132 2063 6f6c 2d6d 642d 367b 2520 656e  12 col-md-6{% en
-0000d3e0: 6462 6c6f 636b 2025 7d22 3e7b 7b20 325f  dblock %}">{{ 2_
-0000d3f0: 6c65 6674 5f61 207d 7d3c 2f64 6976 3e0a  left_a }}</div>.
-0000d400: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d410: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d420: 2020 2020 3c64 6976 2063 6c61 7373 3d22      <div class="
-0000d430: 7b25 2062 6c6f 636b 2032 5f6c 6566 745f  {% block 2_left_
-0000d440: 6e6f 5f63 656e 7465 725f 6162 5f62 2025  no_center_ab_b %
-0000d450: 7d63 6f6c 2d31 3220 636f 6c2d 6d64 2d36  }col-12 col-md-6
-0000d460: 7b25 2065 6e64 626c 6f63 6b20 257d 223e  {% endblock %}">
-0000d470: 7b7b 2032 5f6c 6566 745f 6220 7d7d 3c2f  {{ 2_left_b }}</
-0000d480: 6469 763e 0a20 2020 2020 2020 2020 2020  div>.           
-0000d490: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d4a0: 2020 2020 2020 2020 207b 2520 656c 6966           {% elif
-0000d4b0: 2032 5f6c 6566 745f 6120 257d 0a20 2020   2_left_a %}.   
+0000d2f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d300: 2020 207b 2520 656c 6966 2032 5f72 6967     {% elif 2_rig
+0000d310: 6874 5f61 2025 7d0a 2020 2020 2020 2020  ht_a %}.        
+0000d320: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d330: 2020 2020 2020 2020 2020 2020 3c64 6976              <div
+0000d340: 2063 6c61 7373 3d22 636f 6c2d 3132 223e   class="col-12">
+0000d350: 7b7b 2032 5f72 6967 6874 5f61 207d 7d3c  {{ 2_right_a }}<
+0000d360: 2f64 6976 3e0a 2020 2020 2020 2020 2020  /div>.          
+0000d370: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d380: 2020 2020 2020 2020 2020 7b25 2065 6c73            {% els
+0000d390: 6520 257d 0a20 2020 2020 2020 2020 2020  e %}.           
+0000d3a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d3b0: 2020 2020 2020 2020 203c 6469 7620 636c           <div cl
+0000d3c0: 6173 733d 2263 6f6c 2d31 3222 3e7b 7b20  ass="col-12">{{ 
+0000d3d0: 325f 7269 6768 745f 6220 7d7d 3c2f 6469  2_right_b }}</di
+0000d3e0: 763e 0a20 2020 2020 2020 2020 2020 2020  v>.             
+0000d3f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d400: 2020 2020 2020 207b 2520 656e 6469 6620         {% endif 
+0000d410: 257d 0a20 2020 2020 2020 2020 2020 2020  %}.             
+0000d420: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d430: 2020 203c 2f64 6976 3e0a 2020 2020 2020     </div>.      
+0000d440: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d450: 2020 2020 2020 3c2f 6469 763e 0a20 2020        </div>.   
+0000d460: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d470: 2020 2020 207b 2520 656e 6469 6620 257d       {% endif %}
+0000d480: 0a0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000d490: 2020 2020 2020 3c21 2d2d 204e 6f20 626c        <!-- No bl
+0000d4a0: 6f63 6b73 2069 6e20 6365 6e74 6572 2070  ocks in center p
+0000d4b0: 6f73 6974 696f 6e73 202d 2d3e 0a20 2020  ositions -->.   
 0000d4c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d4d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d4e0: 203c 6469 7620 636c 6173 733d 2263 6f6c   <div class="col
-0000d4f0: 2d31 3222 3e7b 7b20 325f 6c65 6674 5f61  -12">{{ 2_left_a
-0000d500: 207d 7d3c 2f64 6976 3e0a 2020 2020 2020   }}</div>.      
-0000d510: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d4d0: 207b 2520 656c 7365 2025 7d0a 2020 2020   {% else %}.    
+0000d4e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d4f0: 2020 2020 7b25 2069 6620 325f 6c65 6674      {% if 2_left
+0000d500: 5f61 206f 7220 325f 6c65 6674 5f62 2025  _a or 2_left_b %
+0000d510: 7d0a 2020 2020 2020 2020 2020 2020 2020  }.              
 0000d520: 2020 2020 2020 2020 2020 2020 2020 7b25                {%
-0000d530: 2065 6c73 6520 257d 0a20 2020 2020 2020   else %}.       
-0000d540: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d550: 2020 2020 2020 2020 2020 2020 203c 6469               <di
-0000d560: 7620 636c 6173 733d 2263 6f6c 2d31 3222  v class="col-12"
-0000d570: 3e7b 7b20 325f 6c65 6674 5f62 207d 7d3c  >{{ 2_left_b }}<
-0000d580: 2f64 6976 3e0a 2020 2020 2020 2020 2020  /div>.          
-0000d590: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d5a0: 2020 2020 2020 2020 2020 7b25 2065 6e64            {% end
-0000d5b0: 6966 2025 7d0a 2020 2020 2020 2020 2020  if %}.          
+0000d530: 2069 6620 325f 6c65 6674 5f61 2061 6e64   if 2_left_a and
+0000d540: 2032 5f6c 6566 745f 6220 257d 0a20 2020   2_left_b %}.   
+0000d550: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d560: 2020 2020 2020 2020 203c 6469 7620 636c           <div cl
+0000d570: 6173 733d 227b 2520 626c 6f63 6b20 325f  ass="{% block 2_
+0000d580: 6c65 6674 5f6e 6f5f 6365 6e74 6572 5f61  left_no_center_a
+0000d590: 6220 257d 636f 6c2d 3132 2063 6f6c 2d6d  b %}col-12 col-m
+0000d5a0: 642d 367b 2520 656e 6462 6c6f 636b 2025  d-6{% endblock %
+0000d5b0: 7d22 3e0a 2020 2020 2020 2020 2020 2020  }">.            
 0000d5c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d5d0: 2020 2020 2020 3c2f 6469 763e 0a20 2020        </div>.   
-0000d5e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d5f0: 2020 2020 2020 2020 203c 2f64 6976 3e0a           </div>.
-0000d600: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d610: 2020 2020 2020 2020 7b25 2065 6e64 6966          {% endif
-0000d620: 2025 7d0a 0a20 2020 2020 2020 2020 2020   %}..           
-0000d630: 2020 2020 2020 2020 2020 2020 207b 2520               {% 
-0000d640: 6966 2032 5f72 6967 6874 5f61 206f 7220  if 2_right_a or 
-0000d650: 325f 7269 6768 745f 6220 257d 0a20 2020  2_right_b %}.   
-0000d660: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d670: 2020 2020 2020 2020 207b 2520 6966 2032           {% if 2
-0000d680: 5f72 6967 6874 5f61 2061 6e64 2032 5f72  _right_a and 2_r
-0000d690: 6967 6874 5f62 2025 7d0a 2020 2020 2020  ight_b %}.      
-0000d6a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d6b0: 2020 2020 2020 3c64 6976 2063 6c61 7373        <div class
-0000d6c0: 3d22 7b25 2062 6c6f 636b 2032 5f72 6967  ="{% block 2_rig
-0000d6d0: 6874 5f6e 6f5f 6365 6e74 6572 5f61 6220  ht_no_center_ab 
-0000d6e0: 257d 636f 6c2d 3132 2063 6f6c 2d6d 642d  %}col-12 col-md-
-0000d6f0: 367b 2520 656e 6462 6c6f 636b 2025 7d22  6{% endblock %}"
-0000d700: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
-0000d710: 2020 2020 2020 2020 2020 2020 2020 7b25                {%
-0000d720: 2065 6c69 6620 325f 7269 6768 745f 6120   elif 2_right_a 
-0000d730: 257d 0a20 2020 2020 2020 2020 2020 2020  %}.             
-0000d740: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-0000d750: 6469 7620 636c 6173 733d 227b 2520 626c  div class="{% bl
-0000d760: 6f63 6b20 325f 7269 6768 745f 6e6f 5f63  ock 2_right_no_c
-0000d770: 656e 7465 725f 6120 257d 636f 6c2d 3132  enter_a %}col-12
-0000d780: 2063 6f6c 2d6d 642d 367b 2520 656e 6462   col-md-6{% endb
-0000d790: 6c6f 636b 2025 7d22 3e0a 2020 2020 2020  lock %}">.      
-0000d7a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d7b0: 2020 2020 2020 7b25 2065 6c69 6620 325f        {% elif 2_
-0000d7c0: 7269 6768 745f 6220 257d 0a20 2020 2020  right_b %}.     
-0000d7d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d7e0: 2020 2020 2020 203c 6469 7620 636c 6173         <div clas
-0000d7f0: 733d 227b 2520 626c 6f63 6b20 325f 7269  s="{% block 2_ri
-0000d800: 6768 745f 6e6f 5f63 656e 7465 725f 6220  ght_no_center_b 
-0000d810: 257d 636f 6c2d 3132 2063 6f6c 2d6d 642d  %}col-12 col-md-
-0000d820: 367b 2520 656e 6462 6c6f 636b 2025 7d22  6{% endblock %}"
-0000d830: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
-0000d840: 2020 2020 2020 2020 2020 2020 2020 7b25                {%
-0000d850: 2065 6e64 6966 2025 7d0a 2020 2020 2020   endif %}.      
-0000d860: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d870: 2020 2020 2020 2020 2020 3c64 6976 2063            <div c
-0000d880: 6c61 7373 3d22 726f 7722 3e0a 2020 2020  lass="row">.    
+0000d5d0: 7b25 2065 6c69 6620 325f 6c65 6674 5f61  {% elif 2_left_a
+0000d5e0: 2025 7d0a 2020 2020 2020 2020 2020 2020   %}.            
+0000d5f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d600: 3c64 6976 2063 6c61 7373 3d22 7b25 2062  <div class="{% b
+0000d610: 6c6f 636b 2032 5f6c 6566 745f 6e6f 5f63  lock 2_left_no_c
+0000d620: 656e 7465 725f 6120 257d 636f 6c2d 3132  enter_a %}col-12
+0000d630: 2063 6f6c 2d6d 642d 367b 2520 656e 6462   col-md-6{% endb
+0000d640: 6c6f 636b 2025 7d22 3e0a 2020 2020 2020  lock %}">.      
+0000d650: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d660: 2020 2020 2020 7b25 2065 6c69 6620 325f        {% elif 2_
+0000d670: 6c65 6674 5f62 2025 7d0a 2020 2020 2020  left_b %}.      
+0000d680: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d690: 2020 2020 2020 3c64 6976 2063 6c61 7373        <div class
+0000d6a0: 3d22 7b25 2062 6c6f 636b 2032 5f6c 6566  ="{% block 2_lef
+0000d6b0: 745f 6e6f 5f63 656e 7465 725f 6220 257d  t_no_center_b %}
+0000d6c0: 636f 6c2d 3132 2063 6f6c 2d6d 642d 367b  col-12 col-md-6{
+0000d6d0: 2520 656e 6462 6c6f 636b 2025 7d22 3e0a  % endblock %}">.
+0000d6e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d6f0: 2020 2020 2020 2020 2020 2020 7b25 2065              {% e
+0000d700: 6e64 6966 2025 7d0a 2020 2020 2020 2020  ndif %}.        
+0000d710: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d720: 2020 2020 2020 2020 3c64 6976 2063 6c61          <div cla
+0000d730: 7373 3d22 726f 7722 3e0a 2020 2020 2020  ss="row">.      
+0000d740: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d750: 2020 2020 2020 2020 2020 2020 2020 7b25                {%
+0000d760: 2069 6620 325f 6c65 6674 5f61 2061 6e64   if 2_left_a and
+0000d770: 2032 5f6c 6566 745f 6220 257d 0a20 2020   2_left_b %}.   
+0000d780: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d790: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d7a0: 203c 6469 7620 636c 6173 733d 227b 2520   <div class="{% 
+0000d7b0: 626c 6f63 6b20 325f 6c65 6674 5f6e 6f5f  block 2_left_no_
+0000d7c0: 6365 6e74 6572 5f61 625f 6120 257d 636f  center_ab_a %}co
+0000d7d0: 6c2d 3132 2063 6f6c 2d6d 642d 367b 2520  l-12 col-md-6{% 
+0000d7e0: 656e 6462 6c6f 636b 2025 7d22 3e7b 7b20  endblock %}">{{ 
+0000d7f0: 325f 6c65 6674 5f61 207d 7d3c 2f64 6976  2_left_a }}</div
+0000d800: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
+0000d810: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d820: 2020 2020 2020 3c64 6976 2063 6c61 7373        <div class
+0000d830: 3d22 7b25 2062 6c6f 636b 2032 5f6c 6566  ="{% block 2_lef
+0000d840: 745f 6e6f 5f63 656e 7465 725f 6162 5f62  t_no_center_ab_b
+0000d850: 2025 7d63 6f6c 2d31 3220 636f 6c2d 6d64   %}col-12 col-md
+0000d860: 2d36 7b25 2065 6e64 626c 6f63 6b20 257d  -6{% endblock %}
+0000d870: 223e 7b7b 2032 5f6c 6566 745f 6220 7d7d  ">{{ 2_left_b }}
+0000d880: 3c2f 6469 763e 0a20 2020 2020 2020 2020  </div>.         
 0000d890: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d8a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d8b0: 7b25 2069 6620 325f 7269 6768 745f 6120  {% if 2_right_a 
-0000d8c0: 616e 6420 325f 7269 6768 745f 6220 257d  and 2_right_b %}
-0000d8d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000d8e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d8f0: 2020 2020 203c 6469 7620 636c 6173 733d       <div class=
-0000d900: 227b 2520 626c 6f63 6b20 325f 7269 6768  "{% block 2_righ
-0000d910: 745f 6e6f 5f63 656e 7465 725f 6162 5f61  t_no_center_ab_a
-0000d920: 2025 7d63 6f6c 2d31 3220 636f 6c2d 6d64   %}col-12 col-md
-0000d930: 2d36 7b25 2065 6e64 626c 6f63 6b20 257d  -6{% endblock %}
-0000d940: 223e 7b7b 2032 5f72 6967 6874 5f61 207d  ">{{ 2_right_a }
-0000d950: 7d3c 2f64 6976 3e0a 2020 2020 2020 2020  }</div>.        
-0000d960: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d970: 2020 2020 2020 2020 2020 2020 3c64 6976              <div
-0000d980: 2063 6c61 7373 3d22 7b25 2062 6c6f 636b   class="{% block
-0000d990: 2032 5f72 6967 6874 5f6e 6f5f 6365 6e74   2_right_no_cent
-0000d9a0: 6572 5f61 625f 6220 257d 636f 6c2d 3132  er_ab_b %}col-12
-0000d9b0: 2063 6f6c 2d6d 642d 367b 2520 656e 6462   col-md-6{% endb
-0000d9c0: 6c6f 636b 2025 7d22 3e7b 7b20 325f 7269  lock %}">{{ 2_ri
-0000d9d0: 6768 745f 6220 7d7d 2f64 6976 3e0a 2020  ght_b }}/div>.  
+0000d8a0: 2020 2020 2020 2020 2020 207b 2520 656c             {% el
+0000d8b0: 6966 2032 5f6c 6566 745f 6120 257d 0a20  if 2_left_a %}. 
+0000d8c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d8d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d8e0: 2020 203c 6469 7620 636c 6173 733d 2263     <div class="c
+0000d8f0: 6f6c 2d31 3222 3e7b 7b20 325f 6c65 6674  ol-12">{{ 2_left
+0000d900: 5f61 207d 7d3c 2f64 6976 3e0a 2020 2020  _a }}</div>.    
+0000d910: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d920: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d930: 7b25 2065 6c73 6520 257d 0a20 2020 2020  {% else %}.     
+0000d940: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d950: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+0000d960: 6469 7620 636c 6173 733d 2263 6f6c 2d31  div class="col-1
+0000d970: 3222 3e7b 7b20 325f 6c65 6674 5f62 207d  2">{{ 2_left_b }
+0000d980: 7d3c 2f64 6976 3e0a 2020 2020 2020 2020  }</div>.        
+0000d990: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d9a0: 2020 2020 2020 2020 2020 2020 7b25 2065              {% e
+0000d9b0: 6e64 6966 2025 7d0a 2020 2020 2020 2020  ndif %}.        
+0000d9c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d9d0: 2020 2020 2020 2020 3c2f 6469 763e 0a20          </div>. 
 0000d9e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d9f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000da00: 2020 7b25 2065 6c69 6620 325f 7269 6768    {% elif 2_righ
-0000da10: 745f 6120 257d 0a20 2020 2020 2020 2020  t_a %}.         
-0000da20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000da30: 2020 2020 2020 2020 2020 203c 6469 7620             <div 
-0000da40: 636c 6173 733d 2263 6f6c 2d31 3222 3e7b  class="col-12">{
-0000da50: 7b20 325f 7269 6768 745f 6120 7d7d 3c2f  { 2_right_a }}</
-0000da60: 6469 763e 0a20 2020 2020 2020 2020 2020  div>.           
-0000da70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000da80: 2020 2020 2020 2020 207b 2520 656c 7365           {% else
-0000da90: 2025 7d0a 2020 2020 2020 2020 2020 2020   %}.            
+0000d9f0: 2020 2020 2020 2020 2020 203c 2f64 6976             </div
+0000da00: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
+0000da10: 2020 2020 2020 2020 2020 7b25 2065 6e64            {% end
+0000da20: 6966 2025 7d0a 0a20 2020 2020 2020 2020  if %}..         
+0000da30: 2020 2020 2020 2020 2020 2020 2020 207b                 {
+0000da40: 2520 6966 2032 5f72 6967 6874 5f61 206f  % if 2_right_a o
+0000da50: 7220 325f 7269 6768 745f 6220 257d 0a20  r 2_right_b %}. 
+0000da60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000da70: 2020 2020 2020 2020 2020 207b 2520 6966             {% if
+0000da80: 2032 5f72 6967 6874 5f61 2061 6e64 2032   2_right_a and 2
+0000da90: 5f72 6967 6874 5f62 2025 7d0a 2020 2020  _right_b %}.    
 0000daa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000dab0: 2020 2020 2020 2020 3c64 6976 2063 6c61          <div cla
-0000dac0: 7373 3d22 636f 6c2d 3132 223e 7b7b 2032  ss="col-12">{{ 2
-0000dad0: 5f72 6967 6874 5f62 207d 7d3c 2f64 6976  _right_b }}</div
-0000dae0: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
-0000daf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000db00: 2020 2020 2020 7b25 2065 6e64 6966 2025        {% endif %
-0000db10: 7d0a 2020 2020 2020 2020 2020 2020 2020  }.              
-0000db20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000db30: 2020 3c2f 6469 763e 0a20 2020 2020 2020    </div>.       
+0000dac0: 7373 3d22 7b25 2062 6c6f 636b 2032 5f72  ss="{% block 2_r
+0000dad0: 6967 6874 5f6e 6f5f 6365 6e74 6572 5f61  ight_no_center_a
+0000dae0: 6220 257d 636f 6c2d 3132 2063 6f6c 2d6d  b %}col-12 col-m
+0000daf0: 642d 367b 2520 656e 6462 6c6f 636b 2025  d-6{% endblock %
+0000db00: 7d22 3e0a 2020 2020 2020 2020 2020 2020  }">.            
+0000db10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000db20: 7b25 2065 6c69 6620 325f 7269 6768 745f  {% elif 2_right_
+0000db30: 6120 257d 0a20 2020 2020 2020 2020 2020  a %}.           
 0000db40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000db50: 2020 2020 203c 2f64 6976 3e0a 2020 2020       </div>.    
-0000db60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000db70: 2020 2020 7b25 2065 6e64 6966 2025 7d0a      {% endif %}.
-0000db80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000db90: 2020 2020 207b 2520 656e 6469 6620 257d       {% endif %}
-0000dba0: 0a0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000dbb0: 2020 2020 2020 3c21 2d2d 2042 6c6f 636b        <!-- Block
-0000dbc0: 7320 696e 206d 6964 646c 6520 626f 7474  s in middle bott
-0000dbd0: 6f6d 2070 6f73 6974 696f 6e20 2d2d 3e0a  om position -->.
-0000dbe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dbf0: 2020 2020 7b25 2069 6620 325f 6d69 645f      {% if 2_mid_
-0000dc00: 626f 7474 6f6d 5f61 206f 7220 325f 6d69  bottom_a or 2_mi
-0000dc10: 645f 626f 7474 6f6d 5f62 206f 7220 325f  d_bottom_b or 2_
-0000dc20: 6d69 645f 626f 7474 6f6d 5f63 2025 7d0a  mid_bottom_c %}.
-0000dc30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dc40: 2020 2020 3c64 6976 2063 6c61 7373 3d22      <div class="
-0000dc50: 636f 6c2d 3132 223e 0a20 2020 2020 2020  col-12">.       
+0000db50: 203c 6469 7620 636c 6173 733d 227b 2520   <div class="{% 
+0000db60: 626c 6f63 6b20 325f 7269 6768 745f 6e6f  block 2_right_no
+0000db70: 5f63 656e 7465 725f 6120 257d 636f 6c2d  _center_a %}col-
+0000db80: 3132 2063 6f6c 2d6d 642d 367b 2520 656e  12 col-md-6{% en
+0000db90: 6462 6c6f 636b 2025 7d22 3e0a 2020 2020  dblock %}">.    
+0000dba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dbb0: 2020 2020 2020 2020 7b25 2065 6c69 6620          {% elif 
+0000dbc0: 325f 7269 6768 745f 6220 257d 0a20 2020  2_right_b %}.   
+0000dbd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dbe0: 2020 2020 2020 2020 203c 6469 7620 636c           <div cl
+0000dbf0: 6173 733d 227b 2520 626c 6f63 6b20 325f  ass="{% block 2_
+0000dc00: 7269 6768 745f 6e6f 5f63 656e 7465 725f  right_no_center_
+0000dc10: 6220 257d 636f 6c2d 3132 2063 6f6c 2d6d  b %}col-12 col-m
+0000dc20: 642d 367b 2520 656e 6462 6c6f 636b 2025  d-6{% endblock %
+0000dc30: 7d22 3e0a 2020 2020 2020 2020 2020 2020  }">.            
+0000dc40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dc50: 7b25 2065 6e64 6966 2025 7d0a 2020 2020  {% endif %}.    
 0000dc60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dc70: 203c 6469 7620 636c 6173 733d 2272 6f77   <div class="row
-0000dc80: 223e 0a20 2020 2020 2020 2020 2020 2020  ">.             
-0000dc90: 2020 2020 2020 2020 2020 2020 2020 207b                 {
-0000dca0: 2520 6966 2032 5f6d 6964 5f62 6f74 746f  % if 2_mid_botto
-0000dcb0: 6d5f 6120 616e 6420 325f 6d69 645f 626f  m_a and 2_mid_bo
-0000dcc0: 7474 6f6d 5f62 2061 6e64 2032 5f6d 6964  ttom_b and 2_mid
-0000dcd0: 5f62 6f74 746f 6d5f 6320 257d 0a20 2020  _bottom_c %}.   
+0000dc70: 2020 2020 2020 2020 2020 2020 3c64 6976              <div
+0000dc80: 2063 6c61 7373 3d22 726f 7722 3e0a 2020   class="row">.  
+0000dc90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dcb0: 2020 7b25 2069 6620 325f 7269 6768 745f    {% if 2_right_
+0000dcc0: 6120 616e 6420 325f 7269 6768 745f 6220  a and 2_right_b 
+0000dcd0: 257d 0a20 2020 2020 2020 2020 2020 2020  %}.             
 0000dce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dcf0: 2020 2020 2020 2020 2020 2020 203c 6469               <di
-0000dd00: 7620 636c 6173 733d 227b 2520 626c 6f63  v class="{% bloc
-0000dd10: 6b20 325f 6d69 645f 626f 7474 6f6d 5f61  k 2_mid_bottom_a
-0000dd20: 6263 5f61 2025 7d63 6f6c 2d31 3220 636f  bc_a %}col-12 co
-0000dd30: 6c2d 6d64 2d34 7b25 2065 6e64 626c 6f63  l-md-4{% endbloc
-0000dd40: 6b20 257d 223e 7b7b 2032 5f6d 6964 5f62  k %}">{{ 2_mid_b
-0000dd50: 6f74 746f 6d5f 6120 7d7d 3c2f 6469 763e  ottom_a }}</div>
-0000dd60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000dd70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dd80: 203c 6469 7620 636c 6173 733d 227b 2520   <div class="{% 
-0000dd90: 626c 6f63 6b20 325f 6d69 645f 626f 7474  block 2_mid_bott
-0000dda0: 6f6d 5f61 6263 5f62 2025 7d63 6f6c 2d31  om_abc_b %}col-1
-0000ddb0: 3220 636f 6c2d 6d64 2d34 7b25 2065 6e64  2 col-md-4{% end
-0000ddc0: 626c 6f63 6b20 257d 223e 7b7b 2032 5f6d  block %}">{{ 2_m
-0000ddd0: 6964 5f62 6f74 746f 6d5f 6220 7d7d 3c2f  id_bottom_b }}</
-0000dde0: 6469 763e 0a20 2020 2020 2020 2020 2020  div>.           
+0000dcf0: 2020 2020 2020 203c 6469 7620 636c 6173         <div clas
+0000dd00: 733d 227b 2520 626c 6f63 6b20 325f 7269  s="{% block 2_ri
+0000dd10: 6768 745f 6e6f 5f63 656e 7465 725f 6162  ght_no_center_ab
+0000dd20: 5f61 2025 7d63 6f6c 2d31 3220 636f 6c2d  _a %}col-12 col-
+0000dd30: 6d64 2d36 7b25 2065 6e64 626c 6f63 6b20  md-6{% endblock 
+0000dd40: 257d 223e 7b7b 2032 5f72 6967 6874 5f61  %}">{{ 2_right_a
+0000dd50: 207d 7d3c 2f64 6976 3e0a 2020 2020 2020   }}</div>.      
+0000dd60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dd70: 2020 2020 2020 2020 2020 2020 2020 3c64                <d
+0000dd80: 6976 2063 6c61 7373 3d22 7b25 2062 6c6f  iv class="{% blo
+0000dd90: 636b 2032 5f72 6967 6874 5f6e 6f5f 6365  ck 2_right_no_ce
+0000dda0: 6e74 6572 5f61 625f 6220 257d 636f 6c2d  nter_ab_b %}col-
+0000ddb0: 3132 2063 6f6c 2d6d 642d 367b 2520 656e  12 col-md-6{% en
+0000ddc0: 6462 6c6f 636b 2025 7d22 3e7b 7b20 325f  dblock %}">{{ 2_
+0000ddd0: 7269 6768 745f 6220 7d7d 2f64 6976 3e0a  right_b }}/div>.
+0000dde0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000ddf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000de00: 2020 2020 203c 6469 7620 636c 6173 733d       <div class=
-0000de10: 227b 2520 626c 6f63 6b20 325f 6d69 645f  "{% block 2_mid_
-0000de20: 626f 7474 6f6d 5f61 6263 5f63 2025 7d63  bottom_abc_c %}c
-0000de30: 6f6c 2d31 3220 636f 6c2d 6d64 2d34 7b25  ol-12 col-md-4{%
-0000de40: 2065 6e64 626c 6f63 6b20 257d 223e 7b7b   endblock %}">{{
-0000de50: 2032 5f6d 6964 5f62 6f74 746f 6d5f 6320   2_mid_bottom_c 
-0000de60: 7d7d 3c2f 6469 763e 0a20 2020 2020 2020  }}</div>.       
+0000de00: 2020 2020 7b25 2065 6c69 6620 325f 7269      {% elif 2_ri
+0000de10: 6768 745f 6120 257d 0a20 2020 2020 2020  ght_a %}.       
+0000de20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000de30: 2020 2020 2020 2020 2020 2020 203c 6469               <di
+0000de40: 7620 636c 6173 733d 2263 6f6c 2d31 3222  v class="col-12"
+0000de50: 3e7b 7b20 325f 7269 6768 745f 6120 7d7d  >{{ 2_right_a }}
+0000de60: 3c2f 6469 763e 0a20 2020 2020 2020 2020  </div>.         
 0000de70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000de80: 2020 2020 207b 2520 656c 6966 2032 5f6d       {% elif 2_m
-0000de90: 6964 5f62 6f74 746f 6d5f 6120 616e 6420  id_bottom_a and 
-0000dea0: 325f 6d69 645f 626f 7474 6f6d 5f62 2025  2_mid_bottom_b %
-0000deb0: 7d0a 2020 2020 2020 2020 2020 2020 2020  }.              
-0000dec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ded0: 2020 3c64 6976 2063 6c61 7373 3d22 7b25    <div class="{%
-0000dee0: 2062 6c6f 636b 2032 5f6d 6964 5f62 6f74   block 2_mid_bot
-0000def0: 746f 6d5f 6162 5f61 2025 7d63 6f6c 2d31  tom_ab_a %}col-1
-0000df00: 3220 636f 6c2d 6d64 2d38 7b25 2065 6e64  2 col-md-8{% end
-0000df10: 626c 6f63 6b20 257d 223e 7b7b 2032 5f6d  block %}">{{ 2_m
-0000df20: 6964 5f62 6f74 746f 6d5f 6120 7d7d 3c2f  id_bottom_a }}</
-0000df30: 6469 763e 0a20 2020 2020 2020 2020 2020  div>.           
+0000de80: 2020 2020 2020 2020 2020 207b 2520 656c             {% el
+0000de90: 7365 2025 7d0a 2020 2020 2020 2020 2020  se %}.          
+0000dea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000deb0: 2020 2020 2020 2020 2020 3c64 6976 2063            <div c
+0000dec0: 6c61 7373 3d22 636f 6c2d 3132 223e 7b7b  lass="col-12">{{
+0000ded0: 2032 5f72 6967 6874 5f62 207d 7d3c 2f64   2_right_b }}</d
+0000dee0: 6976 3e0a 2020 2020 2020 2020 2020 2020  iv>.            
+0000def0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000df00: 2020 2020 2020 2020 7b25 2065 6e64 6966          {% endif
+0000df10: 2025 7d0a 2020 2020 2020 2020 2020 2020   %}.            
+0000df20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000df30: 2020 2020 3c2f 6469 763e 0a20 2020 2020      </div>.     
 0000df40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000df50: 2020 2020 203c 6469 7620 636c 6173 733d       <div class=
-0000df60: 227b 2520 626c 6f63 6b20 325f 6d69 645f  "{% block 2_mid_
-0000df70: 626f 7474 6f6d 5f61 625f 6220 257d 636f  bottom_ab_b %}co
-0000df80: 6c2d 3132 2063 6f6c 2d6d 642d 347b 2520  l-12 col-md-4{% 
-0000df90: 656e 6462 6c6f 636b 2025 7d22 3e7b 7b20  endblock %}">{{ 
-0000dfa0: 325f 6d69 645f 626f 7474 6f6d 5f62 207d  2_mid_bottom_b }
-0000dfb0: 7d3c 2f64 6976 3e0a 2020 2020 2020 2020  }</div>.        
-0000dfc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dfd0: 2020 2020 7b25 2065 6c69 6620 325f 6d69      {% elif 2_mi
-0000dfe0: 645f 626f 7474 6f6d 5f61 2061 6e64 2032  d_bottom_a and 2
-0000dff0: 5f6d 6964 5f62 6f74 746f 6d5f 6320 257d  _mid_bottom_c %}
-0000e000: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000e010: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e020: 203c 6469 7620 636c 6173 733d 227b 2520   <div class="{% 
-0000e030: 626c 6f63 6b20 325f 6d69 645f 626f 7474  block 2_mid_bott
-0000e040: 6f6d 5f61 635f 6120 257d 636f 6c2d 3132  om_ac_a %}col-12
-0000e050: 2063 6f6c 2d6d 642d 367b 2520 656e 6462   col-md-6{% endb
-0000e060: 6c6f 636b 2025 7d22 3e7b 7b20 325f 6d69  lock %}">{{ 2_mi
-0000e070: 645f 626f 7474 6f6d 5f61 207d 7d3c 2f64  d_bottom_a }}</d
-0000e080: 6976 3e0a 2020 2020 2020 2020 2020 2020  iv>.            
+0000df50: 2020 2020 2020 203c 2f64 6976 3e0a 2020         </div>.  
+0000df60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000df70: 2020 2020 2020 7b25 2065 6e64 6966 2025        {% endif %
+0000df80: 7d0a 0a20 2020 2020 2020 2020 2020 2020  }..             
+0000df90: 2020 2020 2020 207b 2520 656e 6469 6620         {% endif 
+0000dfa0: 257d 0a0a 2020 2020 2020 2020 2020 2020  %}..            
+0000dfb0: 2020 2020 2020 2020 3c21 2d2d 2042 6c6f          <!-- Blo
+0000dfc0: 636b 7320 696e 206d 6964 646c 6520 626f  cks in middle bo
+0000dfd0: 7474 6f6d 2070 6f73 6974 696f 6e20 2d2d  ttom position --
+0000dfe0: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
+0000dff0: 2020 2020 2020 7b25 2069 6620 325f 6d69        {% if 2_mi
+0000e000: 645f 626f 7474 6f6d 5f61 206f 7220 325f  d_bottom_a or 2_
+0000e010: 6d69 645f 626f 7474 6f6d 5f62 206f 7220  mid_bottom_b or 
+0000e020: 325f 6d69 645f 626f 7474 6f6d 5f63 2025  2_mid_bottom_c %
+0000e030: 7d0a 2020 2020 2020 2020 2020 2020 2020  }.              
+0000e040: 2020 2020 2020 3c64 6976 2063 6c61 7373        <div class
+0000e050: 3d22 636f 6c2d 3132 223e 0a20 2020 2020  ="col-12">.     
+0000e060: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e070: 2020 203c 6469 7620 636c 6173 733d 2272     <div class="r
+0000e080: 6f77 223e 0a20 2020 2020 2020 2020 2020  ow">.           
 0000e090: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e0a0: 2020 2020 3c64 6976 2063 6c61 7373 3d22      <div class="
-0000e0b0: 7b25 2062 6c6f 636b 2032 5f6d 6964 5f62  {% block 2_mid_b
-0000e0c0: 6f74 746f 6d5f 6163 5f63 2025 7d63 6f6c  ottom_ac_c %}col
-0000e0d0: 2d31 3220 636f 6c2d 6d64 2d36 7b25 2065  -12 col-md-6{% e
-0000e0e0: 6e64 626c 6f63 6b20 257d 223e 7b7b 2032  ndblock %}">{{ 2
-0000e0f0: 5f6d 6964 5f62 6f74 746f 6d5f 6320 7d7d  _mid_bottom_c }}
-0000e100: 3c2f 6469 763e 0a20 2020 2020 2020 2020  </div>.         
-0000e110: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e120: 2020 207b 2520 656c 6966 2032 5f6d 6964     {% elif 2_mid
-0000e130: 5f62 6f74 746f 6d5f 6220 616e 6420 325f  _bottom_b and 2_
-0000e140: 6d69 645f 626f 7474 6f6d 5f63 2025 7d0a  mid_bottom_c %}.
-0000e150: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e160: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e170: 3c64 6976 2063 6c61 7373 3d22 7b25 2062  <div class="{% b
-0000e180: 6c6f 636b 2032 5f6d 6964 5f62 6f74 746f  lock 2_mid_botto
-0000e190: 6d5f 6263 5f62 2025 7d63 6f6c 2d31 3220  m_bc_b %}col-12 
-0000e1a0: 636f 6c2d 6d64 2d34 7b25 2065 6e64 626c  col-md-4{% endbl
-0000e1b0: 6f63 6b20 257d 223e 7b7b 2032 5f6d 6964  ock %}">{{ 2_mid
-0000e1c0: 5f62 6f74 746f 6d5f 6220 7d7d 3c2f 6469  _bottom_b }}</di
-0000e1d0: 763e 0a20 2020 2020 2020 2020 2020 2020  v>.             
-0000e1e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e1f0: 2020 203c 6469 7620 636c 6173 733d 227b     <div class="{
-0000e200: 2520 626c 6f63 6b20 325f 6d69 645f 626f  % block 2_mid_bo
-0000e210: 7474 6f6d 5f62 635f 6320 257d 636f 6c2d  ttom_bc_c %}col-
-0000e220: 3132 2063 6f6c 2d6d 642d 387b 2520 656e  12 col-md-8{% en
-0000e230: 6462 6c6f 636b 2025 7d22 3e7b 7b20 325f  dblock %}">{{ 2_
-0000e240: 6d69 645f 626f 7474 6f6d 5f63 207d 7d3c  mid_bottom_c }}<
-0000e250: 2f64 6976 3e0a 2020 2020 2020 2020 2020  /div>.          
-0000e260: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e270: 2020 7b25 2065 6c73 6520 257d 0a20 2020    {% else %}.   
-0000e280: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e290: 2020 2020 2020 2020 2020 2020 203c 6469               <di
-0000e2a0: 7620 636c 6173 733d 2263 6f6c 2d31 3222  v class="col-12"
-0000e2b0: 3e7b 7b20 325f 6d69 645f 626f 7474 6f6d  >{{ 2_mid_bottom
-0000e2c0: 5f61 207d 7d7b 7b20 325f 6d69 645f 626f  _a }}{{ 2_mid_bo
-0000e2d0: 7474 6f6d 5f62 207d 7d7b 7b20 325f 6d69  ttom_b }}{{ 2_mi
-0000e2e0: 645f 626f 7474 6f6d 5f63 207d 7d3c 2f64  d_bottom_c }}</d
-0000e2f0: 6976 3e0a 2020 2020 2020 2020 2020 2020  iv>.            
-0000e300: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e310: 7b25 2065 6e64 6966 2025 7d0a 2020 2020  {% endif %}.    
-0000e320: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e330: 2020 2020 3c2f 6469 763e 0a20 2020 2020      </div>.     
-0000e340: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-0000e350: 2f64 6976 3e0a 2020 2020 2020 2020 2020  /div>.          
-0000e360: 2020 2020 2020 2020 2020 7b25 2065 6e64            {% end
-0000e370: 6966 2025 7d0a 0a20 2020 2020 2020 2020  if %}..         
-0000e380: 2020 2020 2020 2020 2020 203c 212d 2d20             <!-- 
-0000e390: 426c 6f63 6b73 2069 6e20 626f 7474 6f6d  Blocks in bottom
-0000e3a0: 2070 6f73 6974 696f 6e20 2d2d 3e0a 2020   position -->.  
-0000e3b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e3c0: 2020 7b25 2069 6620 325f 626f 7474 6f6d    {% if 2_bottom
-0000e3d0: 5f61 206f 7220 325f 626f 7474 6f6d 5f62  _a or 2_bottom_b
-0000e3e0: 206f 7220 325f 626f 7474 6f6d 5f63 2025   or 2_bottom_c %
-0000e3f0: 7d0a 2020 2020 2020 2020 2020 2020 2020  }.              
-0000e400: 2020 2020 2020 3c64 6976 2063 6c61 7373        <div class
-0000e410: 3d22 636f 6c2d 3132 223e 0a20 2020 2020  ="col-12">.     
-0000e420: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e430: 2020 203c 6469 7620 636c 6173 733d 2272     <div class="r
-0000e440: 6f77 223e 0a20 2020 2020 2020 2020 2020  ow">.           
-0000e450: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e460: 207b 2520 6966 2032 5f62 6f74 746f 6d5f   {% if 2_bottom_
-0000e470: 6120 616e 6420 325f 626f 7474 6f6d 5f62  a and 2_bottom_b
-0000e480: 2061 6e64 2032 5f62 6f74 746f 6d5f 6320   and 2_bottom_c 
-0000e490: 257d 0a20 2020 2020 2020 2020 2020 2020  %}.             
-0000e4a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e4b0: 2020 203c 6469 7620 636c 6173 733d 227b     <div class="{
-0000e4c0: 2520 626c 6f63 6b20 325f 626f 7474 6f6d  % block 2_bottom
-0000e4d0: 5f61 6263 5f61 2025 7d63 6f6c 2d31 3220  _abc_a %}col-12 
-0000e4e0: 636f 6c2d 6d64 2d34 7b25 2065 6e64 626c  col-md-4{% endbl
-0000e4f0: 6f63 6b20 257d 223e 7b7b 2032 5f62 6f74  ock %}">{{ 2_bot
-0000e500: 746f 6d5f 6120 7d7d 3c2f 6469 763e 0a20  tom_a }}</div>. 
+0000e0a0: 207b 2520 6966 2032 5f6d 6964 5f62 6f74   {% if 2_mid_bot
+0000e0b0: 746f 6d5f 6120 616e 6420 325f 6d69 645f  tom_a and 2_mid_
+0000e0c0: 626f 7474 6f6d 5f62 2061 6e64 2032 5f6d  bottom_b and 2_m
+0000e0d0: 6964 5f62 6f74 746f 6d5f 6320 257d 0a20  id_bottom_c %}. 
+0000e0e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e0f0: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+0000e100: 6469 7620 636c 6173 733d 227b 2520 626c  div class="{% bl
+0000e110: 6f63 6b20 325f 6d69 645f 626f 7474 6f6d  ock 2_mid_bottom
+0000e120: 5f61 6263 5f61 2025 7d63 6f6c 2d31 3220  _abc_a %}col-12 
+0000e130: 636f 6c2d 6d64 2d34 7b25 2065 6e64 626c  col-md-4{% endbl
+0000e140: 6f63 6b20 257d 223e 7b7b 2032 5f6d 6964  ock %}">{{ 2_mid
+0000e150: 5f62 6f74 746f 6d5f 6120 7d7d 3c2f 6469  _bottom_a }}</di
+0000e160: 763e 0a20 2020 2020 2020 2020 2020 2020  v>.             
+0000e170: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e180: 2020 203c 6469 7620 636c 6173 733d 227b     <div class="{
+0000e190: 2520 626c 6f63 6b20 325f 6d69 645f 626f  % block 2_mid_bo
+0000e1a0: 7474 6f6d 5f61 6263 5f62 2025 7d63 6f6c  ttom_abc_b %}col
+0000e1b0: 2d31 3220 636f 6c2d 6d64 2d34 7b25 2065  -12 col-md-4{% e
+0000e1c0: 6e64 626c 6f63 6b20 257d 223e 7b7b 2032  ndblock %}">{{ 2
+0000e1d0: 5f6d 6964 5f62 6f74 746f 6d5f 6220 7d7d  _mid_bottom_b }}
+0000e1e0: 3c2f 6469 763e 0a20 2020 2020 2020 2020  </div>.         
+0000e1f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e200: 2020 2020 2020 203c 6469 7620 636c 6173         <div clas
+0000e210: 733d 227b 2520 626c 6f63 6b20 325f 6d69  s="{% block 2_mi
+0000e220: 645f 626f 7474 6f6d 5f61 6263 5f63 2025  d_bottom_abc_c %
+0000e230: 7d63 6f6c 2d31 3220 636f 6c2d 6d64 2d34  }col-12 col-md-4
+0000e240: 7b25 2065 6e64 626c 6f63 6b20 257d 223e  {% endblock %}">
+0000e250: 7b7b 2032 5f6d 6964 5f62 6f74 746f 6d5f  {{ 2_mid_bottom_
+0000e260: 6320 7d7d 3c2f 6469 763e 0a20 2020 2020  c }}</div>.     
+0000e270: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e280: 2020 2020 2020 207b 2520 656c 6966 2032         {% elif 2
+0000e290: 5f6d 6964 5f62 6f74 746f 6d5f 6120 616e  _mid_bottom_a an
+0000e2a0: 6420 325f 6d69 645f 626f 7474 6f6d 5f62  d 2_mid_bottom_b
+0000e2b0: 2025 7d0a 2020 2020 2020 2020 2020 2020   %}.            
+0000e2c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e2d0: 2020 2020 3c64 6976 2063 6c61 7373 3d22      <div class="
+0000e2e0: 7b25 2062 6c6f 636b 2032 5f6d 6964 5f62  {% block 2_mid_b
+0000e2f0: 6f74 746f 6d5f 6162 5f61 2025 7d63 6f6c  ottom_ab_a %}col
+0000e300: 2d31 3220 636f 6c2d 6d64 2d38 7b25 2065  -12 col-md-8{% e
+0000e310: 6e64 626c 6f63 6b20 257d 223e 7b7b 2032  ndblock %}">{{ 2
+0000e320: 5f6d 6964 5f62 6f74 746f 6d5f 6120 7d7d  _mid_bottom_a }}
+0000e330: 3c2f 6469 763e 0a20 2020 2020 2020 2020  </div>.         
+0000e340: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e350: 2020 2020 2020 203c 6469 7620 636c 6173         <div clas
+0000e360: 733d 227b 2520 626c 6f63 6b20 325f 6d69  s="{% block 2_mi
+0000e370: 645f 626f 7474 6f6d 5f61 625f 6220 257d  d_bottom_ab_b %}
+0000e380: 636f 6c2d 3132 2063 6f6c 2d6d 642d 347b  col-12 col-md-4{
+0000e390: 2520 656e 6462 6c6f 636b 2025 7d22 3e7b  % endblock %}">{
+0000e3a0: 7b20 325f 6d69 645f 626f 7474 6f6d 5f62  { 2_mid_bottom_b
+0000e3b0: 207d 7d3c 2f64 6976 3e0a 2020 2020 2020   }}</div>.      
+0000e3c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e3d0: 2020 2020 2020 7b25 2065 6c69 6620 325f        {% elif 2_
+0000e3e0: 6d69 645f 626f 7474 6f6d 5f61 2061 6e64  mid_bottom_a and
+0000e3f0: 2032 5f6d 6964 5f62 6f74 746f 6d5f 6320   2_mid_bottom_c 
+0000e400: 257d 0a20 2020 2020 2020 2020 2020 2020  %}.             
+0000e410: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e420: 2020 203c 6469 7620 636c 6173 733d 227b     <div class="{
+0000e430: 2520 626c 6f63 6b20 325f 6d69 645f 626f  % block 2_mid_bo
+0000e440: 7474 6f6d 5f61 635f 6120 257d 636f 6c2d  ttom_ac_a %}col-
+0000e450: 3132 2063 6f6c 2d6d 642d 367b 2520 656e  12 col-md-6{% en
+0000e460: 6462 6c6f 636b 2025 7d22 3e7b 7b20 325f  dblock %}">{{ 2_
+0000e470: 6d69 645f 626f 7474 6f6d 5f61 207d 7d3c  mid_bottom_a }}<
+0000e480: 2f64 6976 3e0a 2020 2020 2020 2020 2020  /div>.          
+0000e490: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e4a0: 2020 2020 2020 3c64 6976 2063 6c61 7373        <div class
+0000e4b0: 3d22 7b25 2062 6c6f 636b 2032 5f6d 6964  ="{% block 2_mid
+0000e4c0: 5f62 6f74 746f 6d5f 6163 5f63 2025 7d63  _bottom_ac_c %}c
+0000e4d0: 6f6c 2d31 3220 636f 6c2d 6d64 2d36 7b25  ol-12 col-md-6{%
+0000e4e0: 2065 6e64 626c 6f63 6b20 257d 223e 7b7b   endblock %}">{{
+0000e4f0: 2032 5f6d 6964 5f62 6f74 746f 6d5f 6320   2_mid_bottom_c 
+0000e500: 7d7d 3c2f 6469 763e 0a20 2020 2020 2020  }}</div>.       
 0000e510: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e520: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-0000e530: 6469 7620 636c 6173 733d 227b 2520 626c  div class="{% bl
-0000e540: 6f63 6b20 325f 626f 7474 6f6d 5f61 6263  ock 2_bottom_abc
-0000e550: 5f62 2025 7d63 6f6c 2d31 3220 636f 6c2d  _b %}col-12 col-
-0000e560: 6d64 2d34 7b25 2065 6e64 626c 6f63 6b20  md-4{% endblock 
-0000e570: 257d 223e 7b7b 2032 5f62 6f74 746f 6d5f  %}">{{ 2_bottom_
-0000e580: 6220 7d7d 3c2f 6469 763e 0a20 2020 2020  b }}</div>.     
-0000e590: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e5a0: 2020 2020 2020 2020 2020 203c 6469 7620             <div 
-0000e5b0: 636c 6173 733d 227b 2520 626c 6f63 6b20  class="{% block 
-0000e5c0: 325f 626f 7474 6f6d 5f61 6263 5f63 2025  2_bottom_abc_c %
-0000e5d0: 7d63 6f6c 2d31 3220 636f 6c2d 6d64 2d34  }col-12 col-md-4
-0000e5e0: 7b25 2065 6e64 626c 6f63 6b20 257d 223e  {% endblock %}">
-0000e5f0: 7b7b 2032 5f62 6f74 746f 6d5f 6320 7d7d  {{ 2_bottom_c }}
-0000e600: 3c2f 6469 763e 0a20 2020 2020 2020 2020  </div>.         
-0000e610: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e620: 2020 207b 2520 656c 6966 2032 5f62 6f74     {% elif 2_bot
-0000e630: 746f 6d5f 6120 616e 6420 325f 626f 7474  tom_a and 2_bott
-0000e640: 6f6d 5f62 2025 7d0a 2020 2020 2020 2020  om_b %}.        
-0000e650: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e660: 2020 2020 2020 2020 3c64 6976 2063 6c61          <div cla
-0000e670: 7373 3d22 7b25 2062 6c6f 636b 2032 5f62  ss="{% block 2_b
-0000e680: 6f74 746f 6d5f 6162 5f61 2025 7d63 6f6c  ottom_ab_a %}col
-0000e690: 2d31 3220 636f 6c2d 6d64 2d38 7b25 2065  -12 col-md-8{% e
-0000e6a0: 6e64 626c 6f63 6b20 257d 223e 7b7b 2032  ndblock %}">{{ 2
-0000e6b0: 5f62 6f74 746f 6d5f 6120 7d7d 3c2f 6469  _bottom_a }}</di
-0000e6c0: 763e 0a20 2020 2020 2020 2020 2020 2020  v>.             
-0000e6d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e6e0: 2020 203c 6469 7620 636c 6173 733d 227b     <div class="{
-0000e6f0: 2520 626c 6f63 6b20 325f 626f 7474 6f6d  % block 2_bottom
-0000e700: 5f61 625f 6220 257d 636f 6c2d 3132 2063  _ab_b %}col-12 c
-0000e710: 6f6c 2d6d 642d 347b 2520 656e 6462 6c6f  ol-md-4{% endblo
-0000e720: 636b 2025 7d22 3e7b 7b20 325f 626f 7474  ck %}">{{ 2_bott
-0000e730: 6f6d 5f62 207d 7d3c 2f64 6976 3e0a 2020  om_b }}</div>.  
+0000e520: 2020 2020 207b 2520 656c 6966 2032 5f6d       {% elif 2_m
+0000e530: 6964 5f62 6f74 746f 6d5f 6220 616e 6420  id_bottom_b and 
+0000e540: 325f 6d69 645f 626f 7474 6f6d 5f63 2025  2_mid_bottom_c %
+0000e550: 7d0a 2020 2020 2020 2020 2020 2020 2020  }.              
+0000e560: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e570: 2020 3c64 6976 2063 6c61 7373 3d22 7b25    <div class="{%
+0000e580: 2062 6c6f 636b 2032 5f6d 6964 5f62 6f74   block 2_mid_bot
+0000e590: 746f 6d5f 6263 5f62 2025 7d63 6f6c 2d31  tom_bc_b %}col-1
+0000e5a0: 3220 636f 6c2d 6d64 2d34 7b25 2065 6e64  2 col-md-4{% end
+0000e5b0: 626c 6f63 6b20 257d 223e 7b7b 2032 5f6d  block %}">{{ 2_m
+0000e5c0: 6964 5f62 6f74 746f 6d5f 6220 7d7d 3c2f  id_bottom_b }}</
+0000e5d0: 6469 763e 0a20 2020 2020 2020 2020 2020  div>.           
+0000e5e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e5f0: 2020 2020 203c 6469 7620 636c 6173 733d       <div class=
+0000e600: 227b 2520 626c 6f63 6b20 325f 6d69 645f  "{% block 2_mid_
+0000e610: 626f 7474 6f6d 5f62 635f 6320 257d 636f  bottom_bc_c %}co
+0000e620: 6c2d 3132 2063 6f6c 2d6d 642d 387b 2520  l-12 col-md-8{% 
+0000e630: 656e 6462 6c6f 636b 2025 7d22 3e7b 7b20  endblock %}">{{ 
+0000e640: 325f 6d69 645f 626f 7474 6f6d 5f63 207d  2_mid_bottom_c }
+0000e650: 7d3c 2f64 6976 3e0a 2020 2020 2020 2020  }</div>.        
+0000e660: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e670: 2020 2020 7b25 2065 6c73 6520 257d 0a20      {% else %}. 
+0000e680: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e690: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+0000e6a0: 6469 7620 636c 6173 733d 2263 6f6c 2d31  div class="col-1
+0000e6b0: 3222 3e7b 7b20 325f 6d69 645f 626f 7474  2">{{ 2_mid_bott
+0000e6c0: 6f6d 5f61 207d 7d7b 7b20 325f 6d69 645f  om_a }}{{ 2_mid_
+0000e6d0: 626f 7474 6f6d 5f62 207d 7d7b 7b20 325f  bottom_b }}{{ 2_
+0000e6e0: 6d69 645f 626f 7474 6f6d 5f63 207d 7d3c  mid_bottom_c }}<
+0000e6f0: 2f64 6976 3e0a 2020 2020 2020 2020 2020  /div>.          
+0000e700: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e710: 2020 7b25 2065 6e64 6966 2025 7d0a 2020    {% endif %}.  
+0000e720: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e730: 2020 2020 2020 3c2f 6469 763e 0a20 2020        </div>.   
 0000e740: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e750: 2020 2020 2020 2020 2020 7b25 2065 6c69            {% eli
-0000e760: 6620 325f 626f 7474 6f6d 5f61 2061 6e64  f 2_bottom_a and
-0000e770: 2032 5f62 6f74 746f 6d5f 6320 257d 0a20   2_bottom_c %}. 
-0000e780: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e790: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-0000e7a0: 6469 7620 636c 6173 733d 227b 2520 626c  div class="{% bl
-0000e7b0: 6f63 6b20 325f 626f 7474 6f6d 5f61 635f  ock 2_bottom_ac_
-0000e7c0: 6120 257d 636f 6c2d 3132 2063 6f6c 2d6d  a %}col-12 col-m
-0000e7d0: 642d 367b 2520 656e 6462 6c6f 636b 2025  d-6{% endblock %
-0000e7e0: 7d22 3e7b 7b20 325f 626f 7474 6f6d 5f61  }">{{ 2_bottom_a
-0000e7f0: 207d 7d3c 2f64 6976 3e0a 2020 2020 2020   }}</div>.      
-0000e800: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e810: 2020 2020 2020 2020 2020 3c64 6976 2063            <div c
-0000e820: 6c61 7373 3d22 7b25 2062 6c6f 636b 2032  lass="{% block 2
-0000e830: 5f62 6f74 746f 6d5f 6163 5f63 2025 7d63  _bottom_ac_c %}c
-0000e840: 6f6c 2d31 3220 636f 6c2d 6d64 2d36 7b25  ol-12 col-md-6{%
-0000e850: 2065 6e64 626c 6f63 6b20 257d 223e 7b7b   endblock %}">{{
-0000e860: 2032 5f62 6f74 746f 6d5f 6320 7d7d 3c2f   2_bottom_c }}</
-0000e870: 6469 763e 0a20 2020 2020 2020 2020 2020  div>.           
-0000e880: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e890: 207b 2520 656c 6966 2032 5f62 6f74 746f   {% elif 2_botto
-0000e8a0: 6d5f 6220 616e 6420 325f 626f 7474 6f6d  m_b and 2_bottom
-0000e8b0: 5f63 2025 7d0a 2020 2020 2020 2020 2020  _c %}.          
-0000e8c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e8d0: 2020 2020 2020 3c64 6976 2063 6c61 7373        <div class
-0000e8e0: 3d22 7b25 2062 6c6f 636b 2032 5f62 6f74  ="{% block 2_bot
-0000e8f0: 746f 6d5f 6263 5f62 2025 7d63 6f6c 2d31  tom_bc_b %}col-1
-0000e900: 3220 636f 6c2d 6d64 2d34 7b25 2065 6e64  2 col-md-4{% end
-0000e910: 626c 6f63 6b20 257d 223e 7b7b 2032 5f62  block %}">{{ 2_b
-0000e920: 6f74 746f 6d5f 6220 7d7d 3c2f 6469 763e  ottom_b }}</div>
-0000e930: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000e940: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e950: 203c 6469 7620 636c 6173 733d 227b 2520   <div class="{% 
-0000e960: 626c 6f63 6b20 325f 626f 7474 6f6d 5f62  block 2_bottom_b
-0000e970: 635f 6320 257d 636f 6c2d 3132 2063 6f6c  c_c %}col-12 col
-0000e980: 2d6d 642d 387b 2520 656e 6462 6c6f 636b  -md-8{% endblock
-0000e990: 2025 7d22 3e7b 7b20 325f 626f 7474 6f6d   %}">{{ 2_bottom
-0000e9a0: 5f63 207d 7d3c 2f64 6976 3e0a 2020 2020  _c }}</div>.    
-0000e9b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e9c0: 2020 2020 2020 2020 7b25 2065 6c73 6520          {% else 
-0000e9d0: 257d 0a20 2020 2020 2020 2020 2020 2020  %}.             
-0000e9e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e9f0: 2020 203c 6469 7620 636c 6173 733d 2263     <div class="c
-0000ea00: 6f6c 2d31 3222 3e7b 7b20 325f 626f 7474  ol-12">{{ 2_bott
-0000ea10: 6f6d 5f61 207d 7d7b 7b20 325f 626f 7474  om_a }}{{ 2_bott
-0000ea20: 6f6d 5f62 207d 7d7b 7b20 325f 626f 7474  om_b }}{{ 2_bott
-0000ea30: 6f6d 5f63 207d 7d3c 2f64 6976 3e0a 2020  om_c }}</div>.  
-0000ea40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ea50: 2020 2020 2020 2020 2020 7b25 2065 6e64            {% end
-0000ea60: 6966 2025 7d0a 2020 2020 2020 2020 2020  if %}.          
-0000ea70: 2020 2020 2020 2020 2020 2020 2020 3c2f                </
-0000ea80: 6469 763e 0a20 2020 2020 2020 2020 2020  div>.           
-0000ea90: 2020 2020 2020 2020 203c 2f64 6976 3e0a           </div>.
-0000eaa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000eab0: 2020 2020 7b25 2065 6e64 6966 2025 7d0a      {% endif %}.
-0000eac0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000ead0: 203c 2f64 6976 3e0a 2020 2020 2020 2020   </div>.        
-0000eae0: 2020 2020 3c2f 6469 763e 0a20 2020 2020      </div>.     
-0000eaf0: 2020 203c 2f64 6976 3e0a 2020 2020 7b25     </div>.    {%
-0000eb00: 2065 6e64 6966 2025 7d0a 2020 2020 7b25   endif %}.    {%
-0000eb10: 2065 6e64 626c 6f63 6b20 7365 6374 696f   endblock sectio
-0000eb20: 6e5f 3220 257d 0a20 2020 203c 212d 2d20  n_2 %}.    <!-- 
-0000eb30: 656e 6420 5365 6374 696f 6e20 3220 2d2d  end Section 2 --
-0000eb40: 3e0a 0a20 2020 203c 212d 2d2d 2d2d 2d2d  >..    <!-------
-0000eb50: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0000eb60: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0000eb70: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0000eb80: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 3e0a  -------------->.
-0000eb90: 0a20 2020 203c 212d 2d20 5365 6374 696f  .    <!-- Sectio
-0000eba0: 6e20 3320 2d2d 3e0a 2020 2020 7b25 2062  n 3 -->.    {% b
-0000ebb0: 6c6f 636b 2073 6563 7469 6f6e 5f33 2025  lock section_3 %
-0000ebc0: 7d0a 2020 2020 7b25 2062 6c6f 636b 735f  }.    {% blocks_
-0000ebd0: 696e 5f70 6f73 6974 696f 6e20 7365 6374  in_position sect
-0000ebe0: 696f 6e3d 2273 6563 7469 6f6e 2d33 2220  ion="section-3" 
-0000ebf0: 6173 2073 6563 7469 6f6e 5f33 2025 7d0a  as section_3 %}.
-0000ec00: 2020 2020 7b25 2069 6620 7365 6374 696f      {% if sectio
-0000ec10: 6e5f 3320 257d 0a20 2020 2020 2020 207b  n_3 %}.        {
-0000ec20: 2520 6c6f 6164 5f62 6c6f 636b 7320 7365  % load_blocks se
-0000ec30: 6374 696f 6e3d 2233 2d74 6f70 2d61 2220  ction="3-top-a" 
-0000ec40: 6173 2033 5f74 6f70 5f61 2025 7d0a 2020  as 3_top_a %}.  
-0000ec50: 2020 2020 2020 7b25 206c 6f61 645f 626c        {% load_bl
-0000ec60: 6f63 6b73 2073 6563 7469 6f6e 3d22 332d  ocks section="3-
-0000ec70: 746f 702d 6222 2061 7320 335f 746f 705f  top-b" as 3_top_
-0000ec80: 6220 257d 0a20 2020 2020 2020 207b 2520  b %}.        {% 
-0000ec90: 6c6f 6164 5f62 6c6f 636b 7320 7365 6374  load_blocks sect
-0000eca0: 696f 6e3d 2233 2d74 6f70 2d63 2220 6173  ion="3-top-c" as
-0000ecb0: 2033 5f74 6f70 5f63 2025 7d0a 0a20 2020   3_top_c %}..   
-0000ecc0: 2020 2020 207b 2520 6c6f 6164 5f62 6c6f       {% load_blo
-0000ecd0: 636b 7320 7365 6374 696f 6e3d 2233 2d6d  cks section="3-m
-0000ece0: 6964 2d74 6f70 2d61 2220 6173 2033 5f6d  id-top-a" as 3_m
-0000ecf0: 6964 5f74 6f70 5f61 2025 7d0a 2020 2020  id_top_a %}.    
-0000ed00: 2020 2020 7b25 206c 6f61 645f 626c 6f63      {% load_bloc
-0000ed10: 6b73 2073 6563 7469 6f6e 3d22 332d 6d69  ks section="3-mi
-0000ed20: 642d 746f 702d 6222 2061 7320 335f 6d69  d-top-b" as 3_mi
-0000ed30: 645f 746f 705f 6220 257d 0a20 2020 2020  d_top_b %}.     
-0000ed40: 2020 207b 2520 6c6f 6164 5f62 6c6f 636b     {% load_block
-0000ed50: 7320 7365 6374 696f 6e3d 2233 2d6d 6964  s section="3-mid
-0000ed60: 2d74 6f70 2d63 2220 6173 2033 5f6d 6964  -top-c" as 3_mid
-0000ed70: 5f74 6f70 5f63 2025 7d0a 0a20 2020 2020  _top_c %}..     
-0000ed80: 2020 207b 2520 6c6f 6164 5f62 6c6f 636b     {% load_block
-0000ed90: 7320 7365 6374 696f 6e3d 2233 2d6c 6566  s section="3-lef
-0000eda0: 742d 6122 2061 7320 335f 6c65 6674 5f61  t-a" as 3_left_a
-0000edb0: 2025 7d0a 2020 2020 2020 2020 7b25 206c   %}.        {% l
-0000edc0: 6f61 645f 626c 6f63 6b73 2073 6563 7469  oad_blocks secti
-0000edd0: 6f6e 3d22 332d 6c65 6674 2d62 2220 6173  on="3-left-b" as
-0000ede0: 2033 5f6c 6566 745f 6220 257d 0a0a 2020   3_left_b %}..  
-0000edf0: 2020 2020 2020 7b25 206c 6f61 645f 626c        {% load_bl
-0000ee00: 6f63 6b73 2073 6563 7469 6f6e 3d22 332d  ocks section="3-
-0000ee10: 6365 6e74 6572 2d74 6f70 2d61 2220 6173  center-top-a" as
-0000ee20: 2033 5f63 656e 7465 725f 746f 705f 6120   3_center_top_a 
-0000ee30: 257d 0a20 2020 2020 2020 207b 2520 6c6f  %}.        {% lo
-0000ee40: 6164 5f62 6c6f 636b 7320 7365 6374 696f  ad_blocks sectio
-0000ee50: 6e3d 2233 2d63 656e 7465 722d 746f 702d  n="3-center-top-
-0000ee60: 6222 2061 7320 335f 6365 6e74 6572 5f74  b" as 3_center_t
-0000ee70: 6f70 5f62 2025 7d0a 2020 2020 2020 2020  op_b %}.        
-0000ee80: 7b25 206c 6f61 645f 626c 6f63 6b73 2073  {% load_blocks s
-0000ee90: 6563 7469 6f6e 3d22 332d 6365 6e74 6572  ection="3-center
-0000eea0: 2d74 6f70 2d63 2220 6173 2033 5f63 656e  -top-c" as 3_cen
-0000eeb0: 7465 725f 746f 705f 6320 257d 0a0a 2020  ter_top_c %}..  
-0000eec0: 2020 2020 2020 7b25 206c 6f61 645f 626c        {% load_bl
-0000eed0: 6f63 6b73 2073 6563 7469 6f6e 3d22 332d  ocks section="3-
-0000eee0: 6365 6e74 6572 2d6d 6964 2d74 6f70 2d61  center-mid-top-a
-0000eef0: 2220 6173 2033 5f63 656e 7465 725f 6d69  " as 3_center_mi
-0000ef00: 645f 746f 705f 6120 257d 0a20 2020 2020  d_top_a %}.     
-0000ef10: 2020 207b 2520 6c6f 6164 5f62 6c6f 636b     {% load_block
-0000ef20: 7320 7365 6374 696f 6e3d 2233 2d63 656e  s section="3-cen
-0000ef30: 7465 722d 6d69 642d 746f 702d 6222 2061  ter-mid-top-b" a
-0000ef40: 7320 335f 6365 6e74 6572 5f6d 6964 5f74  s 3_center_mid_t
-0000ef50: 6f70 5f62 2025 7d0a 2020 2020 2020 2020  op_b %}.        
-0000ef60: 7b25 206c 6f61 645f 626c 6f63 6b73 2073  {% load_blocks s
-0000ef70: 6563 7469 6f6e 3d22 332d 6365 6e74 6572  ection="3-center
-0000ef80: 2d6d 6964 2d74 6f70 2d63 2220 6173 2033  -mid-top-c" as 3
-0000ef90: 5f63 656e 7465 725f 6d69 645f 746f 705f  _center_mid_top_
-0000efa0: 6320 257d 0a0a 2020 2020 2020 2020 7b25  c %}..        {%
-0000efb0: 206c 6f61 645f 626c 6f63 6b73 2073 6563   load_blocks sec
-0000efc0: 7469 6f6e 3d22 332d 6365 6e74 6572 2d63  tion="3-center-c
-0000efd0: 6f6e 7465 6e74 2220 6173 2033 5f63 656e  ontent" as 3_cen
-0000efe0: 7465 725f 636f 6e74 656e 7420 257d 0a0a  ter_content %}..
-0000eff0: 2020 2020 2020 2020 7b25 206c 6f61 645f          {% load_
-0000f000: 626c 6f63 6b73 2073 6563 7469 6f6e 3d22  blocks section="
-0000f010: 332d 6365 6e74 6572 2d6d 6964 2d62 6f74  3-center-mid-bot
-0000f020: 746f 6d2d 6122 2061 7320 335f 6365 6e74  tom-a" as 3_cent
-0000f030: 6572 5f6d 6964 5f62 6f74 746f 6d5f 6120  er_mid_bottom_a 
-0000f040: 257d 0a20 2020 2020 2020 207b 2520 6c6f  %}.        {% lo
-0000f050: 6164 5f62 6c6f 636b 7320 7365 6374 696f  ad_blocks sectio
-0000f060: 6e3d 2233 2d63 656e 7465 722d 6d69 642d  n="3-center-mid-
-0000f070: 626f 7474 6f6d 2d62 2220 6173 2033 5f63  bottom-b" as 3_c
-0000f080: 656e 7465 725f 6d69 645f 626f 7474 6f6d  enter_mid_bottom
-0000f090: 5f62 2025 7d0a 2020 2020 2020 2020 7b25  _b %}.        {%
-0000f0a0: 206c 6f61 645f 626c 6f63 6b73 2073 6563   load_blocks sec
-0000f0b0: 7469 6f6e 3d22 332d 6365 6e74 6572 2d6d  tion="3-center-m
-0000f0c0: 6964 2d62 6f74 746f 6d2d 6322 2061 7320  id-bottom-c" as 
-0000f0d0: 335f 6365 6e74 6572 5f6d 6964 5f62 6f74  3_center_mid_bot
-0000f0e0: 746f 6d5f 6320 257d 0a0a 2020 2020 2020  tom_c %}..      
-0000f0f0: 2020 7b25 206c 6f61 645f 626c 6f63 6b73    {% load_blocks
-0000f100: 2073 6563 7469 6f6e 3d22 332d 6365 6e74   section="3-cent
-0000f110: 6572 2d62 6f74 746f 6d2d 6122 2061 7320  er-bottom-a" as 
-0000f120: 335f 6365 6e74 6572 5f62 6f74 746f 6d5f  3_center_bottom_
-0000f130: 6120 257d 0a20 2020 2020 2020 207b 2520  a %}.        {% 
-0000f140: 6c6f 6164 5f62 6c6f 636b 7320 7365 6374  load_blocks sect
-0000f150: 696f 6e3d 2233 2d63 656e 7465 722d 626f  ion="3-center-bo
-0000f160: 7474 6f6d 2d62 2220 6173 2033 5f63 656e  ttom-b" as 3_cen
-0000f170: 7465 725f 626f 7474 6f6d 5f62 2025 7d0a  ter_bottom_b %}.
-0000f180: 2020 2020 2020 2020 7b25 206c 6f61 645f          {% load_
-0000f190: 626c 6f63 6b73 2073 6563 7469 6f6e 3d22  blocks section="
-0000f1a0: 332d 6365 6e74 6572 2d62 6f74 746f 6d2d  3-center-bottom-
-0000f1b0: 6322 2061 7320 335f 6365 6e74 6572 5f62  c" as 3_center_b
-0000f1c0: 6f74 746f 6d5f 6320 257d 0a0a 2020 2020  ottom_c %}..    
-0000f1d0: 2020 2020 7b25 206c 6f61 645f 626c 6f63      {% load_bloc
-0000f1e0: 6b73 2073 6563 7469 6f6e 3d22 332d 7269  ks section="3-ri
-0000f1f0: 6768 742d 6122 2061 7320 335f 7269 6768  ght-a" as 3_righ
-0000f200: 745f 6120 257d 0a20 2020 2020 2020 207b  t_a %}.        {
-0000f210: 2520 6c6f 6164 5f62 6c6f 636b 7320 7365  % load_blocks se
-0000f220: 6374 696f 6e3d 2233 2d72 6967 6874 2d62  ction="3-right-b
-0000f230: 2220 6173 2033 5f72 6967 6874 5f62 2025  " as 3_right_b %
-0000f240: 7d0a 0a20 2020 2020 2020 207b 2520 6c6f  }..        {% lo
-0000f250: 6164 5f62 6c6f 636b 7320 7365 6374 696f  ad_blocks sectio
-0000f260: 6e3d 2233 2d6d 6964 2d62 6f74 746f 6d2d  n="3-mid-bottom-
-0000f270: 6122 2061 7320 335f 6d69 645f 626f 7474  a" as 3_mid_bott
-0000f280: 6f6d 5f61 2025 7d0a 2020 2020 2020 2020  om_a %}.        
-0000f290: 7b25 206c 6f61 645f 626c 6f63 6b73 2073  {% load_blocks s
-0000f2a0: 6563 7469 6f6e 3d22 332d 6d69 642d 626f  ection="3-mid-bo
-0000f2b0: 7474 6f6d 2d62 2220 6173 2033 5f6d 6964  ttom-b" as 3_mid
-0000f2c0: 5f62 6f74 746f 6d5f 6220 257d 0a20 2020  _bottom_b %}.   
-0000f2d0: 2020 2020 207b 2520 6c6f 6164 5f62 6c6f       {% load_blo
-0000f2e0: 636b 7320 7365 6374 696f 6e3d 2233 2d6d  cks section="3-m
-0000f2f0: 6964 2d62 6f74 746f 6d2d 6322 2061 7320  id-bottom-c" as 
-0000f300: 335f 6d69 645f 626f 7474 6f6d 5f63 2025  3_mid_bottom_c %
-0000f310: 7d0a 0a20 2020 2020 2020 207b 2520 6c6f  }..        {% lo
-0000f320: 6164 5f62 6c6f 636b 7320 7365 6374 696f  ad_blocks sectio
-0000f330: 6e3d 2233 2d62 6f74 746f 6d2d 6122 2061  n="3-bottom-a" a
-0000f340: 7320 335f 626f 7474 6f6d 5f61 2025 7d0a  s 3_bottom_a %}.
-0000f350: 2020 2020 2020 2020 7b25 206c 6f61 645f          {% load_
-0000f360: 626c 6f63 6b73 2073 6563 7469 6f6e 3d22  blocks section="
-0000f370: 332d 626f 7474 6f6d 2d62 2220 6173 2033  3-bottom-b" as 3
-0000f380: 5f62 6f74 746f 6d5f 6220 257d 0a20 2020  _bottom_b %}.   
-0000f390: 2020 2020 207b 2520 6c6f 6164 5f62 6c6f       {% load_blo
-0000f3a0: 636b 7320 7365 6374 696f 6e3d 2233 2d62  cks section="3-b
-0000f3b0: 6f74 746f 6d2d 6322 2061 7320 335f 626f  ottom-c" as 3_bo
-0000f3c0: 7474 6f6d 5f63 2025 7d0a 0a20 2020 2020  ttom_c %}..     
-0000f3d0: 2020 203c 6469 7620 636c 6173 733d 227b     <div class="{
-0000f3e0: 2520 626c 6f63 6b20 7365 6374 696f 6e5f  % block section_
-0000f3f0: 335f 636c 6173 7365 7320 257d 7079 2d35  3_classes %}py-5
-0000f400: 7b25 2065 6e64 626c 6f63 6b20 257d 223e  {% endblock %}">
-0000f410: 0a20 2020 2020 2020 2020 2020 203c 6469  .            <di
-0000f420: 7620 636c 6173 733d 2263 6f6e 7461 696e  v class="contain
-0000f430: 6572 223e 0a20 2020 2020 2020 2020 2020  er">.           
-0000f440: 2020 2020 203c 6469 7620 636c 6173 733d       <div class=
-0000f450: 2272 6f77 206d 782d 3022 3e0a 0a20 2020  "row mx-0">..   
-0000f460: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f470: 203c 212d 2d20 546f 7020 2d2d 3e0a 2020   <!-- Top -->.  
-0000f480: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f490: 2020 7b25 2069 6620 335f 746f 705f 6120    {% if 3_top_a 
-0000f4a0: 6f72 2033 5f74 6f70 5f62 206f 7220 335f  or 3_top_b or 3_
-0000f4b0: 746f 705f 6320 257d 0a20 2020 2020 2020  top_c %}.       
-0000f4c0: 2020 2020 2020 2020 2020 2020 203c 6469               <di
-0000f4d0: 7620 636c 6173 733d 2263 6f6c 2d31 3222  v class="col-12"
-0000f4e0: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
-0000f4f0: 2020 2020 2020 2020 2020 3c64 6976 2063            <div c
-0000f500: 6c61 7373 3d22 726f 7722 3e0a 2020 2020  lass="row">.    
-0000f510: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f520: 2020 2020 2020 2020 7b25 2069 6620 335f          {% if 3_
-0000f530: 746f 705f 6120 616e 6420 335f 746f 705f  top_a and 3_top_
-0000f540: 6220 616e 6420 335f 746f 705f 6320 257d  b and 3_top_c %}
-0000f550: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000f560: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f570: 203c 6469 7620 636c 6173 733d 227b 2520   <div class="{% 
-0000f580: 626c 6f63 6b20 335f 746f 705f 6162 635f  block 3_top_abc_
-0000f590: 6120 257d 636f 6c2d 3132 2063 6f6c 2d6d  a %}col-12 col-m
-0000f5a0: 642d 347b 2520 656e 6462 6c6f 636b 2025  d-4{% endblock %
-0000f5b0: 7d22 3e7b 7b20 335f 746f 705f 6120 7d7d  }">{{ 3_top_a }}
-0000f5c0: 3c2f 6469 763e 0a20 2020 2020 2020 2020  </div>.         
-0000f5d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f5e0: 2020 2020 2020 203c 6469 7620 636c 6173         <div clas
-0000f5f0: 733d 227b 2520 626c 6f63 6b20 335f 746f  s="{% block 3_to
-0000f600: 705f 6162 635f 6220 257d 636f 6c2d 3132  p_abc_b %}col-12
-0000f610: 2063 6f6c 2d6d 642d 347b 2520 656e 6462   col-md-4{% endb
-0000f620: 6c6f 636b 2025 7d22 3e7b 7b20 335f 746f  lock %}">{{ 3_to
-0000f630: 705f 6220 7d7d 3c2f 6469 763e 0a20 2020  p_b }}</div>.   
-0000f640: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f650: 2020 2020 2020 2020 2020 2020 203c 6469               <di
-0000f660: 7620 636c 6173 733d 227b 2520 626c 6f63  v class="{% bloc
-0000f670: 6b20 335f 746f 705f 6162 635f 6320 257d  k 3_top_abc_c %}
-0000f680: 636f 6c2d 3132 2063 6f6c 2d6d 642d 347b  col-12 col-md-4{
-0000f690: 2520 656e 6462 6c6f 636b 2025 7d22 3e7b  % endblock %}">{
-0000f6a0: 7b20 335f 746f 705f 6320 7d7d 3c2f 6469  { 3_top_c }}</di
-0000f6b0: 763e 0a20 2020 2020 2020 2020 2020 2020  v>.             
-0000f6c0: 2020 2020 2020 2020 2020 2020 2020 207b                 {
-0000f6d0: 2520 656c 6966 2033 5f74 6f70 5f61 2061  % elif 3_top_a a
-0000f6e0: 6e64 2033 5f74 6f70 5f62 2025 7d0a 2020  nd 3_top_b %}.  
-0000f6f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f700: 2020 2020 2020 2020 2020 2020 2020 3c64                <d
-0000f710: 6976 2063 6c61 7373 3d22 7b25 2062 6c6f  iv class="{% blo
-0000f720: 636b 2033 5f74 6f70 5f61 625f 6120 257d  ck 3_top_ab_a %}
-0000f730: 636f 6c2d 3132 2063 6f6c 2d6d 642d 387b  col-12 col-md-8{
-0000f740: 2520 656e 6462 6c6f 636b 2025 7d22 3e7b  % endblock %}">{
-0000f750: 7b20 335f 746f 705f 6120 7d7d 3c2f 6469  { 3_top_a }}</di
-0000f760: 763e 0a20 2020 2020 2020 2020 2020 2020  v>.             
-0000f770: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f780: 2020 203c 6469 7620 636c 6173 733d 227b     <div class="{
-0000f790: 2520 626c 6f63 6b20 335f 746f 705f 6162  % block 3_top_ab
-0000f7a0: 5f62 2025 7d63 6f6c 2d31 3220 636f 6c2d  _b %}col-12 col-
-0000f7b0: 6d64 2d34 7b25 2065 6e64 626c 6f63 6b20  md-4{% endblock 
-0000f7c0: 257d 223e 7b7b 2033 5f74 6f70 5f62 207d  %}">{{ 3_top_b }
-0000f7d0: 7d3c 2f64 6976 3e0a 2020 2020 2020 2020  }</div>.        
-0000f7e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f7f0: 2020 2020 7b25 2065 6c69 6620 335f 746f      {% elif 3_to
-0000f800: 705f 6120 616e 6420 335f 746f 705f 6320  p_a and 3_top_c 
-0000f810: 257d 0a20 2020 2020 2020 2020 2020 2020  %}.             
-0000f820: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f830: 2020 203c 6469 7620 636c 6173 733d 227b     <div class="{
-0000f840: 2520 626c 6f63 6b20 335f 746f 705f 6163  % block 3_top_ac
-0000f850: 5f61 2025 7d63 6f6c 2d31 3220 636f 6c2d  _a %}col-12 col-
-0000f860: 6d64 2d36 7b25 2065 6e64 626c 6f63 6b20  md-6{% endblock 
-0000f870: 257d 223e 7b7b 2033 5f74 6f70 5f61 207d  %}">{{ 3_top_a }
-0000f880: 7d3c 2f64 6976 3e0a 2020 2020 2020 2020  }</div>.        
-0000f890: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f8a0: 2020 2020 2020 2020 3c64 6976 2063 6c61          <div cla
-0000f8b0: 7373 3d22 7b25 2062 6c6f 636b 2033 5f74  ss="{% block 3_t
-0000f8c0: 6f70 5f61 635f 6320 257d 636f 6c2d 3132  op_ac_c %}col-12
-0000f8d0: 2063 6f6c 2d6d 642d 367b 2520 656e 6462   col-md-6{% endb
-0000f8e0: 6c6f 636b 2025 7d22 3e7b 7b20 335f 746f  lock %}">{{ 3_to
-0000f8f0: 705f 6320 7d7d 3c2f 6469 763e 0a20 2020  p_c }}</div>.   
-0000f900: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f910: 2020 2020 2020 2020 207b 2520 656c 6966           {% elif
-0000f920: 2033 5f74 6f70 5f62 2061 6e64 2033 5f74   3_top_b and 3_t
-0000f930: 6f70 5f63 2025 7d0a 2020 2020 2020 2020  op_c %}.        
-0000f940: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f950: 2020 2020 2020 2020 3c64 6976 2063 6c61          <div cla
-0000f960: 7373 3d22 7b25 2062 6c6f 636b 2033 5f74  ss="{% block 3_t
-0000f970: 6f70 5f62 635f 6220 257d 636f 6c2d 3132  op_bc_b %}col-12
-0000f980: 2063 6f6c 2d6d 642d 347b 2520 656e 6462   col-md-4{% endb
-0000f990: 6c6f 636b 2025 7d22 3e7b 7b20 335f 746f  lock %}">{{ 3_to
-0000f9a0: 705f 6220 7d7d 3c2f 6469 763e 0a20 2020  p_b }}</div>.   
-0000f9b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f9c0: 2020 2020 2020 2020 2020 2020 203c 6469               <di
-0000f9d0: 7620 636c 6173 733d 227b 2520 626c 6f63  v class="{% bloc
-0000f9e0: 6b20 335f 746f 705f 6263 5f63 2025 7d63  k 3_top_bc_c %}c
-0000f9f0: 6f6c 2d31 3220 636f 6c2d 6d64 2d38 7b25  ol-12 col-md-8{%
-0000fa00: 2065 6e64 626c 6f63 6b20 257d 223e 7b7b   endblock %}">{{
-0000fa10: 2033 5f74 6f70 5f63 207d 7d3c 2f64 6976   3_top_c }}</div
-0000fa20: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
-0000fa30: 2020 2020 2020 2020 2020 2020 2020 7b25                {%
-0000fa40: 2065 6c73 6520 257d 0a20 2020 2020 2020   else %}.       
-0000fa50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fa60: 2020 2020 2020 2020 203c 6469 7620 636c           <div cl
-0000fa70: 6173 733d 2263 6f6c 2d31 3222 3e7b 7b20  ass="col-12">{{ 
-0000fa80: 335f 746f 705f 6120 7d7d 7b7b 2033 5f74  3_top_a }}{{ 3_t
-0000fa90: 6f70 5f62 207d 7d7b 7b20 335f 746f 705f  op_b }}{{ 3_top_
-0000faa0: 6320 7d7d 3c2f 6469 763e 0a20 2020 2020  c }}</div>.     
-0000fab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fac0: 2020 2020 2020 207b 2520 656e 6469 6620         {% endif 
-0000fad0: 257d 0a20 2020 2020 2020 2020 2020 2020  %}.             
-0000fae0: 2020 2020 2020 2020 2020 203c 2f64 6976             </div
-0000faf0: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
-0000fb00: 2020 2020 2020 3c2f 6469 763e 0a20 2020        </div>.   
-0000fb10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fb20: 207b 2520 656e 6469 6620 257d 0a20 2020   {% endif %}.   
-0000fb30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fb40: 203c 212d 2d20 656e 6420 546f 7020 2d2d   <!-- end Top --
-0000fb50: 3e0a 0a20 2020 2020 2020 2020 2020 2020  >..             
-0000fb60: 2020 2020 2020 203c 212d 2d20 4d69 6464         <!-- Midd
-0000fb70: 6c65 2054 6f70 202d 2d3e 0a20 2020 2020  le Top -->.     
-0000fb80: 2020 2020 2020 2020 2020 2020 2020 207b                 {
-0000fb90: 2520 6966 2033 5f6d 6964 5f74 6f70 5f61  % if 3_mid_top_a
-0000fba0: 206f 7220 335f 6d69 645f 746f 705f 6220   or 3_mid_top_b 
-0000fbb0: 6f72 2033 5f6d 6964 5f74 6f70 5f63 2025  or 3_mid_top_c %
-0000fbc0: 7d0a 2020 2020 2020 2020 2020 2020 2020  }.              
-0000fbd0: 2020 2020 2020 3c64 6976 2063 6c61 7373        <div class
-0000fbe0: 3d22 636f 6c2d 3132 223e 0a20 2020 2020  ="col-12">.     
-0000fbf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fc00: 2020 203c 6469 7620 636c 6173 733d 2272     <div class="r
-0000fc10: 6f77 223e 0a20 2020 2020 2020 2020 2020  ow">.           
+0000e750: 203c 2f64 6976 3e0a 2020 2020 2020 2020   </div>.        
+0000e760: 2020 2020 2020 2020 2020 2020 7b25 2065              {% e
+0000e770: 6e64 6966 2025 7d0a 0a20 2020 2020 2020  ndif %}..       
+0000e780: 2020 2020 2020 2020 2020 2020 203c 212d               <!-
+0000e790: 2d20 426c 6f63 6b73 2069 6e20 626f 7474  - Blocks in bott
+0000e7a0: 6f6d 2070 6f73 6974 696f 6e20 2d2d 3e0a  om position -->.
+0000e7b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e7c0: 2020 2020 7b25 2069 6620 325f 626f 7474      {% if 2_bott
+0000e7d0: 6f6d 5f61 206f 7220 325f 626f 7474 6f6d  om_a or 2_bottom
+0000e7e0: 5f62 206f 7220 325f 626f 7474 6f6d 5f63  _b or 2_bottom_c
+0000e7f0: 2025 7d0a 2020 2020 2020 2020 2020 2020   %}.            
+0000e800: 2020 2020 2020 2020 3c64 6976 2063 6c61          <div cla
+0000e810: 7373 3d22 636f 6c2d 3132 223e 0a20 2020  ss="col-12">.   
+0000e820: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e830: 2020 2020 203c 6469 7620 636c 6173 733d       <div class=
+0000e840: 2272 6f77 223e 0a20 2020 2020 2020 2020  "row">.         
+0000e850: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e860: 2020 207b 2520 6966 2032 5f62 6f74 746f     {% if 2_botto
+0000e870: 6d5f 6120 616e 6420 325f 626f 7474 6f6d  m_a and 2_bottom
+0000e880: 5f62 2061 6e64 2032 5f62 6f74 746f 6d5f  _b and 2_bottom_
+0000e890: 6320 257d 0a20 2020 2020 2020 2020 2020  c %}.           
+0000e8a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e8b0: 2020 2020 203c 6469 7620 636c 6173 733d       <div class=
+0000e8c0: 227b 2520 626c 6f63 6b20 325f 626f 7474  "{% block 2_bott
+0000e8d0: 6f6d 5f61 6263 5f61 2025 7d63 6f6c 2d31  om_abc_a %}col-1
+0000e8e0: 3220 636f 6c2d 6d64 2d34 7b25 2065 6e64  2 col-md-4{% end
+0000e8f0: 626c 6f63 6b20 257d 223e 7b7b 2032 5f62  block %}">{{ 2_b
+0000e900: 6f74 746f 6d5f 6120 7d7d 3c2f 6469 763e  ottom_a }}</div>
+0000e910: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000e920: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e930: 203c 6469 7620 636c 6173 733d 227b 2520   <div class="{% 
+0000e940: 626c 6f63 6b20 325f 626f 7474 6f6d 5f61  block 2_bottom_a
+0000e950: 6263 5f62 2025 7d63 6f6c 2d31 3220 636f  bc_b %}col-12 co
+0000e960: 6c2d 6d64 2d34 7b25 2065 6e64 626c 6f63  l-md-4{% endbloc
+0000e970: 6b20 257d 223e 7b7b 2032 5f62 6f74 746f  k %}">{{ 2_botto
+0000e980: 6d5f 6220 7d7d 3c2f 6469 763e 0a20 2020  m_b }}</div>.   
+0000e990: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e9a0: 2020 2020 2020 2020 2020 2020 203c 6469               <di
+0000e9b0: 7620 636c 6173 733d 227b 2520 626c 6f63  v class="{% bloc
+0000e9c0: 6b20 325f 626f 7474 6f6d 5f61 6263 5f63  k 2_bottom_abc_c
+0000e9d0: 2025 7d63 6f6c 2d31 3220 636f 6c2d 6d64   %}col-12 col-md
+0000e9e0: 2d34 7b25 2065 6e64 626c 6f63 6b20 257d  -4{% endblock %}
+0000e9f0: 223e 7b7b 2032 5f62 6f74 746f 6d5f 6320  ">{{ 2_bottom_c 
+0000ea00: 7d7d 3c2f 6469 763e 0a20 2020 2020 2020  }}</div>.       
+0000ea10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ea20: 2020 2020 207b 2520 656c 6966 2032 5f62       {% elif 2_b
+0000ea30: 6f74 746f 6d5f 6120 616e 6420 325f 626f  ottom_a and 2_bo
+0000ea40: 7474 6f6d 5f62 2025 7d0a 2020 2020 2020  ttom_b %}.      
+0000ea50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ea60: 2020 2020 2020 2020 2020 3c64 6976 2063            <div c
+0000ea70: 6c61 7373 3d22 7b25 2062 6c6f 636b 2032  lass="{% block 2
+0000ea80: 5f62 6f74 746f 6d5f 6162 5f61 2025 7d63  _bottom_ab_a %}c
+0000ea90: 6f6c 2d31 3220 636f 6c2d 6d64 2d38 7b25  ol-12 col-md-8{%
+0000eaa0: 2065 6e64 626c 6f63 6b20 257d 223e 7b7b   endblock %}">{{
+0000eab0: 2032 5f62 6f74 746f 6d5f 6120 7d7d 3c2f   2_bottom_a }}</
+0000eac0: 6469 763e 0a20 2020 2020 2020 2020 2020  div>.           
+0000ead0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000eae0: 2020 2020 203c 6469 7620 636c 6173 733d       <div class=
+0000eaf0: 227b 2520 626c 6f63 6b20 325f 626f 7474  "{% block 2_bott
+0000eb00: 6f6d 5f61 625f 6220 257d 636f 6c2d 3132  om_ab_b %}col-12
+0000eb10: 2063 6f6c 2d6d 642d 347b 2520 656e 6462   col-md-4{% endb
+0000eb20: 6c6f 636b 2025 7d22 3e7b 7b20 325f 626f  lock %}">{{ 2_bo
+0000eb30: 7474 6f6d 5f62 207d 7d3c 2f64 6976 3e0a  ttom_b }}</div>.
+0000eb40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000eb50: 2020 2020 2020 2020 2020 2020 7b25 2065              {% e
+0000eb60: 6c69 6620 325f 626f 7474 6f6d 5f61 2061  lif 2_bottom_a a
+0000eb70: 6e64 2032 5f62 6f74 746f 6d5f 6320 257d  nd 2_bottom_c %}
+0000eb80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000eb90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000eba0: 203c 6469 7620 636c 6173 733d 227b 2520   <div class="{% 
+0000ebb0: 626c 6f63 6b20 325f 626f 7474 6f6d 5f61  block 2_bottom_a
+0000ebc0: 635f 6120 257d 636f 6c2d 3132 2063 6f6c  c_a %}col-12 col
+0000ebd0: 2d6d 642d 367b 2520 656e 6462 6c6f 636b  -md-6{% endblock
+0000ebe0: 2025 7d22 3e7b 7b20 325f 626f 7474 6f6d   %}">{{ 2_bottom
+0000ebf0: 5f61 207d 7d3c 2f64 6976 3e0a 2020 2020  _a }}</div>.    
+0000ec00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ec10: 2020 2020 2020 2020 2020 2020 3c64 6976              <div
+0000ec20: 2063 6c61 7373 3d22 7b25 2062 6c6f 636b   class="{% block
+0000ec30: 2032 5f62 6f74 746f 6d5f 6163 5f63 2025   2_bottom_ac_c %
+0000ec40: 7d63 6f6c 2d31 3220 636f 6c2d 6d64 2d36  }col-12 col-md-6
+0000ec50: 7b25 2065 6e64 626c 6f63 6b20 257d 223e  {% endblock %}">
+0000ec60: 7b7b 2032 5f62 6f74 746f 6d5f 6320 7d7d  {{ 2_bottom_c }}
+0000ec70: 3c2f 6469 763e 0a20 2020 2020 2020 2020  </div>.         
+0000ec80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ec90: 2020 207b 2520 656c 6966 2032 5f62 6f74     {% elif 2_bot
+0000eca0: 746f 6d5f 6220 616e 6420 325f 626f 7474  tom_b and 2_bott
+0000ecb0: 6f6d 5f63 2025 7d0a 2020 2020 2020 2020  om_c %}.        
+0000ecc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ecd0: 2020 2020 2020 2020 3c64 6976 2063 6c61          <div cla
+0000ece0: 7373 3d22 7b25 2062 6c6f 636b 2032 5f62  ss="{% block 2_b
+0000ecf0: 6f74 746f 6d5f 6263 5f62 2025 7d63 6f6c  ottom_bc_b %}col
+0000ed00: 2d31 3220 636f 6c2d 6d64 2d34 7b25 2065  -12 col-md-4{% e
+0000ed10: 6e64 626c 6f63 6b20 257d 223e 7b7b 2032  ndblock %}">{{ 2
+0000ed20: 5f62 6f74 746f 6d5f 6220 7d7d 3c2f 6469  _bottom_b }}</di
+0000ed30: 763e 0a20 2020 2020 2020 2020 2020 2020  v>.             
+0000ed40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ed50: 2020 203c 6469 7620 636c 6173 733d 227b     <div class="{
+0000ed60: 2520 626c 6f63 6b20 325f 626f 7474 6f6d  % block 2_bottom
+0000ed70: 5f62 635f 6320 257d 636f 6c2d 3132 2063  _bc_c %}col-12 c
+0000ed80: 6f6c 2d6d 642d 387b 2520 656e 6462 6c6f  ol-md-8{% endblo
+0000ed90: 636b 2025 7d22 3e7b 7b20 325f 626f 7474  ck %}">{{ 2_bott
+0000eda0: 6f6d 5f63 207d 7d3c 2f64 6976 3e0a 2020  om_c }}</div>.  
+0000edb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000edc0: 2020 2020 2020 2020 2020 7b25 2065 6c73            {% els
+0000edd0: 6520 257d 0a20 2020 2020 2020 2020 2020  e %}.           
+0000ede0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000edf0: 2020 2020 203c 6469 7620 636c 6173 733d       <div class=
+0000ee00: 2263 6f6c 2d31 3222 3e7b 7b20 325f 626f  "col-12">{{ 2_bo
+0000ee10: 7474 6f6d 5f61 207d 7d7b 7b20 325f 626f  ttom_a }}{{ 2_bo
+0000ee20: 7474 6f6d 5f62 207d 7d7b 7b20 325f 626f  ttom_b }}{{ 2_bo
+0000ee30: 7474 6f6d 5f63 207d 7d3c 2f64 6976 3e0a  ttom_c }}</div>.
+0000ee40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ee50: 2020 2020 2020 2020 2020 2020 7b25 2065              {% e
+0000ee60: 6e64 6966 2025 7d0a 2020 2020 2020 2020  ndif %}.        
+0000ee70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ee80: 3c2f 6469 763e 0a20 2020 2020 2020 2020  </div>.         
+0000ee90: 2020 2020 2020 2020 2020 203c 2f64 6976             </div
+0000eea0: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
+0000eeb0: 2020 2020 2020 7b25 2065 6e64 6966 2025        {% endif %
+0000eec0: 7d0a 0a20 2020 2020 2020 2020 2020 2020  }..             
+0000eed0: 2020 203c 2f64 6976 3e0a 2020 2020 2020     </div>.      
+0000eee0: 2020 2020 2020 3c2f 6469 763e 0a20 2020        </div>.   
+0000eef0: 2020 2020 203c 2f64 6976 3e0a 2020 2020       </div>.    
+0000ef00: 7b25 2065 6e64 6966 2025 7d0a 2020 2020  {% endif %}.    
+0000ef10: 7b25 2065 6e64 626c 6f63 6b20 7365 6374  {% endblock sect
+0000ef20: 696f 6e5f 3220 257d 0a20 2020 203c 212d  ion_2 %}.    <!-
+0000ef30: 2d20 656e 6420 5365 6374 696f 6e20 3220  - end Section 2 
+0000ef40: 2d2d 3e0a 0a20 2020 203c 212d 2d2d 2d2d  -->..    <!-----
+0000ef50: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+0000ef60: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+0000ef70: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+0000ef80: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+0000ef90: 3e0a 0a20 2020 203c 212d 2d20 5365 6374  >..    <!-- Sect
+0000efa0: 696f 6e20 3320 2d2d 3e0a 2020 2020 7b25  ion 3 -->.    {%
+0000efb0: 2062 6c6f 636b 2073 6563 7469 6f6e 5f33   block section_3
+0000efc0: 2025 7d0a 2020 2020 7b25 2062 6c6f 636b   %}.    {% block
+0000efd0: 735f 696e 5f70 6f73 6974 696f 6e20 7365  s_in_position se
+0000efe0: 6374 696f 6e3d 2273 6563 7469 6f6e 2d33  ction="section-3
+0000eff0: 2220 6173 2073 6563 7469 6f6e 5f33 2025  " as section_3 %
+0000f000: 7d0a 2020 2020 7b25 2069 6620 7365 6374  }.    {% if sect
+0000f010: 696f 6e5f 3320 257d 0a20 2020 2020 2020  ion_3 %}.       
+0000f020: 207b 2520 6c6f 6164 5f62 6c6f 636b 7320   {% load_blocks 
+0000f030: 7365 6374 696f 6e3d 2233 2d74 6f70 2d61  section="3-top-a
+0000f040: 2220 6173 2033 5f74 6f70 5f61 2025 7d0a  " as 3_top_a %}.
+0000f050: 2020 2020 2020 2020 7b25 206c 6f61 645f          {% load_
+0000f060: 626c 6f63 6b73 2073 6563 7469 6f6e 3d22  blocks section="
+0000f070: 332d 746f 702d 6222 2061 7320 335f 746f  3-top-b" as 3_to
+0000f080: 705f 6220 257d 0a20 2020 2020 2020 207b  p_b %}.        {
+0000f090: 2520 6c6f 6164 5f62 6c6f 636b 7320 7365  % load_blocks se
+0000f0a0: 6374 696f 6e3d 2233 2d74 6f70 2d63 2220  ction="3-top-c" 
+0000f0b0: 6173 2033 5f74 6f70 5f63 2025 7d0a 0a20  as 3_top_c %}.. 
+0000f0c0: 2020 2020 2020 207b 2520 6c6f 6164 5f62         {% load_b
+0000f0d0: 6c6f 636b 7320 7365 6374 696f 6e3d 2233  locks section="3
+0000f0e0: 2d6d 6964 2d74 6f70 2d61 2220 6173 2033  -mid-top-a" as 3
+0000f0f0: 5f6d 6964 5f74 6f70 5f61 2025 7d0a 2020  _mid_top_a %}.  
+0000f100: 2020 2020 2020 7b25 206c 6f61 645f 626c        {% load_bl
+0000f110: 6f63 6b73 2073 6563 7469 6f6e 3d22 332d  ocks section="3-
+0000f120: 6d69 642d 746f 702d 6222 2061 7320 335f  mid-top-b" as 3_
+0000f130: 6d69 645f 746f 705f 6220 257d 0a20 2020  mid_top_b %}.   
+0000f140: 2020 2020 207b 2520 6c6f 6164 5f62 6c6f       {% load_blo
+0000f150: 636b 7320 7365 6374 696f 6e3d 2233 2d6d  cks section="3-m
+0000f160: 6964 2d74 6f70 2d63 2220 6173 2033 5f6d  id-top-c" as 3_m
+0000f170: 6964 5f74 6f70 5f63 2025 7d0a 0a20 2020  id_top_c %}..   
+0000f180: 2020 2020 207b 2520 6c6f 6164 5f62 6c6f       {% load_blo
+0000f190: 636b 7320 7365 6374 696f 6e3d 2233 2d6c  cks section="3-l
+0000f1a0: 6566 742d 6122 2061 7320 335f 6c65 6674  eft-a" as 3_left
+0000f1b0: 5f61 2025 7d0a 2020 2020 2020 2020 7b25  _a %}.        {%
+0000f1c0: 206c 6f61 645f 626c 6f63 6b73 2073 6563   load_blocks sec
+0000f1d0: 7469 6f6e 3d22 332d 6c65 6674 2d62 2220  tion="3-left-b" 
+0000f1e0: 6173 2033 5f6c 6566 745f 6220 257d 0a0a  as 3_left_b %}..
+0000f1f0: 2020 2020 2020 2020 7b25 206c 6f61 645f          {% load_
+0000f200: 626c 6f63 6b73 2073 6563 7469 6f6e 3d22  blocks section="
+0000f210: 332d 6365 6e74 6572 2d74 6f70 2d61 2220  3-center-top-a" 
+0000f220: 6173 2033 5f63 656e 7465 725f 746f 705f  as 3_center_top_
+0000f230: 6120 257d 0a20 2020 2020 2020 207b 2520  a %}.        {% 
+0000f240: 6c6f 6164 5f62 6c6f 636b 7320 7365 6374  load_blocks sect
+0000f250: 696f 6e3d 2233 2d63 656e 7465 722d 746f  ion="3-center-to
+0000f260: 702d 6222 2061 7320 335f 6365 6e74 6572  p-b" as 3_center
+0000f270: 5f74 6f70 5f62 2025 7d0a 2020 2020 2020  _top_b %}.      
+0000f280: 2020 7b25 206c 6f61 645f 626c 6f63 6b73    {% load_blocks
+0000f290: 2073 6563 7469 6f6e 3d22 332d 6365 6e74   section="3-cent
+0000f2a0: 6572 2d74 6f70 2d63 2220 6173 2033 5f63  er-top-c" as 3_c
+0000f2b0: 656e 7465 725f 746f 705f 6320 257d 0a0a  enter_top_c %}..
+0000f2c0: 2020 2020 2020 2020 7b25 206c 6f61 645f          {% load_
+0000f2d0: 626c 6f63 6b73 2073 6563 7469 6f6e 3d22  blocks section="
+0000f2e0: 332d 6365 6e74 6572 2d6d 6964 2d74 6f70  3-center-mid-top
+0000f2f0: 2d61 2220 6173 2033 5f63 656e 7465 725f  -a" as 3_center_
+0000f300: 6d69 645f 746f 705f 6120 257d 0a20 2020  mid_top_a %}.   
+0000f310: 2020 2020 207b 2520 6c6f 6164 5f62 6c6f       {% load_blo
+0000f320: 636b 7320 7365 6374 696f 6e3d 2233 2d63  cks section="3-c
+0000f330: 656e 7465 722d 6d69 642d 746f 702d 6222  enter-mid-top-b"
+0000f340: 2061 7320 335f 6365 6e74 6572 5f6d 6964   as 3_center_mid
+0000f350: 5f74 6f70 5f62 2025 7d0a 2020 2020 2020  _top_b %}.      
+0000f360: 2020 7b25 206c 6f61 645f 626c 6f63 6b73    {% load_blocks
+0000f370: 2073 6563 7469 6f6e 3d22 332d 6365 6e74   section="3-cent
+0000f380: 6572 2d6d 6964 2d74 6f70 2d63 2220 6173  er-mid-top-c" as
+0000f390: 2033 5f63 656e 7465 725f 6d69 645f 746f   3_center_mid_to
+0000f3a0: 705f 6320 257d 0a0a 2020 2020 2020 2020  p_c %}..        
+0000f3b0: 7b25 206c 6f61 645f 626c 6f63 6b73 2073  {% load_blocks s
+0000f3c0: 6563 7469 6f6e 3d22 332d 6365 6e74 6572  ection="3-center
+0000f3d0: 2d63 6f6e 7465 6e74 2220 6173 2033 5f63  -content" as 3_c
+0000f3e0: 656e 7465 725f 636f 6e74 656e 7420 257d  enter_content %}
+0000f3f0: 0a0a 2020 2020 2020 2020 7b25 206c 6f61  ..        {% loa
+0000f400: 645f 626c 6f63 6b73 2073 6563 7469 6f6e  d_blocks section
+0000f410: 3d22 332d 6365 6e74 6572 2d6d 6964 2d62  ="3-center-mid-b
+0000f420: 6f74 746f 6d2d 6122 2061 7320 335f 6365  ottom-a" as 3_ce
+0000f430: 6e74 6572 5f6d 6964 5f62 6f74 746f 6d5f  nter_mid_bottom_
+0000f440: 6120 257d 0a20 2020 2020 2020 207b 2520  a %}.        {% 
+0000f450: 6c6f 6164 5f62 6c6f 636b 7320 7365 6374  load_blocks sect
+0000f460: 696f 6e3d 2233 2d63 656e 7465 722d 6d69  ion="3-center-mi
+0000f470: 642d 626f 7474 6f6d 2d62 2220 6173 2033  d-bottom-b" as 3
+0000f480: 5f63 656e 7465 725f 6d69 645f 626f 7474  _center_mid_bott
+0000f490: 6f6d 5f62 2025 7d0a 2020 2020 2020 2020  om_b %}.        
+0000f4a0: 7b25 206c 6f61 645f 626c 6f63 6b73 2073  {% load_blocks s
+0000f4b0: 6563 7469 6f6e 3d22 332d 6365 6e74 6572  ection="3-center
+0000f4c0: 2d6d 6964 2d62 6f74 746f 6d2d 6322 2061  -mid-bottom-c" a
+0000f4d0: 7320 335f 6365 6e74 6572 5f6d 6964 5f62  s 3_center_mid_b
+0000f4e0: 6f74 746f 6d5f 6320 257d 0a0a 2020 2020  ottom_c %}..    
+0000f4f0: 2020 2020 7b25 206c 6f61 645f 626c 6f63      {% load_bloc
+0000f500: 6b73 2073 6563 7469 6f6e 3d22 332d 6365  ks section="3-ce
+0000f510: 6e74 6572 2d62 6f74 746f 6d2d 6122 2061  nter-bottom-a" a
+0000f520: 7320 335f 6365 6e74 6572 5f62 6f74 746f  s 3_center_botto
+0000f530: 6d5f 6120 257d 0a20 2020 2020 2020 207b  m_a %}.        {
+0000f540: 2520 6c6f 6164 5f62 6c6f 636b 7320 7365  % load_blocks se
+0000f550: 6374 696f 6e3d 2233 2d63 656e 7465 722d  ction="3-center-
+0000f560: 626f 7474 6f6d 2d62 2220 6173 2033 5f63  bottom-b" as 3_c
+0000f570: 656e 7465 725f 626f 7474 6f6d 5f62 2025  enter_bottom_b %
+0000f580: 7d0a 2020 2020 2020 2020 7b25 206c 6f61  }.        {% loa
+0000f590: 645f 626c 6f63 6b73 2073 6563 7469 6f6e  d_blocks section
+0000f5a0: 3d22 332d 6365 6e74 6572 2d62 6f74 746f  ="3-center-botto
+0000f5b0: 6d2d 6322 2061 7320 335f 6365 6e74 6572  m-c" as 3_center
+0000f5c0: 5f62 6f74 746f 6d5f 6320 257d 0a0a 2020  _bottom_c %}..  
+0000f5d0: 2020 2020 2020 7b25 206c 6f61 645f 626c        {% load_bl
+0000f5e0: 6f63 6b73 2073 6563 7469 6f6e 3d22 332d  ocks section="3-
+0000f5f0: 7269 6768 742d 6122 2061 7320 335f 7269  right-a" as 3_ri
+0000f600: 6768 745f 6120 257d 0a20 2020 2020 2020  ght_a %}.       
+0000f610: 207b 2520 6c6f 6164 5f62 6c6f 636b 7320   {% load_blocks 
+0000f620: 7365 6374 696f 6e3d 2233 2d72 6967 6874  section="3-right
+0000f630: 2d62 2220 6173 2033 5f72 6967 6874 5f62  -b" as 3_right_b
+0000f640: 2025 7d0a 0a20 2020 2020 2020 207b 2520   %}..        {% 
+0000f650: 6c6f 6164 5f62 6c6f 636b 7320 7365 6374  load_blocks sect
+0000f660: 696f 6e3d 2233 2d6d 6964 2d62 6f74 746f  ion="3-mid-botto
+0000f670: 6d2d 6122 2061 7320 335f 6d69 645f 626f  m-a" as 3_mid_bo
+0000f680: 7474 6f6d 5f61 2025 7d0a 2020 2020 2020  ttom_a %}.      
+0000f690: 2020 7b25 206c 6f61 645f 626c 6f63 6b73    {% load_blocks
+0000f6a0: 2073 6563 7469 6f6e 3d22 332d 6d69 642d   section="3-mid-
+0000f6b0: 626f 7474 6f6d 2d62 2220 6173 2033 5f6d  bottom-b" as 3_m
+0000f6c0: 6964 5f62 6f74 746f 6d5f 6220 257d 0a20  id_bottom_b %}. 
+0000f6d0: 2020 2020 2020 207b 2520 6c6f 6164 5f62         {% load_b
+0000f6e0: 6c6f 636b 7320 7365 6374 696f 6e3d 2233  locks section="3
+0000f6f0: 2d6d 6964 2d62 6f74 746f 6d2d 6322 2061  -mid-bottom-c" a
+0000f700: 7320 335f 6d69 645f 626f 7474 6f6d 5f63  s 3_mid_bottom_c
+0000f710: 2025 7d0a 0a20 2020 2020 2020 207b 2520   %}..        {% 
+0000f720: 6c6f 6164 5f62 6c6f 636b 7320 7365 6374  load_blocks sect
+0000f730: 696f 6e3d 2233 2d62 6f74 746f 6d2d 6122  ion="3-bottom-a"
+0000f740: 2061 7320 335f 626f 7474 6f6d 5f61 2025   as 3_bottom_a %
+0000f750: 7d0a 2020 2020 2020 2020 7b25 206c 6f61  }.        {% loa
+0000f760: 645f 626c 6f63 6b73 2073 6563 7469 6f6e  d_blocks section
+0000f770: 3d22 332d 626f 7474 6f6d 2d62 2220 6173  ="3-bottom-b" as
+0000f780: 2033 5f62 6f74 746f 6d5f 6220 257d 0a20   3_bottom_b %}. 
+0000f790: 2020 2020 2020 207b 2520 6c6f 6164 5f62         {% load_b
+0000f7a0: 6c6f 636b 7320 7365 6374 696f 6e3d 2233  locks section="3
+0000f7b0: 2d62 6f74 746f 6d2d 6322 2061 7320 335f  -bottom-c" as 3_
+0000f7c0: 626f 7474 6f6d 5f63 2025 7d0a 0a20 2020  bottom_c %}..   
+0000f7d0: 2020 2020 203c 6469 7620 636c 6173 733d       <div class=
+0000f7e0: 227b 2520 626c 6f63 6b20 7365 6374 696f  "{% block sectio
+0000f7f0: 6e5f 335f 636c 6173 7365 7320 257d 7079  n_3_classes %}py
+0000f800: 2d35 7b25 2065 6e64 626c 6f63 6b20 257d  -5{% endblock %}
+0000f810: 223e 0a20 2020 2020 2020 2020 2020 203c  ">.            <
+0000f820: 6469 7620 636c 6173 733d 2263 6f6e 7461  div class="conta
+0000f830: 696e 6572 223e 0a20 2020 2020 2020 2020  iner">.         
+0000f840: 2020 2020 2020 203c 6469 7620 636c 6173         <div clas
+0000f850: 733d 2272 6f77 206d 782d 3022 3e0a 0a20  s="row mx-0">.. 
+0000f860: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f870: 2020 203c 212d 2d20 546f 7020 2d2d 3e0a     <!-- Top -->.
+0000f880: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f890: 2020 2020 7b25 2069 6620 335f 746f 705f      {% if 3_top_
+0000f8a0: 6120 6f72 2033 5f74 6f70 5f62 206f 7220  a or 3_top_b or 
+0000f8b0: 335f 746f 705f 6320 257d 0a20 2020 2020  3_top_c %}.     
+0000f8c0: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+0000f8d0: 6469 7620 636c 6173 733d 2263 6f6c 2d31  div class="col-1
+0000f8e0: 3222 3e0a 2020 2020 2020 2020 2020 2020  2">.            
+0000f8f0: 2020 2020 2020 2020 2020 2020 3c64 6976              <div
+0000f900: 2063 6c61 7373 3d22 726f 7722 3e0a 2020   class="row">.  
+0000f910: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f920: 2020 2020 2020 2020 2020 7b25 2069 6620            {% if 
+0000f930: 335f 746f 705f 6120 616e 6420 335f 746f  3_top_a and 3_to
+0000f940: 705f 6220 616e 6420 335f 746f 705f 6320  p_b and 3_top_c 
+0000f950: 257d 0a20 2020 2020 2020 2020 2020 2020  %}.             
+0000f960: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f970: 2020 203c 6469 7620 636c 6173 733d 227b     <div class="{
+0000f980: 2520 626c 6f63 6b20 335f 746f 705f 6162  % block 3_top_ab
+0000f990: 635f 6120 257d 636f 6c2d 3132 2063 6f6c  c_a %}col-12 col
+0000f9a0: 2d6d 642d 347b 2520 656e 6462 6c6f 636b  -md-4{% endblock
+0000f9b0: 2025 7d22 3e7b 7b20 335f 746f 705f 6120   %}">{{ 3_top_a 
+0000f9c0: 7d7d 3c2f 6469 763e 0a20 2020 2020 2020  }}</div>.       
+0000f9d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f9e0: 2020 2020 2020 2020 203c 6469 7620 636c           <div cl
+0000f9f0: 6173 733d 227b 2520 626c 6f63 6b20 335f  ass="{% block 3_
+0000fa00: 746f 705f 6162 635f 6220 257d 636f 6c2d  top_abc_b %}col-
+0000fa10: 3132 2063 6f6c 2d6d 642d 347b 2520 656e  12 col-md-4{% en
+0000fa20: 6462 6c6f 636b 2025 7d22 3e7b 7b20 335f  dblock %}">{{ 3_
+0000fa30: 746f 705f 6220 7d7d 3c2f 6469 763e 0a20  top_b }}</div>. 
+0000fa40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fa50: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+0000fa60: 6469 7620 636c 6173 733d 227b 2520 626c  div class="{% bl
+0000fa70: 6f63 6b20 335f 746f 705f 6162 635f 6320  ock 3_top_abc_c 
+0000fa80: 257d 636f 6c2d 3132 2063 6f6c 2d6d 642d  %}col-12 col-md-
+0000fa90: 347b 2520 656e 6462 6c6f 636b 2025 7d22  4{% endblock %}"
+0000faa0: 3e7b 7b20 335f 746f 705f 6320 7d7d 3c2f  >{{ 3_top_c }}</
+0000fab0: 6469 763e 0a20 2020 2020 2020 2020 2020  div>.           
+0000fac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fad0: 207b 2520 656c 6966 2033 5f74 6f70 5f61   {% elif 3_top_a
+0000fae0: 2061 6e64 2033 5f74 6f70 5f62 2025 7d0a   and 3_top_b %}.
+0000faf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fb00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fb10: 3c64 6976 2063 6c61 7373 3d22 7b25 2062  <div class="{% b
+0000fb20: 6c6f 636b 2033 5f74 6f70 5f61 625f 6120  lock 3_top_ab_a 
+0000fb30: 257d 636f 6c2d 3132 2063 6f6c 2d6d 642d  %}col-12 col-md-
+0000fb40: 387b 2520 656e 6462 6c6f 636b 2025 7d22  8{% endblock %}"
+0000fb50: 3e7b 7b20 335f 746f 705f 6120 7d7d 3c2f  >{{ 3_top_a }}</
+0000fb60: 6469 763e 0a20 2020 2020 2020 2020 2020  div>.           
+0000fb70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fb80: 2020 2020 203c 6469 7620 636c 6173 733d       <div class=
+0000fb90: 227b 2520 626c 6f63 6b20 335f 746f 705f  "{% block 3_top_
+0000fba0: 6162 5f62 2025 7d63 6f6c 2d31 3220 636f  ab_b %}col-12 co
+0000fbb0: 6c2d 6d64 2d34 7b25 2065 6e64 626c 6f63  l-md-4{% endbloc
+0000fbc0: 6b20 257d 223e 7b7b 2033 5f74 6f70 5f62  k %}">{{ 3_top_b
+0000fbd0: 207d 7d3c 2f64 6976 3e0a 2020 2020 2020   }}</div>.      
+0000fbe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fbf0: 2020 2020 2020 7b25 2065 6c69 6620 335f        {% elif 3_
+0000fc00: 746f 705f 6120 616e 6420 335f 746f 705f  top_a and 3_top_
+0000fc10: 6320 257d 0a20 2020 2020 2020 2020 2020  c %}.           
 0000fc20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fc30: 207b 2520 6966 2033 5f6d 6964 5f74 6f70   {% if 3_mid_top
-0000fc40: 5f61 2061 6e64 2033 5f6d 6964 5f74 6f70  _a and 3_mid_top
-0000fc50: 5f62 2061 6e64 2033 5f6d 6964 5f74 6f70  _b and 3_mid_top
-0000fc60: 5f63 2025 7d0a 2020 2020 2020 2020 2020  _c %}.          
-0000fc70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fc80: 2020 2020 2020 3c64 6976 2063 6c61 7373        <div class
-0000fc90: 3d22 7b25 2062 6c6f 636b 2033 5f6d 6964  ="{% block 3_mid
-0000fca0: 5f74 6f70 5f61 6263 5f61 2025 7d63 6f6c  _top_abc_a %}col
-0000fcb0: 2d31 3220 636f 6c2d 6d64 2d34 7b25 2065  -12 col-md-4{% e
-0000fcc0: 6e64 626c 6f63 6b20 257d 223e 7b7b 2033  ndblock %}">{{ 3
-0000fcd0: 5f6d 6964 5f74 6f70 5f61 207d 7d3c 2f64  _mid_top_a }}</d
-0000fce0: 6976 3e0a 2020 2020 2020 2020 2020 2020  iv>.            
-0000fcf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fd00: 2020 2020 3c64 6976 2063 6c61 7373 3d22      <div class="
-0000fd10: 7b25 2062 6c6f 636b 2033 5f6d 6964 5f74  {% block 3_mid_t
-0000fd20: 6f70 5f61 6263 5f62 2025 7d63 6f6c 2d31  op_abc_b %}col-1
-0000fd30: 3220 636f 6c2d 6d64 2d34 7b25 2065 6e64  2 col-md-4{% end
-0000fd40: 626c 6f63 6b20 257d 223e 7b7b 2033 5f6d  block %}">{{ 3_m
-0000fd50: 6964 5f74 6f70 5f62 207d 7d3c 2f64 6976  id_top_b }}</div
-0000fd60: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
-0000fd70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fd80: 2020 3c64 6976 2063 6c61 7373 3d22 7b25    <div class="{%
-0000fd90: 2062 6c6f 636b 2033 5f6d 6964 5f74 6f70   block 3_mid_top
-0000fda0: 5f61 6263 5f63 2025 7d63 6f6c 2d31 3220  _abc_c %}col-12 
-0000fdb0: 636f 6c2d 6d64 2d34 7b25 2065 6e64 626c  col-md-4{% endbl
-0000fdc0: 6f63 6b20 257d 223e 7b7b 2033 5f6d 6964  ock %}">{{ 3_mid
-0000fdd0: 5f74 6f70 5f63 207d 7d3c 2f64 6976 3e0a  _top_c }}</div>.
-0000fde0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fdf0: 2020 2020 2020 2020 2020 2020 7b25 2065              {% e
-0000fe00: 6c69 6620 335f 6d69 645f 746f 705f 6120  lif 3_mid_top_a 
-0000fe10: 616e 6420 335f 6d69 645f 746f 705f 6220  and 3_mid_top_b 
-0000fe20: 257d 0a20 2020 2020 2020 2020 2020 2020  %}.             
+0000fc30: 2020 2020 203c 6469 7620 636c 6173 733d       <div class=
+0000fc40: 227b 2520 626c 6f63 6b20 335f 746f 705f  "{% block 3_top_
+0000fc50: 6163 5f61 2025 7d63 6f6c 2d31 3220 636f  ac_a %}col-12 co
+0000fc60: 6c2d 6d64 2d36 7b25 2065 6e64 626c 6f63  l-md-6{% endbloc
+0000fc70: 6b20 257d 223e 7b7b 2033 5f74 6f70 5f61  k %}">{{ 3_top_a
+0000fc80: 207d 7d3c 2f64 6976 3e0a 2020 2020 2020   }}</div>.      
+0000fc90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fca0: 2020 2020 2020 2020 2020 3c64 6976 2063            <div c
+0000fcb0: 6c61 7373 3d22 7b25 2062 6c6f 636b 2033  lass="{% block 3
+0000fcc0: 5f74 6f70 5f61 635f 6320 257d 636f 6c2d  _top_ac_c %}col-
+0000fcd0: 3132 2063 6f6c 2d6d 642d 367b 2520 656e  12 col-md-6{% en
+0000fce0: 6462 6c6f 636b 2025 7d22 3e7b 7b20 335f  dblock %}">{{ 3_
+0000fcf0: 746f 705f 6320 7d7d 3c2f 6469 763e 0a20  top_c }}</div>. 
+0000fd00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fd10: 2020 2020 2020 2020 2020 207b 2520 656c             {% el
+0000fd20: 6966 2033 5f74 6f70 5f62 2061 6e64 2033  if 3_top_b and 3
+0000fd30: 5f74 6f70 5f63 2025 7d0a 2020 2020 2020  _top_c %}.      
+0000fd40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fd50: 2020 2020 2020 2020 2020 3c64 6976 2063            <div c
+0000fd60: 6c61 7373 3d22 7b25 2062 6c6f 636b 2033  lass="{% block 3
+0000fd70: 5f74 6f70 5f62 635f 6220 257d 636f 6c2d  _top_bc_b %}col-
+0000fd80: 3132 2063 6f6c 2d6d 642d 347b 2520 656e  12 col-md-4{% en
+0000fd90: 6462 6c6f 636b 2025 7d22 3e7b 7b20 335f  dblock %}">{{ 3_
+0000fda0: 746f 705f 6220 7d7d 3c2f 6469 763e 0a20  top_b }}</div>. 
+0000fdb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fdc0: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+0000fdd0: 6469 7620 636c 6173 733d 227b 2520 626c  div class="{% bl
+0000fde0: 6f63 6b20 335f 746f 705f 6263 5f63 2025  ock 3_top_bc_c %
+0000fdf0: 7d63 6f6c 2d31 3220 636f 6c2d 6d64 2d38  }col-12 col-md-8
+0000fe00: 7b25 2065 6e64 626c 6f63 6b20 257d 223e  {% endblock %}">
+0000fe10: 7b7b 2033 5f74 6f70 5f63 207d 7d3c 2f64  {{ 3_top_c }}</d
+0000fe20: 6976 3e0a 2020 2020 2020 2020 2020 2020  iv>.            
 0000fe30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fe40: 2020 203c 6469 7620 636c 6173 733d 227b     <div class="{
-0000fe50: 2520 626c 6f63 6b20 335f 6d69 645f 746f  % block 3_mid_to
-0000fe60: 705f 6162 5f61 2025 7d63 6f6c 2d31 3220  p_ab_a %}col-12 
-0000fe70: 636f 6c2d 6d64 2d38 7b25 2065 6e64 626c  col-md-8{% endbl
-0000fe80: 6f63 6b20 257d 223e 7b7b 2033 5f6d 6964  ock %}">{{ 3_mid
-0000fe90: 5f74 6f70 5f61 207d 7d3c 2f64 6976 3e0a  _top_a }}</div>.
-0000fea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fe40: 7b25 2065 6c73 6520 257d 0a20 2020 2020  {% else %}.     
+0000fe50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fe60: 2020 2020 2020 2020 2020 203c 6469 7620             <div 
+0000fe70: 636c 6173 733d 2263 6f6c 2d31 3222 3e7b  class="col-12">{
+0000fe80: 7b20 335f 746f 705f 6120 7d7d 7b7b 2033  { 3_top_a }}{{ 3
+0000fe90: 5f74 6f70 5f62 207d 7d7b 7b20 335f 746f  _top_b }}{{ 3_to
+0000fea0: 705f 6320 7d7d 3c2f 6469 763e 0a20 2020  p_c }}</div>.   
 0000feb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fec0: 3c64 6976 2063 6c61 7373 3d22 7b25 2062  <div class="{% b
-0000fed0: 6c6f 636b 2033 5f6d 6964 5f74 6f70 5f61  lock 3_mid_top_a
-0000fee0: 625f 6220 257d 636f 6c2d 3132 2063 6f6c  b_b %}col-12 col
-0000fef0: 2d6d 642d 347b 2520 656e 6462 6c6f 636b  -md-4{% endblock
-0000ff00: 2025 7d22 3e7b 7b20 335f 6d69 645f 746f   %}">{{ 3_mid_to
-0000ff10: 705f 6220 7d7d 3c2f 6469 763e 0a20 2020  p_b }}</div>.   
-0000ff20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ff30: 2020 2020 2020 2020 207b 2520 656c 6966           {% elif
-0000ff40: 2033 5f6d 6964 5f74 6f70 5f61 2061 6e64   3_mid_top_a and
-0000ff50: 2033 5f6d 6964 5f74 6f70 5f63 2025 7d0a   3_mid_top_c %}.
-0000ff60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ff70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ff80: 3c64 6976 2063 6c61 7373 3d22 7b25 2062  <div class="{% b
-0000ff90: 6c6f 636b 2033 5f6d 6964 5f74 6f70 5f61  lock 3_mid_top_a
-0000ffa0: 635f 6120 257d 636f 6c2d 3132 2063 6f6c  c_a %}col-12 col
-0000ffb0: 2d6d 642d 367b 2520 656e 6462 6c6f 636b  -md-6{% endblock
-0000ffc0: 2025 7d22 3e7b 7b20 335f 6d69 645f 746f   %}">{{ 3_mid_to
-0000ffd0: 705f 6120 7d7d 3c2f 6469 763e 0a20 2020  p_a }}</div>.   
-0000ffe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fff0: 2020 2020 2020 2020 2020 2020 203c 6469               <di
-00010000: 7620 636c 6173 733d 227b 2520 626c 6f63  v class="{% bloc
-00010010: 6b20 335f 6d69 645f 746f 705f 6163 5f63  k 3_mid_top_ac_c
-00010020: 2025 7d63 6f6c 2d31 3220 636f 6c2d 6d64   %}col-12 col-md
-00010030: 2d36 7b25 2065 6e64 626c 6f63 6b20 257d  -6{% endblock %}
-00010040: 223e 7b7b 2033 5f6d 6964 5f74 6f70 5f63  ">{{ 3_mid_top_c
-00010050: 207d 7d3c 2f64 6976 3e0a 2020 2020 2020   }}</div>.      
-00010060: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010070: 2020 2020 2020 7b25 2065 6c69 6620 335f        {% elif 3_
-00010080: 6d69 645f 746f 705f 6220 616e 6420 335f  mid_top_b and 3_
-00010090: 6d69 645f 746f 705f 6320 257d 0a20 2020  mid_top_c %}.   
-000100a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000100b0: 2020 2020 2020 2020 2020 2020 203c 6469               <di
-000100c0: 7620 636c 6173 733d 227b 2520 626c 6f63  v class="{% bloc
-000100d0: 6b20 335f 6d69 645f 746f 705f 6263 5f62  k 3_mid_top_bc_b
-000100e0: 2025 7d63 6f6c 2d31 3220 636f 6c2d 6d64   %}col-12 col-md
-000100f0: 2d34 7b25 2065 6e64 626c 6f63 6b20 257d  -4{% endblock %}
-00010100: 223e 7b7b 2033 5f6d 6964 5f74 6f70 5f62  ">{{ 3_mid_top_b
-00010110: 207d 7d3c 2f64 6976 3e0a 2020 2020 2020   }}</div>.      
-00010120: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010130: 2020 2020 2020 2020 2020 3c64 6976 2063            <div c
-00010140: 6c61 7373 3d22 7b25 2062 6c6f 636b 2033  lass="{% block 3
-00010150: 5f6d 6964 5f74 6f70 5f62 635f 6320 257d  _mid_top_bc_c %}
-00010160: 636f 6c2d 3132 2063 6f6c 2d6d 642d 387b  col-12 col-md-8{
-00010170: 2520 656e 6462 6c6f 636b 2025 7d22 3e7b  % endblock %}">{
-00010180: 7b20 335f 6d69 645f 746f 705f 6320 7d7d  { 3_mid_top_c }}
-00010190: 3c2f 6469 763e 0a20 2020 2020 2020 2020  </div>.         
-000101a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000101b0: 2020 207b 2520 656c 7365 2025 7d0a 2020     {% else %}.  
-000101c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000101d0: 2020 2020 2020 2020 2020 2020 2020 3c64                <d
-000101e0: 6976 2063 6c61 7373 3d22 636f 6c2d 3132  iv class="col-12
-000101f0: 223e 7b7b 2033 5f6d 6964 5f74 6f70 5f61  ">{{ 3_mid_top_a
-00010200: 207d 7d7b 7b20 335f 6d69 645f 746f 705f   }}{{ 3_mid_top_
-00010210: 6220 7d7d 7b7b 2033 5f6d 6964 5f74 6f70  b }}{{ 3_mid_top
-00010220: 5f63 207d 7d3c 2f64 6976 3e0a 2020 2020  _c }}</div>.    
+0000fec0: 2020 2020 2020 2020 207b 2520 656e 6469           {% endi
+0000fed0: 6620 257d 0a20 2020 2020 2020 2020 2020  f %}.           
+0000fee0: 2020 2020 2020 2020 2020 2020 203c 2f64               </d
+0000fef0: 6976 3e0a 2020 2020 2020 2020 2020 2020  iv>.            
+0000ff00: 2020 2020 2020 2020 3c2f 6469 763e 0a20          </div>. 
+0000ff10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ff20: 2020 207b 2520 656e 6469 6620 257d 0a20     {% endif %}. 
+0000ff30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ff40: 2020 203c 212d 2d20 656e 6420 546f 7020     <!-- end Top 
+0000ff50: 2d2d 3e0a 0a20 2020 2020 2020 2020 2020  -->..           
+0000ff60: 2020 2020 2020 2020 203c 212d 2d20 4d69           <!-- Mi
+0000ff70: 6464 6c65 2054 6f70 202d 2d3e 0a20 2020  ddle Top -->.   
+0000ff80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ff90: 207b 2520 6966 2033 5f6d 6964 5f74 6f70   {% if 3_mid_top
+0000ffa0: 5f61 206f 7220 335f 6d69 645f 746f 705f  _a or 3_mid_top_
+0000ffb0: 6220 6f72 2033 5f6d 6964 5f74 6f70 5f63  b or 3_mid_top_c
+0000ffc0: 2025 7d0a 2020 2020 2020 2020 2020 2020   %}.            
+0000ffd0: 2020 2020 2020 2020 3c64 6976 2063 6c61          <div cla
+0000ffe0: 7373 3d22 636f 6c2d 3132 223e 0a20 2020  ss="col-12">.   
+0000fff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010000: 2020 2020 203c 6469 7620 636c 6173 733d       <div class=
+00010010: 2272 6f77 223e 0a20 2020 2020 2020 2020  "row">.         
+00010020: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010030: 2020 207b 2520 6966 2033 5f6d 6964 5f74     {% if 3_mid_t
+00010040: 6f70 5f61 2061 6e64 2033 5f6d 6964 5f74  op_a and 3_mid_t
+00010050: 6f70 5f62 2061 6e64 2033 5f6d 6964 5f74  op_b and 3_mid_t
+00010060: 6f70 5f63 2025 7d0a 2020 2020 2020 2020  op_c %}.        
+00010070: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010080: 2020 2020 2020 2020 3c64 6976 2063 6c61          <div cla
+00010090: 7373 3d22 7b25 2062 6c6f 636b 2033 5f6d  ss="{% block 3_m
+000100a0: 6964 5f74 6f70 5f61 6263 5f61 2025 7d63  id_top_abc_a %}c
+000100b0: 6f6c 2d31 3220 636f 6c2d 6d64 2d34 7b25  ol-12 col-md-4{%
+000100c0: 2065 6e64 626c 6f63 6b20 257d 223e 7b7b   endblock %}">{{
+000100d0: 2033 5f6d 6964 5f74 6f70 5f61 207d 7d3c   3_mid_top_a }}<
+000100e0: 2f64 6976 3e0a 2020 2020 2020 2020 2020  /div>.          
+000100f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010100: 2020 2020 2020 3c64 6976 2063 6c61 7373        <div class
+00010110: 3d22 7b25 2062 6c6f 636b 2033 5f6d 6964  ="{% block 3_mid
+00010120: 5f74 6f70 5f61 6263 5f62 2025 7d63 6f6c  _top_abc_b %}col
+00010130: 2d31 3220 636f 6c2d 6d64 2d34 7b25 2065  -12 col-md-4{% e
+00010140: 6e64 626c 6f63 6b20 257d 223e 7b7b 2033  ndblock %}">{{ 3
+00010150: 5f6d 6964 5f74 6f70 5f62 207d 7d3c 2f64  _mid_top_b }}</d
+00010160: 6976 3e0a 2020 2020 2020 2020 2020 2020  iv>.            
+00010170: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010180: 2020 2020 3c64 6976 2063 6c61 7373 3d22      <div class="
+00010190: 7b25 2062 6c6f 636b 2033 5f6d 6964 5f74  {% block 3_mid_t
+000101a0: 6f70 5f61 6263 5f63 2025 7d63 6f6c 2d31  op_abc_c %}col-1
+000101b0: 3220 636f 6c2d 6d64 2d34 7b25 2065 6e64  2 col-md-4{% end
+000101c0: 626c 6f63 6b20 257d 223e 7b7b 2033 5f6d  block %}">{{ 3_m
+000101d0: 6964 5f74 6f70 5f63 207d 7d3c 2f64 6976  id_top_c }}</div
+000101e0: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
+000101f0: 2020 2020 2020 2020 2020 2020 2020 7b25                {%
+00010200: 2065 6c69 6620 335f 6d69 645f 746f 705f   elif 3_mid_top_
+00010210: 6120 616e 6420 335f 6d69 645f 746f 705f  a and 3_mid_top_
+00010220: 6220 257d 0a20 2020 2020 2020 2020 2020  b %}.           
 00010230: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010240: 2020 2020 2020 2020 7b25 2065 6e64 6966          {% endif
-00010250: 2025 7d0a 2020 2020 2020 2020 2020 2020   %}.            
-00010260: 2020 2020 2020 2020 2020 2020 3c2f 6469              </di
-00010270: 763e 0a20 2020 2020 2020 2020 2020 2020  v>.             
-00010280: 2020 2020 2020 203c 2f64 6976 3e0a 2020         </div>.  
-00010290: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000102a0: 2020 7b25 2065 6e64 6966 2025 7d0a 2020    {% endif %}.  
+00010240: 2020 2020 203c 6469 7620 636c 6173 733d       <div class=
+00010250: 227b 2520 626c 6f63 6b20 335f 6d69 645f  "{% block 3_mid_
+00010260: 746f 705f 6162 5f61 2025 7d63 6f6c 2d31  top_ab_a %}col-1
+00010270: 3220 636f 6c2d 6d64 2d38 7b25 2065 6e64  2 col-md-8{% end
+00010280: 626c 6f63 6b20 257d 223e 7b7b 2033 5f6d  block %}">{{ 3_m
+00010290: 6964 5f74 6f70 5f61 207d 7d3c 2f64 6976  id_top_a }}</div
+000102a0: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
 000102b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000102c0: 2020 3c21 2d2d 2065 6e64 204d 6964 646c    <!-- end Middl
-000102d0: 6520 546f 7020 2d2d 3e0a 0a20 2020 2020  e Top -->..     
-000102e0: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-000102f0: 212d 2d20 426c 6f63 6b73 2069 6e20 6365  !-- Blocks in ce
-00010300: 6e74 6572 2070 6f73 6974 696f 6e73 202d  nter positions -
-00010310: 2d3e 0a20 2020 2020 2020 2020 2020 2020  ->.             
-00010320: 2020 2020 2020 207b 2520 6966 2033 5f63         {% if 3_c
-00010330: 656e 7465 725f 746f 705f 6120 6f72 2033  enter_top_a or 3
-00010340: 5f63 656e 7465 725f 746f 705f 6220 6f72  _center_top_b or
-00010350: 2033 5f63 656e 7465 725f 746f 705f 6320   3_center_top_c 
-00010360: 6f72 2033 5f63 656e 7465 725f 6d69 645f  or 3_center_mid_
-00010370: 746f 705f 6120 6f72 2033 5f63 656e 7465  top_a or 3_cente
-00010380: 725f 6d69 645f 746f 705f 6220 6f72 2033  r_mid_top_b or 3
-00010390: 5f63 656e 7465 725f 6d69 645f 746f 705f  _center_mid_top_
-000103a0: 6320 6f72 2033 5f63 656e 7465 725f 636f  c or 3_center_co
-000103b0: 6e74 656e 7420 6f72 2033 5f63 656e 7465  ntent or 3_cente
-000103c0: 725f 6d69 645f 626f 7474 6f6d 5f61 206f  r_mid_bottom_a o
-000103d0: 7220 335f 6365 6e74 6572 5f6d 6964 5f62  r 3_center_mid_b
-000103e0: 6f74 746f 6d5f 6220 6f72 2033 5f63 656e  ottom_b or 3_cen
-000103f0: 7465 725f 6d69 645f 626f 7474 6f6d 5f63  ter_mid_bottom_c
-00010400: 206f 7220 335f 6365 6e74 6572 5f62 6f74   or 3_center_bot
-00010410: 746f 6d5f 6120 6f72 2033 5f63 656e 7465  tom_a or 3_cente
-00010420: 725f 626f 7474 6f6d 5f62 206f 7220 335f  r_bottom_b or 3_
-00010430: 6365 6e74 6572 5f62 6f74 746f 6d5f 6320  center_bottom_c 
-00010440: 257d 0a0a 2020 2020 2020 2020 2020 2020  %}..            
-00010450: 2020 2020 2020 2020 2020 2020 3c21 2d2d              <!--
-00010460: 2042 6c6f 636b 7320 696e 206c 6566 7420   Blocks in left 
-00010470: 636f 6c75 6d6e 202d 2d3e 0a20 2020 2020  column -->.     
-00010480: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010490: 2020 207b 2520 6966 2033 5f6c 6566 745f     {% if 3_left_
-000104a0: 6120 6f72 2033 5f6c 6566 745f 6220 257d  a or 3_left_b %}
-000104b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000104c0: 2020 2020 2020 2020 2020 2020 207b 2520               {% 
-000104d0: 6966 2033 5f6c 6566 745f 6120 616e 6420  if 3_left_a and 
-000104e0: 335f 6c65 6674 5f62 2025 7d0a 2020 2020  3_left_b %}.    
-000104f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010500: 2020 2020 2020 2020 3c64 6976 2063 6c61          <div cla
-00010510: 7373 3d22 7b25 2062 6c6f 636b 2033 5f6c  ss="{% block 3_l
-00010520: 6566 745f 6162 2025 7d63 6f6c 2d31 3220  eft_ab %}col-12 
-00010530: 636f 6c2d 6c67 2d34 206d 622d 3520 6d62  col-lg-4 mb-5 mb
-00010540: 2d6c 672d 307b 2520 656e 6462 6c6f 636b  -lg-0{% endblock
-00010550: 2025 7d22 3e0a 2020 2020 2020 2020 2020   %}">.          
-00010560: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010570: 2020 7b25 2065 6c69 6620 335f 6c65 6674    {% elif 3_left
-00010580: 5f61 2025 7d0a 2020 2020 2020 2020 2020  _a %}.          
-00010590: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000105a0: 2020 3c64 6976 2063 6c61 7373 3d22 7b25    <div class="{%
-000105b0: 2062 6c6f 636b 2033 5f6c 6566 745f 6120   block 3_left_a 
-000105c0: 257d 636f 6c2d 3132 2063 6f6c 2d6c 672d  %}col-12 col-lg-
-000105d0: 3320 6d62 2d35 206d 622d 6c67 2d30 7b25  3 mb-5 mb-lg-0{%
-000105e0: 2065 6e64 626c 6f63 6b20 257d 223e 0a20   endblock %}">. 
-000105f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010600: 2020 2020 2020 2020 2020 207b 2520 656c             {% el
-00010610: 7365 2025 7d0a 2020 2020 2020 2020 2020  se %}.          
-00010620: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010630: 2020 3c64 6976 2063 6c61 7373 3d22 7b25    <div class="{%
-00010640: 2062 6c6f 636b 2033 5f6c 6566 745f 6220   block 3_left_b 
-00010650: 257d 636f 6c2d 3132 2063 6f6c 2d6c 672d  %}col-12 col-lg-
-00010660: 3320 6d62 2d35 206d 622d 6c67 2d30 7b25  3 mb-5 mb-lg-0{%
-00010670: 2065 6e64 626c 6f63 6b20 257d 223e 0a20   endblock %}">. 
-00010680: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010690: 2020 2020 2020 2020 2020 207b 2520 656e             {% en
-000106a0: 6469 6620 257d 0a20 2020 2020 2020 2020  dif %}.         
+000102c0: 2020 3c64 6976 2063 6c61 7373 3d22 7b25    <div class="{%
+000102d0: 2062 6c6f 636b 2033 5f6d 6964 5f74 6f70   block 3_mid_top
+000102e0: 5f61 625f 6220 257d 636f 6c2d 3132 2063  _ab_b %}col-12 c
+000102f0: 6f6c 2d6d 642d 347b 2520 656e 6462 6c6f  ol-md-4{% endblo
+00010300: 636b 2025 7d22 3e7b 7b20 335f 6d69 645f  ck %}">{{ 3_mid_
+00010310: 746f 705f 6220 7d7d 3c2f 6469 763e 0a20  top_b }}</div>. 
+00010320: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010330: 2020 2020 2020 2020 2020 207b 2520 656c             {% el
+00010340: 6966 2033 5f6d 6964 5f74 6f70 5f61 2061  if 3_mid_top_a a
+00010350: 6e64 2033 5f6d 6964 5f74 6f70 5f63 2025  nd 3_mid_top_c %
+00010360: 7d0a 2020 2020 2020 2020 2020 2020 2020  }.              
+00010370: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010380: 2020 3c64 6976 2063 6c61 7373 3d22 7b25    <div class="{%
+00010390: 2062 6c6f 636b 2033 5f6d 6964 5f74 6f70   block 3_mid_top
+000103a0: 5f61 635f 6120 257d 636f 6c2d 3132 2063  _ac_a %}col-12 c
+000103b0: 6f6c 2d6d 642d 367b 2520 656e 6462 6c6f  ol-md-6{% endblo
+000103c0: 636b 2025 7d22 3e7b 7b20 335f 6d69 645f  ck %}">{{ 3_mid_
+000103d0: 746f 705f 6120 7d7d 3c2f 6469 763e 0a20  top_a }}</div>. 
+000103e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000103f0: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+00010400: 6469 7620 636c 6173 733d 227b 2520 626c  div class="{% bl
+00010410: 6f63 6b20 335f 6d69 645f 746f 705f 6163  ock 3_mid_top_ac
+00010420: 5f63 2025 7d63 6f6c 2d31 3220 636f 6c2d  _c %}col-12 col-
+00010430: 6d64 2d36 7b25 2065 6e64 626c 6f63 6b20  md-6{% endblock 
+00010440: 257d 223e 7b7b 2033 5f6d 6964 5f74 6f70  %}">{{ 3_mid_top
+00010450: 5f63 207d 7d3c 2f64 6976 3e0a 2020 2020  _c }}</div>.    
+00010460: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010470: 2020 2020 2020 2020 7b25 2065 6c69 6620          {% elif 
+00010480: 335f 6d69 645f 746f 705f 6220 616e 6420  3_mid_top_b and 
+00010490: 335f 6d69 645f 746f 705f 6320 257d 0a20  3_mid_top_c %}. 
+000104a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000104b0: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+000104c0: 6469 7620 636c 6173 733d 227b 2520 626c  div class="{% bl
+000104d0: 6f63 6b20 335f 6d69 645f 746f 705f 6263  ock 3_mid_top_bc
+000104e0: 5f62 2025 7d63 6f6c 2d31 3220 636f 6c2d  _b %}col-12 col-
+000104f0: 6d64 2d34 7b25 2065 6e64 626c 6f63 6b20  md-4{% endblock 
+00010500: 257d 223e 7b7b 2033 5f6d 6964 5f74 6f70  %}">{{ 3_mid_top
+00010510: 5f62 207d 7d3c 2f64 6976 3e0a 2020 2020  _b }}</div>.    
+00010520: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010530: 2020 2020 2020 2020 2020 2020 3c64 6976              <div
+00010540: 2063 6c61 7373 3d22 7b25 2062 6c6f 636b   class="{% block
+00010550: 2033 5f6d 6964 5f74 6f70 5f62 635f 6320   3_mid_top_bc_c 
+00010560: 257d 636f 6c2d 3132 2063 6f6c 2d6d 642d  %}col-12 col-md-
+00010570: 387b 2520 656e 6462 6c6f 636b 2025 7d22  8{% endblock %}"
+00010580: 3e7b 7b20 335f 6d69 645f 746f 705f 6320  >{{ 3_mid_top_c 
+00010590: 7d7d 3c2f 6469 763e 0a20 2020 2020 2020  }}</div>.       
+000105a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000105b0: 2020 2020 207b 2520 656c 7365 2025 7d0a       {% else %}.
+000105c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000105d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000105e0: 3c64 6976 2063 6c61 7373 3d22 636f 6c2d  <div class="col-
+000105f0: 3132 223e 7b7b 2033 5f6d 6964 5f74 6f70  12">{{ 3_mid_top
+00010600: 5f61 207d 7d7b 7b20 335f 6d69 645f 746f  _a }}{{ 3_mid_to
+00010610: 705f 6220 7d7d 7b7b 2033 5f6d 6964 5f74  p_b }}{{ 3_mid_t
+00010620: 6f70 5f63 207d 7d3c 2f64 6976 3e0a 2020  op_c }}</div>.  
+00010630: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010640: 2020 2020 2020 2020 2020 7b25 2065 6e64            {% end
+00010650: 6966 2025 7d0a 2020 2020 2020 2020 2020  if %}.          
+00010660: 2020 2020 2020 2020 2020 2020 2020 3c2f                </
+00010670: 6469 763e 0a20 2020 2020 2020 2020 2020  div>.           
+00010680: 2020 2020 2020 2020 203c 2f64 6976 3e0a           </div>.
+00010690: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000106a0: 2020 2020 7b25 2065 6e64 6966 2025 7d0a      {% endif %}.
 000106b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000106c0: 2020 2020 2020 203c 6469 7620 636c 6173         <div clas
-000106d0: 733d 2272 6f77 223e 0a20 2020 2020 2020  s="row">.       
+000106c0: 2020 2020 3c21 2d2d 2065 6e64 204d 6964      <!-- end Mid
+000106d0: 646c 6520 546f 7020 2d2d 3e0a 0a20 2020  dle Top -->..   
 000106e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000106f0: 2020 2020 2020 2020 2020 2020 207b 2520               {% 
-00010700: 6966 2033 5f6c 6566 745f 6120 616e 6420  if 3_left_a and 
-00010710: 335f 6c65 6674 5f62 2025 7d0a 2020 2020  3_left_b %}.    
-00010720: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010730: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010740: 3c64 6976 2063 6c61 7373 3d22 7b25 2062  <div class="{% b
-00010750: 6c6f 636b 2033 5f6c 6566 745f 6162 5f61  lock 3_left_ab_a
-00010760: 2025 7d63 6f6c 2d31 3220 636f 6c2d 6c67   %}col-12 col-lg
-00010770: 2d36 7b25 2065 6e64 626c 6f63 6b20 257d  -6{% endblock %}
-00010780: 223e 7b7b 2033 5f6c 6566 745f 6120 7d7d  ">{{ 3_left_a }}
-00010790: 3c2f 6469 763e 0a20 2020 2020 2020 2020  </div>.         
-000107a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000107b0: 2020 2020 2020 2020 2020 203c 6469 7620             <div 
-000107c0: 636c 6173 733d 227b 2520 626c 6f63 6b20  class="{% block 
-000107d0: 335f 6c65 6674 5f61 625f 6220 257d 636f  3_left_ab_b %}co
-000107e0: 6c2d 3132 2063 6f6c 2d6c 672d 367b 2520  l-12 col-lg-6{% 
-000107f0: 656e 6462 6c6f 636b 2025 7d22 3e7b 7b20  endblock %}">{{ 
-00010800: 335f 6c65 6674 5f62 207d 7d3c 2f64 6976  3_left_b }}</div
-00010810: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
-00010820: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010830: 2020 2020 2020 7b25 2065 6c69 6620 335f        {% elif 3_
-00010840: 6c65 6674 5f61 2025 7d0a 2020 2020 2020  left_a %}.      
-00010850: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010860: 2020 2020 2020 2020 2020 2020 2020 3c64                <d
-00010870: 6976 2063 6c61 7373 3d22 636f 6c2d 3132  iv class="col-12
-00010880: 223e 7b7b 2033 5f6c 6566 745f 6120 7d7d  ">{{ 3_left_a }}
-00010890: 3c2f 6469 763e 0a20 2020 2020 2020 2020  </div>.         
-000108a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000108b0: 2020 2020 2020 2020 2020 207b 2520 656c             {% el
-000108c0: 7365 2025 7d0a 2020 2020 2020 2020 2020  se %}.          
-000108d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000108e0: 2020 2020 2020 2020 2020 3c64 6976 2063            <div c
-000108f0: 6c61 7373 3d22 636f 6c2d 3132 223e 7b7b  lass="col-12">{{
-00010900: 2033 5f6c 6566 745f 6220 7d7d 3c2f 6469   3_left_b }}</di
-00010910: 763e 0a20 2020 2020 2020 2020 2020 2020  v>.             
-00010920: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010930: 2020 2020 2020 207b 2520 656e 6469 6620         {% endif 
-00010940: 257d 0a20 2020 2020 2020 2020 2020 2020  %}.             
-00010950: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010960: 2020 203c 2f64 6976 3e0a 2020 2020 2020     </div>.      
-00010970: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010980: 2020 2020 2020 3c2f 6469 763e 0a20 2020        </div>.   
+000106f0: 203c 212d 2d20 426c 6f63 6b73 2069 6e20   <!-- Blocks in 
+00010700: 6365 6e74 6572 2070 6f73 6974 696f 6e73  center positions
+00010710: 202d 2d3e 0a20 2020 2020 2020 2020 2020   -->.           
+00010720: 2020 2020 2020 2020 207b 2520 6966 2033           {% if 3
+00010730: 5f63 656e 7465 725f 746f 705f 6120 6f72  _center_top_a or
+00010740: 2033 5f63 656e 7465 725f 746f 705f 6220   3_center_top_b 
+00010750: 6f72 2033 5f63 656e 7465 725f 746f 705f  or 3_center_top_
+00010760: 6320 6f72 2033 5f63 656e 7465 725f 6d69  c or 3_center_mi
+00010770: 645f 746f 705f 6120 6f72 2033 5f63 656e  d_top_a or 3_cen
+00010780: 7465 725f 6d69 645f 746f 705f 6220 6f72  ter_mid_top_b or
+00010790: 2033 5f63 656e 7465 725f 6d69 645f 746f   3_center_mid_to
+000107a0: 705f 6320 6f72 2033 5f63 656e 7465 725f  p_c or 3_center_
+000107b0: 636f 6e74 656e 7420 6f72 2033 5f63 656e  content or 3_cen
+000107c0: 7465 725f 6d69 645f 626f 7474 6f6d 5f61  ter_mid_bottom_a
+000107d0: 206f 7220 335f 6365 6e74 6572 5f6d 6964   or 3_center_mid
+000107e0: 5f62 6f74 746f 6d5f 6220 6f72 2033 5f63  _bottom_b or 3_c
+000107f0: 656e 7465 725f 6d69 645f 626f 7474 6f6d  enter_mid_bottom
+00010800: 5f63 206f 7220 335f 6365 6e74 6572 5f62  _c or 3_center_b
+00010810: 6f74 746f 6d5f 6120 6f72 2033 5f63 656e  ottom_a or 3_cen
+00010820: 7465 725f 626f 7474 6f6d 5f62 206f 7220  ter_bottom_b or 
+00010830: 335f 6365 6e74 6572 5f62 6f74 746f 6d5f  3_center_bottom_
+00010840: 6320 257d 0a0a 2020 2020 2020 2020 2020  c %}..          
+00010850: 2020 2020 2020 2020 2020 2020 2020 3c21                <!
+00010860: 2d2d 2042 6c6f 636b 7320 696e 206c 6566  -- Blocks in lef
+00010870: 7420 636f 6c75 6d6e 202d 2d3e 0a20 2020  t column -->.   
+00010880: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010890: 2020 2020 207b 2520 6966 2033 5f6c 6566       {% if 3_lef
+000108a0: 745f 6120 6f72 2033 5f6c 6566 745f 6220  t_a or 3_left_b 
+000108b0: 257d 0a20 2020 2020 2020 2020 2020 2020  %}.             
+000108c0: 2020 2020 2020 2020 2020 2020 2020 207b                 {
+000108d0: 2520 6966 2033 5f6c 6566 745f 6120 616e  % if 3_left_a an
+000108e0: 6420 335f 6c65 6674 5f62 2025 7d0a 2020  d 3_left_b %}.  
+000108f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010900: 2020 2020 2020 2020 2020 3c64 6976 2063            <div c
+00010910: 6c61 7373 3d22 7b25 2062 6c6f 636b 2033  lass="{% block 3
+00010920: 5f6c 6566 745f 6162 2025 7d63 6f6c 2d31  _left_ab %}col-1
+00010930: 3220 636f 6c2d 6c67 2d34 206d 622d 3520  2 col-lg-4 mb-5 
+00010940: 6d62 2d6c 672d 307b 2520 656e 6462 6c6f  mb-lg-0{% endblo
+00010950: 636b 2025 7d22 3e0a 2020 2020 2020 2020  ck %}">.        
+00010960: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010970: 2020 2020 7b25 2065 6c69 6620 335f 6c65      {% elif 3_le
+00010980: 6674 5f61 2025 7d0a 2020 2020 2020 2020  ft_a %}.        
 00010990: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000109a0: 2020 2020 207b 2520 656e 6469 6620 257d       {% endif %}
-000109b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000109c0: 2020 2020 2020 2020 203c 212d 2d20 656e           <!-- en
-000109d0: 6420 426c 6f63 6b73 2069 6e20 6c65 6674  d Blocks in left
-000109e0: 2063 6f6c 756d 6e20 2d2d 3e0a 0a20 2020   column -->..   
-000109f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010a00: 2020 2020 203c 212d 2d20 426c 6f63 6b73       <!-- Blocks
-00010a10: 2069 6e20 4365 6e74 6572 2063 6f6c 756d   in Center colum
-00010a20: 6e20 2874 616b 6573 2061 7661 696c 6162  n (takes availab
-00010a30: 6c65 2073 7061 6365 2920 2d2d 3e0a 2020  le space) -->.  
-00010a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010a50: 2020 2020 2020 7b25 2069 6620 335f 6c65        {% if 3_le
-00010a60: 6674 5f61 2061 6e64 2033 5f6c 6566 745f  ft_a and 3_left_
-00010a70: 6220 616e 6420 335f 7269 6768 745f 6120  b and 3_right_a 
-00010a80: 616e 6420 335f 7269 6768 745f 6220 257d  and 3_right_b %}
-00010a90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00010aa0: 2020 2020 2020 2020 203c 6469 7620 636c           <div cl
-00010ab0: 6173 733d 227b 2520 626c 6f63 6b20 335f  ass="{% block 3_
-00010ac0: 6365 6e74 6572 5f6c 6566 745f 6162 5f72  center_left_ab_r
-00010ad0: 6967 6874 5f61 6220 257d 636f 6c2d 3132  ight_ab %}col-12
-00010ae0: 2063 6f6c 2d6c 672d 347b 2520 656e 6462   col-lg-4{% endb
-00010af0: 6c6f 636b 2025 7d22 3e0a 2020 2020 2020  lock %}">.      
-00010b00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010b10: 2020 7b25 2065 6c69 6620 335f 6c65 6674    {% elif 3_left
-00010b20: 5f61 2061 6e64 2033 5f6c 6566 745f 6220  _a and 3_left_b 
-00010b30: 616e 6420 335f 7269 6768 745f 6120 257d  and 3_right_a %}
-00010b40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00010b50: 2020 2020 2020 2020 203c 6469 7620 636c           <div cl
-00010b60: 6173 733d 227b 2520 626c 6f63 6b20 335f  ass="{% block 3_
-00010b70: 6365 6e74 6572 5f6c 6566 745f 6162 5f72  center_left_ab_r
-00010b80: 6967 6874 5f61 2025 7d63 6f6c 2d31 3220  ight_a %}col-12 
-00010b90: 636f 6c2d 6c67 2d35 7b25 2065 6e64 626c  col-lg-5{% endbl
-00010ba0: 6f63 6b20 257d 223e 0a20 2020 2020 2020  ock %}">.       
-00010bb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010bc0: 207b 2520 656c 6966 2033 5f6c 6566 745f   {% elif 3_left_
-00010bd0: 6120 616e 6420 335f 6c65 6674 5f62 2061  a and 3_left_b a
-00010be0: 6e64 2033 5f72 6967 6874 5f62 2025 7d0a  nd 3_right_b %}.
-00010bf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010c00: 2020 2020 2020 2020 3c64 6976 2063 6c61          <div cla
-00010c10: 7373 3d22 7b25 2062 6c6f 636b 2033 5f63  ss="{% block 3_c
-00010c20: 656e 7465 725f 6c65 6674 5f61 625f 7269  enter_left_ab_ri
-00010c30: 6768 745f 6220 257d 636f 6c2d 3132 2063  ght_b %}col-12 c
-00010c40: 6f6c 2d6c 672d 347b 2520 656e 6462 6c6f  ol-lg-4{% endblo
-00010c50: 636b 2025 7d22 3e0a 2020 2020 2020 2020  ck %}">.        
+000109a0: 2020 2020 3c64 6976 2063 6c61 7373 3d22      <div class="
+000109b0: 7b25 2062 6c6f 636b 2033 5f6c 6566 745f  {% block 3_left_
+000109c0: 6120 257d 636f 6c2d 3132 2063 6f6c 2d6c  a %}col-12 col-l
+000109d0: 672d 3320 6d62 2d35 206d 622d 6c67 2d30  g-3 mb-5 mb-lg-0
+000109e0: 7b25 2065 6e64 626c 6f63 6b20 257d 223e  {% endblock %}">
+000109f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00010a00: 2020 2020 2020 2020 2020 2020 207b 2520               {% 
+00010a10: 656c 7365 2025 7d0a 2020 2020 2020 2020  else %}.        
+00010a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010a30: 2020 2020 3c64 6976 2063 6c61 7373 3d22      <div class="
+00010a40: 7b25 2062 6c6f 636b 2033 5f6c 6566 745f  {% block 3_left_
+00010a50: 6220 257d 636f 6c2d 3132 2063 6f6c 2d6c  b %}col-12 col-l
+00010a60: 672d 3320 6d62 2d35 206d 622d 6c67 2d30  g-3 mb-5 mb-lg-0
+00010a70: 7b25 2065 6e64 626c 6f63 6b20 257d 223e  {% endblock %}">
+00010a80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00010a90: 2020 2020 2020 2020 2020 2020 207b 2520               {% 
+00010aa0: 656e 6469 6620 257d 0a20 2020 2020 2020  endif %}.       
+00010ab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010ac0: 2020 2020 2020 2020 203c 6469 7620 636c           <div cl
+00010ad0: 6173 733d 2272 6f77 223e 0a20 2020 2020  ass="row">.     
+00010ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010af0: 2020 2020 2020 2020 2020 2020 2020 207b                 {
+00010b00: 2520 6966 2033 5f6c 6566 745f 6120 616e  % if 3_left_a an
+00010b10: 6420 335f 6c65 6674 5f62 2025 7d0a 2020  d 3_left_b %}.  
+00010b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010b30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010b40: 2020 3c64 6976 2063 6c61 7373 3d22 7b25    <div class="{%
+00010b50: 2062 6c6f 636b 2033 5f6c 6566 745f 6162   block 3_left_ab
+00010b60: 5f61 2025 7d63 6f6c 2d31 3220 636f 6c2d  _a %}col-12 col-
+00010b70: 6c67 2d36 7b25 2065 6e64 626c 6f63 6b20  lg-6{% endblock 
+00010b80: 257d 223e 7b7b 2033 5f6c 6566 745f 6120  %}">{{ 3_left_a 
+00010b90: 7d7d 3c2f 6469 763e 0a20 2020 2020 2020  }}</div>.       
+00010ba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010bb0: 2020 2020 2020 2020 2020 2020 203c 6469               <di
+00010bc0: 7620 636c 6173 733d 227b 2520 626c 6f63  v class="{% bloc
+00010bd0: 6b20 335f 6c65 6674 5f61 625f 6220 257d  k 3_left_ab_b %}
+00010be0: 636f 6c2d 3132 2063 6f6c 2d6c 672d 367b  col-12 col-lg-6{
+00010bf0: 2520 656e 6462 6c6f 636b 2025 7d22 3e7b  % endblock %}">{
+00010c00: 7b20 335f 6c65 6674 5f62 207d 7d3c 2f64  { 3_left_b }}</d
+00010c10: 6976 3e0a 2020 2020 2020 2020 2020 2020  iv>.            
+00010c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010c30: 2020 2020 2020 2020 7b25 2065 6c69 6620          {% elif 
+00010c40: 335f 6c65 6674 5f61 2025 7d0a 2020 2020  3_left_a %}.    
+00010c50: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00010c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010c70: 7b25 2065 6c69 6620 335f 6c65 6674 5f61  {% elif 3_left_a
-00010c80: 2061 6e64 2033 5f72 6967 6874 5f61 2061   and 3_right_a a
-00010c90: 6e64 2033 5f72 6967 6874 5f62 2025 7d0a  nd 3_right_b %}.
+00010c70: 3c64 6976 2063 6c61 7373 3d22 636f 6c2d  <div class="col-
+00010c80: 3132 223e 7b7b 2033 5f6c 6566 745f 6120  12">{{ 3_left_a 
+00010c90: 7d7d 3c2f 6469 763e 0a20 2020 2020 2020  }}</div>.       
 00010ca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010cb0: 2020 2020 2020 2020 3c64 6976 2063 6c61          <div cla
-00010cc0: 7373 3d22 7b25 2062 6c6f 636b 2033 5f63  ss="{% block 3_c
-00010cd0: 656e 7465 725f 6c65 6674 5f61 5f72 6967  enter_left_a_rig
-00010ce0: 6874 5f61 6220 257d 636f 6c2d 3132 2063  ht_ab %}col-12 c
-00010cf0: 6f6c 2d6c 672d 357b 2520 656e 6462 6c6f  ol-lg-5{% endblo
-00010d00: 636b 2025 7d22 3e0a 2020 2020 2020 2020  ck %}">.        
-00010d10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010d20: 7b25 2065 6c69 6620 335f 6c65 6674 5f61  {% elif 3_left_a
-00010d30: 2061 6e64 2033 5f72 6967 6874 5f61 2025   and 3_right_a %
-00010d40: 7d0a 2020 2020 2020 2020 2020 2020 2020  }.              
-00010d50: 2020 2020 2020 2020 2020 3c64 6976 2063            <div c
-00010d60: 6c61 7373 3d22 7b25 2062 6c6f 636b 2033  lass="{% block 3
-00010d70: 5f63 656e 7465 725f 6c65 6674 5f61 5f72  _center_left_a_r
-00010d80: 6967 6874 5f61 2025 7d63 6f6c 2d31 3220  ight_a %}col-12 
-00010d90: 636f 6c2d 6c67 2d36 7b25 2065 6e64 626c  col-lg-6{% endbl
-00010da0: 6f63 6b20 257d 223e 0a20 2020 2020 2020  ock %}">.       
-00010db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010dc0: 207b 2520 656c 6966 2033 5f6c 6566 745f   {% elif 3_left_
-00010dd0: 6120 616e 6420 335f 7269 6768 745f 6220  a and 3_right_b 
-00010de0: 257d 0a20 2020 2020 2020 2020 2020 2020  %}.             
-00010df0: 2020 2020 2020 2020 2020 203c 6469 7620             <div 
-00010e00: 636c 6173 733d 227b 2520 626c 6f63 6b20  class="{% block 
-00010e10: 335f 6365 6e74 6572 5f6c 6566 745f 615f  3_center_left_a_
-00010e20: 7269 6768 745f 6220 257d 636f 6c2d 3132  right_b %}col-12
-00010e30: 2063 6f6c 2d6c 672d 357b 2520 656e 6462   col-lg-5{% endb
-00010e40: 6c6f 636b 2025 7d22 3e0a 2020 2020 2020  lock %}">.      
-00010e50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010e60: 2020 7b25 2065 6c69 6620 335f 6c65 6674    {% elif 3_left
-00010e70: 5f62 2061 6e64 2033 5f72 6967 6874 5f61  _b and 3_right_a
-00010e80: 2061 6e64 2033 5f72 6967 6874 5f62 2025   and 3_right_b %
-00010e90: 7d0a 2020 2020 2020 2020 2020 2020 2020  }.              
-00010ea0: 2020 2020 2020 2020 2020 3c64 6976 2063            <div c
-00010eb0: 6c61 7373 3d22 7b25 2062 6c6f 636b 2033  lass="{% block 3
-00010ec0: 5f63 656e 7465 725f 6c65 6674 5f62 5f72  _center_left_b_r
-00010ed0: 6967 6874 5f61 6220 257d 636f 6c2d 3132  ight_ab %}col-12
-00010ee0: 2063 6f6c 2d6c 672d 3420 6f66 6673 6574   col-lg-4 offset
-00010ef0: 2d6c 672d 317b 2520 656e 6462 6c6f 636b  -lg-1{% endblock
-00010f00: 2025 7d22 3e0a 2020 2020 2020 2020 2020   %}">.          
-00010f10: 2020 2020 2020 2020 2020 2020 2020 7b25                {%
-00010f20: 2065 6c69 6620 335f 6c65 6674 5f62 2061   elif 3_left_b a
-00010f30: 6e64 2033 5f72 6967 6874 5f61 2025 7d0a  nd 3_right_a %}.
-00010f40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010f50: 2020 2020 2020 2020 3c64 6976 2063 6c61          <div cla
-00010f60: 7373 3d22 7b25 2062 6c6f 636b 2033 5f63  ss="{% block 3_c
-00010f70: 656e 7465 725f 6c65 6674 5f62 5f72 6967  enter_left_b_rig
-00010f80: 6874 5f61 2025 7d63 6f6c 2d31 3220 636f  ht_a %}col-12 co
-00010f90: 6c2d 6c67 2d35 206f 6666 7365 742d 6c67  l-lg-5 offset-lg
-00010fa0: 2d31 7b25 2065 6e64 626c 6f63 6b20 257d  -1{% endblock %}
-00010fb0: 223e 0a20 2020 2020 2020 2020 2020 2020  ">.             
-00010fc0: 2020 2020 2020 2020 2020 207b 2520 656c             {% el
-00010fd0: 6966 2033 5f6c 6566 745f 6220 616e 6420  if 3_left_b and 
-00010fe0: 335f 7269 6768 745f 6220 257d 0a20 2020  3_right_b %}.   
-00010ff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011000: 2020 2020 203c 6469 7620 636c 6173 733d       <div class=
-00011010: 227b 2520 626c 6f63 6b20 335f 6365 6e74  "{% block 3_cent
-00011020: 6572 5f6c 6566 745f 625f 7269 6768 745f  er_left_b_right_
-00011030: 6220 257d 636f 6c2d 3132 2063 6f6c 2d6c  b %}col-12 col-l
-00011040: 672d 3420 6f66 6673 6574 2d6c 672d 317b  g-4 offset-lg-1{
-00011050: 2520 656e 6462 6c6f 636b 2025 7d22 3e0a  % endblock %}">.
+00010cb0: 2020 2020 2020 2020 2020 2020 207b 2520               {% 
+00010cc0: 656c 7365 2025 7d0a 2020 2020 2020 2020  else %}.        
+00010cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010ce0: 2020 2020 2020 2020 2020 2020 3c64 6976              <div
+00010cf0: 2063 6c61 7373 3d22 636f 6c2d 3132 223e   class="col-12">
+00010d00: 7b7b 2033 5f6c 6566 745f 6220 7d7d 3c2f  {{ 3_left_b }}</
+00010d10: 6469 763e 0a20 2020 2020 2020 2020 2020  div>.           
+00010d20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010d30: 2020 2020 2020 2020 207b 2520 656e 6469           {% endi
+00010d40: 6620 257d 0a20 2020 2020 2020 2020 2020  f %}.           
+00010d50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010d60: 2020 2020 203c 2f64 6976 3e0a 2020 2020       </div>.    
+00010d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010d80: 2020 2020 2020 2020 3c2f 6469 763e 0a20          </div>. 
+00010d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010da0: 2020 2020 2020 207b 2520 656e 6469 6620         {% endif 
+00010db0: 257d 0a20 2020 2020 2020 2020 2020 2020  %}.             
+00010dc0: 2020 2020 2020 2020 2020 203c 212d 2d20             <!-- 
+00010dd0: 656e 6420 426c 6f63 6b73 2069 6e20 6c65  end Blocks in le
+00010de0: 6674 2063 6f6c 756d 6e20 2d2d 3e0a 0a20  ft column -->.. 
+00010df0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010e00: 2020 2020 2020 203c 212d 2d20 426c 6f63         <!-- Bloc
+00010e10: 6b73 2069 6e20 4365 6e74 6572 2063 6f6c  ks in Center col
+00010e20: 756d 6e20 2874 616b 6573 2061 7661 696c  umn (takes avail
+00010e30: 6162 6c65 2073 7061 6365 2920 2d2d 3e0a  able space) -->.
+00010e40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010e50: 2020 2020 2020 2020 7b25 2069 6620 335f          {% if 3_
+00010e60: 6c65 6674 5f61 2061 6e64 2033 5f6c 6566  left_a and 3_lef
+00010e70: 745f 6220 616e 6420 335f 7269 6768 745f  t_b and 3_right_
+00010e80: 6120 616e 6420 335f 7269 6768 745f 6220  a and 3_right_b 
+00010e90: 257d 0a20 2020 2020 2020 2020 2020 2020  %}.             
+00010ea0: 2020 2020 2020 2020 2020 203c 6469 7620             <div 
+00010eb0: 636c 6173 733d 227b 2520 626c 6f63 6b20  class="{% block 
+00010ec0: 335f 6365 6e74 6572 5f6c 6566 745f 6162  3_center_left_ab
+00010ed0: 5f72 6967 6874 5f61 6220 257d 636f 6c2d  _right_ab %}col-
+00010ee0: 3132 2063 6f6c 2d6c 672d 347b 2520 656e  12 col-lg-4{% en
+00010ef0: 6462 6c6f 636b 2025 7d22 3e0a 2020 2020  dblock %}">.    
+00010f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010f10: 2020 2020 7b25 2065 6c69 6620 335f 6c65      {% elif 3_le
+00010f20: 6674 5f61 2061 6e64 2033 5f6c 6566 745f  ft_a and 3_left_
+00010f30: 6220 616e 6420 335f 7269 6768 745f 6120  b and 3_right_a 
+00010f40: 257d 0a20 2020 2020 2020 2020 2020 2020  %}.             
+00010f50: 2020 2020 2020 2020 2020 203c 6469 7620             <div 
+00010f60: 636c 6173 733d 227b 2520 626c 6f63 6b20  class="{% block 
+00010f70: 335f 6365 6e74 6572 5f6c 6566 745f 6162  3_center_left_ab
+00010f80: 5f72 6967 6874 5f61 2025 7d63 6f6c 2d31  _right_a %}col-1
+00010f90: 3220 636f 6c2d 6c67 2d35 7b25 2065 6e64  2 col-lg-5{% end
+00010fa0: 626c 6f63 6b20 257d 223e 0a20 2020 2020  block %}">.     
+00010fb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010fc0: 2020 207b 2520 656c 6966 2033 5f6c 6566     {% elif 3_lef
+00010fd0: 745f 6120 616e 6420 335f 6c65 6674 5f62  t_a and 3_left_b
+00010fe0: 2061 6e64 2033 5f72 6967 6874 5f62 2025   and 3_right_b %
+00010ff0: 7d0a 2020 2020 2020 2020 2020 2020 2020  }.              
+00011000: 2020 2020 2020 2020 2020 3c64 6976 2063            <div c
+00011010: 6c61 7373 3d22 7b25 2062 6c6f 636b 2033  lass="{% block 3
+00011020: 5f63 656e 7465 725f 6c65 6674 5f61 625f  _center_left_ab_
+00011030: 7269 6768 745f 6220 257d 636f 6c2d 3132  right_b %}col-12
+00011040: 2063 6f6c 2d6c 672d 347b 2520 656e 6462   col-lg-4{% endb
+00011050: 6c6f 636b 2025 7d22 3e0a 2020 2020 2020  lock %}">.      
 00011060: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011070: 2020 2020 2020 2020 7b25 2065 6c69 6620          {% elif 
-00011080: 335f 6c65 6674 5f61 2061 6e64 2033 5f6c  3_left_a and 3_l
-00011090: 6566 745f 6220 257d 0a20 2020 2020 2020  eft_b %}.       
-000110a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000110b0: 203c 6469 7620 636c 6173 733d 227b 2520   <div class="{% 
-000110c0: 626c 6f63 6b20 335f 6365 6e74 6572 5f6c  block 3_center_l
-000110d0: 6566 745f 6162 2025 7d63 6f6c 2d31 3220  eft_ab %}col-12 
-000110e0: 636f 6c2d 6c67 2d38 7b25 2065 6e64 626c  col-lg-8{% endbl
-000110f0: 6f63 6b20 257d 223e 0a20 2020 2020 2020  ock %}">.       
-00011100: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011110: 207b 2520 656c 6966 2033 5f6c 6566 745f   {% elif 3_left_
-00011120: 6120 257d 0a20 2020 2020 2020 2020 2020  a %}.           
-00011130: 2020 2020 2020 2020 2020 2020 203c 6469               <di
-00011140: 7620 636c 6173 733d 227b 2520 626c 6f63  v class="{% bloc
-00011150: 6b20 335f 6365 6e74 6572 5f6c 6566 745f  k 3_center_left_
-00011160: 6120 257d 636f 6c2d 3132 2063 6f6c 2d6c  a %}col-12 col-l
-00011170: 672d 397b 2520 656e 6462 6c6f 636b 2025  g-9{% endblock %
-00011180: 7d22 3e0a 2020 2020 2020 2020 2020 2020  }">.            
-00011190: 2020 2020 2020 2020 2020 2020 7b25 2065              {% e
-000111a0: 6c69 6620 335f 6c65 6674 5f62 2025 7d0a  lif 3_left_b %}.
+00011070: 2020 7b25 2065 6c69 6620 335f 6c65 6674    {% elif 3_left
+00011080: 5f61 2061 6e64 2033 5f72 6967 6874 5f61  _a and 3_right_a
+00011090: 2061 6e64 2033 5f72 6967 6874 5f62 2025   and 3_right_b %
+000110a0: 7d0a 2020 2020 2020 2020 2020 2020 2020  }.              
+000110b0: 2020 2020 2020 2020 2020 3c64 6976 2063            <div c
+000110c0: 6c61 7373 3d22 7b25 2062 6c6f 636b 2033  lass="{% block 3
+000110d0: 5f63 656e 7465 725f 6c65 6674 5f61 5f72  _center_left_a_r
+000110e0: 6967 6874 5f61 6220 257d 636f 6c2d 3132  ight_ab %}col-12
+000110f0: 2063 6f6c 2d6c 672d 357b 2520 656e 6462   col-lg-5{% endb
+00011100: 6c6f 636b 2025 7d22 3e0a 2020 2020 2020  lock %}">.      
+00011110: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011120: 2020 7b25 2065 6c69 6620 335f 6c65 6674    {% elif 3_left
+00011130: 5f61 2061 6e64 2033 5f72 6967 6874 5f61  _a and 3_right_a
+00011140: 2025 7d0a 2020 2020 2020 2020 2020 2020   %}.            
+00011150: 2020 2020 2020 2020 2020 2020 3c64 6976              <div
+00011160: 2063 6c61 7373 3d22 7b25 2062 6c6f 636b   class="{% block
+00011170: 2033 5f63 656e 7465 725f 6c65 6674 5f61   3_center_left_a
+00011180: 5f72 6967 6874 5f61 2025 7d63 6f6c 2d31  _right_a %}col-1
+00011190: 3220 636f 6c2d 6c67 2d36 7b25 2065 6e64  2 col-lg-6{% end
+000111a0: 626c 6f63 6b20 257d 223e 0a20 2020 2020  block %}">.     
 000111b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000111c0: 2020 2020 2020 2020 3c64 6976 2063 6c61          <div cla
-000111d0: 7373 3d22 7b25 2062 6c6f 636b 2033 5f63  ss="{% block 3_c
-000111e0: 656e 7465 725f 6c65 6674 5f62 2025 7d63  enter_left_b %}c
-000111f0: 6f6c 2d31 3220 636f 6c2d 6c67 2d38 206f  ol-12 col-lg-8 o
-00011200: 6666 7365 742d 6c67 2d31 7b25 2065 6e64  ffset-lg-1{% end
-00011210: 626c 6f63 6b20 257d 223e 0a20 2020 2020  block %}">.     
-00011220: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011230: 2020 207b 2520 656c 6966 2033 5f72 6967     {% elif 3_rig
-00011240: 6874 5f61 2061 6e64 2033 5f72 6967 6874  ht_a and 3_right
-00011250: 5f62 2025 7d0a 2020 2020 2020 2020 2020  _b %}.          
-00011260: 2020 2020 2020 2020 2020 2020 2020 3c64                <d
-00011270: 6976 2063 6c61 7373 3d22 7b25 2062 6c6f  iv class="{% blo
-00011280: 636b 2033 5f63 656e 7465 725f 7269 6768  ck 3_center_righ
-00011290: 745f 6162 2025 7d63 6f6c 2d31 3220 636f  t_ab %}col-12 co
-000112a0: 6c2d 6c67 2d38 7b25 2065 6e64 626c 6f63  l-lg-8{% endbloc
-000112b0: 6b20 257d 223e 0a20 2020 2020 2020 2020  k %}">.         
-000112c0: 2020 2020 2020 2020 2020 2020 2020 207b                 {
-000112d0: 2520 656c 6966 2033 5f72 6967 6874 5f61  % elif 3_right_a
-000112e0: 2025 7d0a 2020 2020 2020 2020 2020 2020   %}.            
-000112f0: 2020 2020 2020 2020 2020 2020 3c64 6976              <div
-00011300: 2063 6c61 7373 3d22 7b25 2062 6c6f 636b   class="{% block
-00011310: 2033 5f63 656e 7465 725f 7269 6768 745f   3_center_right_
-00011320: 6120 257d 636f 6c2d 3132 2063 6f6c 2d6c  a %}col-12 col-l
-00011330: 672d 397b 2520 656e 6462 6c6f 636b 2025  g-9{% endblock %
-00011340: 7d22 3e0a 2020 2020 2020 2020 2020 2020  }">.            
-00011350: 2020 2020 2020 2020 2020 2020 7b25 2065              {% e
-00011360: 6c69 6620 335f 7269 6768 745f 6220 257d  lif 3_right_b %}
-00011370: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00011380: 2020 2020 2020 2020 203c 6469 7620 636c           <div cl
-00011390: 6173 733d 227b 2520 626c 6f63 6b20 335f  ass="{% block 3_
-000113a0: 6365 6e74 6572 5f72 6967 6874 5f62 2025  center_right_b %
-000113b0: 7d63 6f6c 2d31 3220 636f 6c2d 6c67 2d38  }col-12 col-lg-8
-000113c0: 7b25 2065 6e64 626c 6f63 6b20 257d 223e  {% endblock %}">
-000113d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000113e0: 2020 2020 2020 2020 207b 2520 656c 7365           {% else
-000113f0: 2025 7d0a 2020 2020 2020 2020 2020 2020   %}.            
-00011400: 2020 2020 2020 2020 2020 2020 3c64 6976              <div
-00011410: 2063 6c61 7373 3d22 7b25 2062 6c6f 636b   class="{% block
-00011420: 2033 5f63 656e 7465 7220 257d 636f 6c2d   3_center %}col-
-00011430: 3132 7b25 2065 6e64 626c 6f63 6b20 257d  12{% endblock %}
-00011440: 223e 0a20 2020 2020 2020 2020 2020 2020  ">.             
-00011450: 2020 2020 2020 2020 2020 207b 2520 656e             {% en
-00011460: 6469 6620 257d 0a20 2020 2020 2020 2020  dif %}.         
-00011470: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-00011480: 212d 2d20 456e 6420 426c 6f63 6b73 2069  !-- End Blocks i
-00011490: 6e20 4365 6e74 6572 2063 6f6c 756d 6e20  n Center column 
-000114a0: 2874 616b 6573 2061 7661 696c 6162 6c65  (takes available
-000114b0: 2073 7061 6365 2920 2d2d 3e0a 0a20 2020   space) -->..   
-000114c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000114d0: 2020 2020 2020 2020 203c 212d 2d20 4365           <!-- Ce
-000114e0: 6e74 6572 2074 6f70 202d 2d3e 0a20 2020  nter top -->.   
-000114f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011500: 2020 2020 2020 2020 207b 2520 6966 2033           {% if 3
-00011510: 5f63 656e 7465 725f 746f 705f 6120 6f72  _center_top_a or
-00011520: 2033 5f63 656e 7465 725f 746f 705f 6220   3_center_top_b 
-00011530: 6f72 2033 5f63 656e 7465 725f 746f 705f  or 3_center_top_
-00011540: 6320 257d 0a20 2020 2020 2020 2020 2020  c %}.           
-00011550: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011560: 203c 6469 7620 636c 6173 733d 2272 6f77   <div class="row
-00011570: 223e 0a20 2020 2020 2020 2020 2020 2020  ">.             
-00011580: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011590: 2020 207b 2520 6966 2033 5f63 656e 7465     {% if 3_cente
-000115a0: 725f 746f 705f 6120 616e 6420 335f 6365  r_top_a and 3_ce
-000115b0: 6e74 6572 5f74 6f70 5f62 2061 6e64 2033  nter_top_b and 3
-000115c0: 5f63 656e 7465 725f 746f 705f 6320 257d  _center_top_c %}
-000115d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000115e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000115f0: 2020 2020 203c 6469 7620 636c 6173 733d       <div class=
-00011600: 227b 2520 626c 6f63 6b20 335f 6365 6e74  "{% block 3_cent
-00011610: 6572 5f74 6f70 5f61 6263 5f61 2025 7d63  er_top_abc_a %}c
-00011620: 6f6c 2d31 3220 636f 6c2d 6d64 2d34 7b25  ol-12 col-md-4{%
-00011630: 2065 6e64 626c 6f63 6b20 257d 223e 7b7b   endblock %}">{{
-00011640: 2033 5f63 656e 7465 725f 746f 705f 6120   3_center_top_a 
-00011650: 7d7d 3c2f 6469 763e 0a20 2020 2020 2020  }}</div>.       
+000111c0: 2020 207b 2520 656c 6966 2033 5f6c 6566     {% elif 3_lef
+000111d0: 745f 6120 616e 6420 335f 7269 6768 745f  t_a and 3_right_
+000111e0: 6220 257d 0a20 2020 2020 2020 2020 2020  b %}.           
+000111f0: 2020 2020 2020 2020 2020 2020 203c 6469               <di
+00011200: 7620 636c 6173 733d 227b 2520 626c 6f63  v class="{% bloc
+00011210: 6b20 335f 6365 6e74 6572 5f6c 6566 745f  k 3_center_left_
+00011220: 615f 7269 6768 745f 6220 257d 636f 6c2d  a_right_b %}col-
+00011230: 3132 2063 6f6c 2d6c 672d 357b 2520 656e  12 col-lg-5{% en
+00011240: 6462 6c6f 636b 2025 7d22 3e0a 2020 2020  dblock %}">.    
+00011250: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011260: 2020 2020 7b25 2065 6c69 6620 335f 6c65      {% elif 3_le
+00011270: 6674 5f62 2061 6e64 2033 5f72 6967 6874  ft_b and 3_right
+00011280: 5f61 2061 6e64 2033 5f72 6967 6874 5f62  _a and 3_right_b
+00011290: 2025 7d0a 2020 2020 2020 2020 2020 2020   %}.            
+000112a0: 2020 2020 2020 2020 2020 2020 3c64 6976              <div
+000112b0: 2063 6c61 7373 3d22 7b25 2062 6c6f 636b   class="{% block
+000112c0: 2033 5f63 656e 7465 725f 6c65 6674 5f62   3_center_left_b
+000112d0: 5f72 6967 6874 5f61 6220 257d 636f 6c2d  _right_ab %}col-
+000112e0: 3132 2063 6f6c 2d6c 672d 3420 6f66 6673  12 col-lg-4 offs
+000112f0: 6574 2d6c 672d 317b 2520 656e 6462 6c6f  et-lg-1{% endblo
+00011300: 636b 2025 7d22 3e0a 2020 2020 2020 2020  ck %}">.        
+00011310: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011320: 7b25 2065 6c69 6620 335f 6c65 6674 5f62  {% elif 3_left_b
+00011330: 2061 6e64 2033 5f72 6967 6874 5f61 2025   and 3_right_a %
+00011340: 7d0a 2020 2020 2020 2020 2020 2020 2020  }.              
+00011350: 2020 2020 2020 2020 2020 3c64 6976 2063            <div c
+00011360: 6c61 7373 3d22 7b25 2062 6c6f 636b 2033  lass="{% block 3
+00011370: 5f63 656e 7465 725f 6c65 6674 5f62 5f72  _center_left_b_r
+00011380: 6967 6874 5f61 2025 7d63 6f6c 2d31 3220  ight_a %}col-12 
+00011390: 636f 6c2d 6c67 2d35 206f 6666 7365 742d  col-lg-5 offset-
+000113a0: 6c67 2d31 7b25 2065 6e64 626c 6f63 6b20  lg-1{% endblock 
+000113b0: 257d 223e 0a20 2020 2020 2020 2020 2020  %}">.           
+000113c0: 2020 2020 2020 2020 2020 2020 207b 2520               {% 
+000113d0: 656c 6966 2033 5f6c 6566 745f 6220 616e  elif 3_left_b an
+000113e0: 6420 335f 7269 6768 745f 6220 257d 0a20  d 3_right_b %}. 
+000113f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011400: 2020 2020 2020 203c 6469 7620 636c 6173         <div clas
+00011410: 733d 227b 2520 626c 6f63 6b20 335f 6365  s="{% block 3_ce
+00011420: 6e74 6572 5f6c 6566 745f 625f 7269 6768  nter_left_b_righ
+00011430: 745f 6220 257d 636f 6c2d 3132 2063 6f6c  t_b %}col-12 col
+00011440: 2d6c 672d 3420 6f66 6673 6574 2d6c 672d  -lg-4 offset-lg-
+00011450: 317b 2520 656e 6462 6c6f 636b 2025 7d22  1{% endblock %}"
+00011460: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
+00011470: 2020 2020 2020 2020 2020 7b25 2065 6c69            {% eli
+00011480: 6620 335f 6c65 6674 5f61 2061 6e64 2033  f 3_left_a and 3
+00011490: 5f6c 6566 745f 6220 257d 0a20 2020 2020  _left_b %}.     
+000114a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000114b0: 2020 203c 6469 7620 636c 6173 733d 227b     <div class="{
+000114c0: 2520 626c 6f63 6b20 335f 6365 6e74 6572  % block 3_center
+000114d0: 5f6c 6566 745f 6162 2025 7d63 6f6c 2d31  _left_ab %}col-1
+000114e0: 3220 636f 6c2d 6c67 2d38 7b25 2065 6e64  2 col-lg-8{% end
+000114f0: 626c 6f63 6b20 257d 223e 0a20 2020 2020  block %}">.     
+00011500: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011510: 2020 207b 2520 656c 6966 2033 5f6c 6566     {% elif 3_lef
+00011520: 745f 6120 257d 0a20 2020 2020 2020 2020  t_a %}.         
+00011530: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+00011540: 6469 7620 636c 6173 733d 227b 2520 626c  div class="{% bl
+00011550: 6f63 6b20 335f 6365 6e74 6572 5f6c 6566  ock 3_center_lef
+00011560: 745f 6120 257d 636f 6c2d 3132 2063 6f6c  t_a %}col-12 col
+00011570: 2d6c 672d 397b 2520 656e 6462 6c6f 636b  -lg-9{% endblock
+00011580: 2025 7d22 3e0a 2020 2020 2020 2020 2020   %}">.          
+00011590: 2020 2020 2020 2020 2020 2020 2020 7b25                {%
+000115a0: 2065 6c69 6620 335f 6c65 6674 5f62 2025   elif 3_left_b %
+000115b0: 7d0a 2020 2020 2020 2020 2020 2020 2020  }.              
+000115c0: 2020 2020 2020 2020 2020 3c64 6976 2063            <div c
+000115d0: 6c61 7373 3d22 7b25 2062 6c6f 636b 2033  lass="{% block 3
+000115e0: 5f63 656e 7465 725f 6c65 6674 5f62 2025  _center_left_b %
+000115f0: 7d63 6f6c 2d31 3220 636f 6c2d 6c67 2d38  }col-12 col-lg-8
+00011600: 206f 6666 7365 742d 6c67 2d31 7b25 2065   offset-lg-1{% e
+00011610: 6e64 626c 6f63 6b20 257d 223e 0a20 2020  ndblock %}">.   
+00011620: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011630: 2020 2020 207b 2520 656c 6966 2033 5f72       {% elif 3_r
+00011640: 6967 6874 5f61 2061 6e64 2033 5f72 6967  ight_a and 3_rig
+00011650: 6874 5f62 2025 7d0a 2020 2020 2020 2020  ht_b %}.        
 00011660: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011670: 2020 2020 2020 2020 2020 2020 203c 6469               <di
-00011680: 7620 636c 6173 733d 227b 2520 626c 6f63  v class="{% bloc
-00011690: 6b20 335f 6365 6e74 6572 5f74 6f70 5f61  k 3_center_top_a
-000116a0: 6263 5f62 2025 7d63 6f6c 2d31 3220 636f  bc_b %}col-12 co
-000116b0: 6c2d 6d64 2d34 7b25 2065 6e64 626c 6f63  l-md-4{% endbloc
-000116c0: 6b20 257d 223e 7b7b 2033 5f63 656e 7465  k %}">{{ 3_cente
-000116d0: 725f 746f 705f 6220 7d7d 3c2f 6469 763e  r_top_b }}</div>
-000116e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000116f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011700: 2020 2020 203c 6469 7620 636c 6173 733d       <div class=
-00011710: 227b 2520 626c 6f63 6b20 335f 6365 6e74  "{% block 3_cent
-00011720: 6572 5f74 6f70 5f61 6263 5f63 2025 7d63  er_top_abc_c %}c
-00011730: 6f6c 2d31 3220 636f 6c2d 6d64 2d34 7b25  ol-12 col-md-4{%
-00011740: 2065 6e64 626c 6f63 6b20 257d 223e 7b7b   endblock %}">{{
-00011750: 2033 5f63 656e 7465 725f 746f 705f 6320   3_center_top_c 
-00011760: 7d7d 3c2f 6469 763e 0a20 2020 2020 2020  }}</div>.       
-00011770: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011780: 2020 2020 2020 2020 207b 2520 656c 6966           {% elif
-00011790: 2033 5f63 656e 7465 725f 746f 705f 6120   3_center_top_a 
-000117a0: 616e 6420 335f 6365 6e74 6572 5f74 6f70  and 3_center_top
-000117b0: 5f62 2025 7d0a 2020 2020 2020 2020 2020  _b %}.          
-000117c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000117d0: 2020 2020 2020 2020 2020 3c64 6976 2063            <div c
-000117e0: 6c61 7373 3d22 7b25 2062 6c6f 636b 2033  lass="{% block 3
-000117f0: 5f63 656e 7465 725f 746f 705f 6162 5f61  _center_top_ab_a
-00011800: 2025 7d63 6f6c 2d31 3220 636f 6c2d 6d64   %}col-12 col-md
-00011810: 2d38 7b25 2065 6e64 626c 6f63 6b20 257d  -8{% endblock %}
-00011820: 223e 7b7b 2033 5f63 656e 7465 725f 746f  ">{{ 3_center_to
-00011830: 705f 6120 7d7d 3c2f 6469 763e 0a20 2020  p_a }}</div>.   
-00011840: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011850: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011860: 203c 6469 7620 636c 6173 733d 227b 2520   <div class="{% 
-00011870: 626c 6f63 6b20 335f 6365 6e74 6572 5f74  block 3_center_t
-00011880: 6f70 5f61 625f 6220 257d 636f 6c2d 3132  op_ab_b %}col-12
-00011890: 2063 6f6c 2d6d 642d 347b 2520 656e 6462   col-md-4{% endb
-000118a0: 6c6f 636b 2025 7d22 3e7b 7b20 335f 6365  lock %}">{{ 3_ce
-000118b0: 6e74 6572 5f74 6f70 5f62 207d 7d3c 2f64  nter_top_b }}</d
-000118c0: 6976 3e0a 2020 2020 2020 2020 2020 2020  iv>.            
-000118d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000118e0: 2020 2020 7b25 2065 6c69 6620 335f 6365      {% elif 3_ce
-000118f0: 6e74 6572 5f74 6f70 5f61 2061 6e64 2033  nter_top_a and 3
-00011900: 5f63 656e 7465 725f 746f 705f 6320 257d  _center_top_c %}
-00011910: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00011920: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011930: 2020 2020 203c 6469 7620 636c 6173 733d       <div class=
-00011940: 227b 2520 626c 6f63 6b20 335f 6365 6e74  "{% block 3_cent
-00011950: 6572 5f74 6f70 5f61 635f 6120 257d 636f  er_top_ac_a %}co
-00011960: 6c2d 3132 2063 6f6c 2d6d 642d 367b 2520  l-12 col-md-6{% 
-00011970: 656e 6462 6c6f 636b 2025 7d22 3e7b 7b20  endblock %}">{{ 
-00011980: 335f 6365 6e74 6572 5f74 6f70 5f61 207d  3_center_top_a }
-00011990: 7d3c 2f64 6976 3e0a 2020 2020 2020 2020  }</div>.        
-000119a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000119b0: 2020 2020 2020 2020 2020 2020 3c64 6976              <div
-000119c0: 2063 6c61 7373 3d22 7b25 2062 6c6f 636b   class="{% block
-000119d0: 2033 5f63 656e 7465 725f 746f 705f 6163   3_center_top_ac
-000119e0: 5f63 2025 7d63 6f6c 2d31 3220 636f 6c2d  _c %}col-12 col-
-000119f0: 6d64 2d36 7b25 2065 6e64 626c 6f63 6b20  md-6{% endblock 
-00011a00: 257d 223e 7b7b 2033 5f63 656e 7465 725f  %}">{{ 3_center_
-00011a10: 746f 705f 6320 7d7d 3c2f 6469 763e 0a20  top_c }}</div>. 
-00011a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011a30: 2020 2020 2020 2020 2020 2020 2020 207b                 {
-00011a40: 2520 656c 6966 2033 5f63 656e 7465 725f  % elif 3_center_
-00011a50: 746f 705f 6220 616e 6420 335f 6365 6e74  top_b and 3_cent
-00011a60: 6572 5f74 6f70 5f63 2025 7d0a 2020 2020  er_top_c %}.    
-00011a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011a90: 3c64 6976 2063 6c61 7373 3d22 7b25 2062  <div class="{% b
-00011aa0: 6c6f 636b 2033 5f63 656e 7465 725f 746f  lock 3_center_to
-00011ab0: 705f 6263 5f62 2025 7d63 6f6c 2d31 3220  p_bc_b %}col-12 
-00011ac0: 636f 6c2d 6d64 2d34 7b25 2065 6e64 626c  col-md-4{% endbl
-00011ad0: 6f63 6b20 257d 223e 7b7b 2033 5f63 656e  ock %}">{{ 3_cen
-00011ae0: 7465 725f 746f 705f 6220 7d7d 3c2f 6469  ter_top_b }}</di
-00011af0: 763e 0a20 2020 2020 2020 2020 2020 2020  v>.             
-00011b00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011b10: 2020 2020 2020 203c 6469 7620 636c 6173         <div clas
-00011b20: 733d 227b 2520 626c 6f63 6b20 335f 6365  s="{% block 3_ce
-00011b30: 6e74 6572 5f74 6f70 5f62 635f 6320 257d  nter_top_bc_c %}
-00011b40: 636f 6c2d 3132 2063 6f6c 2d6d 642d 387b  col-12 col-md-8{
-00011b50: 2520 656e 6462 6c6f 636b 2025 7d22 3e7b  % endblock %}">{
-00011b60: 7b20 335f 6365 6e74 6572 5f74 6f70 5f63  { 3_center_top_c
-00011b70: 207d 7d3c 2f64 6976 3e0a 2020 2020 2020   }}</div>.      
-00011b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011b90: 2020 2020 2020 2020 2020 7b25 2065 6c73            {% els
-00011ba0: 6520 257d 0a20 2020 2020 2020 2020 2020  e %}.           
-00011bb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011bc0: 2020 2020 2020 2020 203c 6469 7620 636c           <div cl
-00011bd0: 6173 733d 2263 6f6c 2d31 3222 3e7b 7b20  ass="col-12">{{ 
-00011be0: 335f 6365 6e74 6572 5f74 6f70 5f61 207d  3_center_top_a }
-00011bf0: 7d7b 7b20 335f 6365 6e74 6572 5f74 6f70  }{{ 3_center_top
-00011c00: 5f62 207d 7d7b 7b20 335f 6365 6e74 6572  _b }}{{ 3_center
-00011c10: 5f74 6f70 5f63 207d 7d3c 2f64 6976 3e0a  _top_c }}</div>.
-00011c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011c30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011c40: 7b25 2065 6e64 6966 2025 7d0a 2020 2020  {% endif %}.    
+00011670: 3c64 6976 2063 6c61 7373 3d22 7b25 2062  <div class="{% b
+00011680: 6c6f 636b 2033 5f63 656e 7465 725f 7269  lock 3_center_ri
+00011690: 6768 745f 6162 2025 7d63 6f6c 2d31 3220  ght_ab %}col-12 
+000116a0: 636f 6c2d 6c67 2d38 7b25 2065 6e64 626c  col-lg-8{% endbl
+000116b0: 6f63 6b20 257d 223e 0a20 2020 2020 2020  ock %}">.       
+000116c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000116d0: 207b 2520 656c 6966 2033 5f72 6967 6874   {% elif 3_right
+000116e0: 5f61 2025 7d0a 2020 2020 2020 2020 2020  _a %}.          
+000116f0: 2020 2020 2020 2020 2020 2020 2020 3c64                <d
+00011700: 6976 2063 6c61 7373 3d22 7b25 2062 6c6f  iv class="{% blo
+00011710: 636b 2033 5f63 656e 7465 725f 7269 6768  ck 3_center_righ
+00011720: 745f 6120 257d 636f 6c2d 3132 2063 6f6c  t_a %}col-12 col
+00011730: 2d6c 672d 397b 2520 656e 6462 6c6f 636b  -lg-9{% endblock
+00011740: 2025 7d22 3e0a 2020 2020 2020 2020 2020   %}">.          
+00011750: 2020 2020 2020 2020 2020 2020 2020 7b25                {%
+00011760: 2065 6c69 6620 335f 7269 6768 745f 6220   elif 3_right_b 
+00011770: 257d 0a20 2020 2020 2020 2020 2020 2020  %}.             
+00011780: 2020 2020 2020 2020 2020 203c 6469 7620             <div 
+00011790: 636c 6173 733d 227b 2520 626c 6f63 6b20  class="{% block 
+000117a0: 335f 6365 6e74 6572 5f72 6967 6874 5f62  3_center_right_b
+000117b0: 2025 7d63 6f6c 2d31 3220 636f 6c2d 6c67   %}col-12 col-lg
+000117c0: 2d38 7b25 2065 6e64 626c 6f63 6b20 257d  -8{% endblock %}
+000117d0: 223e 0a20 2020 2020 2020 2020 2020 2020  ">.             
+000117e0: 2020 2020 2020 2020 2020 207b 2520 656c             {% el
+000117f0: 7365 2025 7d0a 2020 2020 2020 2020 2020  se %}.          
+00011800: 2020 2020 2020 2020 2020 2020 2020 3c64                <d
+00011810: 6976 2063 6c61 7373 3d22 7b25 2062 6c6f  iv class="{% blo
+00011820: 636b 2033 5f63 656e 7465 7220 257d 636f  ck 3_center %}co
+00011830: 6c2d 3132 7b25 2065 6e64 626c 6f63 6b20  l-12{% endblock 
+00011840: 257d 223e 0a20 2020 2020 2020 2020 2020  %}">.           
+00011850: 2020 2020 2020 2020 2020 2020 207b 2520               {% 
+00011860: 656e 6469 6620 257d 0a20 2020 2020 2020  endif %}.       
+00011870: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011880: 203c 212d 2d20 456e 6420 426c 6f63 6b73   <!-- End Blocks
+00011890: 2069 6e20 4365 6e74 6572 2063 6f6c 756d   in Center colum
+000118a0: 6e20 2874 616b 6573 2061 7661 696c 6162  n (takes availab
+000118b0: 6c65 2073 7061 6365 2920 2d2d 3e0a 0a20  le space) -->.. 
+000118c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000118d0: 2020 2020 2020 2020 2020 203c 212d 2d20             <!-- 
+000118e0: 4365 6e74 6572 2074 6f70 202d 2d3e 0a20  Center top -->. 
+000118f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011900: 2020 2020 2020 2020 2020 207b 2520 6966             {% if
+00011910: 2033 5f63 656e 7465 725f 746f 705f 6120   3_center_top_a 
+00011920: 6f72 2033 5f63 656e 7465 725f 746f 705f  or 3_center_top_
+00011930: 6220 6f72 2033 5f63 656e 7465 725f 746f  b or 3_center_to
+00011940: 705f 6320 257d 0a20 2020 2020 2020 2020  p_c %}.         
+00011950: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011960: 2020 203c 6469 7620 636c 6173 733d 2272     <div class="r
+00011970: 6f77 223e 0a20 2020 2020 2020 2020 2020  ow">.           
+00011980: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011990: 2020 2020 207b 2520 6966 2033 5f63 656e       {% if 3_cen
+000119a0: 7465 725f 746f 705f 6120 616e 6420 335f  ter_top_a and 3_
+000119b0: 6365 6e74 6572 5f74 6f70 5f62 2061 6e64  center_top_b and
+000119c0: 2033 5f63 656e 7465 725f 746f 705f 6320   3_center_top_c 
+000119d0: 257d 0a20 2020 2020 2020 2020 2020 2020  %}.             
+000119e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000119f0: 2020 2020 2020 203c 6469 7620 636c 6173         <div clas
+00011a00: 733d 227b 2520 626c 6f63 6b20 335f 6365  s="{% block 3_ce
+00011a10: 6e74 6572 5f74 6f70 5f61 6263 5f61 2025  nter_top_abc_a %
+00011a20: 7d63 6f6c 2d31 3220 636f 6c2d 6d64 2d34  }col-12 col-md-4
+00011a30: 7b25 2065 6e64 626c 6f63 6b20 257d 223e  {% endblock %}">
+00011a40: 7b7b 2033 5f63 656e 7465 725f 746f 705f  {{ 3_center_top_
+00011a50: 6120 7d7d 3c2f 6469 763e 0a20 2020 2020  a }}</div>.     
+00011a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011a70: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+00011a80: 6469 7620 636c 6173 733d 227b 2520 626c  div class="{% bl
+00011a90: 6f63 6b20 335f 6365 6e74 6572 5f74 6f70  ock 3_center_top
+00011aa0: 5f61 6263 5f62 2025 7d63 6f6c 2d31 3220  _abc_b %}col-12 
+00011ab0: 636f 6c2d 6d64 2d34 7b25 2065 6e64 626c  col-md-4{% endbl
+00011ac0: 6f63 6b20 257d 223e 7b7b 2033 5f63 656e  ock %}">{{ 3_cen
+00011ad0: 7465 725f 746f 705f 6220 7d7d 3c2f 6469  ter_top_b }}</di
+00011ae0: 763e 0a20 2020 2020 2020 2020 2020 2020  v>.             
+00011af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011b00: 2020 2020 2020 203c 6469 7620 636c 6173         <div clas
+00011b10: 733d 227b 2520 626c 6f63 6b20 335f 6365  s="{% block 3_ce
+00011b20: 6e74 6572 5f74 6f70 5f61 6263 5f63 2025  nter_top_abc_c %
+00011b30: 7d63 6f6c 2d31 3220 636f 6c2d 6d64 2d34  }col-12 col-md-4
+00011b40: 7b25 2065 6e64 626c 6f63 6b20 257d 223e  {% endblock %}">
+00011b50: 7b7b 2033 5f63 656e 7465 725f 746f 705f  {{ 3_center_top_
+00011b60: 6320 7d7d 3c2f 6469 763e 0a20 2020 2020  c }}</div>.     
+00011b70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011b80: 2020 2020 2020 2020 2020 207b 2520 656c             {% el
+00011b90: 6966 2033 5f63 656e 7465 725f 746f 705f  if 3_center_top_
+00011ba0: 6120 616e 6420 335f 6365 6e74 6572 5f74  a and 3_center_t
+00011bb0: 6f70 5f62 2025 7d0a 2020 2020 2020 2020  op_b %}.        
+00011bc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011bd0: 2020 2020 2020 2020 2020 2020 3c64 6976              <div
+00011be0: 2063 6c61 7373 3d22 7b25 2062 6c6f 636b   class="{% block
+00011bf0: 2033 5f63 656e 7465 725f 746f 705f 6162   3_center_top_ab
+00011c00: 5f61 2025 7d63 6f6c 2d31 3220 636f 6c2d  _a %}col-12 col-
+00011c10: 6d64 2d38 7b25 2065 6e64 626c 6f63 6b20  md-8{% endblock 
+00011c20: 257d 223e 7b7b 2033 5f63 656e 7465 725f  %}">{{ 3_center_
+00011c30: 746f 705f 6120 7d7d 3c2f 6469 763e 0a20  top_a }}</div>. 
+00011c40: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00011c50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011c60: 2020 2020 2020 2020 3c2f 6469 763e 0a20          </div>. 
-00011c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011c80: 2020 2020 2020 2020 2020 207b 2520 656e             {% en
-00011c90: 6469 6620 257d 0a20 2020 2020 2020 2020  dif %}.         
-00011ca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011cb0: 2020 203c 212d 2d20 454e 4420 4365 6e74     <!-- END Cent
-00011cc0: 6572 2074 6f70 202d 2d3e 0a0a 2020 2020  er top -->..    
+00011c60: 2020 203c 6469 7620 636c 6173 733d 227b     <div class="{
+00011c70: 2520 626c 6f63 6b20 335f 6365 6e74 6572  % block 3_center
+00011c80: 5f74 6f70 5f61 625f 6220 257d 636f 6c2d  _top_ab_b %}col-
+00011c90: 3132 2063 6f6c 2d6d 642d 347b 2520 656e  12 col-md-4{% en
+00011ca0: 6462 6c6f 636b 2025 7d22 3e7b 7b20 335f  dblock %}">{{ 3_
+00011cb0: 6365 6e74 6572 5f74 6f70 5f62 207d 7d3c  center_top_b }}<
+00011cc0: 2f64 6976 3e0a 2020 2020 2020 2020 2020  /div>.          
 00011cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011ce0: 2020 2020 2020 2020 3c21 2d2d 2043 656e          <!-- Cen
-00011cf0: 7465 7220 6d69 642d 746f 7020 2d2d 3e0a  ter mid-top -->.
-00011d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011d10: 2020 2020 2020 2020 2020 2020 7b25 2069              {% i
-00011d20: 6620 335f 6365 6e74 6572 5f6d 6964 5f74  f 3_center_mid_t
-00011d30: 6f70 5f61 206f 7220 335f 6365 6e74 6572  op_a or 3_center
-00011d40: 5f6d 6964 5f74 6f70 5f62 206f 7220 335f  _mid_top_b or 3_
-00011d50: 6365 6e74 6572 5f74 6f70 5f63 2025 7d0a  center_top_c %}.
-00011d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011d70: 2020 2020 2020 2020 2020 2020 3c64 6976              <div
-00011d80: 2063 6c61 7373 3d22 726f 7722 3e0a 2020   class="row">.  
-00011d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011da0: 2020 2020 2020 2020 2020 2020 2020 7b25                {%
-00011db0: 2069 6620 335f 6365 6e74 6572 5f6d 6964   if 3_center_mid
-00011dc0: 5f74 6f70 5f61 2061 6e64 2033 5f63 656e  _top_a and 3_cen
-00011dd0: 7465 725f 6d69 645f 746f 705f 6220 616e  ter_mid_top_b an
-00011de0: 6420 335f 6365 6e74 6572 5f6d 6964 5f74  d 3_center_mid_t
-00011df0: 6f70 5f63 2025 7d0a 2020 2020 2020 2020  op_c %}.        
-00011e00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011e10: 2020 2020 2020 2020 2020 2020 3c64 6976              <div
-00011e20: 2063 6c61 7373 3d22 7b25 2062 6c6f 636b   class="{% block
-00011e30: 2033 5f63 656e 7465 725f 6d69 645f 746f   3_center_mid_to
-00011e40: 705f 6162 635f 6120 257d 636f 6c2d 3132  p_abc_a %}col-12
-00011e50: 2063 6f6c 2d6d 642d 347b 2520 656e 6462   col-md-4{% endb
-00011e60: 6c6f 636b 2025 7d22 3e7b 7b20 335f 6365  lock %}">{{ 3_ce
-00011e70: 6e74 6572 5f6d 6964 5f74 6f70 5f61 207d  nter_mid_top_a }
-00011e80: 7d3c 2f64 6976 3e0a 2020 2020 2020 2020  }</div>.        
-00011e90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011ea0: 2020 2020 2020 2020 2020 2020 3c64 6976              <div
-00011eb0: 2063 6c61 7373 3d22 7b25 2062 6c6f 636b   class="{% block
-00011ec0: 2033 5f63 656e 7465 725f 6d69 645f 746f   3_center_mid_to
-00011ed0: 705f 6162 635f 6220 257d 636f 6c2d 3132  p_abc_b %}col-12
-00011ee0: 2063 6f6c 2d6d 642d 347b 2520 656e 6462   col-md-4{% endb
-00011ef0: 6c6f 636b 2025 7d22 3e7b 7b20 335f 6365  lock %}">{{ 3_ce
-00011f00: 6e74 6572 5f6d 6964 5f74 6f70 5f62 207d  nter_mid_top_b }
-00011f10: 7d3c 2f64 6976 3e0a 2020 2020 2020 2020  }</div>.        
-00011f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011f30: 2020 2020 2020 2020 2020 2020 3c64 6976              <div
-00011f40: 2063 6c61 7373 3d22 7b25 2062 6c6f 636b   class="{% block
-00011f50: 2033 5f63 656e 7465 725f 6d69 645f 746f   3_center_mid_to
-00011f60: 705f 6162 635f 6320 257d 636f 6c2d 3132  p_abc_c %}col-12
-00011f70: 2063 6f6c 2d6d 642d 347b 2520 656e 6462   col-md-4{% endb
-00011f80: 6c6f 636b 2025 7d22 3e7b 7b20 335f 6365  lock %}">{{ 3_ce
-00011f90: 6e74 6572 5f6d 6964 5f74 6f70 5f63 207d  nter_mid_top_c }
-00011fa0: 7d3c 2f64 6976 3e0a 2020 2020 2020 2020  }</div>.        
+00011ce0: 2020 2020 2020 7b25 2065 6c69 6620 335f        {% elif 3_
+00011cf0: 6365 6e74 6572 5f74 6f70 5f61 2061 6e64  center_top_a and
+00011d00: 2033 5f63 656e 7465 725f 746f 705f 6320   3_center_top_c 
+00011d10: 257d 0a20 2020 2020 2020 2020 2020 2020  %}.             
+00011d20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011d30: 2020 2020 2020 203c 6469 7620 636c 6173         <div clas
+00011d40: 733d 227b 2520 626c 6f63 6b20 335f 6365  s="{% block 3_ce
+00011d50: 6e74 6572 5f74 6f70 5f61 635f 6120 257d  nter_top_ac_a %}
+00011d60: 636f 6c2d 3132 2063 6f6c 2d6d 642d 367b  col-12 col-md-6{
+00011d70: 2520 656e 6462 6c6f 636b 2025 7d22 3e7b  % endblock %}">{
+00011d80: 7b20 335f 6365 6e74 6572 5f74 6f70 5f61  { 3_center_top_a
+00011d90: 207d 7d3c 2f64 6976 3e0a 2020 2020 2020   }}</div>.      
+00011da0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011db0: 2020 2020 2020 2020 2020 2020 2020 3c64                <d
+00011dc0: 6976 2063 6c61 7373 3d22 7b25 2062 6c6f  iv class="{% blo
+00011dd0: 636b 2033 5f63 656e 7465 725f 746f 705f  ck 3_center_top_
+00011de0: 6163 5f63 2025 7d63 6f6c 2d31 3220 636f  ac_c %}col-12 co
+00011df0: 6c2d 6d64 2d36 7b25 2065 6e64 626c 6f63  l-md-6{% endbloc
+00011e00: 6b20 257d 223e 7b7b 2033 5f63 656e 7465  k %}">{{ 3_cente
+00011e10: 725f 746f 705f 6320 7d7d 3c2f 6469 763e  r_top_c }}</div>
+00011e20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00011e30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011e40: 207b 2520 656c 6966 2033 5f63 656e 7465   {% elif 3_cente
+00011e50: 725f 746f 705f 6220 616e 6420 335f 6365  r_top_b and 3_ce
+00011e60: 6e74 6572 5f74 6f70 5f63 2025 7d0a 2020  nter_top_c %}.  
+00011e70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011e80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011e90: 2020 3c64 6976 2063 6c61 7373 3d22 7b25    <div class="{%
+00011ea0: 2062 6c6f 636b 2033 5f63 656e 7465 725f   block 3_center_
+00011eb0: 746f 705f 6263 5f62 2025 7d63 6f6c 2d31  top_bc_b %}col-1
+00011ec0: 3220 636f 6c2d 6d64 2d34 7b25 2065 6e64  2 col-md-4{% end
+00011ed0: 626c 6f63 6b20 257d 223e 7b7b 2033 5f63  block %}">{{ 3_c
+00011ee0: 656e 7465 725f 746f 705f 6220 7d7d 3c2f  enter_top_b }}</
+00011ef0: 6469 763e 0a20 2020 2020 2020 2020 2020  div>.           
+00011f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011f10: 2020 2020 2020 2020 203c 6469 7620 636c           <div cl
+00011f20: 6173 733d 227b 2520 626c 6f63 6b20 335f  ass="{% block 3_
+00011f30: 6365 6e74 6572 5f74 6f70 5f62 635f 6320  center_top_bc_c 
+00011f40: 257d 636f 6c2d 3132 2063 6f6c 2d6d 642d  %}col-12 col-md-
+00011f50: 387b 2520 656e 6462 6c6f 636b 2025 7d22  8{% endblock %}"
+00011f60: 3e7b 7b20 335f 6365 6e74 6572 5f74 6f70  >{{ 3_center_top
+00011f70: 5f63 207d 7d3c 2f64 6976 3e0a 2020 2020  _c }}</div>.    
+00011f80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011f90: 2020 2020 2020 2020 2020 2020 7b25 2065              {% e
+00011fa0: 6c73 6520 257d 0a20 2020 2020 2020 2020  lse %}.         
 00011fb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011fc0: 2020 2020 2020 2020 7b25 2065 6c69 6620          {% elif 
-00011fd0: 335f 6365 6e74 6572 5f6d 6964 5f74 6f70  3_center_mid_top
-00011fe0: 5f61 2061 6e64 2033 5f63 656e 7465 725f  _a and 3_center_
-00011ff0: 6d69 645f 746f 705f 6220 257d 0a20 2020  mid_top_b %}.   
-00012000: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012010: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012020: 203c 6469 7620 636c 6173 733d 227b 2520   <div class="{% 
-00012030: 626c 6f63 6b20 335f 6365 6e74 6572 5f6d  block 3_center_m
-00012040: 6964 5f74 6f70 5f61 625f 6120 257d 636f  id_top_ab_a %}co
-00012050: 6c2d 3132 2063 6f6c 2d6d 642d 387b 2520  l-12 col-md-8{% 
-00012060: 656e 6462 6c6f 636b 2025 7d22 3e7b 7b20  endblock %}">{{ 
-00012070: 335f 6365 6e74 6572 5f6d 6964 5f74 6f70  3_center_mid_top
-00012080: 5f61 207d 7d3c 2f64 6976 3e0a 2020 2020  _a }}</div>.    
-00012090: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011fc0: 2020 2020 2020 2020 2020 203c 6469 7620             <div 
+00011fd0: 636c 6173 733d 2263 6f6c 2d31 3222 3e7b  class="col-12">{
+00011fe0: 7b20 335f 6365 6e74 6572 5f74 6f70 5f61  { 3_center_top_a
+00011ff0: 207d 7d7b 7b20 335f 6365 6e74 6572 5f74   }}{{ 3_center_t
+00012000: 6f70 5f62 207d 7d7b 7b20 335f 6365 6e74  op_b }}{{ 3_cent
+00012010: 6572 5f74 6f70 5f63 207d 7d3c 2f64 6976  er_top_c }}</div
+00012020: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
+00012030: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012040: 2020 7b25 2065 6e64 6966 2025 7d0a 2020    {% endif %}.  
+00012050: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012060: 2020 2020 2020 2020 2020 3c2f 6469 763e            </div>
+00012070: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00012080: 2020 2020 2020 2020 2020 2020 207b 2520               {% 
+00012090: 656e 6469 6620 257d 0a20 2020 2020 2020  endif %}.       
 000120a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000120b0: 3c64 6976 2063 6c61 7373 3d22 7b25 2062  <div class="{% b
-000120c0: 6c6f 636b 2033 5f63 656e 7465 725f 6d69  lock 3_center_mi
-000120d0: 645f 746f 705f 6162 5f62 2025 7d63 6f6c  d_top_ab_b %}col
-000120e0: 2d31 3220 636f 6c2d 6d64 2d34 7b25 2065  -12 col-md-4{% e
-000120f0: 6e64 626c 6f63 6b20 257d 223e 7b7b 2033  ndblock %}">{{ 3
-00012100: 5f63 656e 7465 725f 6d69 645f 746f 705f  _center_mid_top_
-00012110: 6220 7d7d 3c2f 6469 763e 0a20 2020 2020  b }}</div>.     
-00012120: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012130: 2020 2020 2020 2020 2020 207b 2520 656c             {% el
-00012140: 6966 2033 5f63 656e 7465 725f 6d69 645f  if 3_center_mid_
-00012150: 746f 705f 6120 616e 6420 335f 6365 6e74  top_a and 3_cent
-00012160: 6572 5f6d 6964 5f74 6f70 5f63 2025 7d0a  er_mid_top_c %}.
-00012170: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012180: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012190: 2020 2020 3c64 6976 2063 6c61 7373 3d22      <div class="
-000121a0: 7b25 2062 6c6f 636b 2033 5f63 656e 7465  {% block 3_cente
-000121b0: 725f 6d69 645f 746f 705f 6163 5f61 2025  r_mid_top_ac_a %
-000121c0: 7d63 6f6c 2d31 3220 636f 6c2d 6d64 2d36  }col-12 col-md-6
-000121d0: 7b25 2065 6e64 626c 6f63 6b20 257d 223e  {% endblock %}">
-000121e0: 7b7b 2033 5f63 656e 7465 725f 6d69 645f  {{ 3_center_mid_
-000121f0: 746f 705f 6120 7d7d 3c2f 6469 763e 0a20  top_a }}</div>. 
+000120b0: 2020 2020 203c 212d 2d20 454e 4420 4365       <!-- END Ce
+000120c0: 6e74 6572 2074 6f70 202d 2d3e 0a0a 2020  nter top -->..  
+000120d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000120e0: 2020 2020 2020 2020 2020 3c21 2d2d 2043            <!-- C
+000120f0: 656e 7465 7220 6d69 642d 746f 7020 2d2d  enter mid-top --
+00012100: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
+00012110: 2020 2020 2020 2020 2020 2020 2020 7b25                {%
+00012120: 2069 6620 335f 6365 6e74 6572 5f6d 6964   if 3_center_mid
+00012130: 5f74 6f70 5f61 206f 7220 335f 6365 6e74  _top_a or 3_cent
+00012140: 6572 5f6d 6964 5f74 6f70 5f62 206f 7220  er_mid_top_b or 
+00012150: 335f 6365 6e74 6572 5f74 6f70 5f63 2025  3_center_top_c %
+00012160: 7d0a 2020 2020 2020 2020 2020 2020 2020  }.              
+00012170: 2020 2020 2020 2020 2020 2020 2020 3c64                <d
+00012180: 6976 2063 6c61 7373 3d22 726f 7722 3e0a  iv class="row">.
+00012190: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000121a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000121b0: 7b25 2069 6620 335f 6365 6e74 6572 5f6d  {% if 3_center_m
+000121c0: 6964 5f74 6f70 5f61 2061 6e64 2033 5f63  id_top_a and 3_c
+000121d0: 656e 7465 725f 6d69 645f 746f 705f 6220  enter_mid_top_b 
+000121e0: 616e 6420 335f 6365 6e74 6572 5f6d 6964  and 3_center_mid
+000121f0: 5f74 6f70 5f63 2025 7d0a 2020 2020 2020  _top_c %}.      
 00012200: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012210: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012220: 2020 203c 6469 7620 636c 6173 733d 227b     <div class="{
-00012230: 2520 626c 6f63 6b20 335f 6365 6e74 6572  % block 3_center
-00012240: 5f6d 6964 5f74 6f70 5f61 635f 6320 257d  _mid_top_ac_c %}
-00012250: 636f 6c2d 3132 2063 6f6c 2d6d 642d 367b  col-12 col-md-6{
-00012260: 2520 656e 6462 6c6f 636b 2025 7d22 3e7b  % endblock %}">{
-00012270: 7b20 335f 6365 6e74 6572 5f6d 6964 5f74  { 3_center_mid_t
-00012280: 6f70 5f63 207d 7d3c 2f64 6976 3e0a 2020  op_c }}</div>.  
+00012210: 2020 2020 2020 2020 2020 2020 2020 3c64                <d
+00012220: 6976 2063 6c61 7373 3d22 7b25 2062 6c6f  iv class="{% blo
+00012230: 636b 2033 5f63 656e 7465 725f 6d69 645f  ck 3_center_mid_
+00012240: 746f 705f 6162 635f 6120 257d 636f 6c2d  top_abc_a %}col-
+00012250: 3132 2063 6f6c 2d6d 642d 347b 2520 656e  12 col-md-4{% en
+00012260: 6462 6c6f 636b 2025 7d22 3e7b 7b20 335f  dblock %}">{{ 3_
+00012270: 6365 6e74 6572 5f6d 6964 5f74 6f70 5f61  center_mid_top_a
+00012280: 207d 7d3c 2f64 6976 3e0a 2020 2020 2020   }}</div>.      
 00012290: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000122a0: 2020 2020 2020 2020 2020 2020 2020 7b25                {%
-000122b0: 2065 6c69 6620 335f 6365 6e74 6572 5f6d   elif 3_center_m
-000122c0: 6964 5f74 6f70 5f62 2061 6e64 2033 5f63  id_top_b and 3_c
-000122d0: 656e 7465 725f 6d69 645f 746f 705f 6320  enter_mid_top_c 
-000122e0: 257d 0a20 2020 2020 2020 2020 2020 2020  %}.             
-000122f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012300: 2020 2020 2020 203c 6469 7620 636c 6173         <div clas
-00012310: 733d 227b 2520 626c 6f63 6b20 335f 6365  s="{% block 3_ce
-00012320: 6e74 6572 5f6d 6964 5f74 6f70 5f62 635f  nter_mid_top_bc_
-00012330: 6220 257d 636f 6c2d 3132 2063 6f6c 2d6d  b %}col-12 col-m
-00012340: 642d 347b 2520 656e 6462 6c6f 636b 2025  d-4{% endblock %
-00012350: 7d22 3e7b 7b20 335f 6365 6e74 6572 5f6d  }">{{ 3_center_m
-00012360: 6964 5f74 6f70 5f62 207d 7d3c 2f64 6976  id_top_b }}</div
-00012370: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
-00012380: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012390: 2020 2020 2020 3c64 6976 2063 6c61 7373        <div class
-000123a0: 3d22 7b25 2062 6c6f 636b 2033 5f63 656e  ="{% block 3_cen
-000123b0: 7465 725f 6d69 645f 746f 705f 6263 5f63  ter_mid_top_bc_c
-000123c0: 2025 7d63 6f6c 2d31 3220 636f 6c2d 6d64   %}col-12 col-md
-000123d0: 2d38 7b25 2065 6e64 626c 6f63 6b20 257d  -8{% endblock %}
-000123e0: 223e 7b7b 2033 5f63 656e 7465 725f 6d69  ">{{ 3_center_mi
-000123f0: 645f 746f 705f 6320 7d7d 3c2f 6469 763e  d_top_c }}</div>
-00012400: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000122a0: 2020 2020 2020 2020 2020 2020 2020 3c64                <d
+000122b0: 6976 2063 6c61 7373 3d22 7b25 2062 6c6f  iv class="{% blo
+000122c0: 636b 2033 5f63 656e 7465 725f 6d69 645f  ck 3_center_mid_
+000122d0: 746f 705f 6162 635f 6220 257d 636f 6c2d  top_abc_b %}col-
+000122e0: 3132 2063 6f6c 2d6d 642d 347b 2520 656e  12 col-md-4{% en
+000122f0: 6462 6c6f 636b 2025 7d22 3e7b 7b20 335f  dblock %}">{{ 3_
+00012300: 6365 6e74 6572 5f6d 6964 5f74 6f70 5f62  center_mid_top_b
+00012310: 207d 7d3c 2f64 6976 3e0a 2020 2020 2020   }}</div>.      
+00012320: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012330: 2020 2020 2020 2020 2020 2020 2020 3c64                <d
+00012340: 6976 2063 6c61 7373 3d22 7b25 2062 6c6f  iv class="{% blo
+00012350: 636b 2033 5f63 656e 7465 725f 6d69 645f  ck 3_center_mid_
+00012360: 746f 705f 6162 635f 6320 257d 636f 6c2d  top_abc_c %}col-
+00012370: 3132 2063 6f6c 2d6d 642d 347b 2520 656e  12 col-md-4{% en
+00012380: 6462 6c6f 636b 2025 7d22 3e7b 7b20 335f  dblock %}">{{ 3_
+00012390: 6365 6e74 6572 5f6d 6964 5f74 6f70 5f63  center_mid_top_c
+000123a0: 207d 7d3c 2f64 6976 3e0a 2020 2020 2020   }}</div>.      
+000123b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000123c0: 2020 2020 2020 2020 2020 7b25 2065 6c69            {% eli
+000123d0: 6620 335f 6365 6e74 6572 5f6d 6964 5f74  f 3_center_mid_t
+000123e0: 6f70 5f61 2061 6e64 2033 5f63 656e 7465  op_a and 3_cente
+000123f0: 725f 6d69 645f 746f 705f 6220 257d 0a20  r_mid_top_b %}. 
+00012400: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00012410: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012420: 207b 2520 656c 7365 2025 7d0a 2020 2020   {% else %}.    
-00012430: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012440: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012450: 3c64 6976 2063 6c61 7373 3d22 636f 6c2d  <div class="col-
-00012460: 3132 223e 7b7b 2033 5f63 656e 7465 725f  12">{{ 3_center_
-00012470: 6d69 645f 746f 705f 6120 7d7d 7b7b 2033  mid_top_a }}{{ 3
-00012480: 5f63 656e 7465 725f 6d69 645f 746f 705f  _center_mid_top_
-00012490: 6220 7d7d 7b7b 2033 5f63 656e 7465 725f  b }}{{ 3_center_
-000124a0: 6d69 645f 746f 705f 6320 7d7d 3c2f 6469  mid_top_c }}</di
-000124b0: 763e 0a20 2020 2020 2020 2020 2020 2020  v>.             
-000124c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000124d0: 2020 207b 2520 656e 6469 6620 257d 0a20     {% endif %}. 
-000124e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000124f0: 2020 2020 2020 2020 2020 203c 2f64 6976             </div
-00012500: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
-00012510: 2020 2020 2020 2020 2020 2020 2020 7b25                {%
-00012520: 2065 6e64 6966 2025 7d0a 2020 2020 2020   endif %}.      
-00012530: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012540: 2020 2020 2020 3c21 2d2d 2045 4e44 2043        <!-- END C
-00012550: 656e 7465 7220 6d69 642d 746f 7020 2d2d  enter mid-top --
-00012560: 3e0a 0a20 2020 2020 2020 2020 2020 2020  >..             
-00012570: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-00012580: 212d 2d20 4365 6e74 6572 2063 6f6e 7465  !-- Center conte
-00012590: 6e74 202d 2d3e 0a20 2020 2020 2020 2020  nt -->.         
-000125a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000125b0: 2020 207b 2520 6966 2033 5f63 656e 7465     {% if 3_cente
-000125c0: 725f 636f 6e74 656e 7420 257d 0a20 2020  r_content %}.   
-000125d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000125e0: 2020 2020 2020 2020 203c 6469 7620 636c           <div cl
-000125f0: 6173 733d 2272 6f77 223e 0a20 2020 2020  ass="row">.     
-00012600: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012610: 2020 2020 2020 2020 2020 203c 6469 7620             <div 
-00012620: 636c 6173 733d 2263 6f6c 223e 0a20 2020  class="col">.   
-00012630: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012640: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012650: 207b 7b20 335f 6365 6e74 6572 5f63 6f6e   {{ 3_center_con
-00012660: 7465 6e74 207d 7d0a 2020 2020 2020 2020  tent }}.        
-00012670: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012680: 2020 2020 2020 2020 3c2f 6469 763e 0a20          </div>. 
+00012420: 2020 203c 6469 7620 636c 6173 733d 227b     <div class="{
+00012430: 2520 626c 6f63 6b20 335f 6365 6e74 6572  % block 3_center
+00012440: 5f6d 6964 5f74 6f70 5f61 625f 6120 257d  _mid_top_ab_a %}
+00012450: 636f 6c2d 3132 2063 6f6c 2d6d 642d 387b  col-12 col-md-8{
+00012460: 2520 656e 6462 6c6f 636b 2025 7d22 3e7b  % endblock %}">{
+00012470: 7b20 335f 6365 6e74 6572 5f6d 6964 5f74  { 3_center_mid_t
+00012480: 6f70 5f61 207d 7d3c 2f64 6976 3e0a 2020  op_a }}</div>.  
+00012490: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000124a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000124b0: 2020 3c64 6976 2063 6c61 7373 3d22 7b25    <div class="{%
+000124c0: 2062 6c6f 636b 2033 5f63 656e 7465 725f   block 3_center_
+000124d0: 6d69 645f 746f 705f 6162 5f62 2025 7d63  mid_top_ab_b %}c
+000124e0: 6f6c 2d31 3220 636f 6c2d 6d64 2d34 7b25  ol-12 col-md-4{%
+000124f0: 2065 6e64 626c 6f63 6b20 257d 223e 7b7b   endblock %}">{{
+00012500: 2033 5f63 656e 7465 725f 6d69 645f 746f   3_center_mid_to
+00012510: 705f 6220 7d7d 3c2f 6469 763e 0a20 2020  p_b }}</div>.   
+00012520: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012530: 2020 2020 2020 2020 2020 2020 207b 2520               {% 
+00012540: 656c 6966 2033 5f63 656e 7465 725f 6d69  elif 3_center_mi
+00012550: 645f 746f 705f 6120 616e 6420 335f 6365  d_top_a and 3_ce
+00012560: 6e74 6572 5f6d 6964 5f74 6f70 5f63 2025  nter_mid_top_c %
+00012570: 7d0a 2020 2020 2020 2020 2020 2020 2020  }.              
+00012580: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012590: 2020 2020 2020 3c64 6976 2063 6c61 7373        <div class
+000125a0: 3d22 7b25 2062 6c6f 636b 2033 5f63 656e  ="{% block 3_cen
+000125b0: 7465 725f 6d69 645f 746f 705f 6163 5f61  ter_mid_top_ac_a
+000125c0: 2025 7d63 6f6c 2d31 3220 636f 6c2d 6d64   %}col-12 col-md
+000125d0: 2d36 7b25 2065 6e64 626c 6f63 6b20 257d  -6{% endblock %}
+000125e0: 223e 7b7b 2033 5f63 656e 7465 725f 6d69  ">{{ 3_center_mi
+000125f0: 645f 746f 705f 6120 7d7d 3c2f 6469 763e  d_top_a }}</div>
+00012600: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00012610: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012620: 2020 2020 203c 6469 7620 636c 6173 733d       <div class=
+00012630: 227b 2520 626c 6f63 6b20 335f 6365 6e74  "{% block 3_cent
+00012640: 6572 5f6d 6964 5f74 6f70 5f61 635f 6320  er_mid_top_ac_c 
+00012650: 257d 636f 6c2d 3132 2063 6f6c 2d6d 642d  %}col-12 col-md-
+00012660: 367b 2520 656e 6462 6c6f 636b 2025 7d22  6{% endblock %}"
+00012670: 3e7b 7b20 335f 6365 6e74 6572 5f6d 6964  >{{ 3_center_mid
+00012680: 5f74 6f70 5f63 207d 7d3c 2f64 6976 3e0a  _top_c }}</div>.
 00012690: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000126a0: 2020 2020 2020 2020 2020 203c 2f64 6976             </div
-000126b0: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
-000126c0: 2020 2020 2020 2020 2020 2020 2020 7b25                {%
-000126d0: 2065 6e64 6966 2025 7d0a 2020 2020 2020   endif %}.      
-000126e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000126f0: 2020 2020 2020 3c21 2d2d 2045 4e44 2043        <!-- END C
-00012700: 656e 7465 7220 636f 6e74 656e 7420 2d2d  enter content --
-00012710: 3e0a 0a20 2020 2020 2020 2020 2020 2020  >..             
-00012720: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-00012730: 212d 2d20 4365 6e74 6572 206d 6964 2d62  !-- Center mid-b
-00012740: 6f74 746f 6d20 2d2d 3e0a 2020 2020 2020  ottom -->.      
-00012750: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012760: 2020 2020 2020 7b25 2069 6620 335f 6365        {% if 3_ce
-00012770: 6e74 6572 5f6d 6964 5f62 6f74 746f 6d5f  nter_mid_bottom_
-00012780: 6120 6f72 2033 5f63 656e 7465 725f 6d69  a or 3_center_mi
-00012790: 645f 626f 7474 6f6d 5f62 206f 7220 335f  d_bottom_b or 3_
-000127a0: 6365 6e74 6572 5f6d 6964 5f62 6f74 746f  center_mid_botto
-000127b0: 6d5f 6320 257d 0a20 2020 2020 2020 2020  m_c %}.         
-000127c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000127d0: 2020 203c 6469 7620 636c 6173 733d 2272     <div class="r
-000127e0: 6f77 223e 0a20 2020 2020 2020 2020 2020  ow">.           
-000127f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012800: 2020 2020 207b 2520 6966 2033 5f63 656e       {% if 3_cen
-00012810: 7465 725f 6d69 645f 626f 7474 6f6d 5f61  ter_mid_bottom_a
-00012820: 2061 6e64 2033 5f63 656e 7465 725f 6d69   and 3_center_mi
-00012830: 645f 626f 7474 6f6d 5f62 2061 6e64 2033  d_bottom_b and 3
-00012840: 5f63 656e 7465 725f 6d69 645f 626f 7474  _center_mid_bott
-00012850: 6f6d 5f63 2025 7d0a 2020 2020 2020 2020  om_c %}.        
-00012860: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012870: 2020 2020 2020 2020 2020 2020 3c64 6976              <div
-00012880: 2063 6c61 7373 3d22 7b25 2062 6c6f 636b   class="{% block
-00012890: 2033 5f63 656e 7465 725f 6d69 645f 626f   3_center_mid_bo
-000128a0: 7474 6f6d 5f61 6263 5f61 2025 7d63 6f6c  ttom_abc_a %}col
-000128b0: 2d31 3220 636f 6c2d 6d64 2d34 7b25 2065  -12 col-md-4{% e
-000128c0: 6e64 626c 6f63 6b20 257d 223e 7b7b 2033  ndblock %}">{{ 3
-000128d0: 5f63 656e 7465 725f 6d69 645f 626f 7474  _center_mid_bott
-000128e0: 6f6d 5f61 207d 7d3c 2f64 6976 3e0a 2020  om_a }}</div>.  
-000128f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012900: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012910: 2020 3c64 6976 2063 6c61 7373 3d22 7b25    <div class="{%
-00012920: 2062 6c6f 636b 2033 5f63 656e 7465 725f   block 3_center_
-00012930: 6d69 645f 626f 7474 6f6d 5f61 6263 5f62  mid_bottom_abc_b
-00012940: 2025 7d63 6f6c 2d31 3220 636f 6c2d 6d64   %}col-12 col-md
-00012950: 2d34 7b25 2065 6e64 626c 6f63 6b20 257d  -4{% endblock %}
-00012960: 223e 7b7b 2033 5f63 656e 7465 725f 6d69  ">{{ 3_center_mi
-00012970: 645f 626f 7474 6f6d 5f62 207d 7d3c 2f64  d_bottom_b }}</d
-00012980: 6976 3e0a 2020 2020 2020 2020 2020 2020  iv>.            
-00012990: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000129a0: 2020 2020 2020 2020 3c64 6976 2063 6c61          <div cla
-000129b0: 7373 3d22 7b25 2062 6c6f 636b 2033 5f63  ss="{% block 3_c
-000129c0: 656e 7465 725f 6d69 645f 626f 7474 6f6d  enter_mid_bottom
-000129d0: 5f61 6263 5f63 2025 7d63 6f6c 2d31 3220  _abc_c %}col-12 
-000129e0: 636f 6c2d 6d64 2d34 7b25 2065 6e64 626c  col-md-4{% endbl
-000129f0: 6f63 6b20 257d 223e 7b7b 2033 5f63 656e  ock %}">{{ 3_cen
-00012a00: 7465 725f 6d69 645f 626f 7474 6f6d 5f63  ter_mid_bottom_c
-00012a10: 207d 7d3c 2f64 6976 3e0a 2020 2020 2020   }}</div>.      
-00012a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012a30: 2020 2020 2020 2020 2020 7b25 2065 6c69            {% eli
-00012a40: 6620 335f 6365 6e74 6572 5f6d 6964 5f62  f 3_center_mid_b
-00012a50: 6f74 746f 6d5f 6120 616e 6420 335f 6365  ottom_a and 3_ce
-00012a60: 6e74 6572 5f6d 6964 5f62 6f74 746f 6d5f  nter_mid_bottom_
-00012a70: 6220 257d 0a20 2020 2020 2020 2020 2020  b %}.           
-00012a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012a90: 2020 2020 2020 2020 203c 6469 7620 636c           <div cl
-00012aa0: 6173 733d 227b 2520 626c 6f63 6b20 335f  ass="{% block 3_
-00012ab0: 6365 6e74 6572 5f6d 6964 5f62 6f74 746f  center_mid_botto
-00012ac0: 6d5f 6162 5f61 2025 7d63 6f6c 2d31 3220  m_ab_a %}col-12 
-00012ad0: 636f 6c2d 6d64 2d38 7b25 2065 6e64 626c  col-md-8{% endbl
-00012ae0: 6f63 6b20 257d 223e 7b7b 2033 5f63 656e  ock %}">{{ 3_cen
-00012af0: 7465 725f 6d69 645f 626f 7474 6f6d 5f61  ter_mid_bottom_a
-00012b00: 207d 7d3c 2f64 6976 3e0a 2020 2020 2020   }}</div>.      
-00012b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012b20: 2020 2020 2020 2020 2020 2020 2020 3c64                <d
-00012b30: 6976 2063 6c61 7373 3d22 7b25 2062 6c6f  iv class="{% blo
-00012b40: 636b 2033 5f63 656e 7465 725f 6d69 645f  ck 3_center_mid_
-00012b50: 626f 7474 6f6d 5f61 625f 6220 257d 636f  bottom_ab_b %}co
-00012b60: 6c2d 3132 2063 6f6c 2d6d 642d 347b 2520  l-12 col-md-4{% 
-00012b70: 656e 6462 6c6f 636b 2025 7d22 3e7b 7b20  endblock %}">{{ 
-00012b80: 335f 6365 6e74 6572 5f6d 6964 5f62 6f74  3_center_mid_bot
-00012b90: 746f 6d5f 6220 7d7d 3c2f 6469 763e 0a20  tom_b }}</div>. 
-00012ba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012bb0: 2020 2020 2020 2020 2020 2020 2020 207b                 {
-00012bc0: 2520 656c 6966 2033 5f63 656e 7465 725f  % elif 3_center_
-00012bd0: 6d69 645f 626f 7474 6f6d 5f61 2061 6e64  mid_bottom_a and
-00012be0: 2033 5f63 656e 7465 725f 6d69 645f 626f   3_center_mid_bo
-00012bf0: 7474 6f6d 5f63 2025 7d0a 2020 2020 2020  ttom_c %}.      
-00012c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012c10: 2020 2020 2020 2020 2020 2020 2020 3c64                <d
-00012c20: 6976 2063 6c61 7373 3d22 7b25 2062 6c6f  iv class="{% blo
-00012c30: 636b 2033 5f63 656e 7465 725f 6d69 645f  ck 3_center_mid_
-00012c40: 626f 7474 6f6d 5f61 635f 6120 257d 636f  bottom_ac_a %}co
-00012c50: 6c2d 3132 2063 6f6c 2d6d 642d 367b 2520  l-12 col-md-6{% 
-00012c60: 656e 6462 6c6f 636b 2025 7d22 3e7b 7b20  endblock %}">{{ 
-00012c70: 335f 6365 6e74 6572 5f6d 6964 5f62 6f74  3_center_mid_bot
-00012c80: 746f 6d5f 6120 7d7d 3c2f 6469 763e 0a20  tom_a }}</div>. 
-00012c90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012ca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012cb0: 2020 203c 6469 7620 636c 6173 733d 227b     <div class="{
-00012cc0: 2520 626c 6f63 6b20 335f 6365 6e74 6572  % block 3_center
-00012cd0: 5f6d 6964 5f62 6f74 746f 6d5f 6163 5f63  _mid_bottom_ac_c
-00012ce0: 2025 7d63 6f6c 2d31 3220 636f 6c2d 6d64   %}col-12 col-md
-00012cf0: 2d36 7b25 2065 6e64 626c 6f63 6b20 257d  -6{% endblock %}
-00012d00: 223e 7b7b 2033 5f63 656e 7465 725f 6d69  ">{{ 3_center_mi
-00012d10: 645f 626f 7474 6f6d 5f63 207d 7d3c 2f64  d_bottom_c }}</d
-00012d20: 6976 3e0a 2020 2020 2020 2020 2020 2020  iv>.            
-00012d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012d40: 2020 2020 7b25 2065 6c69 6620 335f 6365      {% elif 3_ce
-00012d50: 6e74 6572 5f6d 6964 5f62 6f74 746f 6d5f  nter_mid_bottom_
-00012d60: 6220 616e 6420 335f 6365 6e74 6572 5f6d  b and 3_center_m
-00012d70: 6964 5f62 6f74 746f 6d5f 6320 257d 0a20  id_bottom_c %}. 
-00012d80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000126a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000126b0: 7b25 2065 6c69 6620 335f 6365 6e74 6572  {% elif 3_center
+000126c0: 5f6d 6964 5f74 6f70 5f62 2061 6e64 2033  _mid_top_b and 3
+000126d0: 5f63 656e 7465 725f 6d69 645f 746f 705f  _center_mid_top_
+000126e0: 6320 257d 0a20 2020 2020 2020 2020 2020  c %}.           
+000126f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012700: 2020 2020 2020 2020 203c 6469 7620 636c           <div cl
+00012710: 6173 733d 227b 2520 626c 6f63 6b20 335f  ass="{% block 3_
+00012720: 6365 6e74 6572 5f6d 6964 5f74 6f70 5f62  center_mid_top_b
+00012730: 635f 6220 257d 636f 6c2d 3132 2063 6f6c  c_b %}col-12 col
+00012740: 2d6d 642d 347b 2520 656e 6462 6c6f 636b  -md-4{% endblock
+00012750: 2025 7d22 3e7b 7b20 335f 6365 6e74 6572   %}">{{ 3_center
+00012760: 5f6d 6964 5f74 6f70 5f62 207d 7d3c 2f64  _mid_top_b }}</d
+00012770: 6976 3e0a 2020 2020 2020 2020 2020 2020  iv>.            
+00012780: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012790: 2020 2020 2020 2020 3c64 6976 2063 6c61          <div cla
+000127a0: 7373 3d22 7b25 2062 6c6f 636b 2033 5f63  ss="{% block 3_c
+000127b0: 656e 7465 725f 6d69 645f 746f 705f 6263  enter_mid_top_bc
+000127c0: 5f63 2025 7d63 6f6c 2d31 3220 636f 6c2d  _c %}col-12 col-
+000127d0: 6d64 2d38 7b25 2065 6e64 626c 6f63 6b20  md-8{% endblock 
+000127e0: 257d 223e 7b7b 2033 5f63 656e 7465 725f  %}">{{ 3_center_
+000127f0: 6d69 645f 746f 705f 6320 7d7d 3c2f 6469  mid_top_c }}</di
+00012800: 763e 0a20 2020 2020 2020 2020 2020 2020  v>.             
+00012810: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012820: 2020 207b 2520 656c 7365 2025 7d0a 2020     {% else %}.  
+00012830: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012840: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012850: 2020 3c64 6976 2063 6c61 7373 3d22 636f    <div class="co
+00012860: 6c2d 3132 223e 7b7b 2033 5f63 656e 7465  l-12">{{ 3_cente
+00012870: 725f 6d69 645f 746f 705f 6120 7d7d 7b7b  r_mid_top_a }}{{
+00012880: 2033 5f63 656e 7465 725f 6d69 645f 746f   3_center_mid_to
+00012890: 705f 6220 7d7d 7b7b 2033 5f63 656e 7465  p_b }}{{ 3_cente
+000128a0: 725f 6d69 645f 746f 705f 6320 7d7d 3c2f  r_mid_top_c }}</
+000128b0: 6469 763e 0a20 2020 2020 2020 2020 2020  div>.           
+000128c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000128d0: 2020 2020 207b 2520 656e 6469 6620 257d       {% endif %}
+000128e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000128f0: 2020 2020 2020 2020 2020 2020 203c 2f64               </d
+00012900: 6976 3e0a 2020 2020 2020 2020 2020 2020  iv>.            
+00012910: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012920: 7b25 2065 6e64 6966 2025 7d0a 2020 2020  {% endif %}.    
+00012930: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012940: 2020 2020 2020 2020 3c21 2d2d 2045 4e44          <!-- END
+00012950: 2043 656e 7465 7220 6d69 642d 746f 7020   Center mid-top 
+00012960: 2d2d 3e0a 0a20 2020 2020 2020 2020 2020  -->..           
+00012970: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012980: 203c 212d 2d20 4365 6e74 6572 2063 6f6e   <!-- Center con
+00012990: 7465 6e74 202d 2d3e 0a20 2020 2020 2020  tent -->.       
+000129a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000129b0: 2020 2020 207b 2520 6966 2033 5f63 656e       {% if 3_cen
+000129c0: 7465 725f 636f 6e74 656e 7420 257d 0a20  ter_content %}. 
+000129d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000129e0: 2020 2020 2020 2020 2020 203c 6469 7620             <div 
+000129f0: 636c 6173 733d 2272 6f77 223e 0a20 2020  class="row">.   
+00012a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012a10: 2020 2020 2020 2020 2020 2020 203c 6469               <di
+00012a20: 7620 636c 6173 733d 2263 6f6c 223e 0a20  v class="col">. 
+00012a30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012a50: 2020 207b 7b20 335f 6365 6e74 6572 5f63     {{ 3_center_c
+00012a60: 6f6e 7465 6e74 207d 7d0a 2020 2020 2020  ontent }}.      
+00012a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012a80: 2020 2020 2020 2020 2020 3c2f 6469 763e            </div>
+00012a90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00012aa0: 2020 2020 2020 2020 2020 2020 203c 2f64               </d
+00012ab0: 6976 3e0a 2020 2020 2020 2020 2020 2020  iv>.            
+00012ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012ad0: 7b25 2065 6e64 6966 2025 7d0a 2020 2020  {% endif %}.    
+00012ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012af0: 2020 2020 2020 2020 3c21 2d2d 2045 4e44          <!-- END
+00012b00: 2043 656e 7465 7220 636f 6e74 656e 7420   Center content 
+00012b10: 2d2d 3e0a 0a20 2020 2020 2020 2020 2020  -->..           
+00012b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012b30: 203c 212d 2d20 4365 6e74 6572 206d 6964   <!-- Center mid
+00012b40: 2d62 6f74 746f 6d20 2d2d 3e0a 2020 2020  -bottom -->.    
+00012b50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012b60: 2020 2020 2020 2020 7b25 2069 6620 335f          {% if 3_
+00012b70: 6365 6e74 6572 5f6d 6964 5f62 6f74 746f  center_mid_botto
+00012b80: 6d5f 6120 6f72 2033 5f63 656e 7465 725f  m_a or 3_center_
+00012b90: 6d69 645f 626f 7474 6f6d 5f62 206f 7220  mid_bottom_b or 
+00012ba0: 335f 6365 6e74 6572 5f6d 6964 5f62 6f74  3_center_mid_bot
+00012bb0: 746f 6d5f 6320 257d 0a20 2020 2020 2020  tom_c %}.       
+00012bc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012bd0: 2020 2020 203c 6469 7620 636c 6173 733d       <div class=
+00012be0: 2272 6f77 223e 0a20 2020 2020 2020 2020  "row">.         
+00012bf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012c00: 2020 2020 2020 207b 2520 6966 2033 5f63         {% if 3_c
+00012c10: 656e 7465 725f 6d69 645f 626f 7474 6f6d  enter_mid_bottom
+00012c20: 5f61 2061 6e64 2033 5f63 656e 7465 725f  _a and 3_center_
+00012c30: 6d69 645f 626f 7474 6f6d 5f62 2061 6e64  mid_bottom_b and
+00012c40: 2033 5f63 656e 7465 725f 6d69 645f 626f   3_center_mid_bo
+00012c50: 7474 6f6d 5f63 2025 7d0a 2020 2020 2020  ttom_c %}.      
+00012c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012c70: 2020 2020 2020 2020 2020 2020 2020 3c64                <d
+00012c80: 6976 2063 6c61 7373 3d22 7b25 2062 6c6f  iv class="{% blo
+00012c90: 636b 2033 5f63 656e 7465 725f 6d69 645f  ck 3_center_mid_
+00012ca0: 626f 7474 6f6d 5f61 6263 5f61 2025 7d63  bottom_abc_a %}c
+00012cb0: 6f6c 2d31 3220 636f 6c2d 6d64 2d34 7b25  ol-12 col-md-4{%
+00012cc0: 2065 6e64 626c 6f63 6b20 257d 223e 7b7b   endblock %}">{{
+00012cd0: 2033 5f63 656e 7465 725f 6d69 645f 626f   3_center_mid_bo
+00012ce0: 7474 6f6d 5f61 207d 7d3c 2f64 6976 3e0a  ttom_a }}</div>.
+00012cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012d10: 2020 2020 3c64 6976 2063 6c61 7373 3d22      <div class="
+00012d20: 7b25 2062 6c6f 636b 2033 5f63 656e 7465  {% block 3_cente
+00012d30: 725f 6d69 645f 626f 7474 6f6d 5f61 6263  r_mid_bottom_abc
+00012d40: 5f62 2025 7d63 6f6c 2d31 3220 636f 6c2d  _b %}col-12 col-
+00012d50: 6d64 2d34 7b25 2065 6e64 626c 6f63 6b20  md-4{% endblock 
+00012d60: 257d 223e 7b7b 2033 5f63 656e 7465 725f  %}">{{ 3_center_
+00012d70: 6d69 645f 626f 7474 6f6d 5f62 207d 7d3c  mid_bottom_b }}<
+00012d80: 2f64 6976 3e0a 2020 2020 2020 2020 2020  /div>.          
 00012d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012da0: 2020 203c 6469 7620 636c 6173 733d 227b     <div class="{
-00012db0: 2520 626c 6f63 6b20 335f 6365 6e74 6572  % block 3_center
-00012dc0: 5f6d 6964 5f62 6f74 746f 6d5f 6263 5f62  _mid_bottom_bc_b
-00012dd0: 2025 7d63 6f6c 2d31 3220 636f 6c2d 6d64   %}col-12 col-md
-00012de0: 2d34 7b25 2065 6e64 626c 6f63 6b20 257d  -4{% endblock %}
-00012df0: 223e 7b7b 2033 5f63 656e 7465 725f 6d69  ">{{ 3_center_mi
-00012e00: 645f 626f 7474 6f6d 5f62 207d 7d3c 2f64  d_bottom_b }}</d
-00012e10: 6976 3e0a 2020 2020 2020 2020 2020 2020  iv>.            
+00012da0: 2020 2020 2020 2020 2020 3c64 6976 2063            <div c
+00012db0: 6c61 7373 3d22 7b25 2062 6c6f 636b 2033  lass="{% block 3
+00012dc0: 5f63 656e 7465 725f 6d69 645f 626f 7474  _center_mid_bott
+00012dd0: 6f6d 5f61 6263 5f63 2025 7d63 6f6c 2d31  om_abc_c %}col-1
+00012de0: 3220 636f 6c2d 6d64 2d34 7b25 2065 6e64  2 col-md-4{% end
+00012df0: 626c 6f63 6b20 257d 223e 7b7b 2033 5f63  block %}">{{ 3_c
+00012e00: 656e 7465 725f 6d69 645f 626f 7474 6f6d  enter_mid_bottom
+00012e10: 5f63 207d 7d3c 2f64 6976 3e0a 2020 2020  _c }}</div>.    
 00012e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012e30: 2020 2020 2020 2020 3c64 6976 2063 6c61          <div cla
-00012e40: 7373 3d22 7b25 2062 6c6f 636b 2033 5f63  ss="{% block 3_c
-00012e50: 656e 7465 725f 6d69 645f 626f 7474 6f6d  enter_mid_bottom
-00012e60: 5f62 635f 6320 257d 636f 6c2d 3132 2063  _bc_c %}col-12 c
-00012e70: 6f6c 2d6d 642d 387b 2520 656e 6462 6c6f  ol-md-8{% endblo
-00012e80: 636b 2025 7d22 3e7b 7b20 335f 6365 6e74  ck %}">{{ 3_cent
-00012e90: 6572 5f6d 6964 5f62 6f74 746f 6d5f 6320  er_mid_bottom_c 
-00012ea0: 7d7d 3c2f 6469 763e 0a20 2020 2020 2020  }}</div>.       
-00012eb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012ec0: 2020 2020 2020 2020 207b 2520 656c 7365           {% else
-00012ed0: 2025 7d0a 2020 2020 2020 2020 2020 2020   %}.            
-00012ee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012ef0: 2020 2020 2020 2020 3c64 6976 2063 6c61          <div cla
-00012f00: 7373 3d22 636f 6c2d 3132 223e 7b7b 2033  ss="col-12">{{ 3
-00012f10: 5f63 656e 7465 725f 6d69 645f 626f 7474  _center_mid_bott
-00012f20: 6f6d 5f61 207d 7d7b 7b20 335f 6365 6e74  om_a }}{{ 3_cent
-00012f30: 6572 5f6d 6964 5f62 6f74 746f 6d5f 6220  er_mid_bottom_b 
-00012f40: 7d7d 7b7b 2033 5f63 656e 7465 725f 6d69  }}{{ 3_center_mi
-00012f50: 645f 626f 7474 6f6d 5f63 207d 7d3c 2f64  d_bottom_c }}</d
-00012f60: 6976 3e0a 2020 2020 2020 2020 2020 2020  iv>.            
-00012f70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012f80: 2020 2020 7b25 2065 6e64 6966 2025 7d0a      {% endif %}.
-00012f90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012fa0: 2020 2020 2020 2020 2020 2020 3c2f 6469              </di
-00012fb0: 763e 0a20 2020 2020 2020 2020 2020 2020  v>.             
-00012fc0: 2020 2020 2020 2020 2020 2020 2020 207b                 {
-00012fd0: 2520 656e 6469 6620 257d 0a20 2020 2020  % endif %}.     
-00012fe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012ff0: 2020 2020 2020 203c 212d 2d20 454e 4420         <!-- END 
-00013000: 4365 6e74 6572 206d 6964 2d62 6f74 746f  Center mid-botto
-00013010: 6d20 2d2d 3e0a 0a20 2020 2020 2020 2020  m -->..         
-00013020: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013030: 2020 203c 212d 2d20 4365 6e74 6572 2062     <!-- Center b
-00013040: 6f74 746f 6d20 2d2d 3e0a 2020 2020 2020  ottom -->.      
-00013050: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013060: 2020 2020 2020 7b25 2069 6620 335f 6365        {% if 3_ce
-00013070: 6e74 6572 5f62 6f74 746f 6d5f 6120 6f72  nter_bottom_a or
-00013080: 2033 5f63 656e 7465 725f 626f 7474 6f6d   3_center_bottom
-00013090: 5f62 206f 7220 335f 6365 6e74 6572 5f62  _b or 3_center_b
-000130a0: 6f74 746f 6d5f 6320 257d 0a20 2020 2020  ottom_c %}.     
-000130b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000130c0: 2020 2020 2020 203c 6469 7620 636c 6173         <div clas
-000130d0: 733d 2272 6f77 223e 0a20 2020 2020 2020  s="row">.       
-000130e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000130f0: 2020 2020 2020 2020 207b 2520 6966 2033           {% if 3
-00013100: 5f63 656e 7465 725f 626f 7474 6f6d 5f61  _center_bottom_a
-00013110: 2061 6e64 2033 5f63 656e 7465 725f 626f   and 3_center_bo
-00013120: 7474 6f6d 5f62 2061 6e64 2033 5f63 656e  ttom_b and 3_cen
-00013130: 7465 725f 626f 7474 6f6d 5f63 2025 7d0a  ter_bottom_c %}.
-00013140: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013150: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013160: 2020 2020 3c64 6976 2063 6c61 7373 3d22      <div class="
-00013170: 7b25 2062 6c6f 636b 2033 5f63 656e 7465  {% block 3_cente
-00013180: 725f 626f 7474 6f6d 5f61 6263 5f61 2025  r_bottom_abc_a %
-00013190: 7d63 6f6c 2d31 3220 636f 6c2d 6d64 2d34  }col-12 col-md-4
-000131a0: 7b25 2065 6e64 626c 6f63 6b20 257d 223e  {% endblock %}">
-000131b0: 7b7b 2033 5f63 656e 7465 725f 626f 7474  {{ 3_center_bott
-000131c0: 6f6d 5f61 207d 7d3c 2f64 6976 3e0a 2020  om_a }}</div>.  
-000131d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000131e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000131f0: 2020 3c64 6976 2063 6c61 7373 3d22 7b25    <div class="{%
-00013200: 2062 6c6f 636b 2033 5f63 656e 7465 725f   block 3_center_
-00013210: 626f 7474 6f6d 5f61 6263 5f62 2025 7d63  bottom_abc_b %}c
-00013220: 6f6c 2d31 3220 636f 6c2d 6d64 2d34 7b25  ol-12 col-md-4{%
-00013230: 2065 6e64 626c 6f63 6b20 257d 223e 7b7b   endblock %}">{{
-00013240: 2033 5f63 656e 7465 725f 626f 7474 6f6d   3_center_bottom
-00013250: 5f62 207d 7d3c 2f64 6976 3e0a 2020 2020  _b }}</div>.    
-00013260: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013270: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013280: 3c64 6976 2063 6c61 7373 3d22 7b25 2062  <div class="{% b
-00013290: 6c6f 636b 2033 5f63 656e 7465 725f 626f  lock 3_center_bo
-000132a0: 7474 6f6d 5f61 6263 5f63 2025 7d63 6f6c  ttom_abc_c %}col
-000132b0: 2d31 3220 636f 6c2d 6d64 2d34 7b25 2065  -12 col-md-4{% e
-000132c0: 6e64 626c 6f63 6b20 257d 223e 7b7b 2033  ndblock %}">{{ 3
-000132d0: 5f63 656e 7465 725f 626f 7474 6f6d 5f63  _center_bottom_c
-000132e0: 207d 7d3c 2f64 6976 3e0a 2020 2020 2020   }}</div>.      
-000132f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013300: 2020 2020 2020 2020 2020 7b25 2065 6c69            {% eli
-00013310: 6620 335f 6365 6e74 6572 5f62 6f74 746f  f 3_center_botto
-00013320: 6d5f 6120 616e 6420 335f 6365 6e74 6572  m_a and 3_center
-00013330: 5f62 6f74 746f 6d5f 6220 257d 0a20 2020  _bottom_b %}.   
-00013340: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013350: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013360: 203c 6469 7620 636c 6173 733d 227b 2520   <div class="{% 
-00013370: 626c 6f63 6b20 335f 6365 6e74 6572 5f62  block 3_center_b
-00013380: 6f74 746f 6d5f 6162 5f61 2025 7d63 6f6c  ottom_ab_a %}col
-00013390: 2d31 3220 636f 6c2d 6d64 2d38 7b25 2065  -12 col-md-8{% e
-000133a0: 6e64 626c 6f63 6b20 257d 223e 7b7b 2033  ndblock %}">{{ 3
-000133b0: 5f63 656e 7465 725f 626f 7474 6f6d 5f61  _center_bottom_a
-000133c0: 207d 7d3c 2f64 6976 3e0a 2020 2020 2020   }}</div>.      
-000133d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000133e0: 2020 2020 2020 2020 2020 2020 2020 3c64                <d
-000133f0: 6976 2063 6c61 7373 3d22 7b25 2062 6c6f  iv class="{% blo
-00013400: 636b 2033 5f63 656e 7465 725f 626f 7474  ck 3_center_bott
-00013410: 6f6d 5f61 625f 6220 257d 636f 6c2d 3132  om_ab_b %}col-12
-00013420: 2063 6f6c 2d6d 642d 347b 2520 656e 6462   col-md-4{% endb
-00013430: 6c6f 636b 2025 7d22 3e7b 7b20 335f 6365  lock %}">{{ 3_ce
-00013440: 6e74 6572 5f62 6f74 746f 6d5f 6220 7d7d  nter_bottom_b }}
-00013450: 3c2f 6469 763e 0a20 2020 2020 2020 2020  </div>.         
-00013460: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013470: 2020 2020 2020 207b 2520 656c 6966 2033         {% elif 3
-00013480: 5f63 656e 7465 725f 626f 7474 6f6d 5f61  _center_bottom_a
-00013490: 2061 6e64 2033 5f63 656e 7465 725f 626f   and 3_center_bo
-000134a0: 7474 6f6d 5f63 2025 7d0a 2020 2020 2020  ttom_c %}.      
+00012e30: 2020 2020 2020 2020 2020 2020 7b25 2065              {% e
+00012e40: 6c69 6620 335f 6365 6e74 6572 5f6d 6964  lif 3_center_mid
+00012e50: 5f62 6f74 746f 6d5f 6120 616e 6420 335f  _bottom_a and 3_
+00012e60: 6365 6e74 6572 5f6d 6964 5f62 6f74 746f  center_mid_botto
+00012e70: 6d5f 6220 257d 0a20 2020 2020 2020 2020  m_b %}.         
+00012e80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012e90: 2020 2020 2020 2020 2020 203c 6469 7620             <div 
+00012ea0: 636c 6173 733d 227b 2520 626c 6f63 6b20  class="{% block 
+00012eb0: 335f 6365 6e74 6572 5f6d 6964 5f62 6f74  3_center_mid_bot
+00012ec0: 746f 6d5f 6162 5f61 2025 7d63 6f6c 2d31  tom_ab_a %}col-1
+00012ed0: 3220 636f 6c2d 6d64 2d38 7b25 2065 6e64  2 col-md-8{% end
+00012ee0: 626c 6f63 6b20 257d 223e 7b7b 2033 5f63  block %}">{{ 3_c
+00012ef0: 656e 7465 725f 6d69 645f 626f 7474 6f6d  enter_mid_bottom
+00012f00: 5f61 207d 7d3c 2f64 6976 3e0a 2020 2020  _a }}</div>.    
+00012f10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012f30: 3c64 6976 2063 6c61 7373 3d22 7b25 2062  <div class="{% b
+00012f40: 6c6f 636b 2033 5f63 656e 7465 725f 6d69  lock 3_center_mi
+00012f50: 645f 626f 7474 6f6d 5f61 625f 6220 257d  d_bottom_ab_b %}
+00012f60: 636f 6c2d 3132 2063 6f6c 2d6d 642d 347b  col-12 col-md-4{
+00012f70: 2520 656e 6462 6c6f 636b 2025 7d22 3e7b  % endblock %}">{
+00012f80: 7b20 335f 6365 6e74 6572 5f6d 6964 5f62  { 3_center_mid_b
+00012f90: 6f74 746f 6d5f 6220 7d7d 3c2f 6469 763e  ottom_b }}</div>
+00012fa0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00012fb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012fc0: 207b 2520 656c 6966 2033 5f63 656e 7465   {% elif 3_cente
+00012fd0: 725f 6d69 645f 626f 7474 6f6d 5f61 2061  r_mid_bottom_a a
+00012fe0: 6e64 2033 5f63 656e 7465 725f 6d69 645f  nd 3_center_mid_
+00012ff0: 626f 7474 6f6d 5f63 2025 7d0a 2020 2020  bottom_c %}.    
+00013000: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013010: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013020: 3c64 6976 2063 6c61 7373 3d22 7b25 2062  <div class="{% b
+00013030: 6c6f 636b 2033 5f63 656e 7465 725f 6d69  lock 3_center_mi
+00013040: 645f 626f 7474 6f6d 5f61 635f 6120 257d  d_bottom_ac_a %}
+00013050: 636f 6c2d 3132 2063 6f6c 2d6d 642d 367b  col-12 col-md-6{
+00013060: 2520 656e 6462 6c6f 636b 2025 7d22 3e7b  % endblock %}">{
+00013070: 7b20 335f 6365 6e74 6572 5f6d 6964 5f62  { 3_center_mid_b
+00013080: 6f74 746f 6d5f 6120 7d7d 3c2f 6469 763e  ottom_a }}</div>
+00013090: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000130a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000130b0: 2020 2020 203c 6469 7620 636c 6173 733d       <div class=
+000130c0: 227b 2520 626c 6f63 6b20 335f 6365 6e74  "{% block 3_cent
+000130d0: 6572 5f6d 6964 5f62 6f74 746f 6d5f 6163  er_mid_bottom_ac
+000130e0: 5f63 2025 7d63 6f6c 2d31 3220 636f 6c2d  _c %}col-12 col-
+000130f0: 6d64 2d36 7b25 2065 6e64 626c 6f63 6b20  md-6{% endblock 
+00013100: 257d 223e 7b7b 2033 5f63 656e 7465 725f  %}">{{ 3_center_
+00013110: 6d69 645f 626f 7474 6f6d 5f63 207d 7d3c  mid_bottom_c }}<
+00013120: 2f64 6976 3e0a 2020 2020 2020 2020 2020  /div>.          
+00013130: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013140: 2020 2020 2020 7b25 2065 6c69 6620 335f        {% elif 3_
+00013150: 6365 6e74 6572 5f6d 6964 5f62 6f74 746f  center_mid_botto
+00013160: 6d5f 6220 616e 6420 335f 6365 6e74 6572  m_b and 3_center
+00013170: 5f6d 6964 5f62 6f74 746f 6d5f 6320 257d  _mid_bottom_c %}
+00013180: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00013190: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000131a0: 2020 2020 203c 6469 7620 636c 6173 733d       <div class=
+000131b0: 227b 2520 626c 6f63 6b20 335f 6365 6e74  "{% block 3_cent
+000131c0: 6572 5f6d 6964 5f62 6f74 746f 6d5f 6263  er_mid_bottom_bc
+000131d0: 5f62 2025 7d63 6f6c 2d31 3220 636f 6c2d  _b %}col-12 col-
+000131e0: 6d64 2d34 7b25 2065 6e64 626c 6f63 6b20  md-4{% endblock 
+000131f0: 257d 223e 7b7b 2033 5f63 656e 7465 725f  %}">{{ 3_center_
+00013200: 6d69 645f 626f 7474 6f6d 5f62 207d 7d3c  mid_bottom_b }}<
+00013210: 2f64 6976 3e0a 2020 2020 2020 2020 2020  /div>.          
+00013220: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013230: 2020 2020 2020 2020 2020 3c64 6976 2063            <div c
+00013240: 6c61 7373 3d22 7b25 2062 6c6f 636b 2033  lass="{% block 3
+00013250: 5f63 656e 7465 725f 6d69 645f 626f 7474  _center_mid_bott
+00013260: 6f6d 5f62 635f 6320 257d 636f 6c2d 3132  om_bc_c %}col-12
+00013270: 2063 6f6c 2d6d 642d 387b 2520 656e 6462   col-md-8{% endb
+00013280: 6c6f 636b 2025 7d22 3e7b 7b20 335f 6365  lock %}">{{ 3_ce
+00013290: 6e74 6572 5f6d 6964 5f62 6f74 746f 6d5f  nter_mid_bottom_
+000132a0: 6320 7d7d 3c2f 6469 763e 0a20 2020 2020  c }}</div>.     
+000132b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000132c0: 2020 2020 2020 2020 2020 207b 2520 656c             {% el
+000132d0: 7365 2025 7d0a 2020 2020 2020 2020 2020  se %}.          
+000132e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000132f0: 2020 2020 2020 2020 2020 3c64 6976 2063            <div c
+00013300: 6c61 7373 3d22 636f 6c2d 3132 223e 7b7b  lass="col-12">{{
+00013310: 2033 5f63 656e 7465 725f 6d69 645f 626f   3_center_mid_bo
+00013320: 7474 6f6d 5f61 207d 7d7b 7b20 335f 6365  ttom_a }}{{ 3_ce
+00013330: 6e74 6572 5f6d 6964 5f62 6f74 746f 6d5f  nter_mid_bottom_
+00013340: 6220 7d7d 7b7b 2033 5f63 656e 7465 725f  b }}{{ 3_center_
+00013350: 6d69 645f 626f 7474 6f6d 5f63 207d 7d3c  mid_bottom_c }}<
+00013360: 2f64 6976 3e0a 2020 2020 2020 2020 2020  /div>.          
+00013370: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013380: 2020 2020 2020 7b25 2065 6e64 6966 2025        {% endif %
+00013390: 7d0a 2020 2020 2020 2020 2020 2020 2020  }.              
+000133a0: 2020 2020 2020 2020 2020 2020 2020 3c2f                </
+000133b0: 6469 763e 0a20 2020 2020 2020 2020 2020  div>.           
+000133c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000133d0: 207b 2520 656e 6469 6620 257d 0a20 2020   {% endif %}.   
+000133e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000133f0: 2020 2020 2020 2020 203c 212d 2d20 454e           <!-- EN
+00013400: 4420 4365 6e74 6572 206d 6964 2d62 6f74  D Center mid-bot
+00013410: 746f 6d20 2d2d 3e0a 0a20 2020 2020 2020  tom -->..       
+00013420: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013430: 2020 2020 203c 212d 2d20 4365 6e74 6572       <!-- Center
+00013440: 2062 6f74 746f 6d20 2d2d 3e0a 2020 2020   bottom -->.    
+00013450: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013460: 2020 2020 2020 2020 7b25 2069 6620 335f          {% if 3_
+00013470: 6365 6e74 6572 5f62 6f74 746f 6d5f 6120  center_bottom_a 
+00013480: 6f72 2033 5f63 656e 7465 725f 626f 7474  or 3_center_bott
+00013490: 6f6d 5f62 206f 7220 335f 6365 6e74 6572  om_b or 3_center
+000134a0: 5f62 6f74 746f 6d5f 6320 257d 0a20 2020  _bottom_c %}.   
 000134b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000134c0: 2020 2020 2020 2020 2020 2020 2020 3c64                <d
-000134d0: 6976 2063 6c61 7373 3d22 7b25 2062 6c6f  iv class="{% blo
-000134e0: 636b 2033 5f63 656e 7465 725f 626f 7474  ck 3_center_bott
-000134f0: 6f6d 5f61 635f 6120 257d 636f 6c2d 3132  om_ac_a %}col-12
-00013500: 2063 6f6c 2d6d 642d 367b 2520 656e 6462   col-md-6{% endb
-00013510: 6c6f 636b 2025 7d22 3e7b 7b20 335f 6365  lock %}">{{ 3_ce
-00013520: 6e74 6572 5f62 6f74 746f 6d5f 6120 7d7d  nter_bottom_a }}
-00013530: 3c2f 6469 763e 0a20 2020 2020 2020 2020  </div>.         
-00013540: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013550: 2020 2020 2020 2020 2020 203c 6469 7620             <div 
-00013560: 636c 6173 733d 227b 2520 626c 6f63 6b20  class="{% block 
-00013570: 335f 6365 6e74 6572 5f62 6f74 746f 6d5f  3_center_bottom_
-00013580: 6163 5f63 2025 7d63 6f6c 2d31 3220 636f  ac_c %}col-12 co
-00013590: 6c2d 6d64 2d36 7b25 2065 6e64 626c 6f63  l-md-6{% endbloc
-000135a0: 6b20 257d 223e 7b7b 2033 5f63 656e 7465  k %}">{{ 3_cente
-000135b0: 725f 626f 7474 6f6d 5f63 207d 7d3c 2f64  r_bottom_c }}</d
-000135c0: 6976 3e0a 2020 2020 2020 2020 2020 2020  iv>.            
+000134c0: 2020 2020 2020 2020 203c 6469 7620 636c           <div cl
+000134d0: 6173 733d 2272 6f77 223e 0a20 2020 2020  ass="row">.     
+000134e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000134f0: 2020 2020 2020 2020 2020 207b 2520 6966             {% if
+00013500: 2033 5f63 656e 7465 725f 626f 7474 6f6d   3_center_bottom
+00013510: 5f61 2061 6e64 2033 5f63 656e 7465 725f  _a and 3_center_
+00013520: 626f 7474 6f6d 5f62 2061 6e64 2033 5f63  bottom_b and 3_c
+00013530: 656e 7465 725f 626f 7474 6f6d 5f63 2025  enter_bottom_c %
+00013540: 7d0a 2020 2020 2020 2020 2020 2020 2020  }.              
+00013550: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013560: 2020 2020 2020 3c64 6976 2063 6c61 7373        <div class
+00013570: 3d22 7b25 2062 6c6f 636b 2033 5f63 656e  ="{% block 3_cen
+00013580: 7465 725f 626f 7474 6f6d 5f61 6263 5f61  ter_bottom_abc_a
+00013590: 2025 7d63 6f6c 2d31 3220 636f 6c2d 6d64   %}col-12 col-md
+000135a0: 2d34 7b25 2065 6e64 626c 6f63 6b20 257d  -4{% endblock %}
+000135b0: 223e 7b7b 2033 5f63 656e 7465 725f 626f  ">{{ 3_center_bo
+000135c0: 7474 6f6d 5f61 207d 7d3c 2f64 6976 3e0a  ttom_a }}</div>.
 000135d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000135e0: 2020 2020 7b25 2065 6c69 6620 335f 6365      {% elif 3_ce
-000135f0: 6e74 6572 5f62 6f74 746f 6d5f 6220 616e  nter_bottom_b an
-00013600: 6420 335f 6365 6e74 6572 5f62 6f74 746f  d 3_center_botto
-00013610: 6d5f 6320 257d 0a20 2020 2020 2020 2020  m_c %}.         
-00013620: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013630: 2020 2020 2020 2020 2020 203c 6469 7620             <div 
-00013640: 636c 6173 733d 227b 2520 626c 6f63 6b20  class="{% block 
-00013650: 335f 6365 6e74 6572 5f62 6f74 746f 6d5f  3_center_bottom_
-00013660: 6263 5f62 2025 7d63 6f6c 2d31 3220 636f  bc_b %}col-12 co
-00013670: 6c2d 6d64 2d34 7b25 2065 6e64 626c 6f63  l-md-4{% endbloc
-00013680: 6b20 257d 223e 7b7b 2033 5f63 656e 7465  k %}">{{ 3_cente
-00013690: 725f 626f 7474 6f6d 5f62 207d 7d3c 2f64  r_bottom_b }}</d
-000136a0: 6976 3e0a 2020 2020 2020 2020 2020 2020  iv>.            
-000136b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000136c0: 2020 2020 2020 2020 3c64 6976 2063 6c61          <div cla
-000136d0: 7373 3d22 7b25 2062 6c6f 636b 2033 5f63  ss="{% block 3_c
-000136e0: 656e 7465 725f 626f 7474 6f6d 5f62 635f  enter_bottom_bc_
-000136f0: 6320 257d 636f 6c2d 3132 2063 6f6c 2d6d  c %}col-12 col-m
-00013700: 642d 387b 2520 656e 6462 6c6f 636b 2025  d-8{% endblock %
-00013710: 7d22 3e7b 7b20 335f 6365 6e74 6572 5f62  }">{{ 3_center_b
-00013720: 6f74 746f 6d5f 6320 7d7d 3c2f 6469 763e  ottom_c }}</div>
-00013730: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000135e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000135f0: 2020 2020 3c64 6976 2063 6c61 7373 3d22      <div class="
+00013600: 7b25 2062 6c6f 636b 2033 5f63 656e 7465  {% block 3_cente
+00013610: 725f 626f 7474 6f6d 5f61 6263 5f62 2025  r_bottom_abc_b %
+00013620: 7d63 6f6c 2d31 3220 636f 6c2d 6d64 2d34  }col-12 col-md-4
+00013630: 7b25 2065 6e64 626c 6f63 6b20 257d 223e  {% endblock %}">
+00013640: 7b7b 2033 5f63 656e 7465 725f 626f 7474  {{ 3_center_bott
+00013650: 6f6d 5f62 207d 7d3c 2f64 6976 3e0a 2020  om_b }}</div>.  
+00013660: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013670: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013680: 2020 3c64 6976 2063 6c61 7373 3d22 7b25    <div class="{%
+00013690: 2062 6c6f 636b 2033 5f63 656e 7465 725f   block 3_center_
+000136a0: 626f 7474 6f6d 5f61 6263 5f63 2025 7d63  bottom_abc_c %}c
+000136b0: 6f6c 2d31 3220 636f 6c2d 6d64 2d34 7b25  ol-12 col-md-4{%
+000136c0: 2065 6e64 626c 6f63 6b20 257d 223e 7b7b   endblock %}">{{
+000136d0: 2033 5f63 656e 7465 725f 626f 7474 6f6d   3_center_bottom
+000136e0: 5f63 207d 7d3c 2f64 6976 3e0a 2020 2020  _c }}</div>.    
+000136f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013700: 2020 2020 2020 2020 2020 2020 7b25 2065              {% e
+00013710: 6c69 6620 335f 6365 6e74 6572 5f62 6f74  lif 3_center_bot
+00013720: 746f 6d5f 6120 616e 6420 335f 6365 6e74  tom_a and 3_cent
+00013730: 6572 5f62 6f74 746f 6d5f 6220 257d 0a20  er_bottom_b %}. 
 00013740: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013750: 207b 2520 656c 7365 2025 7d0a 2020 2020   {% else %}.    
-00013760: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013770: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013780: 3c64 6976 2063 6c61 7373 3d22 636f 6c2d  <div class="col-
-00013790: 3132 223e 7b7b 2033 5f63 656e 7465 725f  12">{{ 3_center_
-000137a0: 626f 7474 6f6d 5f61 207d 7d7b 7b20 335f  bottom_a }}{{ 3_
-000137b0: 6365 6e74 6572 5f62 6f74 746f 6d5f 6220  center_bottom_b 
-000137c0: 7d7d 7b7b 2033 5f63 656e 7465 725f 626f  }}{{ 3_center_bo
-000137d0: 7474 6f6d 5f63 207d 7d3c 2f64 6976 3e0a  ttom_c }}</div>.
+00013750: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013760: 2020 203c 6469 7620 636c 6173 733d 227b     <div class="{
+00013770: 2520 626c 6f63 6b20 335f 6365 6e74 6572  % block 3_center
+00013780: 5f62 6f74 746f 6d5f 6162 5f61 2025 7d63  _bottom_ab_a %}c
+00013790: 6f6c 2d31 3220 636f 6c2d 6d64 2d38 7b25  ol-12 col-md-8{%
+000137a0: 2065 6e64 626c 6f63 6b20 257d 223e 7b7b   endblock %}">{{
+000137b0: 2033 5f63 656e 7465 725f 626f 7474 6f6d   3_center_bottom
+000137c0: 5f61 207d 7d3c 2f64 6976 3e0a 2020 2020  _a }}</div>.    
+000137d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000137e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000137f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013800: 7b25 2065 6e64 6966 2025 7d0a 2020 2020  {% endif %}.    
-00013810: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013820: 2020 2020 2020 2020 3c2f 6469 763e 0a20          </div>. 
-00013830: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013840: 2020 2020 2020 2020 2020 207b 2520 656e             {% en
-00013850: 6469 6620 257d 0a0a 2020 2020 2020 2020  dif %}..        
+000137f0: 3c64 6976 2063 6c61 7373 3d22 7b25 2062  <div class="{% b
+00013800: 6c6f 636b 2033 5f63 656e 7465 725f 626f  lock 3_center_bo
+00013810: 7474 6f6d 5f61 625f 6220 257d 636f 6c2d  ttom_ab_b %}col-
+00013820: 3132 2063 6f6c 2d6d 642d 347b 2520 656e  12 col-md-4{% en
+00013830: 6462 6c6f 636b 2025 7d22 3e7b 7b20 335f  dblock %}">{{ 3_
+00013840: 6365 6e74 6572 5f62 6f74 746f 6d5f 6220  center_bottom_b 
+00013850: 7d7d 3c2f 6469 763e 0a20 2020 2020 2020  }}</div>.       
 00013860: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013870: 3c2f 6469 763e 0a20 2020 2020 2020 2020  </div>.         
-00013880: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-00013890: 212d 2d20 456e 6420 4365 6e74 6572 2063  !-- End Center c
-000138a0: 6f6c 756d 6e20 2d2d 3e0a 0a20 2020 2020  olumn -->..     
+00013870: 2020 2020 2020 2020 207b 2520 656c 6966           {% elif
+00013880: 2033 5f63 656e 7465 725f 626f 7474 6f6d   3_center_bottom
+00013890: 5f61 2061 6e64 2033 5f63 656e 7465 725f  _a and 3_center_
+000138a0: 626f 7474 6f6d 5f63 2025 7d0a 2020 2020  bottom_c %}.    
 000138b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000138c0: 2020 203c 212d 2d20 4275 696c 6420 7269     <!-- Build ri
-000138d0: 6768 7420 636f 6c75 6d6e 202d 2d3e 0a20  ght column -->. 
-000138e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000138f0: 2020 2020 2020 207b 2520 6966 2033 5f72         {% if 3_r
-00013900: 6967 6874 5f61 206f 7220 335f 7269 6768  ight_a or 3_righ
-00013910: 745f 6220 257d 0a20 2020 2020 2020 2020  t_b %}.         
-00013920: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013930: 2020 207b 2520 6966 2033 5f72 6967 6874     {% if 3_right
-00013940: 5f61 2061 6e64 2033 5f72 6967 6874 5f62  _a and 3_right_b
-00013950: 2025 7d0a 2020 2020 2020 2020 2020 2020   %}.            
-00013960: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013970: 3c64 6976 2063 6c61 7373 3d22 7b25 2062  <div class="{% b
-00013980: 6c6f 636b 2033 5f72 6967 6874 5f61 6220  lock 3_right_ab 
-00013990: 257d 636f 6c2d 3132 2063 6f6c 2d6c 672d  %}col-12 col-lg-
-000139a0: 3420 6d74 2d35 206d 742d 6c67 2d30 7b25  4 mt-5 mt-lg-0{%
-000139b0: 2065 6e64 626c 6f63 6b20 257d 223e 0a20   endblock %}">. 
-000139c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000139d0: 2020 2020 2020 2020 2020 207b 2520 656c             {% el
-000139e0: 6966 2033 5f72 6967 6874 5f61 2025 7d0a  if 3_right_a %}.
-000139f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013a00: 2020 2020 2020 2020 2020 2020 3c64 6976              <div
-00013a10: 2063 6c61 7373 3d22 7b25 2062 6c6f 636b   class="{% block
-00013a20: 2033 5f72 6967 6874 5f61 2025 7d63 6f6c   3_right_a %}col
-00013a30: 2d31 3220 636f 6c2d 6c67 2d33 206d 742d  -12 col-lg-3 mt-
-00013a40: 3520 6d74 2d6c 672d 307b 2520 656e 6462  5 mt-lg-0{% endb
-00013a50: 6c6f 636b 2025 7d22 3e0a 2020 2020 2020  lock %}">.      
-00013a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013a70: 2020 2020 2020 7b25 2065 6c73 6520 257d        {% else %}
-00013a80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00013a90: 2020 2020 2020 2020 2020 2020 203c 6469               <di
-00013aa0: 7620 636c 6173 733d 227b 2520 626c 6f63  v class="{% bloc
-00013ab0: 6b20 335f 7269 6768 745f 6220 257d 636f  k 3_right_b %}co
-00013ac0: 6c2d 3132 2063 6f6c 2d6c 672d 3320 6f66  l-12 col-lg-3 of
-00013ad0: 6673 6574 2d6c 672d 3120 6d74 2d35 206d  fset-lg-1 mt-5 m
-00013ae0: 742d 6c67 2d30 7b25 2065 6e64 626c 6f63  t-lg-0{% endbloc
-00013af0: 6b20 257d 223e 0a20 2020 2020 2020 2020  k %}">.         
-00013b00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013b10: 2020 207b 2520 656e 6469 6620 257d 0a20     {% endif %}. 
-00013b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013b30: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-00013b40: 6469 7620 636c 6173 733d 2272 6f77 223e  div class="row">
-00013b50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000138c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000138d0: 3c64 6976 2063 6c61 7373 3d22 7b25 2062  <div class="{% b
+000138e0: 6c6f 636b 2033 5f63 656e 7465 725f 626f  lock 3_center_bo
+000138f0: 7474 6f6d 5f61 635f 6120 257d 636f 6c2d  ttom_ac_a %}col-
+00013900: 3132 2063 6f6c 2d6d 642d 367b 2520 656e  12 col-md-6{% en
+00013910: 6462 6c6f 636b 2025 7d22 3e7b 7b20 335f  dblock %}">{{ 3_
+00013920: 6365 6e74 6572 5f62 6f74 746f 6d5f 6120  center_bottom_a 
+00013930: 7d7d 3c2f 6469 763e 0a20 2020 2020 2020  }}</div>.       
+00013940: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013950: 2020 2020 2020 2020 2020 2020 203c 6469               <di
+00013960: 7620 636c 6173 733d 227b 2520 626c 6f63  v class="{% bloc
+00013970: 6b20 335f 6365 6e74 6572 5f62 6f74 746f  k 3_center_botto
+00013980: 6d5f 6163 5f63 2025 7d63 6f6c 2d31 3220  m_ac_c %}col-12 
+00013990: 636f 6c2d 6d64 2d36 7b25 2065 6e64 626c  col-md-6{% endbl
+000139a0: 6f63 6b20 257d 223e 7b7b 2033 5f63 656e  ock %}">{{ 3_cen
+000139b0: 7465 725f 626f 7474 6f6d 5f63 207d 7d3c  ter_bottom_c }}<
+000139c0: 2f64 6976 3e0a 2020 2020 2020 2020 2020  /div>.          
+000139d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000139e0: 2020 2020 2020 7b25 2065 6c69 6620 335f        {% elif 3_
+000139f0: 6365 6e74 6572 5f62 6f74 746f 6d5f 6220  center_bottom_b 
+00013a00: 616e 6420 335f 6365 6e74 6572 5f62 6f74  and 3_center_bot
+00013a10: 746f 6d5f 6320 257d 0a20 2020 2020 2020  tom_c %}.       
+00013a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013a30: 2020 2020 2020 2020 2020 2020 203c 6469               <di
+00013a40: 7620 636c 6173 733d 227b 2520 626c 6f63  v class="{% bloc
+00013a50: 6b20 335f 6365 6e74 6572 5f62 6f74 746f  k 3_center_botto
+00013a60: 6d5f 6263 5f62 2025 7d63 6f6c 2d31 3220  m_bc_b %}col-12 
+00013a70: 636f 6c2d 6d64 2d34 7b25 2065 6e64 626c  col-md-4{% endbl
+00013a80: 6f63 6b20 257d 223e 7b7b 2033 5f63 656e  ock %}">{{ 3_cen
+00013a90: 7465 725f 626f 7474 6f6d 5f62 207d 7d3c  ter_bottom_b }}<
+00013aa0: 2f64 6976 3e0a 2020 2020 2020 2020 2020  /div>.          
+00013ab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013ac0: 2020 2020 2020 2020 2020 3c64 6976 2063            <div c
+00013ad0: 6c61 7373 3d22 7b25 2062 6c6f 636b 2033  lass="{% block 3
+00013ae0: 5f63 656e 7465 725f 626f 7474 6f6d 5f62  _center_bottom_b
+00013af0: 635f 6320 257d 636f 6c2d 3132 2063 6f6c  c_c %}col-12 col
+00013b00: 2d6d 642d 387b 2520 656e 6462 6c6f 636b  -md-8{% endblock
+00013b10: 2025 7d22 3e7b 7b20 335f 6365 6e74 6572   %}">{{ 3_center
+00013b20: 5f62 6f74 746f 6d5f 6320 7d7d 3c2f 6469  _bottom_c }}</di
+00013b30: 763e 0a20 2020 2020 2020 2020 2020 2020  v>.             
+00013b40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013b50: 2020 207b 2520 656c 7365 2025 7d0a 2020     {% else %}.  
 00013b60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013b70: 2020 2020 207b 2520 6966 2033 5f72 6967       {% if 3_rig
-00013b80: 6874 5f61 2061 6e64 2033 5f72 6967 6874  ht_a and 3_right
-00013b90: 5f62 2025 7d0a 2020 2020 2020 2020 2020  _b %}.          
-00013ba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013bb0: 2020 2020 2020 2020 2020 3c64 6976 2063            <div c
-00013bc0: 6c61 7373 3d22 7b25 2062 6c6f 636b 2033  lass="{% block 3
-00013bd0: 5f72 6967 6874 5f61 625f 6120 257d 636f  _right_ab_a %}co
-00013be0: 6c2d 3132 2063 6f6c 2d6c 672d 367b 2520  l-12 col-lg-6{% 
-00013bf0: 656e 6462 6c6f 636b 2025 7d22 3e7b 7b20  endblock %}">{{ 
-00013c00: 335f 7269 6768 745f 6120 7d7d 3c2f 6469  3_right_a }}</di
-00013c10: 763e 0a20 2020 2020 2020 2020 2020 2020  v>.             
-00013c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013c30: 2020 2020 2020 203c 6469 7620 636c 6173         <div clas
-00013c40: 733d 227b 2520 626c 6f63 6b20 335f 7269  s="{% block 3_ri
-00013c50: 6768 745f 6162 5f62 2025 7d63 6f6c 2d31  ght_ab_b %}col-1
-00013c60: 3220 636f 6c2d 6c67 2d36 7b25 2065 6e64  2 col-lg-6{% end
-00013c70: 626c 6f63 6b20 257d 223e 7b7b 2033 5f72  block %}">{{ 3_r
-00013c80: 6967 6874 5f62 207d 7d3c 2f64 6976 3e0a  ight_b }}</div>.
-00013c90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013ca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013cb0: 2020 2020 7b25 2065 6c69 6620 335f 7269      {% elif 3_ri
-00013cc0: 6768 745f 6120 257d 0a20 2020 2020 2020  ght_a %}.       
-00013cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013ce0: 2020 2020 2020 2020 2020 2020 203c 6469               <di
-00013cf0: 7620 636c 6173 733d 2263 6f6c 2d31 3222  v class="col-12"
-00013d00: 3e7b 7b20 335f 7269 6768 745f 6120 7d7d  >{{ 3_right_a }}
-00013d10: 3c2f 6469 763e 0a20 2020 2020 2020 2020  </div>.         
+00013b70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013b80: 2020 3c64 6976 2063 6c61 7373 3d22 636f    <div class="co
+00013b90: 6c2d 3132 223e 7b7b 2033 5f63 656e 7465  l-12">{{ 3_cente
+00013ba0: 725f 626f 7474 6f6d 5f61 207d 7d7b 7b20  r_bottom_a }}{{ 
+00013bb0: 335f 6365 6e74 6572 5f62 6f74 746f 6d5f  3_center_bottom_
+00013bc0: 6220 7d7d 7b7b 2033 5f63 656e 7465 725f  b }}{{ 3_center_
+00013bd0: 626f 7474 6f6d 5f63 207d 7d3c 2f64 6976  bottom_c }}</div
+00013be0: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
+00013bf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013c00: 2020 7b25 2065 6e64 6966 2025 7d0a 2020    {% endif %}.  
+00013c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013c20: 2020 2020 2020 2020 2020 3c2f 6469 763e            </div>
+00013c30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00013c40: 2020 2020 2020 2020 2020 2020 207b 2520               {% 
+00013c50: 656e 6469 6620 257d 0a0a 2020 2020 2020  endif %}..      
+00013c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013c70: 2020 3c2f 6469 763e 0a20 2020 2020 2020    </div>.       
+00013c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013c90: 203c 212d 2d20 456e 6420 4365 6e74 6572   <!-- End Center
+00013ca0: 2063 6f6c 756d 6e20 2d2d 3e0a 0a20 2020   column -->..   
+00013cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013cc0: 2020 2020 203c 212d 2d20 4275 696c 6420       <!-- Build 
+00013cd0: 7269 6768 7420 636f 6c75 6d6e 202d 2d3e  right column -->
+00013ce0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00013cf0: 2020 2020 2020 2020 207b 2520 6966 2033           {% if 3
+00013d00: 5f72 6967 6874 5f61 206f 7220 335f 7269  _right_a or 3_ri
+00013d10: 6768 745f 6220 257d 0a20 2020 2020 2020  ght_b %}.       
 00013d20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013d30: 2020 2020 2020 2020 2020 207b 2520 656c             {% el
-00013d40: 7365 2025 7d0a 2020 2020 2020 2020 2020  se %}.          
-00013d50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013d60: 2020 2020 2020 2020 2020 3c64 6976 2063            <div c
-00013d70: 6c61 7373 3d22 636f 6c2d 3132 223e 7b7b  lass="col-12">{{
-00013d80: 2033 5f72 6967 6874 5f62 207d 7d3c 2f64   3_right_b }}</d
-00013d90: 6976 3e0a 2020 2020 2020 2020 2020 2020  iv>.            
-00013da0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013db0: 2020 2020 2020 2020 7b25 2065 6e64 6966          {% endif
-00013dc0: 2025 7d0a 2020 2020 2020 2020 2020 2020   %}.            
-00013dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013de0: 2020 2020 3c2f 6469 763e 0a20 2020 2020      </div>.     
-00013df0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013e00: 2020 2020 2020 203c 2f64 6976 3e0a 2020         </div>.  
-00013e10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013e20: 2020 2020 2020 7b25 2065 6e64 6966 2025        {% endif %
-00013e30: 7d0a 0a20 2020 2020 2020 2020 2020 2020  }..             
-00013e40: 2020 2020 2020 203c 212d 2d20 4e6f 2062         <!-- No b
-00013e50: 6c6f 636b 7320 696e 2063 656e 7465 7220  locks in center 
-00013e60: 706f 7369 7469 6f6e 7320 2d2d 3e0a 2020  positions -->.  
-00013e70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013e80: 2020 7b25 2065 6c73 6520 257d 0a20 2020    {% else %}.   
-00013e90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013ea0: 2020 2020 207b 2520 6966 2033 5f6c 6566       {% if 3_lef
-00013eb0: 745f 6120 6f72 2033 5f6c 6566 745f 6220  t_a or 3_left_b 
-00013ec0: 257d 0a20 2020 2020 2020 2020 2020 2020  %}.             
-00013ed0: 2020 2020 2020 2020 2020 2020 2020 207b                 {
-00013ee0: 2520 6966 2033 5f6c 6566 745f 6120 616e  % if 3_left_a an
-00013ef0: 6420 335f 6c65 6674 5f62 2025 7d0a 2020  d 3_left_b %}.  
+00013d30: 2020 2020 207b 2520 6966 2033 5f72 6967       {% if 3_rig
+00013d40: 6874 5f61 2061 6e64 2033 5f72 6967 6874  ht_a and 3_right
+00013d50: 5f62 2025 7d0a 2020 2020 2020 2020 2020  _b %}.          
+00013d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013d70: 2020 3c64 6976 2063 6c61 7373 3d22 7b25    <div class="{%
+00013d80: 2062 6c6f 636b 2033 5f72 6967 6874 5f61   block 3_right_a
+00013d90: 6220 257d 636f 6c2d 3132 2063 6f6c 2d6c  b %}col-12 col-l
+00013da0: 672d 3420 6d74 2d35 206d 742d 6c67 2d30  g-4 mt-5 mt-lg-0
+00013db0: 7b25 2065 6e64 626c 6f63 6b20 257d 223e  {% endblock %}">
+00013dc0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00013dd0: 2020 2020 2020 2020 2020 2020 207b 2520               {% 
+00013de0: 656c 6966 2033 5f72 6967 6874 5f61 2025  elif 3_right_a %
+00013df0: 7d0a 2020 2020 2020 2020 2020 2020 2020  }.              
+00013e00: 2020 2020 2020 2020 2020 2020 2020 3c64                <d
+00013e10: 6976 2063 6c61 7373 3d22 7b25 2062 6c6f  iv class="{% blo
+00013e20: 636b 2033 5f72 6967 6874 5f61 2025 7d63  ck 3_right_a %}c
+00013e30: 6f6c 2d31 3220 636f 6c2d 6c67 2d33 206d  ol-12 col-lg-3 m
+00013e40: 742d 3520 6d74 2d6c 672d 307b 2520 656e  t-5 mt-lg-0{% en
+00013e50: 6462 6c6f 636b 2025 7d22 3e0a 2020 2020  dblock %}">.    
+00013e60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013e70: 2020 2020 2020 2020 7b25 2065 6c73 6520          {% else 
+00013e80: 257d 0a20 2020 2020 2020 2020 2020 2020  %}.             
+00013e90: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+00013ea0: 6469 7620 636c 6173 733d 227b 2520 626c  div class="{% bl
+00013eb0: 6f63 6b20 335f 7269 6768 745f 6220 257d  ock 3_right_b %}
+00013ec0: 636f 6c2d 3132 2063 6f6c 2d6c 672d 3320  col-12 col-lg-3 
+00013ed0: 6f66 6673 6574 2d6c 672d 3120 6d74 2d35  offset-lg-1 mt-5
+00013ee0: 206d 742d 6c67 2d30 7b25 2065 6e64 626c   mt-lg-0{% endbl
+00013ef0: 6f63 6b20 257d 223e 0a20 2020 2020 2020  ock %}">.       
 00013f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013f10: 2020 2020 2020 2020 2020 3c64 6976 2063            <div c
-00013f20: 6c61 7373 3d22 7b25 2062 6c6f 636b 2033  lass="{% block 3
-00013f30: 5f6c 6566 745f 6e6f 5f63 656e 7465 725f  _left_no_center_
-00013f40: 6162 2025 7d63 6f6c 2d31 3220 636f 6c2d  ab %}col-12 col-
-00013f50: 6d64 2d36 7b25 2065 6e64 626c 6f63 6b20  md-6{% endblock 
-00013f60: 257d 223e 0a20 2020 2020 2020 2020 2020  %}">.           
-00013f70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013f80: 207b 2520 656c 6966 2033 5f6c 6566 745f   {% elif 3_left_
-00013f90: 6120 257d 0a20 2020 2020 2020 2020 2020  a %}.           
+00013f10: 2020 2020 207b 2520 656e 6469 6620 257d       {% endif %}
+00013f20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00013f30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013f40: 203c 6469 7620 636c 6173 733d 2272 6f77   <div class="row
+00013f50: 223e 0a20 2020 2020 2020 2020 2020 2020  ">.             
+00013f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013f70: 2020 2020 2020 207b 2520 6966 2033 5f72         {% if 3_r
+00013f80: 6967 6874 5f61 2061 6e64 2033 5f72 6967  ight_a and 3_rig
+00013f90: 6874 5f62 2025 7d0a 2020 2020 2020 2020  ht_b %}.        
 00013fa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013fb0: 203c 6469 7620 636c 6173 733d 227b 2520   <div class="{% 
-00013fc0: 626c 6f63 6b20 335f 6c65 6674 5f6e 6f5f  block 3_left_no_
-00013fd0: 6365 6e74 6572 5f61 2025 7d63 6f6c 2d31  center_a %}col-1
-00013fe0: 3220 636f 6c2d 6d64 2d36 7b25 2065 6e64  2 col-md-6{% end
-00013ff0: 626c 6f63 6b20 257d 223e 0a20 2020 2020  block %}">.     
-00014000: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014010: 2020 2020 2020 207b 2520 656c 6966 2033         {% elif 3
-00014020: 5f6c 6566 745f 6220 257d 0a20 2020 2020  _left_b %}.     
-00014030: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014040: 2020 2020 2020 203c 6469 7620 636c 6173         <div clas
-00014050: 733d 227b 2520 626c 6f63 6b20 335f 6c65  s="{% block 3_le
-00014060: 6674 5f6e 6f5f 6365 6e74 6572 5f62 2025  ft_no_center_b %
-00014070: 7d63 6f6c 2d31 3220 636f 6c2d 6d64 2d36  }col-12 col-md-6
-00014080: 7b25 2065 6e64 626c 6f63 6b20 257d 223e  {% endblock %}">
-00014090: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000140a0: 2020 2020 2020 2020 2020 2020 207b 2520               {% 
-000140b0: 656e 6469 6620 257d 0a20 2020 2020 2020  endif %}.       
-000140c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000140d0: 2020 2020 2020 2020 203c 6469 7620 636c           <div cl
-000140e0: 6173 733d 2272 6f77 223e 0a20 2020 2020  ass="row">.     
-000140f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014100: 2020 2020 2020 2020 2020 2020 2020 207b                 {
-00014110: 2520 6966 2033 5f6c 6566 745f 6120 616e  % if 3_left_a an
-00014120: 6420 335f 6c65 6674 5f62 2025 7d0a 2020  d 3_left_b %}.  
-00014130: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014140: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014150: 2020 3c64 6976 2063 6c61 7373 3d22 7b25    <div class="{%
-00014160: 2062 6c6f 636b 2033 5f6c 6566 745f 6e6f   block 3_left_no
-00014170: 5f63 656e 7465 725f 6162 5f61 2025 7d63  _center_ab_a %}c
-00014180: 6f6c 2d31 3220 636f 6c2d 6d64 2d36 7b25  ol-12 col-md-6{%
-00014190: 2065 6e64 626c 6f63 6b20 257d 223e 7b7b   endblock %}">{{
-000141a0: 2033 5f6c 6566 745f 6120 7d7d 3c2f 6469   3_left_a }}</di
-000141b0: 763e 0a20 2020 2020 2020 2020 2020 2020  v>.             
-000141c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000141d0: 2020 2020 2020 203c 6469 7620 636c 6173         <div clas
-000141e0: 733d 227b 2520 626c 6f63 6b20 335f 6c65  s="{% block 3_le
-000141f0: 6674 5f6e 6f5f 6365 6e74 6572 5f61 625f  ft_no_center_ab_
-00014200: 6220 257d 636f 6c2d 3132 2063 6f6c 2d6d  b %}col-12 col-m
-00014210: 642d 367b 2520 656e 6462 6c6f 636b 2025  d-6{% endblock %
-00014220: 7d22 3e7b 7b20 335f 6c65 6674 5f62 207d  }">{{ 3_left_b }
-00014230: 7d3c 2f64 6976 3e0a 2020 2020 2020 2020  }</div>.        
-00014240: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014250: 2020 2020 2020 2020 2020 2020 7b25 2065              {% e
-00014260: 6c69 6620 335f 6c65 6674 5f61 2025 7d0a  lif 3_left_a %}.
+00013fb0: 2020 2020 2020 2020 2020 2020 3c64 6976              <div
+00013fc0: 2063 6c61 7373 3d22 7b25 2062 6c6f 636b   class="{% block
+00013fd0: 2033 5f72 6967 6874 5f61 625f 6120 257d   3_right_ab_a %}
+00013fe0: 636f 6c2d 3132 2063 6f6c 2d6c 672d 367b  col-12 col-lg-6{
+00013ff0: 2520 656e 6462 6c6f 636b 2025 7d22 3e7b  % endblock %}">{
+00014000: 7b20 335f 7269 6768 745f 6120 7d7d 3c2f  { 3_right_a }}</
+00014010: 6469 763e 0a20 2020 2020 2020 2020 2020  div>.           
+00014020: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014030: 2020 2020 2020 2020 203c 6469 7620 636c           <div cl
+00014040: 6173 733d 227b 2520 626c 6f63 6b20 335f  ass="{% block 3_
+00014050: 7269 6768 745f 6162 5f62 2025 7d63 6f6c  right_ab_b %}col
+00014060: 2d31 3220 636f 6c2d 6c67 2d36 7b25 2065  -12 col-lg-6{% e
+00014070: 6e64 626c 6f63 6b20 257d 223e 7b7b 2033  ndblock %}">{{ 3
+00014080: 5f72 6967 6874 5f62 207d 7d3c 2f64 6976  _right_b }}</div
+00014090: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
+000140a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000140b0: 2020 2020 2020 7b25 2065 6c69 6620 335f        {% elif 3_
+000140c0: 7269 6768 745f 6120 257d 0a20 2020 2020  right_a %}.     
+000140d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000140e0: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+000140f0: 6469 7620 636c 6173 733d 2263 6f6c 2d31  div class="col-1
+00014100: 3222 3e7b 7b20 335f 7269 6768 745f 6120  2">{{ 3_right_a 
+00014110: 7d7d 3c2f 6469 763e 0a20 2020 2020 2020  }}</div>.       
+00014120: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014130: 2020 2020 2020 2020 2020 2020 207b 2520               {% 
+00014140: 656c 7365 2025 7d0a 2020 2020 2020 2020  else %}.        
+00014150: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014160: 2020 2020 2020 2020 2020 2020 3c64 6976              <div
+00014170: 2063 6c61 7373 3d22 636f 6c2d 3132 223e   class="col-12">
+00014180: 7b7b 2033 5f72 6967 6874 5f62 207d 7d3c  {{ 3_right_b }}<
+00014190: 2f64 6976 3e0a 2020 2020 2020 2020 2020  /div>.          
+000141a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000141b0: 2020 2020 2020 2020 2020 7b25 2065 6e64            {% end
+000141c0: 6966 2025 7d0a 2020 2020 2020 2020 2020  if %}.          
+000141d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000141e0: 2020 2020 2020 3c2f 6469 763e 0a20 2020        </div>.   
+000141f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014200: 2020 2020 2020 2020 203c 2f64 6976 3e0a           </div>.
+00014210: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014220: 2020 2020 2020 2020 7b25 2065 6e64 6966          {% endif
+00014230: 2025 7d0a 0a20 2020 2020 2020 2020 2020   %}..           
+00014240: 2020 2020 2020 2020 203c 212d 2d20 4e6f           <!-- No
+00014250: 2062 6c6f 636b 7320 696e 2063 656e 7465   blocks in cente
+00014260: 7220 706f 7369 7469 6f6e 7320 2d2d 3e0a  r positions -->.
 00014270: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014280: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014290: 2020 2020 3c64 6976 2063 6c61 7373 3d22      <div class="
-000142a0: 636f 6c2d 3132 223e 7b7b 2033 5f6c 6566  col-12">{{ 3_lef
-000142b0: 745f 6120 7d7d 3c2f 6469 763e 0a20 2020  t_a }}</div>.   
-000142c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014280: 2020 2020 7b25 2065 6c73 6520 257d 0a20      {% else %}. 
+00014290: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000142a0: 2020 2020 2020 207b 2520 6966 2033 5f6c         {% if 3_l
+000142b0: 6566 745f 6120 6f72 2033 5f6c 6566 745f  eft_a or 3_left_
+000142c0: 6220 257d 0a20 2020 2020 2020 2020 2020  b %}.           
 000142d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000142e0: 207b 2520 656c 7365 2025 7d0a 2020 2020   {% else %}.    
-000142f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000142e0: 207b 2520 6966 2033 5f6c 6566 745f 6120   {% if 3_left_a 
+000142f0: 616e 6420 335f 6c65 6674 5f62 2025 7d0a  and 3_left_b %}.
 00014300: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014310: 3c64 6976 2063 6c61 7373 3d22 636f 6c2d  <div class="col-
-00014320: 3132 223e 7b7b 2033 5f6c 6566 745f 6220  12">{{ 3_left_b 
-00014330: 7d7d 3c2f 6469 763e 0a20 2020 2020 2020  }}</div>.       
-00014340: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014350: 2020 2020 2020 2020 2020 2020 207b 2520               {% 
-00014360: 656e 6469 6620 257d 0a20 2020 2020 2020  endif %}.       
+00014310: 2020 2020 2020 2020 2020 2020 3c64 6976              <div
+00014320: 2063 6c61 7373 3d22 7b25 2062 6c6f 636b   class="{% block
+00014330: 2033 5f6c 6566 745f 6e6f 5f63 656e 7465   3_left_no_cente
+00014340: 725f 6162 2025 7d63 6f6c 2d31 3220 636f  r_ab %}col-12 co
+00014350: 6c2d 6d64 2d36 7b25 2065 6e64 626c 6f63  l-md-6{% endbloc
+00014360: 6b20 257d 223e 0a20 2020 2020 2020 2020  k %}">.         
 00014370: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014380: 2020 2020 2020 2020 203c 2f64 6976 3e0a           </div>.
-00014390: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000143a0: 2020 2020 2020 2020 2020 2020 3c2f 6469              </di
-000143b0: 763e 0a20 2020 2020 2020 2020 2020 2020  v>.             
-000143c0: 2020 2020 2020 2020 2020 207b 2520 656e             {% en
-000143d0: 6469 6620 257d 0a0a 2020 2020 2020 2020  dif %}..        
-000143e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000143f0: 7b25 2069 6620 335f 7269 6768 745f 6120  {% if 3_right_a 
-00014400: 6f72 2033 5f72 6967 6874 5f62 2025 7d0a  or 3_right_b %}.
-00014410: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014420: 2020 2020 2020 2020 2020 2020 7b25 2069              {% i
-00014430: 6620 335f 7269 6768 745f 6120 616e 6420  f 3_right_a and 
-00014440: 335f 7269 6768 745f 6220 257d 0a20 2020  3_right_b %}.   
-00014450: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014460: 2020 2020 2020 2020 203c 6469 7620 636c           <div cl
-00014470: 6173 733d 227b 2520 626c 6f63 6b20 335f  ass="{% block 3_
-00014480: 7269 6768 745f 6e6f 5f63 656e 7465 725f  right_no_center_
-00014490: 6162 2025 7d63 6f6c 2d31 3220 636f 6c2d  ab %}col-12 col-
-000144a0: 6d64 2d36 7b25 2065 6e64 626c 6f63 6b20  md-6{% endblock 
-000144b0: 257d 223e 0a20 2020 2020 2020 2020 2020  %}">.           
+00014380: 2020 207b 2520 656c 6966 2033 5f6c 6566     {% elif 3_lef
+00014390: 745f 6120 257d 0a20 2020 2020 2020 2020  t_a %}.         
+000143a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000143b0: 2020 203c 6469 7620 636c 6173 733d 227b     <div class="{
+000143c0: 2520 626c 6f63 6b20 335f 6c65 6674 5f6e  % block 3_left_n
+000143d0: 6f5f 6365 6e74 6572 5f61 2025 7d63 6f6c  o_center_a %}col
+000143e0: 2d31 3220 636f 6c2d 6d64 2d36 7b25 2065  -12 col-md-6{% e
+000143f0: 6e64 626c 6f63 6b20 257d 223e 0a20 2020  ndblock %}">.   
+00014400: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014410: 2020 2020 2020 2020 207b 2520 656c 6966           {% elif
+00014420: 2033 5f6c 6566 745f 6220 257d 0a20 2020   3_left_b %}.   
+00014430: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014440: 2020 2020 2020 2020 203c 6469 7620 636c           <div cl
+00014450: 6173 733d 227b 2520 626c 6f63 6b20 335f  ass="{% block 3_
+00014460: 6c65 6674 5f6e 6f5f 6365 6e74 6572 5f62  left_no_center_b
+00014470: 2025 7d63 6f6c 2d31 3220 636f 6c2d 6d64   %}col-12 col-md
+00014480: 2d36 7b25 2065 6e64 626c 6f63 6b20 257d  -6{% endblock %}
+00014490: 223e 0a20 2020 2020 2020 2020 2020 2020  ">.             
+000144a0: 2020 2020 2020 2020 2020 2020 2020 207b                 {
+000144b0: 2520 656e 6469 6620 257d 0a20 2020 2020  % endif %}.     
 000144c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000144d0: 207b 2520 656c 6966 2033 5f72 6967 6874   {% elif 3_right
-000144e0: 5f61 2025 7d0a 2020 2020 2020 2020 2020  _a %}.          
+000144d0: 2020 2020 2020 2020 2020 203c 6469 7620             <div 
+000144e0: 636c 6173 733d 2272 6f77 223e 0a20 2020  class="row">.   
 000144f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014500: 2020 3c64 6976 2063 6c61 7373 3d22 7b25    <div class="{%
-00014510: 2062 6c6f 636b 2033 5f72 6967 6874 5f6e   block 3_right_n
-00014520: 6f5f 6365 6e74 6572 5f61 2025 7d63 6f6c  o_center_a %}col
-00014530: 2d31 3220 636f 6c2d 6d64 2d36 7b25 2065  -12 col-md-6{% e
-00014540: 6e64 626c 6f63 6b20 257d 223e 0a20 2020  ndblock %}">.   
-00014550: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014560: 2020 2020 2020 2020 207b 2520 656c 6966           {% elif
-00014570: 2033 5f72 6967 6874 5f62 2025 7d0a 2020   3_right_b %}.  
-00014580: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014590: 2020 2020 2020 2020 2020 3c64 6976 2063            <div c
-000145a0: 6c61 7373 3d22 7b25 2062 6c6f 636b 2033  lass="{% block 3
-000145b0: 5f72 6967 6874 5f6e 6f5f 6365 6e74 6572  _right_no_center
-000145c0: 5f62 2025 7d63 6f6c 2d31 3220 636f 6c2d  _b %}col-12 col-
-000145d0: 6d64 2d36 7b25 2065 6e64 626c 6f63 6b20  md-6{% endblock 
-000145e0: 257d 223e 0a20 2020 2020 2020 2020 2020  %}">.           
-000145f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014600: 207b 2520 656e 6469 6620 257d 0a20 2020   {% endif %}.   
-00014610: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014620: 2020 2020 2020 2020 2020 2020 203c 6469               <di
-00014630: 7620 636c 6173 733d 2272 6f77 223e 0a20  v class="row">. 
+00014500: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014510: 207b 2520 6966 2033 5f6c 6566 745f 6120   {% if 3_left_a 
+00014520: 616e 6420 335f 6c65 6674 5f62 2025 7d0a  and 3_left_b %}.
+00014530: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014540: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014550: 2020 2020 3c64 6976 2063 6c61 7373 3d22      <div class="
+00014560: 7b25 2062 6c6f 636b 2033 5f6c 6566 745f  {% block 3_left_
+00014570: 6e6f 5f63 656e 7465 725f 6162 5f61 2025  no_center_ab_a %
+00014580: 7d63 6f6c 2d31 3220 636f 6c2d 6d64 2d36  }col-12 col-md-6
+00014590: 7b25 2065 6e64 626c 6f63 6b20 257d 223e  {% endblock %}">
+000145a0: 7b7b 2033 5f6c 6566 745f 6120 7d7d 3c2f  {{ 3_left_a }}</
+000145b0: 6469 763e 0a20 2020 2020 2020 2020 2020  div>.           
+000145c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000145d0: 2020 2020 2020 2020 203c 6469 7620 636c           <div cl
+000145e0: 6173 733d 227b 2520 626c 6f63 6b20 335f  ass="{% block 3_
+000145f0: 6c65 6674 5f6e 6f5f 6365 6e74 6572 5f61  left_no_center_a
+00014600: 625f 6220 257d 636f 6c2d 3132 2063 6f6c  b_b %}col-12 col
+00014610: 2d6d 642d 367b 2520 656e 6462 6c6f 636b  -md-6{% endblock
+00014620: 2025 7d22 3e7b 7b20 335f 6c65 6674 5f62   %}">{{ 3_left_b
+00014630: 207d 7d3c 2f64 6976 3e0a 2020 2020 2020   }}</div>.      
 00014640: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014650: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014660: 2020 207b 2520 6966 2033 5f72 6967 6874     {% if 3_right
-00014670: 5f61 2061 6e64 2033 5f72 6967 6874 5f62  _a and 3_right_b
-00014680: 2025 7d0a 2020 2020 2020 2020 2020 2020   %}.            
-00014690: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000146a0: 2020 2020 2020 2020 3c64 6976 2063 6c61          <div cla
-000146b0: 7373 3d22 7b25 2062 6c6f 636b 2033 5f72  ss="{% block 3_r
-000146c0: 6967 6874 5f6e 6f5f 6365 6e74 6572 5f61  ight_no_center_a
-000146d0: 625f 6120 257d 636f 6c2d 3132 2063 6f6c  b_a %}col-12 col
-000146e0: 2d6d 642d 367b 2520 656e 6462 6c6f 636b  -md-6{% endblock
-000146f0: 2025 7d22 3e7b 7b20 335f 7269 6768 745f   %}">{{ 3_right_
-00014700: 6120 7d7d 3c2f 6469 763e 0a20 2020 2020  a }}</div>.     
-00014710: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014720: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-00014730: 6469 7620 636c 6173 733d 227b 2520 626c  div class="{% bl
-00014740: 6f63 6b20 335f 7269 6768 745f 6e6f 5f63  ock 3_right_no_c
-00014750: 656e 7465 725f 6162 5f62 2025 7d63 6f6c  enter_ab_b %}col
-00014760: 2d31 3220 636f 6c2d 6d64 2d36 7b25 2065  -12 col-md-6{% e
-00014770: 6e64 626c 6f63 6b20 257d 223e 7b7b 2033  ndblock %}">{{ 3
-00014780: 5f72 6967 6874 5f62 207d 7d2f 6469 763e  _right_b }}/div>
-00014790: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000147a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000147b0: 2020 2020 207b 2520 656c 6966 2033 5f72       {% elif 3_r
-000147c0: 6967 6874 5f61 2025 7d0a 2020 2020 2020  ight_a %}.      
-000147d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000147e0: 2020 2020 2020 2020 2020 2020 2020 3c64                <d
-000147f0: 6976 2063 6c61 7373 3d22 636f 6c2d 3132  iv class="col-12
-00014800: 223e 7b7b 2033 5f72 6967 6874 5f61 207d  ">{{ 3_right_a }
-00014810: 7d3c 2f64 6976 3e0a 2020 2020 2020 2020  }</div>.        
-00014820: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014830: 2020 2020 2020 2020 2020 2020 7b25 2065              {% e
-00014840: 6c73 6520 257d 0a20 2020 2020 2020 2020  lse %}.         
+00014650: 2020 2020 2020 2020 2020 2020 2020 7b25                {%
+00014660: 2065 6c69 6620 335f 6c65 6674 5f61 2025   elif 3_left_a %
+00014670: 7d0a 2020 2020 2020 2020 2020 2020 2020  }.              
+00014680: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014690: 2020 2020 2020 3c64 6976 2063 6c61 7373        <div class
+000146a0: 3d22 636f 6c2d 3132 223e 7b7b 2033 5f6c  ="col-12">{{ 3_l
+000146b0: 6566 745f 6120 7d7d 3c2f 6469 763e 0a20  eft_a }}</div>. 
+000146c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000146d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000146e0: 2020 207b 2520 656c 7365 2025 7d0a 2020     {% else %}.  
+000146f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014700: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014710: 2020 3c64 6976 2063 6c61 7373 3d22 636f    <div class="co
+00014720: 6c2d 3132 223e 7b7b 2033 5f6c 6566 745f  l-12">{{ 3_left_
+00014730: 6220 7d7d 3c2f 6469 763e 0a20 2020 2020  b }}</div>.     
+00014740: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014750: 2020 2020 2020 2020 2020 2020 2020 207b                 {
+00014760: 2520 656e 6469 6620 257d 0a20 2020 2020  % endif %}.     
+00014770: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014780: 2020 2020 2020 2020 2020 203c 2f64 6976             </div
+00014790: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
+000147a0: 2020 2020 2020 2020 2020 2020 2020 3c2f                </
+000147b0: 6469 763e 0a20 2020 2020 2020 2020 2020  div>.           
+000147c0: 2020 2020 2020 2020 2020 2020 207b 2520               {% 
+000147d0: 656e 6469 6620 257d 0a0a 2020 2020 2020  endif %}..      
+000147e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000147f0: 2020 7b25 2069 6620 335f 7269 6768 745f    {% if 3_right_
+00014800: 6120 6f72 2033 5f72 6967 6874 5f62 2025  a or 3_right_b %
+00014810: 7d0a 2020 2020 2020 2020 2020 2020 2020  }.              
+00014820: 2020 2020 2020 2020 2020 2020 2020 7b25                {%
+00014830: 2069 6620 335f 7269 6768 745f 6120 616e   if 3_right_a an
+00014840: 6420 335f 7269 6768 745f 6220 257d 0a20  d 3_right_b %}. 
 00014850: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00014860: 2020 2020 2020 2020 2020 203c 6469 7620             <div 
-00014870: 636c 6173 733d 2263 6f6c 2d31 3222 3e7b  class="col-12">{
-00014880: 7b20 335f 7269 6768 745f 6220 7d7d 3c2f  { 3_right_b }}</
-00014890: 6469 763e 0a20 2020 2020 2020 2020 2020  div>.           
-000148a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000148b0: 2020 2020 2020 2020 207b 2520 656e 6469           {% endi
-000148c0: 6620 257d 0a20 2020 2020 2020 2020 2020  f %}.           
-000148d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000148e0: 2020 2020 203c 2f64 6976 3e0a 2020 2020       </div>.    
+00014870: 636c 6173 733d 227b 2520 626c 6f63 6b20  class="{% block 
+00014880: 335f 7269 6768 745f 6e6f 5f63 656e 7465  3_right_no_cente
+00014890: 725f 6162 2025 7d63 6f6c 2d31 3220 636f  r_ab %}col-12 co
+000148a0: 6c2d 6d64 2d36 7b25 2065 6e64 626c 6f63  l-md-6{% endbloc
+000148b0: 6b20 257d 223e 0a20 2020 2020 2020 2020  k %}">.         
+000148c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000148d0: 2020 207b 2520 656c 6966 2033 5f72 6967     {% elif 3_rig
+000148e0: 6874 5f61 2025 7d0a 2020 2020 2020 2020  ht_a %}.        
 000148f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014900: 2020 2020 2020 2020 3c2f 6469 763e 0a20          </div>. 
-00014910: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014920: 2020 2020 2020 207b 2520 656e 6469 6620         {% endif 
-00014930: 257d 0a0a 2020 2020 2020 2020 2020 2020  %}..            
-00014940: 2020 2020 2020 2020 7b25 2065 6e64 6966          {% endif
-00014950: 2025 7d0a 0a20 2020 2020 2020 2020 2020   %}..           
-00014960: 2020 2020 2020 2020 203c 212d 2d20 426c           <!-- Bl
-00014970: 6f63 6b73 2069 6e20 6d69 6464 6c65 2062  ocks in middle b
-00014980: 6f74 746f 6d20 706f 7369 7469 6f6e 202d  ottom position -
-00014990: 2d3e 0a20 2020 2020 2020 2020 2020 2020  ->.             
-000149a0: 2020 2020 2020 207b 2520 6966 2033 5f6d         {% if 3_m
-000149b0: 6964 5f62 6f74 746f 6d5f 6120 6f72 2033  id_bottom_a or 3
-000149c0: 5f6d 6964 5f62 6f74 746f 6d5f 6220 6f72  _mid_bottom_b or
-000149d0: 2033 5f6d 6964 5f62 6f74 746f 6d5f 6320   3_mid_bottom_c 
-000149e0: 257d 0a20 2020 2020 2020 2020 2020 2020  %}.             
-000149f0: 2020 2020 2020 203c 6469 7620 636c 6173         <div clas
-00014a00: 733d 2263 6f6c 2d31 3222 3e0a 2020 2020  s="col-12">.    
+00014900: 2020 2020 3c64 6976 2063 6c61 7373 3d22      <div class="
+00014910: 7b25 2062 6c6f 636b 2033 5f72 6967 6874  {% block 3_right
+00014920: 5f6e 6f5f 6365 6e74 6572 5f61 2025 7d63  _no_center_a %}c
+00014930: 6f6c 2d31 3220 636f 6c2d 6d64 2d36 7b25  ol-12 col-md-6{%
+00014940: 2065 6e64 626c 6f63 6b20 257d 223e 0a20   endblock %}">. 
+00014950: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014960: 2020 2020 2020 2020 2020 207b 2520 656c             {% el
+00014970: 6966 2033 5f72 6967 6874 5f62 2025 7d0a  if 3_right_b %}.
+00014980: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014990: 2020 2020 2020 2020 2020 2020 3c64 6976              <div
+000149a0: 2063 6c61 7373 3d22 7b25 2062 6c6f 636b   class="{% block
+000149b0: 2033 5f72 6967 6874 5f6e 6f5f 6365 6e74   3_right_no_cent
+000149c0: 6572 5f62 2025 7d63 6f6c 2d31 3220 636f  er_b %}col-12 co
+000149d0: 6c2d 6d64 2d36 7b25 2065 6e64 626c 6f63  l-md-6{% endbloc
+000149e0: 6b20 257d 223e 0a20 2020 2020 2020 2020  k %}">.         
+000149f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014a00: 2020 207b 2520 656e 6469 6620 257d 0a20     {% endif %}. 
 00014a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014a20: 2020 2020 3c64 6976 2063 6c61 7373 3d22      <div class="
-00014a30: 726f 7722 3e0a 2020 2020 2020 2020 2020  row">.          
-00014a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014a50: 2020 7b25 2069 6620 335f 6d69 645f 626f    {% if 3_mid_bo
-00014a60: 7474 6f6d 5f61 2061 6e64 2033 5f6d 6964  ttom_a and 3_mid
-00014a70: 5f62 6f74 746f 6d5f 6220 616e 6420 335f  _bottom_b and 3_
-00014a80: 6d69 645f 626f 7474 6f6d 5f63 2025 7d0a  mid_bottom_c %}.
+00014a20: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+00014a30: 6469 7620 636c 6173 733d 2272 6f77 223e  div class="row">
+00014a40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00014a50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014a60: 2020 2020 207b 2520 6966 2033 5f72 6967       {% if 3_rig
+00014a70: 6874 5f61 2061 6e64 2033 5f72 6967 6874  ht_a and 3_right
+00014a80: 5f62 2025 7d0a 2020 2020 2020 2020 2020  _b %}.          
 00014a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014ab0: 3c64 6976 2063 6c61 7373 3d22 7b25 2062  <div class="{% b
-00014ac0: 6c6f 636b 2033 5f6d 6964 5f62 6f74 746f  lock 3_mid_botto
-00014ad0: 6d5f 6162 635f 6120 257d 636f 6c2d 3132  m_abc_a %}col-12
-00014ae0: 2063 6f6c 2d6d 642d 347b 2520 656e 6462   col-md-4{% endb
-00014af0: 6c6f 636b 2025 7d22 3e7b 7b20 335f 6d69  lock %}">{{ 3_mi
-00014b00: 645f 626f 7474 6f6d 5f61 207d 7d3c 2f64  d_bottom_a }}</d
-00014b10: 6976 3e0a 2020 2020 2020 2020 2020 2020  iv>.            
+00014aa0: 2020 2020 2020 2020 2020 3c64 6976 2063            <div c
+00014ab0: 6c61 7373 3d22 7b25 2062 6c6f 636b 2033  lass="{% block 3
+00014ac0: 5f72 6967 6874 5f6e 6f5f 6365 6e74 6572  _right_no_center
+00014ad0: 5f61 625f 6120 257d 636f 6c2d 3132 2063  _ab_a %}col-12 c
+00014ae0: 6f6c 2d6d 642d 367b 2520 656e 6462 6c6f  ol-md-6{% endblo
+00014af0: 636b 2025 7d22 3e7b 7b20 335f 7269 6768  ck %}">{{ 3_righ
+00014b00: 745f 6120 7d7d 3c2f 6469 763e 0a20 2020  t_a }}</div>.   
+00014b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00014b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014b30: 2020 2020 3c64 6976 2063 6c61 7373 3d22      <div class="
-00014b40: 7b25 2062 6c6f 636b 2033 5f6d 6964 5f62  {% block 3_mid_b
-00014b50: 6f74 746f 6d5f 6162 635f 6220 257d 636f  ottom_abc_b %}co
-00014b60: 6c2d 3132 2063 6f6c 2d6d 642d 347b 2520  l-12 col-md-4{% 
-00014b70: 656e 6462 6c6f 636b 2025 7d22 3e7b 7b20  endblock %}">{{ 
-00014b80: 335f 6d69 645f 626f 7474 6f6d 5f62 207d  3_mid_bottom_b }
-00014b90: 7d3c 2f64 6976 3e0a 2020 2020 2020 2020  }</div>.        
+00014b30: 203c 6469 7620 636c 6173 733d 227b 2520   <div class="{% 
+00014b40: 626c 6f63 6b20 335f 7269 6768 745f 6e6f  block 3_right_no
+00014b50: 5f63 656e 7465 725f 6162 5f62 2025 7d63  _center_ab_b %}c
+00014b60: 6f6c 2d31 3220 636f 6c2d 6d64 2d36 7b25  ol-12 col-md-6{%
+00014b70: 2065 6e64 626c 6f63 6b20 257d 223e 7b7b   endblock %}">{{
+00014b80: 2033 5f72 6967 6874 5f62 207d 7d2f 6469   3_right_b }}/di
+00014b90: 763e 0a20 2020 2020 2020 2020 2020 2020  v>.             
 00014ba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014bb0: 2020 2020 2020 2020 3c64 6976 2063 6c61          <div cla
-00014bc0: 7373 3d22 7b25 2062 6c6f 636b 2033 5f6d  ss="{% block 3_m
-00014bd0: 6964 5f62 6f74 746f 6d5f 6162 635f 6320  id_bottom_abc_c 
-00014be0: 257d 636f 6c2d 3132 2063 6f6c 2d6d 642d  %}col-12 col-md-
-00014bf0: 347b 2520 656e 6462 6c6f 636b 2025 7d22  4{% endblock %}"
-00014c00: 3e7b 7b20 335f 6d69 645f 626f 7474 6f6d  >{{ 3_mid_bottom
-00014c10: 5f63 207d 7d3c 2f64 6976 3e0a 2020 2020  _c }}</div>.    
+00014bb0: 2020 2020 2020 207b 2520 656c 6966 2033         {% elif 3
+00014bc0: 5f72 6967 6874 5f61 2025 7d0a 2020 2020  _right_a %}.    
+00014bd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014be0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014bf0: 3c64 6976 2063 6c61 7373 3d22 636f 6c2d  <div class="col-
+00014c00: 3132 223e 7b7b 2033 5f72 6967 6874 5f61  12">{{ 3_right_a
+00014c10: 207d 7d3c 2f64 6976 3e0a 2020 2020 2020   }}</div>.      
 00014c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014c30: 2020 2020 2020 2020 7b25 2065 6c69 6620          {% elif 
-00014c40: 335f 6d69 645f 626f 7474 6f6d 5f61 2061  3_mid_bottom_a a
-00014c50: 6e64 2033 5f6d 6964 5f62 6f74 746f 6d5f  nd 3_mid_bottom_
-00014c60: 6220 257d 0a20 2020 2020 2020 2020 2020  b %}.           
-00014c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014c80: 2020 2020 203c 6469 7620 636c 6173 733d       <div class=
-00014c90: 227b 2520 626c 6f63 6b20 335f 6d69 645f  "{% block 3_mid_
-00014ca0: 626f 7474 6f6d 5f61 625f 6120 257d 636f  bottom_ab_a %}co
-00014cb0: 6c2d 3132 2063 6f6c 2d6d 642d 387b 2520  l-12 col-md-8{% 
-00014cc0: 656e 6462 6c6f 636b 2025 7d22 3e7b 7b20  endblock %}">{{ 
-00014cd0: 335f 6d69 645f 626f 7474 6f6d 5f61 207d  3_mid_bottom_a }
-00014ce0: 7d3c 2f64 6976 3e0a 2020 2020 2020 2020  }</div>.        
+00014c30: 2020 2020 2020 2020 2020 2020 2020 7b25                {%
+00014c40: 2065 6c73 6520 257d 0a20 2020 2020 2020   else %}.       
+00014c50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014c60: 2020 2020 2020 2020 2020 2020 203c 6469               <di
+00014c70: 7620 636c 6173 733d 2263 6f6c 2d31 3222  v class="col-12"
+00014c80: 3e7b 7b20 335f 7269 6768 745f 6220 7d7d  >{{ 3_right_b }}
+00014c90: 3c2f 6469 763e 0a20 2020 2020 2020 2020  </div>.         
+00014ca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014cb0: 2020 2020 2020 2020 2020 207b 2520 656e             {% en
+00014cc0: 6469 6620 257d 0a20 2020 2020 2020 2020  dif %}.         
+00014cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014ce0: 2020 2020 2020 203c 2f64 6976 3e0a 2020         </div>.  
 00014cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014d00: 2020 2020 2020 2020 3c64 6976 2063 6c61          <div cla
-00014d10: 7373 3d22 7b25 2062 6c6f 636b 2033 5f6d  ss="{% block 3_m
-00014d20: 6964 5f62 6f74 746f 6d5f 6162 5f62 2025  id_bottom_ab_b %
-00014d30: 7d63 6f6c 2d31 3220 636f 6c2d 6d64 2d34  }col-12 col-md-4
-00014d40: 7b25 2065 6e64 626c 6f63 6b20 257d 223e  {% endblock %}">
-00014d50: 7b7b 2033 5f6d 6964 5f62 6f74 746f 6d5f  {{ 3_mid_bottom_
-00014d60: 6220 7d7d 3c2f 6469 763e 0a20 2020 2020  b }}</div>.     
-00014d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014d80: 2020 2020 2020 207b 2520 656c 6966 2033         {% elif 3
-00014d90: 5f6d 6964 5f62 6f74 746f 6d5f 6120 616e  _mid_bottom_a an
-00014da0: 6420 335f 6d69 645f 626f 7474 6f6d 5f63  d 3_mid_bottom_c
-00014db0: 2025 7d0a 2020 2020 2020 2020 2020 2020   %}.            
-00014dc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014dd0: 2020 2020 3c64 6976 2063 6c61 7373 3d22      <div class="
-00014de0: 7b25 2062 6c6f 636b 2033 5f6d 6964 5f62  {% block 3_mid_b
-00014df0: 6f74 746f 6d5f 6163 5f61 2025 7d63 6f6c  ottom_ac_a %}col
-00014e00: 2d31 3220 636f 6c2d 6d64 2d36 7b25 2065  -12 col-md-6{% e
-00014e10: 6e64 626c 6f63 6b20 257d 223e 7b7b 2033  ndblock %}">{{ 3
-00014e20: 5f6d 6964 5f62 6f74 746f 6d5f 6120 7d7d  _mid_bottom_a }}
-00014e30: 3c2f 6469 763e 0a20 2020 2020 2020 2020  </div>.         
+00014d00: 2020 2020 2020 2020 2020 3c2f 6469 763e            </div>
+00014d10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00014d20: 2020 2020 2020 2020 207b 2520 656e 6469           {% endi
+00014d30: 6620 257d 0a0a 2020 2020 2020 2020 2020  f %}..          
+00014d40: 2020 2020 2020 2020 2020 7b25 2065 6e64            {% end
+00014d50: 6966 2025 7d0a 0a20 2020 2020 2020 2020  if %}..         
+00014d60: 2020 2020 2020 2020 2020 203c 212d 2d20             <!-- 
+00014d70: 426c 6f63 6b73 2069 6e20 6d69 6464 6c65  Blocks in middle
+00014d80: 2062 6f74 746f 6d20 706f 7369 7469 6f6e   bottom position
+00014d90: 202d 2d3e 0a20 2020 2020 2020 2020 2020   -->.           
+00014da0: 2020 2020 2020 2020 207b 2520 6966 2033           {% if 3
+00014db0: 5f6d 6964 5f62 6f74 746f 6d5f 6120 6f72  _mid_bottom_a or
+00014dc0: 2033 5f6d 6964 5f62 6f74 746f 6d5f 6220   3_mid_bottom_b 
+00014dd0: 6f72 2033 5f6d 6964 5f62 6f74 746f 6d5f  or 3_mid_bottom_
+00014de0: 6320 257d 0a20 2020 2020 2020 2020 2020  c %}.           
+00014df0: 2020 2020 2020 2020 203c 6469 7620 636c           <div cl
+00014e00: 6173 733d 2263 6f6c 2d31 3222 3e0a 2020  ass="col-12">.  
+00014e10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014e20: 2020 2020 2020 3c64 6976 2063 6c61 7373        <div class
+00014e30: 3d22 726f 7722 3e0a 2020 2020 2020 2020  ="row">.        
 00014e40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014e50: 2020 2020 2020 203c 6469 7620 636c 6173         <div clas
-00014e60: 733d 227b 2520 626c 6f63 6b20 335f 6d69  s="{% block 3_mi
-00014e70: 645f 626f 7474 6f6d 5f61 635f 6320 257d  d_bottom_ac_c %}
-00014e80: 636f 6c2d 3132 2063 6f6c 2d6d 642d 367b  col-12 col-md-6{
-00014e90: 2520 656e 6462 6c6f 636b 2025 7d22 3e7b  % endblock %}">{
-00014ea0: 7b20 335f 6d69 645f 626f 7474 6f6d 5f63  { 3_mid_bottom_c
-00014eb0: 207d 7d3c 2f64 6976 3e0a 2020 2020 2020   }}</div>.      
-00014ec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014ed0: 2020 2020 2020 7b25 2065 6c69 6620 335f        {% elif 3_
-00014ee0: 6d69 645f 626f 7474 6f6d 5f62 2061 6e64  mid_bottom_b and
-00014ef0: 2033 5f6d 6964 5f62 6f74 746f 6d5f 6320   3_mid_bottom_c 
-00014f00: 257d 0a20 2020 2020 2020 2020 2020 2020  %}.             
-00014f10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014f20: 2020 203c 6469 7620 636c 6173 733d 227b     <div class="{
-00014f30: 2520 626c 6f63 6b20 335f 6d69 645f 626f  % block 3_mid_bo
-00014f40: 7474 6f6d 5f62 635f 6220 257d 636f 6c2d  ttom_bc_b %}col-
-00014f50: 3132 2063 6f6c 2d6d 642d 347b 2520 656e  12 col-md-4{% en
-00014f60: 6462 6c6f 636b 2025 7d22 3e7b 7b20 335f  dblock %}">{{ 3_
-00014f70: 6d69 645f 626f 7474 6f6d 5f62 207d 7d3c  mid_bottom_b }}<
-00014f80: 2f64 6976 3e0a 2020 2020 2020 2020 2020  /div>.          
-00014f90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014fa0: 2020 2020 2020 3c64 6976 2063 6c61 7373        <div class
-00014fb0: 3d22 7b25 2062 6c6f 636b 2033 5f6d 6964  ="{% block 3_mid
-00014fc0: 5f62 6f74 746f 6d5f 6263 5f63 2025 7d63  _bottom_bc_c %}c
-00014fd0: 6f6c 2d31 3220 636f 6c2d 6d64 2d38 7b25  ol-12 col-md-8{%
-00014fe0: 2065 6e64 626c 6f63 6b20 257d 223e 7b7b   endblock %}">{{
-00014ff0: 2033 5f6d 6964 5f62 6f74 746f 6d5f 6320   3_mid_bottom_c 
-00015000: 7d7d 3c2f 6469 763e 0a20 2020 2020 2020  }}</div>.       
-00015010: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015020: 2020 2020 207b 2520 656c 7365 2025 7d0a       {% else %}.
-00015030: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015040: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015050: 3c64 6976 2063 6c61 7373 3d22 636f 6c2d  <div class="col-
-00015060: 3132 223e 7b7b 2033 5f6d 6964 5f62 6f74  12">{{ 3_mid_bot
-00015070: 746f 6d5f 6120 7d7d 7b7b 2033 5f6d 6964  tom_a }}{{ 3_mid
-00015080: 5f62 6f74 746f 6d5f 6220 7d7d 7b7b 2033  _bottom_b }}{{ 3
-00015090: 5f6d 6964 5f62 6f74 746f 6d5f 6320 7d7d  _mid_bottom_c }}
-000150a0: 3c2f 6469 763e 0a20 2020 2020 2020 2020  </div>.         
-000150b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000150c0: 2020 207b 2520 656e 6469 6620 257d 0a20     {% endif %}. 
-000150d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000150e0: 2020 2020 2020 203c 2f64 6976 3e0a 2020         </div>.  
+00014e50: 2020 2020 7b25 2069 6620 335f 6d69 645f      {% if 3_mid_
+00014e60: 626f 7474 6f6d 5f61 2061 6e64 2033 5f6d  bottom_a and 3_m
+00014e70: 6964 5f62 6f74 746f 6d5f 6220 616e 6420  id_bottom_b and 
+00014e80: 335f 6d69 645f 626f 7474 6f6d 5f63 2025  3_mid_bottom_c %
+00014e90: 7d0a 2020 2020 2020 2020 2020 2020 2020  }.              
+00014ea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014eb0: 2020 3c64 6976 2063 6c61 7373 3d22 7b25    <div class="{%
+00014ec0: 2062 6c6f 636b 2033 5f6d 6964 5f62 6f74   block 3_mid_bot
+00014ed0: 746f 6d5f 6162 635f 6120 257d 636f 6c2d  tom_abc_a %}col-
+00014ee0: 3132 2063 6f6c 2d6d 642d 347b 2520 656e  12 col-md-4{% en
+00014ef0: 6462 6c6f 636b 2025 7d22 3e7b 7b20 335f  dblock %}">{{ 3_
+00014f00: 6d69 645f 626f 7474 6f6d 5f61 207d 7d3c  mid_bottom_a }}<
+00014f10: 2f64 6976 3e0a 2020 2020 2020 2020 2020  /div>.          
+00014f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014f30: 2020 2020 2020 3c64 6976 2063 6c61 7373        <div class
+00014f40: 3d22 7b25 2062 6c6f 636b 2033 5f6d 6964  ="{% block 3_mid
+00014f50: 5f62 6f74 746f 6d5f 6162 635f 6220 257d  _bottom_abc_b %}
+00014f60: 636f 6c2d 3132 2063 6f6c 2d6d 642d 347b  col-12 col-md-4{
+00014f70: 2520 656e 6462 6c6f 636b 2025 7d22 3e7b  % endblock %}">{
+00014f80: 7b20 335f 6d69 645f 626f 7474 6f6d 5f62  { 3_mid_bottom_b
+00014f90: 207d 7d3c 2f64 6976 3e0a 2020 2020 2020   }}</div>.      
+00014fa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014fb0: 2020 2020 2020 2020 2020 3c64 6976 2063            <div c
+00014fc0: 6c61 7373 3d22 7b25 2062 6c6f 636b 2033  lass="{% block 3
+00014fd0: 5f6d 6964 5f62 6f74 746f 6d5f 6162 635f  _mid_bottom_abc_
+00014fe0: 6320 257d 636f 6c2d 3132 2063 6f6c 2d6d  c %}col-12 col-m
+00014ff0: 642d 347b 2520 656e 6462 6c6f 636b 2025  d-4{% endblock %
+00015000: 7d22 3e7b 7b20 335f 6d69 645f 626f 7474  }">{{ 3_mid_bott
+00015010: 6f6d 5f63 207d 7d3c 2f64 6976 3e0a 2020  om_c }}</div>.  
+00015020: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015030: 2020 2020 2020 2020 2020 7b25 2065 6c69            {% eli
+00015040: 6620 335f 6d69 645f 626f 7474 6f6d 5f61  f 3_mid_bottom_a
+00015050: 2061 6e64 2033 5f6d 6964 5f62 6f74 746f   and 3_mid_botto
+00015060: 6d5f 6220 257d 0a20 2020 2020 2020 2020  m_b %}.         
+00015070: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015080: 2020 2020 2020 203c 6469 7620 636c 6173         <div clas
+00015090: 733d 227b 2520 626c 6f63 6b20 335f 6d69  s="{% block 3_mi
+000150a0: 645f 626f 7474 6f6d 5f61 625f 6120 257d  d_bottom_ab_a %}
+000150b0: 636f 6c2d 3132 2063 6f6c 2d6d 642d 387b  col-12 col-md-8{
+000150c0: 2520 656e 6462 6c6f 636b 2025 7d22 3e7b  % endblock %}">{
+000150d0: 7b20 335f 6d69 645f 626f 7474 6f6d 5f61  { 3_mid_bottom_a
+000150e0: 207d 7d3c 2f64 6976 3e0a 2020 2020 2020   }}</div>.      
 000150f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015100: 2020 3c2f 6469 763e 0a20 2020 2020 2020    </div>.       
-00015110: 2020 2020 2020 2020 2020 2020 207b 2520               {% 
-00015120: 656e 6469 6620 257d 0a0a 2020 2020 2020  endif %}..      
-00015130: 2020 2020 2020 2020 2020 2020 2020 3c21                <!
-00015140: 2d2d 2042 6c6f 636b 7320 696e 2062 6f74  -- Blocks in bot
-00015150: 746f 6d20 706f 7369 7469 6f6e 202d 2d3e  tom position -->
-00015160: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00015170: 2020 2020 207b 2520 6966 2033 5f62 6f74       {% if 3_bot
-00015180: 746f 6d5f 6120 6f72 2033 5f62 6f74 746f  tom_a or 3_botto
-00015190: 6d5f 6220 6f72 2033 5f62 6f74 746f 6d5f  m_b or 3_bottom_
-000151a0: 6320 257d 0a20 2020 2020 2020 2020 2020  c %}.           
-000151b0: 2020 2020 2020 2020 203c 6469 7620 636c           <div cl
-000151c0: 6173 733d 2263 6f6c 2d31 3222 3e0a 2020  ass="col-12">.  
-000151d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000151e0: 2020 2020 2020 3c64 6976 2063 6c61 7373        <div class
-000151f0: 3d22 726f 7722 3e0a 2020 2020 2020 2020  ="row">.        
-00015200: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015210: 2020 2020 7b25 2069 6620 335f 626f 7474      {% if 3_bott
-00015220: 6f6d 5f61 2061 6e64 2033 5f62 6f74 746f  om_a and 3_botto
-00015230: 6d5f 6220 616e 6420 335f 626f 7474 6f6d  m_b and 3_bottom
-00015240: 5f63 2025 7d0a 2020 2020 2020 2020 2020  _c %}.          
-00015250: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015260: 2020 2020 2020 3c64 6976 2063 6c61 7373        <div class
-00015270: 3d22 7b25 2062 6c6f 636b 2033 5f62 6f74  ="{% block 3_bot
-00015280: 746f 6d5f 6162 635f 6120 257d 636f 6c2d  tom_abc_a %}col-
-00015290: 3132 2063 6f6c 2d6d 642d 347b 2520 656e  12 col-md-4{% en
-000152a0: 6462 6c6f 636b 2025 7d22 3e7b 7b20 335f  dblock %}">{{ 3_
-000152b0: 626f 7474 6f6d 5f61 207d 7d3c 2f64 6976  bottom_a }}</div
-000152c0: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
-000152d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000152e0: 2020 3c64 6976 2063 6c61 7373 3d22 7b25    <div class="{%
-000152f0: 2062 6c6f 636b 2033 5f62 6f74 746f 6d5f   block 3_bottom_
-00015300: 6162 635f 6220 257d 636f 6c2d 3132 2063  abc_b %}col-12 c
-00015310: 6f6c 2d6d 642d 347b 2520 656e 6462 6c6f  ol-md-4{% endblo
-00015320: 636b 2025 7d22 3e7b 7b20 335f 626f 7474  ck %}">{{ 3_bott
-00015330: 6f6d 5f62 207d 7d3c 2f64 6976 3e0a 2020  om_b }}</div>.  
-00015340: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015350: 2020 2020 2020 2020 2020 2020 2020 3c64                <d
-00015360: 6976 2063 6c61 7373 3d22 7b25 2062 6c6f  iv class="{% blo
-00015370: 636b 2033 5f62 6f74 746f 6d5f 6162 635f  ck 3_bottom_abc_
-00015380: 6320 257d 636f 6c2d 3132 2063 6f6c 2d6d  c %}col-12 col-m
-00015390: 642d 347b 2520 656e 6462 6c6f 636b 2025  d-4{% endblock %
-000153a0: 7d22 3e7b 7b20 335f 626f 7474 6f6d 5f63  }">{{ 3_bottom_c
-000153b0: 207d 7d3c 2f64 6976 3e0a 2020 2020 2020   }}</div>.      
-000153c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000153d0: 2020 2020 2020 7b25 2065 6c69 6620 335f        {% elif 3_
-000153e0: 626f 7474 6f6d 5f61 2061 6e64 2033 5f62  bottom_a and 3_b
-000153f0: 6f74 746f 6d5f 6220 257d 0a20 2020 2020  ottom_b %}.     
-00015400: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015410: 2020 2020 2020 2020 2020 203c 6469 7620             <div 
-00015420: 636c 6173 733d 227b 2520 626c 6f63 6b20  class="{% block 
-00015430: 335f 626f 7474 6f6d 5f61 625f 6120 257d  3_bottom_ab_a %}
-00015440: 636f 6c2d 3132 2063 6f6c 2d6d 642d 387b  col-12 col-md-8{
-00015450: 2520 656e 6462 6c6f 636b 2025 7d22 3e7b  % endblock %}">{
-00015460: 7b20 335f 626f 7474 6f6d 5f61 207d 7d3c  { 3_bottom_a }}<
-00015470: 2f64 6976 3e0a 2020 2020 2020 2020 2020  /div>.          
-00015480: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015490: 2020 2020 2020 3c64 6976 2063 6c61 7373        <div class
-000154a0: 3d22 7b25 2062 6c6f 636b 2033 5f62 6f74  ="{% block 3_bot
-000154b0: 746f 6d5f 6162 5f62 2025 7d63 6f6c 2d31  tom_ab_b %}col-1
-000154c0: 3220 636f 6c2d 6d64 2d34 7b25 2065 6e64  2 col-md-4{% end
-000154d0: 626c 6f63 6b20 257d 223e 7b7b 2033 5f62  block %}">{{ 3_b
-000154e0: 6f74 746f 6d5f 6220 7d7d 3c2f 6469 763e  ottom_b }}</div>
-000154f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00015500: 2020 2020 2020 2020 2020 2020 207b 2520               {% 
-00015510: 656c 6966 2033 5f62 6f74 746f 6d5f 6120  elif 3_bottom_a 
-00015520: 616e 6420 335f 626f 7474 6f6d 5f63 2025  and 3_bottom_c %
-00015530: 7d0a 2020 2020 2020 2020 2020 2020 2020  }.              
-00015540: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015550: 2020 3c64 6976 2063 6c61 7373 3d22 7b25    <div class="{%
-00015560: 2062 6c6f 636b 2033 5f62 6f74 746f 6d5f   block 3_bottom_
-00015570: 6163 5f61 2025 7d63 6f6c 2d31 3220 636f  ac_a %}col-12 co
-00015580: 6c2d 6d64 2d36 7b25 2065 6e64 626c 6f63  l-md-6{% endbloc
-00015590: 6b20 257d 223e 7b7b 2033 5f62 6f74 746f  k %}">{{ 3_botto
-000155a0: 6d5f 6120 7d7d 3c2f 6469 763e 0a20 2020  m_a }}</div>.   
-000155b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000155c0: 2020 2020 2020 2020 2020 2020 203c 6469               <di
-000155d0: 7620 636c 6173 733d 227b 2520 626c 6f63  v class="{% bloc
-000155e0: 6b20 335f 626f 7474 6f6d 5f61 635f 6320  k 3_bottom_ac_c 
-000155f0: 257d 636f 6c2d 3132 2063 6f6c 2d6d 642d  %}col-12 col-md-
-00015600: 367b 2520 656e 6462 6c6f 636b 2025 7d22  6{% endblock %}"
-00015610: 3e7b 7b20 335f 626f 7474 6f6d 5f63 207d  >{{ 3_bottom_c }
-00015620: 7d3c 2f64 6976 3e0a 2020 2020 2020 2020  }</div>.        
-00015630: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015640: 2020 2020 7b25 2065 6c69 6620 335f 626f      {% elif 3_bo
-00015650: 7474 6f6d 5f62 2061 6e64 2033 5f62 6f74  ttom_b and 3_bot
-00015660: 746f 6d5f 6320 257d 0a20 2020 2020 2020  tom_c %}.       
-00015670: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015680: 2020 2020 2020 2020 203c 6469 7620 636c           <div cl
-00015690: 6173 733d 227b 2520 626c 6f63 6b20 335f  ass="{% block 3_
-000156a0: 626f 7474 6f6d 5f62 635f 6220 257d 636f  bottom_bc_b %}co
-000156b0: 6c2d 3132 2063 6f6c 2d6d 642d 347b 2520  l-12 col-md-4{% 
-000156c0: 656e 6462 6c6f 636b 2025 7d22 3e7b 7b20  endblock %}">{{ 
-000156d0: 335f 626f 7474 6f6d 5f62 207d 7d3c 2f64  3_bottom_b }}</d
-000156e0: 6976 3e0a 2020 2020 2020 2020 2020 2020  iv>.            
-000156f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015700: 2020 2020 3c64 6976 2063 6c61 7373 3d22      <div class="
-00015710: 7b25 2062 6c6f 636b 2033 5f62 6f74 746f  {% block 3_botto
-00015720: 6d5f 6263 5f63 2025 7d63 6f6c 2d31 3220  m_bc_c %}col-12 
-00015730: 636f 6c2d 6d64 2d38 7b25 2065 6e64 626c  col-md-8{% endbl
-00015740: 6f63 6b20 257d 223e 7b7b 2033 5f62 6f74  ock %}">{{ 3_bot
-00015750: 746f 6d5f 6320 7d7d 3c2f 6469 763e 0a20  tom_c }}</div>. 
-00015760: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015770: 2020 2020 2020 2020 2020 207b 2520 656c             {% el
-00015780: 7365 2025 7d0a 2020 2020 2020 2020 2020  se %}.          
-00015790: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000157a0: 2020 2020 2020 3c64 6976 2063 6c61 7373        <div class
-000157b0: 3d22 636f 6c2d 3132 223e 7b7b 2033 5f62  ="col-12">{{ 3_b
-000157c0: 6f74 746f 6d5f 6120 7d7d 7b7b 2033 5f62  ottom_a }}{{ 3_b
-000157d0: 6f74 746f 6d5f 6220 7d7d 7b7b 2033 5f62  ottom_b }}{{ 3_b
-000157e0: 6f74 746f 6d5f 6320 7d7d 3c2f 6469 763e  ottom_c }}</div>
-000157f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00015800: 2020 2020 2020 2020 2020 2020 207b 2520               {% 
-00015810: 656e 6469 6620 257d 0a20 2020 2020 2020  endif %}.       
-00015820: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015830: 203c 2f64 6976 3e0a 2020 2020 2020 2020   </div>.        
-00015840: 2020 2020 2020 2020 2020 2020 3c2f 6469              </di
-00015850: 763e 0a20 2020 2020 2020 2020 2020 2020  v>.             
-00015860: 2020 2020 2020 207b 2520 656e 6469 6620         {% endif 
-00015870: 257d 0a0a 2020 2020 2020 2020 2020 2020  %}..            
-00015880: 2020 2020 3c2f 6469 763e 0a20 2020 2020      </div>.     
-00015890: 2020 2020 2020 203c 2f64 6976 3e0a 2020         </div>.  
-000158a0: 2020 2020 2020 3c2f 6469 763e 0a20 2020        </div>.   
-000158b0: 207b 2520 656e 6469 6620 257d 0a20 2020   {% endif %}.   
-000158c0: 207b 2520 656e 6462 6c6f 636b 2073 6563   {% endblock sec
-000158d0: 7469 6f6e 5f33 2025 7d0a 2020 2020 3c21  tion_3 %}.    <!
-000158e0: 2d2d 2065 6e64 2053 6563 7469 6f6e 2033  -- end Section 3
-000158f0: 202d 2d3e 0a0a 2020 2020 7b25 2063 6f6d   -->..    {% com
-00015900: 6d65 6e74 2025 7d0a 2020 2020 3c64 6976  ment %}.    <div
-00015910: 2063 6c61 7373 3d22 636f 6f6b 6965 6261   class="cookieba
-00015920: 7222 3e0a 2020 2020 2020 2020 3c70 3e7b  r">.        <p>{
-00015930: 2520 7472 616e 7320 2251 7565 7374 6f20  % trans "Questo 
-00015940: 7369 746f 2075 7469 6c69 7a7a 6120 636f  sito utilizza co
-00015950: 6f6b 6965 2074 6563 6e69 6369 2c20 616e  okie tecnici, an
-00015960: 616c 7974 6963 7320 6520 6469 2074 6572  alytics e di ter
-00015970: 7a65 2070 6172 7469 2e22 2025 7d0a 2020  ze parti." %}.  
-00015980: 2020 2020 2020 2020 203c 6272 3e0a 2020           <br>.  
-00015990: 2020 2020 2020 2020 207b 2520 7472 616e           {% tran
-000159a0: 7320 2250 726f 7365 6775 656e 646f 206e  s "Proseguendo n
-000159b0: 656c 6c61 206e 6176 6967 617a 696f 6e65  ella navigazione
-000159c0: 2061 6363 6574 7469 206c e280 9975 7469   accetti l...uti
-000159d0: 6c69 7a7a 6f20 6465 6920 636f 6f6b 6965  lizzo dei cookie
-000159e0: 2e22 2025 7d0a 2020 2020 2020 2020 3c2f  ." %}.        </
-000159f0: 703e 0a20 2020 2020 2020 203c 6469 7620  p>.        <div 
-00015a00: 636c 6173 733d 2263 6f6f 6b69 6562 6172  class="cookiebar
-00015a10: 2d62 7574 746f 6e73 223e 0a20 2020 2020  -buttons">.     
-00015a20: 2020 2020 2020 203c 6120 6872 6566 3d22         <a href="
-00015a30: 2322 2063 6c61 7373 3d22 636f 6f6b 6965  #" class="cookie
-00015a40: 6261 722d 6274 6e22 3e0a 2020 2020 2020  bar-btn">.      
-00015a50: 2020 2020 2020 2020 2020 7b25 2074 7261            {% tra
-00015a60: 6e73 2022 5072 6566 6572 656e 7a65 2220  ns "Preferenze" 
-00015a70: 257d 203c 7370 616e 2063 6c61 7373 3d22  %} <span class="
-00015a80: 7669 7375 616c 6c79 2d68 6964 6465 6e22  visually-hidden"
-00015a90: 3e63 6f6f 6b69 6573 3c2f 7370 616e 3e0a  >cookies</span>.
-00015aa0: 2020 2020 2020 2020 2020 2020 3c2f 613e              </a>
-00015ab0: 0a20 2020 2020 2020 2020 2020 203c 6275  .            <bu
-00015ac0: 7474 6f6e 2064 6174 612d 6163 6365 7074  tton data-accept
-00015ad0: 3d22 636f 6f6b 6965 6261 7222 2063 6c61  ="cookiebar" cla
-00015ae0: 7373 3d22 636f 6f6b 6965 6261 722d 6274  ss="cookiebar-bt
-00015af0: 6e20 636f 6f6b 6965 6261 722d 636f 6e66  n cookiebar-conf
-00015b00: 6972 6d22 3e0a 2020 2020 2020 2020 2020  irm">.          
-00015b10: 2020 2020 2020 7b25 2074 7261 6e73 2022        {% trans "
-00015b20: 4163 6365 7474 6f22 2025 7d3c 7370 616e  Accetto" %}<span
-00015b30: 2063 6c61 7373 3d22 7669 7375 616c 6c79   class="visually
-00015b40: 2d68 6964 6465 6e22 3e20 6920 636f 6f6b  -hidden"> i cook
-00015b50: 6965 733c 2f73 7061 6e3e 0a20 2020 2020  ies</span>.     
-00015b60: 2020 2020 2020 203c 2f62 7574 746f 6e3e         </button>
-00015b70: 0a20 2020 2020 2020 203c 2f64 6976 3e0a  .        </div>.
-00015b80: 2020 2020 3c2f 6469 763e 0a20 2020 207b      </div>.    {
-00015b90: 2520 656e 6463 6f6d 6d65 6e74 2025 7d0a  % endcomment %}.
-00015ba0: 0a20 2020 203c 6120 6872 6566 3d22 2322  .    <a href="#"
-00015bb0: 0a20 2020 2020 2020 6172 6961 2d68 6964  .       aria-hid
-00015bc0: 6465 6e3d 2274 7275 6522 0a20 2020 2020  den="true".     
-00015bd0: 2020 6461 7461 2d62 732d 746f 6767 6c65    data-bs-toggle
-00015be0: 3d22 6261 636b 746f 746f 7022 0a20 2020  ="backtotop".   
-00015bf0: 2020 2020 636c 6173 733d 2262 6163 6b2d      class="back-
-00015c00: 746f 2d74 6f70 2062 6163 6b2d 746f 2d74  to-top back-to-t
-00015c10: 6f70 2d73 6d61 6c6c 223e 0a20 2020 2020  op-small">.     
-00015c20: 2020 203c 7376 6720 636c 6173 733d 2269     <svg class="i
-00015c30: 636f 6e20 6963 6f6e 2d6c 6967 6874 223e  con icon-light">
-00015c40: 0a20 2020 2020 2020 2020 2020 203c 7573  .            <us
-00015c50: 6520 786c 696e 6b3a 6872 6566 3d22 7b25  e xlink:href="{%
-00015c60: 2073 7461 7469 6320 2773 7667 2f73 7072   static 'svg/spr
-00015c70: 6974 6573 2e73 7667 2720 257d 2369 742d  ites.svg' %}#it-
-00015c80: 6172 726f 772d 7570 223e 3c2f 7573 653e  arrow-up"></use>
-00015c90: 0a20 2020 2020 2020 203c 2f73 7667 3e0a  .        </svg>.
-00015ca0: 2020 2020 3c2f 613e 0a7b 2520 656e 6462      </a>.{% endb
-00015cb0: 6c6f 636b 2063 6f6e 7461 696e 6572 2025  lock container %
-00015cc0: 7d0a 3c21 2d2d 2065 6e64 2043 6f6e 7461  }.<!-- end Conta
-00015cd0: 696e 6572 202d 2d3e 0a0a 7b25 2062 6c6f  iner -->..{% blo
-00015ce0: 636b 2065 7874 7261 5f73 6372 6970 7473  ck extra_scripts
-00015cf0: 2025 7d0a 7b7b 2062 6c6f 636b 2e73 7570   %}.{{ block.sup
-00015d00: 6572 207d 7d0a 3c73 6372 6970 7420 7372  er }}.<script sr
-00015d10: 633d 227b 2520 756e 6963 6d73 5f74 656d  c="{% unicms_tem
-00015d20: 706c 6174 655f 6974 616c 6961 5f73 7461  plate_italia_sta
-00015d30: 7469 635f 7061 7468 2027 6a73 2f70 6173  tic_path 'js/pas
-00015d40: 7369 7665 5f6c 6973 7465 6e65 7273 2e6a  sive_listeners.j
-00015d50: 7327 2025 7d22 3e3c 2f73 6372 6970 743e  s' %}"></script>
-00015d60: 0a3c 7363 7269 7074 2073 7263 3d22 7b25  .<script src="{%
-00015d70: 2075 6e69 636d 735f 7465 6d70 6c61 7465   unicms_template
-00015d80: 5f69 7461 6c69 615f 7374 6174 6963 5f70  _italia_static_p
-00015d90: 6174 6820 276a 732f 6465 6665 7272 6564  ath 'js/deferred
-00015da0: 5f69 6672 616d 655f 7372 632e 6a73 2720  _iframe_src.js' 
-00015db0: 257d 223e 3c2f 7363 7269 7074 3e0a 7b25  %}"></script>.{%
-00015dc0: 2073 6574 7469 6e67 735f 7661 6c75 6520   settings_value 
-00015dd0: 2243 4d53 5f50 4154 485f 5052 4546 4958  "CMS_PATH_PREFIX
-00015de0: 2220 6173 2063 6d73 5f70 6174 685f 7072  " as cms_path_pr
-00015df0: 6566 6978 2025 7d0a 7b25 2069 6e63 6c75  efix %}.{% inclu
-00015e00: 6465 2022 696e 6974 732f 7365 6172 6368  de "inits/search
-00015e10: 2d69 6e70 7574 2d68 616e 646c 6572 2e68  -input-handler.h
-00015e20: 746d 6c22 2077 6974 6820 636d 735f 7061  tml" with cms_pa
-00015e30: 7468 5f70 7265 6669 783d 636d 735f 7061  th_prefix=cms_pa
-00015e40: 7468 5f70 7265 6669 7820 257d 0a7b 2520  th_prefix %}.{% 
-00015e50: 656e 6462 6c6f 636b 2065 7874 7261 5f73  endblock extra_s
-00015e60: 6372 6970 7473 2025 7d0a                 cripts %}.
+00015100: 2020 2020 2020 2020 2020 3c64 6976 2063            <div c
+00015110: 6c61 7373 3d22 7b25 2062 6c6f 636b 2033  lass="{% block 3
+00015120: 5f6d 6964 5f62 6f74 746f 6d5f 6162 5f62  _mid_bottom_ab_b
+00015130: 2025 7d63 6f6c 2d31 3220 636f 6c2d 6d64   %}col-12 col-md
+00015140: 2d34 7b25 2065 6e64 626c 6f63 6b20 257d  -4{% endblock %}
+00015150: 223e 7b7b 2033 5f6d 6964 5f62 6f74 746f  ">{{ 3_mid_botto
+00015160: 6d5f 6220 7d7d 3c2f 6469 763e 0a20 2020  m_b }}</div>.   
+00015170: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015180: 2020 2020 2020 2020 207b 2520 656c 6966           {% elif
+00015190: 2033 5f6d 6964 5f62 6f74 746f 6d5f 6120   3_mid_bottom_a 
+000151a0: 616e 6420 335f 6d69 645f 626f 7474 6f6d  and 3_mid_bottom
+000151b0: 5f63 2025 7d0a 2020 2020 2020 2020 2020  _c %}.          
+000151c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000151d0: 2020 2020 2020 3c64 6976 2063 6c61 7373        <div class
+000151e0: 3d22 7b25 2062 6c6f 636b 2033 5f6d 6964  ="{% block 3_mid
+000151f0: 5f62 6f74 746f 6d5f 6163 5f61 2025 7d63  _bottom_ac_a %}c
+00015200: 6f6c 2d31 3220 636f 6c2d 6d64 2d36 7b25  ol-12 col-md-6{%
+00015210: 2065 6e64 626c 6f63 6b20 257d 223e 7b7b   endblock %}">{{
+00015220: 2033 5f6d 6964 5f62 6f74 746f 6d5f 6120   3_mid_bottom_a 
+00015230: 7d7d 3c2f 6469 763e 0a20 2020 2020 2020  }}</div>.       
+00015240: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015250: 2020 2020 2020 2020 203c 6469 7620 636c           <div cl
+00015260: 6173 733d 227b 2520 626c 6f63 6b20 335f  ass="{% block 3_
+00015270: 6d69 645f 626f 7474 6f6d 5f61 635f 6320  mid_bottom_ac_c 
+00015280: 257d 636f 6c2d 3132 2063 6f6c 2d6d 642d  %}col-12 col-md-
+00015290: 367b 2520 656e 6462 6c6f 636b 2025 7d22  6{% endblock %}"
+000152a0: 3e7b 7b20 335f 6d69 645f 626f 7474 6f6d  >{{ 3_mid_bottom
+000152b0: 5f63 207d 7d3c 2f64 6976 3e0a 2020 2020  _c }}</div>.    
+000152c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000152d0: 2020 2020 2020 2020 7b25 2065 6c69 6620          {% elif 
+000152e0: 335f 6d69 645f 626f 7474 6f6d 5f62 2061  3_mid_bottom_b a
+000152f0: 6e64 2033 5f6d 6964 5f62 6f74 746f 6d5f  nd 3_mid_bottom_
+00015300: 6320 257d 0a20 2020 2020 2020 2020 2020  c %}.           
+00015310: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015320: 2020 2020 203c 6469 7620 636c 6173 733d       <div class=
+00015330: 227b 2520 626c 6f63 6b20 335f 6d69 645f  "{% block 3_mid_
+00015340: 626f 7474 6f6d 5f62 635f 6220 257d 636f  bottom_bc_b %}co
+00015350: 6c2d 3132 2063 6f6c 2d6d 642d 347b 2520  l-12 col-md-4{% 
+00015360: 656e 6462 6c6f 636b 2025 7d22 3e7b 7b20  endblock %}">{{ 
+00015370: 335f 6d69 645f 626f 7474 6f6d 5f62 207d  3_mid_bottom_b }
+00015380: 7d3c 2f64 6976 3e0a 2020 2020 2020 2020  }</div>.        
+00015390: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000153a0: 2020 2020 2020 2020 3c64 6976 2063 6c61          <div cla
+000153b0: 7373 3d22 7b25 2062 6c6f 636b 2033 5f6d  ss="{% block 3_m
+000153c0: 6964 5f62 6f74 746f 6d5f 6263 5f63 2025  id_bottom_bc_c %
+000153d0: 7d63 6f6c 2d31 3220 636f 6c2d 6d64 2d38  }col-12 col-md-8
+000153e0: 7b25 2065 6e64 626c 6f63 6b20 257d 223e  {% endblock %}">
+000153f0: 7b7b 2033 5f6d 6964 5f62 6f74 746f 6d5f  {{ 3_mid_bottom_
+00015400: 6320 7d7d 3c2f 6469 763e 0a20 2020 2020  c }}</div>.     
+00015410: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015420: 2020 2020 2020 207b 2520 656c 7365 2025         {% else %
+00015430: 7d0a 2020 2020 2020 2020 2020 2020 2020  }.              
+00015440: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015450: 2020 3c64 6976 2063 6c61 7373 3d22 636f    <div class="co
+00015460: 6c2d 3132 223e 7b7b 2033 5f6d 6964 5f62  l-12">{{ 3_mid_b
+00015470: 6f74 746f 6d5f 6120 7d7d 7b7b 2033 5f6d  ottom_a }}{{ 3_m
+00015480: 6964 5f62 6f74 746f 6d5f 6220 7d7d 7b7b  id_bottom_b }}{{
+00015490: 2033 5f6d 6964 5f62 6f74 746f 6d5f 6320   3_mid_bottom_c 
+000154a0: 7d7d 3c2f 6469 763e 0a20 2020 2020 2020  }}</div>.       
+000154b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000154c0: 2020 2020 207b 2520 656e 6469 6620 257d       {% endif %}
+000154d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000154e0: 2020 2020 2020 2020 203c 2f64 6976 3e0a           </div>.
+000154f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015500: 2020 2020 3c2f 6469 763e 0a20 2020 2020      </div>.     
+00015510: 2020 2020 2020 2020 2020 2020 2020 207b                 {
+00015520: 2520 656e 6469 6620 257d 0a0a 2020 2020  % endif %}..    
+00015530: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015540: 3c21 2d2d 2042 6c6f 636b 7320 696e 2062  <!-- Blocks in b
+00015550: 6f74 746f 6d20 706f 7369 7469 6f6e 202d  ottom position -
+00015560: 2d3e 0a20 2020 2020 2020 2020 2020 2020  ->.             
+00015570: 2020 2020 2020 207b 2520 6966 2033 5f62         {% if 3_b
+00015580: 6f74 746f 6d5f 6120 6f72 2033 5f62 6f74  ottom_a or 3_bot
+00015590: 746f 6d5f 6220 6f72 2033 5f62 6f74 746f  tom_b or 3_botto
+000155a0: 6d5f 6320 257d 0a20 2020 2020 2020 2020  m_c %}.         
+000155b0: 2020 2020 2020 2020 2020 203c 6469 7620             <div 
+000155c0: 636c 6173 733d 2263 6f6c 2d31 3222 3e0a  class="col-12">.
+000155d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000155e0: 2020 2020 2020 2020 3c64 6976 2063 6c61          <div cla
+000155f0: 7373 3d22 726f 7722 3e0a 2020 2020 2020  ss="row">.      
+00015600: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015610: 2020 2020 2020 7b25 2069 6620 335f 626f        {% if 3_bo
+00015620: 7474 6f6d 5f61 2061 6e64 2033 5f62 6f74  ttom_a and 3_bot
+00015630: 746f 6d5f 6220 616e 6420 335f 626f 7474  tom_b and 3_bott
+00015640: 6f6d 5f63 2025 7d0a 2020 2020 2020 2020  om_c %}.        
+00015650: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015660: 2020 2020 2020 2020 3c64 6976 2063 6c61          <div cla
+00015670: 7373 3d22 7b25 2062 6c6f 636b 2033 5f62  ss="{% block 3_b
+00015680: 6f74 746f 6d5f 6162 635f 6120 257d 636f  ottom_abc_a %}co
+00015690: 6c2d 3132 2063 6f6c 2d6d 642d 347b 2520  l-12 col-md-4{% 
+000156a0: 656e 6462 6c6f 636b 2025 7d22 3e7b 7b20  endblock %}">{{ 
+000156b0: 335f 626f 7474 6f6d 5f61 207d 7d3c 2f64  3_bottom_a }}</d
+000156c0: 6976 3e0a 2020 2020 2020 2020 2020 2020  iv>.            
+000156d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000156e0: 2020 2020 3c64 6976 2063 6c61 7373 3d22      <div class="
+000156f0: 7b25 2062 6c6f 636b 2033 5f62 6f74 746f  {% block 3_botto
+00015700: 6d5f 6162 635f 6220 257d 636f 6c2d 3132  m_abc_b %}col-12
+00015710: 2063 6f6c 2d6d 642d 347b 2520 656e 6462   col-md-4{% endb
+00015720: 6c6f 636b 2025 7d22 3e7b 7b20 335f 626f  lock %}">{{ 3_bo
+00015730: 7474 6f6d 5f62 207d 7d3c 2f64 6976 3e0a  ttom_b }}</div>.
+00015740: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015750: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015760: 3c64 6976 2063 6c61 7373 3d22 7b25 2062  <div class="{% b
+00015770: 6c6f 636b 2033 5f62 6f74 746f 6d5f 6162  lock 3_bottom_ab
+00015780: 635f 6320 257d 636f 6c2d 3132 2063 6f6c  c_c %}col-12 col
+00015790: 2d6d 642d 347b 2520 656e 6462 6c6f 636b  -md-4{% endblock
+000157a0: 2025 7d22 3e7b 7b20 335f 626f 7474 6f6d   %}">{{ 3_bottom
+000157b0: 5f63 207d 7d3c 2f64 6976 3e0a 2020 2020  _c }}</div>.    
+000157c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000157d0: 2020 2020 2020 2020 7b25 2065 6c69 6620          {% elif 
+000157e0: 335f 626f 7474 6f6d 5f61 2061 6e64 2033  3_bottom_a and 3
+000157f0: 5f62 6f74 746f 6d5f 6220 257d 0a20 2020  _bottom_b %}.   
+00015800: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015810: 2020 2020 2020 2020 2020 2020 203c 6469               <di
+00015820: 7620 636c 6173 733d 227b 2520 626c 6f63  v class="{% bloc
+00015830: 6b20 335f 626f 7474 6f6d 5f61 625f 6120  k 3_bottom_ab_a 
+00015840: 257d 636f 6c2d 3132 2063 6f6c 2d6d 642d  %}col-12 col-md-
+00015850: 387b 2520 656e 6462 6c6f 636b 2025 7d22  8{% endblock %}"
+00015860: 3e7b 7b20 335f 626f 7474 6f6d 5f61 207d  >{{ 3_bottom_a }
+00015870: 7d3c 2f64 6976 3e0a 2020 2020 2020 2020  }</div>.        
+00015880: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015890: 2020 2020 2020 2020 3c64 6976 2063 6c61          <div cla
+000158a0: 7373 3d22 7b25 2062 6c6f 636b 2033 5f62  ss="{% block 3_b
+000158b0: 6f74 746f 6d5f 6162 5f62 2025 7d63 6f6c  ottom_ab_b %}col
+000158c0: 2d31 3220 636f 6c2d 6d64 2d34 7b25 2065  -12 col-md-4{% e
+000158d0: 6e64 626c 6f63 6b20 257d 223e 7b7b 2033  ndblock %}">{{ 3
+000158e0: 5f62 6f74 746f 6d5f 6220 7d7d 3c2f 6469  _bottom_b }}</di
+000158f0: 763e 0a20 2020 2020 2020 2020 2020 2020  v>.             
+00015900: 2020 2020 2020 2020 2020 2020 2020 207b                 {
+00015910: 2520 656c 6966 2033 5f62 6f74 746f 6d5f  % elif 3_bottom_
+00015920: 6120 616e 6420 335f 626f 7474 6f6d 5f63  a and 3_bottom_c
+00015930: 2025 7d0a 2020 2020 2020 2020 2020 2020   %}.            
+00015940: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015950: 2020 2020 3c64 6976 2063 6c61 7373 3d22      <div class="
+00015960: 7b25 2062 6c6f 636b 2033 5f62 6f74 746f  {% block 3_botto
+00015970: 6d5f 6163 5f61 2025 7d63 6f6c 2d31 3220  m_ac_a %}col-12 
+00015980: 636f 6c2d 6d64 2d36 7b25 2065 6e64 626c  col-md-6{% endbl
+00015990: 6f63 6b20 257d 223e 7b7b 2033 5f62 6f74  ock %}">{{ 3_bot
+000159a0: 746f 6d5f 6120 7d7d 3c2f 6469 763e 0a20  tom_a }}</div>. 
+000159b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000159c0: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+000159d0: 6469 7620 636c 6173 733d 227b 2520 626c  div class="{% bl
+000159e0: 6f63 6b20 335f 626f 7474 6f6d 5f61 635f  ock 3_bottom_ac_
+000159f0: 6320 257d 636f 6c2d 3132 2063 6f6c 2d6d  c %}col-12 col-m
+00015a00: 642d 367b 2520 656e 6462 6c6f 636b 2025  d-6{% endblock %
+00015a10: 7d22 3e7b 7b20 335f 626f 7474 6f6d 5f63  }">{{ 3_bottom_c
+00015a20: 207d 7d3c 2f64 6976 3e0a 2020 2020 2020   }}</div>.      
+00015a30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015a40: 2020 2020 2020 7b25 2065 6c69 6620 335f        {% elif 3_
+00015a50: 626f 7474 6f6d 5f62 2061 6e64 2033 5f62  bottom_b and 3_b
+00015a60: 6f74 746f 6d5f 6320 257d 0a20 2020 2020  ottom_c %}.     
+00015a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015a80: 2020 2020 2020 2020 2020 203c 6469 7620             <div 
+00015a90: 636c 6173 733d 227b 2520 626c 6f63 6b20  class="{% block 
+00015aa0: 335f 626f 7474 6f6d 5f62 635f 6220 257d  3_bottom_bc_b %}
+00015ab0: 636f 6c2d 3132 2063 6f6c 2d6d 642d 347b  col-12 col-md-4{
+00015ac0: 2520 656e 6462 6c6f 636b 2025 7d22 3e7b  % endblock %}">{
+00015ad0: 7b20 335f 626f 7474 6f6d 5f62 207d 7d3c  { 3_bottom_b }}<
+00015ae0: 2f64 6976 3e0a 2020 2020 2020 2020 2020  /div>.          
+00015af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015b00: 2020 2020 2020 3c64 6976 2063 6c61 7373        <div class
+00015b10: 3d22 7b25 2062 6c6f 636b 2033 5f62 6f74  ="{% block 3_bot
+00015b20: 746f 6d5f 6263 5f63 2025 7d63 6f6c 2d31  tom_bc_c %}col-1
+00015b30: 3220 636f 6c2d 6d64 2d38 7b25 2065 6e64  2 col-md-8{% end
+00015b40: 626c 6f63 6b20 257d 223e 7b7b 2033 5f62  block %}">{{ 3_b
+00015b50: 6f74 746f 6d5f 6320 7d7d 3c2f 6469 763e  ottom_c }}</div>
+00015b60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00015b70: 2020 2020 2020 2020 2020 2020 207b 2520               {% 
+00015b80: 656c 7365 2025 7d0a 2020 2020 2020 2020  else %}.        
+00015b90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015ba0: 2020 2020 2020 2020 3c64 6976 2063 6c61          <div cla
+00015bb0: 7373 3d22 636f 6c2d 3132 223e 7b7b 2033  ss="col-12">{{ 3
+00015bc0: 5f62 6f74 746f 6d5f 6120 7d7d 7b7b 2033  _bottom_a }}{{ 3
+00015bd0: 5f62 6f74 746f 6d5f 6220 7d7d 7b7b 2033  _bottom_b }}{{ 3
+00015be0: 5f62 6f74 746f 6d5f 6320 7d7d 3c2f 6469  _bottom_c }}</di
+00015bf0: 763e 0a20 2020 2020 2020 2020 2020 2020  v>.             
+00015c00: 2020 2020 2020 2020 2020 2020 2020 207b                 {
+00015c10: 2520 656e 6469 6620 257d 0a20 2020 2020  % endif %}.     
+00015c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015c30: 2020 203c 2f64 6976 3e0a 2020 2020 2020     </div>.      
+00015c40: 2020 2020 2020 2020 2020 2020 2020 3c2f                </
+00015c50: 6469 763e 0a20 2020 2020 2020 2020 2020  div>.           
+00015c60: 2020 2020 2020 2020 207b 2520 656e 6469           {% endi
+00015c70: 6620 257d 0a0a 2020 2020 2020 2020 2020  f %}..          
+00015c80: 2020 2020 2020 3c2f 6469 763e 0a20 2020        </div>.   
+00015c90: 2020 2020 2020 2020 203c 2f64 6976 3e0a           </div>.
+00015ca0: 2020 2020 2020 2020 3c2f 6469 763e 0a20          </div>. 
+00015cb0: 2020 207b 2520 656e 6469 6620 257d 0a20     {% endif %}. 
+00015cc0: 2020 207b 2520 656e 6462 6c6f 636b 2073     {% endblock s
+00015cd0: 6563 7469 6f6e 5f33 2025 7d0a 2020 2020  ection_3 %}.    
+00015ce0: 3c21 2d2d 2065 6e64 2053 6563 7469 6f6e  <!-- end Section
+00015cf0: 2033 202d 2d3e 0a0a 2020 2020 7b25 2063   3 -->..    {% c
+00015d00: 6f6d 6d65 6e74 2025 7d0a 2020 2020 3c64  omment %}.    <d
+00015d10: 6976 2063 6c61 7373 3d22 636f 6f6b 6965  iv class="cookie
+00015d20: 6261 7222 3e0a 2020 2020 2020 2020 3c70  bar">.        <p
+00015d30: 3e7b 2520 7472 616e 7320 2251 7565 7374  >{% trans "Quest
+00015d40: 6f20 7369 746f 2075 7469 6c69 7a7a 6120  o sito utilizza 
+00015d50: 636f 6f6b 6965 2074 6563 6e69 6369 2c20  cookie tecnici, 
+00015d60: 616e 616c 7974 6963 7320 6520 6469 2074  analytics e di t
+00015d70: 6572 7a65 2070 6172 7469 2e22 2025 7d0a  erze parti." %}.
+00015d80: 2020 2020 2020 2020 2020 203c 6272 3e0a             <br>.
+00015d90: 2020 2020 2020 2020 2020 207b 2520 7472             {% tr
+00015da0: 616e 7320 2250 726f 7365 6775 656e 646f  ans "Proseguendo
+00015db0: 206e 656c 6c61 206e 6176 6967 617a 696f   nella navigazio
+00015dc0: 6e65 2061 6363 6574 7469 206c e280 9975  ne accetti l...u
+00015dd0: 7469 6c69 7a7a 6f20 6465 6920 636f 6f6b  tilizzo dei cook
+00015de0: 6965 2e22 2025 7d0a 2020 2020 2020 2020  ie." %}.        
+00015df0: 3c2f 703e 0a20 2020 2020 2020 203c 6469  </p>.        <di
+00015e00: 7620 636c 6173 733d 2263 6f6f 6b69 6562  v class="cookieb
+00015e10: 6172 2d62 7574 746f 6e73 223e 0a20 2020  ar-buttons">.   
+00015e20: 2020 2020 2020 2020 203c 6120 6872 6566           <a href
+00015e30: 3d22 2322 2063 6c61 7373 3d22 636f 6f6b  ="#" class="cook
+00015e40: 6965 6261 722d 6274 6e22 3e0a 2020 2020  iebar-btn">.    
+00015e50: 2020 2020 2020 2020 2020 2020 7b25 2074              {% t
+00015e60: 7261 6e73 2022 5072 6566 6572 656e 7a65  rans "Preferenze
+00015e70: 2220 257d 203c 7370 616e 2063 6c61 7373  " %} <span class
+00015e80: 3d22 7669 7375 616c 6c79 2d68 6964 6465  ="visually-hidde
+00015e90: 6e22 3e63 6f6f 6b69 6573 3c2f 7370 616e  n">cookies</span
+00015ea0: 3e0a 2020 2020 2020 2020 2020 2020 3c2f  >.            </
+00015eb0: 613e 0a20 2020 2020 2020 2020 2020 203c  a>.            <
+00015ec0: 6275 7474 6f6e 2064 6174 612d 6163 6365  button data-acce
+00015ed0: 7074 3d22 636f 6f6b 6965 6261 7222 2063  pt="cookiebar" c
+00015ee0: 6c61 7373 3d22 636f 6f6b 6965 6261 722d  lass="cookiebar-
+00015ef0: 6274 6e20 636f 6f6b 6965 6261 722d 636f  btn cookiebar-co
+00015f00: 6e66 6972 6d22 3e0a 2020 2020 2020 2020  nfirm">.        
+00015f10: 2020 2020 2020 2020 7b25 2074 7261 6e73          {% trans
+00015f20: 2022 4163 6365 7474 6f22 2025 7d3c 7370   "Accetto" %}<sp
+00015f30: 616e 2063 6c61 7373 3d22 7669 7375 616c  an class="visual
+00015f40: 6c79 2d68 6964 6465 6e22 3e20 6920 636f  ly-hidden"> i co
+00015f50: 6f6b 6965 733c 2f73 7061 6e3e 0a20 2020  okies</span>.   
+00015f60: 2020 2020 2020 2020 203c 2f62 7574 746f           </butto
+00015f70: 6e3e 0a20 2020 2020 2020 203c 2f64 6976  n>.        </div
+00015f80: 3e0a 2020 2020 3c2f 6469 763e 0a20 2020  >.    </div>.   
+00015f90: 207b 2520 656e 6463 6f6d 6d65 6e74 2025   {% endcomment %
+00015fa0: 7d0a 0a20 2020 203c 6120 6872 6566 3d22  }..    <a href="
+00015fb0: 2322 0a20 2020 2020 2020 6172 6961 2d68  #".       aria-h
+00015fc0: 6964 6465 6e3d 2274 7275 6522 0a20 2020  idden="true".   
+00015fd0: 2020 2020 6461 7461 2d62 732d 746f 6767      data-bs-togg
+00015fe0: 6c65 3d22 6261 636b 746f 746f 7022 0a20  le="backtotop". 
+00015ff0: 2020 2020 2020 636c 6173 733d 2262 6163        class="bac
+00016000: 6b2d 746f 2d74 6f70 2062 6163 6b2d 746f  k-to-top back-to
+00016010: 2d74 6f70 2d73 6d61 6c6c 223e 0a20 2020  -top-small">.   
+00016020: 2020 2020 203c 7376 6720 636c 6173 733d       <svg class=
+00016030: 2269 636f 6e20 6963 6f6e 2d6c 6967 6874  "icon icon-light
+00016040: 223e 0a20 2020 2020 2020 2020 2020 203c  ">.            <
+00016050: 7573 6520 786c 696e 6b3a 6872 6566 3d22  use xlink:href="
+00016060: 7b25 2073 7461 7469 6320 2773 7667 2f73  {% static 'svg/s
+00016070: 7072 6974 6573 2e73 7667 2720 257d 2369  prites.svg' %}#i
+00016080: 742d 6172 726f 772d 7570 223e 3c2f 7573  t-arrow-up"></us
+00016090: 653e 0a20 2020 2020 2020 203c 2f73 7667  e>.        </svg
+000160a0: 3e0a 2020 2020 3c2f 613e 0a7b 2520 656e  >.    </a>.{% en
+000160b0: 6462 6c6f 636b 2063 6f6e 7461 696e 6572  dblock container
+000160c0: 2025 7d0a 3c21 2d2d 2065 6e64 2043 6f6e   %}.<!-- end Con
+000160d0: 7461 696e 6572 202d 2d3e 0a0a 7b25 2062  tainer -->..{% b
+000160e0: 6c6f 636b 2065 7874 7261 5f73 6372 6970  lock extra_scrip
+000160f0: 7473 2025 7d0a 7b7b 2062 6c6f 636b 2e73  ts %}.{{ block.s
+00016100: 7570 6572 207d 7d0a 3c73 6372 6970 7420  uper }}.<script 
+00016110: 7372 633d 227b 2520 756e 6963 6d73 5f74  src="{% unicms_t
+00016120: 656d 706c 6174 655f 6974 616c 6961 5f73  emplate_italia_s
+00016130: 7461 7469 635f 7061 7468 2027 6a73 2f70  tatic_path 'js/p
+00016140: 6173 7369 7665 5f6c 6973 7465 6e65 7273  assive_listeners
+00016150: 2e6a 7327 2025 7d22 3e3c 2f73 6372 6970  .js' %}"></scrip
+00016160: 743e 0a3c 7363 7269 7074 2073 7263 3d22  t>.<script src="
+00016170: 7b25 2075 6e69 636d 735f 7465 6d70 6c61  {% unicms_templa
+00016180: 7465 5f69 7461 6c69 615f 7374 6174 6963  te_italia_static
+00016190: 5f70 6174 6820 276a 732f 6465 6665 7272  _path 'js/deferr
+000161a0: 6564 5f69 6672 616d 655f 7372 632e 6a73  ed_iframe_src.js
+000161b0: 2720 257d 223e 3c2f 7363 7269 7074 3e0a  ' %}"></script>.
+000161c0: 7b25 2073 6574 7469 6e67 735f 7661 6c75  {% settings_valu
+000161d0: 6520 2243 4d53 5f50 4154 485f 5052 4546  e "CMS_PATH_PREF
+000161e0: 4958 2220 6173 2063 6d73 5f70 6174 685f  IX" as cms_path_
+000161f0: 7072 6566 6978 2025 7d0a 7b25 2069 6e63  prefix %}.{% inc
+00016200: 6c75 6465 2022 696e 6974 732f 7365 6172  lude "inits/sear
+00016210: 6368 2d69 6e70 7574 2d68 616e 646c 6572  ch-input-handler
+00016220: 2e68 746d 6c22 2077 6974 6820 636d 735f  .html" with cms_
+00016230: 7061 7468 5f70 7265 6669 783d 636d 735f  path_prefix=cms_
+00016240: 7061 7468 5f70 7265 6669 7820 257d 0a0a  path_prefix %}..
+00016250: 7b25 2062 6c6f 636b 2068 746d 6c5f 626f  {% block html_bo
+00016260: 7474 6f6d 2025 7d0a 2020 2020 7b25 206c  ttom %}.    {% l
+00016270: 6f61 645f 626c 6f63 6b73 2073 6563 7469  oad_blocks secti
+00016280: 6f6e 3d22 6874 6d6c 2d62 6f74 746f 6d22  on="html-bottom"
+00016290: 2061 7320 6874 6d6c 5f62 6f74 746f 6d20   as html_bottom 
+000162a0: 257d 0a20 2020 207b 7b20 6874 6d6c 5f62  %}.    {{ html_b
+000162b0: 6f74 746f 6d20 7d7d 0a7b 2520 656e 6462  ottom }}.{% endb
+000162c0: 6c6f 636b 2068 746d 6c5f 626f 7474 6f6d  lock html_bottom
+000162d0: 2025 7d0a 7b25 2065 6e64 626c 6f63 6b20   %}.{% endblock 
+000162e0: 6578 7472 615f 7363 7269 7074 7320 257d  extra_scripts %}
+000162f0: 0a                                       .
```

### Comparing `unicms_template_italia-1.0.3/src/unicms_template_italia/templates/blocks/italia_carousel_hero_slider.html` & `unicms_template_italia-1.1.0/src/unicms_template_italia/templates/blocks/italia_carousel_hero_slider.html`

 * *Files identical despite different names*

### Comparing `unicms_template_italia-1.0.3/src/unicms_template_italia/templates/blocks/italia_media_collection_image_grid.html` & `unicms_template_italia-1.1.0/src/unicms_template_italia/templates/blocks/italia_media_collection_image_grid.html`

 * *Files identical despite different names*

### Comparing `unicms_template_italia-1.0.3/src/unicms_template_italia/templates/blocks/italia_media_collection_image_slider.html` & `unicms_template_italia-1.1.0/src/unicms_template_italia/templates/blocks/italia_media_collection_image_slider.html`

 * *Files identical despite different names*

### Comparing `unicms_template_italia-1.0.3/src/unicms_template_italia/templates/blocks/italia_media_collection_image_slider_full.html` & `unicms_template_italia-1.1.0/src/unicms_template_italia/templates/blocks/italia_media_collection_image_slider_full.html`

 * *Files identical despite different names*

### Comparing `unicms_template_italia-1.0.3/src/unicms_template_italia/templates/blocks/italia_media_collection_list.html` & `unicms_template_italia-1.1.0/src/unicms_template_italia/templates/blocks/italia_media_collection_list.html`

 * *Files identical despite different names*

### Comparing `unicms_template_italia-1.0.3/src/unicms_template_italia/templates/blocks/italia_menu_main.html` & `unicms_template_italia-1.1.0/src/unicms_template_italia/templates/blocks/italia_menu_main.html`

 * *Files identical despite different names*

### Comparing `unicms_template_italia-1.0.3/src/unicms_template_italia/templates/blocks/italia_menu_side.html` & `unicms_template_italia-1.1.0/src/unicms_template_italia/templates/blocks/italia_menu_side.html`

 * *Files identical despite different names*

### Comparing `unicms_template_italia-1.0.3/src/unicms_template_italia/templates/blocks/italia_pub_alert.html` & `unicms_template_italia-1.1.0/src/unicms_template_italia/templates/blocks/italia_pub_alert.html`

 * *Files identical despite different names*

### Comparing `unicms_template_italia-1.0.3/src/unicms_template_italia/templates/blocks/italia_pub_collapse.html` & `unicms_template_italia-1.1.0/src/unicms_template_italia/templates/blocks/italia_pub_collapse.html`

 * *Files identical despite different names*

### Comparing `unicms_template_italia-1.0.3/src/unicms_template_italia/templates/blocks/italia_pub_collapse_logo_image.html` & `unicms_template_italia-1.1.0/src/unicms_template_italia/templates/blocks/italia_pub_collapse_logo_image.html`

 * *Files identical despite different names*

### Comparing `unicms_template_italia-1.0.3/src/unicms_template_italia/templates/blocks/italia_search_engine.html` & `unicms_template_italia-1.1.0/src/unicms_template_italia/templates/blocks/italia_search_engine.html`

 * *Files 1% similar despite different names*

```diff
@@ -111,15 +111,15 @@
                                                 </label>
                                                 <input
                                                     id="date_from"
                                                     type="date"
                                                     placeholder="{% trans 'From publishing date' %}">
                                             </div>
                                             <div class="col-sm mt-5 mt-sm-0">
-                                                <label for="date_from" style="font-size: .7777777778rem; margin-top: -30px">
+                                                <label for="date_to" style="font-size: .7777777778rem; margin-top: -30px">
                                                     {% trans 'To publishing date' %}
                                                 </label>
                                                 <input
                                                     id="date_to"
                                                     type="date"
                                                     placeholder="{% trans 'To publishing date' %}">
                                             </div>
@@ -163,20 +163,14 @@
                                                         {% for site, domain in sites %}
                                                             {% if '*' in allowed_search_sites or domain in allowed_search_sites %}
                                                             <option value="{{ domain }}">
                                                                 {{ domain }}
                                                             </option>
                                                             {% endif %}
                                                         {% endfor %}
-                                                        {% cms_categories as categories %}
-                                                        {% for cat in categories %}
-                                                        <option value="{{ cat }}">
-                                                            {{ cat }}
-                                                        </option>
-                                                        {% endfor %}
                                                       </select>
                                                 </div>
                                             </div>
                                         </div>
                                     </div>
                                     {% endif %}
                                 </div>
```

### Comparing `unicms_template_italia-1.0.3/src/unicms_template_italia/templates/components/italia_editorialboard_frontend_menu.html` & `unicms_template_italia-1.1.0/src/unicms_template_italia/templates/components/italia_editorialboard_frontend_menu.html`

 * *Files identical despite different names*

### Comparing `unicms_template_italia-1.0.3/src/unicms_template_italia/templates/includes/social_share.html` & `unicms_template_italia-1.1.0/src/unicms_template_italia/templates/includes/social_share.html`

 * *Files identical despite different names*

### Comparing `unicms_template_italia-1.0.3/src/unicms_template_italia/templatetags/unicms_template_italia.py` & `unicms_template_italia-1.1.0/src/unicms_template_italia/templatetags/unicms_template_italia.py`

 * *Files identical despite different names*

### Comparing `unicms_template_italia-1.0.3/unicms_template_italia.egg-info/PKG-INFO` & `unicms_template_italia-1.1.0/unicms_template_italia.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unicms-template-italia
-Version: 1.0.3
+Version: 1.1.0
 Summary: uniCMS Template based on Bootstrap Italia design
 Home-page: https://github.com/UniversitaDellaCalabria/unicms-template-italia
 Author: Giuseppe De Marco, Francesco Filicetti
 Author-email: giuseppe.demarco@unical.it, francesco.filicetti@unical.it
 License: Apache License 2.0
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `unicms_template_italia-1.0.3/unicms_template_italia.egg-info/SOURCES.txt` & `unicms_template_italia-1.1.0/unicms_template_italia.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 src/unicms_template_italia/settings.py
 src/unicms_template_italia/locale/it/LC_MESSAGES/django.mo
 src/unicms_template_italia/locale/it/LC_MESSAGES/django.po
 src/unicms_template_italia/static/css/vendor/owl.carousel.min.css
 src/unicms_template_italia/static/js/axios.1.1.3.js
 src/unicms_template_italia/static/js/axios.min.js.map
 src/unicms_template_italia/static/js/deferred_iframe_src.js
+src/unicms_template_italia/static/js/jquery.3.6.3.min.js
 src/unicms_template_italia/static/js/passive_listeners.js
 src/unicms_template_italia/static/js/vue.2.7.14.js
 src/unicms_template_italia/static/js/vue.options.js
 src/unicms_template_italia/static/js/vendor/owl.carousel.min.js
 src/unicms_template_italia/templates/bases/unicms_italia.html
 src/unicms_template_italia/templates/blocks/italia_carousel_hero_slider.html
 src/unicms_template_italia/templates/blocks/italia_heading.html
```

