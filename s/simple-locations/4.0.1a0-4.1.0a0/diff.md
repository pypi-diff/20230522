# Comparing `tmp/simple_locations-4.0.1a0.tar.gz` & `tmp/simple_locations-4.1.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simple_locations-4.0.1a0.tar", max compression
+gzip compressed data, was "simple_locations-4.1.0a0.tar", max compression
```

## Comparing `simple_locations-4.0.1a0.tar` & `simple_locations-4.1.0a0.tar`

### file list

```diff
@@ -1,66 +1,64 @@
--rw-r--r--   0        0        0     2339 2023-03-27 07:57:29.884293 simple_locations-4.0.1a0/README.md
--rw-r--r--   0        0        0     1587 2023-03-27 07:58:43.984066 simple_locations-4.0.1a0/pyproject.toml
--rw-r--r--   0        0        0        0 2022-04-13 00:21:55.695397 simple_locations-4.0.1a0/simple_locations/__init__.py
--rw-r--r--   0        0        0     1599 2022-04-14 01:38:42.132188 simple_locations-4.0.1a0/simple_locations/admin.py
--rw-r--r--   0        0        0      143 2023-03-27 07:57:37.771328 simple_locations-4.0.1a0/simple_locations/api.py
--rw-r--r--   0        0        0     2973 2023-03-27 07:57:37.771328 simple_locations-4.0.1a0/simple_locations/feature_manager.py
--rw-r--r--   0        0        0      595 2022-04-13 00:21:55.695397 simple_locations-4.0.1a0/simple_locations/fixtures/initial_data.json
--rw-r--r--   0        0        0     1874 2022-04-14 01:38:42.132188 simple_locations-4.0.1a0/simple_locations/forms.py
--rw-r--r--   0        0        0     3592 2023-03-27 07:57:37.772328 simple_locations-4.0.1a0/simple_locations/gis_functions.py
--rw-r--r--   0        0        0     1116 2022-04-13 00:21:55.695397 simple_locations-4.0.1a0/simple_locations/locale/fr/LC_MESSAGES/django.po
--rw-r--r--   0        0        0        0 2022-04-13 00:21:55.695397 simple_locations-4.0.1a0/simple_locations/management/__init__.py
--rw-r--r--   0        0        0        0 2022-04-13 00:21:55.695397 simple_locations-4.0.1a0/simple_locations/management/commands/__init__.py
--rw-r--r--   0        0        0     6709 2023-03-27 07:57:37.773328 simple_locations-4.0.1a0/simple_locations/management/commands/create_borders.py
--rw-r--r--   0        0        0      725 2023-03-27 07:57:37.774328 simple_locations-4.0.1a0/simple_locations/management/commands/create_projected_areas.py
--rw-r--r--   0        0        0      712 2023-03-27 07:57:37.774328 simple_locations-4.0.1a0/simple_locations/management/commands/dump_locations.py
--rw-r--r--   0        0        0    10538 2023-03-27 07:57:37.774328 simple_locations-4.0.1a0/simple_locations/management/commands/import_dird.py
--rw-r--r--   0        0        0     2032 2023-03-27 07:57:37.775328 simple_locations-4.0.1a0/simple_locations/manager.py
--rw-r--r--   0        0        0     4814 2022-04-14 01:38:42.132188 simple_locations-4.0.1a0/simple_locations/migrations/0001_initial.py
--rw-r--r--   0        0        0      546 2022-04-14 01:38:42.132188 simple_locations-4.0.1a0/simple_locations/migrations/0002_load_initial_data.py
--rw-r--r--   0        0        0      505 2022-04-13 00:21:55.695397 simple_locations-4.0.1a0/simple_locations/migrations/0003_auto_20170320_1024.py
--rw-r--r--   0        0        0     1326 2022-04-13 00:21:55.695397 simple_locations-4.0.1a0/simple_locations/migrations/0004_auto_20170330_1618.py
--rw-r--r--   0        0        0      506 2022-04-13 00:21:55.695397 simple_locations-4.0.1a0/simple_locations/migrations/0005_auto_20170403_1507.py
--rw-r--r--   0        0        0      412 2022-04-13 00:21:55.695397 simple_locations-4.0.1a0/simple_locations/migrations/0006_auto_20180202_1540.py
--rw-r--r--   0        0        0      548 2022-04-13 00:21:55.695397 simple_locations-4.0.1a0/simple_locations/migrations/0007_area_geom_can_be_blank.py
--rw-r--r--   0        0        0     2284 2022-04-14 01:38:42.132188 simple_locations-4.0.1a0/simple_locations/migrations/0008_auto_20200804_0554.py
--rw-r--r--   0        0        0      404 2022-04-14 01:38:42.132188 simple_locations-4.0.1a0/simple_locations/migrations/0009_auto_20211111_0805.py
--rw-r--r--   0        0        0      675 2022-04-14 01:38:42.133188 simple_locations-4.0.1a0/simple_locations/migrations/0010_add_border_model.py
--rw-r--r--   0        0        0      725 2022-04-14 01:38:42.133188 simple_locations-4.0.1a0/simple_locations/migrations/0011_denormed_border_fields.py
--rw-r--r--   0        0        0     1034 2022-04-14 01:38:42.133188 simple_locations-4.0.1a0/simple_locations/migrations/0012_auto_20220221_0817.py
--rw-r--r--   0        0        0     1120 2022-04-14 01:38:42.133188 simple_locations-4.0.1a0/simple_locations/migrations/0013_auto_20220307_0618.py
--rw-r--r--   0        0        0        0 2022-04-13 00:21:55.695397 simple_locations-4.0.1a0/simple_locations/migrations/__init__.py
--rw-r--r--   0        0        0      346 2023-03-27 07:57:37.776328 simple_locations-4.0.1a0/simple_locations/model_schemas.py
--rw-r--r--   0        0        0     8308 2023-03-27 07:57:37.776328 simple_locations-4.0.1a0/simple_locations/models.py
--rw-r--r--   0        0        0     1710 2023-03-27 07:57:37.776328 simple_locations-4.0.1a0/simple_locations/models.pyi
--rw-r--r--   0        0        0      125 2023-03-27 07:57:37.777328 simple_locations-4.0.1a0/simple_locations/requirements.in
--rw-r--r--   0        0        0     2549 2023-03-27 07:57:37.777328 simple_locations-4.0.1a0/simple_locations/router.py
--rw-r--r--   0        0        0      971 2023-03-27 07:57:37.777328 simple_locations-4.0.1a0/simple_locations/schemas.py
--rw-r--r--   0        0        0        0 2022-04-14 01:38:42.133188 simple_locations-4.0.1a0/simple_locations/settings.py
--rw-r--r--   0        0        0     1993 2022-04-13 00:21:55.695397 simple_locations-4.0.1a0/simple_locations/static/css/tree-default-line.gif
--rw-r--r--   0        0        0     2281 2022-04-13 00:21:55.695397 simple_locations-4.0.1a0/simple_locations/static/css/tree.css
--rw-r--r--   0        0        0     3208 2022-04-13 00:21:55.695397 simple_locations-4.0.1a0/simple_locations/static/images/ajax-loader.gif
--rwxr-xr-x   0        0        0      715 2022-04-13 00:21:55.695397 simple_locations-4.0.1a0/simple_locations/static/images/delete.png
--rwxr-xr-x   0        0        0      618 2022-04-13 00:21:55.695397 simple_locations-4.0.1a0/simple_locations/static/images/edit.png
--rw-r--r--   0        0        0      837 2022-04-13 00:21:55.695397 simple_locations-4.0.1a0/simple_locations/static/images/minus.gif
--rw-r--r--   0        0        0      841 2022-04-13 00:21:55.696397 simple_locations-4.0.1a0/simple_locations/static/images/plus.gif
--rw-r--r--   0        0        0     1993 2022-04-13 00:21:55.696397 simple_locations-4.0.1a0/simple_locations/static/images/tree-default-line.gif
--rw-r--r--   0        0        0     2606 2022-04-13 00:21:55.696397 simple_locations-4.0.1a0/simple_locations/static/javascripts/simple_locations.js
--rw-r--r--   0        0        0     6826 2022-04-13 00:21:55.696397 simple_locations-4.0.1a0/simple_locations/static/uni_form/blue.uni-form.css
--rw-r--r--   0        0        0     6283 2022-04-13 00:21:55.696397 simple_locations-4.0.1a0/simple_locations/static/uni_form/dark.uni-form.css
--rw-r--r--   0        0        0     6696 2022-04-13 00:21:55.696397 simple_locations-4.0.1a0/simple_locations/static/uni_form/default.uni-form.css
--rwxr-xr-x   0        0        0    20976 2022-04-13 00:21:55.696397 simple_locations-4.0.1a0/simple_locations/static/uni_form/jquery.js
--rwxr-xr-x   0        0        0     7824 2022-04-13 00:21:55.696397 simple_locations-4.0.1a0/simple_locations/static/uni_form/uni-form.css
--rwxr-xr-x   0        0        0     1074 2022-04-13 00:21:55.696397 simple_locations-4.0.1a0/simple_locations/static/uni_form/uni-form.jquery.js
--rw-r--r--   0        0        0      124 2022-04-13 00:21:55.696397 simple_locations-4.0.1a0/simple_locations/templates/simple_locations/admin/osm.html
--rw-r--r--   0        0        0      182 2022-04-13 00:21:55.696397 simple_locations-4.0.1a0/simple_locations/templates/simple_locations/admin/osm.js
--rw-r--r--   0        0        0     1089 2022-04-13 00:21:55.696397 simple_locations-4.0.1a0/simple_locations/templates/simple_locations/index.html
--rw-r--r--   0        0        0      171 2022-04-13 00:21:55.696397 simple_locations-4.0.1a0/simple_locations/templates/simple_locations/layout-3-panel.html
--rw-r--r--   0        0        0     3376 2022-04-13 00:21:55.696397 simple_locations-4.0.1a0/simple_locations/templates/simple_locations/location_edit.html
--rw-r--r--   0        0        0      965 2022-04-13 00:21:55.696397 simple_locations-4.0.1a0/simple_locations/templates/simple_locations/map.html
--rw-r--r--   0        0        0     2046 2022-04-13 00:21:55.696397 simple_locations-4.0.1a0/simple_locations/templates/simple_locations/treepanel.html
--rw-r--r--   0        0        0      355 2023-03-20 07:14:10.527615 simple_locations-4.0.1a0/simple_locations/translation.py
--rw-r--r--   0        0        0     1139 2023-03-27 07:57:37.777328 simple_locations-4.0.1a0/simple_locations/urls.py
--rw-r--r--   0        0        0     7749 2023-03-27 07:57:37.778329 simple_locations-4.0.1a0/simple_locations/views.py
--rw-r--r--   0        0        0      415 2022-04-14 01:38:42.133188 simple_locations-4.0.1a0/simple_locations/wsgi.py
--rw-r--r--   0        0        0     3717 1970-01-01 00:00:00.000000 simple_locations-4.0.1a0/setup.py
--rw-r--r--   0        0        0     3219 1970-01-01 00:00:00.000000 simple_locations-4.0.1a0/PKG-INFO
+-rw-r--r--   0        0        0     2339 2023-05-22 03:26:52.172541 simple_locations-4.1.0a0/README.md
+-rw-r--r--   0        0        0     1671 2023-05-22 05:11:49.652986 simple_locations-4.1.0a0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-03 05:07:47.518712 simple_locations-4.1.0a0/simple_locations/__init__.py
+-rw-r--r--   0        0        0     1599 2023-05-22 03:26:52.176534 simple_locations-4.1.0a0/simple_locations/admin.py
+-rw-r--r--   0        0        0      143 2023-05-22 03:26:52.172541 simple_locations-4.1.0a0/simple_locations/api.py
+-rw-r--r--   0        0        0     2979 2023-05-22 03:54:05.996050 simple_locations-4.1.0a0/simple_locations/feature_manager.py
+-rw-r--r--   0        0        0      595 2023-04-03 05:07:47.518712 simple_locations-4.1.0a0/simple_locations/fixtures/initial_data.json
+-rw-r--r--   0        0        0     1874 2023-05-22 03:26:52.172541 simple_locations-4.1.0a0/simple_locations/forms.py
+-rw-r--r--   0        0        0     3654 2023-05-22 03:54:05.996050 simple_locations-4.1.0a0/simple_locations/gis_functions.py
+-rw-r--r--   0        0        0     1116 2023-04-03 05:07:47.518712 simple_locations-4.1.0a0/simple_locations/locale/fr/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0        0 2023-04-03 05:07:47.518712 simple_locations-4.1.0a0/simple_locations/management/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-03 05:07:47.518712 simple_locations-4.1.0a0/simple_locations/management/commands/__init__.py
+-rw-r--r--   0        0        0     6723 2023-05-22 03:56:12.240698 simple_locations-4.1.0a0/simple_locations/management/commands/create_borders.py
+-rw-r--r--   0        0        0      725 2023-05-22 03:26:52.172541 simple_locations-4.1.0a0/simple_locations/management/commands/create_projected_areas.py
+-rw-r--r--   0        0        0      712 2023-05-22 03:26:52.172541 simple_locations-4.1.0a0/simple_locations/management/commands/dump_locations.py
+-rw-r--r--   0        0        0    10530 2023-05-22 03:56:32.831755 simple_locations-4.1.0a0/simple_locations/management/commands/import_dird.py
+-rw-r--r--   0        0        0     2046 2023-05-22 03:56:50.506981 simple_locations-4.1.0a0/simple_locations/manager.py
+-rw-r--r--   0        0        0     4814 2023-05-22 03:57:14.709968 simple_locations-4.1.0a0/simple_locations/migrations/0001_initial.py
+-rw-r--r--   0        0        0      546 2023-05-22 03:26:52.172541 simple_locations-4.1.0a0/simple_locations/migrations/0002_load_initial_data.py
+-rw-r--r--   0        0        0      505 2023-04-03 05:07:47.522712 simple_locations-4.1.0a0/simple_locations/migrations/0003_auto_20170320_1024.py
+-rw-r--r--   0        0        0     1326 2023-04-03 05:07:47.518712 simple_locations-4.1.0a0/simple_locations/migrations/0004_auto_20170330_1618.py
+-rw-r--r--   0        0        0      506 2023-04-03 05:07:47.518712 simple_locations-4.1.0a0/simple_locations/migrations/0005_auto_20170403_1507.py
+-rw-r--r--   0        0        0      412 2023-04-03 05:07:47.518712 simple_locations-4.1.0a0/simple_locations/migrations/0006_auto_20180202_1540.py
+-rw-r--r--   0        0        0      548 2023-04-03 05:07:47.518712 simple_locations-4.1.0a0/simple_locations/migrations/0007_area_geom_can_be_blank.py
+-rw-r--r--   0        0        0     2284 2023-05-22 03:57:14.709968 simple_locations-4.1.0a0/simple_locations/migrations/0008_auto_20200804_0554.py
+-rw-r--r--   0        0        0      404 2023-05-22 03:26:52.172541 simple_locations-4.1.0a0/simple_locations/migrations/0009_auto_20211111_0805.py
+-rw-r--r--   0        0        0      675 2023-05-22 03:26:52.172541 simple_locations-4.1.0a0/simple_locations/migrations/0010_add_border_model.py
+-rw-r--r--   0        0        0      725 2023-05-22 03:26:52.172541 simple_locations-4.1.0a0/simple_locations/migrations/0011_denormed_border_fields.py
+-rw-r--r--   0        0        0     1034 2023-05-22 03:26:52.172541 simple_locations-4.1.0a0/simple_locations/migrations/0012_auto_20220221_0817.py
+-rw-r--r--   0        0        0     1120 2023-05-22 03:26:52.176534 simple_locations-4.1.0a0/simple_locations/migrations/0013_auto_20220307_0618.py
+-rw-r--r--   0        0        0        0 2023-04-03 05:07:47.518712 simple_locations-4.1.0a0/simple_locations/migrations/__init__.py
+-rw-r--r--   0        0        0      346 2023-05-22 03:26:52.176534 simple_locations-4.1.0a0/simple_locations/model_schemas.py
+-rw-r--r--   0        0        0     8308 2023-05-22 03:57:09.110198 simple_locations-4.1.0a0/simple_locations/models.py
+-rw-r--r--   0        0        0     1710 2023-05-22 03:26:52.172541 simple_locations-4.1.0a0/simple_locations/models.pyi
+-rw-r--r--   0        0        0      125 2023-05-22 03:26:52.176534 simple_locations-4.1.0a0/simple_locations/requirements.in
+-rw-r--r--   0        0        0     2541 2023-05-22 03:54:05.996050 simple_locations-4.1.0a0/simple_locations/router.py
+-rw-r--r--   0        0        0        0 2023-05-22 03:26:52.176534 simple_locations-4.1.0a0/simple_locations/settings.py
+-rw-r--r--   0        0        0     1993 2023-04-03 05:07:47.522712 simple_locations-4.1.0a0/simple_locations/static/css/tree-default-line.gif
+-rw-r--r--   0        0        0     2281 2023-04-03 05:07:47.522712 simple_locations-4.1.0a0/simple_locations/static/css/tree.css
+-rw-r--r--   0        0        0     3208 2023-04-03 05:07:47.522712 simple_locations-4.1.0a0/simple_locations/static/images/ajax-loader.gif
+-rwxr-xr-x   0        0        0      715 2023-04-03 05:07:47.522712 simple_locations-4.1.0a0/simple_locations/static/images/delete.png
+-rwxr-xr-x   0        0        0      618 2023-04-03 05:07:47.522712 simple_locations-4.1.0a0/simple_locations/static/images/edit.png
+-rw-r--r--   0        0        0      837 2023-04-03 05:07:47.522712 simple_locations-4.1.0a0/simple_locations/static/images/minus.gif
+-rw-r--r--   0        0        0      841 2023-04-03 05:07:47.522712 simple_locations-4.1.0a0/simple_locations/static/images/plus.gif
+-rw-r--r--   0        0        0     1993 2023-04-03 05:07:47.522712 simple_locations-4.1.0a0/simple_locations/static/images/tree-default-line.gif
+-rw-r--r--   0        0        0     2606 2023-04-03 05:07:47.522712 simple_locations-4.1.0a0/simple_locations/static/javascripts/simple_locations.js
+-rw-r--r--   0        0        0     6826 2023-04-03 05:07:47.522712 simple_locations-4.1.0a0/simple_locations/static/uni_form/blue.uni-form.css
+-rw-r--r--   0        0        0     6283 2023-04-03 05:07:47.522712 simple_locations-4.1.0a0/simple_locations/static/uni_form/dark.uni-form.css
+-rw-r--r--   0        0        0     6696 2023-04-03 05:07:47.522712 simple_locations-4.1.0a0/simple_locations/static/uni_form/default.uni-form.css
+-rwxr-xr-x   0        0        0    20976 2023-04-03 05:07:47.522712 simple_locations-4.1.0a0/simple_locations/static/uni_form/jquery.js
+-rwxr-xr-x   0        0        0     7824 2023-04-03 05:07:47.522712 simple_locations-4.1.0a0/simple_locations/static/uni_form/uni-form.css
+-rwxr-xr-x   0        0        0     1074 2023-04-03 05:07:47.522712 simple_locations-4.1.0a0/simple_locations/static/uni_form/uni-form.jquery.js
+-rw-r--r--   0        0        0      124 2023-04-03 05:07:47.522712 simple_locations-4.1.0a0/simple_locations/templates/simple_locations/admin/osm.html
+-rw-r--r--   0        0        0      182 2023-04-03 05:07:47.522712 simple_locations-4.1.0a0/simple_locations/templates/simple_locations/admin/osm.js
+-rw-r--r--   0        0        0     1089 2023-04-03 05:07:47.522712 simple_locations-4.1.0a0/simple_locations/templates/simple_locations/index.html
+-rw-r--r--   0        0        0      171 2023-04-03 05:07:47.522712 simple_locations-4.1.0a0/simple_locations/templates/simple_locations/layout-3-panel.html
+-rw-r--r--   0        0        0     3376 2023-04-03 05:07:47.522712 simple_locations-4.1.0a0/simple_locations/templates/simple_locations/location_edit.html
+-rw-r--r--   0        0        0      965 2023-04-03 05:07:47.522712 simple_locations-4.1.0a0/simple_locations/templates/simple_locations/map.html
+-rw-r--r--   0        0        0     2046 2023-04-03 05:07:47.522712 simple_locations-4.1.0a0/simple_locations/templates/simple_locations/treepanel.html
+-rw-r--r--   0        0        0      355 2023-05-22 03:26:52.176534 simple_locations-4.1.0a0/simple_locations/translation.py
+-rw-r--r--   0        0        0     1139 2023-05-22 03:26:52.176534 simple_locations-4.1.0a0/simple_locations/urls.py
+-rw-r--r--   0        0        0     7749 2023-05-22 03:26:52.176534 simple_locations-4.1.0a0/simple_locations/views.py
+-rw-r--r--   0        0        0      415 2023-05-22 03:26:52.176534 simple_locations-4.1.0a0/simple_locations/wsgi.py
+-rw-r--r--   0        0        0     3271 1970-01-01 00:00:00.000000 simple_locations-4.1.0a0/PKG-INFO
```

### Comparing `simple_locations-4.0.1a0/README.md` & `simple_locations-4.1.0a0/README.md`

 * *Files identical despite different names*

### Comparing `simple_locations-4.0.1a0/pyproject.toml` & `simple_locations-4.1.0a0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -13,17 +13,21 @@
   | \.tox
   | \.venv
   | env
   | migrations
 )/
 '''
 
+[tool.ruff]
+line-length = 119
+exclude = ['migrations']
+
 [tool.poetry]
 name = "simple-locations"
-version = "4.0.1a0"
+version = "4.1.0a0"
 description = "The common location package for Catalpa's projects"
 authors = [
   "Joshua Brooks <josh@catalpa.io>",
   "Anders Hofstee <anders@catalpa.io>",
   "Nicoas Hoibian <admin@catalpa.io>",
 ]
 license = "BSD"
@@ -32,28 +36,29 @@
 
 repository = "https://github.com/catalpainternational/simple_locations"
 homepage = "https://github.com/catalpainternational/simple_locations"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 django-mptt = "^0.14.0"
-pydantic = "^1.10.6"
-django-ninja = ">=0.20.0"
+pydantic = ">1.10.6,<2"
+django-ninja = "^0.21.0"
 django-geojson = "^4.0.0"
+geojson-pydantic = "^0.6.2"
 
 [tool.poetry.group.dev]
 optional = true
 
 [tool.poetry.group.dev.dependencies]
-black = {extras = ["jupyter"], version = ">=23.1.0"}
+black = {extras = ["jupyter"], version = "^23.1.0"}
 flake8 = "*"
 isort = "*"
 pre-commit = "*"
 mypy = "*"
-django-stubs = {extras = ["compatible-mypy"], version = ">=1.16.0"}
+django-stubs = {extras = ["compatible-mypy"], version = "^1.16.0"}
 psycopg2-binary = "*"
 pytest-django = "*"
 pytest-cov = "*"
 factory-boy = "*"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
```

### Comparing `simple_locations-4.0.1a0/simple_locations/admin.py` & `simple_locations-4.1.0a0/simple_locations/admin.py`

 * *Files identical despite different names*

### Comparing `simple_locations-4.0.1a0/simple_locations/feature_manager.py` & `simple_locations-4.1.0a0/simple_locations/feature_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import Generator, Union
 
 from django.db import models
+from geojson_pydantic import FeatureCollection, Feature
 
 from simple_locations.gis_functions import JsonFeature
-from simple_locations.schemas import Feature, FeatureCollection
 
 
 class FeatureQueryset(models.QuerySet):
     def to_featurecollection(
         self, simplify: Union[float, None] = None, quantize: Union[int, None] = None
     ) -> FeatureCollection:
         """
@@ -26,15 +26,15 @@
         ====================
         >>> from simple_locations.schemas import Feature
         >>> Feature.parse_obj(Area.geofunctions.all().annotate(JsonFeature()).first().feature)
         >>> # A list of features:
         >>> [Feature.parse_obj(i) for i in Area.geofunctions.filter(kind__name='district').to_features(simplify=1e-3, quantize=5).values_list('feature', flat=True)]
         >>> # A FeatureCollection:
         >>> FeatureCollection.parse_obj(queryset.aggregate(features = JSONBAgg(JsonFeature())))
-        """
+        """  # noqa: E501
         return FeatureCollection.construct(features=[*self.to_features(simplify=simplify, quantize=quantize)])
 
     def annotate_features(self, simplify: Union[float, None] = None, quantize: Union[int, None] = None):
         """
         Annotated 'feature' fields onto the queryset
         """
         return self.annotate(
```

### Comparing `simple_locations-4.0.1a0/simple_locations/fixtures/initial_data.json` & `simple_locations-4.1.0a0/simple_locations/fixtures/initial_data.json`

 * *Files identical despite different names*

### Comparing `simple_locations-4.0.1a0/simple_locations/forms.py` & `simple_locations-4.1.0a0/simple_locations/forms.py`

 * *Files identical despite different names*

### Comparing `simple_locations-4.0.1a0/simple_locations/gis_functions.py` & `simple_locations-4.1.0a0/simple_locations/gis_functions.py`

 * *Files 3% similar despite different names*

```diff
@@ -99,10 +99,11 @@
         g: Union[F, Func] = models.F(geom_field)
         if simplify:
             g = SimplifyPreserve(g, simplify=simplify)
         if quantize:
             g = Quantize(g, quantize=quantize)
         if multi:
             g = Multi(g)
+        expressions.extend((Value("type"), Value("Feature")))
         expressions.extend((Value("geometry"), AsGeoJson(g, bbox=bbox_, crs=crs_, precision=precision_)))
         expressions.extend((Value("properties"), JSONObject(**fields)))
         super().__init__(*expressions)
```

### Comparing `simple_locations-4.0.1a0/simple_locations/locale/fr/LC_MESSAGES/django.po` & `simple_locations-4.1.0a0/simple_locations/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `simple_locations-4.0.1a0/simple_locations/management/commands/create_borders.py` & `simple_locations-4.1.0a0/simple_locations/management/commands/create_borders.py`

 * *Files 1% similar despite different names*

```diff
@@ -101,15 +101,15 @@
 
     update_border_area_array = """
         with areas as (select border_id, array_agg(area_id) as area_ids from simple_locations_border_area group by border_id)
         update simple_locations_border b set area_ids =
             (select areas.area_ids from areas
             where areas.border_id = b.id)
             where b.id in (select border_id from areas)
-    """
+    """  # noqa: E501
 
     update_border_type_array = """
 
         with area_types as (
             select border_id, array_agg(distinct slt.id) area_types from simple_locations_area sla,
                 simple_locations_areatype slt,
                 simple_locations_border_area slba
```

### Comparing `simple_locations-4.0.1a0/simple_locations/management/commands/create_projected_areas.py` & `simple_locations-4.1.0a0/simple_locations/management/commands/create_projected_areas.py`

 * *Files identical despite different names*

### Comparing `simple_locations-4.0.1a0/simple_locations/management/commands/dump_locations.py` & `simple_locations-4.1.0a0/simple_locations/management/commands/dump_locations.py`

 * *Files identical despite different names*

### Comparing `simple_locations-4.0.1a0/simple_locations/management/commands/import_dird.py` & `simple_locations-4.1.0a0/simple_locations/management/commands/import_dird.py`

 * *Files 0% similar despite different names*

```diff
@@ -231,15 +231,15 @@
         Vanimo-Green River District	Vanimo/Green River District
         Wabag District	Wabag District
         Wapenamanda District	Wapenamanda District
         Wewak District	Wewak District
         Wosera-Gawi District	Wosera Gawi District
         Yangoru-Saussia District	Yangoru Saussia District"""
 
-        renames = []  # type: List[RenameDistrict]
+        renames: List[RenameDistrict] = []
 
         for s in sources.split("\n"):
             n = s.split("\t")
             renames.append(RenameDistrict(n[1].strip(), n[0].strip()))
 
         # Area.objects.all().delete()
         self.stdout.write(self.style.MIGRATE_HEADING("~~~ Starting rename ~~~"))
```

### Comparing `simple_locations-4.0.1a0/simple_locations/manager.py` & `simple_locations-4.1.0a0/simple_locations/manager.py`

 * *Files 5% similar despite different names*

```diff
@@ -29,15 +29,15 @@
         geojson serializer but simplified, and carries out more operations in the DB including
         geometry simplifying and quantization
 
         This returns a string, in order to prevent multiple ser / de-ser calls
         """
 
         output = io.StringIO()  # Avoids a round-trip deserializer by using a raw StringIO
-        prefix = """{"type": "FeatureCollection", "crs": {"type": "name", "properties": {"name": "EPSG:4326"}}, "features": ["""
+        prefix = """{"type": "FeatureCollection", "crs": {"type": "name", "properties": {"name": "EPSG:4326"}}, "features": ["""  # noqa: E501
         pattern = '{"type": "Feature", "geometry": %s, "properties": {"id": %s } }'
         suffix = "]}"
 
         output.write(prefix)
         is_first = True
         for obj in self.filter(geom__isnull=False)._annotate_geometries(simplify=simplify, quantize=quantize):
             if is_first:
```

### Comparing `simple_locations-4.0.1a0/simple_locations/migrations/0001_initial.py` & `simple_locations-4.1.0a0/simple_locations/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `simple_locations-4.0.1a0/simple_locations/migrations/0002_load_initial_data.py` & `simple_locations-4.1.0a0/simple_locations/migrations/0002_load_initial_data.py`

 * *Files identical despite different names*

### Comparing `simple_locations-4.0.1a0/simple_locations/migrations/0004_auto_20170330_1618.py` & `simple_locations-4.1.0a0/simple_locations/migrations/0004_auto_20170330_1618.py`

 * *Files identical despite different names*

### Comparing `simple_locations-4.0.1a0/simple_locations/migrations/0007_area_geom_can_be_blank.py` & `simple_locations-4.1.0a0/simple_locations/migrations/0007_area_geom_can_be_blank.py`

 * *Files identical despite different names*

### Comparing `simple_locations-4.0.1a0/simple_locations/migrations/0008_auto_20200804_0554.py` & `simple_locations-4.1.0a0/simple_locations/migrations/0008_auto_20200804_0554.py`

 * *Files identical despite different names*

### Comparing `simple_locations-4.0.1a0/simple_locations/migrations/0010_add_border_model.py` & `simple_locations-4.1.0a0/simple_locations/migrations/0010_add_border_model.py`

 * *Files identical despite different names*

### Comparing `simple_locations-4.0.1a0/simple_locations/migrations/0011_denormed_border_fields.py` & `simple_locations-4.1.0a0/simple_locations/migrations/0011_denormed_border_fields.py`

 * *Files identical despite different names*

### Comparing `simple_locations-4.0.1a0/simple_locations/migrations/0012_auto_20220221_0817.py` & `simple_locations-4.1.0a0/simple_locations/migrations/0012_auto_20220221_0817.py`

 * *Files identical despite different names*

### Comparing `simple_locations-4.0.1a0/simple_locations/migrations/0013_auto_20220307_0618.py` & `simple_locations-4.1.0a0/simple_locations/migrations/0013_auto_20220307_0618.py`

 * *Files identical despite different names*

### Comparing `simple_locations-4.0.1a0/simple_locations/models.py` & `simple_locations-4.1.0a0/simple_locations/models.py`

 * *Files identical despite different names*

### Comparing `simple_locations-4.0.1a0/simple_locations/models.pyi` & `simple_locations-4.1.0a0/simple_locations/models.pyi`

 * *Files identical despite different names*

### Comparing `simple_locations-4.0.1a0/simple_locations/router.py` & `simple_locations-4.1.0a0/simple_locations/router.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 from typing import Generator, List, Tuple
 
 from ninja import Router
 
-from simple_locations import model_schemas, models, schemas
+from geojson_pydantic import FeatureCollection, Feature
+
+from simple_locations import model_schemas, models
 
 router = Router(tags=["SimpleLocations"])
 
 SIMPLIFICATION_LEVELS: Tuple[float, ...] = (0.0, 0.0001, 0.001, 0.01, 0.1, 0.5)
 
 
 @router.get("/area/list.json", response=List[model_schemas.AreaModelSchema])
@@ -21,54 +23,54 @@
 def area_type_list(request):
     """
     List the different area types
     """
     return models.AreaType.objects.all()
 
 
-@router.get("/area/by-id/{area_id}.geojson", response=schemas.Feature)
+@router.get("/area/by-id/{area_id}.geojson", response=Feature)
 def area_id(request, area_id: int):
     """
     Returns the geometry of a single Area
     as a single GeoJSON Feature
     """
-    features: Generator[schemas.Feature, None, None] = models.Area.features.filter(pk=area_id).to_features()
-    return schemas.Feature.parse_obj(next(features))
+    features: Generator[Feature, None, None] = models.Area.features.filter(pk=area_id).to_features()
+    return Feature.parse_obj(next(features))
 
 
-@router.get("/area/by-parent/{area_id}-s{simplify}-q{quantize}.geojson", response=schemas.FeatureCollection)
+@router.get("/area/by-parent/{area_id}-s{simplify}-q{quantize}.geojson", response=FeatureCollection)
 def area_children_compressed(request, area_id: int, simplify: int, quantize: int):
     """
     Returns the direct descendants of a given Area as a FeatureCollection
     applying compression methods
     """
     return models.Area.features.filter(parent=area_id).to_featurecollection(
         simplify=SIMPLIFICATION_LEVELS[simplify], quantize=quantize
     )
 
 
-@router.get("/area/by-parent/{area_id}.geojson", response=schemas.FeatureCollection)
+@router.get("/area/by-parent/{area_id}.geojson", response=FeatureCollection)
 def area_children(request, area_id: int):
     """
     Returns the direct descendants of a given Area as a FeatureCollection
     applying compression methods
     """
     return models.Area.features.filter(parent=area_id).to_featurecollection()
 
 
-@router.get("/area/by-type/{area_type}-s{simplify}-q{quantize}.geojson", response=schemas.FeatureCollection)
+@router.get("/area/by-type/{area_type}-s{simplify}-q{quantize}.geojson", response=FeatureCollection)
 def area_type_compressed(request, area_type: str, simplify: int, quantize: int):
     """
     Returns all areas of a given type
     appliying simplification and quantization
     """
     return models.Area.features.filter(kind__slug=area_type).to_featurecollection(
         simplify=SIMPLIFICATION_LEVELS[simplify], quantize=quantize
     )
 
 
-@router.get("/area/by-type/{area_type}.geojson", response=schemas.FeatureCollection)
+@router.get("/area/by-type/{area_type}.geojson", response=FeatureCollection)
 def area_type(request, area_type: str):
     """
     Returns all areas of a given type
     """
     return models.Area.features.filter(kind__slug=area_type).to_featurecollection()
```

### Comparing `simple_locations-4.0.1a0/simple_locations/static/css/tree-default-line.gif` & `simple_locations-4.1.0a0/simple_locations/static/css/tree-default-line.gif`

 * *Files identical despite different names*

### Comparing `simple_locations-4.0.1a0/simple_locations/static/css/tree.css` & `simple_locations-4.1.0a0/simple_locations/static/css/tree.css`

 * *Files identical despite different names*

### Comparing `simple_locations-4.0.1a0/simple_locations/static/images/ajax-loader.gif` & `simple_locations-4.1.0a0/simple_locations/static/images/ajax-loader.gif`

 * *Files identical despite different names*

### Comparing `simple_locations-4.0.1a0/simple_locations/static/images/delete.png` & `simple_locations-4.1.0a0/simple_locations/static/images/delete.png`

 * *Files identical despite different names*

### Comparing `simple_locations-4.0.1a0/simple_locations/static/images/edit.png` & `simple_locations-4.1.0a0/simple_locations/static/images/edit.png`

 * *Files identical despite different names*

### Comparing `simple_locations-4.0.1a0/simple_locations/static/images/minus.gif` & `simple_locations-4.1.0a0/simple_locations/static/images/minus.gif`

 * *Files identical despite different names*

### Comparing `simple_locations-4.0.1a0/simple_locations/static/images/plus.gif` & `simple_locations-4.1.0a0/simple_locations/static/images/plus.gif`

 * *Files identical despite different names*

### Comparing `simple_locations-4.0.1a0/simple_locations/static/images/tree-default-line.gif` & `simple_locations-4.1.0a0/simple_locations/static/images/tree-default-line.gif`

 * *Files identical despite different names*

### Comparing `simple_locations-4.0.1a0/simple_locations/static/javascripts/simple_locations.js` & `simple_locations-4.1.0a0/simple_locations/static/javascripts/simple_locations.js`

 * *Files identical despite different names*

### Comparing `simple_locations-4.0.1a0/simple_locations/static/uni_form/blue.uni-form.css` & `simple_locations-4.1.0a0/simple_locations/static/uni_form/blue.uni-form.css`

 * *Files identical despite different names*

### Comparing `simple_locations-4.0.1a0/simple_locations/static/uni_form/dark.uni-form.css` & `simple_locations-4.1.0a0/simple_locations/static/uni_form/dark.uni-form.css`

 * *Files identical despite different names*

### Comparing `simple_locations-4.0.1a0/simple_locations/static/uni_form/default.uni-form.css` & `simple_locations-4.1.0a0/simple_locations/static/uni_form/default.uni-form.css`

 * *Files identical despite different names*

### Comparing `simple_locations-4.0.1a0/simple_locations/static/uni_form/jquery.js` & `simple_locations-4.1.0a0/simple_locations/static/uni_form/jquery.js`

 * *Files identical despite different names*

### Comparing `simple_locations-4.0.1a0/simple_locations/static/uni_form/uni-form.css` & `simple_locations-4.1.0a0/simple_locations/static/uni_form/uni-form.css`

 * *Files identical despite different names*

### Comparing `simple_locations-4.0.1a0/simple_locations/static/uni_form/uni-form.jquery.js` & `simple_locations-4.1.0a0/simple_locations/static/uni_form/uni-form.jquery.js`

 * *Files identical despite different names*

### Comparing `simple_locations-4.0.1a0/simple_locations/templates/simple_locations/index.html` & `simple_locations-4.1.0a0/simple_locations/templates/simple_locations/index.html`

 * *Files identical despite different names*

### Comparing `simple_locations-4.0.1a0/simple_locations/templates/simple_locations/location_edit.html` & `simple_locations-4.1.0a0/simple_locations/templates/simple_locations/location_edit.html`

 * *Files identical despite different names*

### Comparing `simple_locations-4.0.1a0/simple_locations/templates/simple_locations/map.html` & `simple_locations-4.1.0a0/simple_locations/templates/simple_locations/map.html`

 * *Files identical despite different names*

### Comparing `simple_locations-4.0.1a0/simple_locations/templates/simple_locations/treepanel.html` & `simple_locations-4.1.0a0/simple_locations/templates/simple_locations/treepanel.html`

 * *Files identical despite different names*

### Comparing `simple_locations-4.0.1a0/simple_locations/urls.py` & `simple_locations-4.1.0a0/simple_locations/urls.py`

 * *Files identical despite different names*

### Comparing `simple_locations-4.0.1a0/simple_locations/views.py` & `simple_locations-4.1.0a0/simple_locations/views.py`

 * *Files identical despite different names*

### Comparing `simple_locations-4.0.1a0/setup.py` & `simple_locations-4.1.0a0/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,44 +1,128 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: simple-locations
+Version: 4.1.0a0
+Summary: The common location package for Catalpa's projects
+Home-page: https://github.com/catalpainternational/simple_locations
+License: BSD
+Author: Joshua Brooks
+Author-email: josh@catalpa.io
+Requires-Python: >=3.8,<4.0
+Classifier: License :: Other/Proprietary License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: django-geojson (>=4.0.0,<5.0.0)
+Requires-Dist: django-mptt (>=0.14.0,<0.15.0)
+Requires-Dist: django-ninja (>=0.21.0,<0.22.0)
+Requires-Dist: geojson-pydantic (>=0.6.2,<0.7.0)
+Requires-Dist: pydantic (>1.10.6,<2)
+Project-URL: Repository, https://github.com/catalpainternational/simple_locations
+Description-Content-Type: text/markdown
 
-packages = \
-['simple_locations',
- 'simple_locations.management',
- 'simple_locations.management.commands',
- 'simple_locations.migrations']
-
-package_data = \
-{'': ['*'],
- 'simple_locations': ['fixtures/*',
-                      'locale/fr/LC_MESSAGES/*',
-                      'static/css/*',
-                      'static/images/*',
-                      'static/javascripts/*',
-                      'static/uni_form/*',
-                      'templates/simple_locations/*',
-                      'templates/simple_locations/admin/*']}
-
-install_requires = \
-['django-geojson>=4.0.0,<5.0.0',
- 'django-mptt>=0.14.0,<0.15.0',
- 'django-ninja>=0.20.0',
- 'pydantic>=1.10.6,<2.0.0']
-
-setup_kwargs = {
-    'name': 'simple-locations',
-    'version': '4.0.1a0',
-    'description': "The common location package for Catalpa's projects",
-    'long_description': '# simple_locations\n\nThe common location package used for catalpa\'s projects. A hierarchical tree of geographical locations supporting location type and GIS data.\n\n## Admin\n\nThe admin site is set up to use Modeltranslations (if available in the parent app)\n\nFor modeltranslations, please remember to run `sync_translation_fields` in order to get `name_en`, `name_tet` etc. fields.\n\n## Environment\n\nThis is intended to be compatible with:\n\n- Django 3.1, 3.2, 4.0\n- Python 3.7, 3.8, 3.9\n\n```sh\ngh repo clone catalpainternational/simple_locations\ncd simple_locations\npython -m venv env\n. env/bin/activate\npip install pip-tools\npip-sync requirements.txt dev.txt\npre-commit install\n```\n\n### Pre Commit\n\nIf `pre-commit` is installed your code will be checked before commit.\nThis includes\n\n- black\n- flake8\n- isort\n- mypy\n\nThe same checks are run on push. See `pytest.yaml` for details on the checks being run.\n\n### New Release\n\nFor a new release, change the `version` property in pyproject.toml and push a git tag with the version number\nFor instance at time of writing the version is `3.1.4` with the tag `v3.1.4`\n\nSee `build.yaml` for details on release tagging\n## Changelog\n\n- Version 3.1.4\n  - Migrating JSON views from openly\n\n- Version 3.1.3\n  - Added `intersects_area` function\n\n- Version 3.1.2\n  - Uses psycopg2-binary for development environment\n\n- Version 3.1.1\n  - Added "border" fields\n  - Added a model for "projected" areas in EPSG:3857\n  - Added commands for border generation and\n  - `./manage.py` and associated project code\n\n- Version 3.0.1\n\n  - Poetry for dependency + packaging\n  - Releases are automated by pushing a `vx.x.x` tag to github\n\n- Version 3.0 (not on pypi)\n\n  - Code style changes (black, flake8)\n\n- Version 2.77\n\n  - first pass of updates for Python 3.8+ and Django 3.1+\n\n- Version 2.75\n\n  - add modeltranslations\n\n- Version 2.74\n\n  - fix CORS issue breaking maps in AreaAdmin\n  - typo in AreaChildrenInline\n\n- Version 2.73\n\n  - add an inline showing children to the Area admin\n  - make the `geom` field optional\n\n- Version 2.72\n  - optionally use django_extensions\' ForeignKeyAutocompleteAdmin in admin interface\n\n\n## Manually Uploading a new version to PyPi\n\nBump `pyproject.toml`\nThen run `poetry build` and `poetry publish`\n\n```bash\npoetry build\npoetry publish\n```\n\nSee the file `build.yml` for the workflow\n',
-    'author': 'Joshua Brooks',
-    'author_email': 'josh@catalpa.io',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/catalpainternational/simple_locations',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.8,<4.0',
-}
+# simple_locations
 
+The common location package used for catalpa's projects. A hierarchical tree of geographical locations supporting location type and GIS data.
+
+## Admin
+
+The admin site is set up to use Modeltranslations (if available in the parent app)
+
+For modeltranslations, please remember to run `sync_translation_fields` in order to get `name_en`, `name_tet` etc. fields.
+
+## Environment
+
+This is intended to be compatible with:
+
+- Django 3.1, 3.2, 4.0
+- Python 3.7, 3.8, 3.9
+
+```sh
+gh repo clone catalpainternational/simple_locations
+cd simple_locations
+python -m venv env
+. env/bin/activate
+pip install pip-tools
+pip-sync requirements.txt dev.txt
+pre-commit install
+```
+
+### Pre Commit
+
+If `pre-commit` is installed your code will be checked before commit.
+This includes
+
+- black
+- flake8
+- isort
+- mypy
+
+The same checks are run on push. See `pytest.yaml` for details on the checks being run.
+
+### New Release
+
+For a new release, change the `version` property in pyproject.toml and push a git tag with the version number
+For instance at time of writing the version is `3.1.4` with the tag `v3.1.4`
+
+See `build.yaml` for details on release tagging
+## Changelog
+
+- Version 3.1.4
+  - Migrating JSON views from openly
+
+- Version 3.1.3
+  - Added `intersects_area` function
+
+- Version 3.1.2
+  - Uses psycopg2-binary for development environment
+
+- Version 3.1.1
+  - Added "border" fields
+  - Added a model for "projected" areas in EPSG:3857
+  - Added commands for border generation and
+  - `./manage.py` and associated project code
+
+- Version 3.0.1
+
+  - Poetry for dependency + packaging
+  - Releases are automated by pushing a `vx.x.x` tag to github
+
+- Version 3.0 (not on pypi)
+
+  - Code style changes (black, flake8)
+
+- Version 2.77
+
+  - first pass of updates for Python 3.8+ and Django 3.1+
+
+- Version 2.75
+
+  - add modeltranslations
+
+- Version 2.74
+
+  - fix CORS issue breaking maps in AreaAdmin
+  - typo in AreaChildrenInline
+
+- Version 2.73
+
+  - add an inline showing children to the Area admin
+  - make the `geom` field optional
+
+- Version 2.72
+  - optionally use django_extensions' ForeignKeyAutocompleteAdmin in admin interface
+
+
+## Manually Uploading a new version to PyPi
+
+Bump `pyproject.toml`
+Then run `poetry build` and `poetry publish`
+
+```bash
+poetry build
+poetry publish
+```
+
+See the file `build.yml` for the workflow
 
-setup(**setup_kwargs)
```

