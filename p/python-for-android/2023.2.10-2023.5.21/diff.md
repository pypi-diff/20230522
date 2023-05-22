# Comparing `tmp/python-for-android-2023.2.10.tar.gz` & `tmp/python-for-android-2023.5.21.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-for-android-2023.2.10.tar", last modified: Sat Feb 11 09:23:29 2023, max compression
+gzip compressed data, was "python-for-android-2023.5.21.tar", last modified: Mon May 22 17:28:07 2023, max compression
```

## Comparing `python-for-android-2023.2.10.tar` & `python-for-android-2023.5.21.tar`

### file list

```diff
@@ -1,784 +1,788 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.463468 python-for-android-2023.2.10/
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/.deepsource.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8172 2023-02-11 09:23:29.463468 python-for-android-2023.2.10/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7084 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.411468 python-for-android-2023.2.10/ci/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/ci/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1453 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/ci/constants.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3810 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/ci/rebuild_updated_recipes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.411468 python-for-android-2023.2.10/doc/
--rw-r--r--   0 runner    (1001) docker     (123)     7467 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/doc/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     7281 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/doc/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.411468 python-for-android-2023.2.10/doc/source/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.411468 python-for-android-2023.2.10/doc/source/_static/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/doc/source/_static/.empty
--rw-r--r--   0 runner    (1001) docker     (123)    15750 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/doc/source/apis.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/doc/source/bootstraps.rst
--rw-r--r--   0 runner    (1001) docker     (123)    10915 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/doc/source/buildoptions.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2933 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/doc/source/commands.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9692 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/doc/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)    10465 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/doc/source/contribute.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4883 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/doc/source/distutils.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/doc/source/docker.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.391468 python-for-android-2023.2.10/doc/source/ext/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.415468 python-for-android-2023.2.10/doc/source/ext/sphinx_rtd_theme/
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/doc/source/ext/sphinx_rtd_theme/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/doc/source/ext/sphinx_rtd_theme/Gemfile
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/doc/source/ext/sphinx_rtd_theme/Gemfile.lock
--rw-r--r--   0 runner    (1001) docker     (123)     2948 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/doc/source/ext/sphinx_rtd_theme/Gruntfile.js
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/doc/source/ext/sphinx_rtd_theme/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/doc/source/ext/sphinx_rtd_theme/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6150 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/doc/source/ext/sphinx_rtd_theme/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      570 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/doc/source/ext/sphinx_rtd_theme/bower.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.415468 python-for-android-2023.2.10/doc/source/ext/sphinx_rtd_theme/demo_docs/
--rw-r--r--   0 runner    (1001) docker     (123)     5621 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/doc/source/ext/sphinx_rtd_theme/demo_docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.415468 python-for-android-2023.2.10/doc/source/ext/sphinx_rtd_theme/demo_docs/source/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/doc/source/ext/sphinx_rtd_theme/demo_docs/source/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8213 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/doc/source/ext/sphinx_rtd_theme/demo_docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)    15469 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/doc/source/ext/sphinx_rtd_theme/demo_docs/source/demo.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7776 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/doc/source/ext/sphinx_rtd_theme/demo_docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/doc/source/ext/sphinx_rtd_theme/demo_docs/source/list.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.415468 python-for-android-2023.2.10/doc/source/ext/sphinx_rtd_theme/demo_docs/source/static/
--rw-r--r--   0 runner    (1001) docker     (123)     9498 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/doc/source/ext/sphinx_rtd_theme/demo_docs/source/static/yi_jing_01_chien.jpg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.415468 python-for-android-2023.2.10/doc/source/ext/sphinx_rtd_theme/demo_docs/source/test_py_module/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/doc/source/ext/sphinx_rtd_theme/demo_docs/source/test_py_module/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2855 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/doc/source/ext/sphinx_rtd_theme/demo_docs/source/test_py_module/test.py
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/doc/source/ext/sphinx_rtd_theme/package.json
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/doc/source/ext/sphinx_rtd_theme/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.415468 python-for-android-2023.2.10/doc/source/ext/sphinx_rtd_theme/sass/
--rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/doc/source/ext/sphinx_rtd_theme/sass/_theme_badge.sass
--rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/doc/source/ext/sphinx_rtd_theme/sass/_theme_badge_fa.sass
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/doc/source/ext/sphinx_rtd_theme/sass/_theme_breadcrumbs.sass
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/doc/source/ext/sphinx_rtd_theme/sass/_theme_font_awesome_compatability.sass
--rw-r--r--   0 runner    (1001) docker     (123)     7473 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/doc/source/ext/sphinx_rtd_theme/sass/_theme_layout.sass
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/doc/source/ext/sphinx_rtd_theme/sass/_theme_mathjax.sass
--rw-r--r--   0 runner    (1001) docker     (123)     9459 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/doc/source/ext/sphinx_rtd_theme/sass/_theme_rst.sass
--rw-r--r--   0 runner    (1001) docker     (123)      875 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/doc/source/ext/sphinx_rtd_theme/sass/_theme_variables.sass
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/doc/source/ext/sphinx_rtd_theme/sass/badge_only.sass
--rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/doc/source/ext/sphinx_rtd_theme/sass/theme.sass
--rw-r--r--   0 runner    (1001) docker     (123)   156671 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/doc/source/ext/sphinx_rtd_theme/screen_desktop.png
--rw-r--r--   0 runner    (1001) docker     (123)    96294 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/doc/source/ext/sphinx_rtd_theme/screen_mobile.png
--rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/doc/source/ext/sphinx_rtd_theme/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.419468 python-for-android-2023.2.10/doc/source/ext/sphinx_rtd_theme/sphinx_rtd_theme/
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/doc/source/ext/sphinx_rtd_theme/sphinx_rtd_theme/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/doc/source/ext/sphinx_rtd_theme/sphinx_rtd_theme/breadcrumbs.html
--rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/doc/source/ext/sphinx_rtd_theme/sphinx_rtd_theme/footer.html
--rw-r--r--   0 runner    (1001) docker     (123)     5355 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/doc/source/ext/sphinx_rtd_theme/sphinx_rtd_theme/layout.html
--rw-r--r--   0 runner    (1001) docker     (123)     7341 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/doc/source/ext/sphinx_rtd_theme/sphinx_rtd_theme/layout_old.html
--rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/doc/source/ext/sphinx_rtd_theme/sphinx_rtd_theme/search.html
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/doc/source/ext/sphinx_rtd_theme/sphinx_rtd_theme/searchbox.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.391468 python-for-android-2023.2.10/doc/source/ext/sphinx_rtd_theme/sphinx_rtd_theme/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.419468 python-for-android-2023.2.10/doc/source/ext/sphinx_rtd_theme/sphinx_rtd_theme/static/css/
--rw-r--r--   0 runner    (1001) docker     (123)     3403 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/doc/source/ext/sphinx_rtd_theme/sphinx_rtd_theme/static/css/badge_only.css
--rw-r--r--   0 runner    (1001) docker     (123)    88728 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/doc/source/ext/sphinx_rtd_theme/sphinx_rtd_theme/static/css/theme.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.419468 python-for-android-2023.2.10/doc/source/ext/sphinx_rtd_theme/sphinx_rtd_theme/static/fonts/
--rw-r--r--   0 runner    (1001) docker     (123)    62856 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/doc/source/ext/sphinx_rtd_theme/sphinx_rtd_theme/static/fonts/FontAwesome.otf
--rw-r--r--   0 runner    (1001) docker     (123)    38205 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/doc/source/ext/sphinx_rtd_theme/sphinx_rtd_theme/static/fonts/fontawesome-webfont.eot
--rw-r--r--   0 runner    (1001) docker     (123)   202148 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/doc/source/ext/sphinx_rtd_theme/sphinx_rtd_theme/static/fonts/fontawesome-webfont.svg
--rw-r--r--   0 runner    (1001) docker     (123)    80652 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/doc/source/ext/sphinx_rtd_theme/sphinx_rtd_theme/static/fonts/fontawesome-webfont.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    44432 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/doc/source/ext/sphinx_rtd_theme/sphinx_rtd_theme/static/fonts/fontawesome-webfont.woff
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.419468 python-for-android-2023.2.10/doc/source/ext/sphinx_rtd_theme/sphinx_rtd_theme/static/js/
--rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/doc/source/ext/sphinx_rtd_theme/sphinx_rtd_theme/static/js/theme.js
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/doc/source/ext/sphinx_rtd_theme/sphinx_rtd_theme/theme.conf
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/doc/source/ext/sphinx_rtd_theme/sphinx_rtd_theme/versions.html
--rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/doc/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3236 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/doc/source/launcher.rst
--rw-r--r--   0 runner    (1001) docker     (123)    12827 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/doc/source/quickstart.rst
--rw-r--r--   0 runner    (1001) docker     (123)    18035 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/doc/source/recipes.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5860 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/doc/source/services.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9371 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/doc/source/testing_pull_requests.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6723 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/doc/source/troubleshooting.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.419468 python-for-android-2023.2.10/python_for_android.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8172 2023-02-11 09:23:29.000000 python-for-android-2023.2.10/python_for_android.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    26700 2023-02-11 09:23:29.000000 python-for-android-2023.2.10/python_for_android.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-11 09:23:29.000000 python-for-android-2023.2.10/python_for_android.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-02-11 09:23:29.000000 python-for-android-2023.2.10/python_for_android.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-02-11 09:23:29.000000 python-for-android-2023.2.10/python_for_android.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-02-11 09:23:29.000000 python-for-android-2023.2.10/python_for_android.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.423468 python-for-android-2023.2.10/pythonforandroid/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/androidndk.py
--rw-r--r--   0 runner    (1001) docker     (123)     9942 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/archs.py
--rw-r--r--   0 runner    (1001) docker     (123)     6092 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/bdistapk.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    17302 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/bootstrap.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.423468 python-for-android-2023.2.10/pythonforandroid/bootstraps/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/bootstraps/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.391468 python-for-android-2023.2.10/pythonforandroid/bootstraps/common/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.423468 python-for-android-2023.2.10/pythonforandroid/bootstraps/common/build/
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/bootstraps/common/build/ant.properties
--rw-r--r--   0 runner    (1001) docker     (123)    42860 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/bootstraps/common/build/build.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.391468 python-for-android-2023.2.10/pythonforandroid/bootstraps/common/build/gradle/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.423468 python-for-android-2023.2.10/pythonforandroid/bootstraps/common/build/gradle/wrapper/
--rw-r--r--   0 runner    (1001) docker     (123)    51017 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/bootstraps/common/build/gradle/wrapper/gradle-wrapper.jar
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/bootstraps/common/build/gradle/wrapper/gradle-wrapper.properties
--rwxr-xr-x   0 runner    (1001) docker     (123)     5080 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/bootstraps/common/build/gradlew
--rw-r--r--   0 runner    (1001) docker     (123)     2314 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/bootstraps/common/build/gradlew.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.423468 python-for-android-2023.2.10/pythonforandroid/bootstraps/common/build/jni/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/bootstraps/common/build/jni/Android.mk
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.423468 python-for-android-2023.2.10/pythonforandroid/bootstraps/common/build/jni/application/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/bootstraps/common/build/jni/application/Android.mk
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.423468 python-for-android-2023.2.10/pythonforandroid/bootstraps/common/build/jni/application/src/
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/bootstraps/common/build/jni/application/src/Android.mk
--rw-r--r--   0 runner    (1001) docker     (123)    12797 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/bootstraps/common/build/jni/application/src/start.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.391468 python-for-android-2023.2.10/pythonforandroid/bootstraps/common/build/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.395468 python-for-android-2023.2.10/pythonforandroid/bootstraps/common/build/src/main/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.395468 python-for-android-2023.2.10/pythonforandroid/bootstraps/common/build/src/main/java/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.395468 python-for-android-2023.2.10/pythonforandroid/bootstraps/common/build/src/main/java/org/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.395468 python-for-android-2023.2.10/pythonforandroid/bootstraps/common/build/src/main/java/org/kamranzafar/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.423468 python-for-android-2023.2.10/pythonforandroid/bootstraps/common/build/src/main/java/org/kamranzafar/jtar/
--rwxr-xr-x   0 runner    (1001) docker     (123)     4308 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/bootstraps/common/build/src/main/java/org/kamranzafar/jtar/Octal.java
--rwxr-xr-x   0 runner    (1001) docker     (123)      881 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/bootstraps/common/build/src/main/java/org/kamranzafar/jtar/TarConstants.java
--rwxr-xr-x   0 runner    (1001) docker     (123)     7543 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/bootstraps/common/build/src/main/java/org/kamranzafar/jtar/TarEntry.java
--rwxr-xr-x   0 runner    (1001) docker     (123)     6536 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/bootstraps/common/build/src/main/java/org/kamranzafar/jtar/TarHeader.java
--rwxr-xr-x   0 runner    (1001) docker     (123)     5470 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/bootstraps/common/build/src/main/java/org/kamranzafar/jtar/TarInputStream.java
--rwxr-xr-x   0 runner    (1001) docker     (123)     4761 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/bootstraps/common/build/src/main/java/org/kamranzafar/jtar/TarOutputStream.java
--rwxr-xr-x   0 runner    (1001) docker     (123)     2179 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/bootstraps/common/build/src/main/java/org/kamranzafar/jtar/TarUtils.java
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.395468 python-for-android-2023.2.10/pythonforandroid/bootstraps/common/build/src/main/java/org/kivy/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.423468 python-for-android-2023.2.10/pythonforandroid/bootstraps/common/build/src/main/java/org/kivy/android/
--rw-r--r--   0 runner    (1001) docker     (123)     7472 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/bootstraps/common/build/src/main/java/org/kivy/android/PythonService.java
--rw-r--r--   0 runner    (1001) docker     (123)     8807 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/bootstraps/common/build/src/main/java/org/kivy/android/PythonUtil.java
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.395468 python-for-android-2023.2.10/pythonforandroid/bootstraps/common/build/src/main/java/org/renpy/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.423468 python-for-android-2023.2.10/pythonforandroid/bootstraps/common/build/src/main/java/org/renpy/android/
--rw-r--r--   0 runner    (1001) docker     (123)     3174 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/bootstraps/common/build/src/main/java/org/renpy/android/AssetExtract.java
--rw-r--r--   0 runner    (1001) docker     (123)     8874 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/bootstraps/common/build/src/main/java/org/renpy/android/Hardware.java
--rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/bootstraps/common/build/src/main/java/org/renpy/android/ResourceManager.java
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.427468 python-for-android-2023.2.10/pythonforandroid/bootstraps/common/build/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/bootstraps/common/build/templates/Service.tmpl.java
--rw-r--r--   0 runner    (1001) docker     (123)      881 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/bootstraps/common/build/templates/build.properties
--rw-r--r--   0 runner    (1001) docker     (123)     3047 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/bootstraps/common/build/templates/build.tmpl.gradle
--rw-r--r--   0 runner    (1001) docker     (123)     4034 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/bootstraps/common/build/templates/build.tmpl.xml
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/bootstraps/common/build/templates/custom_rules.tmpl.xml
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/bootstraps/common/build/templates/gradle.tmpl.properties
--rw-r--r--   0 runner    (1001) docker     (123)     3229 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/bootstraps/common/build/templates/kivy-icon.png
--rw-r--r--   0 runner    (1001) docker     (123)    11584 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/bootstraps/common/build/templates/kivy-presplash.jpg
--rw-r--r--   0 runner    (1001) docker     (123)      757 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/bootstraps/common/build/templates/lottie.xml
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/bootstraps/common/build/whitelist.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.427468 python-for-android-2023.2.10/pythonforandroid/bootstraps/empty/
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/bootstraps/empty/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.427468 python-for-android-2023.2.10/pythonforandroid/bootstraps/empty/build/
--rw-r--r--   0 runner    (1001) docker     (123)        2 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/bootstraps/empty/build/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.427468 python-for-android-2023.2.10/pythonforandroid/bootstraps/sdl2/
--rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/bootstraps/sdl2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.427468 python-for-android-2023.2.10/pythonforandroid/bootstraps/sdl2/build/
--rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/bootstraps/sdl2/build/blacklist.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.427468 python-for-android-2023.2.10/pythonforandroid/bootstraps/sdl2/build/jni/
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/bootstraps/sdl2/build/jni/Application.mk
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.395468 python-for-android-2023.2.10/pythonforandroid/bootstraps/sdl2/build/jni/application/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.427468 python-for-android-2023.2.10/pythonforandroid/bootstraps/sdl2/build/jni/application/src/
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/bootstraps/sdl2/build/jni/application/src/Android_static.mk
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/bootstraps/sdl2/build/jni/application/src/bootstrap_name.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.395468 python-for-android-2023.2.10/pythonforandroid/bootstraps/sdl2/build/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.395468 python-for-android-2023.2.10/pythonforandroid/bootstraps/sdl2/build/src/main/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.427468 python-for-android-2023.2.10/pythonforandroid/bootstraps/sdl2/build/src/main/assets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/bootstraps/sdl2/build/src/main/assets/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.427468 python-for-android-2023.2.10/pythonforandroid/bootstraps/sdl2/build/src/main/java/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/bootstraps/sdl2/build/src/main/java/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.395468 python-for-android-2023.2.10/pythonforandroid/bootstraps/sdl2/build/src/main/java/org/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.395468 python-for-android-2023.2.10/pythonforandroid/bootstraps/sdl2/build/src/main/java/org/kivy/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.427468 python-for-android-2023.2.10/pythonforandroid/bootstraps/sdl2/build/src/main/java/org/kivy/android/
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/bootstraps/sdl2/build/src/main/java/org/kivy/android/GenericBroadcastReceiver.java
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/bootstraps/sdl2/build/src/main/java/org/kivy/android/GenericBroadcastReceiverCallback.java
--rw-r--r--   0 runner    (1001) docker     (123)    24939 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/bootstraps/sdl2/build/src/main/java/org/kivy/android/PythonActivity.java
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.427468 python-for-android-2023.2.10/pythonforandroid/bootstraps/sdl2/build/src/main/java/org/kivy/android/launcher/
--rw-r--r--   0 runner    (1001) docker     (123)     2824 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/bootstraps/sdl2/build/src/main/java/org/kivy/android/launcher/Project.java
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/bootstraps/sdl2/build/src/main/java/org/kivy/android/launcher/ProjectAdapter.java
--rw-r--r--   0 runner    (1001) docker     (123)     2605 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/bootstraps/sdl2/build/src/main/java/org/kivy/android/launcher/ProjectChooser.java
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.427468 python-for-android-2023.2.10/pythonforandroid/bootstraps/sdl2/build/src/main/jniLibs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/bootstraps/sdl2/build/src/main/jniLibs/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.427468 python-for-android-2023.2.10/pythonforandroid/bootstraps/sdl2/build/src/main/libs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/bootstraps/sdl2/build/src/main/libs/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.395468 python-for-android-2023.2.10/pythonforandroid/bootstraps/sdl2/build/src/main/res/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.427468 python-for-android-2023.2.10/pythonforandroid/bootstraps/sdl2/build/src/main/res/drawable/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/bootstraps/sdl2/build/src/main/res/drawable/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.427468 python-for-android-2023.2.10/pythonforandroid/bootstraps/sdl2/build/src/main/res/drawable-hdpi/
--rw-r--r--   0 runner    (1001) docker     (123)     2683 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/bootstraps/sdl2/build/src/main/res/drawable-hdpi/ic_launcher.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.427468 python-for-android-2023.2.10/pythonforandroid/bootstraps/sdl2/build/src/main/res/drawable-mdpi/
--rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/bootstraps/sdl2/build/src/main/res/drawable-mdpi/ic_launcher.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.427468 python-for-android-2023.2.10/pythonforandroid/bootstraps/sdl2/build/src/main/res/drawable-xhdpi/
--rw-r--r--   0 runner    (1001) docker     (123)     3872 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/bootstraps/sdl2/build/src/main/res/drawable-xhdpi/ic_launcher.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.427468 python-for-android-2023.2.10/pythonforandroid/bootstraps/sdl2/build/src/main/res/drawable-xxhdpi/
--rw-r--r--   0 runner    (1001) docker     (123)     6874 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/bootstraps/sdl2/build/src/main/res/drawable-xxhdpi/ic_launcher.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.427468 python-for-android-2023.2.10/pythonforandroid/bootstraps/sdl2/build/src/main/res/layout/
--rw-r--r--   0 runner    (1001) docker     (123)      956 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/bootstraps/sdl2/build/src/main/res/layout/chooser_item.xml
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/bootstraps/sdl2/build/src/main/res/layout/main.xml
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/bootstraps/sdl2/build/src/main/res/layout/project_chooser.xml
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/bootstraps/sdl2/build/src/main/res/layout/project_empty.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.427468 python-for-android-2023.2.10/pythonforandroid/bootstraps/sdl2/build/src/main/res/mipmap/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/bootstraps/sdl2/build/src/main/res/mipmap/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.427468 python-for-android-2023.2.10/pythonforandroid/bootstraps/sdl2/build/src/main/res/mipmap-anydpi-v26/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/bootstraps/sdl2/build/src/main/res/mipmap-anydpi-v26/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.427468 python-for-android-2023.2.10/pythonforandroid/bootstraps/sdl2/build/src/patches/
--rw-r--r--   0 runner    (1001) docker     (123)     3084 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/bootstraps/sdl2/build/src/patches/SDLActivity.java.patch
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.427468 python-for-android-2023.2.10/pythonforandroid/bootstraps/sdl2/build/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     6115 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/bootstraps/sdl2/build/templates/AndroidManifest.tmpl.xml
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/bootstraps/sdl2/build/templates/strings.tmpl.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.431468 python-for-android-2023.2.10/pythonforandroid/bootstraps/service_library/
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/bootstraps/service_library/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.395468 python-for-android-2023.2.10/pythonforandroid/bootstraps/service_library/build/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.395468 python-for-android-2023.2.10/pythonforandroid/bootstraps/service_library/build/jni/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.395468 python-for-android-2023.2.10/pythonforandroid/bootstraps/service_library/build/jni/application/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.431468 python-for-android-2023.2.10/pythonforandroid/bootstraps/service_library/build/jni/application/src/
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/bootstraps/service_library/build/jni/application/src/bootstrap_name.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.395468 python-for-android-2023.2.10/pythonforandroid/bootstraps/service_library/build/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.395468 python-for-android-2023.2.10/pythonforandroid/bootstraps/service_library/build/src/main/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.395468 python-for-android-2023.2.10/pythonforandroid/bootstraps/service_library/build/src/main/java/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.395468 python-for-android-2023.2.10/pythonforandroid/bootstraps/service_library/build/src/main/java/org/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.395468 python-for-android-2023.2.10/pythonforandroid/bootstraps/service_library/build/src/main/java/org/kivy/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.431468 python-for-android-2023.2.10/pythonforandroid/bootstraps/service_library/build/src/main/java/org/kivy/android/
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/bootstraps/service_library/build/src/main/java/org/kivy/android/GenericBroadcastReceiver.java
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/bootstraps/service_library/build/src/main/java/org/kivy/android/GenericBroadcastReceiverCallback.java
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/bootstraps/service_library/build/src/main/java/org/kivy/android/PythonActivity.java
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.395468 python-for-android-2023.2.10/pythonforandroid/bootstraps/service_library/build/src/main/res/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.431468 python-for-android-2023.2.10/pythonforandroid/bootstraps/service_library/build/src/main/res/mipmap/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/bootstraps/service_library/build/src/main/res/mipmap/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.431468 python-for-android-2023.2.10/pythonforandroid/bootstraps/service_library/build/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      730 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/bootstraps/service_library/build/templates/AndroidManifest.tmpl.xml
--rw-r--r--   0 runner    (1001) docker     (123)     3596 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/bootstraps/service_library/build/templates/Service.tmpl.java
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.431468 python-for-android-2023.2.10/pythonforandroid/bootstraps/service_only/
--rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/bootstraps/service_only/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.431468 python-for-android-2023.2.10/pythonforandroid/bootstraps/service_only/build/
--rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/bootstraps/service_only/build/blacklist.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.431468 python-for-android-2023.2.10/pythonforandroid/bootstraps/service_only/build/jni/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/bootstraps/service_only/build/jni/Android.mk
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/bootstraps/service_only/build/jni/Application.mk
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.399468 python-for-android-2023.2.10/pythonforandroid/bootstraps/service_only/build/jni/application/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.431468 python-for-android-2023.2.10/pythonforandroid/bootstraps/service_only/build/jni/application/src/
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/bootstraps/service_only/build/jni/application/src/Android.mk
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/bootstraps/service_only/build/jni/application/src/Android_static.mk
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/bootstraps/service_only/build/jni/application/src/bootstrap_name.h
--rw-r--r--   0 runner    (1001) docker     (123)     3876 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/bootstraps/service_only/build/jni/application/src/pyjniusjni.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.399468 python-for-android-2023.2.10/pythonforandroid/bootstraps/service_only/build/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.399468 python-for-android-2023.2.10/pythonforandroid/bootstraps/service_only/build/src/main/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.431468 python-for-android-2023.2.10/pythonforandroid/bootstraps/service_only/build/src/main/assets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/bootstraps/service_only/build/src/main/assets/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.399468 python-for-android-2023.2.10/pythonforandroid/bootstraps/service_only/build/src/main/java/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.399468 python-for-android-2023.2.10/pythonforandroid/bootstraps/service_only/build/src/main/java/org/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.399468 python-for-android-2023.2.10/pythonforandroid/bootstraps/service_only/build/src/main/java/org/kivy/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.431468 python-for-android-2023.2.10/pythonforandroid/bootstraps/service_only/build/src/main/java/org/kivy/android/
--rw-r--r--   0 runner    (1001) docker     (123)    12411 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/bootstraps/service_only/build/src/main/java/org/kivy/android/PythonActivity.java
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.431468 python-for-android-2023.2.10/pythonforandroid/bootstraps/service_only/build/src/main/jniLibs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/bootstraps/service_only/build/src/main/jniLibs/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.399468 python-for-android-2023.2.10/pythonforandroid/bootstraps/service_only/build/src/main/res/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.431468 python-for-android-2023.2.10/pythonforandroid/bootstraps/service_only/build/src/main/res/drawable/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/bootstraps/service_only/build/src/main/res/drawable/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.431468 python-for-android-2023.2.10/pythonforandroid/bootstraps/service_only/build/src/main/res/mipmap/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/bootstraps/service_only/build/src/main/res/mipmap/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.431468 python-for-android-2023.2.10/pythonforandroid/bootstraps/service_only/build/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     4357 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/bootstraps/service_only/build/templates/AndroidManifest.tmpl.xml
--rw-r--r--   0 runner    (1001) docker     (123)     3549 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/bootstraps/service_only/build/templates/Service.tmpl.java
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/bootstraps/service_only/build/templates/strings.tmpl.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.431468 python-for-android-2023.2.10/pythonforandroid/bootstraps/webview/
--rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/bootstraps/webview/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.431468 python-for-android-2023.2.10/pythonforandroid/bootstraps/webview/build/
--rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/bootstraps/webview/build/blacklist.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.431468 python-for-android-2023.2.10/pythonforandroid/bootstraps/webview/build/jni/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/bootstraps/webview/build/jni/Android.mk
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/bootstraps/webview/build/jni/Application.mk
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.399468 python-for-android-2023.2.10/pythonforandroid/bootstraps/webview/build/jni/application/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.431468 python-for-android-2023.2.10/pythonforandroid/bootstraps/webview/build/jni/application/src/
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/bootstraps/webview/build/jni/application/src/Android.mk
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/bootstraps/webview/build/jni/application/src/Android_static.mk
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/bootstraps/webview/build/jni/application/src/bootstrap_name.h
--rw-r--r--   0 runner    (1001) docker     (123)     3876 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/bootstraps/webview/build/jni/application/src/pyjniusjni.c
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/bootstraps/webview/build/proguard-project.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.399468 python-for-android-2023.2.10/pythonforandroid/bootstraps/webview/build/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.399468 python-for-android-2023.2.10/pythonforandroid/bootstraps/webview/build/src/main/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.431468 python-for-android-2023.2.10/pythonforandroid/bootstraps/webview/build/src/main/assets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/bootstraps/webview/build/src/main/assets/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.399468 python-for-android-2023.2.10/pythonforandroid/bootstraps/webview/build/src/main/java/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.399468 python-for-android-2023.2.10/pythonforandroid/bootstraps/webview/build/src/main/java/org/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.399468 python-for-android-2023.2.10/pythonforandroid/bootstraps/webview/build/src/main/java/org/kivy/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.431468 python-for-android-2023.2.10/pythonforandroid/bootstraps/webview/build/src/main/java/org/kivy/android/
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/bootstraps/webview/build/src/main/java/org/kivy/android/GenericBroadcastReceiver.java
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/bootstraps/webview/build/src/main/java/org/kivy/android/GenericBroadcastReceiverCallback.java
--rw-r--r--   0 runner    (1001) docker     (123)    21735 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/bootstraps/webview/build/src/main/java/org/kivy/android/PythonActivity.java
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.431468 python-for-android-2023.2.10/pythonforandroid/bootstraps/webview/build/src/main/jniLibs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/bootstraps/webview/build/src/main/jniLibs/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.399468 python-for-android-2023.2.10/pythonforandroid/bootstraps/webview/build/src/main/res/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.431468 python-for-android-2023.2.10/pythonforandroid/bootstraps/webview/build/src/main/res/drawable/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/bootstraps/webview/build/src/main/res/drawable/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (123)    16525 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/bootstraps/webview/build/src/main/res/drawable/icon.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.435468 python-for-android-2023.2.10/pythonforandroid/bootstraps/webview/build/src/main/res/layout/
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/bootstraps/webview/build/src/main/res/layout/main.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.435468 python-for-android-2023.2.10/pythonforandroid/bootstraps/webview/build/src/main/res/mipmap/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/bootstraps/webview/build/src/main/res/mipmap/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.435468 python-for-android-2023.2.10/pythonforandroid/bootstraps/webview/build/src/main/res/mipmap-anydpi-v26/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/bootstraps/webview/build/src/main/res/mipmap-anydpi-v26/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.435468 python-for-android-2023.2.10/pythonforandroid/bootstraps/webview/build/src/main/res/values/
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/bootstraps/webview/build/src/main/res/values/strings.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.435468 python-for-android-2023.2.10/pythonforandroid/bootstraps/webview/build/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     5007 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/bootstraps/webview/build/templates/AndroidManifest.tmpl.xml
--rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/bootstraps/webview/build/templates/WebViewLoader.tmpl.java
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/bootstraps/webview/build/templates/strings.tmpl.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.435468 python-for-android-2023.2.10/pythonforandroid/bootstraps/webview/build/templates/test/
--rw-r--r--   0 runner    (1001) docker     (123)     3992 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/bootstraps/webview/build/templates/test/build.tmpl.xml
--rw-r--r--   0 runner    (1001) docker     (123)     3992 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/bootstraps/webview/build/templates/test/build.xml.tmpl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.435468 python-for-android-2023.2.10/pythonforandroid/bootstraps/webview/build/webview_includes/
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/bootstraps/webview/build/webview_includes/_load.html
--rw-r--r--   0 runner    (1001) docker     (123)    37883 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/build.py
--rw-r--r--   0 runner    (1001) docker     (123)    10299 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/distribution.py
--rw-r--r--   0 runner    (1001) docker     (123)      736 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/entrypoints.py
--rw-r--r--   0 runner    (1001) docker     (123)    12437 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     8350 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/patching.py
--rw-r--r--   0 runner    (1001) docker     (123)    13434 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/prerequisites.py
--rw-r--r--   0 runner    (1001) docker     (123)    30760 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/pythonpackage.py
--rw-r--r--   0 runner    (1001) docker     (123)    47248 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipe.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.435468 python-for-android-2023.2.10/pythonforandroid/recipes/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.435468 python-for-android-2023.2.10/pythonforandroid/recipes/Pillow/
--rw-r--r--   0 runner    (1001) docker     (123)     3721 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/Pillow/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.435468 python-for-android-2023.2.10/pythonforandroid/recipes/Pillow/patches/
--rw-r--r--   0 runner    (1001) docker     (123)     7980 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/Pillow/patches/fix-setup.patch
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.435468 python-for-android-2023.2.10/pythonforandroid/recipes/aiohttp/
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/aiohttp/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.435468 python-for-android-2023.2.10/pythonforandroid/recipes/android/
--rw-r--r--   0 runner    (1001) docker     (123)     2970 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/android/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.435468 python-for-android-2023.2.10/pythonforandroid/recipes/android/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.435468 python-for-android-2023.2.10/pythonforandroid/recipes/android/src/android/
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/android/src/android/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9636 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/android/src/android/_android.pyx
--rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/android/src/android/_android_billing.pyx
--rw-r--r--   0 runner    (1001) docker     (123)     3287 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/android/src/android/_android_billing_jni.c
--rw-r--r--   0 runner    (1001) docker     (123)     6312 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/android/src/android/_android_jni.c
--rw-r--r--   0 runner    (1001) docker     (123)     2869 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/android/src/android/_android_sound.pyx
--rw-r--r--   0 runner    (1001) docker     (123)     8244 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/android/src/android/_android_sound_jni.c
--rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/android/src/android/_ctypes_library_finder.py
--rw-r--r--   0 runner    (1001) docker     (123)     8159 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/android/src/android/activity.py
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/android/src/android/billing.py
--rw-r--r--   0 runner    (1001) docker     (123)     3125 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/android/src/android/broadcast.py
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/android/src/android/loadingscreen.py
--rw-r--r--   0 runner    (1001) docker     (123)     6326 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/android/src/android/mixer.py
--rw-r--r--   0 runner    (1001) docker     (123)    19697 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/android/src/android/permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1627 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/android/src/android/runnable.py
--rw-r--r--   0 runner    (1001) docker     (123)     4283 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/android/src/android/storage.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      822 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/android/src/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.435468 python-for-android-2023.2.10/pythonforandroid/recipes/apsw/
--rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/apsw/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.435468 python-for-android-2023.2.10/pythonforandroid/recipes/argon2-cffi/
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/argon2-cffi/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.435468 python-for-android-2023.2.10/pythonforandroid/recipes/atom/
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/atom/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.435468 python-for-android-2023.2.10/pythonforandroid/recipes/audiostream/
--rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/audiostream/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.435468 python-for-android-2023.2.10/pythonforandroid/recipes/babel/
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/babel/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.435468 python-for-android-2023.2.10/pythonforandroid/recipes/bcrypt/
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/bcrypt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.439468 python-for-android-2023.2.10/pythonforandroid/recipes/boost/
--rw-r--r--   0 runner    (1001) docker     (123)     3504 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/boost/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      488 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/boost/disable-so-version.patch
--rw-r--r--   0 runner    (1001) docker     (123)     3470 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/boost/fix-android-issues.patch
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/boost/use-android-libs.patch
--rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/boost/user-config.jam
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.439468 python-for-android-2023.2.10/pythonforandroid/recipes/brokenrecipe/
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/brokenrecipe/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.439468 python-for-android-2023.2.10/pythonforandroid/recipes/cffi/
--rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/cffi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/cffi/disable-pkg-config.patch
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.439468 python-for-android-2023.2.10/pythonforandroid/recipes/coverage/
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/coverage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/coverage/fallback-utf8.patch
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.439468 python-for-android-2023.2.10/pythonforandroid/recipes/cppy/
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/cppy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.439468 python-for-android-2023.2.10/pythonforandroid/recipes/cryptography/
--rw-r--r--   0 runner    (1001) docker     (123)      730 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/cryptography/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.439468 python-for-android-2023.2.10/pythonforandroid/recipes/cymunk/
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/cymunk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.439468 python-for-android-2023.2.10/pythonforandroid/recipes/cython/
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/cython/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.439468 python-for-android-2023.2.10/pythonforandroid/recipes/dateutil/
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/dateutil/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.439468 python-for-android-2023.2.10/pythonforandroid/recipes/decorator/
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/decorator/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.439468 python-for-android-2023.2.10/pythonforandroid/recipes/enaml/
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/enaml/0001-Update-setup.py.patch
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/enaml/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.439468 python-for-android-2023.2.10/pythonforandroid/recipes/ethash/
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/ethash/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.439468 python-for-android-2023.2.10/pythonforandroid/recipes/evdev/
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/evdev/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      805 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/evdev/evcnt.patch
--rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/evdev/evdev-permissions.patch
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/evdev/include-dir.patch
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/evdev/keycnt.patch
--rw-r--r--   0 runner    (1001) docker     (123)    15834 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/evdev/remove-uinput.patch
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.439468 python-for-android-2023.2.10/pythonforandroid/recipes/feedparser/
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/feedparser/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.439468 python-for-android-2023.2.10/pythonforandroid/recipes/ffmpeg/
--rw-r--r--   0 runner    (1001) docker     (123)     5522 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/ffmpeg/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.439468 python-for-android-2023.2.10/pythonforandroid/recipes/ffmpeg/patches/
--rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/ffmpeg/patches/configure.patch
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.439468 python-for-android-2023.2.10/pythonforandroid/recipes/ffpyplayer/
--rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/ffpyplayer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.439468 python-for-android-2023.2.10/pythonforandroid/recipes/ffpyplayer_codecs/
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/ffpyplayer_codecs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.439468 python-for-android-2023.2.10/pythonforandroid/recipes/flask/
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/flask/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.439468 python-for-android-2023.2.10/pythonforandroid/recipes/fontconfig/
--rw-r--r--   0 runner    (1001) docker     (123)      736 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/fontconfig/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.439468 python-for-android-2023.2.10/pythonforandroid/recipes/freetype/
--rw-r--r--   0 runner    (1001) docker     (123)     5455 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/freetype/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.439468 python-for-android-2023.2.10/pythonforandroid/recipes/freetype-py/
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/freetype-py/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/freetype-py/fall-back-to-distutils.patch
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.439468 python-for-android-2023.2.10/pythonforandroid/recipes/genericndkbuild/
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/genericndkbuild/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.439468 python-for-android-2023.2.10/pythonforandroid/recipes/gevent/
--rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/gevent/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/gevent/cross_compiling.patch
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.439468 python-for-android-2023.2.10/pythonforandroid/recipes/greenlet/
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/greenlet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.439468 python-for-android-2023.2.10/pythonforandroid/recipes/groestlcoin_hash/
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/groestlcoin_hash/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.439468 python-for-android-2023.2.10/pythonforandroid/recipes/harfbuzz/
--rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/harfbuzz/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.439468 python-for-android-2023.2.10/pythonforandroid/recipes/hostpython3/
--rw-r--r--   0 runner    (1001) docker     (123)     5109 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/hostpython3/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.443468 python-for-android-2023.2.10/pythonforandroid/recipes/hostpython3/patches/
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/hostpython3/patches/pyconfig_detection.patch
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.443468 python-for-android-2023.2.10/pythonforandroid/recipes/icu/
--rw-r--r--   0 runner    (1001) docker     (123)     4895 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/icu/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2618 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/icu/disable-libs-version.patch
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.443468 python-for-android-2023.2.10/pythonforandroid/recipes/ifaddr/
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/ifaddr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/ifaddr/getifaddrs.patch
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.443468 python-for-android-2023.2.10/pythonforandroid/recipes/ifaddrs/
--rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/ifaddrs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.443468 python-for-android-2023.2.10/pythonforandroid/recipes/jedi/
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/jedi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/jedi/fix_MergedNamesDict_get.patch
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.443468 python-for-android-2023.2.10/pythonforandroid/recipes/jpeg/
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/jpeg/Application.mk
--rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/jpeg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/jpeg/build-static.patch
--rw-r--r--   0 runner    (1001) docker     (123)      561 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/jpeg/remove-version.patch
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.443468 python-for-android-2023.2.10/pythonforandroid/recipes/kivy/
--rw-r--r--   0 runner    (1001) docker     (123)     2879 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/kivy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/kivy/sdl-gl-swapwindow-nogil.patch
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.443468 python-for-android-2023.2.10/pythonforandroid/recipes/kivy3/
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/kivy3/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.443468 python-for-android-2023.2.10/pythonforandroid/recipes/kiwisolver/
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/kiwisolver/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.443468 python-for-android-2023.2.10/pythonforandroid/recipes/lapack/
--rw-r--r--   0 runner    (1001) docker     (123)     3115 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/lapack/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.443468 python-for-android-2023.2.10/pythonforandroid/recipes/leveldb/
--rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/leveldb/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.443468 python-for-android-2023.2.10/pythonforandroid/recipes/libbz2/
--rw-r--r--   0 runner    (1001) docker     (123)     1733 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/libbz2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/libbz2/lib_android.patch
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.443468 python-for-android-2023.2.10/pythonforandroid/recipes/libcurl/
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/libcurl/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.443468 python-for-android-2023.2.10/pythonforandroid/recipes/libexpat/
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/libexpat/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.443468 python-for-android-2023.2.10/pythonforandroid/recipes/libffi/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/libffi/Application.mk
--rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/libffi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      901 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/libffi/disable-mips-check.patch
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/libffi/remove-version-info.patch
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.443468 python-for-android-2023.2.10/pythonforandroid/recipes/libgeos/
--rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/libgeos/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.443468 python-for-android-2023.2.10/pythonforandroid/recipes/libglob/
--rw-r--r--   0 runner    (1001) docker     (123)     2376 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/libglob/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27296 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/libglob/glob.patch
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.443468 python-for-android-2023.2.10/pythonforandroid/recipes/libiconv/
--rw-r--r--   0 runner    (1001) docker     (123)      810 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/libiconv/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.443468 python-for-android-2023.2.10/pythonforandroid/recipes/liblzma/
--rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/liblzma/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.443468 python-for-android-2023.2.10/pythonforandroid/recipes/libmysqlclient/
--rw-r--r--   0 runner    (1001) docker     (123)     2825 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/libmysqlclient/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/libmysqlclient/add-custom-platform.patch
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/libmysqlclient/disable-soname.patch
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/libmysqlclient/disable-soversion.patch
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.443468 python-for-android-2023.2.10/pythonforandroid/recipes/libogg/
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/libogg/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.443468 python-for-android-2023.2.10/pythonforandroid/recipes/libpcre/
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/libpcre/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.443468 python-for-android-2023.2.10/pythonforandroid/recipes/libpq/
--rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/libpq/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.443468 python-for-android-2023.2.10/pythonforandroid/recipes/librt/
--rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/librt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.447468 python-for-android-2023.2.10/pythonforandroid/recipes/libsecp256k1/
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/libsecp256k1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.447468 python-for-android-2023.2.10/pythonforandroid/recipes/libshine/
--rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/libshine/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.447468 python-for-android-2023.2.10/pythonforandroid/recipes/libsodium/
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/libsodium/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      488 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/libsodium/size_max_fix.patch
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.447468 python-for-android-2023.2.10/pythonforandroid/recipes/libtorrent/
--rw-r--r--   0 runner    (1001) docker     (123)     6157 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/libtorrent/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/libtorrent/disable-so-version.patch
--rw-r--r--   0 runner    (1001) docker     (123)      622 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/libtorrent/setup-lib-name.patch
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/libtorrent/use-soname-python.patch
--rw-r--r--   0 runner    (1001) docker     (123)      855 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/libtorrent/user-config-openssl.patch
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.447468 python-for-android-2023.2.10/pythonforandroid/recipes/libtribler/
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/libtribler/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.447468 python-for-android-2023.2.10/pythonforandroid/recipes/libvorbis/
--rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/libvorbis/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.447468 python-for-android-2023.2.10/pythonforandroid/recipes/libvpx/
--rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/libvpx/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.447468 python-for-android-2023.2.10/pythonforandroid/recipes/libvpx/patches/
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/libvpx/patches/0001-android-force-neon-runtime.patch
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.447468 python-for-android-2023.2.10/pythonforandroid/recipes/libwebp/
--rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/libwebp/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.447468 python-for-android-2023.2.10/pythonforandroid/recipes/libx264/
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/libx264/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.447468 python-for-android-2023.2.10/pythonforandroid/recipes/libxml2/
--rw-r--r--   0 runner    (1001) docker     (123)     1929 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/libxml2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27625 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/libxml2/add-glob.c.patch
--rw-r--r--   0 runner    (1001) docker     (123)    21774 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/libxml2/glob.c
--rw-r--r--   0 runner    (1001) docker     (123)     4248 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/libxml2/glob.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.447468 python-for-android-2023.2.10/pythonforandroid/recipes/libxslt/
--rw-r--r--   0 runner    (1001) docker     (123)     2520 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/libxslt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/libxslt/fix-dlopen.patch
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.447468 python-for-android-2023.2.10/pythonforandroid/recipes/libzbar/
--rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/libzbar/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/libzbar/werror.patch
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.447468 python-for-android-2023.2.10/pythonforandroid/recipes/libzmq/
--rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/libzmq/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.447468 python-for-android-2023.2.10/pythonforandroid/recipes/lxml/
--rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/lxml/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.447468 python-for-android-2023.2.10/pythonforandroid/recipes/m2crypto/
--rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/m2crypto/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.447468 python-for-android-2023.2.10/pythonforandroid/recipes/matplotlib/
--rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/matplotlib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.447468 python-for-android-2023.2.10/pythonforandroid/recipes/msgpack-python/
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/msgpack-python/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.447468 python-for-android-2023.2.10/pythonforandroid/recipes/mysqldb/
--rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/mysqldb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/mysqldb/disable-zip.patch
--rw-r--r--   0 runner    (1001) docker     (123)      633 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/mysqldb/override-mysql-config.patch
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.447468 python-for-android-2023.2.10/pythonforandroid/recipes/netifaces/
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/netifaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      549 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/netifaces/fix-build.patch
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.447468 python-for-android-2023.2.10/pythonforandroid/recipes/numpy/
--rw-r--r--   0 runner    (1001) docker     (123)     2797 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/numpy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.447468 python-for-android-2023.2.10/pythonforandroid/recipes/numpy/patches/
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/numpy/patches/add_libm_explicitly_to_build.patch
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/numpy/patches/ranlib.patch
--rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/numpy/patches/remove-default-paths.patch
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.447468 python-for-android-2023.2.10/pythonforandroid/recipes/omemo/
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/omemo/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.447468 python-for-android-2023.2.10/pythonforandroid/recipes/omemo-backend-signal/
--rw-r--r--   0 runner    (1001) docker     (123)      570 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/omemo-backend-signal/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.447468 python-for-android-2023.2.10/pythonforandroid/recipes/openal/
--rw-r--r--   0 runner    (1001) docker     (123)      961 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/openal/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.447468 python-for-android-2023.2.10/pythonforandroid/recipes/opencv/
--rw-r--r--   0 runner    (1001) docker     (123)     6694 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/opencv/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.451468 python-for-android-2023.2.10/pythonforandroid/recipes/opencv/patches/
--rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/opencv/patches/p4a_build.patch
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.451468 python-for-android-2023.2.10/pythonforandroid/recipes/opencv_extras/
--rw-r--r--   0 runner    (1001) docker     (123)      762 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/opencv_extras/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.451468 python-for-android-2023.2.10/pythonforandroid/recipes/openssl/
--rw-r--r--   0 runner    (1001) docker     (123)     5008 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/openssl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/openssl/disable-sover.patch
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.451468 python-for-android-2023.2.10/pythonforandroid/recipes/pandas/
--rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/pandas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/pandas/fix_numpy_includes.patch
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.451468 python-for-android-2023.2.10/pythonforandroid/recipes/pil/
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/pil/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.451468 python-for-android-2023.2.10/pythonforandroid/recipes/png/
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/png/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/png/build_shared_library.patch
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.451468 python-for-android-2023.2.10/pythonforandroid/recipes/preppy/
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/preppy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/preppy/fix-setup.patch
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.451468 python-for-android-2023.2.10/pythonforandroid/recipes/protobuf_cpp/
--rw-r--r--   0 runner    (1001) docker     (123)     6010 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/protobuf_cpp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4155 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/protobuf_cpp/fix-python3-compatibility.patch
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.451468 python-for-android-2023.2.10/pythonforandroid/recipes/psycopg2/
--rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/psycopg2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.451468 python-for-android-2023.2.10/pythonforandroid/recipes/py3dns/
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/py3dns/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.451468 python-for-android-2023.2.10/pythonforandroid/recipes/py3dns/patches/
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/py3dns/patches/android.patch
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.451468 python-for-android-2023.2.10/pythonforandroid/recipes/pyaml/
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/pyaml/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.451468 python-for-android-2023.2.10/pythonforandroid/recipes/pybind11/
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/pybind11/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.451468 python-for-android-2023.2.10/pythonforandroid/recipes/pycparser/
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/pycparser/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.451468 python-for-android-2023.2.10/pythonforandroid/recipes/pycrypto/
--rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/pycrypto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/pycrypto/add_length.patch
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.451468 python-for-android-2023.2.10/pythonforandroid/recipes/pycryptodome/
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/pycryptodome/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.451468 python-for-android-2023.2.10/pythonforandroid/recipes/pydantic/
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/pydantic/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.451468 python-for-android-2023.2.10/pythonforandroid/recipes/pygame/
--rw-r--r--   0 runner    (1001) docker     (123)     2729 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/pygame/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.451468 python-for-android-2023.2.10/pythonforandroid/recipes/pyicu/
--rw-r--r--   0 runner    (1001) docker     (123)      909 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/pyicu/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/pyicu/locale.patch
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.451468 python-for-android-2023.2.10/pythonforandroid/recipes/pyjnius/
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/pyjnius/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/pyjnius/genericndkbuild_jnienv_getter.patch
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.451468 python-for-android-2023.2.10/pythonforandroid/recipes/pyleveldb/
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/pyleveldb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/pyleveldb/bindings-only.patch
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.451468 python-for-android-2023.2.10/pythonforandroid/recipes/pymunk/
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/pymunk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.451468 python-for-android-2023.2.10/pythonforandroid/recipes/pynacl/
--rw-r--r--   0 runner    (1001) docker     (123)      990 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/pynacl/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.451468 python-for-android-2023.2.10/pythonforandroid/recipes/pyogg/
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/pyogg/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.451468 python-for-android-2023.2.10/pythonforandroid/recipes/pyogg/patches/
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/pyogg/patches/fix-find-lib.patch
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.451468 python-for-android-2023.2.10/pythonforandroid/recipes/pyopenal/
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/pyopenal/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.451468 python-for-android-2023.2.10/pythonforandroid/recipes/pyopenal/patches/
--rw-r--r--   0 runner    (1001) docker     (123)      633 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/pyopenal/patches/fix-find-lib.patch
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.451468 python-for-android-2023.2.10/pythonforandroid/recipes/pyopenssl/
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/pyopenssl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/pyopenssl/fix-dlfcn.patch
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.451468 python-for-android-2023.2.10/pythonforandroid/recipes/pyproj/
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/pyproj/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.455468 python-for-android-2023.2.10/pythonforandroid/recipes/pyrxp/
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/pyrxp/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.455468 python-for-android-2023.2.10/pythonforandroid/recipes/pysdl2/
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/pysdl2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.455468 python-for-android-2023.2.10/pythonforandroid/recipes/pysha3/
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/pysha3/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.455468 python-for-android-2023.2.10/pythonforandroid/recipes/python3/
--rw-r--r--   0 runner    (1001) docker     (123)    16612 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/python3/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.455468 python-for-android-2023.2.10/pythonforandroid/recipes/python3/patches/
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/python3/patches/py3.7.1_fix-ctypes-util-find-library.patch
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/python3/patches/py3.7.1_fix-zlib-version.patch
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/python3/patches/py3.7.1_fix_cortex_a8.patch
--rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/python3/patches/py3.8.1.patch
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/python3/patches/py3.8.1_fix_cortex_a8.patch
--rw-r--r--   0 runner    (1001) docker     (123)      636 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/python3/patches/pyconfig_detection.patch
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/python3/patches/reproducible-buildinfo.diff
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.455468 python-for-android-2023.2.10/pythonforandroid/recipes/pytz/
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/pytz/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.455468 python-for-android-2023.2.10/pythonforandroid/recipes/pyusb/
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/pyusb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/pyusb/fix-android.patch
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.455468 python-for-android-2023.2.10/pythonforandroid/recipes/pyzbar/
--rw-r--r--   0 runner    (1001) docker     (123)      862 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/pyzbar/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.455468 python-for-android-2023.2.10/pythonforandroid/recipes/pyzmq/
--rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/pyzmq/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.455468 python-for-android-2023.2.10/pythonforandroid/recipes/regex/
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/regex/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.455468 python-for-android-2023.2.10/pythonforandroid/recipes/reportlab/
--rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/reportlab/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.455468 python-for-android-2023.2.10/pythonforandroid/recipes/reportlab/patches/
--rw-r--r--   0 runner    (1001) docker     (123)     3066 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/reportlab/patches/fix-setup.patch
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.455468 python-for-android-2023.2.10/pythonforandroid/recipes/ruamel.yaml/
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/ruamel.yaml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/ruamel.yaml/disable-pip-req.patch
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.455468 python-for-android-2023.2.10/pythonforandroid/recipes/scipy/
--rw-r--r--   0 runner    (1001) docker     (123)     2995 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/scipy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.455468 python-for-android-2023.2.10/pythonforandroid/recipes/scrypt/
--rw-r--r--   0 runner    (1001) docker     (123)      957 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/scrypt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/scrypt/remove_librt.patch
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.455468 python-for-android-2023.2.10/pythonforandroid/recipes/sdl2/
--rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/sdl2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/sdl2/sdl-orientation-pr-6984.diff
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.455468 python-for-android-2023.2.10/pythonforandroid/recipes/sdl2_image/
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/sdl2_image/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/sdl2_image/enable-webp.patch
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.455468 python-for-android-2023.2.10/pythonforandroid/recipes/sdl2_mixer/
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/sdl2_mixer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.455468 python-for-android-2023.2.10/pythonforandroid/recipes/sdl2_ttf/
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/sdl2_ttf/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.455468 python-for-android-2023.2.10/pythonforandroid/recipes/secp256k1/
--rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/secp256k1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/secp256k1/cross_compile.patch
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/secp256k1/drop_setup_requires.patch
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/secp256k1/find_lib.patch
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/secp256k1/no-download.patch
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/secp256k1/pkg-config.patch
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.455468 python-for-android-2023.2.10/pythonforandroid/recipes/setuptools/
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/setuptools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.455468 python-for-android-2023.2.10/pythonforandroid/recipes/shapely/
--rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/shapely/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2085 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/shapely/setup.patch
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.455468 python-for-android-2023.2.10/pythonforandroid/recipes/six/
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/six/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.455468 python-for-android-2023.2.10/pythonforandroid/recipes/snappy/
--rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/snappy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.459468 python-for-android-2023.2.10/pythonforandroid/recipes/spine/
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/spine/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.459468 python-for-android-2023.2.10/pythonforandroid/recipes/sqlalchemy/
--rw-r--r--   0 runner    (1001) docker     (123)      402 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/sqlalchemy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/sqlalchemy/zipsafe.patch
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.459468 python-for-android-2023.2.10/pythonforandroid/recipes/sqlite3/
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/sqlite3/Android.mk
--rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/sqlite3/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.459468 python-for-android-2023.2.10/pythonforandroid/recipes/storm/
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/storm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.459468 python-for-android-2023.2.10/pythonforandroid/recipes/sympy/
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/sympy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/sympy/fix_android_detection.patch
--rw-r--r--   0 runner    (1001) docker     (123)     9143 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/sympy/fix_pretty_print.patch
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/sympy/fix_timeutils.patch
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.459468 python-for-android-2023.2.10/pythonforandroid/recipes/tflite-runtime/
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/tflite-runtime/CMakeLists.patch
--rw-r--r--   0 runner    (1001) docker     (123)     4358 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/tflite-runtime/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/tflite-runtime/build_with_cmake.patch
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.459468 python-for-android-2023.2.10/pythonforandroid/recipes/twisted/
--rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/twisted/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/twisted/incremental.patch
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/twisted/remove_tests.patch
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.459468 python-for-android-2023.2.10/pythonforandroid/recipes/ujson/
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/ujson/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.459468 python-for-android-2023.2.10/pythonforandroid/recipes/vispy/
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/vispy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/vispy/disable_font_triage.patch
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/vispy/disable_freetype.patch
--rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/vispy/remove_ati_check.patch
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/vispy/use_es2.patch
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.459468 python-for-android-2023.2.10/pythonforandroid/recipes/vlc/
--rw-r--r--   0 runner    (1001) docker     (123)     3179 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/vlc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.459468 python-for-android-2023.2.10/pythonforandroid/recipes/wsaccel/
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/wsaccel/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.459468 python-for-android-2023.2.10/pythonforandroid/recipes/x3dh/
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/x3dh/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/x3dh/requires_fix.patch
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.459468 python-for-android-2023.2.10/pythonforandroid/recipes/xeddsa/
--rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/xeddsa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/xeddsa/remove_dependencies.patch
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.459468 python-for-android-2023.2.10/pythonforandroid/recipes/zbar/
--rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/zbar/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/zbar/zbar-0.10-python-crash.patch
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.459468 python-for-android-2023.2.10/pythonforandroid/recipes/zbarlight/
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/zbarlight/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.459468 python-for-android-2023.2.10/pythonforandroid/recipes/zeroconf/
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/zeroconf/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.459468 python-for-android-2023.2.10/pythonforandroid/recipes/zeroconf/patches/
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/zeroconf/patches/setup.patch
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.459468 python-for-android-2023.2.10/pythonforandroid/recipes/zope/
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/zope/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.459468 python-for-android-2023.2.10/pythonforandroid/recipes/zope_interface/
--rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/zope_interface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/zope_interface/fix-init.patch
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recipes/zope_interface/no_tests.patch
--rw-r--r--   0 runner    (1001) docker     (123)     8374 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/recommendations.py
--rw-r--r--   0 runner    (1001) docker     (123)    54271 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/toolchain.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.463468 python-for-android-2023.2.10/pythonforandroid/tools/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1016 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/tools/biglink
--rwxr-xr-x   0 runner    (1001) docker     (123)     1906 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/tools/liblink
--rwxr-xr-x   0 runner    (1001) docker     (123)       56 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/tools/liblink.sh
--rw-r--r--   0 runner    (1001) docker     (123)     3557 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/pythonforandroid/util.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-11 09:23:29.463468 python-for-android-2023.2.10/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4758 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 09:23:29.463468 python-for-android-2023.2.10/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4785 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/tests/test_androidmodule_ctypes_finder.py
--rw-r--r--   0 runner    (1001) docker     (123)     5516 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/tests/test_androidndk.py
--rw-r--r--   0 runner    (1001) docker     (123)    13122 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/tests/test_archs.py
--rw-r--r--   0 runner    (1001) docker     (123)    25705 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/tests/test_bootstrap.py
--rw-r--r--   0 runner    (1001) docker     (123)     5129 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/tests/test_bootstrap_build.py
--rw-r--r--   0 runner    (1001) docker     (123)     5978 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/tests/test_build.py
--rw-r--r--   0 runner    (1001) docker     (123)    11340 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/tests/test_distribution.py
--rw-r--r--   0 runner    (1001) docker     (123)     8924 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/tests/test_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/tests/test_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    11906 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/tests/test_prerequisites.py
--rw-r--r--   0 runner    (1001) docker     (123)     3645 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/tests/test_pythonpackage.py
--rw-r--r--   0 runner    (1001) docker     (123)    12109 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/tests/test_pythonpackage_basic.py
--rw-r--r--   0 runner    (1001) docker     (123)    12007 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/tests/test_recipe.py
--rw-r--r--   0 runner    (1001) docker     (123)     9383 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/tests/test_recommendations.py
--rw-r--r--   0 runner    (1001) docker     (123)     6131 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/tests/test_toolchain.py
--rw-r--r--   0 runner    (1001) docker     (123)     5102 2023-02-11 09:23:21.000000 python-for-android-2023.2.10/tests/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.762779 python-for-android-2023.5.21/
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/.deepsource.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8172 2023-05-22 17:28:07.762779 python-for-android-2023.5.21/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7084 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.646778 python-for-android-2023.5.21/ci/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/ci/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1453 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/ci/constants.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3810 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/ci/rebuild_updated_recipes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.646778 python-for-android-2023.5.21/doc/
+-rw-r--r--   0 runner    (1001) docker     (123)     7467 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/doc/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     7281 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/doc/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.650778 python-for-android-2023.5.21/doc/source/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.650778 python-for-android-2023.5.21/doc/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/doc/source/_static/.empty
+-rw-r--r--   0 runner    (1001) docker     (123)    15750 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/doc/source/apis.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/doc/source/bootstraps.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11026 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/doc/source/buildoptions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2933 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/doc/source/commands.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9692 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/doc/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10465 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/doc/source/contribute.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4883 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/doc/source/distutils.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/doc/source/docker.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.606778 python-for-android-2023.5.21/doc/source/ext/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.654778 python-for-android-2023.5.21/doc/source/ext/sphinx_rtd_theme/
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/doc/source/ext/sphinx_rtd_theme/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/doc/source/ext/sphinx_rtd_theme/Gemfile
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/doc/source/ext/sphinx_rtd_theme/Gemfile.lock
+-rw-r--r--   0 runner    (1001) docker     (123)     2948 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/doc/source/ext/sphinx_rtd_theme/Gruntfile.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/doc/source/ext/sphinx_rtd_theme/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/doc/source/ext/sphinx_rtd_theme/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6150 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/doc/source/ext/sphinx_rtd_theme/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/doc/source/ext/sphinx_rtd_theme/bower.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.654778 python-for-android-2023.5.21/doc/source/ext/sphinx_rtd_theme/demo_docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     5621 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/doc/source/ext/sphinx_rtd_theme/demo_docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.654778 python-for-android-2023.5.21/doc/source/ext/sphinx_rtd_theme/demo_docs/source/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/doc/source/ext/sphinx_rtd_theme/demo_docs/source/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8213 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/doc/source/ext/sphinx_rtd_theme/demo_docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15469 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/doc/source/ext/sphinx_rtd_theme/demo_docs/source/demo.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7776 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/doc/source/ext/sphinx_rtd_theme/demo_docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/doc/source/ext/sphinx_rtd_theme/demo_docs/source/list.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.654778 python-for-android-2023.5.21/doc/source/ext/sphinx_rtd_theme/demo_docs/source/static/
+-rw-r--r--   0 runner    (1001) docker     (123)     9498 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/doc/source/ext/sphinx_rtd_theme/demo_docs/source/static/yi_jing_01_chien.jpg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.654778 python-for-android-2023.5.21/doc/source/ext/sphinx_rtd_theme/demo_docs/source/test_py_module/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/doc/source/ext/sphinx_rtd_theme/demo_docs/source/test_py_module/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2855 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/doc/source/ext/sphinx_rtd_theme/demo_docs/source/test_py_module/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/doc/source/ext/sphinx_rtd_theme/package.json
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/doc/source/ext/sphinx_rtd_theme/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.658778 python-for-android-2023.5.21/doc/source/ext/sphinx_rtd_theme/sass/
+-rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/doc/source/ext/sphinx_rtd_theme/sass/_theme_badge.sass
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/doc/source/ext/sphinx_rtd_theme/sass/_theme_badge_fa.sass
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/doc/source/ext/sphinx_rtd_theme/sass/_theme_breadcrumbs.sass
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/doc/source/ext/sphinx_rtd_theme/sass/_theme_font_awesome_compatability.sass
+-rw-r--r--   0 runner    (1001) docker     (123)     7473 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/doc/source/ext/sphinx_rtd_theme/sass/_theme_layout.sass
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/doc/source/ext/sphinx_rtd_theme/sass/_theme_mathjax.sass
+-rw-r--r--   0 runner    (1001) docker     (123)     9459 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/doc/source/ext/sphinx_rtd_theme/sass/_theme_rst.sass
+-rw-r--r--   0 runner    (1001) docker     (123)      875 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/doc/source/ext/sphinx_rtd_theme/sass/_theme_variables.sass
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/doc/source/ext/sphinx_rtd_theme/sass/badge_only.sass
+-rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/doc/source/ext/sphinx_rtd_theme/sass/theme.sass
+-rw-r--r--   0 runner    (1001) docker     (123)   156671 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/doc/source/ext/sphinx_rtd_theme/screen_desktop.png
+-rw-r--r--   0 runner    (1001) docker     (123)    96294 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/doc/source/ext/sphinx_rtd_theme/screen_mobile.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/doc/source/ext/sphinx_rtd_theme/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.662778 python-for-android-2023.5.21/doc/source/ext/sphinx_rtd_theme/sphinx_rtd_theme/
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/doc/source/ext/sphinx_rtd_theme/sphinx_rtd_theme/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/doc/source/ext/sphinx_rtd_theme/sphinx_rtd_theme/breadcrumbs.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/doc/source/ext/sphinx_rtd_theme/sphinx_rtd_theme/footer.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5355 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/doc/source/ext/sphinx_rtd_theme/sphinx_rtd_theme/layout.html
+-rw-r--r--   0 runner    (1001) docker     (123)     7341 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/doc/source/ext/sphinx_rtd_theme/sphinx_rtd_theme/layout_old.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/doc/source/ext/sphinx_rtd_theme/sphinx_rtd_theme/search.html
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/doc/source/ext/sphinx_rtd_theme/sphinx_rtd_theme/searchbox.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.606778 python-for-android-2023.5.21/doc/source/ext/sphinx_rtd_theme/sphinx_rtd_theme/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.662778 python-for-android-2023.5.21/doc/source/ext/sphinx_rtd_theme/sphinx_rtd_theme/static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     3403 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/doc/source/ext/sphinx_rtd_theme/sphinx_rtd_theme/static/css/badge_only.css
+-rw-r--r--   0 runner    (1001) docker     (123)    88728 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/doc/source/ext/sphinx_rtd_theme/sphinx_rtd_theme/static/css/theme.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.662778 python-for-android-2023.5.21/doc/source/ext/sphinx_rtd_theme/sphinx_rtd_theme/static/fonts/
+-rw-r--r--   0 runner    (1001) docker     (123)    62856 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/doc/source/ext/sphinx_rtd_theme/sphinx_rtd_theme/static/fonts/FontAwesome.otf
+-rw-r--r--   0 runner    (1001) docker     (123)    38205 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/doc/source/ext/sphinx_rtd_theme/sphinx_rtd_theme/static/fonts/fontawesome-webfont.eot
+-rw-r--r--   0 runner    (1001) docker     (123)   202148 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/doc/source/ext/sphinx_rtd_theme/sphinx_rtd_theme/static/fonts/fontawesome-webfont.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    80652 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/doc/source/ext/sphinx_rtd_theme/sphinx_rtd_theme/static/fonts/fontawesome-webfont.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    44432 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/doc/source/ext/sphinx_rtd_theme/sphinx_rtd_theme/static/fonts/fontawesome-webfont.woff
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.666778 python-for-android-2023.5.21/doc/source/ext/sphinx_rtd_theme/sphinx_rtd_theme/static/js/
+-rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/doc/source/ext/sphinx_rtd_theme/sphinx_rtd_theme/static/js/theme.js
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/doc/source/ext/sphinx_rtd_theme/sphinx_rtd_theme/theme.conf
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/doc/source/ext/sphinx_rtd_theme/sphinx_rtd_theme/versions.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/doc/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3236 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/doc/source/launcher.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    12827 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/doc/source/quickstart.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    18035 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/doc/source/recipes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5860 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/doc/source/services.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9371 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/doc/source/testing_pull_requests.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6723 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/doc/source/troubleshooting.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.666778 python-for-android-2023.5.21/python_for_android.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8172 2023-05-22 17:28:07.000000 python-for-android-2023.5.21/python_for_android.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    26787 2023-05-22 17:28:07.000000 python-for-android-2023.5.21/python_for_android.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 17:28:07.000000 python-for-android-2023.5.21/python_for_android.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-05-22 17:28:07.000000 python-for-android-2023.5.21/python_for_android.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-22 17:28:07.000000 python-for-android-2023.5.21/python_for_android.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-22 17:28:07.000000 python-for-android-2023.5.21/python_for_android.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.670778 python-for-android-2023.5.21/pythonforandroid/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/androidndk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9942 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/archs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6092 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/bdistapk.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    17302 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/bootstrap.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.670778 python-for-android-2023.5.21/pythonforandroid/bootstraps/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/bootstraps/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.606778 python-for-android-2023.5.21/pythonforandroid/bootstraps/common/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.674778 python-for-android-2023.5.21/pythonforandroid/bootstraps/common/build/
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/bootstraps/common/build/ant.properties
+-rw-r--r--   0 runner    (1001) docker     (123)    43045 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/bootstraps/common/build/build.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.606778 python-for-android-2023.5.21/pythonforandroid/bootstraps/common/build/gradle/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.674778 python-for-android-2023.5.21/pythonforandroid/bootstraps/common/build/gradle/wrapper/
+-rw-r--r--   0 runner    (1001) docker     (123)    51017 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/bootstraps/common/build/gradle/wrapper/gradle-wrapper.jar
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/bootstraps/common/build/gradle/wrapper/gradle-wrapper.properties
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5080 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/bootstraps/common/build/gradlew
+-rw-r--r--   0 runner    (1001) docker     (123)     2314 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/bootstraps/common/build/gradlew.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.674778 python-for-android-2023.5.21/pythonforandroid/bootstraps/common/build/jni/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/bootstraps/common/build/jni/Android.mk
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.674778 python-for-android-2023.5.21/pythonforandroid/bootstraps/common/build/jni/application/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/bootstraps/common/build/jni/application/Android.mk
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.674778 python-for-android-2023.5.21/pythonforandroid/bootstraps/common/build/jni/application/src/
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/bootstraps/common/build/jni/application/src/Android.mk
+-rw-r--r--   0 runner    (1001) docker     (123)    12877 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/bootstraps/common/build/jni/application/src/start.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.610778 python-for-android-2023.5.21/pythonforandroid/bootstraps/common/build/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.610778 python-for-android-2023.5.21/pythonforandroid/bootstraps/common/build/src/main/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.610778 python-for-android-2023.5.21/pythonforandroid/bootstraps/common/build/src/main/java/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.610778 python-for-android-2023.5.21/pythonforandroid/bootstraps/common/build/src/main/java/org/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.610778 python-for-android-2023.5.21/pythonforandroid/bootstraps/common/build/src/main/java/org/kamranzafar/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.678778 python-for-android-2023.5.21/pythonforandroid/bootstraps/common/build/src/main/java/org/kamranzafar/jtar/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4308 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/bootstraps/common/build/src/main/java/org/kamranzafar/jtar/Octal.java
+-rwxr-xr-x   0 runner    (1001) docker     (123)      881 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/bootstraps/common/build/src/main/java/org/kamranzafar/jtar/TarConstants.java
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7543 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/bootstraps/common/build/src/main/java/org/kamranzafar/jtar/TarEntry.java
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6536 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/bootstraps/common/build/src/main/java/org/kamranzafar/jtar/TarHeader.java
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5470 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/bootstraps/common/build/src/main/java/org/kamranzafar/jtar/TarInputStream.java
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4761 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/bootstraps/common/build/src/main/java/org/kamranzafar/jtar/TarOutputStream.java
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2179 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/bootstraps/common/build/src/main/java/org/kamranzafar/jtar/TarUtils.java
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.610778 python-for-android-2023.5.21/pythonforandroid/bootstraps/common/build/src/main/java/org/kivy/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.678778 python-for-android-2023.5.21/pythonforandroid/bootstraps/common/build/src/main/java/org/kivy/android/
+-rw-r--r--   0 runner    (1001) docker     (123)     7590 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/bootstraps/common/build/src/main/java/org/kivy/android/PythonService.java
+-rw-r--r--   0 runner    (1001) docker     (123)     8844 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/bootstraps/common/build/src/main/java/org/kivy/android/PythonUtil.java
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.610778 python-for-android-2023.5.21/pythonforandroid/bootstraps/common/build/src/main/java/org/renpy/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.678778 python-for-android-2023.5.21/pythonforandroid/bootstraps/common/build/src/main/java/org/renpy/android/
+-rw-r--r--   0 runner    (1001) docker     (123)     3174 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/bootstraps/common/build/src/main/java/org/renpy/android/AssetExtract.java
+-rw-r--r--   0 runner    (1001) docker     (123)     8874 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/bootstraps/common/build/src/main/java/org/renpy/android/Hardware.java
+-rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/bootstraps/common/build/src/main/java/org/renpy/android/ResourceManager.java
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.678778 python-for-android-2023.5.21/pythonforandroid/bootstraps/common/build/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/bootstraps/common/build/templates/Service.tmpl.java
+-rw-r--r--   0 runner    (1001) docker     (123)      881 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/bootstraps/common/build/templates/build.properties
+-rw-r--r--   0 runner    (1001) docker     (123)     3047 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/bootstraps/common/build/templates/build.tmpl.gradle
+-rw-r--r--   0 runner    (1001) docker     (123)     4034 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/bootstraps/common/build/templates/build.tmpl.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/bootstraps/common/build/templates/custom_rules.tmpl.xml
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/bootstraps/common/build/templates/gradle.tmpl.properties
+-rw-r--r--   0 runner    (1001) docker     (123)     3229 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/bootstraps/common/build/templates/kivy-icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)    11584 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/bootstraps/common/build/templates/kivy-presplash.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/bootstraps/common/build/templates/lottie.xml
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/bootstraps/common/build/whitelist.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.682778 python-for-android-2023.5.21/pythonforandroid/bootstraps/empty/
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/bootstraps/empty/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.682778 python-for-android-2023.5.21/pythonforandroid/bootstraps/empty/build/
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/bootstraps/empty/build/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.682778 python-for-android-2023.5.21/pythonforandroid/bootstraps/sdl2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/bootstraps/sdl2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.682778 python-for-android-2023.5.21/pythonforandroid/bootstraps/sdl2/build/
+-rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/bootstraps/sdl2/build/blacklist.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.682778 python-for-android-2023.5.21/pythonforandroid/bootstraps/sdl2/build/jni/
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/bootstraps/sdl2/build/jni/Application.mk
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.610778 python-for-android-2023.5.21/pythonforandroid/bootstraps/sdl2/build/jni/application/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.682778 python-for-android-2023.5.21/pythonforandroid/bootstraps/sdl2/build/jni/application/src/
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/bootstraps/sdl2/build/jni/application/src/Android_static.mk
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/bootstraps/sdl2/build/jni/application/src/bootstrap_name.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.614778 python-for-android-2023.5.21/pythonforandroid/bootstraps/sdl2/build/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.610778 python-for-android-2023.5.21/pythonforandroid/bootstraps/sdl2/build/src/main/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.682778 python-for-android-2023.5.21/pythonforandroid/bootstraps/sdl2/build/src/main/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/bootstraps/sdl2/build/src/main/assets/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.682778 python-for-android-2023.5.21/pythonforandroid/bootstraps/sdl2/build/src/main/java/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/bootstraps/sdl2/build/src/main/java/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.610778 python-for-android-2023.5.21/pythonforandroid/bootstraps/sdl2/build/src/main/java/org/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.610778 python-for-android-2023.5.21/pythonforandroid/bootstraps/sdl2/build/src/main/java/org/kivy/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.682778 python-for-android-2023.5.21/pythonforandroid/bootstraps/sdl2/build/src/main/java/org/kivy/android/
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/bootstraps/sdl2/build/src/main/java/org/kivy/android/GenericBroadcastReceiver.java
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/bootstraps/sdl2/build/src/main/java/org/kivy/android/GenericBroadcastReceiverCallback.java
+-rw-r--r--   0 runner    (1001) docker     (123)    24939 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/bootstraps/sdl2/build/src/main/java/org/kivy/android/PythonActivity.java
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.682778 python-for-android-2023.5.21/pythonforandroid/bootstraps/sdl2/build/src/main/java/org/kivy/android/launcher/
+-rw-r--r--   0 runner    (1001) docker     (123)     2824 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/bootstraps/sdl2/build/src/main/java/org/kivy/android/launcher/Project.java
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/bootstraps/sdl2/build/src/main/java/org/kivy/android/launcher/ProjectAdapter.java
+-rw-r--r--   0 runner    (1001) docker     (123)     2605 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/bootstraps/sdl2/build/src/main/java/org/kivy/android/launcher/ProjectChooser.java
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.682778 python-for-android-2023.5.21/pythonforandroid/bootstraps/sdl2/build/src/main/jniLibs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/bootstraps/sdl2/build/src/main/jniLibs/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.682778 python-for-android-2023.5.21/pythonforandroid/bootstraps/sdl2/build/src/main/libs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/bootstraps/sdl2/build/src/main/libs/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.614778 python-for-android-2023.5.21/pythonforandroid/bootstraps/sdl2/build/src/main/res/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.682778 python-for-android-2023.5.21/pythonforandroid/bootstraps/sdl2/build/src/main/res/drawable/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/bootstraps/sdl2/build/src/main/res/drawable/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.682778 python-for-android-2023.5.21/pythonforandroid/bootstraps/sdl2/build/src/main/res/drawable-hdpi/
+-rw-r--r--   0 runner    (1001) docker     (123)     2683 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/bootstraps/sdl2/build/src/main/res/drawable-hdpi/ic_launcher.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.686778 python-for-android-2023.5.21/pythonforandroid/bootstraps/sdl2/build/src/main/res/drawable-mdpi/
+-rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/bootstraps/sdl2/build/src/main/res/drawable-mdpi/ic_launcher.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.686778 python-for-android-2023.5.21/pythonforandroid/bootstraps/sdl2/build/src/main/res/drawable-xhdpi/
+-rw-r--r--   0 runner    (1001) docker     (123)     3872 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/bootstraps/sdl2/build/src/main/res/drawable-xhdpi/ic_launcher.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.686778 python-for-android-2023.5.21/pythonforandroid/bootstraps/sdl2/build/src/main/res/drawable-xxhdpi/
+-rw-r--r--   0 runner    (1001) docker     (123)     6874 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/bootstraps/sdl2/build/src/main/res/drawable-xxhdpi/ic_launcher.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.686778 python-for-android-2023.5.21/pythonforandroid/bootstraps/sdl2/build/src/main/res/layout/
+-rw-r--r--   0 runner    (1001) docker     (123)      956 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/bootstraps/sdl2/build/src/main/res/layout/chooser_item.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/bootstraps/sdl2/build/src/main/res/layout/main.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/bootstraps/sdl2/build/src/main/res/layout/project_chooser.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/bootstraps/sdl2/build/src/main/res/layout/project_empty.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.686778 python-for-android-2023.5.21/pythonforandroid/bootstraps/sdl2/build/src/main/res/mipmap/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/bootstraps/sdl2/build/src/main/res/mipmap/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.686778 python-for-android-2023.5.21/pythonforandroid/bootstraps/sdl2/build/src/main/res/mipmap-anydpi-v26/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/bootstraps/sdl2/build/src/main/res/mipmap-anydpi-v26/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.686778 python-for-android-2023.5.21/pythonforandroid/bootstraps/sdl2/build/src/patches/
+-rw-r--r--   0 runner    (1001) docker     (123)     3084 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/bootstraps/sdl2/build/src/patches/SDLActivity.java.patch
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.686778 python-for-android-2023.5.21/pythonforandroid/bootstraps/sdl2/build/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     6279 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/bootstraps/sdl2/build/templates/AndroidManifest.tmpl.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/bootstraps/sdl2/build/templates/strings.tmpl.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.686778 python-for-android-2023.5.21/pythonforandroid/bootstraps/service_library/
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/bootstraps/service_library/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.614778 python-for-android-2023.5.21/pythonforandroid/bootstraps/service_library/build/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.614778 python-for-android-2023.5.21/pythonforandroid/bootstraps/service_library/build/jni/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.614778 python-for-android-2023.5.21/pythonforandroid/bootstraps/service_library/build/jni/application/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.686778 python-for-android-2023.5.21/pythonforandroid/bootstraps/service_library/build/jni/application/src/
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/bootstraps/service_library/build/jni/application/src/bootstrap_name.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.614778 python-for-android-2023.5.21/pythonforandroid/bootstraps/service_library/build/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.614778 python-for-android-2023.5.21/pythonforandroid/bootstraps/service_library/build/src/main/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.614778 python-for-android-2023.5.21/pythonforandroid/bootstraps/service_library/build/src/main/java/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.614778 python-for-android-2023.5.21/pythonforandroid/bootstraps/service_library/build/src/main/java/org/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.614778 python-for-android-2023.5.21/pythonforandroid/bootstraps/service_library/build/src/main/java/org/kivy/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.690778 python-for-android-2023.5.21/pythonforandroid/bootstraps/service_library/build/src/main/java/org/kivy/android/
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/bootstraps/service_library/build/src/main/java/org/kivy/android/GenericBroadcastReceiver.java
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/bootstraps/service_library/build/src/main/java/org/kivy/android/GenericBroadcastReceiverCallback.java
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/bootstraps/service_library/build/src/main/java/org/kivy/android/PythonActivity.java
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.614778 python-for-android-2023.5.21/pythonforandroid/bootstraps/service_library/build/src/main/res/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.690778 python-for-android-2023.5.21/pythonforandroid/bootstraps/service_library/build/src/main/res/mipmap/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/bootstraps/service_library/build/src/main/res/mipmap/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.690778 python-for-android-2023.5.21/pythonforandroid/bootstraps/service_library/build/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/bootstraps/service_library/build/templates/AndroidManifest.tmpl.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     3596 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/bootstraps/service_library/build/templates/Service.tmpl.java
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.690778 python-for-android-2023.5.21/pythonforandroid/bootstraps/service_only/
+-rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/bootstraps/service_only/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.690778 python-for-android-2023.5.21/pythonforandroid/bootstraps/service_only/build/
+-rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/bootstraps/service_only/build/blacklist.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.690778 python-for-android-2023.5.21/pythonforandroid/bootstraps/service_only/build/jni/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/bootstraps/service_only/build/jni/Android.mk
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/bootstraps/service_only/build/jni/Application.mk
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.614778 python-for-android-2023.5.21/pythonforandroid/bootstraps/service_only/build/jni/application/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.690778 python-for-android-2023.5.21/pythonforandroid/bootstraps/service_only/build/jni/application/src/
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/bootstraps/service_only/build/jni/application/src/Android.mk
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/bootstraps/service_only/build/jni/application/src/Android_static.mk
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/bootstraps/service_only/build/jni/application/src/bootstrap_name.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3876 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/bootstraps/service_only/build/jni/application/src/pyjniusjni.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.614778 python-for-android-2023.5.21/pythonforandroid/bootstraps/service_only/build/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.618778 python-for-android-2023.5.21/pythonforandroid/bootstraps/service_only/build/src/main/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.690778 python-for-android-2023.5.21/pythonforandroid/bootstraps/service_only/build/src/main/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/bootstraps/service_only/build/src/main/assets/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.618778 python-for-android-2023.5.21/pythonforandroid/bootstraps/service_only/build/src/main/java/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.618778 python-for-android-2023.5.21/pythonforandroid/bootstraps/service_only/build/src/main/java/org/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.618778 python-for-android-2023.5.21/pythonforandroid/bootstraps/service_only/build/src/main/java/org/kivy/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.690778 python-for-android-2023.5.21/pythonforandroid/bootstraps/service_only/build/src/main/java/org/kivy/android/
+-rw-r--r--   0 runner    (1001) docker     (123)    12411 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/bootstraps/service_only/build/src/main/java/org/kivy/android/PythonActivity.java
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.690778 python-for-android-2023.5.21/pythonforandroid/bootstraps/service_only/build/src/main/jniLibs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/bootstraps/service_only/build/src/main/jniLibs/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.618778 python-for-android-2023.5.21/pythonforandroid/bootstraps/service_only/build/src/main/res/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.690778 python-for-android-2023.5.21/pythonforandroid/bootstraps/service_only/build/src/main/res/drawable/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/bootstraps/service_only/build/src/main/res/drawable/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.690778 python-for-android-2023.5.21/pythonforandroid/bootstraps/service_only/build/src/main/res/mipmap/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/bootstraps/service_only/build/src/main/res/mipmap/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.694778 python-for-android-2023.5.21/pythonforandroid/bootstraps/service_only/build/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     4357 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/bootstraps/service_only/build/templates/AndroidManifest.tmpl.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     3549 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/bootstraps/service_only/build/templates/Service.tmpl.java
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/bootstraps/service_only/build/templates/strings.tmpl.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.694778 python-for-android-2023.5.21/pythonforandroid/bootstraps/webview/
+-rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/bootstraps/webview/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.694778 python-for-android-2023.5.21/pythonforandroid/bootstraps/webview/build/
+-rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/bootstraps/webview/build/blacklist.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.694778 python-for-android-2023.5.21/pythonforandroid/bootstraps/webview/build/jni/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/bootstraps/webview/build/jni/Android.mk
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/bootstraps/webview/build/jni/Application.mk
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.618778 python-for-android-2023.5.21/pythonforandroid/bootstraps/webview/build/jni/application/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.694778 python-for-android-2023.5.21/pythonforandroid/bootstraps/webview/build/jni/application/src/
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/bootstraps/webview/build/jni/application/src/Android.mk
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/bootstraps/webview/build/jni/application/src/Android_static.mk
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/bootstraps/webview/build/jni/application/src/bootstrap_name.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3876 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/bootstraps/webview/build/jni/application/src/pyjniusjni.c
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/bootstraps/webview/build/proguard-project.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.618778 python-for-android-2023.5.21/pythonforandroid/bootstraps/webview/build/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.618778 python-for-android-2023.5.21/pythonforandroid/bootstraps/webview/build/src/main/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.694778 python-for-android-2023.5.21/pythonforandroid/bootstraps/webview/build/src/main/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/bootstraps/webview/build/src/main/assets/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.618778 python-for-android-2023.5.21/pythonforandroid/bootstraps/webview/build/src/main/java/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.618778 python-for-android-2023.5.21/pythonforandroid/bootstraps/webview/build/src/main/java/org/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.618778 python-for-android-2023.5.21/pythonforandroid/bootstraps/webview/build/src/main/java/org/kivy/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.694778 python-for-android-2023.5.21/pythonforandroid/bootstraps/webview/build/src/main/java/org/kivy/android/
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/bootstraps/webview/build/src/main/java/org/kivy/android/GenericBroadcastReceiver.java
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/bootstraps/webview/build/src/main/java/org/kivy/android/GenericBroadcastReceiverCallback.java
+-rw-r--r--   0 runner    (1001) docker     (123)    21735 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/bootstraps/webview/build/src/main/java/org/kivy/android/PythonActivity.java
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.694778 python-for-android-2023.5.21/pythonforandroid/bootstraps/webview/build/src/main/jniLibs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/bootstraps/webview/build/src/main/jniLibs/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.618778 python-for-android-2023.5.21/pythonforandroid/bootstraps/webview/build/src/main/res/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.694778 python-for-android-2023.5.21/pythonforandroid/bootstraps/webview/build/src/main/res/drawable/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/bootstraps/webview/build/src/main/res/drawable/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (123)    16525 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/bootstraps/webview/build/src/main/res/drawable/icon.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.698778 python-for-android-2023.5.21/pythonforandroid/bootstraps/webview/build/src/main/res/layout/
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/bootstraps/webview/build/src/main/res/layout/main.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.698778 python-for-android-2023.5.21/pythonforandroid/bootstraps/webview/build/src/main/res/mipmap/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/bootstraps/webview/build/src/main/res/mipmap/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.698778 python-for-android-2023.5.21/pythonforandroid/bootstraps/webview/build/src/main/res/mipmap-anydpi-v26/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/bootstraps/webview/build/src/main/res/mipmap-anydpi-v26/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.698778 python-for-android-2023.5.21/pythonforandroid/bootstraps/webview/build/src/main/res/values/
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/bootstraps/webview/build/src/main/res/values/strings.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.698778 python-for-android-2023.5.21/pythonforandroid/bootstraps/webview/build/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     5007 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/bootstraps/webview/build/templates/AndroidManifest.tmpl.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/bootstraps/webview/build/templates/WebViewLoader.tmpl.java
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/bootstraps/webview/build/templates/strings.tmpl.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.698778 python-for-android-2023.5.21/pythonforandroid/bootstraps/webview/build/templates/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     3992 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/bootstraps/webview/build/templates/test/build.tmpl.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     3992 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/bootstraps/webview/build/templates/test/build.xml.tmpl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.698778 python-for-android-2023.5.21/pythonforandroid/bootstraps/webview/build/webview_includes/
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/bootstraps/webview/build/webview_includes/_load.html
+-rw-r--r--   0 runner    (1001) docker     (123)    37883 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/build.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11066 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/distribution.py
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/entrypoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12437 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8350 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/patching.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13434 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/prerequisites.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30760 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/pythonpackage.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47248 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipe.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.698778 python-for-android-2023.5.21/pythonforandroid/recipes/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.698778 python-for-android-2023.5.21/pythonforandroid/recipes/Pillow/
+-rw-r--r--   0 runner    (1001) docker     (123)     3721 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/Pillow/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.698778 python-for-android-2023.5.21/pythonforandroid/recipes/Pillow/patches/
+-rw-r--r--   0 runner    (1001) docker     (123)     7980 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/Pillow/patches/fix-setup.patch
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.698778 python-for-android-2023.5.21/pythonforandroid/recipes/aiohttp/
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/aiohttp/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.698778 python-for-android-2023.5.21/pythonforandroid/recipes/android/
+-rw-r--r--   0 runner    (1001) docker     (123)     2970 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/android/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.698778 python-for-android-2023.5.21/pythonforandroid/recipes/android/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.702778 python-for-android-2023.5.21/pythonforandroid/recipes/android/src/android/
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/android/src/android/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9636 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/android/src/android/_android.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/android/src/android/_android_billing.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     3287 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/android/src/android/_android_billing_jni.c
+-rw-r--r--   0 runner    (1001) docker     (123)     6312 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/android/src/android/_android_jni.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2869 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/android/src/android/_android_sound.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     8244 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/android/src/android/_android_sound_jni.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/android/src/android/_ctypes_library_finder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8159 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/android/src/android/activity.py
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/android/src/android/billing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3125 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/android/src/android/broadcast.py
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/android/src/android/loadingscreen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6326 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/android/src/android/mixer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19697 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/android/src/android/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1627 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/android/src/android/runnable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4283 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/android/src/android/storage.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      822 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/android/src/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.702778 python-for-android-2023.5.21/pythonforandroid/recipes/apsw/
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/apsw/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.702778 python-for-android-2023.5.21/pythonforandroid/recipes/argon2-cffi/
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/argon2-cffi/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.702778 python-for-android-2023.5.21/pythonforandroid/recipes/atom/
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/atom/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.702778 python-for-android-2023.5.21/pythonforandroid/recipes/audiostream/
+-rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/audiostream/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.702778 python-for-android-2023.5.21/pythonforandroid/recipes/av/
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/av/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.706778 python-for-android-2023.5.21/pythonforandroid/recipes/av_codecs/
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/av_codecs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.706778 python-for-android-2023.5.21/pythonforandroid/recipes/babel/
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/babel/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.706778 python-for-android-2023.5.21/pythonforandroid/recipes/bcrypt/
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/bcrypt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.706778 python-for-android-2023.5.21/pythonforandroid/recipes/boost/
+-rw-r--r--   0 runner    (1001) docker     (123)     3504 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/boost/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/boost/disable-so-version.patch
+-rw-r--r--   0 runner    (1001) docker     (123)     3470 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/boost/fix-android-issues.patch
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/boost/use-android-libs.patch
+-rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/boost/user-config.jam
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.706778 python-for-android-2023.5.21/pythonforandroid/recipes/brokenrecipe/
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/brokenrecipe/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.706778 python-for-android-2023.5.21/pythonforandroid/recipes/cffi/
+-rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/cffi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/cffi/disable-pkg-config.patch
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.706778 python-for-android-2023.5.21/pythonforandroid/recipes/coverage/
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/coverage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/coverage/fallback-utf8.patch
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.706778 python-for-android-2023.5.21/pythonforandroid/recipes/cppy/
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/cppy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.706778 python-for-android-2023.5.21/pythonforandroid/recipes/cryptography/
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/cryptography/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.706778 python-for-android-2023.5.21/pythonforandroid/recipes/cymunk/
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/cymunk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.706778 python-for-android-2023.5.21/pythonforandroid/recipes/cython/
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/cython/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.706778 python-for-android-2023.5.21/pythonforandroid/recipes/dateutil/
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/dateutil/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.710779 python-for-android-2023.5.21/pythonforandroid/recipes/decorator/
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/decorator/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.710779 python-for-android-2023.5.21/pythonforandroid/recipes/enaml/
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/enaml/0001-Update-setup.py.patch
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/enaml/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.710779 python-for-android-2023.5.21/pythonforandroid/recipes/ethash/
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/ethash/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.710779 python-for-android-2023.5.21/pythonforandroid/recipes/evdev/
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/evdev/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/evdev/evcnt.patch
+-rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/evdev/evdev-permissions.patch
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/evdev/include-dir.patch
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/evdev/keycnt.patch
+-rw-r--r--   0 runner    (1001) docker     (123)    15834 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/evdev/remove-uinput.patch
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.710779 python-for-android-2023.5.21/pythonforandroid/recipes/feedparser/
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/feedparser/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.710779 python-for-android-2023.5.21/pythonforandroid/recipes/ffmpeg/
+-rw-r--r--   0 runner    (1001) docker     (123)     5522 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/ffmpeg/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.710779 python-for-android-2023.5.21/pythonforandroid/recipes/ffmpeg/patches/
+-rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/ffmpeg/patches/configure.patch
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.710779 python-for-android-2023.5.21/pythonforandroid/recipes/ffpyplayer/
+-rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/ffpyplayer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.710779 python-for-android-2023.5.21/pythonforandroid/recipes/ffpyplayer_codecs/
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/ffpyplayer_codecs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.710779 python-for-android-2023.5.21/pythonforandroid/recipes/flask/
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/flask/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.710779 python-for-android-2023.5.21/pythonforandroid/recipes/fontconfig/
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/fontconfig/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.714779 python-for-android-2023.5.21/pythonforandroid/recipes/freetype/
+-rw-r--r--   0 runner    (1001) docker     (123)     5455 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/freetype/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.714779 python-for-android-2023.5.21/pythonforandroid/recipes/freetype-py/
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/freetype-py/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/freetype-py/fall-back-to-distutils.patch
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.714779 python-for-android-2023.5.21/pythonforandroid/recipes/genericndkbuild/
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/genericndkbuild/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.714779 python-for-android-2023.5.21/pythonforandroid/recipes/gevent/
+-rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/gevent/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/gevent/cross_compiling.patch
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.714779 python-for-android-2023.5.21/pythonforandroid/recipes/greenlet/
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/greenlet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.714779 python-for-android-2023.5.21/pythonforandroid/recipes/groestlcoin_hash/
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/groestlcoin_hash/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.714779 python-for-android-2023.5.21/pythonforandroid/recipes/harfbuzz/
+-rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/harfbuzz/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.714779 python-for-android-2023.5.21/pythonforandroid/recipes/hostpython3/
+-rw-r--r--   0 runner    (1001) docker     (123)     5111 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/hostpython3/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.714779 python-for-android-2023.5.21/pythonforandroid/recipes/hostpython3/patches/
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/hostpython3/patches/pyconfig_detection.patch
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.714779 python-for-android-2023.5.21/pythonforandroid/recipes/icu/
+-rw-r--r--   0 runner    (1001) docker     (123)     4895 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/icu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2618 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/icu/disable-libs-version.patch
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.714779 python-for-android-2023.5.21/pythonforandroid/recipes/ifaddr/
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/ifaddr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/ifaddr/getifaddrs.patch
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.714779 python-for-android-2023.5.21/pythonforandroid/recipes/ifaddrs/
+-rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/ifaddrs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.714779 python-for-android-2023.5.21/pythonforandroid/recipes/jedi/
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/jedi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/jedi/fix_MergedNamesDict_get.patch
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.718778 python-for-android-2023.5.21/pythonforandroid/recipes/jpeg/
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/jpeg/Application.mk
+-rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/jpeg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/jpeg/build-static.patch
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/jpeg/remove-version.patch
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.718778 python-for-android-2023.5.21/pythonforandroid/recipes/kivy/
+-rw-r--r--   0 runner    (1001) docker     (123)     2921 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/kivy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/kivy/sdl-gl-swapwindow-nogil.patch
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.718778 python-for-android-2023.5.21/pythonforandroid/recipes/kivy3/
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/kivy3/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.718778 python-for-android-2023.5.21/pythonforandroid/recipes/kiwisolver/
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/kiwisolver/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.718778 python-for-android-2023.5.21/pythonforandroid/recipes/lapack/
+-rw-r--r--   0 runner    (1001) docker     (123)     3115 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/lapack/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.718778 python-for-android-2023.5.21/pythonforandroid/recipes/leveldb/
+-rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/leveldb/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.718778 python-for-android-2023.5.21/pythonforandroid/recipes/libbz2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1733 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/libbz2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/libbz2/lib_android.patch
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.718778 python-for-android-2023.5.21/pythonforandroid/recipes/libcurl/
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/libcurl/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.718778 python-for-android-2023.5.21/pythonforandroid/recipes/libexpat/
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/libexpat/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.718778 python-for-android-2023.5.21/pythonforandroid/recipes/libffi/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/libffi/Application.mk
+-rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/libffi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      901 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/libffi/disable-mips-check.patch
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/libffi/remove-version-info.patch
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.718778 python-for-android-2023.5.21/pythonforandroid/recipes/libgeos/
+-rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/libgeos/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.718778 python-for-android-2023.5.21/pythonforandroid/recipes/libglob/
+-rw-r--r--   0 runner    (1001) docker     (123)     2376 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/libglob/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27296 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/libglob/glob.patch
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.722779 python-for-android-2023.5.21/pythonforandroid/recipes/libiconv/
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/libiconv/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.722779 python-for-android-2023.5.21/pythonforandroid/recipes/liblzma/
+-rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/liblzma/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.722779 python-for-android-2023.5.21/pythonforandroid/recipes/libmysqlclient/
+-rw-r--r--   0 runner    (1001) docker     (123)     2825 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/libmysqlclient/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/libmysqlclient/add-custom-platform.patch
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/libmysqlclient/disable-soname.patch
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/libmysqlclient/disable-soversion.patch
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.722779 python-for-android-2023.5.21/pythonforandroid/recipes/libogg/
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/libogg/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.722779 python-for-android-2023.5.21/pythonforandroid/recipes/libpcre/
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/libpcre/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.722779 python-for-android-2023.5.21/pythonforandroid/recipes/libpq/
+-rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/libpq/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.722779 python-for-android-2023.5.21/pythonforandroid/recipes/librt/
+-rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/librt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.722779 python-for-android-2023.5.21/pythonforandroid/recipes/libsecp256k1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/libsecp256k1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.722779 python-for-android-2023.5.21/pythonforandroid/recipes/libshine/
+-rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/libshine/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.722779 python-for-android-2023.5.21/pythonforandroid/recipes/libsodium/
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/libsodium/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/libsodium/size_max_fix.patch
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.722779 python-for-android-2023.5.21/pythonforandroid/recipes/libtorrent/
+-rw-r--r--   0 runner    (1001) docker     (123)     6157 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/libtorrent/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/libtorrent/disable-so-version.patch
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/libtorrent/setup-lib-name.patch
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/libtorrent/use-soname-python.patch
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/libtorrent/user-config-openssl.patch
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.726779 python-for-android-2023.5.21/pythonforandroid/recipes/libtribler/
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/libtribler/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.726779 python-for-android-2023.5.21/pythonforandroid/recipes/libvorbis/
+-rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/libvorbis/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.726779 python-for-android-2023.5.21/pythonforandroid/recipes/libvpx/
+-rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/libvpx/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.726779 python-for-android-2023.5.21/pythonforandroid/recipes/libvpx/patches/
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/libvpx/patches/0001-android-force-neon-runtime.patch
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.726779 python-for-android-2023.5.21/pythonforandroid/recipes/libwebp/
+-rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/libwebp/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.726779 python-for-android-2023.5.21/pythonforandroid/recipes/libx264/
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/libx264/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.726779 python-for-android-2023.5.21/pythonforandroid/recipes/libxml2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1929 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/libxml2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27625 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/libxml2/add-glob.c.patch
+-rw-r--r--   0 runner    (1001) docker     (123)    21774 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/libxml2/glob.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4248 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/libxml2/glob.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.726779 python-for-android-2023.5.21/pythonforandroid/recipes/libxslt/
+-rw-r--r--   0 runner    (1001) docker     (123)     2520 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/libxslt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/libxslt/fix-dlopen.patch
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.726779 python-for-android-2023.5.21/pythonforandroid/recipes/libzbar/
+-rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/libzbar/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/libzbar/werror.patch
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.726779 python-for-android-2023.5.21/pythonforandroid/recipes/libzmq/
+-rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/libzmq/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.726779 python-for-android-2023.5.21/pythonforandroid/recipes/lxml/
+-rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/lxml/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.726779 python-for-android-2023.5.21/pythonforandroid/recipes/m2crypto/
+-rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/m2crypto/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.730779 python-for-android-2023.5.21/pythonforandroid/recipes/matplotlib/
+-rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/matplotlib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.730779 python-for-android-2023.5.21/pythonforandroid/recipes/msgpack-python/
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/msgpack-python/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.730779 python-for-android-2023.5.21/pythonforandroid/recipes/mysqldb/
+-rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/mysqldb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/mysqldb/disable-zip.patch
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/mysqldb/override-mysql-config.patch
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.730779 python-for-android-2023.5.21/pythonforandroid/recipes/netifaces/
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/netifaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/netifaces/fix-build.patch
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.730779 python-for-android-2023.5.21/pythonforandroid/recipes/numpy/
+-rw-r--r--   0 runner    (1001) docker     (123)     2797 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/numpy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.730779 python-for-android-2023.5.21/pythonforandroid/recipes/numpy/patches/
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/numpy/patches/add_libm_explicitly_to_build.patch
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/numpy/patches/ranlib.patch
+-rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/numpy/patches/remove-default-paths.patch
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.730779 python-for-android-2023.5.21/pythonforandroid/recipes/omemo/
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/omemo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.730779 python-for-android-2023.5.21/pythonforandroid/recipes/omemo-backend-signal/
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/omemo-backend-signal/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.730779 python-for-android-2023.5.21/pythonforandroid/recipes/openal/
+-rw-r--r--   0 runner    (1001) docker     (123)      961 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/openal/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.734779 python-for-android-2023.5.21/pythonforandroid/recipes/opencv/
+-rw-r--r--   0 runner    (1001) docker     (123)     6694 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/opencv/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.734779 python-for-android-2023.5.21/pythonforandroid/recipes/opencv/patches/
+-rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/opencv/patches/p4a_build.patch
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.734779 python-for-android-2023.5.21/pythonforandroid/recipes/opencv_extras/
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/opencv_extras/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.734779 python-for-android-2023.5.21/pythonforandroid/recipes/openssl/
+-rw-r--r--   0 runner    (1001) docker     (123)     5008 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/openssl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/openssl/disable-sover.patch
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.734779 python-for-android-2023.5.21/pythonforandroid/recipes/pandas/
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/pandas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/pandas/fix_numpy_includes.patch
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.734779 python-for-android-2023.5.21/pythonforandroid/recipes/pil/
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/pil/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.734779 python-for-android-2023.5.21/pythonforandroid/recipes/png/
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/png/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/png/build_shared_library.patch
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.734779 python-for-android-2023.5.21/pythonforandroid/recipes/preppy/
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/preppy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/preppy/fix-setup.patch
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.734779 python-for-android-2023.5.21/pythonforandroid/recipes/protobuf_cpp/
+-rw-r--r--   0 runner    (1001) docker     (123)     6010 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/protobuf_cpp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4155 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/protobuf_cpp/fix-python3-compatibility.patch
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.734779 python-for-android-2023.5.21/pythonforandroid/recipes/psycopg2/
+-rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/psycopg2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.734779 python-for-android-2023.5.21/pythonforandroid/recipes/py3dns/
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/py3dns/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.734779 python-for-android-2023.5.21/pythonforandroid/recipes/py3dns/patches/
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/py3dns/patches/android.patch
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.734779 python-for-android-2023.5.21/pythonforandroid/recipes/pyaml/
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/pyaml/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.734779 python-for-android-2023.5.21/pythonforandroid/recipes/pybind11/
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/pybind11/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.738779 python-for-android-2023.5.21/pythonforandroid/recipes/pycparser/
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/pycparser/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.738779 python-for-android-2023.5.21/pythonforandroid/recipes/pycrypto/
+-rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/pycrypto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/pycrypto/add_length.patch
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.738779 python-for-android-2023.5.21/pythonforandroid/recipes/pycryptodome/
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/pycryptodome/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.738779 python-for-android-2023.5.21/pythonforandroid/recipes/pydantic/
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/pydantic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.738779 python-for-android-2023.5.21/pythonforandroid/recipes/pygame/
+-rw-r--r--   0 runner    (1001) docker     (123)     2729 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/pygame/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.738779 python-for-android-2023.5.21/pythonforandroid/recipes/pyicu/
+-rw-r--r--   0 runner    (1001) docker     (123)      909 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/pyicu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/pyicu/locale.patch
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.738779 python-for-android-2023.5.21/pythonforandroid/recipes/pyjnius/
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/pyjnius/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/pyjnius/genericndkbuild_jnienv_getter.patch
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.738779 python-for-android-2023.5.21/pythonforandroid/recipes/pyleveldb/
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/pyleveldb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/pyleveldb/bindings-only.patch
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.738779 python-for-android-2023.5.21/pythonforandroid/recipes/pymunk/
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/pymunk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.738779 python-for-android-2023.5.21/pythonforandroid/recipes/pynacl/
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/pynacl/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.738779 python-for-android-2023.5.21/pythonforandroid/recipes/pyogg/
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/pyogg/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.738779 python-for-android-2023.5.21/pythonforandroid/recipes/pyogg/patches/
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/pyogg/patches/fix-find-lib.patch
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.738779 python-for-android-2023.5.21/pythonforandroid/recipes/pyopenal/
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/pyopenal/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.738779 python-for-android-2023.5.21/pythonforandroid/recipes/pyopenal/patches/
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/pyopenal/patches/fix-find-lib.patch
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.742779 python-for-android-2023.5.21/pythonforandroid/recipes/pyopenssl/
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/pyopenssl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/pyopenssl/fix-dlfcn.patch
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.742779 python-for-android-2023.5.21/pythonforandroid/recipes/pyproj/
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/pyproj/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.742779 python-for-android-2023.5.21/pythonforandroid/recipes/pyrxp/
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/pyrxp/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.742779 python-for-android-2023.5.21/pythonforandroid/recipes/pysdl2/
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/pysdl2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.742779 python-for-android-2023.5.21/pythonforandroid/recipes/pysha3/
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/pysha3/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.742779 python-for-android-2023.5.21/pythonforandroid/recipes/python3/
+-rw-r--r--   0 runner    (1001) docker     (123)    16801 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/python3/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.742779 python-for-android-2023.5.21/pythonforandroid/recipes/python3/patches/
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/python3/patches/py3.7.1_fix-ctypes-util-find-library.patch
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/python3/patches/py3.7.1_fix-zlib-version.patch
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/python3/patches/py3.7.1_fix_cortex_a8.patch
+-rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/python3/patches/py3.8.1.patch
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/python3/patches/py3.8.1_fix_cortex_a8.patch
+-rw-r--r--   0 runner    (1001) docker     (123)      636 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/python3/patches/pyconfig_detection.patch
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/python3/patches/reproducible-buildinfo.diff
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.742779 python-for-android-2023.5.21/pythonforandroid/recipes/pytz/
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/pytz/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.742779 python-for-android-2023.5.21/pythonforandroid/recipes/pyusb/
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/pyusb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/pyusb/fix-android.patch
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.742779 python-for-android-2023.5.21/pythonforandroid/recipes/pyzbar/
+-rw-r--r--   0 runner    (1001) docker     (123)      862 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/pyzbar/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.742779 python-for-android-2023.5.21/pythonforandroid/recipes/pyzmq/
+-rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/pyzmq/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.746779 python-for-android-2023.5.21/pythonforandroid/recipes/regex/
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/regex/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.746779 python-for-android-2023.5.21/pythonforandroid/recipes/reportlab/
+-rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/reportlab/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.746779 python-for-android-2023.5.21/pythonforandroid/recipes/reportlab/patches/
+-rw-r--r--   0 runner    (1001) docker     (123)     3066 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/reportlab/patches/fix-setup.patch
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.746779 python-for-android-2023.5.21/pythonforandroid/recipes/ruamel.yaml/
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/ruamel.yaml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/ruamel.yaml/disable-pip-req.patch
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.746779 python-for-android-2023.5.21/pythonforandroid/recipes/scipy/
+-rw-r--r--   0 runner    (1001) docker     (123)     2995 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/scipy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.746779 python-for-android-2023.5.21/pythonforandroid/recipes/scrypt/
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/scrypt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/scrypt/remove_librt.patch
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.746779 python-for-android-2023.5.21/pythonforandroid/recipes/sdl2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/sdl2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/sdl2/sdl-orientation-pr-6984.diff
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.746779 python-for-android-2023.5.21/pythonforandroid/recipes/sdl2_image/
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/sdl2_image/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/sdl2_image/enable-webp.patch
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.746779 python-for-android-2023.5.21/pythonforandroid/recipes/sdl2_mixer/
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/sdl2_mixer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.746779 python-for-android-2023.5.21/pythonforandroid/recipes/sdl2_ttf/
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/sdl2_ttf/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.746779 python-for-android-2023.5.21/pythonforandroid/recipes/secp256k1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/secp256k1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/secp256k1/cross_compile.patch
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/secp256k1/drop_setup_requires.patch
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/secp256k1/find_lib.patch
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/secp256k1/no-download.patch
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/secp256k1/pkg-config.patch
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.750779 python-for-android-2023.5.21/pythonforandroid/recipes/setuptools/
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/setuptools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.750779 python-for-android-2023.5.21/pythonforandroid/recipes/shapely/
+-rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/shapely/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2085 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/shapely/setup.patch
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.750779 python-for-android-2023.5.21/pythonforandroid/recipes/six/
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/six/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.750779 python-for-android-2023.5.21/pythonforandroid/recipes/snappy/
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/snappy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.750779 python-for-android-2023.5.21/pythonforandroid/recipes/spine/
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/spine/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.750779 python-for-android-2023.5.21/pythonforandroid/recipes/sqlalchemy/
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/sqlalchemy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/sqlalchemy/zipsafe.patch
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.750779 python-for-android-2023.5.21/pythonforandroid/recipes/sqlite3/
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/sqlite3/Android.mk
+-rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/sqlite3/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.750779 python-for-android-2023.5.21/pythonforandroid/recipes/storm/
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/storm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.750779 python-for-android-2023.5.21/pythonforandroid/recipes/sympy/
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/sympy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/sympy/fix_android_detection.patch
+-rw-r--r--   0 runner    (1001) docker     (123)     9143 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/sympy/fix_pretty_print.patch
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/sympy/fix_timeutils.patch
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.750779 python-for-android-2023.5.21/pythonforandroid/recipes/tflite-runtime/
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/tflite-runtime/CMakeLists.patch
+-rw-r--r--   0 runner    (1001) docker     (123)     4358 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/tflite-runtime/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/tflite-runtime/build_with_cmake.patch
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.754779 python-for-android-2023.5.21/pythonforandroid/recipes/twisted/
+-rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/twisted/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/twisted/incremental.patch
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/twisted/remove_tests.patch
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.754779 python-for-android-2023.5.21/pythonforandroid/recipes/ujson/
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/ujson/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.754779 python-for-android-2023.5.21/pythonforandroid/recipes/vispy/
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/vispy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/vispy/disable_font_triage.patch
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/vispy/disable_freetype.patch
+-rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/vispy/remove_ati_check.patch
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/vispy/use_es2.patch
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.754779 python-for-android-2023.5.21/pythonforandroid/recipes/vlc/
+-rw-r--r--   0 runner    (1001) docker     (123)     3179 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/vlc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.754779 python-for-android-2023.5.21/pythonforandroid/recipes/wsaccel/
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/wsaccel/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.754779 python-for-android-2023.5.21/pythonforandroid/recipes/x3dh/
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/x3dh/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/x3dh/requires_fix.patch
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.754779 python-for-android-2023.5.21/pythonforandroid/recipes/xeddsa/
+-rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/xeddsa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/xeddsa/remove_dependencies.patch
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.754779 python-for-android-2023.5.21/pythonforandroid/recipes/zbar/
+-rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/zbar/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/zbar/zbar-0.10-python-crash.patch
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.754779 python-for-android-2023.5.21/pythonforandroid/recipes/zbarlight/
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/zbarlight/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.754779 python-for-android-2023.5.21/pythonforandroid/recipes/zeroconf/
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/zeroconf/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.754779 python-for-android-2023.5.21/pythonforandroid/recipes/zeroconf/patches/
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/zeroconf/patches/setup.patch
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.758779 python-for-android-2023.5.21/pythonforandroid/recipes/zope/
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/zope/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.758779 python-for-android-2023.5.21/pythonforandroid/recipes/zope_interface/
+-rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/zope_interface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/zope_interface/fix-init.patch
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recipes/zope_interface/no_tests.patch
+-rw-r--r--   0 runner    (1001) docker     (123)     8374 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/recommendations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54271 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/toolchain.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.758779 python-for-android-2023.5.21/pythonforandroid/tools/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1016 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/tools/biglink
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1923 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/tools/liblink
+-rwxr-xr-x   0 runner    (1001) docker     (123)       56 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/tools/liblink.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     3557 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/pythonforandroid/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 17:28:07.762779 python-for-android-2023.5.21/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4758 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:07.762779 python-for-android-2023.5.21/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4785 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/tests/test_androidmodule_ctypes_finder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5516 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/tests/test_androidndk.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13122 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/tests/test_archs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25705 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/tests/test_bootstrap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5129 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/tests/test_bootstrap_build.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5978 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/tests/test_build.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11340 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/tests/test_distribution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8924 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/tests/test_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/tests/test_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11906 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/tests/test_prerequisites.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3645 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/tests/test_pythonpackage.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12109 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/tests/test_pythonpackage_basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12007 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/tests/test_recipe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9383 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/tests/test_recommendations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6131 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/tests/test_toolchain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5102 2023-05-22 17:27:57.000000 python-for-android-2023.5.21/tests/test_util.py
```

### Comparing `python-for-android-2023.2.10/LICENSE` & `python-for-android-2023.5.21/LICENSE`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/PKG-INFO` & `python-for-android-2023.5.21/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-for-android
-Version: 2023.2.10
+Version: 2023.5.21
 Summary: Android APK packager for Python scripts and apps
 Home-page: https://github.com/kivy/python-for-android
 Author: The Kivy team
 Author-email: kivy-dev@googlegroups.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `python-for-android-2023.2.10/README.md` & `python-for-android-2023.5.21/README.md`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/ci/constants.py` & `python-for-android-2023.5.21/ci/constants.py`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/ci/rebuild_updated_recipes.py` & `python-for-android-2023.5.21/ci/rebuild_updated_recipes.py`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/doc/Makefile` & `python-for-android-2023.5.21/doc/Makefile`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/doc/make.bat` & `python-for-android-2023.5.21/doc/make.bat`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/doc/source/apis.rst` & `python-for-android-2023.5.21/doc/source/apis.rst`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/doc/source/bootstraps.rst` & `python-for-android-2023.5.21/doc/source/bootstraps.rst`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/doc/source/buildoptions.rst` & `python-for-android-2023.5.21/doc/source/buildoptions.rst`

 * *Files 0% similar despite different names*

```diff
@@ -67,14 +67,15 @@
   attribute of the activity in the ``AndroidManifest.xml`` file. If not set, the value 
   will be synthesized from the ``--orientation`` option.
   The full list of valid options is given under ``android:screenOrientation``
   in the `Android documentation <https://developer.android.com/guide/topics/manifest/activity-element.html>`__.
 - ``--icon``: A path to the png file to use as the application icon.
 - ``--permission``: A permission that needs to be declared into the App ``AndroidManifest.xml``.
   For multiple permissions, add multiple ``--permission`` arguments.
+  ``--home-app`` Gives you the option to set your application as a home app (launcher) on your Android device.
 
   .. Note ::
     ``--permission`` accepts the following syntaxes: 
     ``--permission (name=android.permission.WRITE_EXTERNAL_STORAGE;maxSdkVersion=18)``
     or ``--permission android.permission.WRITE_EXTERNAL_STORAGE``.
 
     The first syntax is used to set additional properties to the permission
```

### Comparing `python-for-android-2023.2.10/doc/source/commands.rst` & `python-for-android-2023.5.21/doc/source/commands.rst`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/doc/source/conf.py` & `python-for-android-2023.5.21/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/doc/source/contribute.rst` & `python-for-android-2023.5.21/doc/source/contribute.rst`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/doc/source/distutils.rst` & `python-for-android-2023.5.21/doc/source/distutils.rst`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/doc/source/docker.rst` & `python-for-android-2023.5.21/doc/source/docker.rst`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/doc/source/ext/sphinx_rtd_theme/Gruntfile.js` & `python-for-android-2023.5.21/doc/source/ext/sphinx_rtd_theme/Gruntfile.js`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/doc/source/ext/sphinx_rtd_theme/LICENSE` & `python-for-android-2023.5.21/doc/source/ext/sphinx_rtd_theme/LICENSE`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/doc/source/ext/sphinx_rtd_theme/README.rst` & `python-for-android-2023.5.21/doc/source/ext/sphinx_rtd_theme/README.rst`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/doc/source/ext/sphinx_rtd_theme/bower.json` & `python-for-android-2023.5.21/doc/source/ext/sphinx_rtd_theme/bower.json`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/doc/source/ext/sphinx_rtd_theme/demo_docs/Makefile` & `python-for-android-2023.5.21/doc/source/ext/sphinx_rtd_theme/demo_docs/Makefile`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/doc/source/ext/sphinx_rtd_theme/demo_docs/source/conf.py` & `python-for-android-2023.5.21/doc/source/ext/sphinx_rtd_theme/demo_docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/doc/source/ext/sphinx_rtd_theme/demo_docs/source/demo.rst` & `python-for-android-2023.5.21/doc/source/ext/sphinx_rtd_theme/demo_docs/source/demo.rst`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/doc/source/ext/sphinx_rtd_theme/demo_docs/source/index.rst` & `python-for-android-2023.5.21/doc/source/ext/sphinx_rtd_theme/demo_docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/doc/source/ext/sphinx_rtd_theme/demo_docs/source/list.rst` & `python-for-android-2023.5.21/doc/source/ext/sphinx_rtd_theme/demo_docs/source/list.rst`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/doc/source/ext/sphinx_rtd_theme/demo_docs/source/static/yi_jing_01_chien.jpg` & `python-for-android-2023.5.21/doc/source/ext/sphinx_rtd_theme/demo_docs/source/static/yi_jing_01_chien.jpg`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/doc/source/ext/sphinx_rtd_theme/demo_docs/source/test_py_module/test.py` & `python-for-android-2023.5.21/doc/source/ext/sphinx_rtd_theme/demo_docs/source/test_py_module/test.py`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/doc/source/ext/sphinx_rtd_theme/sass/_theme_badge.sass` & `python-for-android-2023.5.21/doc/source/ext/sphinx_rtd_theme/sass/_theme_badge.sass`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/doc/source/ext/sphinx_rtd_theme/sass/_theme_badge_fa.sass` & `python-for-android-2023.5.21/doc/source/ext/sphinx_rtd_theme/sass/_theme_badge_fa.sass`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/doc/source/ext/sphinx_rtd_theme/sass/_theme_layout.sass` & `python-for-android-2023.5.21/doc/source/ext/sphinx_rtd_theme/sass/_theme_layout.sass`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/doc/source/ext/sphinx_rtd_theme/sass/_theme_rst.sass` & `python-for-android-2023.5.21/doc/source/ext/sphinx_rtd_theme/sass/_theme_rst.sass`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/doc/source/ext/sphinx_rtd_theme/sass/_theme_variables.sass` & `python-for-android-2023.5.21/doc/source/ext/sphinx_rtd_theme/sass/_theme_variables.sass`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/doc/source/ext/sphinx_rtd_theme/sass/badge_only.sass` & `python-for-android-2023.5.21/doc/source/ext/sphinx_rtd_theme/sass/badge_only.sass`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/doc/source/ext/sphinx_rtd_theme/sass/theme.sass` & `python-for-android-2023.5.21/doc/source/ext/sphinx_rtd_theme/sass/theme.sass`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/doc/source/ext/sphinx_rtd_theme/screen_desktop.png` & `python-for-android-2023.5.21/doc/source/ext/sphinx_rtd_theme/screen_desktop.png`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/doc/source/ext/sphinx_rtd_theme/screen_mobile.png` & `python-for-android-2023.5.21/doc/source/ext/sphinx_rtd_theme/screen_mobile.png`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/doc/source/ext/sphinx_rtd_theme/setup.py` & `python-for-android-2023.5.21/doc/source/ext/sphinx_rtd_theme/setup.py`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/doc/source/ext/sphinx_rtd_theme/sphinx_rtd_theme/breadcrumbs.html` & `python-for-android-2023.5.21/doc/source/ext/sphinx_rtd_theme/sphinx_rtd_theme/breadcrumbs.html`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/doc/source/ext/sphinx_rtd_theme/sphinx_rtd_theme/footer.html` & `python-for-android-2023.5.21/doc/source/ext/sphinx_rtd_theme/sphinx_rtd_theme/footer.html`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/doc/source/ext/sphinx_rtd_theme/sphinx_rtd_theme/layout.html` & `python-for-android-2023.5.21/doc/source/ext/sphinx_rtd_theme/sphinx_rtd_theme/layout.html`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/doc/source/ext/sphinx_rtd_theme/sphinx_rtd_theme/layout_old.html` & `python-for-android-2023.5.21/doc/source/ext/sphinx_rtd_theme/sphinx_rtd_theme/layout_old.html`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/doc/source/ext/sphinx_rtd_theme/sphinx_rtd_theme/search.html` & `python-for-android-2023.5.21/doc/source/ext/sphinx_rtd_theme/sphinx_rtd_theme/search.html`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/doc/source/ext/sphinx_rtd_theme/sphinx_rtd_theme/static/css/badge_only.css` & `python-for-android-2023.5.21/doc/source/ext/sphinx_rtd_theme/sphinx_rtd_theme/static/css/badge_only.css`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/doc/source/ext/sphinx_rtd_theme/sphinx_rtd_theme/static/css/theme.css` & `python-for-android-2023.5.21/doc/source/ext/sphinx_rtd_theme/sphinx_rtd_theme/static/css/theme.css`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/doc/source/ext/sphinx_rtd_theme/sphinx_rtd_theme/static/fonts/FontAwesome.otf` & `python-for-android-2023.5.21/doc/source/ext/sphinx_rtd_theme/sphinx_rtd_theme/static/fonts/FontAwesome.otf`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/doc/source/ext/sphinx_rtd_theme/sphinx_rtd_theme/static/fonts/fontawesome-webfont.eot` & `python-for-android-2023.5.21/doc/source/ext/sphinx_rtd_theme/sphinx_rtd_theme/static/fonts/fontawesome-webfont.eot`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/doc/source/ext/sphinx_rtd_theme/sphinx_rtd_theme/static/fonts/fontawesome-webfont.svg` & `python-for-android-2023.5.21/doc/source/ext/sphinx_rtd_theme/sphinx_rtd_theme/static/fonts/fontawesome-webfont.svg`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/doc/source/ext/sphinx_rtd_theme/sphinx_rtd_theme/static/fonts/fontawesome-webfont.ttf` & `python-for-android-2023.5.21/doc/source/ext/sphinx_rtd_theme/sphinx_rtd_theme/static/fonts/fontawesome-webfont.ttf`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/doc/source/ext/sphinx_rtd_theme/sphinx_rtd_theme/static/fonts/fontawesome-webfont.woff` & `python-for-android-2023.5.21/doc/source/ext/sphinx_rtd_theme/sphinx_rtd_theme/static/fonts/fontawesome-webfont.woff`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/doc/source/ext/sphinx_rtd_theme/sphinx_rtd_theme/static/js/theme.js` & `python-for-android-2023.5.21/doc/source/ext/sphinx_rtd_theme/sphinx_rtd_theme/static/js/theme.js`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/doc/source/ext/sphinx_rtd_theme/sphinx_rtd_theme/versions.html` & `python-for-android-2023.5.21/doc/source/ext/sphinx_rtd_theme/sphinx_rtd_theme/versions.html`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/doc/source/index.rst` & `python-for-android-2023.5.21/doc/source/index.rst`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/doc/source/launcher.rst` & `python-for-android-2023.5.21/doc/source/launcher.rst`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/doc/source/quickstart.rst` & `python-for-android-2023.5.21/doc/source/quickstart.rst`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/doc/source/recipes.rst` & `python-for-android-2023.5.21/doc/source/recipes.rst`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/doc/source/services.rst` & `python-for-android-2023.5.21/doc/source/services.rst`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/doc/source/testing_pull_requests.rst` & `python-for-android-2023.5.21/doc/source/testing_pull_requests.rst`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/doc/source/troubleshooting.rst` & `python-for-android-2023.5.21/doc/source/troubleshooting.rst`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/python_for_android.egg-info/PKG-INFO` & `python-for-android-2023.5.21/python_for_android.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-for-android
-Version: 2023.2.10
+Version: 2023.5.21
 Summary: Android APK packager for Python scripts and apps
 Home-page: https://github.com/kivy/python-for-android
 Author: The Kivy team
 Author-email: kivy-dev@googlegroups.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `python-for-android-2023.2.10/python_for_android.egg-info/SOURCES.txt` & `python-for-android-2023.5.21/python_for_android.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -232,14 +232,16 @@
 pythonforandroid/recipes/android/src/android/permissions.py
 pythonforandroid/recipes/android/src/android/runnable.py
 pythonforandroid/recipes/android/src/android/storage.py
 pythonforandroid/recipes/apsw/__init__.py
 pythonforandroid/recipes/argon2-cffi/__init__.py
 pythonforandroid/recipes/atom/__init__.py
 pythonforandroid/recipes/audiostream/__init__.py
+pythonforandroid/recipes/av/__init__.py
+pythonforandroid/recipes/av_codecs/__init__.py
 pythonforandroid/recipes/babel/__init__.py
 pythonforandroid/recipes/bcrypt/__init__.py
 pythonforandroid/recipes/boost/__init__.py
 pythonforandroid/recipes/boost/disable-so-version.patch
 pythonforandroid/recipes/boost/fix-android-issues.patch
 pythonforandroid/recipes/boost/use-android-libs.patch
 pythonforandroid/recipes/boost/user-config.jam
```

### Comparing `python-for-android-2023.2.10/pythonforandroid/androidndk.py` & `python-for-android-2023.5.21/pythonforandroid/androidndk.py`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/archs.py` & `python-for-android-2023.5.21/pythonforandroid/archs.py`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/bdistapk.py` & `python-for-android-2023.5.21/pythonforandroid/bdistapk.py`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/bootstrap.py` & `python-for-android-2023.5.21/pythonforandroid/bootstrap.py`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/bootstraps/common/build/ant.properties` & `python-for-android-2023.5.21/pythonforandroid/bootstraps/common/build/ant.properties`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/bootstraps/common/build/build.py` & `python-for-android-2023.5.21/pythonforandroid/bootstraps/common/build/build.py`

 * *Files 0% similar despite different names*

```diff
@@ -494,22 +494,24 @@
             base_service_class=base_service_class,
         )
 
     # Find the SDK directory and target API
     with open('project.properties', 'r') as fileh:
         target = fileh.read().strip()
     android_api = target.split('-')[1]
-    try:
-        int(android_api)
-    except (ValueError, TypeError):
+
+    if android_api.isdigit():
+        android_api = int(android_api)
+    else:
         raise ValueError(
             "failed to extract the Android API level from " +
             "build.properties. expected int, got: '" +
             str(android_api) + "'"
         )
+
     with open('local.properties', 'r') as fileh:
         sdk_dir = fileh.read().strip()
     sdk_dir = sdk_dir[8:]
 
     # Try to build with the newest available build tools
     ignored = {".DS_Store", ".ds_store"}
     build_tools_versions = [x for x in listdir(join(sdk_dir, 'build-tools')) if x not in ignored]
@@ -769,14 +771,16 @@
                           'same number of groups of numbers as previous '
                           'versions.'),
                     required=True)
     if get_bootstrap_name() == "sdl2":
         ap.add_argument('--launcher', dest='launcher', action='store_true',
                         help=('Provide this argument to build a multi-app '
                               'launcher, rather than a single app.'))
+        ap.add_argument('--home-app', dest='home_app', action='store_true', default=False,
+                        help=('Turn your application into a home app (launcher)'))
     ap.add_argument('--permission', dest='permissions', action='append', default=[],
                     help='The permissions to give this app.', nargs='+')
     ap.add_argument('--meta-data', dest='meta_data', action='append', default=[],
                     help='Custom key=value to add in application metadata')
     ap.add_argument('--uses-library', dest='android_used_libs', action='append', default=[],
                     help='Used shared libraries included using <uses-library> tag in AndroidManifest.xml')
     ap.add_argument('--asset', dest='assets',
```

### Comparing `python-for-android-2023.2.10/pythonforandroid/bootstraps/common/build/gradle/wrapper/gradle-wrapper.jar` & `python-for-android-2023.5.21/pythonforandroid/bootstraps/common/build/gradle/wrapper/gradle-wrapper.jar`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/bootstraps/common/build/gradlew` & `python-for-android-2023.5.21/pythonforandroid/bootstraps/common/build/gradlew`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/bootstraps/common/build/gradlew.bat` & `python-for-android-2023.5.21/pythonforandroid/bootstraps/common/build/gradlew.bat`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/bootstraps/common/build/jni/application/src/Android.mk` & `python-for-android-2023.5.21/pythonforandroid/bootstraps/common/build/jni/application/src/Android.mk`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/bootstraps/common/build/jni/application/src/start.c` & `python-for-android-2023.5.21/pythonforandroid/bootstraps/common/build/jni/application/src/start.c`

 * *Files 2% similar despite different names*

```diff
@@ -202,15 +202,15 @@
 
   PyRun_SimpleString("import androidembed\nandroidembed.log('testing python "
                      "print redirection')");
 
   /* inject our bootstrap code to redirect python stdin/stdout
    * replace sys.path with our path
    */
-  PyRun_SimpleString("import sys, posix\n");
+  PyRun_SimpleString("import io, sys, posix\n");
 
   char add_site_packages_dir[256];
 
   if (dir_exists(python_bundle_dir)) {
     snprintf(add_site_packages_dir, 256,
              "sys.path.append('%s/site-packages')",
              python_bundle_dir);
@@ -220,25 +220,27 @@
                        "from os.path import realpath, join, dirname");
     PyRun_SimpleString(add_site_packages_dir);
     /* "sys.path.append(join(dirname(realpath(__file__)), 'site-packages'))") */
     PyRun_SimpleString("sys.path = ['.'] + sys.path");
   }
 
   PyRun_SimpleString(
-      "class LogFile(object):\n"
+      "class LogFile(io.IOBase):\n"
       "    def __init__(self):\n"
       "        self.__buffer = ''\n"
+      "    def readable(self):\n"
+      "        return False\n"
+      "    def writable(self):\n"
+      "        return True\n"
       "    def write(self, s):\n"
       "        s = self.__buffer + s\n"
       "        lines = s.split('\\n')\n"
       "        for l in lines[:-1]:\n"
       "            androidembed.log(l.replace('\\x00', ''))\n"
       "        self.__buffer = lines[-1]\n"
-      "    def flush(self):\n"
-      "        return\n"
       "sys.stdout = sys.stderr = LogFile()\n"
       "print('Android path', sys.path)\n"
       "import os\n"
       "print('os.environ is', os.environ)\n"
       "print('Android kivy bootstrap done. __name__ is', __name__)");
 
 #if PY_MAJOR_VERSION < 3
```

### Comparing `python-for-android-2023.2.10/pythonforandroid/bootstraps/common/build/src/main/java/org/kamranzafar/jtar/Octal.java` & `python-for-android-2023.5.21/pythonforandroid/bootstraps/common/build/src/main/java/org/kamranzafar/jtar/Octal.java`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/bootstraps/common/build/src/main/java/org/kamranzafar/jtar/TarConstants.java` & `python-for-android-2023.5.21/pythonforandroid/bootstraps/common/build/src/main/java/org/kamranzafar/jtar/TarConstants.java`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/bootstraps/common/build/src/main/java/org/kamranzafar/jtar/TarEntry.java` & `python-for-android-2023.5.21/pythonforandroid/bootstraps/common/build/src/main/java/org/kamranzafar/jtar/TarEntry.java`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/bootstraps/common/build/src/main/java/org/kamranzafar/jtar/TarHeader.java` & `python-for-android-2023.5.21/pythonforandroid/bootstraps/common/build/src/main/java/org/kamranzafar/jtar/TarHeader.java`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/bootstraps/common/build/src/main/java/org/kamranzafar/jtar/TarInputStream.java` & `python-for-android-2023.5.21/pythonforandroid/bootstraps/common/build/src/main/java/org/kamranzafar/jtar/TarInputStream.java`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/bootstraps/common/build/src/main/java/org/kamranzafar/jtar/TarOutputStream.java` & `python-for-android-2023.5.21/pythonforandroid/bootstraps/common/build/src/main/java/org/kamranzafar/jtar/TarOutputStream.java`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/bootstraps/common/build/src/main/java/org/kamranzafar/jtar/TarUtils.java` & `python-for-android-2023.5.21/pythonforandroid/bootstraps/common/build/src/main/java/org/kamranzafar/jtar/TarUtils.java`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/bootstraps/common/build/src/main/java/org/kivy/android/PythonService.java` & `python-for-android-2023.5.21/pythonforandroid/bootstraps/common/build/src/main/java/org/kivy/android/PythonService.java`

 * *Files 3% similar despite different names*

```diff
@@ -109,26 +109,28 @@
         Context context = getApplicationContext();
         Intent contextIntent = new Intent(context, PythonActivity.class);
         PendingIntent pIntent = PendingIntent.getActivity(context, 0, contextIntent,
             PendingIntent.FLAG_IMMUTABLE | PendingIntent.FLAG_UPDATE_CURRENT);
 
 	// Unspecified icon uses default.
 	int smallIconId = context.getApplicationInfo().icon;
-	if (!smallIconName.equals("")){
-	    int resId = getResources().getIdentifier(smallIconName, "mipmap",
-						     getPackageName());
-	    if (resId ==0) {
-		resId = getResources().getIdentifier(smallIconName, "drawable",
-						     getPackageName());
-	    }
-	    if (resId !=0) {
-		smallIconId = resId;
-	    }
-	}
-	    
+    if (smallIconName != null) {
+        if (!smallIconName.equals("")){
+            int resId = getResources().getIdentifier(smallIconName, "mipmap",
+                                 getPackageName());
+            if (resId ==0) {
+            resId = getResources().getIdentifier(smallIconName, "drawable",
+                                 getPackageName());
+            }
+            if (resId !=0) {
+            smallIconId = resId;
+            }
+        }
+    }
+
 	if (Build.VERSION.SDK_INT < Build.VERSION_CODES.O) {
 	    // This constructor is deprecated
             notification = new Notification(
                 smallIconId, serviceTitle, System.currentTimeMillis());
             try {
                 // prevent using NotificationCompat, this saves 100kb on apk
                 Method func = notification.getClass().getMethod(
@@ -139,17 +141,16 @@
                      IllegalArgumentException | InvocationTargetException e) {
             }
         } else {
             // for android 8+ we need to create our own channel
             // https://stackoverflow.com/questions/47531742/startforeground-fail-after-upgrade-to-android-8-1
             String NOTIFICATION_CHANNEL_ID = "org.kivy.p4a" + getServiceId();
             String channelName = "Background Service" + getServiceId();
-            NotificationChannel chan = new NotificationChannel(NOTIFICATION_CHANNEL_ID, channelName, 
-                NotificationManager.IMPORTANCE_NONE);
-            
+            NotificationChannel chan = new NotificationChannel(NOTIFICATION_CHANNEL_ID, channelName, NotificationManager.IMPORTANCE_NONE);
+
             chan.setLightColor(Color.BLUE);
             chan.setLockscreenVisibility(Notification.VISIBILITY_PRIVATE);
             NotificationManager manager = (NotificationManager) getSystemService(Context.NOTIFICATION_SERVICE);
             manager.createNotificationChannel(chan);
 
             Notification.Builder builder = new Notification.Builder(context, NOTIFICATION_CHANNEL_ID);
             builder.setContentTitle(contentTitle);
```

### Comparing `python-for-android-2023.2.10/pythonforandroid/bootstraps/common/build/src/main/java/org/kivy/android/PythonUtil.java` & `python-for-android-2023.5.21/pythonforandroid/bootstraps/common/build/src/main/java/org/kivy/android/PythonUtil.java`

 * *Files 1% similar despite different names*

```diff
@@ -50,14 +50,15 @@
         addLibraryIfExists(libsList, "SDL2_mixer", libsDir);
         addLibraryIfExists(libsList, "SDL2_ttf", libsDir);
         libsList.add("python3.5m");
         libsList.add("python3.6m");
         libsList.add("python3.7m");
         libsList.add("python3.8");
         libsList.add("python3.9");
+        libsList.add("python3.10");
         libsList.add("main");
         return libsList;
     }
 
     public static void loadLibraries(File filesDir, File libsDir) {
         boolean foundPython = false;
 
@@ -69,15 +70,15 @@
                     foundPython = true;
                 }
             } catch(UnsatisfiedLinkError e) {
                 // If this is the last possible libpython
                 // load, and it has failed, give a more
                 // general error
                 Log.v(TAG, "Library loading error: " + e.getMessage());
-                if (lib.startsWith("python3.9") && !foundPython) {
+                if (lib.startsWith("python3.10") && !foundPython) {
                     throw new RuntimeException("Could not load any libpythonXXX.so");
                 } else if (lib.startsWith("python")) {
                     continue;
                 } else {
                     Log.v(TAG, "An UnsatisfiedLinkError occurred loading " + lib);
                     throw e;
                 }
```

### Comparing `python-for-android-2023.2.10/pythonforandroid/bootstraps/common/build/src/main/java/org/renpy/android/AssetExtract.java` & `python-for-android-2023.5.21/pythonforandroid/bootstraps/common/build/src/main/java/org/renpy/android/AssetExtract.java`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/bootstraps/common/build/src/main/java/org/renpy/android/Hardware.java` & `python-for-android-2023.5.21/pythonforandroid/bootstraps/common/build/src/main/java/org/renpy/android/Hardware.java`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/bootstraps/common/build/src/main/java/org/renpy/android/ResourceManager.java` & `python-for-android-2023.5.21/pythonforandroid/bootstraps/common/build/src/main/java/org/renpy/android/ResourceManager.java`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/bootstraps/common/build/templates/Service.tmpl.java` & `python-for-android-2023.5.21/pythonforandroid/bootstraps/common/build/templates/Service.tmpl.java`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/bootstraps/common/build/templates/build.properties` & `python-for-android-2023.5.21/pythonforandroid/bootstraps/common/build/templates/build.properties`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/bootstraps/common/build/templates/build.tmpl.gradle` & `python-for-android-2023.5.21/pythonforandroid/bootstraps/common/build/templates/build.tmpl.gradle`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/bootstraps/common/build/templates/build.tmpl.xml` & `python-for-android-2023.5.21/pythonforandroid/bootstraps/common/build/templates/build.tmpl.xml`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/bootstraps/common/build/templates/custom_rules.tmpl.xml` & `python-for-android-2023.5.21/pythonforandroid/bootstraps/common/build/templates/custom_rules.tmpl.xml`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/bootstraps/common/build/templates/kivy-icon.png` & `python-for-android-2023.5.21/pythonforandroid/bootstraps/common/build/templates/kivy-icon.png`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/bootstraps/common/build/templates/kivy-presplash.jpg` & `python-for-android-2023.5.21/pythonforandroid/bootstraps/common/build/templates/kivy-presplash.jpg`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/bootstraps/common/build/templates/lottie.xml` & `python-for-android-2023.5.21/pythonforandroid/bootstraps/common/build/templates/lottie.xml`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/bootstraps/sdl2/__init__.py` & `python-for-android-2023.5.21/pythonforandroid/bootstraps/sdl2/__init__.py`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/bootstraps/sdl2/build/blacklist.txt` & `python-for-android-2023.5.21/pythonforandroid/bootstraps/sdl2/build/blacklist.txt`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/bootstraps/sdl2/build/src/main/java/org/kivy/android/PythonActivity.java` & `python-for-android-2023.5.21/pythonforandroid/bootstraps/sdl2/build/src/main/java/org/kivy/android/PythonActivity.java`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/bootstraps/sdl2/build/src/main/java/org/kivy/android/launcher/Project.java` & `python-for-android-2023.5.21/pythonforandroid/bootstraps/sdl2/build/src/main/java/org/kivy/android/launcher/Project.java`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/bootstraps/sdl2/build/src/main/java/org/kivy/android/launcher/ProjectAdapter.java` & `python-for-android-2023.5.21/pythonforandroid/bootstraps/sdl2/build/src/main/java/org/kivy/android/launcher/ProjectAdapter.java`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/bootstraps/sdl2/build/src/main/java/org/kivy/android/launcher/ProjectChooser.java` & `python-for-android-2023.5.21/pythonforandroid/bootstraps/sdl2/build/src/main/java/org/kivy/android/launcher/ProjectChooser.java`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/bootstraps/sdl2/build/src/main/res/drawable-hdpi/ic_launcher.png` & `python-for-android-2023.5.21/pythonforandroid/bootstraps/sdl2/build/src/main/res/drawable-hdpi/ic_launcher.png`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/bootstraps/sdl2/build/src/main/res/drawable-mdpi/ic_launcher.png` & `python-for-android-2023.5.21/pythonforandroid/bootstraps/sdl2/build/src/main/res/drawable-mdpi/ic_launcher.png`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/bootstraps/sdl2/build/src/main/res/drawable-xhdpi/ic_launcher.png` & `python-for-android-2023.5.21/pythonforandroid/bootstraps/sdl2/build/src/main/res/drawable-xhdpi/ic_launcher.png`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/bootstraps/sdl2/build/src/main/res/drawable-xxhdpi/ic_launcher.png` & `python-for-android-2023.5.21/pythonforandroid/bootstraps/sdl2/build/src/main/res/drawable-xxhdpi/ic_launcher.png`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/bootstraps/sdl2/build/src/main/res/layout/chooser_item.xml` & `python-for-android-2023.5.21/pythonforandroid/bootstraps/sdl2/build/src/main/res/layout/chooser_item.xml`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/bootstraps/sdl2/build/src/patches/SDLActivity.java.patch` & `python-for-android-2023.5.21/pythonforandroid/bootstraps/sdl2/build/src/patches/SDLActivity.java.patch`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/bootstraps/sdl2/build/templates/AndroidManifest.tmpl.xml` & `python-for-android-2023.5.21/pythonforandroid/bootstraps/sdl2/build/templates/AndroidManifest.tmpl.xml`

 * *Files 2% similar despite different names*

```diff
@@ -72,27 +72,30 @@
                   android:screenOrientation="{{ args.manifest_orientation }}"
                   android:exported="true"
                   {% if args.activity_launch_mode %}
                   android:launchMode="{{ args.activity_launch_mode }}"
                   {% endif %}
                   >
 
-            {% if args.launcher %}
             <intent-filter>
+            {% if args.launcher %}            
                 <action android:name="org.kivy.LAUNCH" />
                 <category android:name="android.intent.category.DEFAULT" />
                 <data android:scheme="{{ url_scheme }}" />
-            </intent-filter>
             {% else  %}
-            <intent-filter>
                 <action android:name="android.intent.action.MAIN" />
                 <category android:name="android.intent.category.LAUNCHER" />
-            </intent-filter>
             {% endif %}
 
+            {% if args.home_app %}
+                <category android:name="android.intent.category.HOME" />
+                <category android:name="android.intent.category.DEFAULT" />
+            {% endif %}
+            </intent-filter>
+
             {%- if args.intent_filters -%}
             {{- args.intent_filters -}}
             {%- endif -%}
         </activity>
 
         {% if args.launcher %}
         <activity android:name="org.kivy.android.launcher.ProjectChooser"
```

### Comparing `python-for-android-2023.2.10/pythonforandroid/bootstraps/service_library/build/templates/AndroidManifest.tmpl.xml` & `python-for-android-2023.5.21/pythonforandroid/bootstraps/service_library/build/templates/AndroidManifest.tmpl.xml`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/bootstraps/service_library/build/templates/Service.tmpl.java` & `python-for-android-2023.5.21/pythonforandroid/bootstraps/service_library/build/templates/Service.tmpl.java`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/bootstraps/service_only/__init__.py` & `python-for-android-2023.5.21/pythonforandroid/bootstraps/service_only/__init__.py`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/bootstraps/service_only/build/blacklist.txt` & `python-for-android-2023.5.21/pythonforandroid/bootstraps/service_only/build/blacklist.txt`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/bootstraps/service_only/build/jni/application/src/pyjniusjni.c` & `python-for-android-2023.5.21/pythonforandroid/bootstraps/service_only/build/jni/application/src/pyjniusjni.c`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/bootstraps/service_only/build/src/main/java/org/kivy/android/PythonActivity.java` & `python-for-android-2023.5.21/pythonforandroid/bootstraps/service_only/build/src/main/java/org/kivy/android/PythonActivity.java`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/bootstraps/service_only/build/templates/AndroidManifest.tmpl.xml` & `python-for-android-2023.5.21/pythonforandroid/bootstraps/service_only/build/templates/AndroidManifest.tmpl.xml`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/bootstraps/service_only/build/templates/Service.tmpl.java` & `python-for-android-2023.5.21/pythonforandroid/bootstraps/service_only/build/templates/Service.tmpl.java`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/bootstraps/webview/__init__.py` & `python-for-android-2023.5.21/pythonforandroid/bootstraps/webview/__init__.py`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/bootstraps/webview/build/blacklist.txt` & `python-for-android-2023.5.21/pythonforandroid/bootstraps/webview/build/blacklist.txt`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/bootstraps/webview/build/jni/application/src/pyjniusjni.c` & `python-for-android-2023.5.21/pythonforandroid/bootstraps/webview/build/jni/application/src/pyjniusjni.c`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/bootstraps/webview/build/proguard-project.txt` & `python-for-android-2023.5.21/pythonforandroid/bootstraps/webview/build/proguard-project.txt`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/bootstraps/webview/build/src/main/java/org/kivy/android/PythonActivity.java` & `python-for-android-2023.5.21/pythonforandroid/bootstraps/webview/build/src/main/java/org/kivy/android/PythonActivity.java`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/bootstraps/webview/build/src/main/res/drawable/icon.png` & `python-for-android-2023.5.21/pythonforandroid/bootstraps/webview/build/src/main/res/drawable/icon.png`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/bootstraps/webview/build/templates/AndroidManifest.tmpl.xml` & `python-for-android-2023.5.21/pythonforandroid/bootstraps/webview/build/templates/AndroidManifest.tmpl.xml`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/bootstraps/webview/build/templates/WebViewLoader.tmpl.java` & `python-for-android-2023.5.21/pythonforandroid/bootstraps/webview/build/templates/WebViewLoader.tmpl.java`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/bootstraps/webview/build/templates/test/build.tmpl.xml` & `python-for-android-2023.5.21/pythonforandroid/bootstraps/webview/build/templates/test/build.tmpl.xml`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/bootstraps/webview/build/templates/test/build.xml.tmpl` & `python-for-android-2023.5.21/pythonforandroid/bootstraps/webview/build/templates/test/build.xml.tmpl`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/build.py` & `python-for-android-2023.5.21/pythonforandroid/build.py`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/distribution.py` & `python-for-android-2023.5.21/pythonforandroid/distribution.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from os.path import exists, join
 import glob
 import json
 
-from pythonforandroid.logger import (info, info_notify, warning, Err_Style, Err_Fore)
+from pythonforandroid.logger import (debug, info, info_notify, warning, Err_Style, Err_Fore)
 from pythonforandroid.util import current_directory, BuildInterruptingException
 from shutil import rmtree
 
 
 class Distribution:
     '''State container for information about a distribution (i.e. an
     Android project).
@@ -87,23 +87,25 @@
         allow_replace_dist : bool
             If True, will allow an existing dist with the specified
             name but incompatible requirements to be overwritten by
             a new one with the current requirements.
         '''
 
         possible_dists = Distribution.get_distributions(ctx)
+        debug(f"All possible dists: {possible_dists}")
 
         # Will hold dists that would be built in the same folder as an existing dist
         folder_match_dist = None
 
         # 0) Check if a dist with that name and architecture already exists
         if name is not None and name:
             possible_dists = [
                 d for d in possible_dists if
                 (d.name == name) and all(arch_name in d.archs for arch_name in archs)]
+            debug(f"Dist matching name and arch: {possible_dists}")
 
             if possible_dists:
                 # There should only be one folder with a given dist name *and* arch.
                 # We could check that here, but for compatibility let's let it slide
                 # and just record the details of one of them. We only use this data to
                 # possibly fail the build later, so it doesn't really matter if there
                 # was more than one clash.
@@ -111,43 +113,55 @@
 
         # 1) Check if any existing dists meet the requirements
         _possible_dists = []
         for dist in possible_dists:
             if (
                 ndk_api is not None and dist.ndk_api != ndk_api
             ) or dist.ndk_api is None:
+                debug(
+                    f"dist {dist} failed to match ndk_api, target api {ndk_api}, dist api {dist.ndk_api}"
+                )
                 continue
             for recipe in recipes:
                 if recipe not in dist.recipes:
+                    debug(f"dist {dist} missing recipe {recipe}")
                     break
             else:
                 _possible_dists.append(dist)
         possible_dists = _possible_dists
+        debug(f"Dist matching ndk_api and recipe: {possible_dists}")
 
         if possible_dists:
             info('Of the existing distributions, the following meet '
                  'the given requirements:')
             pretty_log_dists(possible_dists)
         else:
             info('No existing dists meet the given requirements!')
 
         # If any dist has perfect recipes, arch and NDK API, return it
         for dist in possible_dists:
             if force_build:
+                debug("Skipping dist due to forced build")
                 continue
             if ndk_api is not None and dist.ndk_api != ndk_api:
+                debug("Skipping dist due to ndk_api mismatch")
                 continue
             if not all(arch_name in dist.archs for arch_name in archs):
+                debug("Skipping dist due to arch mismatch")
                 continue
             if (set(dist.recipes) == set(recipes) or
                 (set(recipes).issubset(set(dist.recipes)) and
                  not require_perfect_match)):
                 info_notify('{} has compatible recipes, using this one'
                             .format(dist.name))
                 return dist
+            else:
+                debug(
+                    f"Skipping dist due to recipes mismatch, expected {set(recipes)}, actual {set(dist.recipes)}"
+                )
 
         # If there was a name match but we didn't already choose it,
         # then the existing dist is incompatible with the requested
         # configuration and the build cannot continue
         if folder_match_dist is not None and not allow_replace_dist:
             raise BuildInterruptingException(
                 'Asked for dist with name {name} with recipes ({req_recipes}) and '
```

### Comparing `python-for-android-2023.2.10/pythonforandroid/entrypoints.py` & `python-for-android-2023.5.21/pythonforandroid/entrypoints.py`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/graph.py` & `python-for-android-2023.5.21/pythonforandroid/graph.py`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/logger.py` & `python-for-android-2023.5.21/pythonforandroid/logger.py`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/patching.py` & `python-for-android-2023.5.21/pythonforandroid/patching.py`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/prerequisites.py` & `python-for-android-2023.5.21/pythonforandroid/prerequisites.py`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/pythonpackage.py` & `python-for-android-2023.5.21/pythonforandroid/pythonpackage.py`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/recipe.py` & `python-for-android-2023.5.21/pythonforandroid/recipe.py`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/recipes/Pillow/__init__.py` & `python-for-android-2023.5.21/pythonforandroid/recipes/Pillow/__init__.py`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/recipes/Pillow/patches/fix-setup.patch` & `python-for-android-2023.5.21/pythonforandroid/recipes/Pillow/patches/fix-setup.patch`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/recipes/aiohttp/__init__.py` & `python-for-android-2023.5.21/pythonforandroid/recipes/aiohttp/__init__.py`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/recipes/android/__init__.py` & `python-for-android-2023.5.21/pythonforandroid/recipes/android/__init__.py`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/recipes/android/src/android/_android.pyx` & `python-for-android-2023.5.21/pythonforandroid/recipes/android/src/android/_android.pyx`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/recipes/android/src/android/_android_billing.pyx` & `python-for-android-2023.5.21/pythonforandroid/recipes/android/src/android/_android_billing.pyx`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/recipes/android/src/android/_android_billing_jni.c` & `python-for-android-2023.5.21/pythonforandroid/recipes/android/src/android/_android_billing_jni.c`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/recipes/android/src/android/_android_jni.c` & `python-for-android-2023.5.21/pythonforandroid/recipes/android/src/android/_android_jni.c`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/recipes/android/src/android/_android_sound.pyx` & `python-for-android-2023.5.21/pythonforandroid/recipes/android/src/android/_android_sound.pyx`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/recipes/android/src/android/_android_sound_jni.c` & `python-for-android-2023.5.21/pythonforandroid/recipes/android/src/android/_android_sound_jni.c`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/recipes/android/src/android/_ctypes_library_finder.py` & `python-for-android-2023.5.21/pythonforandroid/recipes/android/src/android/_ctypes_library_finder.py`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/recipes/android/src/android/activity.py` & `python-for-android-2023.5.21/pythonforandroid/recipes/android/src/android/activity.py`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/recipes/android/src/android/broadcast.py` & `python-for-android-2023.5.21/pythonforandroid/recipes/android/src/android/broadcast.py`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/recipes/android/src/android/mixer.py` & `python-for-android-2023.5.21/pythonforandroid/recipes/android/src/android/mixer.py`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/recipes/android/src/android/permissions.py` & `python-for-android-2023.5.21/pythonforandroid/recipes/android/src/android/permissions.py`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/recipes/android/src/android/runnable.py` & `python-for-android-2023.5.21/pythonforandroid/recipes/android/src/android/runnable.py`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/recipes/android/src/android/storage.py` & `python-for-android-2023.5.21/pythonforandroid/recipes/android/src/android/storage.py`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/recipes/android/src/setup.py` & `python-for-android-2023.5.21/pythonforandroid/recipes/android/src/setup.py`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/recipes/apsw/__init__.py` & `python-for-android-2023.5.21/pythonforandroid/recipes/apsw/__init__.py`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/recipes/audiostream/__init__.py` & `python-for-android-2023.5.21/pythonforandroid/recipes/audiostream/__init__.py`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/recipes/bcrypt/__init__.py` & `python-for-android-2023.5.21/pythonforandroid/recipes/bcrypt/__init__.py`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/recipes/boost/__init__.py` & `python-for-android-2023.5.21/pythonforandroid/recipes/boost/__init__.py`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/recipes/boost/fix-android-issues.patch` & `python-for-android-2023.5.21/pythonforandroid/recipes/boost/fix-android-issues.patch`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/recipes/boost/user-config.jam` & `python-for-android-2023.5.21/pythonforandroid/recipes/boost/user-config.jam`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/recipes/cffi/__init__.py` & `python-for-android-2023.5.21/pythonforandroid/recipes/cffi/__init__.py`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/recipes/cffi/disable-pkg-config.patch` & `python-for-android-2023.5.21/pythonforandroid/recipes/cffi/disable-pkg-config.patch`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/recipes/cryptography/__init__.py` & `python-for-android-2023.5.21/pythonforandroid/recipes/cryptography/__init__.py`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/recipes/enaml/0001-Update-setup.py.patch` & `python-for-android-2023.5.21/pythonforandroid/recipes/enaml/0001-Update-setup.py.patch`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/recipes/evdev/__init__.py` & `python-for-android-2023.5.21/pythonforandroid/recipes/evdev/__init__.py`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/recipes/evdev/evcnt.patch` & `python-for-android-2023.5.21/pythonforandroid/recipes/evdev/evcnt.patch`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/recipes/evdev/evdev-permissions.patch` & `python-for-android-2023.5.21/pythonforandroid/recipes/evdev/evdev-permissions.patch`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/recipes/evdev/keycnt.patch` & `python-for-android-2023.5.21/pythonforandroid/recipes/evdev/keycnt.patch`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/recipes/evdev/remove-uinput.patch` & `python-for-android-2023.5.21/pythonforandroid/recipes/evdev/remove-uinput.patch`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/recipes/ffmpeg/__init__.py` & `python-for-android-2023.5.21/pythonforandroid/recipes/ffmpeg/__init__.py`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/recipes/ffmpeg/patches/configure.patch` & `python-for-android-2023.5.21/pythonforandroid/recipes/ffmpeg/patches/configure.patch`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/recipes/ffpyplayer/__init__.py` & `python-for-android-2023.5.21/pythonforandroid/recipes/ffpyplayer/__init__.py`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/recipes/fontconfig/__init__.py` & `python-for-android-2023.5.21/pythonforandroid/recipes/fontconfig/__init__.py`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/recipes/freetype/__init__.py` & `python-for-android-2023.5.21/pythonforandroid/recipes/freetype/__init__.py`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/recipes/genericndkbuild/__init__.py` & `python-for-android-2023.5.21/pythonforandroid/recipes/genericndkbuild/__init__.py`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/recipes/gevent/__init__.py` & `python-for-android-2023.5.21/pythonforandroid/recipes/gevent/__init__.py`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/recipes/gevent/cross_compiling.patch` & `python-for-android-2023.5.21/pythonforandroid/recipes/gevent/cross_compiling.patch`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/recipes/harfbuzz/__init__.py` & `python-for-android-2023.5.21/pythonforandroid/recipes/harfbuzz/__init__.py`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/recipes/hostpython3/__init__.py` & `python-for-android-2023.5.21/pythonforandroid/recipes/hostpython3/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,15 @@
         Refactored from deleted class ``python.HostPythonRecipe`` into here.
 
     .. versionchanged:: 0.6.0
         Refactored into  the new class
         :class:`~pythonforandroid.python.HostPythonRecipe`
     '''
 
-    version = '3.9.9'
+    version = '3.10.10'
     name = 'hostpython3'
 
     build_subdir = 'native-build'
     '''Specify the sub build directory for the hostpython3 recipe. Defaults
     to ``native-build``.'''
 
     url = 'https://www.python.org/ftp/python/{version}/Python-{version}.tgz'
```

### Comparing `python-for-android-2023.2.10/pythonforandroid/recipes/hostpython3/patches/pyconfig_detection.patch` & `python-for-android-2023.5.21/pythonforandroid/recipes/hostpython3/patches/pyconfig_detection.patch`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/recipes/icu/__init__.py` & `python-for-android-2023.5.21/pythonforandroid/recipes/icu/__init__.py`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/recipes/icu/disable-libs-version.patch` & `python-for-android-2023.5.21/pythonforandroid/recipes/icu/disable-libs-version.patch`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/recipes/ifaddr/getifaddrs.patch` & `python-for-android-2023.5.21/pythonforandroid/recipes/ifaddr/getifaddrs.patch`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/recipes/ifaddrs/__init__.py` & `python-for-android-2023.5.21/pythonforandroid/recipes/ifaddrs/__init__.py`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/recipes/jedi/fix_MergedNamesDict_get.patch` & `python-for-android-2023.5.21/pythonforandroid/recipes/jedi/fix_MergedNamesDict_get.patch`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/recipes/jpeg/__init__.py` & `python-for-android-2023.5.21/pythonforandroid/recipes/jpeg/__init__.py`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/recipes/jpeg/build-static.patch` & `python-for-android-2023.5.21/pythonforandroid/recipes/jpeg/build-static.patch`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/recipes/jpeg/remove-version.patch` & `python-for-android-2023.5.21/pythonforandroid/recipes/jpeg/remove-version.patch`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/recipes/kivy/__init__.py` & `python-for-android-2023.5.21/pythonforandroid/recipes/kivy/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,20 +18,20 @@
 
         return packaging.version.parse(
             str(kivy_version)
         ) < packaging.version.Version("2.2.0.dev0")
 
 
 class KivyRecipe(CythonRecipe):
-    version = '2.1.0'
+    version = '2.2.0'
     url = 'https://github.com/kivy/kivy/archive/{version}.zip'
     name = 'kivy'
 
     depends = ['sdl2', 'pyjnius', 'setuptools']
-    python_depends = ['certifi']
+    python_depends = ['certifi', 'chardet', 'idna', 'requests', 'urllib3']
 
     # sdl-gl-swapwindow-nogil.patch is needed to avoid a deadlock.
     # See: https://github.com/kivy/kivy/pull/8025
     # WARNING: Remove this patch when a new Kivy version is released.
     patches = [("sdl-gl-swapwindow-nogil.patch", is_kivy_affected_by_deadlock_issue)]
 
     def cythonize_build(self, env, build_dir='.'):
```

### Comparing `python-for-android-2023.2.10/pythonforandroid/recipes/kivy/sdl-gl-swapwindow-nogil.patch` & `python-for-android-2023.5.21/pythonforandroid/recipes/kivy/sdl-gl-swapwindow-nogil.patch`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/recipes/kivy3/__init__.py` & `python-for-android-2023.5.21/pythonforandroid/recipes/kivy3/__init__.py`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/recipes/lapack/__init__.py` & `python-for-android-2023.5.21/pythonforandroid/recipes/lapack/__init__.py`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/recipes/leveldb/__init__.py` & `python-for-android-2023.5.21/pythonforandroid/recipes/leveldb/__init__.py`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/recipes/libbz2/__init__.py` & `python-for-android-2023.5.21/pythonforandroid/recipes/libbz2/__init__.py`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/recipes/libbz2/lib_android.patch` & `python-for-android-2023.5.21/pythonforandroid/recipes/libbz2/lib_android.patch`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/recipes/libcurl/__init__.py` & `python-for-android-2023.5.21/pythonforandroid/recipes/libcurl/__init__.py`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/recipes/libexpat/__init__.py` & `python-for-android-2023.5.21/pythonforandroid/recipes/libexpat/__init__.py`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/recipes/libffi/__init__.py` & `python-for-android-2023.5.21/pythonforandroid/recipes/libffi/__init__.py`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/recipes/libffi/disable-mips-check.patch` & `python-for-android-2023.5.21/pythonforandroid/recipes/libffi/disable-mips-check.patch`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/recipes/libffi/remove-version-info.patch` & `python-for-android-2023.5.21/pythonforandroid/recipes/libffi/remove-version-info.patch`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/recipes/libgeos/__init__.py` & `python-for-android-2023.5.21/pythonforandroid/recipes/libgeos/__init__.py`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/recipes/libglob/__init__.py` & `python-for-android-2023.5.21/pythonforandroid/recipes/libglob/__init__.py`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/recipes/libglob/glob.patch` & `python-for-android-2023.5.21/pythonforandroid/recipes/libglob/glob.patch`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/recipes/libiconv/__init__.py` & `python-for-android-2023.5.21/pythonforandroid/recipes/libiconv/__init__.py`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/recipes/liblzma/__init__.py` & `python-for-android-2023.5.21/pythonforandroid/recipes/liblzma/__init__.py`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/recipes/libmysqlclient/__init__.py` & `python-for-android-2023.5.21/pythonforandroid/recipes/libmysqlclient/__init__.py`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/recipes/libmysqlclient/disable-soversion.patch` & `python-for-android-2023.5.21/pythonforandroid/recipes/libmysqlclient/disable-soversion.patch`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/recipes/libogg/__init__.py` & `python-for-android-2023.5.21/pythonforandroid/recipes/libogg/__init__.py`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/recipes/libpcre/__init__.py` & `python-for-android-2023.5.21/pythonforandroid/recipes/libpcre/__init__.py`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/recipes/libpq/__init__.py` & `python-for-android-2023.5.21/pythonforandroid/recipes/libpq/__init__.py`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/recipes/librt/__init__.py` & `python-for-android-2023.5.21/pythonforandroid/recipes/librt/__init__.py`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/recipes/libsecp256k1/__init__.py` & `python-for-android-2023.5.21/pythonforandroid/recipes/libsecp256k1/__init__.py`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/recipes/libshine/__init__.py` & `python-for-android-2023.5.21/pythonforandroid/recipes/libshine/__init__.py`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/recipes/libsodium/__init__.py` & `python-for-android-2023.5.21/pythonforandroid/recipes/libsodium/__init__.py`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/recipes/libtorrent/__init__.py` & `python-for-android-2023.5.21/pythonforandroid/recipes/libtorrent/__init__.py`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/recipes/libtorrent/setup-lib-name.patch` & `python-for-android-2023.5.21/pythonforandroid/recipes/libtorrent/setup-lib-name.patch`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/recipes/libtorrent/user-config-openssl.patch` & `python-for-android-2023.5.21/pythonforandroid/recipes/libtorrent/user-config-openssl.patch`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/recipes/libtribler/__init__.py` & `python-for-android-2023.5.21/pythonforandroid/recipes/libtribler/__init__.py`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/recipes/libvorbis/__init__.py` & `python-for-android-2023.5.21/pythonforandroid/recipes/libvorbis/__init__.py`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/recipes/libvpx/__init__.py` & `python-for-android-2023.5.21/pythonforandroid/recipes/libvpx/__init__.py`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/recipes/libvpx/patches/0001-android-force-neon-runtime.patch` & `python-for-android-2023.5.21/pythonforandroid/recipes/libvpx/patches/0001-android-force-neon-runtime.patch`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/recipes/libwebp/__init__.py` & `python-for-android-2023.5.21/pythonforandroid/recipes/libwebp/__init__.py`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/recipes/libx264/__init__.py` & `python-for-android-2023.5.21/pythonforandroid/recipes/libx264/__init__.py`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/recipes/libxml2/__init__.py` & `python-for-android-2023.5.21/pythonforandroid/recipes/libxml2/__init__.py`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/recipes/libxml2/add-glob.c.patch` & `python-for-android-2023.5.21/pythonforandroid/recipes/libxml2/add-glob.c.patch`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/recipes/libxml2/glob.c` & `python-for-android-2023.5.21/pythonforandroid/recipes/libxml2/glob.c`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/recipes/libxml2/glob.h` & `python-for-android-2023.5.21/pythonforandroid/recipes/libxml2/glob.h`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/recipes/libxslt/__init__.py` & `python-for-android-2023.5.21/pythonforandroid/recipes/libxslt/__init__.py`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/recipes/libzbar/__init__.py` & `python-for-android-2023.5.21/pythonforandroid/recipes/libzbar/__init__.py`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/recipes/libzmq/__init__.py` & `python-for-android-2023.5.21/pythonforandroid/recipes/libzmq/__init__.py`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/recipes/lxml/__init__.py` & `python-for-android-2023.5.21/pythonforandroid/recipes/lxml/__init__.py`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/recipes/m2crypto/__init__.py` & `python-for-android-2023.5.21/pythonforandroid/recipes/m2crypto/__init__.py`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/recipes/matplotlib/__init__.py` & `python-for-android-2023.5.21/pythonforandroid/recipes/matplotlib/__init__.py`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/recipes/mysqldb/__init__.py` & `python-for-android-2023.5.21/pythonforandroid/recipes/mysqldb/__init__.py`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/recipes/mysqldb/override-mysql-config.patch` & `python-for-android-2023.5.21/pythonforandroid/recipes/mysqldb/override-mysql-config.patch`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/recipes/netifaces/fix-build.patch` & `python-for-android-2023.5.21/pythonforandroid/recipes/netifaces/fix-build.patch`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/recipes/numpy/__init__.py` & `python-for-android-2023.5.21/pythonforandroid/recipes/numpy/__init__.py`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/recipes/numpy/patches/add_libm_explicitly_to_build.patch` & `python-for-android-2023.5.21/pythonforandroid/recipes/numpy/patches/add_libm_explicitly_to_build.patch`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/recipes/numpy/patches/ranlib.patch` & `python-for-android-2023.5.21/pythonforandroid/recipes/numpy/patches/ranlib.patch`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/recipes/numpy/patches/remove-default-paths.patch` & `python-for-android-2023.5.21/pythonforandroid/recipes/numpy/patches/remove-default-paths.patch`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/recipes/omemo-backend-signal/__init__.py` & `python-for-android-2023.5.21/pythonforandroid/recipes/omemo-backend-signal/__init__.py`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/recipes/openal/__init__.py` & `python-for-android-2023.5.21/pythonforandroid/recipes/openal/__init__.py`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/recipes/opencv/__init__.py` & `python-for-android-2023.5.21/pythonforandroid/recipes/opencv/__init__.py`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/recipes/opencv/patches/p4a_build.patch` & `python-for-android-2023.5.21/pythonforandroid/recipes/opencv/patches/p4a_build.patch`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/recipes/opencv_extras/__init__.py` & `python-for-android-2023.5.21/pythonforandroid/recipes/opencv_extras/__init__.py`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/recipes/openssl/__init__.py` & `python-for-android-2023.5.21/pythonforandroid/recipes/openssl/__init__.py`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/recipes/pandas/__init__.py` & `python-for-android-2023.5.21/pythonforandroid/recipes/pandas/__init__.py`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/recipes/pandas/fix_numpy_includes.patch` & `python-for-android-2023.5.21/pythonforandroid/recipes/pandas/fix_numpy_includes.patch`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/recipes/pil/__init__.py` & `python-for-android-2023.5.21/pythonforandroid/recipes/pil/__init__.py`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/recipes/png/__init__.py` & `python-for-android-2023.5.21/pythonforandroid/recipes/png/__init__.py`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/recipes/preppy/fix-setup.patch` & `python-for-android-2023.5.21/pythonforandroid/recipes/preppy/fix-setup.patch`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/recipes/protobuf_cpp/__init__.py` & `python-for-android-2023.5.21/pythonforandroid/recipes/protobuf_cpp/__init__.py`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/recipes/protobuf_cpp/fix-python3-compatibility.patch` & `python-for-android-2023.5.21/pythonforandroid/recipes/protobuf_cpp/fix-python3-compatibility.patch`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/recipes/psycopg2/__init__.py` & `python-for-android-2023.5.21/pythonforandroid/recipes/psycopg2/__init__.py`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/recipes/py3dns/patches/android.patch` & `python-for-android-2023.5.21/pythonforandroid/recipes/py3dns/patches/android.patch`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/recipes/pycrypto/__init__.py` & `python-for-android-2023.5.21/pythonforandroid/recipes/pycrypto/__init__.py`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/recipes/pygame/__init__.py` & `python-for-android-2023.5.21/pythonforandroid/recipes/pygame/__init__.py`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/recipes/pyicu/__init__.py` & `python-for-android-2023.5.21/pythonforandroid/recipes/pyicu/__init__.py`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/recipes/pyjnius/__init__.py` & `python-for-android-2023.5.21/pythonforandroid/recipes/pyjnius/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pythonforandroid.toolchain import shprint, current_directory, info
 from pythonforandroid.patching import will_build
 import sh
 from os.path import join
 
 
 class PyjniusRecipe(CythonRecipe):
-    version = '1.4.2'
+    version = '1.5.0'
     url = 'https://github.com/kivy/pyjnius/archive/{version}.zip'
     name = 'pyjnius'
     depends = [('genericndkbuild', 'sdl2'), 'six']
     site_packages_name = 'jnius'
 
     patches = [('genericndkbuild_jnienv_getter.patch', will_build('genericndkbuild'))]
```

### Comparing `python-for-android-2023.2.10/pythonforandroid/recipes/pyjnius/genericndkbuild_jnienv_getter.patch` & `python-for-android-2023.5.21/pythonforandroid/recipes/pyjnius/genericndkbuild_jnienv_getter.patch`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/recipes/pyleveldb/__init__.py` & `python-for-android-2023.5.21/pythonforandroid/recipes/pyleveldb/__init__.py`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/recipes/pyleveldb/bindings-only.patch` & `python-for-android-2023.5.21/pythonforandroid/recipes/pyleveldb/bindings-only.patch`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/recipes/pymunk/__init__.py` & `python-for-android-2023.5.21/pythonforandroid/recipes/pymunk/__init__.py`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/recipes/pynacl/__init__.py` & `python-for-android-2023.5.21/pythonforandroid/recipes/pynacl/__init__.py`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/recipes/pyogg/patches/fix-find-lib.patch` & `python-for-android-2023.5.21/pythonforandroid/recipes/pyogg/patches/fix-find-lib.patch`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/recipes/pyopenal/patches/fix-find-lib.patch` & `python-for-android-2023.5.21/pythonforandroid/recipes/pyopenal/patches/fix-find-lib.patch`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/recipes/pyopenssl/fix-dlfcn.patch` & `python-for-android-2023.5.21/pythonforandroid/recipes/pyopenssl/fix-dlfcn.patch`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/recipes/pysha3/__init__.py` & `python-for-android-2023.5.21/pythonforandroid/recipes/pysha3/__init__.py`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/recipes/python3/__init__.py` & `python-for-android-2023.5.21/pythonforandroid/recipes/python3/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,36 +52,38 @@
           and :mod:`~pythonforandroid.recipes.liblzma`
 
     .. versionchanged:: 0.6.0
         Refactored into class
         :class:`~pythonforandroid.python.GuestPythonRecipe`
     '''
 
-    version = '3.9.9'
+    version = '3.10.10'
     url = 'https://www.python.org/ftp/python/{version}/Python-{version}.tgz'
     name = 'python3'
 
     patches = [
         'patches/pyconfig_detection.patch',
         'patches/reproducible-buildinfo.diff',
 
         # Python 3.7.1
         ('patches/py3.7.1_fix-ctypes-util-find-library.patch', version_starts_with("3.7")),
         ('patches/py3.7.1_fix-zlib-version.patch', version_starts_with("3.7")),
 
         # Python 3.8.1 & 3.9.X
         ('patches/py3.8.1.patch', version_starts_with("3.8")),
-        ('patches/py3.8.1.patch', version_starts_with("3.9"))
+        ('patches/py3.8.1.patch', version_starts_with("3.9")),
+        ('patches/py3.8.1.patch', version_starts_with("3.10"))
     ]
 
     if shutil.which('lld') is not None:
         patches = patches + [
             ("patches/py3.7.1_fix_cortex_a8.patch", version_starts_with("3.7")),
             ("patches/py3.8.1_fix_cortex_a8.patch", version_starts_with("3.8")),
-            ("patches/py3.8.1_fix_cortex_a8.patch", version_starts_with("3.9"))
+            ("patches/py3.8.1_fix_cortex_a8.patch", version_starts_with("3.9")),
+            ("patches/py3.8.1_fix_cortex_a8.patch", version_starts_with("3.10"))
         ]
 
     depends = ['hostpython3', 'sqlite3', 'openssl', 'libffi']
     # those optional depends allow us to build python compression modules:
     #   - _bz2.so
     #   - _lzma.so
     opt_depends = ['libbz2', 'liblzma']
@@ -92,14 +94,15 @@
         '--build={android_build}',
         '--enable-shared',
         '--enable-ipv6',
         'ac_cv_file__dev_ptmx=yes',
         'ac_cv_file__dev_ptc=no',
         '--without-ensurepip',
         'ac_cv_little_endian_double=yes',
+        'ac_cv_header_sys_eventfd_h=no',
         '--prefix={prefix}',
         '--exec-prefix={exec_prefix}',
         '--enable-loadable-sqlite-extensions')
     '''The configure arguments needed to build the python recipe. Those are
     used in method :meth:`build_arch` (if not overwritten like python3's
     recipe does).
     '''
```

### Comparing `python-for-android-2023.2.10/pythonforandroid/recipes/python3/patches/py3.7.1_fix-zlib-version.patch` & `python-for-android-2023.5.21/pythonforandroid/recipes/python3/patches/py3.7.1_fix-zlib-version.patch`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/recipes/python3/patches/py3.7.1_fix_cortex_a8.patch` & `python-for-android-2023.5.21/pythonforandroid/recipes/python3/patches/py3.7.1_fix_cortex_a8.patch`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/recipes/python3/patches/py3.8.1.patch` & `python-for-android-2023.5.21/pythonforandroid/recipes/python3/patches/py3.8.1.patch`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/recipes/python3/patches/py3.8.1_fix_cortex_a8.patch` & `python-for-android-2023.5.21/pythonforandroid/recipes/python3/patches/py3.8.1_fix_cortex_a8.patch`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/recipes/python3/patches/pyconfig_detection.patch` & `python-for-android-2023.5.21/pythonforandroid/recipes/python3/patches/pyconfig_detection.patch`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/recipes/python3/patches/reproducible-buildinfo.diff` & `python-for-android-2023.5.21/pythonforandroid/recipes/python3/patches/reproducible-buildinfo.diff`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/recipes/pyusb/fix-android.patch` & `python-for-android-2023.5.21/pythonforandroid/recipes/pyusb/fix-android.patch`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/recipes/pyzbar/__init__.py` & `python-for-android-2023.5.21/pythonforandroid/recipes/pyzbar/__init__.py`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/recipes/pyzmq/__init__.py` & `python-for-android-2023.5.21/pythonforandroid/recipes/pyzmq/__init__.py`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/recipes/reportlab/__init__.py` & `python-for-android-2023.5.21/pythonforandroid/recipes/reportlab/__init__.py`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/recipes/reportlab/patches/fix-setup.patch` & `python-for-android-2023.5.21/pythonforandroid/recipes/reportlab/patches/fix-setup.patch`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/recipes/ruamel.yaml/disable-pip-req.patch` & `python-for-android-2023.5.21/pythonforandroid/recipes/ruamel.yaml/disable-pip-req.patch`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/recipes/scipy/__init__.py` & `python-for-android-2023.5.21/pythonforandroid/recipes/scipy/__init__.py`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/recipes/scrypt/__init__.py` & `python-for-android-2023.5.21/pythonforandroid/recipes/scrypt/__init__.py`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/recipes/scrypt/remove_librt.patch` & `python-for-android-2023.5.21/pythonforandroid/recipes/scrypt/remove_librt.patch`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/recipes/sdl2/__init__.py` & `python-for-android-2023.5.21/pythonforandroid/recipes/sdl2/__init__.py`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/recipes/sdl2/sdl-orientation-pr-6984.diff` & `python-for-android-2023.5.21/pythonforandroid/recipes/sdl2/sdl-orientation-pr-6984.diff`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/recipes/sdl2_image/__init__.py` & `python-for-android-2023.5.21/pythonforandroid/recipes/sdl2_image/__init__.py`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/recipes/secp256k1/__init__.py` & `python-for-android-2023.5.21/pythonforandroid/recipes/secp256k1/__init__.py`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/recipes/secp256k1/pkg-config.patch` & `python-for-android-2023.5.21/pythonforandroid/recipes/secp256k1/pkg-config.patch`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/recipes/shapely/__init__.py` & `python-for-android-2023.5.21/pythonforandroid/recipes/shapely/__init__.py`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/recipes/shapely/setup.patch` & `python-for-android-2023.5.21/pythonforandroid/recipes/shapely/setup.patch`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/recipes/snappy/__init__.py` & `python-for-android-2023.5.21/pythonforandroid/recipes/snappy/__init__.py`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/recipes/sqlite3/__init__.py` & `python-for-android-2023.5.21/pythonforandroid/recipes/sqlite3/__init__.py`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/recipes/storm/__init__.py` & `python-for-android-2023.5.21/pythonforandroid/recipes/storm/__init__.py`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/recipes/sympy/fix_android_detection.patch` & `python-for-android-2023.5.21/pythonforandroid/recipes/sympy/fix_android_detection.patch`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/recipes/sympy/fix_pretty_print.patch` & `python-for-android-2023.5.21/pythonforandroid/recipes/sympy/fix_pretty_print.patch`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/recipes/tflite-runtime/CMakeLists.patch` & `python-for-android-2023.5.21/pythonforandroid/recipes/tflite-runtime/CMakeLists.patch`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/recipes/tflite-runtime/__init__.py` & `python-for-android-2023.5.21/pythonforandroid/recipes/tflite-runtime/__init__.py`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/recipes/tflite-runtime/build_with_cmake.patch` & `python-for-android-2023.5.21/pythonforandroid/recipes/tflite-runtime/build_with_cmake.patch`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/recipes/twisted/__init__.py` & `python-for-android-2023.5.21/pythonforandroid/recipes/twisted/__init__.py`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/recipes/twisted/incremental.patch` & `python-for-android-2023.5.21/pythonforandroid/recipes/twisted/incremental.patch`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/recipes/twisted/remove_tests.patch` & `python-for-android-2023.5.21/pythonforandroid/recipes/twisted/remove_tests.patch`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/recipes/vispy/disable_font_triage.patch` & `python-for-android-2023.5.21/pythonforandroid/recipes/vispy/disable_font_triage.patch`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/recipes/vispy/disable_freetype.patch` & `python-for-android-2023.5.21/pythonforandroid/recipes/vispy/disable_freetype.patch`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/recipes/vispy/remove_ati_check.patch` & `python-for-android-2023.5.21/pythonforandroid/recipes/vispy/remove_ati_check.patch`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/recipes/vlc/__init__.py` & `python-for-android-2023.5.21/pythonforandroid/recipes/vlc/__init__.py`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/recipes/xeddsa/__init__.py` & `python-for-android-2023.5.21/pythonforandroid/recipes/xeddsa/__init__.py`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/recipes/xeddsa/remove_dependencies.patch` & `python-for-android-2023.5.21/pythonforandroid/recipes/xeddsa/remove_dependencies.patch`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/recipes/zbar/__init__.py` & `python-for-android-2023.5.21/pythonforandroid/recipes/zbar/__init__.py`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/recipes/zbar/zbar-0.10-python-crash.patch` & `python-for-android-2023.5.21/pythonforandroid/recipes/zbar/zbar-0.10-python-crash.patch`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/recipes/zbarlight/__init__.py` & `python-for-android-2023.5.21/pythonforandroid/recipes/zbarlight/__init__.py`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/recipes/zeroconf/patches/setup.patch` & `python-for-android-2023.5.21/pythonforandroid/recipes/zeroconf/patches/setup.patch`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/recipes/zope/__init__.py` & `python-for-android-2023.5.21/pythonforandroid/recipes/zope/__init__.py`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/recipes/zope_interface/__init__.py` & `python-for-android-2023.5.21/pythonforandroid/recipes/zope_interface/__init__.py`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/recommendations.py` & `python-for-android-2023.5.21/pythonforandroid/recommendations.py`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/toolchain.py` & `python-for-android-2023.5.21/pythonforandroid/toolchain.py`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/tools/biglink` & `python-for-android-2023.5.21/pythonforandroid/tools/biglink`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/pythonforandroid/tools/liblink` & `python-for-android-2023.5.21/pythonforandroid/tools/liblink`

 * *Files 10% similar despite different names*

```diff
@@ -31,14 +31,15 @@
     if opt in ("--sysroot", "-isysroot", "-framework", "-undefined",
             "-macosx_version_min"):
         i += 1
         continue
 
     if opt.startswith(
             ("-I", "-isystem", "-m", "-f", "-O", "-g", "-D", "-R")):
+        continue
 
     if opt.startswith("-"):
         print(sys.argv)
         print("Unknown option: %s" % opt)
         sys.exit(1)
 
     if not opt.endswith('.o'):
```

### Comparing `python-for-android-2023.2.10/pythonforandroid/util.py` & `python-for-android-2023.5.21/pythonforandroid/util.py`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/setup.py` & `python-for-android-2023.5.21/setup.py`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/tests/test_androidmodule_ctypes_finder.py` & `python-for-android-2023.5.21/tests/test_androidmodule_ctypes_finder.py`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/tests/test_androidndk.py` & `python-for-android-2023.5.21/tests/test_androidndk.py`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/tests/test_archs.py` & `python-for-android-2023.5.21/tests/test_archs.py`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/tests/test_bootstrap.py` & `python-for-android-2023.5.21/tests/test_bootstrap.py`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/tests/test_bootstrap_build.py` & `python-for-android-2023.5.21/tests/test_bootstrap_build.py`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/tests/test_build.py` & `python-for-android-2023.5.21/tests/test_build.py`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/tests/test_distribution.py` & `python-for-android-2023.5.21/tests/test_distribution.py`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/tests/test_graph.py` & `python-for-android-2023.5.21/tests/test_graph.py`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/tests/test_logger.py` & `python-for-android-2023.5.21/tests/test_logger.py`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/tests/test_prerequisites.py` & `python-for-android-2023.5.21/tests/test_prerequisites.py`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/tests/test_pythonpackage.py` & `python-for-android-2023.5.21/tests/test_pythonpackage.py`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/tests/test_pythonpackage_basic.py` & `python-for-android-2023.5.21/tests/test_pythonpackage_basic.py`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/tests/test_recipe.py` & `python-for-android-2023.5.21/tests/test_recipe.py`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/tests/test_recommendations.py` & `python-for-android-2023.5.21/tests/test_recommendations.py`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/tests/test_toolchain.py` & `python-for-android-2023.5.21/tests/test_toolchain.py`

 * *Files identical despite different names*

### Comparing `python-for-android-2023.2.10/tests/test_util.py` & `python-for-android-2023.5.21/tests/test_util.py`

 * *Files identical despite different names*

