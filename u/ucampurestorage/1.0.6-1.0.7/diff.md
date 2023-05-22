# Comparing `tmp/ucampurestorage-1.0.6.tar.gz` & `tmp/ucampurestorage-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ucampurestorage-1.0.6.tar", last modified: Sat May 20 02:18:08 2023, max compression
+gzip compressed data, was "ucampurestorage-1.0.7.tar", last modified: Mon May 22 00:25:55 2023, max compression
```

## Comparing `ucampurestorage-1.0.6.tar` & `ucampurestorage-1.0.7.tar`

### file list

```diff
@@ -1,167 +1,26 @@
-drwxrwxr-x   0 im        (1000) im        (1000)        0 2023-05-20 02:18:08.553928 ucampurestorage-1.0.6/
--rw-rw-r--   0 im        (1000) im        (1000)       62 2023-05-20 01:36:26.000000 ucampurestorage-1.0.6/.coveragerc
--rw-rw-r--   0 im        (1000) im        (1000)       64 2023-05-20 01:36:26.000000 ucampurestorage-1.0.6/.flake8
--rw-rw-r--   0 im        (1000) im        (1000)      581 2023-05-20 01:36:26.000000 ucampurestorage-1.0.6/.gitignore
--rw-rw-r--   0 im        (1000) im        (1000)     1403 2023-05-20 01:36:26.000000 ucampurestorage-1.0.6/.gitlab-ci.yml
--rw-rw-r--   0 im        (1000) im        (1000)      107 2023-05-20 01:36:26.000000 ucampurestorage-1.0.6/Dockerfile
--rw-rw-r--   0 im        (1000) im        (1000)     1094 2023-05-20 01:36:26.000000 ucampurestorage-1.0.6/LICENSE
--rw-rw-r--   0 im        (1000) im        (1000)    20061 2023-05-20 02:18:08.553928 ucampurestorage-1.0.6/PKG-INFO
--rw-rw-r--   0 im        (1000) im        (1000)    19690 2023-05-20 01:36:26.000000 ucampurestorage-1.0.6/README.md
-drwxrwxr-x   0 im        (1000) im        (1000)        0 2023-05-20 02:18:08.129932 ucampurestorage-1.0.6/compose/
--rw-rw-r--   0 im        (1000) im        (1000)      503 2023-05-20 01:36:26.000000 ucampurestorage-1.0.6/compose/docs.Dockerfile
--rw-rw-r--   0 im        (1000) im        (1000)      270 2023-05-20 01:36:26.000000 ucampurestorage-1.0.6/compose/docs.yml
--rw-rw-r--   0 im        (1000) im        (1000)       73 2023-05-20 01:36:26.000000 ucampurestorage-1.0.6/compose/docs_http.Dockerfile
--rw-rw-r--   0 im        (1000) im        (1000)      174 2023-05-20 01:36:26.000000 ucampurestorage-1.0.6/compose/pytest.Dockerfile
--rw-rw-r--   0 im        (1000) im        (1000)      172 2023-05-20 01:36:26.000000 ucampurestorage-1.0.6/compose/tox.Dockerfile
--rw-rw-r--   0 im        (1000) im        (1000)      161 2023-05-20 01:36:26.000000 ucampurestorage-1.0.6/compose/tox.env
--rw-rw-r--   0 im        (1000) im        (1000)      367 2023-05-20 01:36:26.000000 ucampurestorage-1.0.6/compose/tox.yml
-drwxrwxr-x   0 im        (1000) im        (1000)        0 2023-05-20 02:18:08.169931 ucampurestorage-1.0.6/docs/
--rw-rw-r--   0 im        (1000) im        (1000)      634 2023-05-20 01:36:26.000000 ucampurestorage-1.0.6/docs/Makefile
--rw-rw-r--   0 im        (1000) im        (1000)    20154 2023-05-20 01:36:26.000000 ucampurestorage-1.0.6/docs/README.rst
-drwxrwxr-x   0 im        (1000) im        (1000)        0 2023-05-20 02:18:07.989933 ucampurestorage-1.0.6/docs/_build/
-drwxrwxr-x   0 im        (1000) im        (1000)        0 2023-05-20 02:18:08.205931 ucampurestorage-1.0.6/docs/_build/doctrees/
--rw-rw-r--   0 im        (1000) im        (1000)     7261 2023-05-20 01:36:26.000000 ucampurestorage-1.0.6/docs/_build/doctrees/changelog.doctree
--rw-rw-r--   0 im        (1000) im        (1000)   217803 2023-05-20 01:36:26.000000 ucampurestorage-1.0.6/docs/_build/doctrees/environment.pickle
--rw-rw-r--   0 im        (1000) im        (1000)     5361 2023-05-20 01:36:26.000000 ucampurestorage-1.0.6/docs/_build/doctrees/index.doctree
--rw-rw-r--   0 im        (1000) im        (1000)     2774 2023-05-20 01:36:26.000000 ucampurestorage-1.0.6/docs/_build/doctrees/modules.doctree
--rw-rw-r--   0 im        (1000) im        (1000)    47975 2023-05-20 01:36:26.000000 ucampurestorage-1.0.6/docs/_build/doctrees/readme.doctree
--rw-rw-r--   0 im        (1000) im        (1000)     3364 2023-05-20 01:36:26.000000 ucampurestorage-1.0.6/docs/_build/doctrees/readme_link.doctree
--rw-rw-r--   0 im        (1000) im        (1000)     4245 2023-05-20 01:36:26.000000 ucampurestorage-1.0.6/docs/_build/doctrees/ucampurestorage.doctree
--rw-rw-r--   0 im        (1000) im        (1000)   392846 2023-05-20 01:36:26.000000 ucampurestorage-1.0.6/docs/_build/doctrees/ucampurestorage.lib.doctree
--rw-rw-r--   0 im        (1000) im        (1000)    82637 2023-05-20 01:36:26.000000 ucampurestorage-1.0.6/docs/_build/doctrees/ucampurestorage.tests.doctree
-drwxrwxr-x   0 im        (1000) im        (1000)        0 2023-05-20 02:18:08.257930 ucampurestorage-1.0.6/docs/_build/html/
--rw-rw-r--   0 im        (1000) im        (1000)      230 2023-05-20 01:36:26.000000 ucampurestorage-1.0.6/docs/_build/html/.buildinfo
-drwxrwxr-x   0 im        (1000) im        (1000)        0 2023-05-20 02:18:08.265930 ucampurestorage-1.0.6/docs/_build/html/_images/
--rw-rw-r--   0 im        (1000) im        (1000)   127824 2023-05-20 01:36:26.000000 ucampurestorage-1.0.6/docs/_build/html/_images/pure_storage.jpg
--rw-rw-r--   0 im        (1000) im        (1000)   127824 2023-05-20 01:36:26.000000 ucampurestorage-1.0.6/docs/_build/html/_images/pure_storage1.jpg
-drwxrwxr-x   0 im        (1000) im        (1000)        0 2023-05-20 02:18:08.269930 ucampurestorage-1.0.6/docs/_build/html/_modules/
--rw-rw-r--   0 im        (1000) im        (1000)     4473 2023-05-20 01:36:26.000000 ucampurestorage-1.0.6/docs/_build/html/_modules/index.html
-drwxrwxr-x   0 im        (1000) im        (1000)        0 2023-05-20 02:18:08.009933 ucampurestorage-1.0.6/docs/_build/html/_modules/ucampurestorage/
-drwxrwxr-x   0 im        (1000) im        (1000)        0 2023-05-20 02:18:08.293930 ucampurestorage-1.0.6/docs/_build/html/_modules/ucampurestorage/lib/
--rw-rw-r--   0 im        (1000) im        (1000)    17027 2023-05-20 01:36:26.000000 ucampurestorage-1.0.6/docs/_build/html/_modules/ucampurestorage/lib/httpclient.html
--rw-rw-r--   0 im        (1000) im        (1000)   162036 2023-05-20 01:36:26.000000 ucampurestorage-1.0.6/docs/_build/html/_modules/ucampurestorage/lib/options.html
--rw-rw-r--   0 im        (1000) im        (1000)   110228 2023-05-20 01:36:26.000000 ucampurestorage-1.0.6/docs/_build/html/_modules/ucampurestorage/lib/process.html
--rw-rw-r--   0 im        (1000) im        (1000)   230414 2023-05-20 01:36:26.000000 ucampurestorage-1.0.6/docs/_build/html/_modules/ucampurestorage/lib/pureconnect.html
--rw-rw-r--   0 im        (1000) im        (1000)    27634 2023-05-20 01:36:26.000000 ucampurestorage-1.0.6/docs/_build/html/_modules/ucampurestorage/lib/tokencreater.html
-drwxrwxr-x   0 im        (1000) im        (1000)        0 2023-05-20 02:18:08.309930 ucampurestorage-1.0.6/docs/_build/html/_modules/ucampurestorage/tests/
--rw-rw-r--   0 im        (1000) im        (1000)     7825 2023-05-20 01:36:26.000000 ucampurestorage-1.0.6/docs/_build/html/_modules/ucampurestorage/tests/test_httpclient.html
--rw-rw-r--   0 im        (1000) im        (1000)    39634 2023-05-20 01:36:26.000000 ucampurestorage-1.0.6/docs/_build/html/_modules/ucampurestorage/tests/test_process.html
--rw-rw-r--   0 im        (1000) im        (1000)    20339 2023-05-20 01:36:26.000000 ucampurestorage-1.0.6/docs/_build/html/_modules/ucampurestorage/tests/test_pureconnection.html
--rw-rw-r--   0 im        (1000) im        (1000)    13133 2023-05-20 01:36:26.000000 ucampurestorage-1.0.6/docs/_build/html/_modules/ucampurestorage/tests/test_tokencreater.html
-drwxrwxr-x   0 im        (1000) im        (1000)        0 2023-05-20 02:18:08.321930 ucampurestorage-1.0.6/docs/_build/html/_sources/
--rw-rw-r--   0 im        (1000) im        (1000)      425 2023-05-20 01:36:26.000000 ucampurestorage-1.0.6/docs/_build/html/_sources/changelog.rst.txt
--rw-rw-r--   0 im        (1000) im        (1000)      568 2023-05-20 01:36:26.000000 ucampurestorage-1.0.6/docs/_build/html/_sources/index.rst.txt
--rw-rw-r--   0 im        (1000) im        (1000)       82 2023-05-20 01:36:26.000000 ucampurestorage-1.0.6/docs/_build/html/_sources/modules.rst.txt
--rw-rw-r--   0 im        (1000) im        (1000)    20154 2023-05-20 01:36:26.000000 ucampurestorage-1.0.6/docs/_build/html/_sources/readme.rst.txt
--rw-rw-r--   0 im        (1000) im        (1000)       52 2023-05-20 01:36:26.000000 ucampurestorage-1.0.6/docs/_build/html/_sources/readme_link.rst.txt
--rw-rw-r--   0 im        (1000) im        (1000)     1089 2023-05-20 01:36:26.000000 ucampurestorage-1.0.6/docs/_build/html/_sources/ucampurestorage.lib.rst.txt
--rw-rw-r--   0 im        (1000) im        (1000)      272 2023-05-20 01:36:26.000000 ucampurestorage-1.0.6/docs/_build/html/_sources/ucampurestorage.rst.txt
--rw-rw-r--   0 im        (1000) im        (1000)     1213 2023-05-20 01:36:26.000000 ucampurestorage-1.0.6/docs/_build/html/_sources/ucampurestorage.tests.rst.txt
-drwxrwxr-x   0 im        (1000) im        (1000)        0 2023-05-20 02:18:08.393929 ucampurestorage-1.0.6/docs/_build/html/_static/
--rw-rw-r--   0 im        (1000) im        (1000)    14692 2023-05-20 01:36:26.000000 ucampurestorage-1.0.6/docs/_build/html/_static/basic.css
-drwxrwxr-x   0 im        (1000) im        (1000)        0 2023-05-20 02:18:08.405929 ucampurestorage-1.0.6/docs/_build/html/_static/css/
--rw-rw-r--   0 im        (1000) im        (1000)     3229 2023-05-20 01:36:26.000000 ucampurestorage-1.0.6/docs/_build/html/_static/css/badge_only.css
-drwxrwxr-x   0 im        (1000) im        (1000)        0 2023-05-20 02:18:08.481928 ucampurestorage-1.0.6/docs/_build/html/_static/css/fonts/
--rw-rw-r--   0 im        (1000) im        (1000)    87624 2023-05-20 01:36:27.000000 ucampurestorage-1.0.6/docs/_build/html/_static/css/fonts/Roboto-Slab-Bold.woff
--rw-rw-r--   0 im        (1000) im        (1000)    67312 2023-05-20 01:36:27.000000 ucampurestorage-1.0.6/docs/_build/html/_static/css/fonts/Roboto-Slab-Bold.woff2
--rw-rw-r--   0 im        (1000) im        (1000)    86288 2023-05-20 01:36:27.000000 ucampurestorage-1.0.6/docs/_build/html/_static/css/fonts/Roboto-Slab-Regular.woff
--rw-rw-r--   0 im        (1000) im        (1000)    66444 2023-05-20 01:36:27.000000 ucampurestorage-1.0.6/docs/_build/html/_static/css/fonts/Roboto-Slab-Regular.woff2
--rw-rw-r--   0 im        (1000) im        (1000)   165742 2023-05-20 01:36:27.000000 ucampurestorage-1.0.6/docs/_build/html/_static/css/fonts/fontawesome-webfont.eot
--rw-rw-r--   0 im        (1000) im        (1000)   444379 2023-05-20 01:36:27.000000 ucampurestorage-1.0.6/docs/_build/html/_static/css/fonts/fontawesome-webfont.svg
--rw-rw-r--   0 im        (1000) im        (1000)   165548 2023-05-20 01:36:27.000000 ucampurestorage-1.0.6/docs/_build/html/_static/css/fonts/fontawesome-webfont.ttf
--rw-rw-r--   0 im        (1000) im        (1000)    98024 2023-05-20 01:36:27.000000 ucampurestorage-1.0.6/docs/_build/html/_static/css/fonts/fontawesome-webfont.woff
--rw-rw-r--   0 im        (1000) im        (1000)    77160 2023-05-20 01:36:27.000000 ucampurestorage-1.0.6/docs/_build/html/_static/css/fonts/fontawesome-webfont.woff2
--rw-rw-r--   0 im        (1000) im        (1000)   323344 2023-05-20 01:36:27.000000 ucampurestorage-1.0.6/docs/_build/html/_static/css/fonts/lato-bold-italic.woff
--rw-rw-r--   0 im        (1000) im        (1000)   193308 2023-05-20 01:36:27.000000 ucampurestorage-1.0.6/docs/_build/html/_static/css/fonts/lato-bold-italic.woff2
--rw-rw-r--   0 im        (1000) im        (1000)   309728 2023-05-20 01:36:27.000000 ucampurestorage-1.0.6/docs/_build/html/_static/css/fonts/lato-bold.woff
--rw-rw-r--   0 im        (1000) im        (1000)   184912 2023-05-20 01:36:27.000000 ucampurestorage-1.0.6/docs/_build/html/_static/css/fonts/lato-bold.woff2
--rw-rw-r--   0 im        (1000) im        (1000)   328412 2023-05-20 01:36:27.000000 ucampurestorage-1.0.6/docs/_build/html/_static/css/fonts/lato-normal-italic.woff
--rw-rw-r--   0 im        (1000) im        (1000)   195704 2023-05-20 01:36:27.000000 ucampurestorage-1.0.6/docs/_build/html/_static/css/fonts/lato-normal-italic.woff2
--rw-rw-r--   0 im        (1000) im        (1000)   309192 2023-05-20 01:36:27.000000 ucampurestorage-1.0.6/docs/_build/html/_static/css/fonts/lato-normal.woff
--rw-rw-r--   0 im        (1000) im        (1000)   182708 2023-05-20 01:36:27.000000 ucampurestorage-1.0.6/docs/_build/html/_static/css/fonts/lato-normal.woff2
--rw-rw-r--   0 im        (1000) im        (1000)   135235 2023-05-20 01:36:27.000000 ucampurestorage-1.0.6/docs/_build/html/_static/css/theme.css
--rw-rw-r--   0 im        (1000) im        (1000)    10766 2023-05-20 01:36:27.000000 ucampurestorage-1.0.6/docs/_build/html/_static/doctools.js
--rw-rw-r--   0 im        (1000) im        (1000)      422 2023-05-20 01:36:27.000000 ucampurestorage-1.0.6/docs/_build/html/_static/documentation_options.js
--rw-rw-r--   0 im        (1000) im        (1000)      286 2023-05-20 01:36:27.000000 ucampurestorage-1.0.6/docs/_build/html/_static/file.png
--rw-rw-r--   0 im        (1000) im        (1000)   287630 2023-05-20 01:36:27.000000 ucampurestorage-1.0.6/docs/_build/html/_static/jquery-3.5.1.js
--rw-rw-r--   0 im        (1000) im        (1000)    89476 2023-05-20 01:36:27.000000 ucampurestorage-1.0.6/docs/_build/html/_static/jquery.js
-drwxrwxr-x   0 im        (1000) im        (1000)        0 2023-05-20 02:18:08.513928 ucampurestorage-1.0.6/docs/_build/html/_static/js/
--rw-rw-r--   0 im        (1000) im        (1000)      934 2023-05-20 01:36:27.000000 ucampurestorage-1.0.6/docs/_build/html/_static/js/badge_only.js
--rw-rw-r--   0 im        (1000) im        (1000)     4370 2023-05-20 01:36:27.000000 ucampurestorage-1.0.6/docs/_build/html/_static/js/html5shiv-printshiv.min.js
--rw-rw-r--   0 im        (1000) im        (1000)     2734 2023-05-20 01:36:27.000000 ucampurestorage-1.0.6/docs/_build/html/_static/js/html5shiv.min.js
--rw-rw-r--   0 im        (1000) im        (1000)     5023 2023-05-20 01:36:27.000000 ucampurestorage-1.0.6/docs/_build/html/_static/js/theme.js
--rw-rw-r--   0 im        (1000) im        (1000)    10854 2023-05-20 01:36:27.000000 ucampurestorage-1.0.6/docs/_build/html/_static/language_data.js
--rw-rw-r--   0 im        (1000) im        (1000)       90 2023-05-20 01:36:27.000000 ucampurestorage-1.0.6/docs/_build/html/_static/minus.png
--rw-rw-r--   0 im        (1000) im        (1000)     4467 2023-05-20 01:36:27.000000 ucampurestorage-1.0.6/docs/_build/html/_static/nbsphinx-broken-thumbnail.svg
--rw-rw-r--   0 im        (1000) im        (1000)     6625 2023-05-20 01:36:27.000000 ucampurestorage-1.0.6/docs/_build/html/_static/nbsphinx-code-cells.css
--rw-rw-r--   0 im        (1000) im        (1000)      584 2023-05-20 01:36:27.000000 ucampurestorage-1.0.6/docs/_build/html/_static/nbsphinx-gallery.css
--rw-rw-r--   0 im        (1000) im        (1000)     2871 2023-05-20 01:36:27.000000 ucampurestorage-1.0.6/docs/_build/html/_static/nbsphinx-no-thumbnail.svg
--rw-rw-r--   0 im        (1000) im        (1000)       90 2023-05-20 01:36:27.000000 ucampurestorage-1.0.6/docs/_build/html/_static/plus.png
--rw-rw-r--   0 im        (1000) im        (1000)     4819 2023-05-20 01:36:27.000000 ucampurestorage-1.0.6/docs/_build/html/_static/pygments.css
--rw-rw-r--   0 im        (1000) im        (1000)    16634 2023-05-20 01:36:27.000000 ucampurestorage-1.0.6/docs/_build/html/_static/searchtools.js
--rw-rw-r--   0 im        (1000) im        (1000)     4712 2023-05-20 01:36:27.000000 ucampurestorage-1.0.6/docs/_build/html/_static/sphinx_highlight.js
--rw-rw-r--   0 im        (1000) im        (1000)    68420 2023-05-20 01:36:27.000000 ucampurestorage-1.0.6/docs/_build/html/_static/underscore-1.13.1.js
--rw-rw-r--   0 im        (1000) im        (1000)    19530 2023-05-20 01:36:27.000000 ucampurestorage-1.0.6/docs/_build/html/_static/underscore.js
--rw-rw-r--   0 im        (1000) im        (1000)     5266 2023-05-20 01:36:27.000000 ucampurestorage-1.0.6/docs/_build/html/changelog.html
--rw-rw-r--   0 im        (1000) im        (1000)    39834 2023-05-20 01:36:27.000000 ucampurestorage-1.0.6/docs/_build/html/genindex.html
--rw-rw-r--   0 im        (1000) im        (1000)     6243 2023-05-20 01:36:27.000000 ucampurestorage-1.0.6/docs/_build/html/index.html
--rw-rw-r--   0 im        (1000) im        (1000)     7579 2023-05-20 01:36:27.000000 ucampurestorage-1.0.6/docs/_build/html/modules.html
--rw-rw-r--   0 im        (1000) im        (1000)     1660 2023-05-20 01:36:27.000000 ucampurestorage-1.0.6/docs/_build/html/objects.inv
--rw-rw-r--   0 im        (1000) im        (1000)     7107 2023-05-20 01:36:27.000000 ucampurestorage-1.0.6/docs/_build/html/py-modindex.html
--rw-rw-r--   0 im        (1000) im        (1000)    96267 2023-05-20 01:36:27.000000 ucampurestorage-1.0.6/docs/_build/html/readme.html
--rw-rw-r--   0 im        (1000) im        (1000)     3746 2023-05-20 01:36:27.000000 ucampurestorage-1.0.6/docs/_build/html/readme_link.html
--rw-rw-r--   0 im        (1000) im        (1000)     3918 2023-05-20 01:36:27.000000 ucampurestorage-1.0.6/docs/_build/html/search.html
--rw-rw-r--   0 im        (1000) im        (1000)    16441 2023-05-20 01:36:27.000000 ucampurestorage-1.0.6/docs/_build/html/searchindex.js
--rw-rw-r--   0 im        (1000) im        (1000)     8243 2023-05-20 01:36:27.000000 ucampurestorage-1.0.6/docs/_build/html/ucampurestorage.html
--rw-rw-r--   0 im        (1000) im        (1000)   140493 2023-05-20 01:36:27.000000 ucampurestorage-1.0.6/docs/_build/html/ucampurestorage.lib.html
--rw-rw-r--   0 im        (1000) im        (1000)    44645 2023-05-20 01:36:27.000000 ucampurestorage-1.0.6/docs/_build/html/ucampurestorage.tests.html
--rw-rw-r--   0 im        (1000) im        (1000)      425 2023-05-20 02:17:39.000000 ucampurestorage-1.0.6/docs/changelog.rst
--rw-rw-r--   0 im        (1000) im        (1000)     1118 2023-05-20 01:36:27.000000 ucampurestorage-1.0.6/docs/conf.py
--rw-rw-r--   0 im        (1000) im        (1000)      568 2023-05-20 01:36:27.000000 ucampurestorage-1.0.6/docs/index.rst
--rw-rw-r--   0 im        (1000) im        (1000)      765 2023-05-20 01:36:27.000000 ucampurestorage-1.0.6/docs/make.bat
--rw-rw-r--   0 im        (1000) im        (1000)       82 2023-05-20 01:36:27.000000 ucampurestorage-1.0.6/docs/modules.rst
--rw-rw-r--   0 im        (1000) im        (1000)   127824 2023-05-20 01:36:27.000000 ucampurestorage-1.0.6/docs/pure_storage.jpg
--rw-rw-r--   0 im        (1000) im        (1000)     1089 2023-05-20 01:36:27.000000 ucampurestorage-1.0.6/docs/ucampurestorage.lib.rst
--rw-rw-r--   0 im        (1000) im        (1000)      272 2023-05-20 01:36:27.000000 ucampurestorage-1.0.6/docs/ucampurestorage.rst
--rw-rw-r--   0 im        (1000) im        (1000)     1213 2023-05-20 01:36:27.000000 ucampurestorage-1.0.6/docs/ucampurestorage.tests.rst
--rw-rw-r--   0 im        (1000) im        (1000)   127824 2023-05-20 01:36:27.000000 ucampurestorage-1.0.6/pure_storage.jpg
--rw-rw-r--   0 im        (1000) im        (1000)     1331 2023-05-20 01:55:11.000000 ucampurestorage-1.0.6/pyproject.toml
--rw-rw-r--   0 im        (1000) im        (1000)      119 2023-05-20 01:36:27.000000 ucampurestorage-1.0.6/requirements-dev.txt
--rw-rw-r--   0 im        (1000) im        (1000)       60 2023-05-20 01:36:27.000000 ucampurestorage-1.0.6/requirements.txt
--rw-rw-r--   0 im        (1000) im        (1000)       38 2023-05-20 02:18:08.553928 ucampurestorage-1.0.6/setup.cfg
--rw-rw-r--   0 im        (1000) im        (1000)      666 2023-05-20 01:36:27.000000 ucampurestorage-1.0.6/tox.ini
-drwxrwxr-x   0 im        (1000) im        (1000)        0 2023-05-20 02:18:08.541928 ucampurestorage-1.0.6/ucampurecli/
--rw-rw-r--   0 im        (1000) im        (1000)     2391 2023-05-20 01:36:27.000000 ucampurestorage-1.0.6/ucampurecli/README.md
--rwxrwxr-x   0 im        (1000) im        (1000)     2419 2023-05-20 01:36:27.000000 ucampurestorage-1.0.6/ucampurecli/pure_clone_volume
--rwxrwxr-x   0 im        (1000) im        (1000)     2859 2023-05-20 01:36:27.000000 ucampurestorage-1.0.6/ucampurecli/pure_create_snapshot
--rwxrwxr-x   0 im        (1000) im        (1000)     2442 2023-05-20 01:36:27.000000 ucampurestorage-1.0.6/ucampurecli/pure_create_volume
--rwxrwxr-x   0 im        (1000) im        (1000)     2080 2023-05-20 01:36:27.000000 ucampurestorage-1.0.6/ucampurecli/pure_delete_volume
--rwxrwxr-x   0 im        (1000) im        (1000)     4851 2023-05-20 01:36:27.000000 ucampurestorage-1.0.6/ucampurecli/pure_eradicate_destroyed_volume
--rwxrwxr-x   0 im        (1000) im        (1000)     2818 2023-05-20 01:36:27.000000 ucampurestorage-1.0.6/ucampurecli/pure_map_volume
--rwxrwxr-x   0 im        (1000) im        (1000)     2015 2023-05-20 01:36:27.000000 ucampurestorage-1.0.6/ucampurecli/pure_record_destoyed_volume
--rwxrwxr-x   0 im        (1000) im        (1000)     3164 2023-05-20 01:36:27.000000 ucampurestorage-1.0.6/ucampurecli/pure_replace_volume
--rwxrwxr-x   0 im        (1000) im        (1000)     2081 2023-05-20 01:36:27.000000 ucampurestorage-1.0.6/ucampurecli/pure_unmap_volume
-drwxrwxr-x   0 im        (1000) im        (1000)        0 2023-05-20 02:18:08.545928 ucampurestorage-1.0.6/ucampurestorage/
--rw-rw-r--   0 im        (1000) im        (1000)       77 2023-05-20 02:17:53.000000 ucampurestorage-1.0.6/ucampurestorage/__init__.py
--rw-rw-r--   0 im        (1000) im        (1000)     1384 2023-05-20 01:36:27.000000 ucampurestorage-1.0.6/ucampurestorage/__main__.py
-drwxrwxr-x   0 im        (1000) im        (1000)        0 2023-05-20 02:18:08.553928 ucampurestorage-1.0.6/ucampurestorage/lib/
--rw-rw-r--   0 im        (1000) im        (1000)        0 2023-05-20 01:36:27.000000 ucampurestorage-1.0.6/ucampurestorage/lib/__init__.py
--rw-rw-r--   0 im        (1000) im        (1000)     2578 2023-05-20 01:36:27.000000 ucampurestorage-1.0.6/ucampurestorage/lib/httpclient.py
--rw-rw-r--   0 im        (1000) im        (1000)    41551 2023-05-20 01:36:27.000000 ucampurestorage-1.0.6/ucampurestorage/lib/options.py
--rw-rw-r--   0 im        (1000) im        (1000)    24787 2023-05-20 01:36:27.000000 ucampurestorage-1.0.6/ucampurestorage/lib/process.py
--rw-rw-r--   0 im        (1000) im        (1000)    50375 2023-05-20 01:36:27.000000 ucampurestorage-1.0.6/ucampurestorage/lib/pureconnect.py
--rw-rw-r--   0 im        (1000) im        (1000)     6044 2023-05-20 01:36:27.000000 ucampurestorage-1.0.6/ucampurestorage/lib/tokencreater.py
-drwxrwxr-x   0 im        (1000) im        (1000)        0 2023-05-20 02:18:08.553928 ucampurestorage-1.0.6/ucampurestorage/tests/
--rw-rw-r--   0 im        (1000) im        (1000)        0 2023-05-20 01:36:27.000000 ucampurestorage-1.0.6/ucampurestorage/tests/__init__.py
--rw-rw-r--   0 im        (1000) im        (1000)      699 2023-05-20 01:36:27.000000 ucampurestorage-1.0.6/ucampurestorage/tests/test_httpclient.py
--rw-rw-r--   0 im        (1000) im        (1000)     6950 2023-05-20 01:36:27.000000 ucampurestorage-1.0.6/ucampurestorage/tests/test_process.py
--rw-rw-r--   0 im        (1000) im        (1000)     3321 2023-05-20 01:36:27.000000 ucampurestorage-1.0.6/ucampurestorage/tests/test_pureconnection.py
--rw-rw-r--   0 im        (1000) im        (1000)        0 2023-05-20 01:36:27.000000 ucampurestorage-1.0.6/ucampurestorage/tests/test_tasks.py
--rw-rw-r--   0 im        (1000) im        (1000)     2189 2023-05-20 01:36:27.000000 ucampurestorage-1.0.6/ucampurestorage/tests/test_tokencreater.py
-drwxrwxr-x   0 im        (1000) im        (1000)        0 2023-05-20 02:18:08.553928 ucampurestorage-1.0.6/ucampurestorage.egg-info/
--rw-rw-r--   0 im        (1000) im        (1000)    20061 2023-05-20 02:18:07.000000 ucampurestorage-1.0.6/ucampurestorage.egg-info/PKG-INFO
--rw-rw-r--   0 im        (1000) im        (1000)     5469 2023-05-20 02:18:07.000000 ucampurestorage-1.0.6/ucampurestorage.egg-info/SOURCES.txt
--rw-rw-r--   0 im        (1000) im        (1000)        1 2023-05-20 02:18:07.000000 ucampurestorage-1.0.6/ucampurestorage.egg-info/dependency_links.txt
--rw-rw-r--   0 im        (1000) im        (1000)       66 2023-05-20 02:18:07.000000 ucampurestorage-1.0.6/ucampurestorage.egg-info/entry_points.txt
--rw-rw-r--   0 im        (1000) im        (1000)      109 2023-05-20 02:18:07.000000 ucampurestorage-1.0.6/ucampurestorage.egg-info/requires.txt
--rw-rw-r--   0 im        (1000) im        (1000)       16 2023-05-20 02:18:07.000000 ucampurestorage-1.0.6/ucampurestorage.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 00:25:55.780921 ucampurestorage-1.0.7/
+-rw-rw-r--   0 root         (0) root         (0)     1094 2023-05-22 00:08:34.000000 ucampurestorage-1.0.7/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    20061 2023-05-22 00:25:55.768921 ucampurestorage-1.0.7/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)    19690 2023-05-22 00:08:34.000000 ucampurestorage-1.0.7/README.md
+-rw-rw-r--   0 root         (0) root         (0)     1331 2023-05-22 00:08:34.000000 ucampurestorage-1.0.7/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-22 00:25:55.780921 ucampurestorage-1.0.7/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 00:25:55.736921 ucampurestorage-1.0.7/ucampurecli/
+-rwxrwxr-x   0 root         (0) root         (0)     2419 2023-05-22 00:08:34.000000 ucampurestorage-1.0.7/ucampurecli/pure_clone_volume
+-rwxrwxr-x   0 root         (0) root         (0)     2859 2023-05-22 00:08:34.000000 ucampurestorage-1.0.7/ucampurecli/pure_create_snapshot
+-rwxrwxr-x   0 root         (0) root         (0)     2442 2023-05-22 00:08:34.000000 ucampurestorage-1.0.7/ucampurecli/pure_create_volume
+-rwxrwxr-x   0 root         (0) root         (0)     2080 2023-05-22 00:08:34.000000 ucampurestorage-1.0.7/ucampurecli/pure_delete_volume
+-rwxrwxr-x   0 root         (0) root         (0)     4851 2023-05-22 00:08:34.000000 ucampurestorage-1.0.7/ucampurecli/pure_eradicate_destroyed_volume
+-rwxrwxr-x   0 root         (0) root         (0)     2822 2023-05-22 00:08:34.000000 ucampurestorage-1.0.7/ucampurecli/pure_map_volume
+-rwxrwxr-x   0 root         (0) root         (0)     2015 2023-05-22 00:08:34.000000 ucampurestorage-1.0.7/ucampurecli/pure_record_destoyed_volume
+-rwxrwxr-x   0 root         (0) root         (0)     3164 2023-05-22 00:08:34.000000 ucampurestorage-1.0.7/ucampurecli/pure_replace_volume
+-rwxrwxr-x   0 root         (0) root         (0)     2559 2023-05-22 00:08:34.000000 ucampurestorage-1.0.7/ucampurecli/pure_unmap_volume
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 00:25:55.740921 ucampurestorage-1.0.7/ucampurestorage/
+-rw-rw-r--   0 root         (0) root         (0)       77 2023-05-22 00:21:13.000000 ucampurestorage-1.0.7/ucampurestorage/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     1384 2023-05-22 00:08:34.000000 ucampurestorage-1.0.7/ucampurestorage/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 00:25:55.748921 ucampurestorage-1.0.7/ucampurestorage.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    20061 2023-05-22 00:25:55.000000 ucampurestorage-1.0.7/ucampurestorage.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      623 2023-05-22 00:25:55.000000 ucampurestorage-1.0.7/ucampurestorage.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-22 00:25:55.000000 ucampurestorage-1.0.7/ucampurestorage.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       66 2023-05-22 00:25:55.000000 ucampurestorage-1.0.7/ucampurestorage.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      109 2023-05-22 00:25:55.000000 ucampurestorage-1.0.7/ucampurestorage.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2023-05-22 00:25:55.000000 ucampurestorage-1.0.7/ucampurestorage.egg-info/top_level.txt
```

### Comparing `ucampurestorage-1.0.6/LICENSE` & `ucampurestorage-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `ucampurestorage-1.0.6/PKG-INFO` & `ucampurestorage-1.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ucampurestorage
-Version: 1.0.6
+Version: 1.0.7
 Summary: Pure Storage module for the utilization in Cambridge University
 Author-email: Ishan Mahajan <imahajan0007@gmail.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `ucampurestorage-1.0.6/README.md` & `ucampurestorage-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `ucampurestorage-1.0.6/docs/README.rst` & `ucampurestorage-1.0.7/ucampurestorage.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,152 +1,151 @@
+Metadata-Version: 2.1
+Name: ucampurestorage
+Version: 1.0.7
+Summary: Pure Storage module for the utilization in Cambridge University
+Author-email: Ishan Mahajan <imahajan0007@gmail.com>
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE
 
-UCAM PURE STORAGE
-=================
+# UCAM PURE STORAGE 
+![Pure Storage](pure_storage.jpg "Pure Storage logo")
 
+###### [Module Document](http://ifs-test-client1.srv.uis.private.cam.ac.uk:8080/index.html)
 
-.. image:: pure_storage.jpg
-   :target: pure_storage.jpg
-   :alt: Pure Storage
-
-
-`Module Document <http://ifs-test-client1.srv.uis.private.cam.ac.uk:8080/index.html>`_
-##########################################################################################
-
-Introduction
-^^^^^^^^^^^^
-
+### Introduction
 The CLI developed in this project allows the user to interact with PureStorage using REST API.
 
-With this CLI, you can list the existing volumes, servers, etc, on the Dell SCs, clone volumes, create snapshots, replace existing volumes with a golden image, etc. It is also able to configure system /etc/fstab and multipath when needed in some operations like volume mapping and mounting.
-
-Running the Application
-^^^^^^^^^^^^^^^^^^^^^^^
 
-Prerequisites
-~~~~~~~~~~~~~
+With this CLI, you can list the existing volumes, servers, etc, on the Dell SCs, clone volumes, create snapshots, replace existing volumes with a golden image, etc. It is also able to configure system /etc/fstab and multipath when needed in some operations like volume mapping and mounting.
 
+### Running the Application
 
-* `requests 2.30.0 <https://pypi.org/project/requests/2.30.0/>`_
-* `pyjwt <https://pypi.org/project/PyJWT/2.7.0/>`_\ `[crypto] <https://pypi.org/project/cryptography/40.0.2/>`_
-* `paramiko 3.1.0 <https://pypi.org/project/paramiko/3.1.0/>`_
-* `distro 1.8.0 <https://pypi.org/project/distro/1.8.0/>`_
+#### Prerequisites
+* [requests 2.30.0](https://pypi.org/project/requests/2.30.0/)
+* [pyjwt](https://pypi.org/project/PyJWT/2.7.0/)[[crypto]](https://pypi.org/project/cryptography/40.0.2/)
+* [paramiko 3.1.0](https://pypi.org/project/paramiko/3.1.0/)
+* [distro 1.8.0](https://pypi.org/project/distro/1.8.0/)
 
 Download the private key from the 1PASSWORD utilized to create the API account on the purestorage and fetch the credentials required.
+1. Pure Storage Arrays [user and passowrd]
+2. PureAPI information [client_id, key_id, client_name, storage, keyfile]
 
-
-#. Pure Storage Arrays [user and passowrd]
-#. PureAPI information [client_id, key_id, client_name, storage, keyfile]
-
-Installation
-^^^^^^^^^^^^
-
+### Installation
 To install the ucampurestorage pip package
 
-.. code-block::
-
-   pip3 install ucampurestorage
+```
+pip3 install ucampurestorage
+```
 
 CLI
 The help shows how to use ucampurestorage.
 
-.. code-block::
+```
+    usage: __main__.py [-h] [-v] [--storage STORAGE] [--port PORT] [--client_id CLIENT_ID] [--key_id KEY_ID] [--client_name CLIENT_NAME] [--user USER] [--password PASSWORD] [--is_secure IS_SECURE]
+                   [--record_config RECORD_CONFIG] [--file FILE] [--keyfile KEYFILE]
+                   {tokengen,list,volume,host,snapshot} ...
+
+    Manage Pure Storage Manager objects via REST API.
+
+    positional arguments:
+    {tokengen,list,volume,host,snapshot}
+        tokengen            Generate Pure Storage API token to access objects. Example: ucampurestorage tokengen --keyfile "./key.pem"
+        list                List Pure objects.
+        volume              Operations with respect to volumes in the Pure objects.
+        host                Operations with respect to hosts in the Pure objects.
+        snapshot            Operations with respect to snapshots in the Pure objects.
+
+    options:
+    -h, --help            show this help message and exit
+    -v, --version         show program's version number and exit
+    --storage STORAGE     Pure hostname. Default: uis-pure-wcdc1.srv.uis.private.cam.ac.uk
+    --port PORT           Pure port. Default: 443
+    --client_id CLIENT_ID
+                            Pure Storage Client ID for API
+    --key_id KEY_ID       Pure Storage Key ID for API
+    --client_name CLIENT_NAME
+                            Pure Storage Client Name for API
+    --user USER           Pure Storage username
+    --password PASSWORD   Pure Storage password
+    --is_secure IS_SECURE
+                            Secure connection. Default: False
+    --record_config RECORD_CONFIG
+                            Record multipath and file system config details. Default: False (do not record system config details)
+    --file FILE           Read arguments from json file
+    --keyfile KEYFILE     path to private keys inorder to generate token for the API call
 
-       usage: __main__.py [-h] [-v] [--storage STORAGE] [--port PORT] [--client_id CLIENT_ID] [--key_id KEY_ID] [--client_name CLIENT_NAME] [--user USER] [--password PASSWORD] [--is_secure IS_SECURE]
-                      [--record_config RECORD_CONFIG] [--file FILE] [--keyfile KEYFILE]
-                      {tokengen,list,volume,host,snapshot} ...
-
-       Manage Pure Storage Manager objects via REST API.
-
-       positional arguments:
-       {tokengen,list,volume,host,snapshot}
-           tokengen            Generate Pure Storage API token to access objects. Example: ucampurestorage tokengen --keyfile "./key.pem"
-           list                List Pure objects.
-           volume              Operations with respect to volumes in the Pure objects.
-           host                Operations with respect to hosts in the Pure objects.
-           snapshot            Operations with respect to snapshots in the Pure objects.
-
-       options:
-       -h, --help            show this help message and exit
-       -v, --version         show program's version number and exit
-       --storage STORAGE     Pure hostname. Default: uis-pure-wcdc1.srv.uis.private.cam.ac.uk
-       --port PORT           Pure port. Default: 443
-       --client_id CLIENT_ID
-                               Pure Storage Client ID for API
-       --key_id KEY_ID       Pure Storage Key ID for API
-       --client_name CLIENT_NAME
-                               Pure Storage Client Name for API
-       --user USER           Pure Storage username
-       --password PASSWORD   Pure Storage password
-       --is_secure IS_SECURE
-                               Secure connection. Default: False
-       --record_config RECORD_CONFIG
-                               Record multipath and file system config details. Default: False (do not record system config details)
-       --file FILE           Read arguments from json file
-       --keyfile KEYFILE     path to private keys inorder to generate token for the API call
+```
 
 For instance to get the list of volumes:
 
-.. code-block::
+```
 
+    python -m ucampurestorage  --client_id "25********************************0d" --key_id "f**************************************d" --client_nam "apitest" --user "pureuser" --password "****" --keyfile "/tmp/fa2xprivate.pem" list --object volumes
+    05/15/2023 13:15:09 [INFO] List of volumes:
+    ('all-cs-dev-db2/cs-dev-db2-vol1', {'name': 'all-cs-dev-db2/cs-dev-db2-vol1', 'created': 1674035421108, 'provisioned': 4398046511104, 'id': '8a92b2eb-d1e5-86ff-bae5-0b3e94a68352', 'serial': 'D11719CD15D049C4000117D1', 'subtype': 'regular', 'destroyed': False, 'connection_count': 1, 'source': {'id': None, 'name': None}, 'space': {'data_reduction': 20.207987278384994, 'shared': None, 'snapshots': 137571, 'system': None, 'thin_provisioning': 0.1090306097175926, 'total_physical': 1741547, 'total_provisioned': 4398046511104, 'total_reduction': 22.680899589580445, 'unique': 1603976, 'virtual': 3918524818432, 'unique_effective': 13794304, 'snapshots_effective': 19247104, 'total_effective': 33041408}, 'host_encryption_key_status': 'none', 'pod': {'id': None, 'name': None}, 'volume_group': {'id': '38422cf2-4b44-5446-e316-774881ac7a97', 'name': 'all-cs-dev-db2'}, 'requested_promotion_state': 'promoted', 'promotion_status': 'promoted', 'priority_adjustment': {'priority_adjustment_operator': '+', 'priority_adjustment_value': 0}})
+    ('wcdc-unstretched::cs-dev-db2-vol2', {'name': 'wcdc-unstretched::cs-dev-db2-vol2', 'created': 1674036405359, 'provisioned': 4398046511104, 'id': '8eb257d2-932c-cc2c-6fc5-aee2c859133a', 'serial': 'D11719CD15D049C4000117D2', 'subtype': 'regular', 'destroyed': False, 'connection_count': 1, 'source': {'id': None, 'name': None}, 'space': {'data_reduction': 14.675370508125324, 'shared': None, 'snapshots': 0, 'system': None, 'thin_provisioning': 0.37564394995570183, 'total_physical': 61310655408, 'total_provisioned': 4398046511104, 'total_reduction': 23.504810287469954, 'unique': 61310655408, 'virtual': 2745946947584, 'unique_effective': 2745946947584, 'snapshots_effective': 0, 'total_effective': 2745946947584}, 'host_encryption_key_status': 'none', 'pod': {'id': 'dcc4618c-e160-2579-2670-a781a02dbecc', 'name': 'wcdc-unstretched'}, 'volume_group': {'id': None, 'name': None}, 'requested_promotion_state': 'promoted', 'promotion_status': 'promoted', 'priority_adjustment': {'priority_adjustment_operator': '+', 'priority_adjustment_value': 0}})
+    ('TEST113', {'name': 'TEST113', 'created': 1683833793733, 'provisioned': 1099511627776, 'id': 'f7868879-0ccf-a062-3d00-fe9749244595', 'serial': 'D11719CD15D049C40003B438', 'subtype': 'regular', 'destroyed': False, 'connection_count': 1, 'source': {'id': None, 'name': None}, 'space': {'data_reduction': 20.153899533669993, 'shared': None, 'snapshots': 962, 'system': None, 'thin_provisioning': 0.9999810345470905, 'total_physical': 4727, 'total_provisioned': 1099511627776, 'total_reduction': 1062663.7618343926, 'unique': 3765, 'virtual': 20852736, 'unique_effective': 1810432, 'snapshots_effective': 1724416, 'total_effective': 3534848}, 'host_encryption_key_status': 'none', 'pod': {'id': None, 'name': None}, 'volume_group': {'id': None, 'name': None}, 'requested_promotion_state': 'promoted', 'promotion_status': 'promoted', 'priority_adjustment': {'priority_adjustment_operator': '+', 'priority_adjustment_value': 0}})
+    ('TEST113_clone', {'name': 'TEST113_clone', 'created': 1683929188193, 'provisioned': 1099511627776, 'id': 'ab0d5603-6151-ad2e-5bbf-f225088b9d45', 'serial': 'D11719CD15D049C40003BB47', 'subtype': 'regular', 'destroyed': False, 'connection_count': 0, 'source': {'id': 'f7868879-0ccf-a062-3d00-fe9749244595', 'name': 'TEST113'}, 'space': {'data_reduction': 20.073879895763707, 'shared': None, 'snapshots': 0, 'system': None, 'thin_provisioning': 0.9999811537563801, 'total_physical': 9087, 'total_provisioned': 1099511627776, 'total_reduction': 1065139.5737316788, 'unique': 9087, 'virtual': 20721664, 'unique_effective': 1712128, 'snapshots_effective': 0, 'total_effective': 1712128}, 'host_encryption_key_status': 'none', 'pod': {'id': None, 'name': None}, 'volume_group': {'id': None, 'name': None}, 'requested_promotion_state': 'promoted', 'promotion_status': 'promoted', 'priority_adjustment': {'priority_adjustment_operator': '+', 'priority_adjustment_value': 0}})
+    ('TEST113_1', {'name': 'TEST113_1', 'created': 1683937754712, 'provisioned': 1099511627776, 'id': 'a92df65f-c621-2ed8-f4a8-6cb14ca3b217', 'serial': 'D11719CD15D049C40003BBF1', 'subtype': 'regular', 'destroyed': False, 'connection_count': 1, 'source': {'id': 'f7868879-0ccf-a062-3d00-fe9749244595', 'name': 'TEST113'}, 'space': {'data_reduction': 20.12940592740464, 'shared': None, 'snapshots': 806, 'system': None, 'thin_provisioning': 0.9999810345470905, 'total_physical': 6032, 'total_provisioned': 1099511627776, 'total_reduction': 1061372.2763959866, 'unique': 5226, 'virtual': 20852736, 'unique_effective': 1810432, 'snapshots_effective': 1724416, 'total_effective': 3534848}, 'host_encryption_key_status': 'none', 'pod': {'id': None, 'name': None}, 'volume_group': {'id': None, 'name': None}, 'requested_promotion_state': 'promoted', 'promotion_status': 'promoted', 'priority_adjustment': {'priority_adjustment_operator': '+', 'priority_adjustment_value': 0}})
+    05/15/2023 13:15:09 [INFO] [Command succeeded - Returns True]
 
-       python -m ucampurestorage  --client_id "25********************************0d" --key_id "f**************************************d" --client_nam "apitest" --user "pureuser" --password "****" --keyfile "/tmp/fa2xprivate.pem" list --object volumes
-       05/15/2023 13:15:09 [INFO] List of volumes:
-       ('all-cs-dev-db2/cs-dev-db2-vol1', {'name': 'all-cs-dev-db2/cs-dev-db2-vol1', 'created': 1674035421108, 'provisioned': 4398046511104, 'id': '8a92b2eb-d1e5-86ff-bae5-0b3e94a68352', 'serial': 'D11719CD15D049C4000117D1', 'subtype': 'regular', 'destroyed': False, 'connection_count': 1, 'source': {'id': None, 'name': None}, 'space': {'data_reduction': 20.207987278384994, 'shared': None, 'snapshots': 137571, 'system': None, 'thin_provisioning': 0.1090306097175926, 'total_physical': 1741547, 'total_provisioned': 4398046511104, 'total_reduction': 22.680899589580445, 'unique': 1603976, 'virtual': 3918524818432, 'unique_effective': 13794304, 'snapshots_effective': 19247104, 'total_effective': 33041408}, 'host_encryption_key_status': 'none', 'pod': {'id': None, 'name': None}, 'volume_group': {'id': '38422cf2-4b44-5446-e316-774881ac7a97', 'name': 'all-cs-dev-db2'}, 'requested_promotion_state': 'promoted', 'promotion_status': 'promoted', 'priority_adjustment': {'priority_adjustment_operator': '+', 'priority_adjustment_value': 0}})
-       ('wcdc-unstretched::cs-dev-db2-vol2', {'name': 'wcdc-unstretched::cs-dev-db2-vol2', 'created': 1674036405359, 'provisioned': 4398046511104, 'id': '8eb257d2-932c-cc2c-6fc5-aee2c859133a', 'serial': 'D11719CD15D049C4000117D2', 'subtype': 'regular', 'destroyed': False, 'connection_count': 1, 'source': {'id': None, 'name': None}, 'space': {'data_reduction': 14.675370508125324, 'shared': None, 'snapshots': 0, 'system': None, 'thin_provisioning': 0.37564394995570183, 'total_physical': 61310655408, 'total_provisioned': 4398046511104, 'total_reduction': 23.504810287469954, 'unique': 61310655408, 'virtual': 2745946947584, 'unique_effective': 2745946947584, 'snapshots_effective': 0, 'total_effective': 2745946947584}, 'host_encryption_key_status': 'none', 'pod': {'id': 'dcc4618c-e160-2579-2670-a781a02dbecc', 'name': 'wcdc-unstretched'}, 'volume_group': {'id': None, 'name': None}, 'requested_promotion_state': 'promoted', 'promotion_status': 'promoted', 'priority_adjustment': {'priority_adjustment_operator': '+', 'priority_adjustment_value': 0}})
-       ('TEST113', {'name': 'TEST113', 'created': 1683833793733, 'provisioned': 1099511627776, 'id': 'f7868879-0ccf-a062-3d00-fe9749244595', 'serial': 'D11719CD15D049C40003B438', 'subtype': 'regular', 'destroyed': False, 'connection_count': 1, 'source': {'id': None, 'name': None}, 'space': {'data_reduction': 20.153899533669993, 'shared': None, 'snapshots': 962, 'system': None, 'thin_provisioning': 0.9999810345470905, 'total_physical': 4727, 'total_provisioned': 1099511627776, 'total_reduction': 1062663.7618343926, 'unique': 3765, 'virtual': 20852736, 'unique_effective': 1810432, 'snapshots_effective': 1724416, 'total_effective': 3534848}, 'host_encryption_key_status': 'none', 'pod': {'id': None, 'name': None}, 'volume_group': {'id': None, 'name': None}, 'requested_promotion_state': 'promoted', 'promotion_status': 'promoted', 'priority_adjustment': {'priority_adjustment_operator': '+', 'priority_adjustment_value': 0}})
-       ('TEST113_clone', {'name': 'TEST113_clone', 'created': 1683929188193, 'provisioned': 1099511627776, 'id': 'ab0d5603-6151-ad2e-5bbf-f225088b9d45', 'serial': 'D11719CD15D049C40003BB47', 'subtype': 'regular', 'destroyed': False, 'connection_count': 0, 'source': {'id': 'f7868879-0ccf-a062-3d00-fe9749244595', 'name': 'TEST113'}, 'space': {'data_reduction': 20.073879895763707, 'shared': None, 'snapshots': 0, 'system': None, 'thin_provisioning': 0.9999811537563801, 'total_physical': 9087, 'total_provisioned': 1099511627776, 'total_reduction': 1065139.5737316788, 'unique': 9087, 'virtual': 20721664, 'unique_effective': 1712128, 'snapshots_effective': 0, 'total_effective': 1712128}, 'host_encryption_key_status': 'none', 'pod': {'id': None, 'name': None}, 'volume_group': {'id': None, 'name': None}, 'requested_promotion_state': 'promoted', 'promotion_status': 'promoted', 'priority_adjustment': {'priority_adjustment_operator': '+', 'priority_adjustment_value': 0}})
-       ('TEST113_1', {'name': 'TEST113_1', 'created': 1683937754712, 'provisioned': 1099511627776, 'id': 'a92df65f-c621-2ed8-f4a8-6cb14ca3b217', 'serial': 'D11719CD15D049C40003BBF1', 'subtype': 'regular', 'destroyed': False, 'connection_count': 1, 'source': {'id': 'f7868879-0ccf-a062-3d00-fe9749244595', 'name': 'TEST113'}, 'space': {'data_reduction': 20.12940592740464, 'shared': None, 'snapshots': 806, 'system': None, 'thin_provisioning': 0.9999810345470905, 'total_physical': 6032, 'total_provisioned': 1099511627776, 'total_reduction': 1061372.2763959866, 'unique': 5226, 'virtual': 20852736, 'unique_effective': 1810432, 'snapshots_effective': 1724416, 'total_effective': 3534848}, 'host_encryption_key_status': 'none', 'pod': {'id': None, 'name': None}, 'volume_group': {'id': None, 'name': None}, 'requested_promotion_state': 'promoted', 'promotion_status': 'promoted', 'priority_adjustment': {'priority_adjustment_operator': '+', 'priority_adjustment_value': 0}})
-       05/15/2023 13:15:09 [INFO] [Command succeeded - Returns True]
+```
 
 You get prompt for client_id, key_id, client_name, storage, user, keyfile, password
 
-.. code-block::
+```
 
+    ucampurestorage  list --object volumes
+    Username: pureuser
+    Client ID: 25********************************0d
+    Key ID: f**************************************d
+    Client Name: apitest
+    Private file location: /tmp/fa2xprivate.pem
+    Password:
+    05/15/2023 13:15:09 [INFO] List of volumes:
+    ('all-cs-dev-db2/cs-dev-db2-vol1', {'name': 'all-cs-dev-db2/cs-dev-db2-vol1', 'created': 1674035421108, 'provisioned': 4398046511104, 'id': '8a92b2eb-d1e5-86ff-bae5-0b3e94a68352', 'serial': 'D11719CD15D049C4000117D1', 'subtype': 'regular', 'destroyed': False, 'connection_count': 1, 'source': {'id': None, 'name': None}, 'space': {'data_reduction': 20.207987278384994, 'shared': None, 'snapshots': 137571, 'system': None, 'thin_provisioning': 0.1090306097175926, 'total_physical': 1741547, 'total_provisioned': 4398046511104, 'total_reduction': 22.680899589580445, 'unique': 1603976, 'virtual': 3918524818432, 'unique_effective': 13794304, 'snapshots_effective': 19247104, 'total_effective': 33041408}, 'host_encryption_key_status': 'none', 'pod': {'id': None, 'name': None}, 'volume_group': {'id': '38422cf2-4b44-5446-e316-774881ac7a97', 'name': 'all-cs-dev-db2'}, 'requested_promotion_state': 'promoted', 'promotion_status': 'promoted', 'priority_adjustment': {'priority_adjustment_operator': '+', 'priority_adjustment_value': 0}})
+    ('wcdc-unstretched::cs-dev-db2-vol2', {'name': 'wcdc-unstretched::cs-dev-db2-vol2', 'created': 1674036405359, 'provisioned': 4398046511104, 'id': '8eb257d2-932c-cc2c-6fc5-aee2c859133a', 'serial': 'D11719CD15D049C4000117D2', 'subtype': 'regular', 'destroyed': False, 'connection_count': 1, 'source': {'id': None, 'name': None}, 'space': {'data_reduction': 14.675370508125324, 'shared': None, 'snapshots': 0, 'system': None, 'thin_provisioning': 0.37564394995570183, 'total_physical': 61310655408, 'total_provisioned': 4398046511104, 'total_reduction': 23.504810287469954, 'unique': 61310655408, 'virtual': 2745946947584, 'unique_effective': 2745946947584, 'snapshots_effective': 0, 'total_effective': 2745946947584}, 'host_encryption_key_status': 'none', 'pod': {'id': 'dcc4618c-e160-2579-2670-a781a02dbecc', 'name': 'wcdc-unstretched'}, 'volume_group': {'id': None, 'name': None}, 'requested_promotion_state': 'promoted', 'promotion_status': 'promoted', 'priority_adjustment': {'priority_adjustment_operator': '+', 'priority_adjustment_value': 0}})
+    ('TEST113', {'name': 'TEST113', 'created': 1683833793733, 'provisioned': 1099511627776, 'id': 'f7868879-0ccf-a062-3d00-fe9749244595', 'serial': 'D11719CD15D049C40003B438', 'subtype': 'regular', 'destroyed': False, 'connection_count': 1, 'source': {'id': None, 'name': None}, 'space': {'data_reduction': 20.153899533669993, 'shared': None, 'snapshots': 962, 'system': None, 'thin_provisioning': 0.9999810345470905, 'total_physical': 4727, 'total_provisioned': 1099511627776, 'total_reduction': 1062663.7618343926, 'unique': 3765, 'virtual': 20852736, 'unique_effective': 1810432, 'snapshots_effective': 1724416, 'total_effective': 3534848}, 'host_encryption_key_status': 'none', 'pod': {'id': None, 'name': None}, 'volume_group': {'id': None, 'name': None}, 'requested_promotion_state': 'promoted', 'promotion_status': 'promoted', 'priority_adjustment': {'priority_adjustment_operator': '+', 'priority_adjustment_value': 0}})
+    ('TEST113_clone', {'name': 'TEST113_clone', 'created': 1683929188193, 'provisioned': 1099511627776, 'id': 'ab0d5603-6151-ad2e-5bbf-f225088b9d45', 'serial': 'D11719CD15D049C40003BB47', 'subtype': 'regular', 'destroyed': False, 'connection_count': 0, 'source': {'id': 'f7868879-0ccf-a062-3d00-fe9749244595', 'name': 'TEST113'}, 'space': {'data_reduction': 20.073879895763707, 'shared': None, 'snapshots': 0, 'system': None, 'thin_provisioning': 0.9999811537563801, 'total_physical': 9087, 'total_provisioned': 1099511627776, 'total_reduction': 1065139.5737316788, 'unique': 9087, 'virtual': 20721664, 'unique_effective': 1712128, 'snapshots_effective': 0, 'total_effective': 1712128}, 'host_encryption_key_status': 'none', 'pod': {'id': None, 'name': None}, 'volume_group': {'id': None, 'name': None}, 'requested_promotion_state': 'promoted', 'promotion_status': 'promoted', 'priority_adjustment': {'priority_adjustment_operator': '+', 'priority_adjustment_value': 0}})
+    ('TEST113_1', {'name': 'TEST113_1', 'created': 1683937754712, 'provisioned': 1099511627776, 'id': 'a92df65f-c621-2ed8-f4a8-6cb14ca3b217', 'serial': 'D11719CD15D049C40003BBF1', 'subtype': 'regular', 'destroyed': False, 'connection_count': 1, 'source': {'id': 'f7868879-0ccf-a062-3d00-fe9749244595', 'name': 'TEST113'}, 'space': {'data_reduction': 20.12940592740464, 'shared': None, 'snapshots': 806, 'system': None, 'thin_provisioning': 0.9999810345470905, 'total_physical': 6032, 'total_provisioned': 1099511627776, 'total_reduction': 1061372.2763959866, 'unique': 5226, 'virtual': 20852736, 'unique_effective': 1810432, 'snapshots_effective': 1724416, 'total_effective': 3534848}, 'host_encryption_key_status': 'none', 'pod': {'id': None, 'name': None}, 'volume_group': {'id': None, 'name': None}, 'requested_promotion_state': 'promoted', 'promotion_status': 'promoted', 'priority_adjustment': {'priority_adjustment_operator': '+', 'priority_adjustment_value': 0}})
+    05/15/2023 13:15:09 [INFO] [Command succeeded - Returns True]
 
-       ucampurestorage  list --object volumes
-       Username: pureuser
-       Client ID: 25********************************0d
-       Key ID: f**************************************d
-       Client Name: apitest
-       Private file location: /tmp/fa2xprivate.pem
-       Password:
-       05/15/2023 13:15:09 [INFO] List of volumes:
-       ('all-cs-dev-db2/cs-dev-db2-vol1', {'name': 'all-cs-dev-db2/cs-dev-db2-vol1', 'created': 1674035421108, 'provisioned': 4398046511104, 'id': '8a92b2eb-d1e5-86ff-bae5-0b3e94a68352', 'serial': 'D11719CD15D049C4000117D1', 'subtype': 'regular', 'destroyed': False, 'connection_count': 1, 'source': {'id': None, 'name': None}, 'space': {'data_reduction': 20.207987278384994, 'shared': None, 'snapshots': 137571, 'system': None, 'thin_provisioning': 0.1090306097175926, 'total_physical': 1741547, 'total_provisioned': 4398046511104, 'total_reduction': 22.680899589580445, 'unique': 1603976, 'virtual': 3918524818432, 'unique_effective': 13794304, 'snapshots_effective': 19247104, 'total_effective': 33041408}, 'host_encryption_key_status': 'none', 'pod': {'id': None, 'name': None}, 'volume_group': {'id': '38422cf2-4b44-5446-e316-774881ac7a97', 'name': 'all-cs-dev-db2'}, 'requested_promotion_state': 'promoted', 'promotion_status': 'promoted', 'priority_adjustment': {'priority_adjustment_operator': '+', 'priority_adjustment_value': 0}})
-       ('wcdc-unstretched::cs-dev-db2-vol2', {'name': 'wcdc-unstretched::cs-dev-db2-vol2', 'created': 1674036405359, 'provisioned': 4398046511104, 'id': '8eb257d2-932c-cc2c-6fc5-aee2c859133a', 'serial': 'D11719CD15D049C4000117D2', 'subtype': 'regular', 'destroyed': False, 'connection_count': 1, 'source': {'id': None, 'name': None}, 'space': {'data_reduction': 14.675370508125324, 'shared': None, 'snapshots': 0, 'system': None, 'thin_provisioning': 0.37564394995570183, 'total_physical': 61310655408, 'total_provisioned': 4398046511104, 'total_reduction': 23.504810287469954, 'unique': 61310655408, 'virtual': 2745946947584, 'unique_effective': 2745946947584, 'snapshots_effective': 0, 'total_effective': 2745946947584}, 'host_encryption_key_status': 'none', 'pod': {'id': 'dcc4618c-e160-2579-2670-a781a02dbecc', 'name': 'wcdc-unstretched'}, 'volume_group': {'id': None, 'name': None}, 'requested_promotion_state': 'promoted', 'promotion_status': 'promoted', 'priority_adjustment': {'priority_adjustment_operator': '+', 'priority_adjustment_value': 0}})
-       ('TEST113', {'name': 'TEST113', 'created': 1683833793733, 'provisioned': 1099511627776, 'id': 'f7868879-0ccf-a062-3d00-fe9749244595', 'serial': 'D11719CD15D049C40003B438', 'subtype': 'regular', 'destroyed': False, 'connection_count': 1, 'source': {'id': None, 'name': None}, 'space': {'data_reduction': 20.153899533669993, 'shared': None, 'snapshots': 962, 'system': None, 'thin_provisioning': 0.9999810345470905, 'total_physical': 4727, 'total_provisioned': 1099511627776, 'total_reduction': 1062663.7618343926, 'unique': 3765, 'virtual': 20852736, 'unique_effective': 1810432, 'snapshots_effective': 1724416, 'total_effective': 3534848}, 'host_encryption_key_status': 'none', 'pod': {'id': None, 'name': None}, 'volume_group': {'id': None, 'name': None}, 'requested_promotion_state': 'promoted', 'promotion_status': 'promoted', 'priority_adjustment': {'priority_adjustment_operator': '+', 'priority_adjustment_value': 0}})
-       ('TEST113_clone', {'name': 'TEST113_clone', 'created': 1683929188193, 'provisioned': 1099511627776, 'id': 'ab0d5603-6151-ad2e-5bbf-f225088b9d45', 'serial': 'D11719CD15D049C40003BB47', 'subtype': 'regular', 'destroyed': False, 'connection_count': 0, 'source': {'id': 'f7868879-0ccf-a062-3d00-fe9749244595', 'name': 'TEST113'}, 'space': {'data_reduction': 20.073879895763707, 'shared': None, 'snapshots': 0, 'system': None, 'thin_provisioning': 0.9999811537563801, 'total_physical': 9087, 'total_provisioned': 1099511627776, 'total_reduction': 1065139.5737316788, 'unique': 9087, 'virtual': 20721664, 'unique_effective': 1712128, 'snapshots_effective': 0, 'total_effective': 1712128}, 'host_encryption_key_status': 'none', 'pod': {'id': None, 'name': None}, 'volume_group': {'id': None, 'name': None}, 'requested_promotion_state': 'promoted', 'promotion_status': 'promoted', 'priority_adjustment': {'priority_adjustment_operator': '+', 'priority_adjustment_value': 0}})
-       ('TEST113_1', {'name': 'TEST113_1', 'created': 1683937754712, 'provisioned': 1099511627776, 'id': 'a92df65f-c621-2ed8-f4a8-6cb14ca3b217', 'serial': 'D11719CD15D049C40003BBF1', 'subtype': 'regular', 'destroyed': False, 'connection_count': 1, 'source': {'id': 'f7868879-0ccf-a062-3d00-fe9749244595', 'name': 'TEST113'}, 'space': {'data_reduction': 20.12940592740464, 'shared': None, 'snapshots': 806, 'system': None, 'thin_provisioning': 0.9999810345470905, 'total_physical': 6032, 'total_provisioned': 1099511627776, 'total_reduction': 1061372.2763959866, 'unique': 5226, 'virtual': 20852736, 'unique_effective': 1810432, 'snapshots_effective': 1724416, 'total_effective': 3534848}, 'host_encryption_key_status': 'none', 'pod': {'id': None, 'name': None}, 'volume_group': {'id': None, 'name': None}, 'requested_promotion_state': 'promoted', 'promotion_status': 'promoted', 'priority_adjustment': {'priority_adjustment_operator': '+', 'priority_adjustment_value': 0}})
-       05/15/2023 13:15:09 [INFO] [Command succeeded - Returns True]
+```
 
 The CLI can also read arguments from the a json file:
 
-.. code-block::
+```
 
+    {
+    "client_id": "25********************************0d",
+    "key_id": "f**************************************d",
+    "client_name": "apitest",
+    "storage": "purestorage.cam.ac.uk",
+    "user": "pureuser",
+    "password": "********,
+    "keyfile": "/tmp/fa2xprivate.pem"
+    }
 
-       {
-       "client_id": "25********************************0d",
-       "key_id": "f**************************************d",
-       "client_name": "apitest",
-       "storage": "purestorage.cam.ac.uk",
-       "user": "pureuser",
-       "password": "********,
-       "keyfile": "/tmp/fa2xprivate.pem"
-       }
+```
 
-To use a config file, use the option --file:
 
-.. code-block::
+To use a config file, use the option --file:
 
+```
 
-       ucampurestorage --file=./ucampurestorage/lib/secrets.json list --object volumes
-       05/15/2023 13:09:11 [INFO] List of volumes:
-       ('all-cs-dev-db2/cs-dev-db2-vol1', {'name': 'all-cs-dev-db2/cs-dev-db2-vol1', 'created': 1674035421108, 'provisioned': 4398046511104, 'id': '8a92b2eb-d1e5-86ff-bae5-0b3e94a68352', 'serial': 'D11719CD15D049C4000117D1', 'subtype': 'regular', 'destroyed': False, 'connection_count': 1, 'source': {'id': None, 'name': None}, 'space': {'data_reduction': 20.207987278384994, 'shared': None, 'snapshots': 137571, 'system': None, 'thin_provisioning': 0.1090306097175926, 'total_physical': 1741547, 'total_provisioned': 4398046511104, 'total_reduction': 22.680899589580445, 'unique': 1603976, 'virtual': 3918524818432, 'unique_effective': 13794304, 'snapshots_effective': 19247104, 'total_effective': 33041408}, 'host_encryption_key_status': 'none', 'pod': {'id': None, 'name': None}, 'volume_group': {'id': '38422cf2-4b44-5446-e316-774881ac7a97', 'name': 'all-cs-dev-db2'}, 'requested_promotion_state': 'promoted', 'promotion_status': 'promoted', 'priority_adjustment': {'priority_adjustment_operator': '+', 'priority_adjustment_value': 0}})
-       ('wcdc-unstretched::cs-dev-db2-vol2', {'name': 'wcdc-unstretched::cs-dev-db2-vol2', 'created': 1674036405359, 'provisioned': 4398046511104, 'id': '8eb257d2-932c-cc2c-6fc5-aee2c859133a', 'serial': 'D11719CD15D049C4000117D2', 'subtype': 'regular', 'destroyed': False, 'connection_count': 1, 'source': {'id': None, 'name': None}, 'space': {'data_reduction': 14.675370508125324, 'shared': None, 'snapshots': 0, 'system': None, 'thin_provisioning': 0.37564394995570183, 'total_physical': 61310655408, 'total_provisioned': 4398046511104, 'total_reduction': 23.504810287469954, 'unique': 61310655408, 'virtual': 2745946947584, 'unique_effective': 2745946947584, 'snapshots_effective': 0, 'total_effective': 2745946947584}, 'host_encryption_key_status': 'none', 'pod': {'id': 'dcc4618c-e160-2579-2670-a781a02dbecc', 'name': 'wcdc-unstretched'}, 'volume_group': {'id': None, 'name': None}, 'requested_promotion_state': 'promoted', 'promotion_status': 'promoted', 'priority_adjustment': {'priority_adjustment_operator': '+', 'priority_adjustment_value': 0}})
-       ('TEST113', {'name': 'TEST113', 'created': 1683833793733, 'provisioned': 1099511627776, 'id': 'f7868879-0ccf-a062-3d00-fe9749244595', 'serial': 'D11719CD15D049C40003B438', 'subtype': 'regular', 'destroyed': False, 'connection_count': 1, 'source': {'id': None, 'name': None}, 'space': {'data_reduction': 20.153899533669993, 'shared': None, 'snapshots': 962, 'system': None, 'thin_provisioning': 0.9999810345470905, 'total_physical': 4727, 'total_provisioned': 1099511627776, 'total_reduction': 1062663.7618343926, 'unique': 3765, 'virtual': 20852736, 'unique_effective': 1810432, 'snapshots_effective': 1724416, 'total_effective': 3534848}, 'host_encryption_key_status': 'none', 'pod': {'id': None, 'name': None}, 'volume_group': {'id': None, 'name': None}, 'requested_promotion_state': 'promoted', 'promotion_status': 'promoted', 'priority_adjustment': {'priority_adjustment_operator': '+', 'priority_adjustment_value': 0}})
-       ('TEST113_clone', {'name': 'TEST113_clone', 'created': 1683929188193, 'provisioned': 1099511627776, 'id': 'ab0d5603-6151-ad2e-5bbf-f225088b9d45', 'serial': 'D11719CD15D049C40003BB47', 'subtype': 'regular', 'destroyed': False, 'connection_count': 0, 'source': {'id': 'f7868879-0ccf-a062-3d00-fe9749244595', 'name': 'TEST113'}, 'space': {'data_reduction': 20.073879895763707, 'shared': None, 'snapshots': 0, 'system': None, 'thin_provisioning': 0.9999811537563801, 'total_physical': 9087, 'total_provisioned': 1099511627776, 'total_reduction': 1065139.5737316788, 'unique': 9087, 'virtual': 20721664, 'unique_effective': 1712128, 'snapshots_effective': 0, 'total_effective': 1712128}, 'host_encryption_key_status': 'none', 'pod': {'id': None, 'name': None}, 'volume_group': {'id': None, 'name': None}, 'requested_promotion_state': 'promoted', 'promotion_status': 'promoted', 'priority_adjustment': {'priority_adjustment_operator': '+', 'priority_adjustment_value': 0}})
-       ('TEST113_1', {'name': 'TEST113_1', 'created': 1683937754712, 'provisioned': 1099511627776, 'id': 'a92df65f-c621-2ed8-f4a8-6cb14ca3b217', 'serial': 'D11719CD15D049C40003BBF1', 'subtype': 'regular', 'destroyed': False, 'connection_count': 1, 'source': {'id': 'f7868879-0ccf-a062-3d00-fe9749244595', 'name': 'TEST113'}, 'space': {'data_reduction': 20.12940592740464, 'shared': None, 'snapshots': 806, 'system': None, 'thin_provisioning': 0.9999810345470905, 'total_physical': 6032, 'total_provisioned': 1099511627776, 'total_reduction': 1061372.2763959866, 'unique': 5226, 'virtual': 20852736, 'unique_effective': 1810432, 'snapshots_effective': 1724416, 'total_effective': 3534848}, 'host_encryption_key_status': 'none', 'pod': {'id': None, 'name': None}, 'volume_group': {'id': None, 'name': None}, 'requested_promotion_state': 'promoted', 'promotion_status': 'promoted', 'priority_adjustment': {'priority_adjustment_operator': '+', 'priority_adjustment_value': 0}})
-       05/15/2023 13:09:11 [INFO] [Command succeeded - Returns True]
+    ucampurestorage --file=./ucampurestorage/lib/secrets.json list --object volumes
+    05/15/2023 13:09:11 [INFO] List of volumes:
+    ('all-cs-dev-db2/cs-dev-db2-vol1', {'name': 'all-cs-dev-db2/cs-dev-db2-vol1', 'created': 1674035421108, 'provisioned': 4398046511104, 'id': '8a92b2eb-d1e5-86ff-bae5-0b3e94a68352', 'serial': 'D11719CD15D049C4000117D1', 'subtype': 'regular', 'destroyed': False, 'connection_count': 1, 'source': {'id': None, 'name': None}, 'space': {'data_reduction': 20.207987278384994, 'shared': None, 'snapshots': 137571, 'system': None, 'thin_provisioning': 0.1090306097175926, 'total_physical': 1741547, 'total_provisioned': 4398046511104, 'total_reduction': 22.680899589580445, 'unique': 1603976, 'virtual': 3918524818432, 'unique_effective': 13794304, 'snapshots_effective': 19247104, 'total_effective': 33041408}, 'host_encryption_key_status': 'none', 'pod': {'id': None, 'name': None}, 'volume_group': {'id': '38422cf2-4b44-5446-e316-774881ac7a97', 'name': 'all-cs-dev-db2'}, 'requested_promotion_state': 'promoted', 'promotion_status': 'promoted', 'priority_adjustment': {'priority_adjustment_operator': '+', 'priority_adjustment_value': 0}})
+    ('wcdc-unstretched::cs-dev-db2-vol2', {'name': 'wcdc-unstretched::cs-dev-db2-vol2', 'created': 1674036405359, 'provisioned': 4398046511104, 'id': '8eb257d2-932c-cc2c-6fc5-aee2c859133a', 'serial': 'D11719CD15D049C4000117D2', 'subtype': 'regular', 'destroyed': False, 'connection_count': 1, 'source': {'id': None, 'name': None}, 'space': {'data_reduction': 14.675370508125324, 'shared': None, 'snapshots': 0, 'system': None, 'thin_provisioning': 0.37564394995570183, 'total_physical': 61310655408, 'total_provisioned': 4398046511104, 'total_reduction': 23.504810287469954, 'unique': 61310655408, 'virtual': 2745946947584, 'unique_effective': 2745946947584, 'snapshots_effective': 0, 'total_effective': 2745946947584}, 'host_encryption_key_status': 'none', 'pod': {'id': 'dcc4618c-e160-2579-2670-a781a02dbecc', 'name': 'wcdc-unstretched'}, 'volume_group': {'id': None, 'name': None}, 'requested_promotion_state': 'promoted', 'promotion_status': 'promoted', 'priority_adjustment': {'priority_adjustment_operator': '+', 'priority_adjustment_value': 0}})
+    ('TEST113', {'name': 'TEST113', 'created': 1683833793733, 'provisioned': 1099511627776, 'id': 'f7868879-0ccf-a062-3d00-fe9749244595', 'serial': 'D11719CD15D049C40003B438', 'subtype': 'regular', 'destroyed': False, 'connection_count': 1, 'source': {'id': None, 'name': None}, 'space': {'data_reduction': 20.153899533669993, 'shared': None, 'snapshots': 962, 'system': None, 'thin_provisioning': 0.9999810345470905, 'total_physical': 4727, 'total_provisioned': 1099511627776, 'total_reduction': 1062663.7618343926, 'unique': 3765, 'virtual': 20852736, 'unique_effective': 1810432, 'snapshots_effective': 1724416, 'total_effective': 3534848}, 'host_encryption_key_status': 'none', 'pod': {'id': None, 'name': None}, 'volume_group': {'id': None, 'name': None}, 'requested_promotion_state': 'promoted', 'promotion_status': 'promoted', 'priority_adjustment': {'priority_adjustment_operator': '+', 'priority_adjustment_value': 0}})
+    ('TEST113_clone', {'name': 'TEST113_clone', 'created': 1683929188193, 'provisioned': 1099511627776, 'id': 'ab0d5603-6151-ad2e-5bbf-f225088b9d45', 'serial': 'D11719CD15D049C40003BB47', 'subtype': 'regular', 'destroyed': False, 'connection_count': 0, 'source': {'id': 'f7868879-0ccf-a062-3d00-fe9749244595', 'name': 'TEST113'}, 'space': {'data_reduction': 20.073879895763707, 'shared': None, 'snapshots': 0, 'system': None, 'thin_provisioning': 0.9999811537563801, 'total_physical': 9087, 'total_provisioned': 1099511627776, 'total_reduction': 1065139.5737316788, 'unique': 9087, 'virtual': 20721664, 'unique_effective': 1712128, 'snapshots_effective': 0, 'total_effective': 1712128}, 'host_encryption_key_status': 'none', 'pod': {'id': None, 'name': None}, 'volume_group': {'id': None, 'name': None}, 'requested_promotion_state': 'promoted', 'promotion_status': 'promoted', 'priority_adjustment': {'priority_adjustment_operator': '+', 'priority_adjustment_value': 0}})
+    ('TEST113_1', {'name': 'TEST113_1', 'created': 1683937754712, 'provisioned': 1099511627776, 'id': 'a92df65f-c621-2ed8-f4a8-6cb14ca3b217', 'serial': 'D11719CD15D049C40003BBF1', 'subtype': 'regular', 'destroyed': False, 'connection_count': 1, 'source': {'id': 'f7868879-0ccf-a062-3d00-fe9749244595', 'name': 'TEST113'}, 'space': {'data_reduction': 20.12940592740464, 'shared': None, 'snapshots': 806, 'system': None, 'thin_provisioning': 0.9999810345470905, 'total_physical': 6032, 'total_provisioned': 1099511627776, 'total_reduction': 1061372.2763959866, 'unique': 5226, 'virtual': 20852736, 'unique_effective': 1810432, 'snapshots_effective': 1724416, 'total_effective': 3534848}, 'host_encryption_key_status': 'none', 'pod': {'id': None, 'name': None}, 'volume_group': {'id': None, 'name': None}, 'requested_promotion_state': 'promoted', 'promotion_status': 'promoted', 'priority_adjustment': {'priority_adjustment_operator': '+', 'priority_adjustment_value': 0}})
+    05/15/2023 13:09:11 [INFO] [Command succeeded - Returns True]
 
-Application logging
-~~~~~~~~~~~~~~~~~~~
+```
 
+#### Application logging
 Logs generated by cli are located in /var/log/ucampurestorage/
+
```

### Comparing `ucampurestorage-1.0.6/pyproject.toml` & `ucampurestorage-1.0.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ucampurestorage-1.0.6/ucampurecli/pure_clone_volume` & `ucampurestorage-1.0.7/ucampurecli/pure_clone_volume`

 * *Files identical despite different names*

### Comparing `ucampurestorage-1.0.6/ucampurecli/pure_create_snapshot` & `ucampurestorage-1.0.7/ucampurecli/pure_create_snapshot`

 * *Files identical despite different names*

### Comparing `ucampurestorage-1.0.6/ucampurecli/pure_create_volume` & `ucampurestorage-1.0.7/ucampurecli/pure_create_volume`

 * *Files identical despite different names*

### Comparing `ucampurestorage-1.0.6/ucampurecli/pure_delete_volume` & `ucampurestorage-1.0.7/ucampurecli/pure_delete_volume`

 * *Files identical despite different names*

### Comparing `ucampurestorage-1.0.6/ucampurecli/pure_eradicate_destroyed_volume` & `ucampurestorage-1.0.7/ucampurecli/pure_eradicate_destroyed_volume`

 * *Files identical despite different names*

### Comparing `ucampurestorage-1.0.6/ucampurecli/pure_map_volume` & `ucampurestorage-1.0.7/ucampurecli/pure_map_volume`

 * *Files 5% similar despite different names*

```diff
@@ -53,15 +53,15 @@
 EOF
 }
 
 ###################################################################
 # Parse the args 
 ###################################################################
 
-while getopts "hn:t:x:k:" opt
+while getopts "hn:p:x:k:" opt
 do
   case $opt in
     h)
       usage
       exit
       ;;
     n)
@@ -83,27 +83,27 @@
   esac
 done
 
 # check required arguments
 if [ -z "$name" ] || [ -z "$mount" ]|| [ -z "$new" ]|| [ -z "$secrets" ]
 then
    usage
-   exit
+   exit 1
 fi
 
 # Call ucampurestorage package
 if [[ $new == 1 ]]
 then
     result=$($ucampurestorage  --record_config True --file $secrets volume map --name $name --mp $mount -new )
 elif [[ $new == 0 ]]
 then
     result=$($ucampurestorage  --record_config True --file $secrets volume map --name $name --mp $mount)
 else
    usage
-   exit
+   exit 1
 fi
 
 if [[ $result == *"[Command succeeded - Returns True]"* ]]
 then
     echo "Command succeeded."
     exit 0
 else
```

### Comparing `ucampurestorage-1.0.6/ucampurecli/pure_record_destoyed_volume` & `ucampurestorage-1.0.7/ucampurecli/pure_record_destoyed_volume`

 * *Files identical despite different names*

### Comparing `ucampurestorage-1.0.6/ucampurecli/pure_replace_volume` & `ucampurestorage-1.0.7/ucampurecli/pure_replace_volume`

 * *Files identical despite different names*

### Comparing `ucampurestorage-1.0.6/ucampurecli/pure_unmap_volume` & `ucampurestorage-1.0.7/ucampurecli/pure_unmap_volume`

 * *Files 20% similar despite different names*

```diff
@@ -23,18 +23,22 @@
 usage: $0 options
 
 This script unmaps a purestorage volume.
 
 OPTIONS:
   -h 
   -n name                             Name of the volume.
+  -w wwn                              WWN of the volume.
+  -p mount point                      mountpoint on the local machine.
   -k /path/to/secrets.json            Secret file containing URL and credential to access Pure Storage.
 
 E.g.
-  $0 -n 123455 -k /path/to/secrets.json
+  1. $0 -n Test123 -k /path/to/secrets.json
+  2. $0 -w 123455 -k /path/to/secrets.json
+  3. $0 -p /t123 -k /path/to/secrets.json
 
 NB. 
 1. /path/to/secrets.json must be in the following format:
 {
   "client_id": "pure_api_client_id",
   "key_id": "pure_api_key_id",
   "client_name": "pure_api_client_name",
@@ -48,40 +52,52 @@
 EOF
 }
 
 ###################################################################
 # Parse the args 
 ###################################################################
 
-while getopts "hn:k:" opt
+while getopts "hn:w:p:k:" opt
 do
   case $opt in
     h)
       usage
       exit
       ;;
     n)
       name=$OPTARG
      ;;
+    w)
+      wwn=$OPTARG
+     ;;
+    p)
+      mountpoint=$OPTARG
+     ;;
     k)
       secrets=$OPTARG
      ;;
     ?)
       usage
       exit
       ;;
   esac
 done
 
 # check required arguments
-if [ -z "$name" ] || [ -z "$secrets" ]
+if [ -z "$secrets" ]
 then
    usage
    exit
 fi
+if [[ ("$name" && "$wwn") || ("$mountpoint" && "$wwn") || ("$name" && "$mountpoint") || ("$name" && "$mountpoint" &&"$wwn") || (-z "$name" && -z "$mountpoint" && -z "$wwn")]]
+then
+   usage
+   exit 
+fi
+
 
 # Call ucampurestorage package
 result=$($ucampurestorage  --record_config True --file $secrets volume unmap --name $name)
 if [[ $result == *"[Command succeeded - Returns True]"* ]]
 then
     echo "Command succeeded."
     exit 0
```

### Comparing `ucampurestorage-1.0.6/ucampurestorage/__main__.py` & `ucampurestorage-1.0.7/ucampurestorage/__main__.py`

 * *Files identical despite different names*

