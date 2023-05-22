# Comparing `tmp/contenttypes.basic-1.8.tar.gz` & `tmp/contenttypes.basic-2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "contenttypes.basic-1.8.tar", last modified: Mon May 22 11:43:51 2023, max compression
+gzip compressed data, was "contenttypes.basic-2.0.tar", last modified: Mon Mar 27 13:05:16 2023, max compression
```

## Comparing `contenttypes.basic-1.8.tar` & `contenttypes.basic-2.0.tar`

### file list

```diff
@@ -1,147 +1,147 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 11:43:51.455737 contenttypes.basic-1.8/
--rwxr-xr-x   0 root         (0) root         (0)     2422 2023-05-22 11:42:49.000000 contenttypes.basic-1.8/CHANGES.rst
--rwxr-xr-x   0 root         (0) root         (0)       62 2020-11-11 11:41:31.000000 contenttypes.basic-1.8/CONTRIBUTORS.rst
--rwxr-xr-x   0 root         (0) root         (0)      586 2020-11-11 11:41:31.000000 contenttypes.basic-1.8/DEVELOP.rst
--rwxr-xr-x   0 root         (0) root         (0)    18092 2020-11-11 11:41:31.000000 contenttypes.basic-1.8/LICENSE.GPL
--rwxr-xr-x   0 root         (0) root         (0)      658 2020-11-11 11:41:31.000000 contenttypes.basic-1.8/LICENSE.rst
--rwxr-xr-x   0 root         (0) root         (0)       69 2020-11-11 11:41:31.000000 contenttypes.basic-1.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     4374 2023-05-22 11:43:51.455737 contenttypes.basic-1.8/PKG-INFO
--rwxr-xr-x   0 root         (0) root         (0)     1086 2020-11-11 11:41:31.000000 contenttypes.basic-1.8/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 11:43:51.169737 contenttypes.basic-1.8/docs/
--rwxr-xr-x   0 root         (0) root         (0)     7915 2020-11-11 11:41:31.000000 contenttypes.basic-1.8/docs/conf.py
--rwxr-xr-x   0 root         (0) root         (0)       77 2020-11-11 11:41:31.000000 contenttypes.basic-1.8/docs/index.rst
--rwxr-xr-x   0 root         (0) root         (0)      321 2023-05-22 11:43:51.456737 contenttypes.basic-1.8/setup.cfg
--rwxr-xr-x   0 root         (0) root         (0)     2297 2023-05-22 11:42:52.000000 contenttypes.basic-1.8/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 11:43:51.117737 contenttypes.basic-1.8/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 11:43:51.169737 contenttypes.basic-1.8/src/contenttypes/
--rwxr-xr-x   0 root         (0) root         (0)       80 2020-11-11 11:41:31.000000 contenttypes.basic-1.8/src/contenttypes/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 11:43:51.173737 contenttypes.basic-1.8/src/contenttypes/basic/
--rwxr-xr-x   0 root         (0) root         (0)      135 2021-02-01 10:25:11.000000 contenttypes.basic-1.8/src/contenttypes/basic/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 11:43:51.174737 contenttypes.basic-1.8/src/contenttypes/basic/behaviors/
--rwxr-xr-x   0 root         (0) root         (0)        0 2020-11-11 11:41:31.000000 contenttypes.basic-1.8/src/contenttypes/basic/behaviors/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)     1248 2020-11-11 11:41:31.000000 contenttypes.basic-1.8/src/contenttypes/basic/behaviors/button_text.py
--rwxr-xr-x   0 root         (0) root         (0)      923 2020-11-11 11:41:31.000000 contenttypes.basic-1.8/src/contenttypes/basic/behaviors/colour.py
--rwxr-xr-x   0 root         (0) root         (0)     3050 2023-03-17 09:59:22.000000 contenttypes.basic-1.8/src/contenttypes/basic/behaviors/configure.zcml
--rwxr-xr-x   0 root         (0) root         (0)      860 2020-11-11 11:41:31.000000 contenttypes.basic-1.8/src/contenttypes/basic/behaviors/hide_text.py
--rwxr-xr-x   0 root         (0) root         (0)      908 2020-11-11 11:41:31.000000 contenttypes.basic-1.8/src/contenttypes/basic/behaviors/icon.py
--rwxr-xr-x   0 root         (0) root         (0)      985 2020-11-11 11:41:31.000000 contenttypes.basic-1.8/src/contenttypes/basic/behaviors/link.py
--rwxr-xr-x   0 root         (0) root         (0)     1003 2020-11-11 11:41:31.000000 contenttypes.basic-1.8/src/contenttypes/basic/behaviors/osmap.py
--rwxr-xr-x   0 root         (0) root         (0)     1115 2023-03-17 10:10:18.000000 contenttypes.basic-1.8/src/contenttypes/basic/behaviors/osmap_advanced.py
--rwxr-xr-x   0 root         (0) root         (0)     1744 2020-11-11 11:41:31.000000 contenttypes.basic-1.8/src/contenttypes/basic/behaviors/text_position.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 11:43:51.241737 contenttypes.basic-1.8/src/contenttypes/basic/browser/
--rwxr-xr-x   0 root         (0) root         (0)        0 2021-02-01 10:26:47.000000 contenttypes.basic-1.8/src/contenttypes/basic/browser/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)     2095 2020-11-11 11:41:31.000000 contenttypes.basic-1.8/src/contenttypes/basic/browser/configure.zcml
--rwxr-xr-x   0 root         (0) root         (0)      466 2020-11-11 11:41:31.000000 contenttypes.basic-1.8/src/contenttypes/basic/browser/default_view.pt
--rwxr-xr-x   0 root         (0) root         (0)      154 2020-11-11 11:41:31.000000 contenttypes.basic-1.8/src/contenttypes/basic/browser/default_view.py
--rwxr-xr-x   0 root         (0) root         (0)     1220 2020-11-11 11:41:31.000000 contenttypes.basic-1.8/src/contenttypes/basic/browser/link.pt
--rwxr-xr-x   0 root         (0) root         (0)     1220 2020-11-11 11:41:31.000000 contenttypes.basic-1.8/src/contenttypes/basic/browser/link_redirect.pt
--rwxr-xr-x   0 root         (0) root         (0)      415 2020-11-11 11:41:31.000000 contenttypes.basic-1.8/src/contenttypes/basic/browser/link_redirect.py
--rwxr-xr-x   0 root         (0) root         (0)      406 2020-11-11 11:41:31.000000 contenttypes.basic-1.8/src/contenttypes/basic/browser/link_redirect_view.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 11:43:51.241737 contenttypes.basic-1.8/src/contenttypes/basic/browser/overrides/
--rwxr-xr-x   0 root         (0) root         (0)        0 2020-11-11 11:41:31.000000 contenttypes.basic-1.8/src/contenttypes/basic/browser/overrides/.gitkeep
--rwxr-xr-x   0 root         (0) root         (0)    80607 2022-09-28 12:19:22.000000 contenttypes.basic-1.8/src/contenttypes/basic/browser/sprite.pt
--rwxr-xr-x   0 root         (0) root         (0)      298 2020-11-11 11:41:31.000000 contenttypes.basic-1.8/src/contenttypes/basic/browser/sprite.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 11:43:51.241737 contenttypes.basic-1.8/src/contenttypes/basic/browser/static/
--rwxr-xr-x   0 root         (0) root         (0)        0 2020-11-11 11:41:31.000000 contenttypes.basic-1.8/src/contenttypes/basic/browser/static/.gitkeep
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 11:43:51.356737 contenttypes.basic-1.8/src/contenttypes/basic/browser/static/osmap/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 11:43:51.367737 contenttypes.basic-1.8/src/contenttypes/basic/browser/static/osmap/images/
--rwxr-xr-x   0 root         (0) root         (0)     1259 2020-11-11 11:41:31.000000 contenttypes.basic-1.8/src/contenttypes/basic/browser/static/osmap/images/layers-2x.png
--rwxr-xr-x   0 root         (0) root         (0)      696 2020-11-11 11:41:31.000000 contenttypes.basic-1.8/src/contenttypes/basic/browser/static/osmap/images/layers.png
--rwxr-xr-x   0 root         (0) root         (0)     2464 2020-11-11 11:41:31.000000 contenttypes.basic-1.8/src/contenttypes/basic/browser/static/osmap/images/marker-icon-2x.png
--rwxr-xr-x   0 root         (0) root         (0)     1466 2020-11-11 11:41:31.000000 contenttypes.basic-1.8/src/contenttypes/basic/browser/static/osmap/images/marker-icon.png
--rwxr-xr-x   0 root         (0) root         (0)      618 2020-11-11 11:41:31.000000 contenttypes.basic-1.8/src/contenttypes/basic/browser/static/osmap/images/marker-shadow.png
--rwxr-xr-x   0 root         (0) root         (0)   398589 2020-11-11 11:41:31.000000 contenttypes.basic-1.8/src/contenttypes/basic/browser/static/osmap/leaflet-src.esm.js
--rwxr-xr-x   0 root         (0) root         (0)   759894 2020-11-11 11:41:31.000000 contenttypes.basic-1.8/src/contenttypes/basic/browser/static/osmap/leaflet-src.esm.js.map
--rwxr-xr-x   0 root         (0) root         (0)   400314 2020-11-11 11:41:31.000000 contenttypes.basic-1.8/src/contenttypes/basic/browser/static/osmap/leaflet-src.js
--rwxr-xr-x   0 root         (0) root         (0)   759986 2020-11-11 11:41:31.000000 contenttypes.basic-1.8/src/contenttypes/basic/browser/static/osmap/leaflet-src.js.map
--rwxr-xr-x   0 root         (0) root         (0)    15395 2020-11-11 11:41:31.000000 contenttypes.basic-1.8/src/contenttypes/basic/browser/static/osmap/leaflet.css
--rwxr-xr-x   0 root         (0) root         (0)   140696 2020-11-11 11:41:31.000000 contenttypes.basic-1.8/src/contenttypes/basic/browser/static/osmap/leaflet.js
--rwxr-xr-x   0 root         (0) root         (0)   191113 2020-11-11 11:41:31.000000 contenttypes.basic-1.8/src/contenttypes/basic/browser/static/osmap/leaflet.js.map
--rwxr-xr-x   0 root         (0) root         (0)     1647 2020-11-11 11:41:31.000000 contenttypes.basic-1.8/src/contenttypes/basic/configure.zcml
--rwxr-xr-x   0 root         (0) root         (0)      773 2020-11-11 11:41:31.000000 contenttypes.basic-1.8/src/contenttypes/basic/contents.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 11:43:51.388737 contenttypes.basic-1.8/src/contenttypes/basic/controlpanel/
--rwxr-xr-x   0 root         (0) root         (0)        0 2020-11-11 11:41:31.000000 contenttypes.basic-1.8/src/contenttypes/basic/controlpanel/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)      424 2020-11-11 11:41:31.000000 contenttypes.basic-1.8/src/contenttypes/basic/controlpanel/configure.zcml
--rwxr-xr-x   0 root         (0) root         (0)      891 2020-11-11 11:41:31.000000 contenttypes.basic-1.8/src/contenttypes/basic/controlpanel/coordinates.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 11:43:51.388737 contenttypes.basic-1.8/src/contenttypes/basic/fields/
--rwxr-xr-x   0 root         (0) root         (0)        0 2020-11-11 11:41:31.000000 contenttypes.basic-1.8/src/contenttypes/basic/fields/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)      238 2020-11-11 11:41:31.000000 contenttypes.basic-1.8/src/contenttypes/basic/fields/colour.py
--rwxr-xr-x   0 root         (0) root         (0)      230 2020-11-11 11:41:31.000000 contenttypes.basic-1.8/src/contenttypes/basic/fields/icon.py
--rwxr-xr-x   0 root         (0) root         (0)      234 2020-11-11 11:41:31.000000 contenttypes.basic-1.8/src/contenttypes/basic/fields/osmap.py
--rwxr-xr-x   0 root         (0) root         (0)      267 2023-03-17 09:54:26.000000 contenttypes.basic-1.8/src/contenttypes/basic/fields/osmap_advanced.py
--rwxr-xr-x   0 root         (0) root         (0)     2204 2023-03-17 10:10:59.000000 contenttypes.basic-1.8/src/contenttypes/basic/interfaces.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 11:43:51.393737 contenttypes.basic-1.8/src/contenttypes/basic/locales/
--rwxr-xr-x   0 root         (0) root         (0)        0 2020-11-11 11:41:31.000000 contenttypes.basic-1.8/src/contenttypes/basic/locales/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 11:43:51.162737 contenttypes.basic-1.8/src/contenttypes/basic/locales/ca/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 11:43:51.394737 contenttypes.basic-1.8/src/contenttypes/basic/locales/ca/LC_MESSAGES/
--rw-r--r--   0 root         (0) root         (0)     4225 2023-03-17 10:52:40.000000 contenttypes.basic-1.8/src/contenttypes/basic/locales/ca/LC_MESSAGES/contenttypes.basic.mo
--rwxr-xr-x   0 root         (0) root         (0)     7013 2023-03-17 10:52:23.000000 contenttypes.basic-1.8/src/contenttypes/basic/locales/ca/LC_MESSAGES/contenttypes.basic.po
--rwxr-xr-x   0 root         (0) root         (0)       98 2020-11-11 11:41:31.000000 contenttypes.basic-1.8/src/contenttypes/basic/locales/compile.sh
--rwxr-xr-x   0 root         (0) root         (0)     5656 2023-03-17 10:50:52.000000 contenttypes.basic-1.8/src/contenttypes/basic/locales/contenttypes.basic.pot
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 11:43:51.162737 contenttypes.basic-1.8/src/contenttypes/basic/locales/en/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 11:43:51.395737 contenttypes.basic-1.8/src/contenttypes/basic/locales/en/LC_MESSAGES/
--rw-r--r--   0 root         (0) root         (0)     4054 2023-03-17 10:52:40.000000 contenttypes.basic-1.8/src/contenttypes/basic/locales/en/LC_MESSAGES/contenttypes.basic.mo
--rwxr-xr-x   0 root         (0) root         (0)     6842 2023-03-17 10:52:03.000000 contenttypes.basic-1.8/src/contenttypes/basic/locales/en/LC_MESSAGES/contenttypes.basic.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 11:43:51.162737 contenttypes.basic-1.8/src/contenttypes/basic/locales/es/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 11:43:51.397737 contenttypes.basic-1.8/src/contenttypes/basic/locales/es/LC_MESSAGES/
--rw-r--r--   0 root         (0) root         (0)     4277 2023-03-17 10:52:40.000000 contenttypes.basic-1.8/src/contenttypes/basic/locales/es/LC_MESSAGES/contenttypes.basic.mo
--rwxr-xr-x   0 root         (0) root         (0)     7065 2023-03-17 10:52:17.000000 contenttypes.basic-1.8/src/contenttypes/basic/locales/es/LC_MESSAGES/contenttypes.basic.po
--rwxr-xr-x   0 root         (0) root         (0)        0 2020-11-11 11:41:31.000000 contenttypes.basic-1.8/src/contenttypes/basic/locales/manual.pot
--rwxr-xr-x   0 root         (0) root         (0)      884 2020-11-11 11:41:31.000000 contenttypes.basic-1.8/src/contenttypes/basic/locales/update.sh
--rwxr-xr-x   0 root         (0) root         (0)      298 2020-11-11 11:41:31.000000 contenttypes.basic-1.8/src/contenttypes/basic/permissions.py
--rwxr-xr-x   0 root         (0) root         (0)      833 2020-11-11 11:41:31.000000 contenttypes.basic-1.8/src/contenttypes/basic/permissions.zcml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 11:43:51.163737 contenttypes.basic-1.8/src/contenttypes/basic/profiles/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 11:43:51.398737 contenttypes.basic-1.8/src/contenttypes/basic/profiles/coordinates-controlpanel/
--rwxr-xr-x   0 root         (0) root         (0)      560 2020-11-11 11:41:31.000000 contenttypes.basic-1.8/src/contenttypes/basic/profiles/coordinates-controlpanel/controlpanel.xml
--rwxr-xr-x   0 root         (0) root         (0)      168 2020-11-11 11:41:31.000000 contenttypes.basic-1.8/src/contenttypes/basic/profiles/coordinates-controlpanel/registry.xml
--rwxr-xr-x   0 root         (0) root         (0)      255 2020-11-11 11:41:31.000000 contenttypes.basic-1.8/src/contenttypes/basic/profiles/coordinates-controlpanel/rolemap.xml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 11:43:51.400737 contenttypes.basic-1.8/src/contenttypes/basic/profiles/default/
--rwxr-xr-x   0 root         (0) root         (0)      180 2020-11-11 11:41:31.000000 contenttypes.basic-1.8/src/contenttypes/basic/profiles/default/browserlayer.xml
--rwxr-xr-x   0 root         (0) root         (0)       90 2020-11-11 11:41:31.000000 contenttypes.basic-1.8/src/contenttypes/basic/profiles/default/metadata.xml
--rwxr-xr-x   0 root         (0) root         (0)      954 2020-11-11 11:41:31.000000 contenttypes.basic-1.8/src/contenttypes/basic/profiles/default/rolemap.xml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 11:43:51.404737 contenttypes.basic-1.8/src/contenttypes/basic/profiles/default/types/
--rwxr-xr-x   0 root         (0) root         (0)     2581 2020-11-11 11:41:31.000000 contenttypes.basic-1.8/src/contenttypes/basic/profiles/default/types/Announcement.xml
--rwxr-xr-x   0 root         (0) root         (0)     2682 2020-11-11 11:41:31.000000 contenttypes.basic-1.8/src/contenttypes/basic/profiles/default/types/Banner.xml
--rwxr-xr-x   0 root         (0) root         (0)     2616 2020-11-11 11:41:31.000000 contenttypes.basic-1.8/src/contenttypes/basic/profiles/default/types/Icon.xml
--rwxr-xr-x   0 root         (0) root         (0)     2674 2020-11-11 11:41:31.000000 contenttypes.basic-1.8/src/contenttypes/basic/profiles/default/types/Slide.xml
--rwxr-xr-x   0 root         (0) root         (0)      326 2020-11-11 11:41:31.000000 contenttypes.basic-1.8/src/contenttypes/basic/profiles/default/types.xml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 11:43:51.404737 contenttypes.basic-1.8/src/contenttypes/basic/profiles/uninstall/
--rwxr-xr-x   0 root         (0) root         (0)      128 2020-11-11 11:41:31.000000 contenttypes.basic-1.8/src/contenttypes/basic/profiles/uninstall/browserlayer.xml
--rwxr-xr-x   0 root         (0) root         (0)      574 2020-11-11 11:41:31.000000 contenttypes.basic-1.8/src/contenttypes/basic/setuphandlers.py
--rwxr-xr-x   0 root         (0) root         (0)     2086 2022-11-10 14:36:00.000000 contenttypes.basic-1.8/src/contenttypes/basic/testing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 11:43:51.414737 contenttypes.basic-1.8/src/contenttypes/basic/tests/
--rwxr-xr-x   0 root         (0) root         (0)     1215 2020-11-11 11:41:31.000000 contenttypes.basic-1.8/src/contenttypes/basic/tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 11:43:51.415737 contenttypes.basic-1.8/src/contenttypes/basic/tests/robot/
--rwxr-xr-x   0 root         (0) root         (0)     2003 2020-11-11 11:41:31.000000 contenttypes.basic-1.8/src/contenttypes/basic/tests/robot/test_example.robot
--rwxr-xr-x   0 root         (0) root         (0)     5888 2020-11-11 11:41:31.000000 contenttypes.basic-1.8/src/contenttypes/basic/tests/test_behaviors.py
--rwxr-xr-x   0 root         (0) root         (0)      913 2020-11-11 11:41:31.000000 contenttypes.basic-1.8/src/contenttypes/basic/tests/test_controlpanel.py
--rwxr-xr-x   0 root         (0) root         (0)     2376 2020-11-11 11:41:31.000000 contenttypes.basic-1.8/src/contenttypes/basic/tests/test_converters.py
--rwxr-xr-x   0 root         (0) root         (0)      890 2020-11-11 11:41:31.000000 contenttypes.basic-1.8/src/contenttypes/basic/tests/test_robot.py
--rwxr-xr-x   0 root         (0) root         (0)     2421 2021-09-02 14:20:34.000000 contenttypes.basic-1.8/src/contenttypes/basic/tests/test_setup.py
--rwxr-xr-x   0 root         (0) root         (0)     1470 2020-11-11 11:41:31.000000 contenttypes.basic-1.8/src/contenttypes/basic/tests/test_views.py
--rwxr-xr-x   0 root         (0) root         (0)      210 2020-11-11 11:41:31.000000 contenttypes.basic-1.8/src/contenttypes/basic/upgrades.py
--rwxr-xr-x   0 root         (0) root         (0)      387 2020-11-11 11:41:31.000000 contenttypes.basic-1.8/src/contenttypes/basic/upgrades.zcml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 11:43:51.453737 contenttypes.basic-1.8/src/contenttypes/basic/widgets/
--rwxr-xr-x   0 root         (0) root         (0)        0 2020-11-11 11:41:31.000000 contenttypes.basic-1.8/src/contenttypes/basic/widgets/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)      692 2020-11-11 11:41:31.000000 contenttypes.basic-1.8/src/contenttypes/basic/widgets/colour.py
--rwxr-xr-x   0 root         (0) root         (0)      583 2022-05-06 08:25:24.000000 contenttypes.basic-1.8/src/contenttypes/basic/widgets/colour_display.pt
--rwxr-xr-x   0 root         (0) root         (0)      617 2022-05-06 08:25:24.000000 contenttypes.basic-1.8/src/contenttypes/basic/widgets/colour_input.pt
--rwxr-xr-x   0 root         (0) root         (0)     1882 2023-03-17 10:13:35.000000 contenttypes.basic-1.8/src/contenttypes/basic/widgets/configure.zcml
--rwxr-xr-x   0 root         (0) root         (0)     1282 2022-04-07 11:39:32.000000 contenttypes.basic-1.8/src/contenttypes/basic/widgets/icon.py
--rwxr-xr-x   0 root         (0) root         (0)      704 2023-03-07 12:54:51.000000 contenttypes.basic-1.8/src/contenttypes/basic/widgets/icon_display.pt
--rwxr-xr-x   0 root         (0) root         (0)     2649 2023-03-07 12:55:31.000000 contenttypes.basic-1.8/src/contenttypes/basic/widgets/icon_input.pt
--rwxr-xr-x   0 root         (0) root         (0)     2171 2023-05-22 11:42:24.000000 contenttypes.basic-1.8/src/contenttypes/basic/widgets/osmap.py
--rwxr-xr-x   0 root         (0) root         (0)     2170 2023-03-17 10:14:50.000000 contenttypes.basic-1.8/src/contenttypes/basic/widgets/osmap_advanced.py
--rwxr-xr-x   0 root         (0) root         (0)     3487 2023-03-17 10:11:54.000000 contenttypes.basic-1.8/src/contenttypes/basic/widgets/osmap_advanced_display.pt
--rwxr-xr-x   0 root         (0) root         (0)    15323 2023-03-17 10:51:49.000000 contenttypes.basic-1.8/src/contenttypes/basic/widgets/osmap_advanced_input.pt
--rwxr-xr-x   0 root         (0) root         (0)     2599 2023-05-22 11:42:23.000000 contenttypes.basic-1.8/src/contenttypes/basic/widgets/osmap_display.pt
--rwxr-xr-x   0 root         (0) root         (0)     6429 2023-05-22 11:42:23.000000 contenttypes.basic-1.8/src/contenttypes/basic/widgets/osmap_input.pt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 11:43:51.171737 contenttypes.basic-1.8/src/contenttypes.basic.egg-info/
--rwxr-xr-x   0 root         (0) root         (0)     4374 2023-05-22 11:43:50.000000 contenttypes.basic-1.8/src/contenttypes.basic.egg-info/PKG-INFO
--rwxr-xr-x   0 root         (0) root         (0)     5393 2023-05-22 11:43:50.000000 contenttypes.basic-1.8/src/contenttypes.basic.egg-info/SOURCES.txt
--rwxr-xr-x   0 root         (0) root         (0)        1 2023-05-22 11:43:50.000000 contenttypes.basic-1.8/src/contenttypes.basic.egg-info/dependency_links.txt
--rwxr-xr-x   0 root         (0) root         (0)      123 2023-05-22 11:43:50.000000 contenttypes.basic-1.8/src/contenttypes.basic.egg-info/entry_points.txt
--rwxr-xr-x   0 root         (0) root         (0)       13 2023-05-22 11:43:50.000000 contenttypes.basic-1.8/src/contenttypes.basic.egg-info/namespace_packages.txt
--rwxr-xr-x   0 root         (0) root         (0)        1 2020-11-11 11:45:30.000000 contenttypes.basic-1.8/src/contenttypes.basic.egg-info/not-zip-safe
--rwxr-xr-x   0 root         (0) root         (0)      173 2023-05-22 11:43:50.000000 contenttypes.basic-1.8/src/contenttypes.basic.egg-info/requires.txt
--rwxr-xr-x   0 root         (0) root         (0)       13 2023-05-22 11:43:50.000000 contenttypes.basic-1.8/src/contenttypes.basic.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 13:05:16.569513 contenttypes.basic-2.0/
+-rwxr-xr-x   0 root         (0) root         (0)     2494 2023-03-27 13:01:28.000000 contenttypes.basic-2.0/CHANGES.rst
+-rwxrwxrwx   0 root         (0) root         (0)       62 2023-03-17 08:35:42.000000 contenttypes.basic-2.0/CONTRIBUTORS.rst
+-rwxrwxrwx   0 root         (0) root         (0)      586 2023-03-17 08:35:42.000000 contenttypes.basic-2.0/DEVELOP.rst
+-rwxrwxrwx   0 root         (0) root         (0)    18092 2023-03-17 08:35:42.000000 contenttypes.basic-2.0/LICENSE.GPL
+-rwxrwxrwx   0 root         (0) root         (0)      658 2023-03-17 08:35:42.000000 contenttypes.basic-2.0/LICENSE.rst
+-rwxrwxrwx   0 root         (0) root         (0)       69 2023-03-17 08:35:42.000000 contenttypes.basic-2.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     4548 2023-03-27 13:05:16.569513 contenttypes.basic-2.0/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)     1086 2023-03-17 08:35:42.000000 contenttypes.basic-2.0/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 13:05:16.530513 contenttypes.basic-2.0/docs/
+-rwxrwxrwx   0 root         (0) root         (0)     7915 2023-03-17 08:35:42.000000 contenttypes.basic-2.0/docs/conf.py
+-rwxrwxrwx   0 root         (0) root         (0)       77 2023-03-17 08:35:42.000000 contenttypes.basic-2.0/docs/index.rst
+-rwxrwxrwx   0 root         (0) root         (0)      321 2023-03-27 13:05:16.570513 contenttypes.basic-2.0/setup.cfg
+-rwxr-xr-x   0 root         (0) root         (0)     2444 2023-03-27 13:00:58.000000 contenttypes.basic-2.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 13:05:16.524513 contenttypes.basic-2.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 13:05:16.530513 contenttypes.basic-2.0/src/contenttypes/
+-rwxrwxrwx   0 root         (0) root         (0)       80 2023-03-17 08:35:42.000000 contenttypes.basic-2.0/src/contenttypes/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 13:05:16.546513 contenttypes.basic-2.0/src/contenttypes/basic/
+-rwxrwxrwx   0 root         (0) root         (0)      135 2023-03-17 08:35:42.000000 contenttypes.basic-2.0/src/contenttypes/basic/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 13:05:16.548513 contenttypes.basic-2.0/src/contenttypes/basic/behaviors/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2023-03-17 08:35:42.000000 contenttypes.basic-2.0/src/contenttypes/basic/behaviors/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     1248 2023-03-17 08:35:42.000000 contenttypes.basic-2.0/src/contenttypes/basic/behaviors/button_text.py
+-rwxrwxrwx   0 root         (0) root         (0)      923 2023-03-17 08:35:42.000000 contenttypes.basic-2.0/src/contenttypes/basic/behaviors/colour.py
+-rwxr-xr-x   0 root         (0) root         (0)     3050 2023-03-17 11:08:05.000000 contenttypes.basic-2.0/src/contenttypes/basic/behaviors/configure.zcml
+-rwxrwxrwx   0 root         (0) root         (0)      860 2023-03-17 08:35:42.000000 contenttypes.basic-2.0/src/contenttypes/basic/behaviors/hide_text.py
+-rwxr-xr-x   0 root         (0) root         (0)      908 2023-03-17 11:07:58.000000 contenttypes.basic-2.0/src/contenttypes/basic/behaviors/icon.py
+-rwxrwxrwx   0 root         (0) root         (0)      985 2023-03-17 08:35:42.000000 contenttypes.basic-2.0/src/contenttypes/basic/behaviors/link.py
+-rwxrwxrwx   0 root         (0) root         (0)     1003 2023-03-17 08:35:42.000000 contenttypes.basic-2.0/src/contenttypes/basic/behaviors/osmap.py
+-rwxr-xr-x   0 root         (0) root         (0)     1115 2023-03-17 11:08:05.000000 contenttypes.basic-2.0/src/contenttypes/basic/behaviors/osmap_advanced.py
+-rwxrwxrwx   0 root         (0) root         (0)     1744 2023-03-17 08:35:42.000000 contenttypes.basic-2.0/src/contenttypes/basic/behaviors/text_position.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 13:05:16.551513 contenttypes.basic-2.0/src/contenttypes/basic/browser/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2023-03-17 08:35:42.000000 contenttypes.basic-2.0/src/contenttypes/basic/browser/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     2095 2023-03-17 08:35:42.000000 contenttypes.basic-2.0/src/contenttypes/basic/browser/configure.zcml
+-rwxrwxrwx   0 root         (0) root         (0)      466 2023-03-17 08:35:42.000000 contenttypes.basic-2.0/src/contenttypes/basic/browser/default_view.pt
+-rwxrwxrwx   0 root         (0) root         (0)      154 2023-03-17 08:35:42.000000 contenttypes.basic-2.0/src/contenttypes/basic/browser/default_view.py
+-rwxrwxrwx   0 root         (0) root         (0)     1220 2023-03-17 08:35:42.000000 contenttypes.basic-2.0/src/contenttypes/basic/browser/link.pt
+-rwxrwxrwx   0 root         (0) root         (0)     1220 2023-03-17 08:35:42.000000 contenttypes.basic-2.0/src/contenttypes/basic/browser/link_redirect.pt
+-rwxrwxrwx   0 root         (0) root         (0)      415 2023-03-17 08:35:42.000000 contenttypes.basic-2.0/src/contenttypes/basic/browser/link_redirect.py
+-rwxrwxrwx   0 root         (0) root         (0)      406 2023-03-17 08:35:42.000000 contenttypes.basic-2.0/src/contenttypes/basic/browser/link_redirect_view.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 13:05:16.551513 contenttypes.basic-2.0/src/contenttypes/basic/browser/overrides/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2023-03-17 08:35:42.000000 contenttypes.basic-2.0/src/contenttypes/basic/browser/overrides/.gitkeep
+-rwxrwxrwx   0 root         (0) root         (0)    80607 2023-03-17 08:35:42.000000 contenttypes.basic-2.0/src/contenttypes/basic/browser/sprite.pt
+-rwxrwxrwx   0 root         (0) root         (0)      298 2023-03-17 08:35:42.000000 contenttypes.basic-2.0/src/contenttypes/basic/browser/sprite.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 13:05:16.551513 contenttypes.basic-2.0/src/contenttypes/basic/browser/static/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2023-03-17 08:35:42.000000 contenttypes.basic-2.0/src/contenttypes/basic/browser/static/.gitkeep
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 13:05:16.555513 contenttypes.basic-2.0/src/contenttypes/basic/browser/static/osmap/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 13:05:16.557513 contenttypes.basic-2.0/src/contenttypes/basic/browser/static/osmap/images/
+-rwxrwxrwx   0 root         (0) root         (0)     1259 2023-03-17 08:35:42.000000 contenttypes.basic-2.0/src/contenttypes/basic/browser/static/osmap/images/layers-2x.png
+-rwxrwxrwx   0 root         (0) root         (0)      696 2023-03-17 08:35:42.000000 contenttypes.basic-2.0/src/contenttypes/basic/browser/static/osmap/images/layers.png
+-rwxrwxrwx   0 root         (0) root         (0)     2464 2023-03-17 08:35:42.000000 contenttypes.basic-2.0/src/contenttypes/basic/browser/static/osmap/images/marker-icon-2x.png
+-rwxrwxrwx   0 root         (0) root         (0)     1466 2023-03-17 08:35:42.000000 contenttypes.basic-2.0/src/contenttypes/basic/browser/static/osmap/images/marker-icon.png
+-rwxrwxrwx   0 root         (0) root         (0)      618 2023-03-17 08:35:42.000000 contenttypes.basic-2.0/src/contenttypes/basic/browser/static/osmap/images/marker-shadow.png
+-rwxrwxrwx   0 root         (0) root         (0)   398589 2023-03-17 08:35:42.000000 contenttypes.basic-2.0/src/contenttypes/basic/browser/static/osmap/leaflet-src.esm.js
+-rwxrwxrwx   0 root         (0) root         (0)   759894 2023-03-17 08:35:42.000000 contenttypes.basic-2.0/src/contenttypes/basic/browser/static/osmap/leaflet-src.esm.js.map
+-rwxrwxrwx   0 root         (0) root         (0)   400314 2023-03-17 08:35:42.000000 contenttypes.basic-2.0/src/contenttypes/basic/browser/static/osmap/leaflet-src.js
+-rwxrwxrwx   0 root         (0) root         (0)   759986 2023-03-17 08:35:42.000000 contenttypes.basic-2.0/src/contenttypes/basic/browser/static/osmap/leaflet-src.js.map
+-rwxrwxrwx   0 root         (0) root         (0)    15395 2023-03-17 08:35:42.000000 contenttypes.basic-2.0/src/contenttypes/basic/browser/static/osmap/leaflet.css
+-rwxrwxrwx   0 root         (0) root         (0)   140696 2023-03-17 08:35:42.000000 contenttypes.basic-2.0/src/contenttypes/basic/browser/static/osmap/leaflet.js
+-rwxrwxrwx   0 root         (0) root         (0)   191113 2023-03-17 08:35:42.000000 contenttypes.basic-2.0/src/contenttypes/basic/browser/static/osmap/leaflet.js.map
+-rwxr-xr-x   0 root         (0) root         (0)     1647 2023-03-17 11:07:58.000000 contenttypes.basic-2.0/src/contenttypes/basic/configure.zcml
+-rwxrwxrwx   0 root         (0) root         (0)      773 2023-03-17 08:35:42.000000 contenttypes.basic-2.0/src/contenttypes/basic/contents.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 13:05:16.557513 contenttypes.basic-2.0/src/contenttypes/basic/controlpanel/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2023-03-17 08:35:42.000000 contenttypes.basic-2.0/src/contenttypes/basic/controlpanel/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)      424 2023-03-17 08:35:42.000000 contenttypes.basic-2.0/src/contenttypes/basic/controlpanel/configure.zcml
+-rwxrwxrwx   0 root         (0) root         (0)      891 2023-03-17 08:35:42.000000 contenttypes.basic-2.0/src/contenttypes/basic/controlpanel/coordinates.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 13:05:16.558513 contenttypes.basic-2.0/src/contenttypes/basic/fields/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2023-03-17 08:35:42.000000 contenttypes.basic-2.0/src/contenttypes/basic/fields/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)      238 2023-03-17 08:35:42.000000 contenttypes.basic-2.0/src/contenttypes/basic/fields/colour.py
+-rwxrwxrwx   0 root         (0) root         (0)      230 2023-03-17 08:35:42.000000 contenttypes.basic-2.0/src/contenttypes/basic/fields/icon.py
+-rwxrwxrwx   0 root         (0) root         (0)      234 2023-03-17 08:35:42.000000 contenttypes.basic-2.0/src/contenttypes/basic/fields/osmap.py
+-rwxr-xr-x   0 root         (0) root         (0)      267 2023-03-17 11:08:05.000000 contenttypes.basic-2.0/src/contenttypes/basic/fields/osmap_advanced.py
+-rwxr-xr-x   0 root         (0) root         (0)     2204 2023-03-17 11:08:05.000000 contenttypes.basic-2.0/src/contenttypes/basic/interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 13:05:16.559513 contenttypes.basic-2.0/src/contenttypes/basic/locales/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2023-03-17 08:35:42.000000 contenttypes.basic-2.0/src/contenttypes/basic/locales/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 13:05:16.526513 contenttypes.basic-2.0/src/contenttypes/basic/locales/ca/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 13:05:16.559513 contenttypes.basic-2.0/src/contenttypes/basic/locales/ca/LC_MESSAGES/
+-rw-r--r--   0 root         (0) root         (0)     4225 2023-03-17 11:31:36.000000 contenttypes.basic-2.0/src/contenttypes/basic/locales/ca/LC_MESSAGES/contenttypes.basic.mo
+-rwxr-xr-x   0 root         (0) root         (0)     7013 2023-03-17 11:08:05.000000 contenttypes.basic-2.0/src/contenttypes/basic/locales/ca/LC_MESSAGES/contenttypes.basic.po
+-rwxrwxrwx   0 root         (0) root         (0)       98 2023-03-17 08:35:42.000000 contenttypes.basic-2.0/src/contenttypes/basic/locales/compile.sh
+-rwxr-xr-x   0 root         (0) root         (0)     5656 2023-03-17 11:08:05.000000 contenttypes.basic-2.0/src/contenttypes/basic/locales/contenttypes.basic.pot
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 13:05:16.526513 contenttypes.basic-2.0/src/contenttypes/basic/locales/en/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 13:05:16.560513 contenttypes.basic-2.0/src/contenttypes/basic/locales/en/LC_MESSAGES/
+-rw-r--r--   0 root         (0) root         (0)     4054 2023-03-17 11:31:36.000000 contenttypes.basic-2.0/src/contenttypes/basic/locales/en/LC_MESSAGES/contenttypes.basic.mo
+-rwxr-xr-x   0 root         (0) root         (0)     6842 2023-03-17 11:08:05.000000 contenttypes.basic-2.0/src/contenttypes/basic/locales/en/LC_MESSAGES/contenttypes.basic.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 13:05:16.526513 contenttypes.basic-2.0/src/contenttypes/basic/locales/es/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 13:05:16.560513 contenttypes.basic-2.0/src/contenttypes/basic/locales/es/LC_MESSAGES/
+-rw-r--r--   0 root         (0) root         (0)     4277 2023-03-17 11:31:36.000000 contenttypes.basic-2.0/src/contenttypes/basic/locales/es/LC_MESSAGES/contenttypes.basic.mo
+-rwxr-xr-x   0 root         (0) root         (0)     7065 2023-03-17 11:08:05.000000 contenttypes.basic-2.0/src/contenttypes/basic/locales/es/LC_MESSAGES/contenttypes.basic.po
+-rwxrwxrwx   0 root         (0) root         (0)        0 2023-03-17 08:35:42.000000 contenttypes.basic-2.0/src/contenttypes/basic/locales/manual.pot
+-rwxrwxrwx   0 root         (0) root         (0)      884 2023-03-17 08:35:42.000000 contenttypes.basic-2.0/src/contenttypes/basic/locales/update.sh
+-rwxrwxrwx   0 root         (0) root         (0)      298 2023-03-17 08:35:42.000000 contenttypes.basic-2.0/src/contenttypes/basic/permissions.py
+-rwxrwxrwx   0 root         (0) root         (0)      833 2023-03-17 08:35:42.000000 contenttypes.basic-2.0/src/contenttypes/basic/permissions.zcml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 13:05:16.527513 contenttypes.basic-2.0/src/contenttypes/basic/profiles/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 13:05:16.561513 contenttypes.basic-2.0/src/contenttypes/basic/profiles/coordinates-controlpanel/
+-rwxrwxrwx   0 root         (0) root         (0)      560 2023-03-17 08:35:42.000000 contenttypes.basic-2.0/src/contenttypes/basic/profiles/coordinates-controlpanel/controlpanel.xml
+-rwxrwxrwx   0 root         (0) root         (0)      168 2023-03-17 08:35:42.000000 contenttypes.basic-2.0/src/contenttypes/basic/profiles/coordinates-controlpanel/registry.xml
+-rwxrwxrwx   0 root         (0) root         (0)      255 2023-03-17 08:35:42.000000 contenttypes.basic-2.0/src/contenttypes/basic/profiles/coordinates-controlpanel/rolemap.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 13:05:16.562513 contenttypes.basic-2.0/src/contenttypes/basic/profiles/default/
+-rwxrwxrwx   0 root         (0) root         (0)      180 2023-03-17 08:35:42.000000 contenttypes.basic-2.0/src/contenttypes/basic/profiles/default/browserlayer.xml
+-rwxrwxrwx   0 root         (0) root         (0)       90 2023-03-17 08:35:42.000000 contenttypes.basic-2.0/src/contenttypes/basic/profiles/default/metadata.xml
+-rwxrwxrwx   0 root         (0) root         (0)      954 2023-03-17 08:35:42.000000 contenttypes.basic-2.0/src/contenttypes/basic/profiles/default/rolemap.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 13:05:16.563513 contenttypes.basic-2.0/src/contenttypes/basic/profiles/default/types/
+-rwxrwxrwx   0 root         (0) root         (0)     2581 2023-03-17 08:35:42.000000 contenttypes.basic-2.0/src/contenttypes/basic/profiles/default/types/Announcement.xml
+-rwxrwxrwx   0 root         (0) root         (0)     2682 2023-03-17 08:35:42.000000 contenttypes.basic-2.0/src/contenttypes/basic/profiles/default/types/Banner.xml
+-rwxrwxrwx   0 root         (0) root         (0)     2616 2023-03-17 08:35:42.000000 contenttypes.basic-2.0/src/contenttypes/basic/profiles/default/types/Icon.xml
+-rwxrwxrwx   0 root         (0) root         (0)     2674 2023-03-17 08:35:42.000000 contenttypes.basic-2.0/src/contenttypes/basic/profiles/default/types/Slide.xml
+-rwxrwxrwx   0 root         (0) root         (0)      326 2023-03-17 08:35:42.000000 contenttypes.basic-2.0/src/contenttypes/basic/profiles/default/types.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 13:05:16.563513 contenttypes.basic-2.0/src/contenttypes/basic/profiles/uninstall/
+-rwxrwxrwx   0 root         (0) root         (0)      128 2023-03-17 08:35:42.000000 contenttypes.basic-2.0/src/contenttypes/basic/profiles/uninstall/browserlayer.xml
+-rwxrwxrwx   0 root         (0) root         (0)      574 2023-03-17 08:35:42.000000 contenttypes.basic-2.0/src/contenttypes/basic/setuphandlers.py
+-rwxrwxrwx   0 root         (0) root         (0)     2086 2023-03-17 08:35:42.000000 contenttypes.basic-2.0/src/contenttypes/basic/testing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 13:05:16.564513 contenttypes.basic-2.0/src/contenttypes/basic/tests/
+-rwxrwxrwx   0 root         (0) root         (0)     1215 2023-03-17 08:35:42.000000 contenttypes.basic-2.0/src/contenttypes/basic/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 13:05:16.564513 contenttypes.basic-2.0/src/contenttypes/basic/tests/robot/
+-rwxrwxrwx   0 root         (0) root         (0)     2003 2023-03-17 08:35:42.000000 contenttypes.basic-2.0/src/contenttypes/basic/tests/robot/test_example.robot
+-rwxrwxrwx   0 root         (0) root         (0)     5888 2023-03-17 08:35:42.000000 contenttypes.basic-2.0/src/contenttypes/basic/tests/test_behaviors.py
+-rwxrwxrwx   0 root         (0) root         (0)      913 2023-03-17 08:35:42.000000 contenttypes.basic-2.0/src/contenttypes/basic/tests/test_controlpanel.py
+-rwxrwxrwx   0 root         (0) root         (0)     2376 2023-03-17 08:35:42.000000 contenttypes.basic-2.0/src/contenttypes/basic/tests/test_converters.py
+-rwxrwxrwx   0 root         (0) root         (0)      890 2023-03-17 08:35:42.000000 contenttypes.basic-2.0/src/contenttypes/basic/tests/test_robot.py
+-rwxrwxrwx   0 root         (0) root         (0)     2421 2023-03-17 08:35:42.000000 contenttypes.basic-2.0/src/contenttypes/basic/tests/test_setup.py
+-rwxrwxrwx   0 root         (0) root         (0)     1470 2023-03-17 08:35:42.000000 contenttypes.basic-2.0/src/contenttypes/basic/tests/test_views.py
+-rwxrwxrwx   0 root         (0) root         (0)      210 2023-03-17 08:35:42.000000 contenttypes.basic-2.0/src/contenttypes/basic/upgrades.py
+-rwxrwxrwx   0 root         (0) root         (0)      387 2023-03-17 08:35:42.000000 contenttypes.basic-2.0/src/contenttypes/basic/upgrades.zcml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 13:05:16.569513 contenttypes.basic-2.0/src/contenttypes/basic/widgets/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2023-03-17 08:35:42.000000 contenttypes.basic-2.0/src/contenttypes/basic/widgets/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)      692 2023-03-17 08:35:42.000000 contenttypes.basic-2.0/src/contenttypes/basic/widgets/colour.py
+-rwxrwxrwx   0 root         (0) root         (0)      583 2023-03-17 08:35:42.000000 contenttypes.basic-2.0/src/contenttypes/basic/widgets/colour_display.pt
+-rwxrwxrwx   0 root         (0) root         (0)      630 2023-03-17 12:04:35.000000 contenttypes.basic-2.0/src/contenttypes/basic/widgets/colour_input.pt
+-rwxr-xr-x   0 root         (0) root         (0)     1994 2023-03-17 12:00:27.000000 contenttypes.basic-2.0/src/contenttypes/basic/widgets/configure.zcml
+-rwxr-xr-x   0 root         (0) root         (0)     1282 2023-03-17 11:07:58.000000 contenttypes.basic-2.0/src/contenttypes/basic/widgets/icon.py
+-rwxrwxrwx   0 root         (0) root         (0)      704 2023-03-17 08:35:42.000000 contenttypes.basic-2.0/src/contenttypes/basic/widgets/icon_display.pt
+-rwxrwxrwx   0 root         (0) root         (0)     2999 2023-03-17 13:54:09.000000 contenttypes.basic-2.0/src/contenttypes/basic/widgets/icon_input.pt
+-rwxrwxrwx   0 root         (0) root         (0)     2094 2023-03-17 08:35:42.000000 contenttypes.basic-2.0/src/contenttypes/basic/widgets/osmap.py
+-rwxr-xr-x   0 root         (0) root         (0)     2170 2023-03-17 11:08:05.000000 contenttypes.basic-2.0/src/contenttypes/basic/widgets/osmap_advanced.py
+-rwxr-xr-x   0 root         (0) root         (0)     3356 2023-03-27 12:40:18.000000 contenttypes.basic-2.0/src/contenttypes/basic/widgets/osmap_advanced_display.pt
+-rwxr-xr-x   0 root         (0) root         (0)    14983 2023-03-27 12:59:13.000000 contenttypes.basic-2.0/src/contenttypes/basic/widgets/osmap_advanced_input.pt
+-rwxrwxrwx   0 root         (0) root         (0)     2341 2023-03-17 13:17:46.000000 contenttypes.basic-2.0/src/contenttypes/basic/widgets/osmap_display.pt
+-rwxrwxrwx   0 root         (0) root         (0)     6053 2023-03-27 11:26:35.000000 contenttypes.basic-2.0/src/contenttypes/basic/widgets/osmap_input.pt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 13:05:16.532513 contenttypes.basic-2.0/src/contenttypes.basic.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4548 2023-03-27 13:05:16.000000 contenttypes.basic-2.0/src/contenttypes.basic.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5393 2023-03-27 13:05:16.000000 contenttypes.basic-2.0/src/contenttypes.basic.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-03-27 13:05:16.000000 contenttypes.basic-2.0/src/contenttypes.basic.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      123 2023-03-27 13:05:16.000000 contenttypes.basic-2.0/src/contenttypes.basic.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-03-27 13:05:16.000000 contenttypes.basic-2.0/src/contenttypes.basic.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-03-17 08:37:24.000000 contenttypes.basic-2.0/src/contenttypes.basic.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      198 2023-03-27 13:05:16.000000 contenttypes.basic-2.0/src/contenttypes.basic.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-03-27 13:05:16.000000 contenttypes.basic-2.0/src/contenttypes.basic.egg-info/top_level.txt
```

### Comparing `contenttypes.basic-1.8/CHANGES.rst` & `contenttypes.basic-2.0/CHANGES.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 Changelog
 =========
 
-
-1.8 (22/05/2023)
+2.0 (27/03/2023)
 ------------------
 
-Fixes:
-
-- Fixes to allow two OSMap widgets
-  [csanahuja]
+- Drop support Python < 3.8. [csanahuja]
+- Update widgets to Boostrap 5 and Plone 6 [csanahuja]
+- Update dependencies [csanahuja]
 
 
 1.7 (17/03/2023)
 ------------------
 
 New features:
```

### Comparing `contenttypes.basic-1.8/DEVELOP.rst` & `contenttypes.basic-2.0/DEVELOP.rst`

 * *Files identical despite different names*

### Comparing `contenttypes.basic-1.8/LICENSE.GPL` & `contenttypes.basic-2.0/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `contenttypes.basic-1.8/LICENSE.rst` & `contenttypes.basic-2.0/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `contenttypes.basic-1.8/PKG-INFO` & `contenttypes.basic-2.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 Metadata-Version: 2.1
 Name: contenttypes.basic
-Version: 1.8
+Version: 2.0
 Summary: Basic content, behaviors, fields and widgets for Plone
 Home-page: https://gitlab.com/csanahuja/contenttypes.basic/
 Author: csanahuja
 Author-email: csanahuja10@gmail.com
 License: GPL version 2
 Keywords: Python Plone
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Plone
 Classifier: Framework :: Plone :: Addon
 Classifier: Framework :: Plone :: 5.2
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Provides-Extra: test
 License-File: LICENSE.GPL
 License-File: LICENSE.rst
 
 .. This README is meant for consumption by humans and pypi. Pypi can render rst files so please do not use Sphinx features.
    If you want to learn more about writing documentation, please check out: http://docs.plone.org/about/documentation_styleguide.html
    This text does not appear on pypi or github. It is a comment.
@@ -100,22 +102,20 @@
 
 - csanahuja, csanahuja10@gmail.com
 
 
 Changelog
 =========
 
-
-1.8 (22/05/2023)
+2.0 (27/03/2023)
 ------------------
 
-Fixes:
-
-- Fixes to allow two OSMap widgets
-  [csanahuja]
+- Drop support Python < 3.8. [csanahuja]
+- Update widgets to Boostrap 5 and Plone 6 [csanahuja]
+- Update dependencies [csanahuja]
 
 
 1.7 (17/03/2023)
 ------------------
 
 New features:
```

### Comparing `contenttypes.basic-1.8/README.rst` & `contenttypes.basic-2.0/README.rst`

 * *Files identical despite different names*

### Comparing `contenttypes.basic-1.8/docs/conf.py` & `contenttypes.basic-2.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `contenttypes.basic-1.8/setup.py` & `contenttypes.basic-2.0/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -10,26 +10,28 @@
     open('CONTRIBUTORS.rst').read(),
     open('CHANGES.rst').read(),
 ])
 
 
 setup(
     name='contenttypes.basic',
-    version='1.8',
+    version='2.0',
     description="Basic content, behaviors, fields and widgets for Plone",
     long_description=long_description,
     # Get more from https://pypi.python.org/pypi?%3Aaction=list_classifiers
     classifiers=[
         "Environment :: Web Environment",
         "Framework :: Plone",
         "Framework :: Plone :: Addon",
         "Framework :: Plone :: 5.2",
         "Programming Language :: Python",
-        "Programming Language :: Python :: 3.6",
-        "Programming Language :: Python :: 3.7",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Operating System :: OS Independent",
         "License :: OSI Approved :: GNU General Public License v2 (GPLv2)",
     ],
     keywords='Python Plone',
     author='csanahuja',
     author_email='csanahuja10@gmail.com',
     url='https://gitlab.com/csanahuja/contenttypes.basic/',
@@ -39,22 +41,24 @@
     },
     license='GPL version 2',
     packages=find_packages('src', exclude=['ez_setup']),
     namespace_packages=['contenttypes'],
     package_dir={'': 'src'},
     include_package_data=True,
     zip_safe=False,
-    python_requires=">=3.6",
+    python_requires=">=3.8",
     install_requires=[
         'setuptools',
         # -*- Extra requirements: -*-
-        'z3c.jbot',
-        'plone.api>=1.8.4',
-        'plone.restapi',
+        'plone.api',
         'plone.app.dexterity',
+        'plone.app.z3cform',
+        'plone.restapi',
+        'plone.z3cform',
+        'z3c.jbot',
     ],
     extras_require={
         'test': [
             'plone.app.testing',
             # Plone KGS does not use this version, because it would break
             # Remove if your package shall be part of coredev.
             # plone_coredev tests as of 2016-04-01.
```

### Comparing `contenttypes.basic-1.8/src/contenttypes/basic/behaviors/button_text.py` & `contenttypes.basic-2.0/src/contenttypes/basic/behaviors/button_text.py`

 * *Files identical despite different names*

### Comparing `contenttypes.basic-1.8/src/contenttypes/basic/behaviors/colour.py` & `contenttypes.basic-2.0/src/contenttypes/basic/behaviors/colour.py`

 * *Files identical despite different names*

### Comparing `contenttypes.basic-1.8/src/contenttypes/basic/behaviors/configure.zcml` & `contenttypes.basic-2.0/src/contenttypes/basic/behaviors/configure.zcml`

 * *Files identical despite different names*

### Comparing `contenttypes.basic-1.8/src/contenttypes/basic/behaviors/hide_text.py` & `contenttypes.basic-2.0/src/contenttypes/basic/behaviors/hide_text.py`

 * *Files identical despite different names*

### Comparing `contenttypes.basic-1.8/src/contenttypes/basic/behaviors/icon.py` & `contenttypes.basic-2.0/src/contenttypes/basic/behaviors/icon.py`

 * *Files identical despite different names*

### Comparing `contenttypes.basic-1.8/src/contenttypes/basic/behaviors/link.py` & `contenttypes.basic-2.0/src/contenttypes/basic/behaviors/link.py`

 * *Files identical despite different names*

### Comparing `contenttypes.basic-1.8/src/contenttypes/basic/behaviors/osmap.py` & `contenttypes.basic-2.0/src/contenttypes/basic/behaviors/osmap.py`

 * *Files identical despite different names*

### Comparing `contenttypes.basic-1.8/src/contenttypes/basic/behaviors/osmap_advanced.py` & `contenttypes.basic-2.0/src/contenttypes/basic/behaviors/osmap_advanced.py`

 * *Files identical despite different names*

### Comparing `contenttypes.basic-1.8/src/contenttypes/basic/behaviors/text_position.py` & `contenttypes.basic-2.0/src/contenttypes/basic/behaviors/text_position.py`

 * *Files identical despite different names*

### Comparing `contenttypes.basic-1.8/src/contenttypes/basic/browser/configure.zcml` & `contenttypes.basic-2.0/src/contenttypes/basic/browser/configure.zcml`

 * *Files identical despite different names*

### Comparing `contenttypes.basic-1.8/src/contenttypes/basic/browser/link.pt` & `contenttypes.basic-2.0/src/contenttypes/basic/browser/link.pt`

 * *Files identical despite different names*

### Comparing `contenttypes.basic-1.8/src/contenttypes/basic/browser/link_redirect.pt` & `contenttypes.basic-2.0/src/contenttypes/basic/browser/link_redirect.pt`

 * *Files identical despite different names*

### Comparing `contenttypes.basic-1.8/src/contenttypes/basic/browser/sprite.pt` & `contenttypes.basic-2.0/src/contenttypes/basic/browser/sprite.pt`

 * *Files identical despite different names*

### Comparing `contenttypes.basic-1.8/src/contenttypes/basic/browser/static/osmap/images/layers-2x.png` & `contenttypes.basic-2.0/src/contenttypes/basic/browser/static/osmap/images/layers-2x.png`

 * *Files identical despite different names*

### Comparing `contenttypes.basic-1.8/src/contenttypes/basic/browser/static/osmap/images/layers.png` & `contenttypes.basic-2.0/src/contenttypes/basic/browser/static/osmap/images/layers.png`

 * *Files identical despite different names*

### Comparing `contenttypes.basic-1.8/src/contenttypes/basic/browser/static/osmap/images/marker-icon-2x.png` & `contenttypes.basic-2.0/src/contenttypes/basic/browser/static/osmap/images/marker-icon-2x.png`

 * *Files identical despite different names*

### Comparing `contenttypes.basic-1.8/src/contenttypes/basic/browser/static/osmap/images/marker-icon.png` & `contenttypes.basic-2.0/src/contenttypes/basic/browser/static/osmap/images/marker-icon.png`

 * *Files identical despite different names*

### Comparing `contenttypes.basic-1.8/src/contenttypes/basic/browser/static/osmap/images/marker-shadow.png` & `contenttypes.basic-2.0/src/contenttypes/basic/browser/static/osmap/images/marker-shadow.png`

 * *Files identical despite different names*

### Comparing `contenttypes.basic-1.8/src/contenttypes/basic/browser/static/osmap/leaflet-src.esm.js` & `contenttypes.basic-2.0/src/contenttypes/basic/browser/static/osmap/leaflet-src.esm.js`

 * *Files identical despite different names*

### Comparing `contenttypes.basic-1.8/src/contenttypes/basic/browser/static/osmap/leaflet-src.esm.js.map` & `contenttypes.basic-2.0/src/contenttypes/basic/browser/static/osmap/leaflet-src.esm.js.map`

 * *Files identical despite different names*

### Comparing `contenttypes.basic-1.8/src/contenttypes/basic/browser/static/osmap/leaflet-src.js` & `contenttypes.basic-2.0/src/contenttypes/basic/browser/static/osmap/leaflet-src.js`

 * *Files identical despite different names*

### Comparing `contenttypes.basic-1.8/src/contenttypes/basic/browser/static/osmap/leaflet-src.js.map` & `contenttypes.basic-2.0/src/contenttypes/basic/browser/static/osmap/leaflet-src.js.map`

 * *Files identical despite different names*

### Comparing `contenttypes.basic-1.8/src/contenttypes/basic/browser/static/osmap/leaflet.css` & `contenttypes.basic-2.0/src/contenttypes/basic/browser/static/osmap/leaflet.css`

 * *Files identical despite different names*

### Comparing `contenttypes.basic-1.8/src/contenttypes/basic/browser/static/osmap/leaflet.js` & `contenttypes.basic-2.0/src/contenttypes/basic/browser/static/osmap/leaflet.js`

 * *Files identical despite different names*

### Comparing `contenttypes.basic-1.8/src/contenttypes/basic/browser/static/osmap/leaflet.js.map` & `contenttypes.basic-2.0/src/contenttypes/basic/browser/static/osmap/leaflet.js.map`

 * *Files identical despite different names*

### Comparing `contenttypes.basic-1.8/src/contenttypes/basic/configure.zcml` & `contenttypes.basic-2.0/src/contenttypes/basic/configure.zcml`

 * *Files identical despite different names*

### Comparing `contenttypes.basic-1.8/src/contenttypes/basic/contents.py` & `contenttypes.basic-2.0/src/contenttypes/basic/contents.py`

 * *Files identical despite different names*

### Comparing `contenttypes.basic-1.8/src/contenttypes/basic/controlpanel/coordinates.py` & `contenttypes.basic-2.0/src/contenttypes/basic/controlpanel/coordinates.py`

 * *Files identical despite different names*

### Comparing `contenttypes.basic-1.8/src/contenttypes/basic/interfaces.py` & `contenttypes.basic-2.0/src/contenttypes/basic/interfaces.py`

 * *Files identical despite different names*

### Comparing `contenttypes.basic-1.8/src/contenttypes/basic/locales/ca/LC_MESSAGES/contenttypes.basic.mo` & `contenttypes.basic-2.0/src/contenttypes/basic/locales/ca/LC_MESSAGES/contenttypes.basic.mo`

 * *Files identical despite different names*

### Comparing `contenttypes.basic-1.8/src/contenttypes/basic/locales/ca/LC_MESSAGES/contenttypes.basic.po` & `contenttypes.basic-2.0/src/contenttypes/basic/locales/ca/LC_MESSAGES/contenttypes.basic.po`

 * *Files identical despite different names*

### Comparing `contenttypes.basic-1.8/src/contenttypes/basic/locales/contenttypes.basic.pot` & `contenttypes.basic-2.0/src/contenttypes/basic/locales/contenttypes.basic.pot`

 * *Files identical despite different names*

### Comparing `contenttypes.basic-1.8/src/contenttypes/basic/locales/en/LC_MESSAGES/contenttypes.basic.mo` & `contenttypes.basic-2.0/src/contenttypes/basic/locales/en/LC_MESSAGES/contenttypes.basic.mo`

 * *Files identical despite different names*

### Comparing `contenttypes.basic-1.8/src/contenttypes/basic/locales/en/LC_MESSAGES/contenttypes.basic.po` & `contenttypes.basic-2.0/src/contenttypes/basic/locales/en/LC_MESSAGES/contenttypes.basic.po`

 * *Files identical despite different names*

### Comparing `contenttypes.basic-1.8/src/contenttypes/basic/locales/es/LC_MESSAGES/contenttypes.basic.mo` & `contenttypes.basic-2.0/src/contenttypes/basic/locales/es/LC_MESSAGES/contenttypes.basic.mo`

 * *Files identical despite different names*

### Comparing `contenttypes.basic-1.8/src/contenttypes/basic/locales/es/LC_MESSAGES/contenttypes.basic.po` & `contenttypes.basic-2.0/src/contenttypes/basic/locales/es/LC_MESSAGES/contenttypes.basic.po`

 * *Files identical despite different names*

### Comparing `contenttypes.basic-1.8/src/contenttypes/basic/locales/update.sh` & `contenttypes.basic-2.0/src/contenttypes/basic/locales/update.sh`

 * *Files identical despite different names*

### Comparing `contenttypes.basic-1.8/src/contenttypes/basic/permissions.zcml` & `contenttypes.basic-2.0/src/contenttypes/basic/permissions.zcml`

 * *Files identical despite different names*

### Comparing `contenttypes.basic-1.8/src/contenttypes/basic/profiles/coordinates-controlpanel/controlpanel.xml` & `contenttypes.basic-2.0/src/contenttypes/basic/profiles/coordinates-controlpanel/controlpanel.xml`

 * *Files identical despite different names*

### Comparing `contenttypes.basic-1.8/src/contenttypes/basic/profiles/default/rolemap.xml` & `contenttypes.basic-2.0/src/contenttypes/basic/profiles/default/rolemap.xml`

 * *Files identical despite different names*

### Comparing `contenttypes.basic-1.8/src/contenttypes/basic/profiles/default/types/Announcement.xml` & `contenttypes.basic-2.0/src/contenttypes/basic/profiles/default/types/Announcement.xml`

 * *Files identical despite different names*

### Comparing `contenttypes.basic-1.8/src/contenttypes/basic/profiles/default/types/Banner.xml` & `contenttypes.basic-2.0/src/contenttypes/basic/profiles/default/types/Banner.xml`

 * *Files identical despite different names*

### Comparing `contenttypes.basic-1.8/src/contenttypes/basic/profiles/default/types/Icon.xml` & `contenttypes.basic-2.0/src/contenttypes/basic/profiles/default/types/Icon.xml`

 * *Files identical despite different names*

### Comparing `contenttypes.basic-1.8/src/contenttypes/basic/profiles/default/types/Slide.xml` & `contenttypes.basic-2.0/src/contenttypes/basic/profiles/default/types/Slide.xml`

 * *Files identical despite different names*

### Comparing `contenttypes.basic-1.8/src/contenttypes/basic/setuphandlers.py` & `contenttypes.basic-2.0/src/contenttypes/basic/setuphandlers.py`

 * *Files identical despite different names*

### Comparing `contenttypes.basic-1.8/src/contenttypes/basic/testing.py` & `contenttypes.basic-2.0/src/contenttypes/basic/testing.py`

 * *Files identical despite different names*

### Comparing `contenttypes.basic-1.8/src/contenttypes/basic/tests/__init__.py` & `contenttypes.basic-2.0/src/contenttypes/basic/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `contenttypes.basic-1.8/src/contenttypes/basic/tests/robot/test_example.robot` & `contenttypes.basic-2.0/src/contenttypes/basic/tests/robot/test_example.robot`

 * *Files identical despite different names*

### Comparing `contenttypes.basic-1.8/src/contenttypes/basic/tests/test_behaviors.py` & `contenttypes.basic-2.0/src/contenttypes/basic/tests/test_behaviors.py`

 * *Files identical despite different names*

### Comparing `contenttypes.basic-1.8/src/contenttypes/basic/tests/test_controlpanel.py` & `contenttypes.basic-2.0/src/contenttypes/basic/tests/test_controlpanel.py`

 * *Files identical despite different names*

### Comparing `contenttypes.basic-1.8/src/contenttypes/basic/tests/test_converters.py` & `contenttypes.basic-2.0/src/contenttypes/basic/tests/test_converters.py`

 * *Files identical despite different names*

### Comparing `contenttypes.basic-1.8/src/contenttypes/basic/tests/test_robot.py` & `contenttypes.basic-2.0/src/contenttypes/basic/tests/test_robot.py`

 * *Files identical despite different names*

### Comparing `contenttypes.basic-1.8/src/contenttypes/basic/tests/test_setup.py` & `contenttypes.basic-2.0/src/contenttypes/basic/tests/test_setup.py`

 * *Files identical despite different names*

### Comparing `contenttypes.basic-1.8/src/contenttypes/basic/tests/test_views.py` & `contenttypes.basic-2.0/src/contenttypes/basic/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `contenttypes.basic-1.8/src/contenttypes/basic/widgets/colour.py` & `contenttypes.basic-2.0/src/contenttypes/basic/widgets/colour.py`

 * *Files identical despite different names*

### Comparing `contenttypes.basic-1.8/src/contenttypes/basic/widgets/colour_display.pt` & `contenttypes.basic-2.0/src/contenttypes/basic/widgets/colour_display.pt`

 * *Files identical despite different names*

### Comparing `contenttypes.basic-1.8/src/contenttypes/basic/widgets/colour_input.pt` & `contenttypes.basic-2.0/src/contenttypes/basic/widgets/colour_input.pt`

 * *Files 20% similar despite different names*

```diff
@@ -4,14 +4,14 @@
       xmlns:tal="http://xml.zope.org/namespaces/tal"
       i18n:domain="contenttypes.basic"
       tal:omit-tag="">
 
     <style>
         .colour-widget {
             width: 100px !important;
-            height: 50px !important;
+            height: 40px !important;
             padding: 5px !important;
         }
     </style>
-    <input id="form-widgets-colour_id_${python:view.id}" class="colour-widget" name="${python:view.name}" value="${python:view.value}" type="color" />
+    <input id="form-widgets-colour_id_${python:view.id}" class="colour-widget form-control" name="${python:view.name}" value="${python:view.value}" type="color" />
 
 </html>
```

### Comparing `contenttypes.basic-1.8/src/contenttypes/basic/widgets/configure.zcml` & `contenttypes.basic-2.0/src/contenttypes/basic/widgets/configure.zcml`

 * *Files 12% similar despite different names*

```diff
@@ -12,53 +12,53 @@
   
   <adapter factory=".osmap.OSMapConverter" />
   <adapter factory=".osmap_advanced.OSMapAdvancedConverter" />
   
   <z3c:widgetTemplate
     mode="input"
     widget="..interfaces.IIconWidget"
-    layer="z3c.form.interfaces.IFormLayer"
+    layer="plone.app.z3cform.interfaces.IPloneFormLayer"
     template="icon_input.pt" />
 
   <z3c:widgetTemplate
     mode="display"
     widget="..interfaces.IIconWidget"
-    layer="z3c.form.interfaces.IFormLayer"
+    layer="plone.app.z3cform.interfaces.IPloneFormLayer"
     template="icon_display.pt" />
 
   <z3c:widgetTemplate
     mode="input"
     widget="..interfaces.IColourWidget"
-    layer="z3c.form.interfaces.IFormLayer"
+    layer="plone.app.z3cform.interfaces.IPloneFormLayer"
     template="colour_input.pt" />
 
   <z3c:widgetTemplate
     mode="display"
     widget="..interfaces.IColourWidget"
-    layer="z3c.form.interfaces.IFormLayer"
+    layer="plone.app.z3cform.interfaces.IPloneFormLayer"
     template="colour_display.pt" />
 
   <z3c:widgetTemplate
     mode="input"
     widget="..interfaces.IOSMapWidget"
-    layer="z3c.form.interfaces.IFormLayer"
+    layer="plone.app.z3cform.interfaces.IPloneFormLayer"
     template="osmap_input.pt" />
 
   <z3c:widgetTemplate
     mode="display"
     widget="..interfaces.IOSMapWidget"
-    layer="z3c.form.interfaces.IFormLayer"
+    layer="plone.app.z3cform.interfaces.IPloneFormLayer"
     template="osmap_display.pt" />
 
   <z3c:widgetTemplate
     mode="input"
     widget="..interfaces.IOSMapAdvancedWidget"
-    layer="z3c.form.interfaces.IFormLayer"
+    layer="plone.app.z3cform.interfaces.IPloneFormLayer"
     template="osmap_advanced_input.pt" />
 
   <z3c:widgetTemplate
     mode="display"
     widget="..interfaces.IOSMapAdvancedWidget"
-    layer="z3c.form.interfaces.IFormLayer"
+    layer="plone.app.z3cform.interfaces.IPloneFormLayer"
     template="osmap_advanced_display.pt" />
 
 </configure>
```

### Comparing `contenttypes.basic-1.8/src/contenttypes/basic/widgets/icon.py` & `contenttypes.basic-2.0/src/contenttypes/basic/widgets/icon.py`

 * *Files identical despite different names*

### Comparing `contenttypes.basic-1.8/src/contenttypes/basic/widgets/icon_display.pt` & `contenttypes.basic-2.0/src/contenttypes/basic/widgets/icon_display.pt`

 * *Files identical despite different names*

### Comparing `contenttypes.basic-1.8/src/contenttypes/basic/widgets/icon_input.pt` & `contenttypes.basic-2.0/src/contenttypes/basic/widgets/icon_input.pt`

 * *Files 18% similar despite different names*

```diff
@@ -5,74 +5,76 @@
       i18n:domain="contenttypes.basic"
       tal:omit-tag="">
 
   <style>
     #formfield-form-widgets-icon_id { 
       position: relative; 
     }
-    .select-icon { 
-      display: inline-block; 
+    .select-icon {
+      display: inline-block;
     }
     .select-icon:hover { 
       background-color: antiquewhite;
     }
-    .icon-btn { 
-      margin-top: 10px; 
-    }
     .icon,
     .icon-choice,
     .icon-selected {
       display: inline-block; 
-      width: 5rem; 
-      height: 5rem; 
+      width: 3rem; 
+      height: 3rem; 
     }
     .pointer { 
       cursor: pointer; 
     }
     .modal-content { 
       padding: 2rem 
     }
   </style>
 
   <input type="hidden" id="form-widgets-icon_id_${python:view.id}" name="${python:view.name}" value="${python:view.value}"/>
 
-  <div class="display-flex button-div"> 
-      <a class="pat-plone-modal mr-3 btn  standalone icon-btn" href="#modal_${python:view.id}">
-        <tal:value condition="python:view.value" i18n:translate="">Change icon</tal:value>
+  <div class="button-div"> 
+      <button type="button" class="btn btn-primary me-4" data-bs-toggle="modal" data-bs-target="#modal_${python:view.id}">
         <tal:not_value condition="python:not view.value" i18n:translate="">Add icon</tal:not_value>
-      </a>
-     
+        <tal:value condition="python:view.value" i18n:translate="">Change icon</tal:value>
+      </button>
       <svg viewBox="0 0 100 100" class="icon-choice" xmlns:xlink="http://www.w3.org/1999/xlink">
         <use id="selected_icon_id_${python:view.id}" xlink:href="${python:view.portal_url}/sprite-icons#${python:view.value}"></use>
       </svg>
-    
   </div>
 
-  <div id="modal_${python:view.id}" style="display: none" class="modal fade bd-example-modal-lg" tabindex="-1" role="dialog" aria-hidden="true">
-
-    <h1 class="plone-modal-title" i18n:translate="">Select an icon</h1>
-
+  <div class="modal fade" id="modal_${python:view.id}" tabindex="-1" aria-labelledby="modalIconLabel-${python:view.id}" aria-hidden="true">
+    <div class="modal-dialog">
+      <div class="modal-content">
+        <div class="modal-header">
+          <h5 class="modal-title" id="modalIconLabel-${python:view.id}" i18n:translate="">Select an icon</h5>
+          <button type="button" class="btn-close" data-bs-dismiss="modal" aria-label="Close"></button>
+        </div>
+        <div class="modal-body">
+          <div class="d-flex flex-wrap">
+          <tal:repeat repeat="item python:view.xml">
+              <a class="select-icon m-2" href="#form-widgets-icon_id_${python:view.id}" data-id="${item}" data-modal-id="${python:view.id}">
+                  <svg viewBox="0 0 100 100" class="icon pointer shape-codepen" xmlns:xlink="http://www.w3.org/1999/xlink">
+                    <use xlink:href="sprite-icons#${item}"></use>
+                  </svg>
+              </a>
+          </tal:repeat>
+          </div>
+        </div>
+      </div>
+    </div>
+  </div>
 
-    <tal:repeat repeat="item python:view.xml">
-        <a class="select-icon" href="#form-widgets-icon_id_${python:view.id}" data-id="${item}" data-modal-id="${python:view.id}">
-            <svg viewBox="0 0 100 100" class="icon pointer shape-codepen" xmlns:xlink="http://www.w3.org/1999/xlink">
-              <use xlink:href="sprite-icons#${item}"></use>
-            </svg>
-        </a>
-    </tal:repeat>
-
-    <script keep-body="true">
-      $(function(){
-        $('.select-icon').on('click', function (e) {
-          var data_id = $(this).data('id');
-          var data_modal_id = $(this).data('modal-id');
-          var url_svg = '${python:view.portal_url}/sprite-icons#';
-          $('#form-widgets-icon_id_' + data_modal_id).attr('value', data_id);
-          $('#selected_icon_id_' + data_modal_id).attr('xlink:href', url_svg + data_id);
-          $('.plone-modal-close').click();
-        })
+  <script keep-body="true">
+    $(function() {
+      $('.select-icon').on('click', function (e) {
+        var data_id = $(this).data('id');
+        var data_modal_id = $(this).data('modal-id');
+        var url_svg = '${python:view.portal_url}/sprite-icons#';
+        $('#form-widgets-icon_id_' + data_modal_id).attr('value', data_id);
+        $('#selected_icon_id_' + data_modal_id).attr('xlink:href', url_svg + data_id);
+        $('.btn-close').click();
       })
-    </script>
-
-  </div>
+    })
+  </script>
 
 </html>
```

### Comparing `contenttypes.basic-1.8/src/contenttypes/basic/widgets/osmap.py` & `contenttypes.basic-2.0/src/contenttypes/basic/widgets/osmap.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,18 +22,14 @@
     timestamp = datetime.now().strftime('%s')
 
     @property
     def portal_url(self):
         return api.portal.get().absolute_url()
 
     @property
-    def field_name(self):
-        return self.field.getName()
-
-    @property
     def default_value(self):
         return self.field.default or '0|0'
 
     def default_value_map(self):
         try:
             return api.portal.get_registry_record(name='coordinates.map_center')
         except InvalidParameterError:
```

### Comparing `contenttypes.basic-1.8/src/contenttypes/basic/widgets/osmap_advanced.py` & `contenttypes.basic-2.0/src/contenttypes/basic/widgets/osmap_advanced.py`

 * *Files identical despite different names*

### Comparing `contenttypes.basic-1.8/src/contenttypes/basic/widgets/osmap_advanced_display.pt` & `contenttypes.basic-2.0/src/contenttypes/basic/widgets/osmap_advanced_display.pt`

 * *Files 12% similar despite different names*

```diff
@@ -3,41 +3,33 @@
       xmlns:i18n="http://xml.zope.org/namespaces/i18n"
       xmlns:tal="http://xml.zope.org/namespaces/tal"
       i18n:domain="contenttypes.basic"
       tal:omit-tag="">
 
     <link rel="stylesheet" type="text/css" href="${python:view.portal_url}/++plone++contenttypes.basic/osmap/leaflet.css">
 
-    <div tal:condition="python:view.value and view.value != '0|0'" id="osmap-widget-map-${python:view.timestamp}" 
+    <div tal:condition="python:view.value and view.value != '0|0'" id="osmap-advanced-widget-map-${python:view.timestamp}" 
         data-value="${python:view.value}"
         data-default_value_map="${python:view.default_value_map()}" 
-    style="height: 500px;"></div>
+        style="height: 500px;"></div>
 
-    <script tal:condition="python:view.value and view.value != '0|0'">
-        requirejs.config({
-            'baseUrl': PORTAL_URL,            
-            'paths':{            
-                "leaflet": "++plone++contenttypes.basic/osmap/leaflet",
-            }
-        })
-
-        require([
-            'jquery',
-            'leaflet',
-        ], function($, L) {
+    <tal:value condition="python:view.value and view.value != '0|0'">
+    <script src="${python:view.portal_url}/++plone++contenttypes.basic/osmap/leaflet.js"></script>
+    <script>
+        $(function () {
             "use strict";
             // Vars
             var timestamp = ${python:view.timestamp};
-            var mapIdSelector = '#osmap-widget-map-'+timestamp;
+            var mapIdSelector = '#osmap-advanced-widget-map-'+timestamp;
             var value = JSON.parse($(mapIdSelector).attr('data-value'));
             var defaultValueMap = $(mapIdSelector).data('default_value_map');
             const elementType = value['type']
 
             // Map
-            var osmap = L.map('osmap-widget-map-'+timestamp).setView(defaultValueMap['coordinates'][0], 15);
+            var osmap = L.map('osmap-advanced-widget-map-'+timestamp).setView(defaultValueMap['coordinates'][0], 15);
             L.tileLayer('http://{s}.tile.osm.org/{z}/{x}/{y}.png', {
                 attribution: '&copy; <a href="//osm.org/copyright">OpenStreetMap</a> contributors'
             }).addTo(osmap);
 
             if (elementType === 'polyline'){
                 renderPolyline()
             }
```

### Comparing `contenttypes.basic-1.8/src/contenttypes/basic/widgets/osmap_advanced_input.pt` & `contenttypes.basic-2.0/src/contenttypes/basic/widgets/osmap_advanced_input.pt`

 * *Files 18% similar despite different names*

```diff
@@ -1,142 +1,127 @@
 <html xmlns="http://www.w3.org/1999/xhtml"
       xmlns:metal="http://xml.zope.org/namespaces/metal"
       xmlns:i18n="http://xml.zope.org/namespaces/i18n"
       xmlns:tal="http://xml.zope.org/namespaces/tal"
       i18n:domain="contenttypes.basic"
-      tal:omit-tag="">
+      tal:omit-tag=""
+      tal:define="icons python:context.restrictedTraverse('@@iconresolver')">
 
 
     <link rel="stylesheet" type="text/css" href="${python:view.portal_url}/++plone++contenttypes.basic/osmap/leaflet.css">
-    <style>
-        .ml-2{margin-left:2rem;}
-        .my-2{margin-top:2rem; margin-bottom:2rem;}
-
-        .nav-geo{
-    background-color: #F2F1F1;
-    border-radius: 5px;
-}
-
-.nav-geo ul li a{
-    background-color: #FCFCFD;
-    border: 1px solid #e5e5e5;
-}
-
-.buscador-geo{
-    margin-top: 15px;
-    align-items: center;
-}
-
-.seatchlocate{
-    width: 150px;
-}
-
-.clear-value-wrapper{
-    margin-top: 15px;
-}
-
-    </style>
 
     <!-- Selector -->
     <div class="nav-geo">
-        <ul class="list-inline nav nav-tabs">
-            <li id="li_menu_point" class="active"><a i18n:translate="" data-toggle="tab" href="#menu_point">Point</a></li>
-            <li id="li_menu_polygon"><a i18n:translate="" data-toggle="tab" href="#menu_polygon">Polygon</a></li>
-            <li id="li_menu_polyline"><a i18n:translate="" data-toggle="tab" href="#menu_polyline">Line</a></li>
+        <ul class="list-inline nav nav-tabs" role=tablist>
+            <li id="li_menu_point" class="nav-item">
+                <button class="nav-link active" id="menu_point-tab" data-bs-toggle="tab" data-bs-target="#menu_point"
+                    type="button" role="tab" aria-controls="menu_point" aria-selected="true" i18n:translate="">Point</button>
+            <li id="li_menu_polygon" class="nav-item">
+                <button class="nav-link" id="menu_polygon-tab" data-bs-toggle="tab" data-bs-target="#menu_polygon"
+                    type="button" role="tab" aria-controls="menu_polygon" aria-selected="true" i18n:translate="">Polygon</button>                
+            </li>
+            <li id="li_menu_polyline" class="nav-item">
+                <button class="nav-link" id="menu_polyline-tab" data-bs-toggle="tab" data-bs-target="#menu_polyline"
+                    type="button" role="tab" aria-controls="menu_polyline" aria-selected="true" i18n:translate="">Line</button>                  
+            </li>
         </ul>
     </div>
 
-
-    <!-- Map -->
-    <div class="row">
-        <div class="col-xs-12">
-            <div id="osmap-widget-map-${python:view.timestamp}" style="height: 500px;z-index: 0;"></div>
-        </div>
-    </div>
-
-    <div class="tap-content">
+    <div class="tab-content">
         <!-- Point -->
-        <div id="menu_point" class="tab-pane fade in active">
-            <div class="row">
-                <div class="buscador-geo display-flex alignitems-center col-xs-12">
+        <div id="menu_point" class="tab-pane fade show active" role="tabpanel" aria-labelledby="menu_point-tab">
+
+            <div class="bg-light p-4">
+                <div class="row d-flex mb-4">
                     <input type="text" placeholder="Type an address" i18n:attributes="placeholder"
-                        tal:attributes="class python:'text-widget required textline-field' if view.required else 'text-widget textline-field'"
-                        id="osmap-widget-address-${python:view.timestamp}" />
-                    <button id="osmap-button-${python:view.timestamp}" class="ml-2 btn btn-primary seatchlocate" type="button" i18n:translate="">Search</button>
+                        class="col-xs-12 col-md-9 text-widget textline-field ${python:view.required and 'required' or ''}"
+                        id="osmap-advanced-widget-address-${python:view.timestamp}" />
+                    <div class="ps-2 col-xs-12 col-md-3 ">
+                        <button class="w-100 btn btn-primary" type="button" id="osmap-advanced-button-${python:view.timestamp}" i18n:translate="">Search</button>
+                    </div>
                 </div>
-            </div>
-            <div class="row">
-                <div class="buscador-geo display-flex alignitems-center col-xs-12">
-                    <input type="text" placeholder="Type coordinates" i18n:attributes="placeholder" id="osmap-input-corrdinates" />
-                    <button id="osmap-input-coordinates-button" class="ml-2 btn btn-primary seatchlocate" type="button" i18n:translate="">Locate</button>
+                <div class="row d-flex coordinates-wrapper">
+                    <input class="col-xs-12 col-md-8" type="text" placeholder="Type coordinates" i18n:attributes="placeholder" id="osmap-advanced-input-coordinates" />
+                    <div class="col-xs-12 col-md-4 d-flex justify-content-between">
+                        <button class="me-2 btn btn-primary flex-fill searchlocate" id="osmap-advanced-input-coordinates-button" type="button" i18n:translate="">Locate</button>
+                        <button class="btn btn-primary flex-fill" type="button" id="clear-coords-advanced-${python:view.timestamp}" i18n:translate=""> Clear coordinates </button>
+                    </div>
                 </div>
             </div>
-            <div class="row my-2 display-flex alignitems-center">
-                <div class="coordinates-wrapper col-xs-12 col-sm-3 hide" data-timestamp=${python:view.timestamp}
-                    tal:define="init_value python:view.value or False;
-                                init_value_map python:view.value or view.default_value_map();">
-                    <input type="text" id="osmap-widget-coordinates-${python:view.timestamp}" name="${python:view.name}" value="${init_value}"
-                        data-init-value="${init_value_map}" placeholder="${init_value}" />
-                </div>
 
-                <div class="clear-value-wrapper col-xs-12 col-sm-6">
-                    <button class="btn btn-primary" type="button" id="clear-coords-${python:view.timestamp}" i18n:translate=""> Clear coordinates </button>
-                </div>
-            </div>
         </div>
         <!-- Polygon -->
-        <div class="row tab-pane fade" id="menu_polygon">
-            <div class="clear-value-wrapper col-xs-6 col-sm-6">
-                <button class="btn btn-primary points_polygon_clear_last" type="button">
-                    <span class="glyphicon glyphicon-arrow-left mr-2"></span>
-                    <span i18n:translate="">Clear last</span>
-                </button>
-                <button class="btn btn-primary points_clear" type="button" i18n:translate=""> Clear points </button>
+        <div id="menu_polygon" class="tab-pane fade" role="tabpanel" aria-labelledby="menu_point-tab">
+            
+            <div class="bg-light p-4">
+                <div class="clear-value-wrapper col-xs-6 col-sm-6">
+                    <button class="btn btn-primary points_polygon_clear_last me-3" type="button">
+                        <tal:icon tal:replace="structure python:icons.tag('arrow-left', tag_class='fs-5' )" />
+                        <span i18n:translate="">Clear last</span>
+                    </button>
+                    <button class="btn btn-primary points_clear" type="button" i18n:translate="">
+                        <tal:icon tal:replace="structure python:icons.tag('arrow-clockwise', tag_class='fs-5' )" />
+                        <span i18n:translate="">Clear points</span>
+                    </button>
+                </div>
             </div>
+
         </div>
 
         <!-- Line -->
-        <div class="row tab-pane fade" id="menu_polyline">
-            <div class="clear-value-wrapper col-xs-6 col-sm-6">
-                <button class="btn btn-primary points_polyline_clear_last" type="button">
-                    <span class="glyphicon glyphicon-arrow-left mr-2"></span>
-                    <span i18n:translate="">Clear last</span>
-                </button>
-                <button class="btn btn-primary polygon_clear" type="button" i18n:translate=""> Clear points </button>
+        <div id="menu_polyline" class="tab-pane fade" role="tabpanel" aria-labelledby="menu_polyline-tab">
+            
+            <div class="bg-light p-4">
+                <div class="clear-value-wrapper col-xs-6 col-sm-6">
+                    <button class="btn btn-primary points_polyline_clear_last me-3" type="button">
+                        <tal:icon tal:replace="structure python:icons.tag('arrow-left', tag_class='fs-5' )" />
+                        <span i18n:translate="">Clear last</span>
+                    </button>
+                    <button class="btn btn-primary points_clear" type="button" i18n:translate="">
+                        <tal:icon tal:replace="structure python:icons.tag('arrow-clockwise', tag_class='fs-5' )" />
+                        <span i18n:translate="">Clear points</span>
+                    </button>
+                </div>
             </div>
+
+        </div>
+    </div>
+
+    <div class="coordinates-wrapper d-none" data-timestamp=${python:view.timestamp}
+        tal:define="init_value python:view.value or False;
+                    init_value_map python:view.value or view.default_value_map();">
+        <input type="text" id="osmap-advanced-widget-coordinates-${python:view.timestamp}" name="${python:view.name}" value="${init_value}"
+            data-init-value="${init_value_map}" placeholder="${init_value}" />
+    </div>
+
+    <!-- Map -->
+    <div class="row">
+        <div class="col-xs-12">
+            <div id="osmap-advanced-widget-map-${python:view.timestamp}" style="height: 500px;z-index: 0;"></div>
         </div>
     </div>
-    <hr>
-    <script>
-        requirejs.config({
-            'baseUrl': PORTAL_URL,            
-            'paths':{            
-                "leaflet": "++plone++contenttypes.basic/osmap/leaflet",
-            }
-        })
 
-        require([
-            'jquery',
-            'leaflet',
-        ], function($, L) {
+    <script src="${python:view.portal_url}/++plone++contenttypes.basic/osmap/leaflet.js"></script>
+    <script>
+        $(function () {
             "use strict";
 
             // Vars
             var timestamp = ${python:view.timestamp};
-            var inputAddress = $('#osmap-widget-address-'+timestamp);
-            var inputCoordinates = $('#osmap-widget-coordinates-'+timestamp);
+            var inputAddress = $('#osmap-advanced-widget-address-' + timestamp);
+            var inputCoordinates = $('#osmap-advanced-widget-coordinates-' + timestamp);
             
             const coord_data_parse = JSON.parse(inputCoordinates.attr('data-init-value'))
             const element_type = coord_data_parse['type']
             let marker = null
             let polygon = null
             let polyline = null
             let points = []
 
-            let osmap = L.map('osmap-widget-map-'+timestamp).setView(coord_data_parse['coordinates'][0], 15);
+            let osmap = L.map('osmap-advanced-widget-map-'+timestamp).setView(coord_data_parse['coordinates'][0], 15);
                 L.tileLayer('http://{s}.tile.osm.org/{z}/{x}/{y}.png', {
                     attribution: '&copy; <a href="//osm.org/copyright">OpenStreetMap</a> contributors'
                 }).addTo(osmap); 
             
             setMap(element_type)
 
             function setMap(element_type) {
@@ -148,77 +133,47 @@
                 }
                 else{
                     renderPoint()
                 }
             }
 
             function renderPoint() { 
-                $('#menu_point').removeClass('hide')
-                $('#menu_point').addClass('active in')
                 setPoint()
             }
 
             function renderPolygon(){
-                $('#li_menu_point').removeClass('active')
-                $('#li_menu_polygon').addClass('active')
-
-                $('#menu_point').addClass('hide')
-                $('#menu_point').removeClass('active in')
-                $('#menu_polyline').addClass('hide')
-                $('#menu_polygon').removeClass('hide')
-                $('#menu_polygon').addClass('active in')
                 points = coord_data_parse['coordinates']
                 polygon = L.polygon(points).addTo(osmap);
                 osmap.fitBounds(polygon.getBounds())
             }
 
             function renderPolyline(){
-
-                $('#li_menu_point').removeClass('active')
-                $('#li_menu_polyline').addClass('active')  
-
-                $('#menu_point').addClass('hide')
-                $('#menu_point').removeClass('active in')
-                $('#menu_polygon').addClass('hide')
-                $('#menu_polyline').removeClass('hide')
-                $('#menu_polyline').addClass('active in') 
                 points = coord_data_parse['coordinates']    
                 polyline = L.polyline(points).addTo(osmap);
                 osmap.fitBounds(polyline.getBounds())  
             }
 
             // Distribution functions
             
             $('#li_menu_point').on('click', function(){
                 setPoint()
-                $('#menu_polygon').addClass('hide')
-                $('#menu_polyline').addClass('hide')
-                $('#menu_point').removeClass('hide')
-
             })
             $('#li_menu_polygon').on('click', function(){
                 setPolygon()
-                $('#menu_point').addClass('hide')
-                $('#menu_polyline').addClass('hide')
-                $('#menu_polygon').removeClass('hide')
-
             })
             $('#li_menu_polyline').on('click', function(){
                 setPolyline()
-                $('#menu_point').addClass('hide')
-                $('#menu_polygon').addClass('hide')
-                $('#menu_polyline').removeClass('hide')
             })
 
             function setPoint(){
                 osmap.off('click')
                 clearMap()
                 timestamp = ${python:view.timestamp};
-                inputAddress = $('#osmap-widget-address-'+timestamp);
-                inputCoordinates = $('#osmap-widget-coordinates-'+timestamp);
+                inputAddress = $('#osmap-advanced-widget-address-'+timestamp);
+                inputCoordinates = $('#osmap-advanced-widget-coordinates-'+timestamp);
                 let coordinatesInfo = JSON.parse(inputCoordinates.attr('data-init-value'))
                 
                 marker = L.marker(coordinatesInfo['coordinates'][0], {draggable:true, autoPan:true}).addTo(osmap);
                 osmap.setView(coordinatesInfo['coordinates'][0], 15)
                 marker.on('move', debounce(updateInputCoordinatesPoint, 500));
             }
 
@@ -259,21 +214,22 @@
 
             // Show coordinates
             $('#show-coords-${python:view.timestamp}').on('input, change, click', function(e){
                 $(this).is(":checked") ? inputCoordinates.css('display', 'block') : inputCoordinates.css('display', 'none')
             });
 
             // Clear coordinates
-            $('#clear-coords-${python:view.timestamp}').on('click', function(e){
-                inputCoordinates.val('0|0')
-                $('#osmap-input-corrdinates').val(null)
+            $('#clear-coords-advanced-${python:view.timestamp}').on('click', function(e){
+                let coords = '{"type": "point", "coordinates": [["' + 0 + '", "' + 0 + '"]]}'
+                inputCoordinates.val(coords)
+                $('#osmap-advanced-input-coordinates').val('0|0')
             });
 
             // Find location
-            $('#osmap-button-${python:view.timestamp}').on('click', function(){
+            $('#osmap-advanced-button-${python:view.timestamp}').on('click', function(){
                 geolocate();
             });
 
             // Clear points
             $('.polygon_clear').on('click', () => {
                 clearMap()
                 points = []
@@ -291,40 +247,40 @@
             });
             // Clear last point - polyline
             $('.points_polyline_clear_last').on('click', () => {
                 points.pop()
                 clearMap()
                 polyline = L.polyline(points).addTo(osmap);
             });
-            $('#osmap-input-coordinates-button').on('click', () => {
+            $('#osmap-advanced-input-coordinates-button').on('click', () => {
                 setGeolocation();
             })
 
             // Resize
             let invalidateSize = setInterval(function(){ 
                 if (osmap.getSize().x !== '0')
                     clearInterval(invalidateSize);
                 osmap.invalidateSize();
             }, 500)
 
             function geolocate(event){
                 $.ajax({
-                    url: 'https://nominatim.openstreetmap.org/search?q=' + $('#osmap-widget-address-${python:view.timestamp}')[0].value + '&format=json',
+                    url: 'https://nominatim.openstreetmap.org/search?q=' + $('#osmap-advanced-widget-address-${python:view.timestamp}')[0].value + '&format=json',
                     type: "GET",
                     success: function(data){
                         if (data.length > 0){
                             marker.setLatLng([data[0]['lat'],data[0]['lon']]);
                             osmap.setView(marker.getLatLng());
                         }
                     }
                 });
             };
 
             function setGeolocation() {
-                let coord = $('#osmap-input-corrdinates').val()
+                let coord = $('#osmap-advanced-input-coordinates').val()
                 if (coord){
                     coord = coord.replace('|', ',')
                     let coordinates = coord.split(',')
                     coord = '{"type": "point", "coordinates": [["' + coordinates[0] + '", "' + coordinates[1] + '"]]}'
                     inputCoordinates.val(coord)
                     osmap.removeLayer(marker)
                     marker = L.marker(coordinates, {draggable:true, autoPan:true}).addTo(osmap);
@@ -333,15 +289,15 @@
                 }
             }
 
             function updateInputCoordinatesPoint(){
                 var coordinates = marker.getLatLng()
                 let coords = '{"type": "point", "coordinates": [["' + coordinates["lat"] + '", "' + coordinates["lng"] + '"]]}'
                 inputCoordinates.val(coords)
-                $('#osmap-input-corrdinates').val(coordinates['lat'] + ',' + coordinates['lng'])
+                $('#osmap-advanced-input-coordinates').val(coordinates['lat'] + '|' + coordinates['lng'])
             }
             function updateInputCoordinates(selector, coords){
                 var coordinates = '{"type": "' + selector + '", "coordinates": ' + JSON.stringify(coords) + '}'
                 inputCoordinates.val(coordinates)
             }
 
 
@@ -372,13 +328,13 @@
                         if (!immediate) func.apply(context, args);
                     };
                     var callNow = immediate && !timeout;
                     clearTimeout(timeout);
                     timeout = setTimeout(later, wait);
                     if (callNow) func.apply(context, args);
                 };
-            };
+            }
 
-        });
+        })
     </script>
 
 </html>
```

### Comparing `contenttypes.basic-1.8/src/contenttypes/basic/widgets/osmap_display.pt` & `contenttypes.basic-2.0/src/contenttypes/basic/widgets/osmap_display.pt`

 * *Files 18% similar despite different names*

```diff
@@ -3,37 +3,29 @@
       xmlns:i18n="http://xml.zope.org/namespaces/i18n"
       xmlns:tal="http://xml.zope.org/namespaces/tal"
       i18n:domain="contenttypes.basic"
       tal:omit-tag="">
 
     <link rel="stylesheet" type="text/css" href="${python:view.portal_url}/++plone++contenttypes.basic/osmap/leaflet.css">
 
-    <div tal:condition="python:view.value and view.value != '0|0'" id="osmap-widget-map-${python:view.field_name}-${python:view.timestamp}" data-value="${python:view.value}" style="height: 500px;"></div>
+    <div tal:condition="python:view.value and view.value != '0|0'" id="osmap-widget-map-${python:view.timestamp}" data-value="${python:view.value}" style="height: 500px;"></div>
 
-    <script tal:condition="python:view.value and view.value != '0|0'">
-        requirejs.config({
-            'baseUrl': PORTAL_URL,            
-            'paths':{            
-                "leaflet": "++plone++contenttypes.basic/osmap/leaflet",
-            }
-        })
+    <tal:value condition="python:view.value and view.value != '0|0'">
+    <script src="${python:view.portal_url}/++plone++contenttypes.basic/osmap/leaflet.js"></script>
+    <script>
+        $(function () {
 
-        require([
-            'jquery',
-            'leaflet',
-        ], function($, L) {
             "use strict";
             // Vars
             var timestamp = ${python:view.timestamp};
-            var name = '${python:view.field_name}';
-            var mapIdSelector = '#osmap-widget-map-'+name+'-'+timestamp;
+            var mapIdSelector = '#osmap-widget-map-'+timestamp;
             var value = parseLatLng($(mapIdSelector).attr('data-value'));
 
             // Map
-            var osmap = L.map('osmap-widget-map-'+name+'-'+timestamp).setView([value.lat, value.lng], 15);
+            var osmap = L.map('osmap-widget-map-'+timestamp).setView([value.lat, value.lng], 15);
             L.tileLayer('http://{s}.tile.osm.org/{z}/{x}/{y}.png', {
                 attribution: '&copy; <a href="//osm.org/copyright">OpenStreetMap</a> contributors'
             }).addTo(osmap);
 
             // Marker
             L.marker([value.lat, value.lng]).addTo(osmap);
 
@@ -57,11 +49,11 @@
                         lat: parseFloat(coors[0]),
                         lng: parseFloat(coors[1])
                     }
                     return coors
                 }
             }
 
-        });
+        })
     </script>
 
 </html>
```

### Comparing `contenttypes.basic-1.8/src/contenttypes/basic/widgets/osmap_input.pt` & `contenttypes.basic-2.0/src/contenttypes/basic/widgets/osmap_input.pt`

 * *Files 14% similar despite different names*

```diff
@@ -3,70 +3,56 @@
       xmlns:i18n="http://xml.zope.org/namespaces/i18n"
       xmlns:tal="http://xml.zope.org/namespaces/tal"
       i18n:domain="contenttypes.basic"
       tal:omit-tag="">
 
 
     <link rel="stylesheet" type="text/css" href="${python:view.portal_url}/++plone++contenttypes.basic/osmap/leaflet.css">
-    <style>
-        .ml-2{margin-left:2rem;}
-        .my-2{margin-top:2rem; margin-bottom:2rem;}
-    </style>
 
     <div class="row">
-        <div class="display-flex alignitems-center col-xs-12">
-            <input type="text" placeholder="Type an address" i18n:attributes="placeholder"
-                tal:attributes="class python:'text-widget required textline-field' if view.required else 'text-widget textline-field'"
-                id="osmap-widget-address-${python:view.field_name}-${python:view.timestamp}" />
-            <button id="osmap-button-${python:view.field_name}-${python:view.timestamp}" class="ml-2 btn btn-primary" type="button" i18n:translate="">Search</button>
-        </div>
-    </div>
-
-    <div class="row my-2 display-flex alignitems-center">
-        <div class="coordinates-wrapper col-xs-12 col-sm-3" 
-            tal:define="init_value python:view.value != '0|0' and view.value or view.default_value;
-                        init_value_map python:view.value != '0|0' and view.value or view.default_value_map();">
-            <input type="text" id="osmap-widget-coordinates-${python:view.field_name}-${python:view.timestamp}" name="${python:view.name}" value="${init_value}"
-                data-init-value="${init_value_map}" placeholder="${init_value}" />
-        </div>
-
-        <div class="clear-value-wrapper col-xs-12 col-sm-6">
-            <button class="btn btn-primary" type="button" id="clear-coords-${python:view.field_name}-${python:view.timestamp}" i18n:translate=""> Clear coordinates </button>
+        <div class="col-xs-12">
+            <div class="bg-light p-4">
+                <div class="row d-flex mb-4">
+                    <input type="text" placeholder="Type an address" i18n:attributes="placeholder"
+                       class="col-xs-12 col-md-9 text-widget textline-field ${python:view.required and 'required' or ''}"
+                        id="osmap-widget-address-${python:view.timestamp}" />
+                    <div class="ps-2 col-xs-12 col-md-3 ">
+                        <button class="w-100 btn btn-primary" type="button" id="osmap-button-${python:view.timestamp}" i18n:translate="">Search</button>
+                    </div>
+                </div>
+                <div class="row coordinates-wrapper d-flex"
+                    tal:define="init_value python:view.value != '0|0' and view.value or view.default_value;
+                                init_value_map python:view.value != '0|0' and view.value or view.default_value_map();">
+                    <input class="col-xs-12 col-md-9" readonly type="text" id="osmap-widget-coordinates-${python:view.timestamp}" name="${python:view.name}" value="${init_value}"
+                        data-init-value="${init_value_map}" placeholder="${init_value}" />
+                    <div class="ps-2 col-xs-12 col-md-3 ">
+                        <button class="w-100 btn btn-primary" type="button" id="clear-coords-${python:view.timestamp}" i18n:translate=""> Clear coordinates </button>
+                    </div>
+                </div>
+            </div>
         </div>
-    </div>
   
-    <div class="row">
         <div class="col-xs-12">
-            <div id="osmap-widget-map-${python:view.field_name}-${python:view.timestamp}" style="height: 500px;z-index: 0;"></div>
+            <div id="osmap-widget-map-${python:view.timestamp}" style="height: 500px;z-index: 0;"></div>
         </div>
     </div>
 
+    <script src="${python:view.portal_url}/++plone++contenttypes.basic/osmap/leaflet.js"></script>
     <script>
-        requirejs.config({
-            'baseUrl': PORTAL_URL,            
-            'paths':{            
-                "leaflet": "++plone++contenttypes.basic/osmap/leaflet",
-            }
-        })
-
-        require([
-            'jquery',
-            'leaflet',
-        ], function($, L) {
+        $(function () {
             "use strict";
 
             // Vars
             var timestamp = ${python:view.timestamp};
-            var name = '${python:view.field_name}';
-            var inputAddress = $('#osmap-widget-address-'+name+'-'+timestamp);
-            var inputCoordinates = $('#osmap-widget-coordinates-'+name+'-'+timestamp);
+            var inputAddress = $('#osmap-widget-address-'+timestamp);
+            var inputCoordinates = $('#osmap-widget-coordinates-'+timestamp);
             var value = parseLatLng(inputCoordinates.attr('data-init-value'));
 
             // Map
-            var osmap = L.map('osmap-widget-map-'+name+'-'+timestamp).setView([value.lat, value.lng], 15);
+            var osmap = L.map('osmap-widget-map-'+timestamp).setView([value.lat, value.lng], 15);
             L.tileLayer('http://{s}.tile.osm.org/{z}/{x}/{y}.png', {
                 attribution: '&copy; <a href="//osm.org/copyright">OpenStreetMap</a> contributors'
             }).addTo(osmap);
 
             // Marker
             var marker = L.marker([value.lat, value.lng], {draggable:true, autoPan:true}).addTo(osmap);
 
@@ -74,31 +60,31 @@
             let invalidateSize = setInterval(function(){ 
                 if (osmap.getSize().x !== '0')
                     clearInterval(invalidateSize);
                 osmap.invalidateSize();
             }, 500)
 
             // Show coordinates
-            $('#show-coords-${python:view.name}-${python:view.timestamp}').on('input, change, click', function(e){
+            $('#show-coords-${python:view.timestamp}').on('input, change, click', function(e){
                 $(this).is(":checked") ? inputCoordinates.css('display', 'block') : inputCoordinates.css('display', 'none')
             });
 
             // Clear coordinates
-            $('#clear-coords-${python:view.name}-${python:view.timestamp}').on('click', function(e){
+            $('#clear-coords-${python:view.timestamp}').on('click', function(e){
                 inputCoordinates.val('0|0')
             });
 
             // Find location
-            $('#osmap-button-${python:view.name}-${python:view.timestamp}').on('click', function(){
+            $('#osmap-button-${python:view.timestamp}').on('click', function(){
                 geolocate();
             });
 
             function geolocate(event){
                 $.ajax({
-                    url: 'https://nominatim.openstreetmap.org/search?q=' + $('#osmap-widget-address-${python:view.name}-${python:view.timestamp}')[0].value + '&format=json',
+                    url: 'https://nominatim.openstreetmap.org/search?q=' + $('#osmap-widget-address-${python:view.timestamp}')[0].value + '&format=json',
                     type: "GET",
                     success: function(data){
                         if (data.length > 0){
                             marker.setLatLng([data[0]['lat'],data[0]['lon']]);
                             osmap.setView(marker.getLatLng());
                         }
                     }
```

### Comparing `contenttypes.basic-1.8/src/contenttypes.basic.egg-info/PKG-INFO` & `contenttypes.basic-2.0/src/contenttypes.basic.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 Metadata-Version: 2.1
 Name: contenttypes.basic
-Version: 1.8
+Version: 2.0
 Summary: Basic content, behaviors, fields and widgets for Plone
 Home-page: https://gitlab.com/csanahuja/contenttypes.basic/
 Author: csanahuja
 Author-email: csanahuja10@gmail.com
 License: GPL version 2
 Keywords: Python Plone
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Plone
 Classifier: Framework :: Plone :: Addon
 Classifier: Framework :: Plone :: 5.2
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Provides-Extra: test
 License-File: LICENSE.GPL
 License-File: LICENSE.rst
 
 .. This README is meant for consumption by humans and pypi. Pypi can render rst files so please do not use Sphinx features.
    If you want to learn more about writing documentation, please check out: http://docs.plone.org/about/documentation_styleguide.html
    This text does not appear on pypi or github. It is a comment.
@@ -100,22 +102,20 @@
 
 - csanahuja, csanahuja10@gmail.com
 
 
 Changelog
 =========
 
-
-1.8 (22/05/2023)
+2.0 (27/03/2023)
 ------------------
 
-Fixes:
-
-- Fixes to allow two OSMap widgets
-  [csanahuja]
+- Drop support Python < 3.8. [csanahuja]
+- Update widgets to Boostrap 5 and Plone 6 [csanahuja]
+- Update dependencies [csanahuja]
 
 
 1.7 (17/03/2023)
 ------------------
 
 New features:
```

### Comparing `contenttypes.basic-1.8/src/contenttypes.basic.egg-info/SOURCES.txt` & `contenttypes.basic-2.0/src/contenttypes.basic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

