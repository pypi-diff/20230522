# Comparing `tmp/open-cravat-2.3.0.tar.gz` & `tmp/open-cravat-2.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "open-cravat-2.3.0.tar", last modified: Mon Mar 13 12:57:17 2023, max compression
+gzip compressed data, was "open-cravat-2.3.1.tar", last modified: Mon May 22 17:05:46 2023, max compression
```

## Comparing `open-cravat-2.3.0.tar` & `open-cravat-2.3.1.tar`

### file list

```diff
@@ -1,336 +1,338 @@
-drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2023-03-13 12:57:17.800377 open-cravat-2.3.0/
--rw-r--r--   0 kyle      (1000) kyle      (1000)     1067 2023-03-13 12:57:17.000000 open-cravat-2.3.0/LICENSE
--rw-r--r--   0 kyle      (1000) kyle      (1000)     1056 2023-03-13 12:57:17.800377 open-cravat-2.3.0/PKG-INFO
--rw-r--r--   0 kyle      (1000) kyle      (1000)      769 2023-03-13 12:57:17.000000 open-cravat-2.3.0/README.rst
-drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2023-03-13 12:57:17.782377 open-cravat-2.3.0/cravat/
--rw-r--r--   0 kyle      (1000) kyle      (1000)     6364 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/__init__.py
--rw-r--r--   0 kyle      (1000) kyle      (1000)    59163 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/admin_util.py
--rw-r--r--   0 kyle      (1000) kyle      (1000)    19659 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/aggregator.py
--rw-r--r--   0 kyle      (1000) kyle      (1000)     2990 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/annotator_options.py
-drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2023-03-13 12:57:17.782377 open-cravat-2.3.0/cravat/annotator_template/
--rw-r--r--   0 kyle      (1000) kyle      (1000)      178 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/annotator_template/annotator_template.md
--rw-r--r--   0 kyle      (1000) kyle      (1000)     2326 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/annotator_template/annotator_template.py
--rw-r--r--   0 kyle      (1000) kyle      (1000)     1460 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/annotator_template/annotator_template.yml
-drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2023-03-13 12:57:17.782377 open-cravat-2.3.0/cravat/annotator_template/data/
--rw-r--r--   0 kyle      (1000) kyle      (1000)        0 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/annotator_template/data/annotator_template.sqlite
--rw-r--r--   0 kyle      (1000) kyle      (1000)    28521 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/base_annotator.py
--rw-r--r--   0 kyle      (1000) kyle      (1000)     2074 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/base_commonmodule.py
--rw-r--r--   0 kyle      (1000) kyle      (1000)     1259 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/base_converter.py
--rw-r--r--   0 kyle      (1000) kyle      (1000)    16380 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/base_mapper.py
--rw-r--r--   0 kyle      (1000) kyle      (1000)    12272 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/base_postaggregator.py
--rw-r--r--   0 kyle      (1000) kyle      (1000)    20758 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/base_summarizer.py
--rw-r--r--   0 kyle      (1000) kyle      (1000)     5266 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/config_loader.py
--rw-r--r--   0 kyle      (1000) kyle      (1000)    11749 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/constants.py
--rw-r--r--   0 kyle      (1000) kyle      (1000)      475 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/cravat-system.template.yml
--rw-r--r--   0 kyle      (1000) kyle      (1000)       80 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/cravat.yml
--rw-r--r--   0 kyle      (1000) kyle      (1000)    32368 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/cravat_admin.py
--rw-r--r--   0 kyle      (1000) kyle      (1000)    85860 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/cravat_class.py
--rw-r--r--   0 kyle      (1000) kyle      (1000)    31397 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/cravat_convert.py
--rw-r--r--   0 kyle      (1000) kyle      (1000)    38318 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/cravat_filter.py
--rw-r--r--   0 kyle      (1000) kyle      (1000)     6424 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/cravat_metrics.py
--rw-r--r--   0 kyle      (1000) kyle      (1000)     1969 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/cravat_pack.py
--rw-r--r--   0 kyle      (1000) kyle      (1000)    51145 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/cravat_report.py
--rw-r--r--   0 kyle      (1000) kyle      (1000)    32133 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/cravat_test.py
--rw-r--r--   0 kyle      (1000) kyle      (1000)    56209 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/cravat_util.py
--rw-r--r--   0 kyle      (1000) kyle      (1000)    20139 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/cravat_web.py
--rw-r--r--   0 kyle      (1000) kyle      (1000)     9036 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/example_input
--rw-r--r--   0 kyle      (1000) kyle      (1000)     1245 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/exceptions.py
--rw-r--r--   0 kyle      (1000) kyle      (1000)    19266 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/inout.py
-drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2023-03-13 12:57:17.782377 open-cravat-2.3.0/cravat/liftover/
--rw-r--r--   0 kyle      (1000) kyle      (1000)   931825 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/liftover/hg18ToHg38.over.chain
--rw-r--r--   0 kyle      (1000) kyle      (1000)   606773 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/liftover/hg19ToHg38.over.chain
--rw-r--r--   0 kyle      (1000) kyle      (1000)     2992 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/mp_runners.py
--rw-r--r--   0 kyle      (1000) kyle      (1000)     7061 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/oc.py
--rw-r--r--   0 kyle      (1000) kyle      (1000)      295 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/runcravat.py
--rw-r--r--   0 kyle      (1000) kyle      (1000)    10553 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/store_utils.py
--rw-r--r--   0 kyle      (1000) kyle      (1000)    10935 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/util.py
-drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2023-03-13 12:57:17.783377 open-cravat-2.3.0/cravat/webresult/
--rw-r--r--   0 kyle      (1000) kyle      (1000)        0 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/webresult/__init__.py
--rw-r--r--   0 kyle      (1000) kyle      (1000)    16774 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/webresult/cravat_view.py
-drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2023-03-13 12:57:17.783377 open-cravat-2.3.0/cravat/webresult/css/
--rw-r--r--   0 kyle      (1000) kyle      (1000)     2389 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/webresult/css/pqselect.min.css
--rw-r--r--   0 kyle      (1000) kyle      (1000)     4948 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/webresult/email.png
--rw-r--r--   0 kyle      (1000) kyle      (1000)      591 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/webresult/favicon.ico
--rw-r--r--   0 kyle      (1000) kyle      (1000)     1351 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/webresult/favicon.png
-drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2023-03-13 12:57:17.784377 open-cravat-2.3.0/cravat/webresult/fonts/
--rw-r--r--   0 kyle      (1000) kyle      (1000)    26456 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/webresult/fonts/roboto-bold-webfont.woff
--rw-r--r--   0 kyle      (1000) kyle      (1000)    19508 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/webresult/fonts/roboto-bold-webfont.woff2
--rw-r--r--   0 kyle      (1000) kyle      (1000)    25692 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/webresult/fonts/roboto-light-webfont.woff
--rw-r--r--   0 kyle      (1000) kyle      (1000)    18980 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/webresult/fonts/roboto-light-webfont.woff2
--rw-r--r--   0 kyle      (1000) kyle      (1000)    26312 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/webresult/fonts/roboto-medium-webfont.woff
--rw-r--r--   0 kyle      (1000) kyle      (1000)    19416 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/webresult/fonts/roboto-medium-webfont.woff2
--rw-r--r--   0 kyle      (1000) kyle      (1000)    33072 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/webresult/fonts/sourcesanspro-bold-webfont.woff
--rw-r--r--   0 kyle      (1000) kyle      (1000)    25740 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/webresult/fonts/sourcesanspro-bold-webfont.woff2
-drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2023-03-13 12:57:17.787377 open-cravat-2.3.0/cravat/webresult/images/
--rw-r--r--   0 kyle      (1000) kyle      (1000)      350 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/webresult/images/arrow-90deg-down.svg
--rw-r--r--   0 kyle      (1000) kyle      (1000)      326 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/webresult/images/arrow-down-right-circle-fill.svg
--rw-r--r--   0 kyle      (1000) kyle      (1000)      379 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/webresult/images/arrow-down-right-circle.svg
--rw-r--r--   0 kyle      (1000) kyle      (1000)      289 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/webresult/images/arrow-down-right.svg
--rw-r--r--   0 kyle      (1000) kyle      (1000)      309 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/webresult/images/arrow-down.svg
--rw-r--r--   0 kyle      (1000) kyle      (1000)      311 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/webresult/images/arrow-left.svg
--rw-r--r--   0 kyle      (1000) kyle      (1000)      312 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/webresult/images/arrow-right.svg
--rw-r--r--   0 kyle      (1000) kyle      (1000)      815 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/webresult/images/arrow-spinner-static.gif
--rw-r--r--   0 kyle      (1000) kyle      (1000)     6792 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/webresult/images/arrow-spinner.gif
--rw-r--r--   0 kyle      (1000) kyle      (1000)      309 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/webresult/images/arrow-up.svg
--rw-r--r--   0 kyle      (1000) kyle      (1000)      706 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/webresult/images/arrows-move.svg
--rw-r--r--   0 kyle      (1000) kyle      (1000)    12538 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/webresult/images/back_arrow.png
--rw-r--r--   0 kyle      (1000) kyle      (1000)   264317 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/webresult/images/bigSpinner.gif
--rw-r--r--   0 kyle      (1000) kyle      (1000)     2302 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/webresult/images/camera.png
--rw-r--r--   0 kyle      (1000) kyle      (1000)     2140 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/webresult/images/camera.svg
--rw-r--r--   0 kyle      (1000) kyle      (1000)      291 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/webresult/images/caret-down.svg
--rw-r--r--   0 kyle      (1000) kyle      (1000)      289 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/webresult/images/caret-right.svg
--rw-r--r--   0 kyle      (1000) kyle      (1000)      916 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/webresult/images/close-button.png
--rw-r--r--   0 kyle      (1000) kyle      (1000)     3125 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/webresult/images/close.png
--rw-r--r--   0 kyle      (1000) kyle      (1000)     2390 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/webresult/images/close.svg
--rw-r--r--   0 kyle      (1000) kyle      (1000)     1160 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/webresult/images/close_icon.png
--rw-r--r--   0 kyle      (1000) kyle      (1000)      722 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/webresult/images/download-material-black.png
--rw-r--r--   0 kyle      (1000) kyle      (1000)     7432 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/webresult/images/download-material-blue.png
--rw-r--r--   0 kyle      (1000) kyle      (1000)      263 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/webresult/images/download.png
--rw-r--r--   0 kyle      (1000) kyle      (1000)     2066 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/webresult/images/download.svg
--rw-r--r--   0 kyle      (1000) kyle      (1000)      378 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/webresult/images/download12.png
--rw-r--r--   0 kyle      (1000) kyle      (1000)      485 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/webresult/images/grip-vertical.svg
--rw-r--r--   0 kyle      (1000) kyle      (1000)      591 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/webresult/images/help_16x16.gif
--rw-r--r--   0 kyle      (1000) kyle      (1000)     7061 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/webresult/images/help_icon.png
--rw-r--r--   0 kyle      (1000) kyle      (1000)    32137 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/webresult/images/loading-gif-animation.gif
--rw-r--r--   0 kyle      (1000) kyle      (1000)     2056 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/webresult/images/mail.png
--rw-r--r--   0 kyle      (1000) kyle      (1000)     1211 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/webresult/images/menu.png
--rw-r--r--   0 kyle      (1000) kyle      (1000)      200 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/webresult/images/minus.png
--rw-r--r--   0 kyle      (1000) kyle      (1000)     1568 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/webresult/images/openNewTab.png
--rw-r--r--   0 kyle      (1000) kyle      (1000)     5131 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/webresult/images/package.png
--rw-r--r--   0 kyle      (1000) kyle      (1000)     1703 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/webresult/images/pencil.png
--rw-r--r--   0 kyle      (1000) kyle      (1000)      805 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/webresult/images/pin-2.png
--rw-r--r--   0 kyle      (1000) kyle      (1000)      698 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/webresult/images/pin.png
--rw-r--r--   0 kyle      (1000) kyle      (1000)     2219 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/webresult/images/pin.svg
--rw-r--r--   0 kyle      (1000) kyle      (1000)     2243 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/webresult/images/plus-circle-dotted.svg
--rw-r--r--   0 kyle      (1000) kyle      (1000)      280 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/webresult/images/plus-circle-fill.svg
--rw-r--r--   0 kyle      (1000) kyle      (1000)      217 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/webresult/images/plus.png
--rw-r--r--   0 kyle      (1000) kyle      (1000)     3324 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/webresult/images/question.png
--rw-r--r--   0 kyle      (1000) kyle      (1000)    13026 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/webresult/images/resize.jpg
--rw-r--r--   0 kyle      (1000) kyle      (1000)     3498 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/webresult/images/save.png
--rw-r--r--   0 kyle      (1000) kyle      (1000)     1408 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/webresult/images/save_new.png
--rw-r--r--   0 kyle      (1000) kyle      (1000)    25171 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/webresult/images/search.png
--rw-r--r--   0 kyle      (1000) kyle      (1000)     4645 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/webresult/images/sorry.png
--rw-r--r--   0 kyle      (1000) kyle      (1000)    55605 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/webresult/images/spinCircle.gif
--rw-r--r--   0 kyle      (1000) kyle      (1000)    25333 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/webresult/images/spinner.gif
--rw-r--r--   0 kyle      (1000) kyle      (1000)     1106 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/webresult/images/triangle-down.png
--rw-r--r--   0 kyle      (1000) kyle      (1000)     1112 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/webresult/images/triangle-right.png
--rw-r--r--   0 kyle      (1000) kyle      (1000)      733 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/webresult/images/upload-material-black.png
--rw-r--r--   0 kyle      (1000) kyle      (1000)     7573 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/webresult/images/upload-material-blue.png
--rw-r--r--   0 kyle      (1000) kyle      (1000)      340 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/webresult/images/x-lg.svg
--rw-r--r--   0 kyle      (1000) kyle      (1000)      332 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/webresult/images/x.svg
--rw-r--r--   0 kyle      (1000) kyle      (1000)     5924 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/webresult/index.html
-drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2023-03-13 12:57:17.789377 open-cravat-2.3.0/cravat/webresult/js/
--rw-r--r--   0 kyle      (1000) kyle      (1000)   398184 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/webresult/js/Chart.js
--rw-r--r--   0 kyle      (1000) kyle      (1000)     9279 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/webresult/js/dom-to-image.min.js
--rw-r--r--   0 kyle      (1000) kyle      (1000)     6000 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/webresult/js/download.js
--rw-r--r--   0 kyle      (1000) kyle      (1000)   954164 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/webresult/js/graphics.js
--rw-r--r--   0 kyle      (1000) kyle      (1000)    86659 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/webresult/js/jquery-3.2.1.min.js
-drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2023-03-13 12:57:17.790377 open-cravat-2.3.0/cravat/webresult/js/jquery-ui-1.12.1.custom/
--rw-r--r--   0 kyle      (1000) kyle      (1000)    12660 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/webresult/js/jquery-ui-1.12.1.custom/AUTHORS.txt
--rw-r--r--   0 kyle      (1000) kyle      (1000)     1817 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/webresult/js/jquery-ui-1.12.1.custom/LICENSE.txt
-drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2023-03-13 12:57:17.778377 open-cravat-2.3.0/cravat/webresult/js/jquery-ui-1.12.1.custom/external/
-drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2023-03-13 12:57:17.790377 open-cravat-2.3.0/cravat/webresult/js/jquery-ui-1.12.1.custom/external/jquery/
--rw-r--r--   0 kyle      (1000) kyle      (1000)   293430 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/webresult/js/jquery-ui-1.12.1.custom/external/jquery/jquery.js
-drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2023-03-13 12:57:17.790377 open-cravat-2.3.0/cravat/webresult/js/jquery-ui-1.12.1.custom/images/
--rw-r--r--   0 kyle      (1000) kyle      (1000)     6992 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/webresult/js/jquery-ui-1.12.1.custom/images/ui-icons_444444_256x240.png
--rw-r--r--   0 kyle      (1000) kyle      (1000)     6988 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/webresult/js/jquery-ui-1.12.1.custom/images/ui-icons_555555_256x240.png
--rw-r--r--   0 kyle      (1000) kyle      (1000)     4549 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/webresult/js/jquery-ui-1.12.1.custom/images/ui-icons_777620_256x240.png
--rw-r--r--   0 kyle      (1000) kyle      (1000)     6999 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/webresult/js/jquery-ui-1.12.1.custom/images/ui-icons_777777_256x240.png
--rw-r--r--   0 kyle      (1000) kyle      (1000)     4549 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/webresult/js/jquery-ui-1.12.1.custom/images/ui-icons_cc0000_256x240.png
--rw-r--r--   0 kyle      (1000) kyle      (1000)     6299 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/webresult/js/jquery-ui-1.12.1.custom/images/ui-icons_ffffff_256x240.png
--rw-r--r--   0 kyle      (1000) kyle      (1000)    32588 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/webresult/js/jquery-ui-1.12.1.custom/index.html
--rw-r--r--   0 kyle      (1000) kyle      (1000)    35997 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.css
--rw-r--r--   0 kyle      (1000) kyle      (1000)   520714 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.js
--rw-r--r--   0 kyle      (1000) kyle      (1000)    30747 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.min.css
--rw-r--r--   0 kyle      (1000) kyle      (1000)   253668 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.min.js
--rw-r--r--   0 kyle      (1000) kyle      (1000)    18705 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.structure.css
--rw-r--r--   0 kyle      (1000) kyle      (1000)    15548 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.structure.min.css
--rw-r--r--   0 kyle      (1000) kyle      (1000)    17342 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.theme.css
--rw-r--r--   0 kyle      (1000) kyle      (1000)    13847 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.theme.min.css
--rw-r--r--   0 kyle      (1000) kyle      (1000)     1340 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/webresult/js/jquery-ui-1.12.1.custom/package.json
--rw-r--r--   0 kyle      (1000) kyle      (1000)    13171 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/webresult/js/jquery.tools.min.js
--rw-r--r--   0 kyle      (1000) kyle      (1000)     5451 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/webresult/js/jquery.url.js
--rw-r--r--   0 kyle      (1000) kyle      (1000)    84772 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/webresult/js/packery.pkgd.js
-drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2023-03-13 12:57:17.791377 open-cravat-2.3.0/cravat/webresult/js/paramquery-pro-3/
--rw-r--r--   0 kyle      (1000) kyle      (1000)    11951 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/webresult/js/paramquery-pro-3/ChangeLog.txt
--rw-r--r--   0 kyle      (1000) kyle      (1000)   103213 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/webresult/js/paramquery-pro-3/EULA.pdf
-drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2023-03-13 12:57:17.792377 open-cravat-2.3.0/cravat/webresult/js/paramquery-pro-3/images/
--rw-r--r--   0 kyle      (1000) kyle      (1000)      230 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/webresult/js/paramquery-pro-3/images/horiz-bg.png
--rw-r--r--   0 kyle      (1000) kyle      (1000)      210 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/webresult/js/paramquery-pro-3/images/horiz-slider-bg.png
--rw-r--r--   0 kyle      (1000) kyle      (1000)      771 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/webresult/js/paramquery-pro-3/images/loading.gif
--rw-r--r--   0 kyle      (1000) kyle      (1000)     1668 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/webresult/js/paramquery-pro-3/images/sprite.png
--rw-r--r--   0 kyle      (1000) kyle      (1000)       51 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/webresult/js/paramquery-pro-3/images/square-blue-tr.gif
--rw-r--r--   0 kyle      (1000) kyle      (1000)       51 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/webresult/js/paramquery-pro-3/images/square-red-rb.gif
--rw-r--r--   0 kyle      (1000) kyle      (1000)       51 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/webresult/js/paramquery-pro-3/images/square-red-tr.gif
--rw-r--r--   0 kyle      (1000) kyle      (1000)       76 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/webresult/js/paramquery-pro-3/images/square_dirty.gif
--rw-r--r--   0 kyle      (1000) kyle      (1000)      216 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/webresult/js/paramquery-pro-3/images/vert-bg.png
--rw-r--r--   0 kyle      (1000) kyle      (1000)      201 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/webresult/js/paramquery-pro-3/images/vert-slider-bg.png
-drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2023-03-13 12:57:17.792377 open-cravat-2.3.0/cravat/webresult/js/paramquery-pro-3/jsZip-2.5.0/
--rw-r--r--   0 kyle      (1000) kyle      (1000)     1169 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/webresult/js/paramquery-pro-3/jsZip-2.5.0/MIT-License.txt
--rw-r--r--   0 kyle      (1000) kyle      (1000)    76985 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/webresult/js/paramquery-pro-3/jsZip-2.5.0/jszip.min.js
-drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2023-03-13 12:57:17.793377 open-cravat-2.3.0/cravat/webresult/js/paramquery-pro-3/localize/
--rw-r--r--   0 kyle      (1000) kyle      (1000)      755 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/webresult/js/paramquery-pro-3/localize/pq-localize-de.js
--rw-r--r--   0 kyle      (1000) kyle      (1000)      774 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/webresult/js/paramquery-pro-3/localize/pq-localize-en.js
--rw-r--r--   0 kyle      (1000) kyle      (1000)      794 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/webresult/js/paramquery-pro-3/localize/pq-localize-es.js
--rw-r--r--   0 kyle      (1000) kyle      (1000)      826 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/webresult/js/paramquery-pro-3/localize/pq-localize-fr.js
--rw-r--r--   0 kyle      (1000) kyle      (1000)      837 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/webresult/js/paramquery-pro-3/localize/pq-localize-hu.js
--rw-r--r--   0 kyle      (1000) kyle      (1000)      830 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/webresult/js/paramquery-pro-3/localize/pq-localize-it.js
--rw-r--r--   0 kyle      (1000) kyle      (1000)      661 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/webresult/js/paramquery-pro-3/localize/pq-localize-ja.js
--rw-r--r--   0 kyle      (1000) kyle      (1000)      796 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/webresult/js/paramquery-pro-3/localize/pq-localize-nl.js
--rw-r--r--   0 kyle      (1000) kyle      (1000)      808 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/webresult/js/paramquery-pro-3/localize/pq-localize-pl.js
--rw-r--r--   0 kyle      (1000) kyle      (1000)      847 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/webresult/js/paramquery-pro-3/localize/pq-localize-pt.js
--rw-r--r--   0 kyle      (1000) kyle      (1000)      797 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/webresult/js/paramquery-pro-3/localize/pq-localize-tr.js
--rw-r--r--   0 kyle      (1000) kyle      (1000)      700 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/webresult/js/paramquery-pro-3/localize/pq-localize-zh.js
-drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2023-03-13 12:57:17.793377 open-cravat-2.3.0/cravat/webresult/js/paramquery-pro-3/pqSelect/
--rw-r--r--   0 kyle      (1000) kyle      (1000)     1153 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/webresult/js/paramquery-pro-3/pqSelect/ChangeLog.txt
--rw-r--r--   0 kyle      (1000) kyle      (1000)      613 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/webresult/js/paramquery-pro-3/pqSelect/pqselect.bootstrap.dev.css
--rw-r--r--   0 kyle      (1000) kyle      (1000)      541 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/webresult/js/paramquery-pro-3/pqSelect/pqselect.bootstrap.min.css
--rw-r--r--   0 kyle      (1000) kyle      (1000)     2973 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/webresult/js/paramquery-pro-3/pqSelect/pqselect.dev.css
--rw-r--r--   0 kyle      (1000) kyle      (1000)    27759 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/webresult/js/paramquery-pro-3/pqSelect/pqselect.dev.js
--rw-r--r--   0 kyle      (1000) kyle      (1000)     2383 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/webresult/js/paramquery-pro-3/pqSelect/pqselect.min.css
--rw-r--r--   0 kyle      (1000) kyle      (1000)    12585 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/webresult/js/paramquery-pro-3/pqSelect/pqselect.min.js
--rw-r--r--   0 kyle      (1000) kyle      (1000)     2408 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/webresult/js/paramquery-pro-3/pqgrid.bootstrap.dev.css
--rw-r--r--   0 kyle      (1000) kyle      (1000)     2034 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/webresult/js/paramquery-pro-3/pqgrid.bootstrap.min.css
--rw-r--r--   0 kyle      (1000) kyle      (1000)    16186 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/webresult/js/paramquery-pro-3/pqgrid.dev.css
--rw-r--r--   0 kyle      (1000) kyle      (1000)   481365 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/webresult/js/paramquery-pro-3/pqgrid.dev.js
--rw-r--r--   0 kyle      (1000) kyle      (1000)    12765 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/webresult/js/paramquery-pro-3/pqgrid.min.css
--rw-r--r--   0 kyle      (1000) kyle      (1000)   242939 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/webresult/js/paramquery-pro-3/pqgrid.min.js
--rw-r--r--   0 kyle      (1000) kyle      (1000)     1646 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/webresult/js/paramquery-pro-3/pqgrid.ui.dev.css
--rw-r--r--   0 kyle      (1000) kyle      (1000)     1286 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/webresult/js/paramquery-pro-3/pqgrid.ui.min.css
--rw-r--r--   0 kyle      (1000) kyle      (1000)      587 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/webresult/js/paramquery-pro-3/readme.txt
-drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2023-03-13 12:57:17.779377 open-cravat-2.3.0/cravat/webresult/js/paramquery-pro-3/themes/
-drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2023-03-13 12:57:17.793377 open-cravat-2.3.0/cravat/webresult/js/paramquery-pro-3/themes/bootstrap/
--rw-r--r--   0 kyle      (1000) kyle      (1000)     4392 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/webresult/js/paramquery-pro-3/themes/bootstrap/pqgrid.css
-drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2023-03-13 12:57:17.793377 open-cravat-2.3.0/cravat/webresult/js/paramquery-pro-3/themes/brown/
--rw-r--r--   0 kyle      (1000) kyle      (1000)     4392 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/webresult/js/paramquery-pro-3/themes/brown/pqgrid.css
-drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2023-03-13 12:57:17.794377 open-cravat-2.3.0/cravat/webresult/js/paramquery-pro-3/themes/chocolate/
--rw-r--r--   0 kyle      (1000) kyle      (1000)     4392 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/webresult/js/paramquery-pro-3/themes/chocolate/pqgrid.css
-drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2023-03-13 12:57:17.794377 open-cravat-2.3.0/cravat/webresult/js/paramquery-pro-3/themes/cocoa/
--rw-r--r--   0 kyle      (1000) kyle      (1000)     4392 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/webresult/js/paramquery-pro-3/themes/cocoa/pqgrid.css
-drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2023-03-13 12:57:17.794377 open-cravat-2.3.0/cravat/webresult/js/paramquery-pro-3/themes/crimson/
--rw-r--r--   0 kyle      (1000) kyle      (1000)     4392 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/webresult/js/paramquery-pro-3/themes/crimson/pqgrid.css
-drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2023-03-13 12:57:17.794377 open-cravat-2.3.0/cravat/webresult/js/paramquery-pro-3/themes/gray/
--rw-r--r--   0 kyle      (1000) kyle      (1000)     4392 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/webresult/js/paramquery-pro-3/themes/gray/pqgrid.css
-drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2023-03-13 12:57:17.794377 open-cravat-2.3.0/cravat/webresult/js/paramquery-pro-3/themes/indigo/
--rw-r--r--   0 kyle      (1000) kyle      (1000)     4392 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/webresult/js/paramquery-pro-3/themes/indigo/pqgrid.css
-drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2023-03-13 12:57:17.794377 open-cravat-2.3.0/cravat/webresult/js/paramquery-pro-3/themes/office/
--rw-r--r--   0 kyle      (1000) kyle      (1000)     4392 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/webresult/js/paramquery-pro-3/themes/office/pqgrid.css
-drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2023-03-13 12:57:17.794377 open-cravat-2.3.0/cravat/webresult/js/paramquery-pro-3/themes/purple/
--rw-r--r--   0 kyle      (1000) kyle      (1000)     4392 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/webresult/js/paramquery-pro-3/themes/purple/pqgrid.css
-drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2023-03-13 12:57:17.794377 open-cravat-2.3.0/cravat/webresult/js/paramquery-pro-3/themes/red/
--rw-r--r--   0 kyle      (1000) kyle      (1000)     4392 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/webresult/js/paramquery-pro-3/themes/red/pqgrid.css
-drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2023-03-13 12:57:17.794377 open-cravat-2.3.0/cravat/webresult/js/paramquery-pro-3/themes/rosybrown/
--rw-r--r--   0 kyle      (1000) kyle      (1000)     4392 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/webresult/js/paramquery-pro-3/themes/rosybrown/pqgrid.css
-drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2023-03-13 12:57:17.794377 open-cravat-2.3.0/cravat/webresult/js/paramquery-pro-3/themes/sandybrown/
--rw-r--r--   0 kyle      (1000) kyle      (1000)     4392 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/webresult/js/paramquery-pro-3/themes/sandybrown/pqgrid.css
-drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2023-03-13 12:57:17.794377 open-cravat-2.3.0/cravat/webresult/js/paramquery-pro-3/themes/steelblue/
--rw-r--r--   0 kyle      (1000) kyle      (1000)     4392 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/webresult/js/paramquery-pro-3/themes/steelblue/pqgrid.css
-drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2023-03-13 12:57:17.794377 open-cravat-2.3.0/cravat/webresult/js/paramquery-pro-3/themes/tan/
--rw-r--r--   0 kyle      (1000) kyle      (1000)     4392 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/webresult/js/paramquery-pro-3/themes/tan/pqgrid.css
-drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2023-03-13 12:57:17.794377 open-cravat-2.3.0/cravat/webresult/js/paramquery-pro-3/themes/violet/
--rw-r--r--   0 kyle      (1000) kyle      (1000)     4392 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/webresult/js/paramquery-pro-3/themes/violet/pqgrid.css
-drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2023-03-13 12:57:17.795377 open-cravat-2.3.0/cravat/webresult/js/paramquery-pro-3/touch-punch/
--rw-r--r--   0 kyle      (1000) kyle      (1000)     1071 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/webresult/js/paramquery-pro-3/touch-punch/ChangeLog.txt
--rw-r--r--   0 kyle      (1000) kyle      (1000)     1190 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/webresult/js/paramquery-pro-3/touch-punch/MIT-LICENSE.txt
--rw-r--r--   0 kyle      (1000) kyle      (1000)     2677 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/webresult/js/paramquery-pro-3/touch-punch/README.md
--rw-r--r--   0 kyle      (1000) kyle      (1000)     3716 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/webresult/js/paramquery-pro-3/touch-punch/touch-punch.dev.js
--rw-r--r--   0 kyle      (1000) kyle      (1000)     1847 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/webresult/js/paramquery-pro-3/touch-punch/touch-punch.min.js
--rw-r--r--   0 kyle      (1000) kyle      (1000)    12591 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/webresult/js/pqselect.min.js
--rw-r--r--   0 kyle      (1000) kyle      (1000)    92225 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/webresult/js/raphael-min.js
--rw-r--r--   0 kyle      (1000) kyle      (1000)     1530 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/webresult/jsonreporter.py
-drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2023-03-13 12:57:17.795377 open-cravat-2.3.0/cravat/webresult/nocache/
-drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2023-03-13 12:57:17.795377 open-cravat-2.3.0/cravat/webresult/nocache/css/
--rw-r--r--   0 kyle      (1000) kyle      (1000)     1714 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/webresult/nocache/css/singlevariantpage.css
--rw-r--r--   0 kyle      (1000) kyle      (1000)    20968 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/webresult/nocache/css/style.css
--rw-r--r--   0 kyle      (1000) kyle      (1000)     2920 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/webresult/nocache/css/widget.css
-drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2023-03-13 12:57:17.796377 open-cravat-2.3.0/cravat/webresult/nocache/js/
--rw-r--r--   0 kyle      (1000) kyle      (1000)    26685 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/webresult/nocache/js/filter.js
--rw-r--r--   0 kyle      (1000) kyle      (1000)    12500 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/webresult/nocache/js/infomgr.js
--rw-r--r--   0 kyle      (1000) kyle      (1000)    43155 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/webresult/nocache/js/main.js
--rw-r--r--   0 kyle      (1000) kyle      (1000)    99662 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/webresult/nocache/js/setup.js
--rw-r--r--   0 kyle      (1000) kyle      (1000)     7986 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/webresult/nocache/js/showvariant.js
--rw-r--r--   0 kyle      (1000) kyle      (1000)    35998 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/webresult/nocache/js/singlevariantpage.js
--rw-r--r--   0 kyle      (1000) kyle      (1000)    31708 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/webresult/nocache/js/util.js
--rw-r--r--   0 kyle      (1000) kyle      (1000)     1688 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/webresult/nocache/js/variables.js
--rw-r--r--   0 kyle      (1000) kyle      (1000)    20474 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/webresult/nocache/js/widgethelper.js
--rw-r--r--   0 kyle      (1000) kyle      (1000)     5535 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/webresult/nocache/variant.html
--rw-r--r--   0 kyle      (1000) kyle      (1000)    10263 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/webresult/question.png
--rw-r--r--   0 kyle      (1000) kyle      (1000)    30111 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/webresult/webresult.py
--rw-r--r--   0 kyle      (1000) kyle      (1000)      173 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/webresult/webviewer.yml
-drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2023-03-13 12:57:17.796377 open-cravat-2.3.0/cravat/webstore/
--rw-r--r--   0 kyle      (1000) kyle      (1000)        0 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/webstore/__init__.py
--rw-r--r--   0 kyle      (1000) kyle      (1000)     1365 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/webstore/cravat_store.css
--rw-r--r--   0 kyle      (1000) kyle      (1000)     1224 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/webstore/favicon.ico
-drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2023-03-13 12:57:17.797377 open-cravat-2.3.0/cravat/webstore/images/
--rw-r--r--   0 kyle      (1000) kyle      (1000)      446 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/webstore/images/chat-dots-fill.svg
--rw-r--r--   0 kyle      (1000) kyle      (1000)      740 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/webstore/images/chat-dots.svg
--rw-r--r--   0 kyle      (1000) kyle      (1000)      396 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/webstore/images/chat-left-text-fill.svg
--rw-r--r--   0 kyle      (1000) kyle      (1000)      545 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/webstore/images/chat-left-text.svg
--rw-r--r--   0 kyle      (1000) kyle      (1000)    22268 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/webstore/images/done.png
--rw-r--r--   0 kyle      (1000) kyle      (1000)     4948 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/webstore/images/email.png
--rw-r--r--   0 kyle      (1000) kyle      (1000)     2226 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/webstore/images/empty.png
--rw-r--r--   0 kyle      (1000) kyle      (1000)     1351 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/webstore/images/favicon.png
--rw-r--r--   0 kyle      (1000) kyle      (1000)     1763 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/webstore/images/folder.png
--rw-r--r--   0 kyle      (1000) kyle      (1000)    38197 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/webstore/images/genericmodulelogo.png
--rw-r--r--   0 kyle      (1000) kyle      (1000)     4766 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/webstore/images/hamburger.png
--rw-r--r--   0 kyle      (1000) kyle      (1000)     1194 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/webstore/images/left_arrow.png
--rw-r--r--   0 kyle      (1000) kyle      (1000)    67804 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/webstore/images/logo.png
--rw-r--r--   0 kyle      (1000) kyle      (1000)     3524 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/webstore/images/new.png
--rw-r--r--   0 kyle      (1000) kyle      (1000)    10263 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/webstore/images/question.png
--rw-r--r--   0 kyle      (1000) kyle      (1000)     1214 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/webstore/images/right_arrow.png
--rw-r--r--   0 kyle      (1000) kyle      (1000)      340 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/webstore/images/x-lg.svg
--rw-r--r--   0 kyle      (1000) kyle      (1000)    86927 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/webstore/jquery-3.3.1.min.js
-drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2023-03-13 12:57:17.797377 open-cravat-2.3.0/cravat/webstore/js/
--rw-r--r--   0 kyle      (1000) kyle      (1000)    75673 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/webstore/js/showdown-1.9.1.min.js
--rw-r--r--   0 kyle      (1000) kyle      (1000)    91924 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/webstore/js/showdown.min.js.map
-drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2023-03-13 12:57:17.797377 open-cravat-2.3.0/cravat/webstore/nocache/
--rw-r--r--   0 kyle      (1000) kyle      (1000)    15017 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/webstore/nocache/webstore.css
--rw-r--r--   0 kyle      (1000) kyle      (1000)    95532 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/webstore/nocache/webstore.js
--rw-r--r--   0 kyle      (1000) kyle      (1000)     2342 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/webstore/sse.py
--rw-r--r--   0 kyle      (1000) kyle      (1000)     1700 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/webstore/store_handlers.py
--rw-r--r--   0 kyle      (1000) kyle      (1000)    16522 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/webstore/webstore.py
--rw-r--r--   0 kyle      (1000) kyle      (1000)      283 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/webstore/ws.html
--rw-r--r--   0 kyle      (1000) kyle      (1000)      720 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/webstore/ws.js
-drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2023-03-13 12:57:17.799377 open-cravat-2.3.0/cravat/websubmit/
--rw-r--r--   0 kyle      (1000) kyle      (1000)       11 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/websubmit/.gitignore
--rw-r--r--   0 kyle      (1000) kyle      (1000)   210024 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/websubmit/Chart.bundle.min.js
--rw-r--r--   0 kyle      (1000) kyle      (1000)        0 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/websubmit/__init__.py
--rw-r--r--   0 kyle      (1000) kyle      (1000)      719 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/websubmit/arrow.png
--rw-r--r--   0 kyle      (1000) kyle      (1000)     2291 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/websubmit/down.png
--rw-r--r--   0 kyle      (1000) kyle      (1000)     4948 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/websubmit/email.png
--rw-r--r--   0 kyle      (1000) kyle      (1000)     1224 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/websubmit/favicon.ico
--rw-r--r--   0 kyle      (1000) kyle      (1000)     1351 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/websubmit/favicon.png
--rw-r--r--   0 kyle      (1000) kyle      (1000)      108 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/websubmit/googleAnalytics.js
--rw-r--r--   0 kyle      (1000) kyle      (1000)     1052 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/websubmit/help.png
-drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2023-03-13 12:57:17.799377 open-cravat-2.3.0/cravat/websubmit/input-examples/
--rw-r--r--   0 kyle      (1000) kyle      (1000)      527 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/websubmit/input-examples/cravat.hg18.txt
--rw-r--r--   0 kyle      (1000) kyle      (1000)      529 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/websubmit/input-examples/cravat.hg19.txt
--rw-r--r--   0 kyle      (1000) kyle      (1000)      529 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/websubmit/input-examples/cravat.hg38.txt
--rw-r--r--   0 kyle      (1000) kyle      (1000)     2199 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/websubmit/input-examples/vcf.hg18.txt
--rw-r--r--   0 kyle      (1000) kyle      (1000)     2199 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/websubmit/input-examples/vcf.hg19.txt
--rw-r--r--   0 kyle      (1000) kyle      (1000)     2199 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/websubmit/input-examples/vcf.hg38.txt
--rw-r--r--   0 kyle      (1000) kyle      (1000)    86927 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/websubmit/jquery-3.3.1.min.js
--rw-r--r--   0 kyle      (1000) kyle      (1000)    53784 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/websubmit/logo.png
--rw-r--r--   0 kyle      (1000) kyle      (1000)    56098 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/websubmit/logo_transparent.png
--rw-r--r--   0 kyle      (1000) kyle      (1000)      225 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/websubmit/menu.png
-drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2023-03-13 12:57:17.800377 open-cravat-2.3.0/cravat/websubmit/nocache/
--rw-r--r--   0 kyle      (1000) kyle      (1000)    13800 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/websubmit/nocache/broken_wheel.gif
--rw-r--r--   0 kyle      (1000) kyle      (1000)    18796 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/websubmit/nocache/index.html
--rw-r--r--   0 kyle      (1000) kyle      (1000)    17372 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/websubmit/nocache/websubmit.css
--rw-r--r--   0 kyle      (1000) kyle      (1000)    83472 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/websubmit/nocache/websubmit.js
--rw-r--r--   0 kyle      (1000) kyle      (1000)    11488 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/websubmit/nointernet.png
--rw-r--r--   0 kyle      (1000) kyle      (1000)    27869 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/websubmit/pqselect.dev.customforsubmit.js
--rw-r--r--   0 kyle      (1000) kyle      (1000)    10263 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/websubmit/question.png
--rw-r--r--   0 kyle      (1000) kyle      (1000)     2167 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/websubmit/refresh.png
--rw-r--r--   0 kyle      (1000) kyle      (1000)      280 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/websubmit/threedots.png
--rw-r--r--   0 kyle      (1000) kyle      (1000)    48552 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/websubmit/websubmit.py
--rw-r--r--   0 kyle      (1000) kyle      (1000)     3724 2023-03-13 12:57:17.000000 open-cravat-2.3.0/cravat/wincravat.pyw
-drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2023-03-13 12:57:17.800377 open-cravat-2.3.0/open_cravat.egg-info/
--rw-r--r--   0 kyle      (1000) kyle      (1000)     1056 2023-03-13 12:57:17.000000 open-cravat-2.3.0/open_cravat.egg-info/PKG-INFO
--rw-r--r--   0 kyle      (1000) kyle      (1000)    12262 2023-03-13 12:57:17.000000 open-cravat-2.3.0/open_cravat.egg-info/SOURCES.txt
--rw-r--r--   0 kyle      (1000) kyle      (1000)        1 2023-03-13 12:57:17.000000 open-cravat-2.3.0/open_cravat.egg-info/dependency_links.txt
--rw-r--r--   0 kyle      (1000) kyle      (1000)       38 2023-03-13 12:57:17.000000 open-cravat-2.3.0/open_cravat.egg-info/entry_points.txt
--rw-r--r--   0 kyle      (1000) kyle      (1000)      184 2023-03-13 12:57:17.000000 open-cravat-2.3.0/open_cravat.egg-info/requires.txt
--rw-r--r--   0 kyle      (1000) kyle      (1000)        7 2023-03-13 12:57:17.000000 open-cravat-2.3.0/open_cravat.egg-info/top_level.txt
--rw-r--r--   0 kyle      (1000) kyle      (1000)       38 2023-03-13 12:57:17.800377 open-cravat-2.3.0/setup.cfg
--rw-r--r--   0 kyle      (1000) kyle      (1000)     2877 2023-03-13 12:57:17.000000 open-cravat-2.3.0/setup.py
+drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2023-05-22 17:05:46.089460 open-cravat-2.3.1/
+-rw-r--r--   0 kyle      (1000) kyle      (1000)     1067 2023-05-22 17:05:45.000000 open-cravat-2.3.1/LICENSE
+-rw-r--r--   0 kyle      (1000) kyle      (1000)     1056 2023-05-22 17:05:46.089460 open-cravat-2.3.1/PKG-INFO
+-rw-r--r--   0 kyle      (1000) kyle      (1000)      769 2023-05-22 17:05:45.000000 open-cravat-2.3.1/README.rst
+drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2023-05-22 17:05:46.062460 open-cravat-2.3.1/cravat/
+-rw-r--r--   0 kyle      (1000) kyle      (1000)     6364 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/__init__.py
+-rw-r--r--   0 kyle      (1000) kyle      (1000)    60557 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/admin_util.py
+-rw-r--r--   0 kyle      (1000) kyle      (1000)    19600 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/aggregator.py
+-rw-r--r--   0 kyle      (1000) kyle      (1000)     2990 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/annotator_options.py
+drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2023-05-22 17:05:46.063460 open-cravat-2.3.1/cravat/annotator_template/
+-rw-r--r--   0 kyle      (1000) kyle      (1000)      178 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/annotator_template/annotator_template.md
+-rw-r--r--   0 kyle      (1000) kyle      (1000)     2326 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/annotator_template/annotator_template.py
+-rw-r--r--   0 kyle      (1000) kyle      (1000)     1460 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/annotator_template/annotator_template.yml
+drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2023-05-22 17:05:46.063460 open-cravat-2.3.1/cravat/annotator_template/data/
+-rw-r--r--   0 kyle      (1000) kyle      (1000)        0 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/annotator_template/data/annotator_template.sqlite
+-rw-r--r--   0 kyle      (1000) kyle      (1000)    28521 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/base_annotator.py
+-rw-r--r--   0 kyle      (1000) kyle      (1000)     2074 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/base_commonmodule.py
+-rw-r--r--   0 kyle      (1000) kyle      (1000)     1259 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/base_converter.py
+-rw-r--r--   0 kyle      (1000) kyle      (1000)    16953 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/base_mapper.py
+-rw-r--r--   0 kyle      (1000) kyle      (1000)    12209 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/base_postaggregator.py
+-rw-r--r--   0 kyle      (1000) kyle      (1000)    20758 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/base_summarizer.py
+-rw-r--r--   0 kyle      (1000) kyle      (1000)     5266 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/config_loader.py
+-rw-r--r--   0 kyle      (1000) kyle      (1000)    11775 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/constants.py
+-rw-r--r--   0 kyle      (1000) kyle      (1000)      475 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/cravat-system.template.yml
+-rw-r--r--   0 kyle      (1000) kyle      (1000)       80 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/cravat.yml
+-rw-r--r--   0 kyle      (1000) kyle      (1000)    32368 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/cravat_admin.py
+-rw-r--r--   0 kyle      (1000) kyle      (1000)    85512 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/cravat_class.py
+-rw-r--r--   0 kyle      (1000) kyle      (1000)    31453 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/cravat_convert.py
+-rw-r--r--   0 kyle      (1000) kyle      (1000)    38094 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/cravat_filter.py
+-rw-r--r--   0 kyle      (1000) kyle      (1000)     6424 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/cravat_metrics.py
+-rw-r--r--   0 kyle      (1000) kyle      (1000)     1969 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/cravat_pack.py
+-rw-r--r--   0 kyle      (1000) kyle      (1000)    51336 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/cravat_report.py
+-rw-r--r--   0 kyle      (1000) kyle      (1000)    32133 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/cravat_test.py
+-rw-r--r--   0 kyle      (1000) kyle      (1000)    56209 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/cravat_util.py
+-rw-r--r--   0 kyle      (1000) kyle      (1000)    20271 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/cravat_web.py
+-rw-r--r--   0 kyle      (1000) kyle      (1000)     9036 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/example_input
+-rw-r--r--   0 kyle      (1000) kyle      (1000)     1245 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/exceptions.py
+-rw-r--r--   0 kyle      (1000) kyle      (1000)    19368 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/inout.py
+drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2023-05-22 17:05:46.063460 open-cravat-2.3.1/cravat/liftover/
+-rw-r--r--   0 kyle      (1000) kyle      (1000)   931825 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/liftover/hg18ToHg38.over.chain
+-rw-r--r--   0 kyle      (1000) kyle      (1000)   606773 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/liftover/hg19ToHg38.over.chain
+-rw-r--r--   0 kyle      (1000) kyle      (1000)     2992 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/mp_runners.py
+-rw-r--r--   0 kyle      (1000) kyle      (1000)     7061 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/oc.py
+-rw-r--r--   0 kyle      (1000) kyle      (1000)      295 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/runcravat.py
+-rw-r--r--   0 kyle      (1000) kyle      (1000)    10553 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/store_utils.py
+-rw-r--r--   0 kyle      (1000) kyle      (1000)    10935 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/util.py
+drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2023-05-22 17:05:46.064460 open-cravat-2.3.1/cravat/webresult/
+-rw-r--r--   0 kyle      (1000) kyle      (1000)        0 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/webresult/__init__.py
+-rw-r--r--   0 kyle      (1000) kyle      (1000)    16774 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/webresult/cravat_view.py
+drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2023-05-22 17:05:46.064460 open-cravat-2.3.1/cravat/webresult/css/
+-rw-r--r--   0 kyle      (1000) kyle      (1000)     2389 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/webresult/css/pqselect.min.css
+-rw-r--r--   0 kyle      (1000) kyle      (1000)     4948 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/webresult/email.png
+-rw-r--r--   0 kyle      (1000) kyle      (1000)      591 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/webresult/favicon.ico
+-rw-r--r--   0 kyle      (1000) kyle      (1000)     1351 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/webresult/favicon.png
+drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2023-05-22 17:05:46.065460 open-cravat-2.3.1/cravat/webresult/fonts/
+-rw-r--r--   0 kyle      (1000) kyle      (1000)    26456 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/webresult/fonts/roboto-bold-webfont.woff
+-rw-r--r--   0 kyle      (1000) kyle      (1000)    19508 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/webresult/fonts/roboto-bold-webfont.woff2
+-rw-r--r--   0 kyle      (1000) kyle      (1000)    25692 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/webresult/fonts/roboto-light-webfont.woff
+-rw-r--r--   0 kyle      (1000) kyle      (1000)    18980 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/webresult/fonts/roboto-light-webfont.woff2
+-rw-r--r--   0 kyle      (1000) kyle      (1000)    26312 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/webresult/fonts/roboto-medium-webfont.woff
+-rw-r--r--   0 kyle      (1000) kyle      (1000)    19416 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/webresult/fonts/roboto-medium-webfont.woff2
+-rw-r--r--   0 kyle      (1000) kyle      (1000)    33072 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/webresult/fonts/sourcesanspro-bold-webfont.woff
+-rw-r--r--   0 kyle      (1000) kyle      (1000)    25740 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/webresult/fonts/sourcesanspro-bold-webfont.woff2
+drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2023-05-22 17:05:46.071460 open-cravat-2.3.1/cravat/webresult/images/
+-rw-r--r--   0 kyle      (1000) kyle      (1000)      350 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/webresult/images/arrow-90deg-down.svg
+-rw-r--r--   0 kyle      (1000) kyle      (1000)      326 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/webresult/images/arrow-down-right-circle-fill.svg
+-rw-r--r--   0 kyle      (1000) kyle      (1000)      379 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/webresult/images/arrow-down-right-circle.svg
+-rw-r--r--   0 kyle      (1000) kyle      (1000)      289 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/webresult/images/arrow-down-right.svg
+-rw-r--r--   0 kyle      (1000) kyle      (1000)      309 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/webresult/images/arrow-down.svg
+-rw-r--r--   0 kyle      (1000) kyle      (1000)      311 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/webresult/images/arrow-left.svg
+-rw-r--r--   0 kyle      (1000) kyle      (1000)      312 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/webresult/images/arrow-right.svg
+-rw-r--r--   0 kyle      (1000) kyle      (1000)      815 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/webresult/images/arrow-spinner-static.gif
+-rw-r--r--   0 kyle      (1000) kyle      (1000)     6792 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/webresult/images/arrow-spinner.gif
+-rw-r--r--   0 kyle      (1000) kyle      (1000)      309 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/webresult/images/arrow-up.svg
+-rw-r--r--   0 kyle      (1000) kyle      (1000)      706 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/webresult/images/arrows-move.svg
+-rw-r--r--   0 kyle      (1000) kyle      (1000)    12538 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/webresult/images/back_arrow.png
+-rw-r--r--   0 kyle      (1000) kyle      (1000)   264317 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/webresult/images/bigSpinner.gif
+-rw-r--r--   0 kyle      (1000) kyle      (1000)     2302 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/webresult/images/camera.png
+-rw-r--r--   0 kyle      (1000) kyle      (1000)     2140 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/webresult/images/camera.svg
+-rw-r--r--   0 kyle      (1000) kyle      (1000)      291 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/webresult/images/caret-down.svg
+-rw-r--r--   0 kyle      (1000) kyle      (1000)      289 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/webresult/images/caret-right.svg
+-rw-r--r--   0 kyle      (1000) kyle      (1000)      916 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/webresult/images/close-button.png
+-rw-r--r--   0 kyle      (1000) kyle      (1000)     3125 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/webresult/images/close.png
+-rw-r--r--   0 kyle      (1000) kyle      (1000)     2390 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/webresult/images/close.svg
+-rw-r--r--   0 kyle      (1000) kyle      (1000)     1160 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/webresult/images/close_icon.png
+-rw-r--r--   0 kyle      (1000) kyle      (1000)      722 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/webresult/images/download-material-black.png
+-rw-r--r--   0 kyle      (1000) kyle      (1000)     7432 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/webresult/images/download-material-blue.png
+-rw-r--r--   0 kyle      (1000) kyle      (1000)      263 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/webresult/images/download.png
+-rw-r--r--   0 kyle      (1000) kyle      (1000)     2066 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/webresult/images/download.svg
+-rw-r--r--   0 kyle      (1000) kyle      (1000)      378 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/webresult/images/download12.png
+-rw-r--r--   0 kyle      (1000) kyle      (1000)      485 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/webresult/images/grip-vertical.svg
+-rw-r--r--   0 kyle      (1000) kyle      (1000)      591 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/webresult/images/help_16x16.gif
+-rw-r--r--   0 kyle      (1000) kyle      (1000)     7061 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/webresult/images/help_icon.png
+-rw-r--r--   0 kyle      (1000) kyle      (1000)    32137 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/webresult/images/loading-gif-animation.gif
+-rw-r--r--   0 kyle      (1000) kyle      (1000)     2056 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/webresult/images/mail.png
+-rw-r--r--   0 kyle      (1000) kyle      (1000)     1211 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/webresult/images/menu.png
+-rw-r--r--   0 kyle      (1000) kyle      (1000)      200 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/webresult/images/minus.png
+-rw-r--r--   0 kyle      (1000) kyle      (1000)     1568 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/webresult/images/openNewTab.png
+-rw-r--r--   0 kyle      (1000) kyle      (1000)     5131 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/webresult/images/package.png
+-rw-r--r--   0 kyle      (1000) kyle      (1000)     1703 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/webresult/images/pencil.png
+-rw-r--r--   0 kyle      (1000) kyle      (1000)      805 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/webresult/images/pin-2.png
+-rw-r--r--   0 kyle      (1000) kyle      (1000)      698 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/webresult/images/pin.png
+-rw-r--r--   0 kyle      (1000) kyle      (1000)     2219 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/webresult/images/pin.svg
+-rw-r--r--   0 kyle      (1000) kyle      (1000)     2243 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/webresult/images/plus-circle-dotted.svg
+-rw-r--r--   0 kyle      (1000) kyle      (1000)      280 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/webresult/images/plus-circle-fill.svg
+-rw-r--r--   0 kyle      (1000) kyle      (1000)      217 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/webresult/images/plus.png
+-rw-r--r--   0 kyle      (1000) kyle      (1000)     3324 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/webresult/images/question.png
+-rw-r--r--   0 kyle      (1000) kyle      (1000)    13026 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/webresult/images/resize.jpg
+-rw-r--r--   0 kyle      (1000) kyle      (1000)     3498 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/webresult/images/save.png
+-rw-r--r--   0 kyle      (1000) kyle      (1000)     1408 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/webresult/images/save_new.png
+-rw-r--r--   0 kyle      (1000) kyle      (1000)    25171 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/webresult/images/search.png
+-rw-r--r--   0 kyle      (1000) kyle      (1000)     4645 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/webresult/images/sorry.png
+-rw-r--r--   0 kyle      (1000) kyle      (1000)    55605 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/webresult/images/spinCircle.gif
+-rw-r--r--   0 kyle      (1000) kyle      (1000)    25333 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/webresult/images/spinner.gif
+-rw-r--r--   0 kyle      (1000) kyle      (1000)     1106 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/webresult/images/triangle-down.png
+-rw-r--r--   0 kyle      (1000) kyle      (1000)     1112 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/webresult/images/triangle-right.png
+-rw-r--r--   0 kyle      (1000) kyle      (1000)      733 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/webresult/images/upload-material-black.png
+-rw-r--r--   0 kyle      (1000) kyle      (1000)     7573 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/webresult/images/upload-material-blue.png
+-rw-r--r--   0 kyle      (1000) kyle      (1000)      340 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/webresult/images/x-lg.svg
+-rw-r--r--   0 kyle      (1000) kyle      (1000)      332 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/webresult/images/x.svg
+-rw-r--r--   0 kyle      (1000) kyle      (1000)     5924 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/webresult/index.html
+drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2023-05-22 17:05:46.072460 open-cravat-2.3.1/cravat/webresult/js/
+-rw-r--r--   0 kyle      (1000) kyle      (1000)   398184 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/webresult/js/Chart.js
+-rw-r--r--   0 kyle      (1000) kyle      (1000)     9279 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/webresult/js/dom-to-image.min.js
+-rw-r--r--   0 kyle      (1000) kyle      (1000)     6000 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/webresult/js/download.js
+-rw-r--r--   0 kyle      (1000) kyle      (1000)   954164 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/webresult/js/graphics.js
+-rw-r--r--   0 kyle      (1000) kyle      (1000)    86659 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/webresult/js/jquery-3.2.1.min.js
+drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2023-05-22 17:05:46.074460 open-cravat-2.3.1/cravat/webresult/js/jquery-ui-1.12.1.custom/
+-rw-r--r--   0 kyle      (1000) kyle      (1000)    12660 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/webresult/js/jquery-ui-1.12.1.custom/AUTHORS.txt
+-rw-r--r--   0 kyle      (1000) kyle      (1000)     1817 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/webresult/js/jquery-ui-1.12.1.custom/LICENSE.txt
+drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2023-05-22 17:05:46.056460 open-cravat-2.3.1/cravat/webresult/js/jquery-ui-1.12.1.custom/external/
+drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2023-05-22 17:05:46.074460 open-cravat-2.3.1/cravat/webresult/js/jquery-ui-1.12.1.custom/external/jquery/
+-rw-r--r--   0 kyle      (1000) kyle      (1000)   293430 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/webresult/js/jquery-ui-1.12.1.custom/external/jquery/jquery.js
+drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2023-05-22 17:05:46.075460 open-cravat-2.3.1/cravat/webresult/js/jquery-ui-1.12.1.custom/images/
+-rw-r--r--   0 kyle      (1000) kyle      (1000)     6992 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/webresult/js/jquery-ui-1.12.1.custom/images/ui-icons_444444_256x240.png
+-rw-r--r--   0 kyle      (1000) kyle      (1000)     6988 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/webresult/js/jquery-ui-1.12.1.custom/images/ui-icons_555555_256x240.png
+-rw-r--r--   0 kyle      (1000) kyle      (1000)     4549 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/webresult/js/jquery-ui-1.12.1.custom/images/ui-icons_777620_256x240.png
+-rw-r--r--   0 kyle      (1000) kyle      (1000)     6999 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/webresult/js/jquery-ui-1.12.1.custom/images/ui-icons_777777_256x240.png
+-rw-r--r--   0 kyle      (1000) kyle      (1000)     4549 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/webresult/js/jquery-ui-1.12.1.custom/images/ui-icons_cc0000_256x240.png
+-rw-r--r--   0 kyle      (1000) kyle      (1000)     6299 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/webresult/js/jquery-ui-1.12.1.custom/images/ui-icons_ffffff_256x240.png
+-rw-r--r--   0 kyle      (1000) kyle      (1000)    32588 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/webresult/js/jquery-ui-1.12.1.custom/index.html
+-rw-r--r--   0 kyle      (1000) kyle      (1000)    35997 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.css
+-rw-r--r--   0 kyle      (1000) kyle      (1000)   520714 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.js
+-rw-r--r--   0 kyle      (1000) kyle      (1000)    30747 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.min.css
+-rw-r--r--   0 kyle      (1000) kyle      (1000)   253668 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.min.js
+-rw-r--r--   0 kyle      (1000) kyle      (1000)    18705 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.structure.css
+-rw-r--r--   0 kyle      (1000) kyle      (1000)    15548 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.structure.min.css
+-rw-r--r--   0 kyle      (1000) kyle      (1000)    17342 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.theme.css
+-rw-r--r--   0 kyle      (1000) kyle      (1000)    13847 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.theme.min.css
+-rw-r--r--   0 kyle      (1000) kyle      (1000)     1340 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/webresult/js/jquery-ui-1.12.1.custom/package.json
+-rw-r--r--   0 kyle      (1000) kyle      (1000)    13171 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/webresult/js/jquery.tools.min.js
+-rw-r--r--   0 kyle      (1000) kyle      (1000)     5451 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/webresult/js/jquery.url.js
+-rw-r--r--   0 kyle      (1000) kyle      (1000)    84772 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/webresult/js/packery.pkgd.js
+drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2023-05-22 17:05:46.076460 open-cravat-2.3.1/cravat/webresult/js/paramquery-pro-3/
+-rw-r--r--   0 kyle      (1000) kyle      (1000)    11951 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/webresult/js/paramquery-pro-3/ChangeLog.txt
+-rw-r--r--   0 kyle      (1000) kyle      (1000)   103213 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/webresult/js/paramquery-pro-3/EULA.pdf
+drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2023-05-22 17:05:46.077460 open-cravat-2.3.1/cravat/webresult/js/paramquery-pro-3/images/
+-rw-r--r--   0 kyle      (1000) kyle      (1000)      230 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/webresult/js/paramquery-pro-3/images/horiz-bg.png
+-rw-r--r--   0 kyle      (1000) kyle      (1000)      210 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/webresult/js/paramquery-pro-3/images/horiz-slider-bg.png
+-rw-r--r--   0 kyle      (1000) kyle      (1000)      771 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/webresult/js/paramquery-pro-3/images/loading.gif
+-rw-r--r--   0 kyle      (1000) kyle      (1000)     1668 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/webresult/js/paramquery-pro-3/images/sprite.png
+-rw-r--r--   0 kyle      (1000) kyle      (1000)       51 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/webresult/js/paramquery-pro-3/images/square-blue-tr.gif
+-rw-r--r--   0 kyle      (1000) kyle      (1000)       51 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/webresult/js/paramquery-pro-3/images/square-red-rb.gif
+-rw-r--r--   0 kyle      (1000) kyle      (1000)       51 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/webresult/js/paramquery-pro-3/images/square-red-tr.gif
+-rw-r--r--   0 kyle      (1000) kyle      (1000)       76 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/webresult/js/paramquery-pro-3/images/square_dirty.gif
+-rw-r--r--   0 kyle      (1000) kyle      (1000)      216 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/webresult/js/paramquery-pro-3/images/vert-bg.png
+-rw-r--r--   0 kyle      (1000) kyle      (1000)      201 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/webresult/js/paramquery-pro-3/images/vert-slider-bg.png
+drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2023-05-22 17:05:46.077460 open-cravat-2.3.1/cravat/webresult/js/paramquery-pro-3/jsZip-2.5.0/
+-rw-r--r--   0 kyle      (1000) kyle      (1000)     1169 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/webresult/js/paramquery-pro-3/jsZip-2.5.0/MIT-License.txt
+-rw-r--r--   0 kyle      (1000) kyle      (1000)    76985 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/webresult/js/paramquery-pro-3/jsZip-2.5.0/jszip.min.js
+drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2023-05-22 17:05:46.078460 open-cravat-2.3.1/cravat/webresult/js/paramquery-pro-3/localize/
+-rw-r--r--   0 kyle      (1000) kyle      (1000)      755 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/webresult/js/paramquery-pro-3/localize/pq-localize-de.js
+-rw-r--r--   0 kyle      (1000) kyle      (1000)      774 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/webresult/js/paramquery-pro-3/localize/pq-localize-en.js
+-rw-r--r--   0 kyle      (1000) kyle      (1000)      794 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/webresult/js/paramquery-pro-3/localize/pq-localize-es.js
+-rw-r--r--   0 kyle      (1000) kyle      (1000)      826 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/webresult/js/paramquery-pro-3/localize/pq-localize-fr.js
+-rw-r--r--   0 kyle      (1000) kyle      (1000)      837 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/webresult/js/paramquery-pro-3/localize/pq-localize-hu.js
+-rw-r--r--   0 kyle      (1000) kyle      (1000)      830 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/webresult/js/paramquery-pro-3/localize/pq-localize-it.js
+-rw-r--r--   0 kyle      (1000) kyle      (1000)      661 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/webresult/js/paramquery-pro-3/localize/pq-localize-ja.js
+-rw-r--r--   0 kyle      (1000) kyle      (1000)      796 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/webresult/js/paramquery-pro-3/localize/pq-localize-nl.js
+-rw-r--r--   0 kyle      (1000) kyle      (1000)      808 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/webresult/js/paramquery-pro-3/localize/pq-localize-pl.js
+-rw-r--r--   0 kyle      (1000) kyle      (1000)      847 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/webresult/js/paramquery-pro-3/localize/pq-localize-pt.js
+-rw-r--r--   0 kyle      (1000) kyle      (1000)      797 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/webresult/js/paramquery-pro-3/localize/pq-localize-tr.js
+-rw-r--r--   0 kyle      (1000) kyle      (1000)      700 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/webresult/js/paramquery-pro-3/localize/pq-localize-zh.js
+drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2023-05-22 17:05:46.079460 open-cravat-2.3.1/cravat/webresult/js/paramquery-pro-3/pqSelect/
+-rw-r--r--   0 kyle      (1000) kyle      (1000)     1153 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/webresult/js/paramquery-pro-3/pqSelect/ChangeLog.txt
+-rw-r--r--   0 kyle      (1000) kyle      (1000)      613 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/webresult/js/paramquery-pro-3/pqSelect/pqselect.bootstrap.dev.css
+-rw-r--r--   0 kyle      (1000) kyle      (1000)      541 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/webresult/js/paramquery-pro-3/pqSelect/pqselect.bootstrap.min.css
+-rw-r--r--   0 kyle      (1000) kyle      (1000)     2973 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/webresult/js/paramquery-pro-3/pqSelect/pqselect.dev.css
+-rw-r--r--   0 kyle      (1000) kyle      (1000)    27759 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/webresult/js/paramquery-pro-3/pqSelect/pqselect.dev.js
+-rw-r--r--   0 kyle      (1000) kyle      (1000)     2383 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/webresult/js/paramquery-pro-3/pqSelect/pqselect.min.css
+-rw-r--r--   0 kyle      (1000) kyle      (1000)    12585 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/webresult/js/paramquery-pro-3/pqSelect/pqselect.min.js
+-rw-r--r--   0 kyle      (1000) kyle      (1000)     2408 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/webresult/js/paramquery-pro-3/pqgrid.bootstrap.dev.css
+-rw-r--r--   0 kyle      (1000) kyle      (1000)     2034 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/webresult/js/paramquery-pro-3/pqgrid.bootstrap.min.css
+-rw-r--r--   0 kyle      (1000) kyle      (1000)    16186 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/webresult/js/paramquery-pro-3/pqgrid.dev.css
+-rw-r--r--   0 kyle      (1000) kyle      (1000)   481365 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/webresult/js/paramquery-pro-3/pqgrid.dev.js
+-rw-r--r--   0 kyle      (1000) kyle      (1000)    12765 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/webresult/js/paramquery-pro-3/pqgrid.min.css
+-rw-r--r--   0 kyle      (1000) kyle      (1000)   242939 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/webresult/js/paramquery-pro-3/pqgrid.min.js
+-rw-r--r--   0 kyle      (1000) kyle      (1000)     1646 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/webresult/js/paramquery-pro-3/pqgrid.ui.dev.css
+-rw-r--r--   0 kyle      (1000) kyle      (1000)     1286 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/webresult/js/paramquery-pro-3/pqgrid.ui.min.css
+-rw-r--r--   0 kyle      (1000) kyle      (1000)      587 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/webresult/js/paramquery-pro-3/readme.txt
+drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2023-05-22 17:05:46.057460 open-cravat-2.3.1/cravat/webresult/js/paramquery-pro-3/themes/
+drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2023-05-22 17:05:46.079460 open-cravat-2.3.1/cravat/webresult/js/paramquery-pro-3/themes/bootstrap/
+-rw-r--r--   0 kyle      (1000) kyle      (1000)     4392 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/webresult/js/paramquery-pro-3/themes/bootstrap/pqgrid.css
+drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2023-05-22 17:05:46.079460 open-cravat-2.3.1/cravat/webresult/js/paramquery-pro-3/themes/brown/
+-rw-r--r--   0 kyle      (1000) kyle      (1000)     4392 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/webresult/js/paramquery-pro-3/themes/brown/pqgrid.css
+drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2023-05-22 17:05:46.079460 open-cravat-2.3.1/cravat/webresult/js/paramquery-pro-3/themes/chocolate/
+-rw-r--r--   0 kyle      (1000) kyle      (1000)     4392 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/webresult/js/paramquery-pro-3/themes/chocolate/pqgrid.css
+drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2023-05-22 17:05:46.079460 open-cravat-2.3.1/cravat/webresult/js/paramquery-pro-3/themes/cocoa/
+-rw-r--r--   0 kyle      (1000) kyle      (1000)     4392 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/webresult/js/paramquery-pro-3/themes/cocoa/pqgrid.css
+drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2023-05-22 17:05:46.079460 open-cravat-2.3.1/cravat/webresult/js/paramquery-pro-3/themes/crimson/
+-rw-r--r--   0 kyle      (1000) kyle      (1000)     4392 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/webresult/js/paramquery-pro-3/themes/crimson/pqgrid.css
+drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2023-05-22 17:05:46.079460 open-cravat-2.3.1/cravat/webresult/js/paramquery-pro-3/themes/gray/
+-rw-r--r--   0 kyle      (1000) kyle      (1000)     4392 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/webresult/js/paramquery-pro-3/themes/gray/pqgrid.css
+drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2023-05-22 17:05:46.080460 open-cravat-2.3.1/cravat/webresult/js/paramquery-pro-3/themes/indigo/
+-rw-r--r--   0 kyle      (1000) kyle      (1000)     4392 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/webresult/js/paramquery-pro-3/themes/indigo/pqgrid.css
+drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2023-05-22 17:05:46.080460 open-cravat-2.3.1/cravat/webresult/js/paramquery-pro-3/themes/office/
+-rw-r--r--   0 kyle      (1000) kyle      (1000)     4392 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/webresult/js/paramquery-pro-3/themes/office/pqgrid.css
+drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2023-05-22 17:05:46.080460 open-cravat-2.3.1/cravat/webresult/js/paramquery-pro-3/themes/purple/
+-rw-r--r--   0 kyle      (1000) kyle      (1000)     4392 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/webresult/js/paramquery-pro-3/themes/purple/pqgrid.css
+drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2023-05-22 17:05:46.080460 open-cravat-2.3.1/cravat/webresult/js/paramquery-pro-3/themes/red/
+-rw-r--r--   0 kyle      (1000) kyle      (1000)     4392 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/webresult/js/paramquery-pro-3/themes/red/pqgrid.css
+drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2023-05-22 17:05:46.080460 open-cravat-2.3.1/cravat/webresult/js/paramquery-pro-3/themes/rosybrown/
+-rw-r--r--   0 kyle      (1000) kyle      (1000)     4392 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/webresult/js/paramquery-pro-3/themes/rosybrown/pqgrid.css
+drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2023-05-22 17:05:46.080460 open-cravat-2.3.1/cravat/webresult/js/paramquery-pro-3/themes/sandybrown/
+-rw-r--r--   0 kyle      (1000) kyle      (1000)     4392 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/webresult/js/paramquery-pro-3/themes/sandybrown/pqgrid.css
+drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2023-05-22 17:05:46.080460 open-cravat-2.3.1/cravat/webresult/js/paramquery-pro-3/themes/steelblue/
+-rw-r--r--   0 kyle      (1000) kyle      (1000)     4392 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/webresult/js/paramquery-pro-3/themes/steelblue/pqgrid.css
+drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2023-05-22 17:05:46.080460 open-cravat-2.3.1/cravat/webresult/js/paramquery-pro-3/themes/tan/
+-rw-r--r--   0 kyle      (1000) kyle      (1000)     4392 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/webresult/js/paramquery-pro-3/themes/tan/pqgrid.css
+drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2023-05-22 17:05:46.080460 open-cravat-2.3.1/cravat/webresult/js/paramquery-pro-3/themes/violet/
+-rw-r--r--   0 kyle      (1000) kyle      (1000)     4392 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/webresult/js/paramquery-pro-3/themes/violet/pqgrid.css
+drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2023-05-22 17:05:46.081460 open-cravat-2.3.1/cravat/webresult/js/paramquery-pro-3/touch-punch/
+-rw-r--r--   0 kyle      (1000) kyle      (1000)     1071 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/webresult/js/paramquery-pro-3/touch-punch/ChangeLog.txt
+-rw-r--r--   0 kyle      (1000) kyle      (1000)     1190 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/webresult/js/paramquery-pro-3/touch-punch/MIT-LICENSE.txt
+-rw-r--r--   0 kyle      (1000) kyle      (1000)     2677 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/webresult/js/paramquery-pro-3/touch-punch/README.md
+-rw-r--r--   0 kyle      (1000) kyle      (1000)     3716 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/webresult/js/paramquery-pro-3/touch-punch/touch-punch.dev.js
+-rw-r--r--   0 kyle      (1000) kyle      (1000)     1847 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/webresult/js/paramquery-pro-3/touch-punch/touch-punch.min.js
+-rw-r--r--   0 kyle      (1000) kyle      (1000)    12591 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/webresult/js/pqselect.min.js
+-rw-r--r--   0 kyle      (1000) kyle      (1000)    92225 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/webresult/js/raphael-min.js
+-rw-r--r--   0 kyle      (1000) kyle      (1000)     1530 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/webresult/jsonreporter.py
+drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2023-05-22 17:05:46.081460 open-cravat-2.3.1/cravat/webresult/nocache/
+drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2023-05-22 17:05:46.081460 open-cravat-2.3.1/cravat/webresult/nocache/css/
+-rw-r--r--   0 kyle      (1000) kyle      (1000)     1714 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/webresult/nocache/css/singlevariantpage.css
+-rw-r--r--   0 kyle      (1000) kyle      (1000)    20968 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/webresult/nocache/css/style.css
+-rw-r--r--   0 kyle      (1000) kyle      (1000)     2920 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/webresult/nocache/css/widget.css
+drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2023-05-22 17:05:46.082460 open-cravat-2.3.1/cravat/webresult/nocache/js/
+-rw-r--r--   0 kyle      (1000) kyle      (1000)    26685 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/webresult/nocache/js/filter.js
+-rw-r--r--   0 kyle      (1000) kyle      (1000)    12851 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/webresult/nocache/js/infomgr.js
+-rw-r--r--   0 kyle      (1000) kyle      (1000)    44175 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/webresult/nocache/js/main.js
+-rw-r--r--   0 kyle      (1000) kyle      (1000)    99662 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/webresult/nocache/js/setup.js
+-rw-r--r--   0 kyle      (1000) kyle      (1000)     7986 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/webresult/nocache/js/showvariant.js
+-rw-r--r--   0 kyle      (1000) kyle      (1000)    35998 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/webresult/nocache/js/singlevariantpage.js
+-rw-r--r--   0 kyle      (1000) kyle      (1000)    31708 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/webresult/nocache/js/util.js
+-rw-r--r--   0 kyle      (1000) kyle      (1000)     1688 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/webresult/nocache/js/variables.js
+-rw-r--r--   0 kyle      (1000) kyle      (1000)    20474 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/webresult/nocache/js/widgethelper.js
+-rw-r--r--   0 kyle      (1000) kyle      (1000)     5535 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/webresult/nocache/variant.html
+-rw-r--r--   0 kyle      (1000) kyle      (1000)    10263 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/webresult/question.png
+-rw-r--r--   0 kyle      (1000) kyle      (1000)    30111 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/webresult/webresult.py
+-rw-r--r--   0 kyle      (1000) kyle      (1000)      173 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/webresult/webviewer.yml
+drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2023-05-22 17:05:46.083460 open-cravat-2.3.1/cravat/webstore/
+-rw-r--r--   0 kyle      (1000) kyle      (1000)        0 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/webstore/__init__.py
+-rw-r--r--   0 kyle      (1000) kyle      (1000)     1365 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/webstore/cravat_store.css
+-rw-r--r--   0 kyle      (1000) kyle      (1000)     1224 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/webstore/favicon.ico
+drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2023-05-22 17:05:46.085460 open-cravat-2.3.1/cravat/webstore/images/
+-rw-r--r--   0 kyle      (1000) kyle      (1000)      446 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/webstore/images/chat-dots-fill.svg
+-rw-r--r--   0 kyle      (1000) kyle      (1000)      740 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/webstore/images/chat-dots.svg
+-rw-r--r--   0 kyle      (1000) kyle      (1000)      396 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/webstore/images/chat-left-text-fill.svg
+-rw-r--r--   0 kyle      (1000) kyle      (1000)      545 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/webstore/images/chat-left-text.svg
+-rw-r--r--   0 kyle      (1000) kyle      (1000)    22268 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/webstore/images/done.png
+-rw-r--r--   0 kyle      (1000) kyle      (1000)     4948 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/webstore/images/email.png
+-rw-r--r--   0 kyle      (1000) kyle      (1000)     2226 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/webstore/images/empty.png
+-rw-r--r--   0 kyle      (1000) kyle      (1000)     1351 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/webstore/images/favicon.png
+-rw-r--r--   0 kyle      (1000) kyle      (1000)     1763 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/webstore/images/folder.png
+-rw-r--r--   0 kyle      (1000) kyle      (1000)    38197 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/webstore/images/genericmodulelogo.png
+-rw-r--r--   0 kyle      (1000) kyle      (1000)     4766 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/webstore/images/hamburger.png
+-rw-r--r--   0 kyle      (1000) kyle      (1000)     1194 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/webstore/images/left_arrow.png
+-rw-r--r--   0 kyle      (1000) kyle      (1000)    67804 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/webstore/images/logo.png
+-rw-r--r--   0 kyle      (1000) kyle      (1000)     3524 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/webstore/images/new.png
+-rw-r--r--   0 kyle      (1000) kyle      (1000)    10263 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/webstore/images/question.png
+-rw-r--r--   0 kyle      (1000) kyle      (1000)     1214 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/webstore/images/right_arrow.png
+-rw-r--r--   0 kyle      (1000) kyle      (1000)      340 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/webstore/images/x-lg.svg
+-rw-r--r--   0 kyle      (1000) kyle      (1000)    86927 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/webstore/jquery-3.3.1.min.js
+drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2023-05-22 17:05:46.085460 open-cravat-2.3.1/cravat/webstore/js/
+-rw-r--r--   0 kyle      (1000) kyle      (1000)    75673 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/webstore/js/showdown-1.9.1.min.js
+-rw-r--r--   0 kyle      (1000) kyle      (1000)    91924 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/webstore/js/showdown.min.js.map
+drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2023-05-22 17:05:46.085460 open-cravat-2.3.1/cravat/webstore/nocache/
+-rw-r--r--   0 kyle      (1000) kyle      (1000)    15017 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/webstore/nocache/webstore.css
+-rw-r--r--   0 kyle      (1000) kyle      (1000)    95532 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/webstore/nocache/webstore.js
+-rw-r--r--   0 kyle      (1000) kyle      (1000)     2342 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/webstore/sse.py
+-rw-r--r--   0 kyle      (1000) kyle      (1000)     1700 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/webstore/store_handlers.py
+-rw-r--r--   0 kyle      (1000) kyle      (1000)    16522 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/webstore/webstore.py
+-rw-r--r--   0 kyle      (1000) kyle      (1000)      283 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/webstore/ws.html
+-rw-r--r--   0 kyle      (1000) kyle      (1000)      720 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/webstore/ws.js
+drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2023-05-22 17:05:46.087460 open-cravat-2.3.1/cravat/websubmit/
+-rw-r--r--   0 kyle      (1000) kyle      (1000)       11 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/websubmit/.gitignore
+-rw-r--r--   0 kyle      (1000) kyle      (1000)   210024 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/websubmit/Chart.bundle.min.js
+-rw-r--r--   0 kyle      (1000) kyle      (1000)        0 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/websubmit/__init__.py
+-rw-r--r--   0 kyle      (1000) kyle      (1000)      719 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/websubmit/arrow.png
+-rw-r--r--   0 kyle      (1000) kyle      (1000)     2291 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/websubmit/down.png
+-rw-r--r--   0 kyle      (1000) kyle      (1000)     4948 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/websubmit/email.png
+-rw-r--r--   0 kyle      (1000) kyle      (1000)     1224 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/websubmit/favicon.ico
+-rw-r--r--   0 kyle      (1000) kyle      (1000)     1351 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/websubmit/favicon.png
+-rw-r--r--   0 kyle      (1000) kyle      (1000)      108 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/websubmit/googleAnalytics.js
+-rw-r--r--   0 kyle      (1000) kyle      (1000)     1052 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/websubmit/help.png
+drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2023-05-22 17:05:46.088460 open-cravat-2.3.1/cravat/websubmit/input-examples/
+-rw-r--r--   0 kyle      (1000) kyle      (1000)      527 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/websubmit/input-examples/cravat.hg18.txt
+-rw-r--r--   0 kyle      (1000) kyle      (1000)      529 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/websubmit/input-examples/cravat.hg19.txt
+-rw-r--r--   0 kyle      (1000) kyle      (1000)      529 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/websubmit/input-examples/cravat.hg38.txt
+-rw-r--r--   0 kyle      (1000) kyle      (1000)     2199 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/websubmit/input-examples/vcf.hg18.txt
+-rw-r--r--   0 kyle      (1000) kyle      (1000)     2199 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/websubmit/input-examples/vcf.hg19.txt
+-rw-r--r--   0 kyle      (1000) kyle      (1000)     2199 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/websubmit/input-examples/vcf.hg38.txt
+-rw-r--r--   0 kyle      (1000) kyle      (1000)    86927 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/websubmit/jquery-3.3.1.min.js
+-rw-r--r--   0 kyle      (1000) kyle      (1000)    53784 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/websubmit/logo.png
+-rw-r--r--   0 kyle      (1000) kyle      (1000)    56098 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/websubmit/logo_transparent.png
+-rw-r--r--   0 kyle      (1000) kyle      (1000)      225 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/websubmit/menu.png
+drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2023-05-22 17:05:46.088460 open-cravat-2.3.1/cravat/websubmit/nocache/
+-rw-r--r--   0 kyle      (1000) kyle      (1000)    13800 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/websubmit/nocache/broken_wheel.gif
+-rw-r--r--   0 kyle      (1000) kyle      (1000)    18796 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/websubmit/nocache/index.html
+-rw-r--r--   0 kyle      (1000) kyle      (1000)    17372 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/websubmit/nocache/websubmit.css
+-rw-r--r--   0 kyle      (1000) kyle      (1000)    83472 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/websubmit/nocache/websubmit.js
+-rw-r--r--   0 kyle      (1000) kyle      (1000)    11488 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/websubmit/nointernet.png
+-rw-r--r--   0 kyle      (1000) kyle      (1000)    27869 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/websubmit/pqselect.dev.customforsubmit.js
+-rw-r--r--   0 kyle      (1000) kyle      (1000)    10263 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/websubmit/question.png
+-rw-r--r--   0 kyle      (1000) kyle      (1000)     2167 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/websubmit/refresh.png
+-rw-r--r--   0 kyle      (1000) kyle      (1000)      280 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/websubmit/threedots.png
+-rw-r--r--   0 kyle      (1000) kyle      (1000)    48552 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/websubmit/websubmit.py
+-rw-r--r--   0 kyle      (1000) kyle      (1000)     3724 2023-05-22 17:05:45.000000 open-cravat-2.3.1/cravat/wincravat.pyw
+drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2023-05-22 17:05:46.089460 open-cravat-2.3.1/open_cravat.egg-info/
+-rw-r--r--   0 kyle      (1000) kyle      (1000)     1056 2023-05-22 17:05:46.000000 open-cravat-2.3.1/open_cravat.egg-info/PKG-INFO
+-rw-r--r--   0 kyle      (1000) kyle      (1000)    12287 2023-05-22 17:05:46.000000 open-cravat-2.3.1/open_cravat.egg-info/SOURCES.txt
+-rw-r--r--   0 kyle      (1000) kyle      (1000)        1 2023-05-22 17:05:46.000000 open-cravat-2.3.1/open_cravat.egg-info/dependency_links.txt
+-rw-r--r--   0 kyle      (1000) kyle      (1000)       38 2023-05-22 17:05:46.000000 open-cravat-2.3.1/open_cravat.egg-info/entry_points.txt
+-rw-r--r--   0 kyle      (1000) kyle      (1000)      184 2023-05-22 17:05:46.000000 open-cravat-2.3.1/open_cravat.egg-info/requires.txt
+-rw-r--r--   0 kyle      (1000) kyle      (1000)        7 2023-05-22 17:05:46.000000 open-cravat-2.3.1/open_cravat.egg-info/top_level.txt
+-rw-r--r--   0 kyle      (1000) kyle      (1000)       38 2023-05-22 17:05:46.089460 open-cravat-2.3.1/setup.cfg
+-rw-r--r--   0 kyle      (1000) kyle      (1000)     2877 2023-05-22 17:05:45.000000 open-cravat-2.3.1/setup.py
+drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2023-05-22 17:05:46.089460 open-cravat-2.3.1/tests/
+-rw-r--r--   0 kyle      (1000) kyle      (1000)     6183 2023-05-22 17:05:45.000000 open-cravat-2.3.1/tests/test_admin_util.py
```

### Comparing `open-cravat-2.3.0/LICENSE` & `open-cravat-2.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `open-cravat-2.3.0/PKG-INFO` & `open-cravat-2.3.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: open-cravat
-Version: 2.3.0
+Version: 2.3.1
 Summary: OpenCRAVAT - variant analysis toolkit
 Home-page: https://www.opencravat.org
 Author: RyangGuk Kim, Kyle Moad, Mike Ryan, and Rachel Karchin
 Author-email: support@opencravat.org
 Requires-Python: >=3.8
 License-File: LICENSE
```

### Comparing `open-cravat-2.3.0/README.rst` & `open-cravat-2.3.1/README.rst`

 * *Files identical despite different names*

### Comparing `open-cravat-2.3.0/cravat/__init__.py` & `open-cravat-2.3.1/cravat/__init__.py`

 * *Files identical despite different names*

### Comparing `open-cravat-2.3.0/cravat/admin_util.py` & `open-cravat-2.3.1/cravat/admin_util.py`

 * *Files 2% similar despite different names*

```diff
@@ -513,52 +513,93 @@
 
 def get_download_counts():
     mic.update_download_counts()
     counts = mic.download_counts
     return counts
 
 
-def get_install_deps(module_name, version=None, skip_installed=True, recursive_depth=0):
+def __get_highest_matching_version(requirement: pkg_resources.Requirement, versions: list) -> str:
+    """Return the highest matching version in 'versions' that satisfies the 'requirement'"""
+    lvers = [LooseVersion(v) for v in versions]
+    lvers.sort(reverse=True)
+    for lv in lvers:
+        if lv.vstring in requirement:
+            return lv.vstring
+    # no matching version found
+    return None
+
+
+def __remove_locally_installed_deps(deps: dict) -> None:
+    to_delete = []
+    # find locally installed packages that match version requirements
+    for name, version in deps.items():
+        v_string = f"{name}>={version}"
+        req = pkg_resources.Requirement(v_string)
+        local_info = get_local_module_info(name)
+        if local_info and local_info.version in req:
+            to_delete += deps[name]
+    
+    # remove those matches
+    for name in to_delete:
+        del deps[name]
+
+    
+def get_install_deps(module_name, version=None, skip_installed=True):
     mic.update_remote()
-    # If input module version not provided, set to highest
-    if version is None:
-        version = get_remote_latest_version(module_name)
     config = mic.get_remote_config(module_name, version=version)
-    req_list = config.get("requires", [])
+    deps_to_check = config.get("requires", [])[:]
+    checked = []
+    reqs_to_install = {}
     deps = {}
-    for req_string in req_list:
+    while deps_to_check:
+        req_string = deps_to_check.pop()
+        if req_string in checked:
+            continue
+
+        checked.append(req_string)
         req = pkg_resources.Requirement(req_string)
+        parent = req.name
         rem_info = get_remote_module_info(req.name)
         # Skip if module does not exist
         if rem_info is None and get_local_module_info(req.name) is None:
+            print(f"Could not find module [{req}]")
             continue
-        if skip_installed:
-            # Skip if a matching version is installed
-            local_info = get_local_module_info(req.name)
-            if local_info and local_info.version in req:
-                continue
+
+        if req.name in reqs_to_install:
+            # TODO: Add some logging about a duplicate dependency:
+            # print(f"Repeat dependency detected: [{req}]")
+            reqs_to_install[req.name] += [str(req.specifier)] if str(req.specifier) else []
+        else:
+            reqs_to_install[req.name] = [str(req.specifier)] if str(req.specifier) else []
+
         # Select the highest matching version
-        lvers = [LooseVersion(v) for v in rem_info.versions]
-        lvers.sort(reverse=True)
-        highest_matching = None
-        for lv in lvers:
-            if lv.vstring in req:
-                highest_matching = lv.vstring
-                break
-        # Dont include if no matching version exists
-        if highest_matching is not None:
-            deps[req.name] = highest_matching
-            # Recursively get dependencies
-            if (recursive_depth < 3):
-                deps = dict(get_install_deps(
-                                module_name=req.name, 
-                                version=highest_matching,
-                                skip_installed=skip_installed,
-                                recursive_depth=recursive_depth + 1
-                            ), **deps)
+        highest_matching = __get_highest_matching_version(req, rem_info.versions)
+
+        if highest_matching is None:
+            # TODO: Add some logging about no matching version:
+            # print(f"Could not find a matching version for module [{req}]")
+            continue
+
+        config = mic.get_remote_config(req.name, version=highest_matching)
+        child_reqs = config.get("requires", [])[:]
+        deps_to_check += child_reqs
+
+    # convert the requirements list to the correct format
+    for name, spec_list in reqs_to_install.items():
+        rem_info = get_remote_module_info(name)
+        full_req_string = f"{name}{','.join(spec_list)}"
+        r = pkg_resources.Requirement(full_req_string)
+        version = __get_highest_matching_version(r, rem_info.versions)
+        if version is None:
+            raise ValueError(f"Could not find appropriate version for module [{name}]")
+        deps[name] = version
+
+    # Skip if a matching version is installed
+    if skip_installed:
+        __remove_locally_installed_deps(deps)
 
     return deps
 
 
 def get_jobs_dir():
     conf = get_system_conf()
     jobs_dir = conf[constants.jobs_dir_key]
```

### Comparing `open-cravat-2.3.0/cravat/aggregator.py` & `open-cravat-2.3.1/cravat/aggregator.py`

 * *Files 1% similar despite different names*

```diff
@@ -162,15 +162,14 @@
                         )
                         last_status_update_time = cur_time
                 except Exception as e:
                     self._log_runtime_error(lnum, line, e)
             self.dbconn.commit()
         self.fill_categories()
         self.cursor.execute("pragma synchronous=2;")
-        self.cursor.execute("pragma journal_mode=delete;")
         end_time = time.time()
         self.logger.info("finished: %s" % time.asctime(time.localtime(end_time)))
         runtime = end_time - start_time
         self.logger.info("runtime: %s" % round(runtime, 3))
         self._cleanup()
         self.status_writer.queue_status_update(
             "status", "Finished {} ({})".format("Aggregator", self.level)
```

### Comparing `open-cravat-2.3.0/cravat/annotator_options.py` & `open-cravat-2.3.1/cravat/annotator_options.py`

 * *Files identical despite different names*

### Comparing `open-cravat-2.3.0/cravat/annotator_template/annotator_template.py` & `open-cravat-2.3.1/cravat/annotator_template/annotator_template.py`

 * *Files identical despite different names*

### Comparing `open-cravat-2.3.0/cravat/annotator_template/annotator_template.yml` & `open-cravat-2.3.1/cravat/annotator_template/annotator_template.yml`

 * *Files identical despite different names*

### Comparing `open-cravat-2.3.0/cravat/base_annotator.py` & `open-cravat-2.3.1/cravat/base_annotator.py`

 * *Files identical despite different names*

### Comparing `open-cravat-2.3.0/cravat/base_commonmodule.py` & `open-cravat-2.3.1/cravat/base_commonmodule.py`

 * *Files identical despite different names*

### Comparing `open-cravat-2.3.0/cravat/base_converter.py` & `open-cravat-2.3.1/cravat/base_converter.py`

 * *Files identical despite different names*

### Comparing `open-cravat-2.3.0/cravat/base_mapper.py` & `open-cravat-2.3.1/cravat/base_mapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -371,14 +371,28 @@
         # TODO: Remove it after a while and add 1.8.0 to the db update chain in cravat_util.
         cols = [
             "base__" + coldef["name"]
             for coldef in crx_def
             if coldef["name"] != "cchange"
         ]
         cols.extend(["tagsampler__numsample"])
+        async def get_database_version(conn=None, cursor=None):
+            q = 'select colval from info where colkey="open-cravat"'
+            await cursor.execute(q)
+            return await cursor.fetchone()
+        result = await cf.exec_db(get_database_version)
+        dbver = result[0]
+        if au.compare_version(dbver, '2.3.0') <= 0:
+            tmp = []
+            for col in cols:
+                if col == 'base__note_variant':
+                    tmp.append('base__note')
+                    continue
+                tmp.append(col)
+            cols = tmp
         data = {}
         t = time.time()
         rows = await cf.exec_db(cf.get_variant_data_for_cols, cols)
         rows_by_hugo = {}
         t = time.time()
         for row in rows:
             hugo = row[-1]
```

### Comparing `open-cravat-2.3.0/cravat/base_postaggregator.py` & `open-cravat-2.3.1/cravat/base_postaggregator.py`

 * *Files 1% similar despite different names*

```diff
@@ -225,24 +225,23 @@
             )
         except Exception as e:
             self._log_exception(e, halt=False)
 
     # Setup function for the base_annotator, different from self.setup()
     # which is intended to be for the derived annotator.
     def base_setup(self):
-        self._alter_tables()
         self.setup()
+        self._alter_tables()
 
     def _open_db_connection(self):
         self.db_path = os.path.join(self.output_dir, self.run_name + ".sqlite")
         if os.path.exists(self.db_path):
             self.dbconn = sqlite3.connect(self.db_path)
             self.cursor = self.dbconn.cursor()
             self.cursor_w = self.dbconn.cursor()
-            self.cursor_w.execute('pragma journal_mode="wal"')
         else:
             msg = self.db_path + " not found"
             if self.logger:
                 self.logger.error(msg)
             sys.exit(msg)
 
     def _close_db_connection(self):
```

### Comparing `open-cravat-2.3.0/cravat/base_summarizer.py` & `open-cravat-2.3.1/cravat/base_summarizer.py`

 * *Files identical despite different names*

### Comparing `open-cravat-2.3.0/cravat/config_loader.py` & `open-cravat-2.3.1/cravat/config_loader.py`

 * *Files identical despite different names*

### Comparing `open-cravat-2.3.0/cravat/constants.py` & `open-cravat-2.3.1/cravat/constants.py`

 * *Files 2% similar despite different names*

```diff
@@ -150,15 +150,15 @@
     {
         "name": "alt_base",
         "title": "Alt Base",
         "type": "string",
         "width": 50,
         "filterable": False,
     },
-    {"name": "note", "title": "Note", "type": "string", "width": 50},
+    {"name": "note_variant", "title": "Variant Note", "type": "string", "width": 50},
 ]
 crv_idx = [["uid"]]
 crx_def = crv_def + [
     {
         "name": "coding",
         "title": "Coding",
         "type": "string",
@@ -217,15 +217,15 @@
     {
         "name": "hugo",
         "title": "Gene",
         "type": "string",
         "width": 70,
         "filterable": True,
     },
-    {"name": "note", "title": "Note", "type": "string", "width": 50},
+    {"name": "note_gene", "title": "Gene Note", "type": "string", "width": 50},
 ]
 crg_idx = [["hugo"]]
 crt_def = [
     {"name": "primary_transcript", "title": "Primary transcript", "type": "string"},
     {"name": "alt_transcript", "title": "Alternate transcript", "type": "string"},
 ]
 crt_idx = [["primary_transcript"]]
```

### Comparing `open-cravat-2.3.0/cravat/cravat_admin.py` & `open-cravat-2.3.1/cravat/cravat_admin.py`

 * *Files identical despite different names*

### Comparing `open-cravat-2.3.0/cravat/cravat_class.py` & `open-cravat-2.3.1/cravat/cravat_class.py`

 * *Files 0% similar despite different names*

```diff
@@ -620,25 +620,14 @@
                     print("Running reporter...")
                 no_problem_in_run, report_response = await self.run_reporter()
             self.update_status("Finished", force=True)
         except Exception as e:
             self.handle_exception(e)
             no_problem_in_run = False
         finally:
-            dbpath = os.path.join(self.output_dir, self.run_name + ".sqlite")
-
-            # Set journal_mode
-            dbconn = sqlite3.connect(dbpath)
-            try:
-                dbconn.execute('pragma journal_mode="delete"')
-            except sqlite3.Error as e:
-                pass
-            finally:
-                dbconn.close()
-
             end_time = time.time()
             display_time = time.asctime(time.localtime(end_time))
             runtime = end_time - self.start_time
             self.metricObj.set_job_data('jobRuntime',round(runtime,3))
             success = "Finished Normally"
             if no_problem_in_run:
                 self.logger.info("finished: {0}".format(display_time))
```

### Comparing `open-cravat-2.3.0/cravat/cravat_convert.py` & `open-cravat-2.3.1/cravat/cravat_convert.py`

 * *Files 0% similar despite different names*

```diff
@@ -401,15 +401,15 @@
             "status",
             "Started {} ({})".format("Converter", self.primary_converter.format_name),
         )
         last_status_update_time = time.time()
         multiple_files = len(self.input_paths) > 1
         fileno = 0
         total_lnum = 0
-        base_re = re.compile("^[ATGC]+|[-]+$")
+        base_re = re.compile("^[ATGCatgc]+|[-]+$")
         write_lnum = 0
         for fn in self.input_paths:
             if self.pipeinput:
                 f = sys.stdin
             else:
                 f = self.open_input_file(fn)
             if self.pipeinput == True:
@@ -671,14 +671,16 @@
 
     def end(self):
         pass
 
     def standardize_pos_ref_alt(self, strand, pos, ref, alt):
         reflen = len(ref)
         altlen = len(alt)
+        ref = ref.upper()
+        alt = alt.upper()
         # Returns without change if same single nucleotide for ref and alt.
         if reflen == 1 and altlen == 1 and ref == alt:
             return pos, ref, alt
         # Trimming from the start and then the end of the sequence
         # where the sequences overlap with the same nucleotides
         new_ref2, new_alt2, new_pos = self.trim_input(ref, alt, pos, strand)
         if new_ref2 == "" or new_ref2 == ".":
```

### Comparing `open-cravat-2.3.0/cravat/cravat_filter.py` & `open-cravat-2.3.1/cravat/cravat_filter.py`

 * *Files 3% similar despite different names*

```diff
@@ -553,15 +553,15 @@
 
     def getgenecount(self):
         loop = asyncio.get_event_loop()
         count = loop.run_until_complete(self.exec_db(self.getcount, "gene"))
         return count
 
     async def getcount(self, level="variant", conn=None, cursor=None):
-        bypassfilter = self.filter == {} and self.filtersql is None and self.includesample is None and self.excludesample is None
+        bypassfilter = not(self.filter or self.filtersql or self.includesample or self.excludesample)
         level = "variant"
         await self.exec_db(self.make_filtered_uid_table)
         if bypassfilter:
             ftable = level
         else:
             ftable = level + "_filtered"
         q = "select count(*) from " + ftable
@@ -642,15 +642,15 @@
             + exclude_where
         )
         await cursor.execute(sql)
         it = await cursor.fetchall()
         return it
 
     async def get_filtered_iterator(self, level="variant", conn=None, cursor=None):
-        bypassfilter = self.filter == {} and self.filtersql is None and self.includesample is None and self.excludesample is None
+        bypassfilter = not(self.filter or self.filtersql or self.includesample or self.excludesample)
         if level == "variant":
             kcol = "base__uid"
             if bypassfilter:
                 ftable = "variant"
             else:
                 ftable = "variant_filtered"
         elif level == "gene":
@@ -751,15 +751,15 @@
             q += " " + where
             if fsample_made:
                 q += " and (v.base__uid in (select base__uid from fsample))"
         return q
 
     async def make_filtered_uid_table(self, conn=None, cursor=None):
         t = time.time()
-        bypassfilter = self.filter == {} and self.filtersql is None and self.includesample is None and self.excludesample is None
+        bypassfilter = not(self.filter or self.filtersql or self.includesample or self.excludesample)
         if bypassfilter == False:
             level = "variant"
             vtable = level
             vftable = level + "_filtered"
             q = "drop table if exists " + vftable
             await cursor.execute(q)
             q = f"create table {vftable} as select v.base__uid from variant as v"
@@ -819,15 +819,15 @@
             await cursor.executemany(q, tdata)
             await conn.commit()
             return True
         else:
             return False
 
     async def make_filtered_hugo_table(self, conn=None, cursor=None):
-        bypassfilter = self.filter == {} and self.filtersql is None and self.includesample is None and self.excludesample is None
+        bypassfilter = not(self.filter or self.filtersql or self.includesample or self.excludesample)
         if bypassfilter == False:
             await cursor.execute("pragma synchronous=0")
             level = "gene"
             vtable = "variant"
             vftable = vtable + "_filtered"
             gftable = level + "_filtered"
             q = "drop table if exists " + gftable
@@ -953,52 +953,52 @@
                 return True
 
     async def get_variant_iterator_filtered_uids_cols(
         self, cols, conn=None, cursor=None
     ):
         if cols[0] == "base__uid":
             cols[0] = "v." + cols[0]
-        bypassfilter = self.filter == {} and self.filtersql is None and self.includesample is None and self.excludesample is None
+        bypassfilter = not(self.filter or self.filtersql or self.includesample or self.excludesample)
         q = "select " + ",".join(cols) + " from variant as v"
         if bypassfilter == False:
             q += " inner join variant_filtered as f on v.base__uid=f.base__uid"
         await cursor.execute(q)
         rows = await cursor.fetchall()
         for row in rows:
             d = {}
             for i in range(len(row)):
                 d[cols[i].split("__")[1]] = row[i]
             yield d
 
     async def get_filtered_hugo_list(self, conn=None, cursor=None):
-        bypassfilter = self.filter == {} and self.filtersql is None and self.includesample is None and self.excludesample is None
+        bypassfilter = not(self.filter or self.filtersql or self.includesample or self.excludesample)
         if bypassfilter:
             q = "select distinct variant.base__hugo from gene, variant where gene.base__hugo==variant.base__hugo"
         else:
             q = "select base__hugo from gene_filtered"
         await cursor.execute(q)
         rows = await cursor.fetchall()
         hugos = [row[0] for row in rows]
         return hugos
 
     async def get_variant_data_for_cols(self, cols, conn=None, cursor=None):
-        bypassfilter = self.filter == {} and self.filtersql is None and self.includesample is None and self.excludesample is None
+        bypassfilter = not(self.filter or self.filtersql or self.includesample or self.excludesample)
         if cols[0] == "base__uid":
             cols[0] = "v.base__uid"
         q = "select {},base__hugo from variant as v".format(",".join(cols))
         if bypassfilter == False:
             q += " inner join variant_filtered as f on v.base__uid=f.base__uid"
         if cols[0] == "v.base__uid":
             cols[0] = "base__uid"
         await cursor.execute(q)
         rows = await cursor.fetchall()
         return rows
 
     async def get_variant_data_for_hugo(self, hugo, cols, conn=None, cursor=None):
-        bypassfilter = self.filter == {} and self.filtersql is None and self.includesample is None and self.excludesample is None
+        bypassfilter = not(self.filter or self.filtersql or self.includesample or self.excludesample)
         if cols[0] == "base__uid":
             cols[0] = "v.base__uid"
         q = "select {} from variant as v".format(",".join(cols))
         if bypassfilter == False:
             q += ' inner join variant_filtered as f on v.base__uid=f.base__uid and v.base__hugo="{}"'.format(
                 hugo
             )
```

### Comparing `open-cravat-2.3.0/cravat/cravat_metrics.py` & `open-cravat-2.3.1/cravat/cravat_metrics.py`

 * *Files identical despite different names*

### Comparing `open-cravat-2.3.0/cravat/cravat_pack.py` & `open-cravat-2.3.1/cravat/cravat_pack.py`

 * *Files identical despite different names*

### Comparing `open-cravat-2.3.0/cravat/cravat_report.py` & `open-cravat-2.3.1/cravat/cravat_report.py`

 * *Files 0% similar despite different names*

```diff
@@ -990,32 +990,39 @@
         row = await cursor.fetchone()
         if row == None:
             ret = False
         else:
             ret = True
         return ret
 
-    #If reports are run with oc report command, update the job database _reports entry in the info table.
+    #If reports are run with oc report command or oc run, update the job database _reports entry in the info table.
     def update_reports_info(self):
         db = sqlite3.connect(self.dbpath)
         cur = db.cursor()
+        new_report = False
 
         q = 'select colval from info where colkey="_reports"'
         cur.execute(q)
         r = cur.fetchone()
         if r is None or r[0] == '':
             reports = []
         else:
             reports = r[0].split(',')
         for rep in self.report_types:
+            if rep == 'text':
+                continue
+            
             if not rep in reports:
                 reports.append(rep)
-        q = 'insert or replace into info values ("_reports", "{}")'.format(",".join(reports))
-        cur.execute(q)
-        db.commit()
+                new_report = True
+        
+        if new_report:        
+            q = 'insert or replace into info values ("_reports", "{}")'.format(",".join(reports))
+            cur.execute(q)
+            db.commit()
         db.close() 
 
 def clean_args(cmd_args):
     if len(cmd_args[0]) == 0:
         cmd_args = cmd_args[1:]
     if cmd_args[0].endswith("oc") or cmd_args[0].endswith("oc.py"):
         cmd_args = cmd_args[1:]
```

### Comparing `open-cravat-2.3.0/cravat/cravat_test.py` & `open-cravat-2.3.1/cravat/cravat_test.py`

 * *Files identical despite different names*

### Comparing `open-cravat-2.3.0/cravat/cravat_util.py` & `open-cravat-2.3.1/cravat/cravat_util.py`

 * *Files identical despite different names*

### Comparing `open-cravat-2.3.0/cravat/cravat_web.py` & `open-cravat-2.3.1/cravat/cravat_web.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,15 +45,15 @@
 servermode = None
 server_ready = None
 ssl_enabled = None
 protocol = None
 http_only = None
 sc = None
 loop = None
-debug = False
+server_traceback = False
 
 parser = argparse.ArgumentParser()
 parser.add_argument(
     "--multiuser",
     dest="servermode",
     action="store_true",
     default=False,
@@ -68,16 +68,16 @@
 parser.add_argument(
     "--http-only",
     action="store_true",
     default=False,
     help="Force not to accept https connection",
 )
 parser.add_argument(
-    "--debug",
-    dest="debug",
+    "--server-traceback",
+    dest="server_traceback",
     action="store_true",
     default=False,
     help="Console echoes exceptions written to log file.",
 )
 parser.add_argument("result", nargs="?", help="Path to a CRAVAT result SQLite file")
 parser.add_argument(
     "--webapp",
@@ -96,16 +96,16 @@
             asyncio.set_event_loop(loop)
         else:
             loop = asyncio.get_event_loop()
         global headless
         headless = args.headless
         global servermode
         servermode = args.servermode
-        global debug
-        debug = args.debug
+        global server_traceback
+        server_traceback = args.server_traceback
         if servermode and importlib.util.find_spec("cravat_multiuser") is not None:
             try:
                 global cravat_multiuser
                 import cravat_multiuser
 
                 loop.create_task(cravat_multiuser.setup_module())
                 global server_ready
@@ -158,15 +158,15 @@
                 sc.load_cert_chain(pem_path)
         if ssl_enabled:
             protocol = "https://"
         else:
             protocol = "http://"
     except Exception as e:
         logger.exception(e)
-        if debug:
+        if server_traceback:
             traceback.print_exc()
         logger.info("Exiting...")
         print(
             "Error occurred while starting OpenCRAVAT server.\nCheck {} for details.".format(
                 log_path
             )
         )
@@ -241,15 +241,15 @@
                 else:
                     url = f"{host}:{port}/submit/nocache/index.html"
             global protocol
             url = protocol + url
         main(url=url, host=host, port=port)
     except Exception as e:
         logger.exception(e)
-        if debug:
+        if server_traceback:
             traceback.print_exc()
         logger.info("Exiting...")
         print(
             "Error occurred while starting OpenCRAVAT server.\nCheck {} for details.".format(
                 log_path
             )
         )
@@ -295,15 +295,15 @@
             host = au.get_system_conf().get("gui_host", def_host)
             port = au.get_system_conf().get("gui_port", 8080)
         server["host"] = host
         server["port"] = port
         return server
     except Exception as e:
         logger.exception(e)
-        if debug:
+        if server_traceback:
             traceback.print_exc()
         logger.info("Exiting...")
         print(
             "Error occurred while OpenCRAVAT server.\nCheck {} for details.".format(
                 log_path
             )
         )
@@ -378,15 +378,15 @@
             nocache = True
         if nocache:
             response.headers["Cache-Control"] = "no-cache"
         return response
     except Exception as e:
         logger.info("Exception occurred at request={}".format(request))
         logger.exception(e)
-        if debug:
+        if server_traceback:
             traceback.print_exc()
         return web.HTTPInternalServerError(
             text=json.dumps({"status": "error", "msg": str(e)})
         )
 
 
 class WebServer(object):
@@ -594,30 +594,30 @@
                     "session_clean_interval", 3600
                 )  # default 1 hr
                 while True:
                     await cravat_multiuser.admindb.clean_sessions(max_age)
                     await asyncio.sleep(interval)
             except Exception as e:
                 logger.exception(e)
-                if debug:
+                if server_traceback:
                     traceback.print_exc()
 
         if servermode and server_ready:
             if "max_session_age" in au.get_system_conf():
                 loop.create_task(clean_sessions())
         global ssl_enabled
         if ssl_enabled:
             global sc
             server = WebServer(loop=loop, ssl_context=sc, url=url, host=host, port=port)
         else:
             server = WebServer(loop=loop, url=url, host=host, port=port)
         loop.run_forever()
     except Exception as e:
         logger.exception(e)
-        if debug:
+        if server_traceback:
             traceback.print_exc()
         logger.info("Exiting...")
         print(
             "Error occurred while starting OpenCRAVAT server.\nCheck {} for details.".format(
                 log_path
             )
         )
```

### Comparing `open-cravat-2.3.0/cravat/example_input` & `open-cravat-2.3.1/cravat/example_input`

 * *Files identical despite different names*

### Comparing `open-cravat-2.3.0/cravat/exceptions.py` & `open-cravat-2.3.1/cravat/exceptions.py`

 * *Files identical despite different names*

### Comparing `open-cravat-2.3.0/cravat/inout.py` & `open-cravat-2.3.1/cravat/inout.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,19 +34,22 @@
         return self.columns[col_index]
 
     def get_all_col_defs(self):
         return self.columns
 
 
 class CravatReader(CravatFile):
-    def __init__(self, path, seekpos=None, chunksize=None):
+    def __init__(self, path, seekpos=None, chunksize=None, encoding='utf-8'):
         super().__init__(path)
         self.seekpos = seekpos
         self.chunksize = chunksize
-        self.encoding = detect_encoding(self.path)
+        if encoding is None:
+            self.encoding = detect_encoding(self.path)
+        else:
+            self.encoding = encoding
         self.annotator_name = ""
         self.annotator_displayname = ""
         self.annotator_version = ""
         self.no_aggregate_cols = []
         self.index_columns = []
         self.report_substitution = None
         self._setup_definition()
```

### Comparing `open-cravat-2.3.0/cravat/liftover/hg18ToHg38.over.chain` & `open-cravat-2.3.1/cravat/liftover/hg18ToHg38.over.chain`

 * *Files identical despite different names*

### Comparing `open-cravat-2.3.0/cravat/liftover/hg19ToHg38.over.chain` & `open-cravat-2.3.1/cravat/liftover/hg19ToHg38.over.chain`

 * *Files identical despite different names*

### Comparing `open-cravat-2.3.0/cravat/mp_runners.py` & `open-cravat-2.3.1/cravat/mp_runners.py`

 * *Files identical despite different names*

### Comparing `open-cravat-2.3.0/cravat/oc.py` & `open-cravat-2.3.1/cravat/oc.py`

 * *Files identical despite different names*

### Comparing `open-cravat-2.3.0/cravat/store_utils.py` & `open-cravat-2.3.1/cravat/store_utils.py`

 * *Files identical despite different names*

### Comparing `open-cravat-2.3.0/cravat/util.py` & `open-cravat-2.3.1/cravat/util.py`

 * *Files identical despite different names*

### Comparing `open-cravat-2.3.0/cravat/webresult/cravat_view.py` & `open-cravat-2.3.1/cravat/webresult/cravat_view.py`

 * *Files identical despite different names*

### Comparing `open-cravat-2.3.0/cravat/webresult/css/pqselect.min.css` & `open-cravat-2.3.1/cravat/webresult/css/pqselect.min.css`

 * *Files identical despite different names*

### Comparing `open-cravat-2.3.0/cravat/webresult/email.png` & `open-cravat-2.3.1/cravat/webresult/email.png`

 * *Files identical despite different names*

### Comparing `open-cravat-2.3.0/cravat/webresult/favicon.ico` & `open-cravat-2.3.1/cravat/webresult/favicon.ico`

 * *Files identical despite different names*

### Comparing `open-cravat-2.3.0/cravat/webresult/favicon.png` & `open-cravat-2.3.1/cravat/webresult/favicon.png`

 * *Files identical despite different names*

### Comparing `open-cravat-2.3.0/cravat/webresult/fonts/roboto-bold-webfont.woff` & `open-cravat-2.3.1/cravat/webresult/fonts/roboto-bold-webfont.woff`

 * *Files identical despite different names*

### Comparing `open-cravat-2.3.0/cravat/webresult/fonts/roboto-bold-webfont.woff2` & `open-cravat-2.3.1/cravat/webresult/fonts/roboto-bold-webfont.woff2`

 * *Files identical despite different names*

### Comparing `open-cravat-2.3.0/cravat/webresult/fonts/roboto-light-webfont.woff` & `open-cravat-2.3.1/cravat/webresult/fonts/roboto-light-webfont.woff`

 * *Files identical despite different names*

### Comparing `open-cravat-2.3.0/cravat/webresult/fonts/roboto-light-webfont.woff2` & `open-cravat-2.3.1/cravat/webresult/fonts/roboto-light-webfont.woff2`

 * *Files identical despite different names*

### Comparing `open-cravat-2.3.0/cravat/webresult/fonts/roboto-medium-webfont.woff` & `open-cravat-2.3.1/cravat/webresult/fonts/roboto-medium-webfont.woff`

 * *Files identical despite different names*

### Comparing `open-cravat-2.3.0/cravat/webresult/fonts/roboto-medium-webfont.woff2` & `open-cravat-2.3.1/cravat/webresult/fonts/roboto-medium-webfont.woff2`

 * *Files identical despite different names*

### Comparing `open-cravat-2.3.0/cravat/webresult/fonts/sourcesanspro-bold-webfont.woff` & `open-cravat-2.3.1/cravat/webresult/fonts/sourcesanspro-bold-webfont.woff`

 * *Files identical despite different names*

### Comparing `open-cravat-2.3.0/cravat/webresult/fonts/sourcesanspro-bold-webfont.woff2` & `open-cravat-2.3.1/cravat/webresult/fonts/sourcesanspro-bold-webfont.woff2`

 * *Files identical despite different names*

### Comparing `open-cravat-2.3.0/cravat/webresult/images/arrow-spinner-static.gif` & `open-cravat-2.3.1/cravat/webresult/images/arrow-spinner-static.gif`

 * *Files identical despite different names*

### Comparing `open-cravat-2.3.0/cravat/webresult/images/arrow-spinner.gif` & `open-cravat-2.3.1/cravat/webresult/images/arrow-spinner.gif`

 * *Files identical despite different names*

### Comparing `open-cravat-2.3.0/cravat/webresult/images/arrows-move.svg` & `open-cravat-2.3.1/cravat/webresult/images/arrows-move.svg`

 * *Files identical despite different names*

### Comparing `open-cravat-2.3.0/cravat/webresult/images/back_arrow.png` & `open-cravat-2.3.1/cravat/webresult/images/back_arrow.png`

 * *Files identical despite different names*

### Comparing `open-cravat-2.3.0/cravat/webresult/images/bigSpinner.gif` & `open-cravat-2.3.1/cravat/webresult/images/bigSpinner.gif`

 * *Files identical despite different names*

### Comparing `open-cravat-2.3.0/cravat/webresult/images/camera.png` & `open-cravat-2.3.1/cravat/webresult/images/camera.png`

 * *Files identical despite different names*

### Comparing `open-cravat-2.3.0/cravat/webresult/images/camera.svg` & `open-cravat-2.3.1/cravat/webresult/images/camera.svg`

 * *Files identical despite different names*

### Comparing `open-cravat-2.3.0/cravat/webresult/images/close-button.png` & `open-cravat-2.3.1/cravat/webresult/images/close-button.png`

 * *Files identical despite different names*

### Comparing `open-cravat-2.3.0/cravat/webresult/images/close.png` & `open-cravat-2.3.1/cravat/webresult/images/close.png`

 * *Files identical despite different names*

### Comparing `open-cravat-2.3.0/cravat/webresult/images/close.svg` & `open-cravat-2.3.1/cravat/webresult/images/close.svg`

 * *Files identical despite different names*

### Comparing `open-cravat-2.3.0/cravat/webresult/images/close_icon.png` & `open-cravat-2.3.1/cravat/webresult/images/close_icon.png`

 * *Files identical despite different names*

### Comparing `open-cravat-2.3.0/cravat/webresult/images/download-material-black.png` & `open-cravat-2.3.1/cravat/webresult/images/download-material-black.png`

 * *Files identical despite different names*

### Comparing `open-cravat-2.3.0/cravat/webresult/images/download-material-blue.png` & `open-cravat-2.3.1/cravat/webresult/images/download-material-blue.png`

 * *Files identical despite different names*

### Comparing `open-cravat-2.3.0/cravat/webresult/images/download.svg` & `open-cravat-2.3.1/cravat/webresult/images/download.svg`

 * *Files identical despite different names*

### Comparing `open-cravat-2.3.0/cravat/webresult/images/help_16x16.gif` & `open-cravat-2.3.1/cravat/webresult/images/help_16x16.gif`

 * *Files identical despite different names*

### Comparing `open-cravat-2.3.0/cravat/webresult/images/help_icon.png` & `open-cravat-2.3.1/cravat/webresult/images/help_icon.png`

 * *Files identical despite different names*

### Comparing `open-cravat-2.3.0/cravat/webresult/images/loading-gif-animation.gif` & `open-cravat-2.3.1/cravat/webresult/images/loading-gif-animation.gif`

 * *Files identical despite different names*

### Comparing `open-cravat-2.3.0/cravat/webresult/images/mail.png` & `open-cravat-2.3.1/cravat/webresult/images/mail.png`

 * *Files identical despite different names*

### Comparing `open-cravat-2.3.0/cravat/webresult/images/menu.png` & `open-cravat-2.3.1/cravat/webresult/images/menu.png`

 * *Files identical despite different names*

### Comparing `open-cravat-2.3.0/cravat/webresult/images/openNewTab.png` & `open-cravat-2.3.1/cravat/webresult/images/openNewTab.png`

 * *Files identical despite different names*

### Comparing `open-cravat-2.3.0/cravat/webresult/images/package.png` & `open-cravat-2.3.1/cravat/webresult/images/package.png`

 * *Files identical despite different names*

### Comparing `open-cravat-2.3.0/cravat/webresult/images/pencil.png` & `open-cravat-2.3.1/cravat/webresult/images/pencil.png`

 * *Files identical despite different names*

### Comparing `open-cravat-2.3.0/cravat/webresult/images/pin-2.png` & `open-cravat-2.3.1/cravat/webresult/images/pin-2.png`

 * *Files identical despite different names*

### Comparing `open-cravat-2.3.0/cravat/webresult/images/pin.png` & `open-cravat-2.3.1/cravat/webresult/images/pin.png`

 * *Files identical despite different names*

### Comparing `open-cravat-2.3.0/cravat/webresult/images/pin.svg` & `open-cravat-2.3.1/cravat/webresult/images/pin.svg`

 * *Files identical despite different names*

### Comparing `open-cravat-2.3.0/cravat/webresult/images/plus-circle-dotted.svg` & `open-cravat-2.3.1/cravat/webresult/images/plus-circle-dotted.svg`

 * *Files identical despite different names*

### Comparing `open-cravat-2.3.0/cravat/webresult/images/question.png` & `open-cravat-2.3.1/cravat/webresult/images/question.png`

 * *Files identical despite different names*

### Comparing `open-cravat-2.3.0/cravat/webresult/images/resize.jpg` & `open-cravat-2.3.1/cravat/webresult/images/resize.jpg`

 * *Files identical despite different names*

### Comparing `open-cravat-2.3.0/cravat/webresult/images/save.png` & `open-cravat-2.3.1/cravat/webresult/images/save.png`

 * *Files identical despite different names*

### Comparing `open-cravat-2.3.0/cravat/webresult/images/save_new.png` & `open-cravat-2.3.1/cravat/webresult/images/save_new.png`

 * *Files identical despite different names*

### Comparing `open-cravat-2.3.0/cravat/webresult/images/search.png` & `open-cravat-2.3.1/cravat/webresult/images/search.png`

 * *Files identical despite different names*

### Comparing `open-cravat-2.3.0/cravat/webresult/images/sorry.png` & `open-cravat-2.3.1/cravat/webresult/images/sorry.png`

 * *Files identical despite different names*

### Comparing `open-cravat-2.3.0/cravat/webresult/images/spinCircle.gif` & `open-cravat-2.3.1/cravat/webresult/images/spinCircle.gif`

 * *Files identical despite different names*

### Comparing `open-cravat-2.3.0/cravat/webresult/images/spinner.gif` & `open-cravat-2.3.1/cravat/webresult/images/spinner.gif`

 * *Files identical despite different names*

### Comparing `open-cravat-2.3.0/cravat/webresult/images/triangle-down.png` & `open-cravat-2.3.1/cravat/webresult/images/triangle-down.png`

 * *Files identical despite different names*

### Comparing `open-cravat-2.3.0/cravat/webresult/images/triangle-right.png` & `open-cravat-2.3.1/cravat/webresult/images/triangle-right.png`

 * *Files identical despite different names*

### Comparing `open-cravat-2.3.0/cravat/webresult/images/upload-material-black.png` & `open-cravat-2.3.1/cravat/webresult/images/upload-material-black.png`

 * *Files identical despite different names*

### Comparing `open-cravat-2.3.0/cravat/webresult/images/upload-material-blue.png` & `open-cravat-2.3.1/cravat/webresult/images/upload-material-blue.png`

 * *Files identical despite different names*

### Comparing `open-cravat-2.3.0/cravat/webresult/index.html` & `open-cravat-2.3.1/cravat/webresult/index.html`

 * *Files identical despite different names*

### Comparing `open-cravat-2.3.0/cravat/webresult/js/Chart.js` & `open-cravat-2.3.1/cravat/webresult/js/Chart.js`

 * *Files identical despite different names*

### Comparing `open-cravat-2.3.0/cravat/webresult/js/dom-to-image.min.js` & `open-cravat-2.3.1/cravat/webresult/js/dom-to-image.min.js`

 * *Files identical despite different names*

### Comparing `open-cravat-2.3.0/cravat/webresult/js/download.js` & `open-cravat-2.3.1/cravat/webresult/js/download.js`

 * *Files identical despite different names*

### Comparing `open-cravat-2.3.0/cravat/webresult/js/graphics.js` & `open-cravat-2.3.1/cravat/webresult/js/graphics.js`

 * *Files identical despite different names*

### Comparing `open-cravat-2.3.0/cravat/webresult/js/jquery-3.2.1.min.js` & `open-cravat-2.3.1/cravat/webresult/js/jquery-3.2.1.min.js`

 * *Files identical despite different names*

### Comparing `open-cravat-2.3.0/cravat/webresult/js/jquery-ui-1.12.1.custom/AUTHORS.txt` & `open-cravat-2.3.1/cravat/webresult/js/jquery-ui-1.12.1.custom/AUTHORS.txt`

 * *Files identical despite different names*

### Comparing `open-cravat-2.3.0/cravat/webresult/js/jquery-ui-1.12.1.custom/LICENSE.txt` & `open-cravat-2.3.1/cravat/webresult/js/jquery-ui-1.12.1.custom/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `open-cravat-2.3.0/cravat/webresult/js/jquery-ui-1.12.1.custom/external/jquery/jquery.js` & `open-cravat-2.3.1/cravat/webresult/js/jquery-ui-1.12.1.custom/external/jquery/jquery.js`

 * *Files identical despite different names*

### Comparing `open-cravat-2.3.0/cravat/webresult/js/jquery-ui-1.12.1.custom/images/ui-icons_444444_256x240.png` & `open-cravat-2.3.1/cravat/webresult/js/jquery-ui-1.12.1.custom/images/ui-icons_444444_256x240.png`

 * *Files identical despite different names*

### Comparing `open-cravat-2.3.0/cravat/webresult/js/jquery-ui-1.12.1.custom/images/ui-icons_555555_256x240.png` & `open-cravat-2.3.1/cravat/webresult/js/jquery-ui-1.12.1.custom/images/ui-icons_555555_256x240.png`

 * *Files identical despite different names*

### Comparing `open-cravat-2.3.0/cravat/webresult/js/jquery-ui-1.12.1.custom/images/ui-icons_777620_256x240.png` & `open-cravat-2.3.1/cravat/webresult/js/jquery-ui-1.12.1.custom/images/ui-icons_777620_256x240.png`

 * *Files identical despite different names*

### Comparing `open-cravat-2.3.0/cravat/webresult/js/jquery-ui-1.12.1.custom/images/ui-icons_777777_256x240.png` & `open-cravat-2.3.1/cravat/webresult/js/jquery-ui-1.12.1.custom/images/ui-icons_777777_256x240.png`

 * *Files identical despite different names*

### Comparing `open-cravat-2.3.0/cravat/webresult/js/jquery-ui-1.12.1.custom/images/ui-icons_cc0000_256x240.png` & `open-cravat-2.3.1/cravat/webresult/js/jquery-ui-1.12.1.custom/images/ui-icons_cc0000_256x240.png`

 * *Files identical despite different names*

### Comparing `open-cravat-2.3.0/cravat/webresult/js/jquery-ui-1.12.1.custom/images/ui-icons_ffffff_256x240.png` & `open-cravat-2.3.1/cravat/webresult/js/jquery-ui-1.12.1.custom/images/ui-icons_ffffff_256x240.png`

 * *Files identical despite different names*

### Comparing `open-cravat-2.3.0/cravat/webresult/js/jquery-ui-1.12.1.custom/index.html` & `open-cravat-2.3.1/cravat/webresult/js/jquery-ui-1.12.1.custom/index.html`

 * *Files identical despite different names*

### Comparing `open-cravat-2.3.0/cravat/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.css` & `open-cravat-2.3.1/cravat/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.css`

 * *Files identical despite different names*

### Comparing `open-cravat-2.3.0/cravat/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.js` & `open-cravat-2.3.1/cravat/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.js`

 * *Files identical despite different names*

### Comparing `open-cravat-2.3.0/cravat/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.min.css` & `open-cravat-2.3.1/cravat/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.min.css`

 * *Files identical despite different names*

### Comparing `open-cravat-2.3.0/cravat/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.min.js` & `open-cravat-2.3.1/cravat/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.min.js`

 * *Files identical despite different names*

### Comparing `open-cravat-2.3.0/cravat/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.structure.css` & `open-cravat-2.3.1/cravat/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.structure.css`

 * *Files identical despite different names*

### Comparing `open-cravat-2.3.0/cravat/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.structure.min.css` & `open-cravat-2.3.1/cravat/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.structure.min.css`

 * *Files identical despite different names*

### Comparing `open-cravat-2.3.0/cravat/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.theme.css` & `open-cravat-2.3.1/cravat/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.theme.css`

 * *Files identical despite different names*

### Comparing `open-cravat-2.3.0/cravat/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.theme.min.css` & `open-cravat-2.3.1/cravat/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.theme.min.css`

 * *Files identical despite different names*

### Comparing `open-cravat-2.3.0/cravat/webresult/js/jquery-ui-1.12.1.custom/package.json` & `open-cravat-2.3.1/cravat/webresult/js/jquery-ui-1.12.1.custom/package.json`

 * *Files identical despite different names*

### Comparing `open-cravat-2.3.0/cravat/webresult/js/jquery.tools.min.js` & `open-cravat-2.3.1/cravat/webresult/js/jquery.tools.min.js`

 * *Files identical despite different names*

### Comparing `open-cravat-2.3.0/cravat/webresult/js/jquery.url.js` & `open-cravat-2.3.1/cravat/webresult/js/jquery.url.js`

 * *Files identical despite different names*

### Comparing `open-cravat-2.3.0/cravat/webresult/js/packery.pkgd.js` & `open-cravat-2.3.1/cravat/webresult/js/packery.pkgd.js`

 * *Files identical despite different names*

### Comparing `open-cravat-2.3.0/cravat/webresult/js/paramquery-pro-3/ChangeLog.txt` & `open-cravat-2.3.1/cravat/webresult/js/paramquery-pro-3/ChangeLog.txt`

 * *Files identical despite different names*

### Comparing `open-cravat-2.3.0/cravat/webresult/js/paramquery-pro-3/EULA.pdf` & `open-cravat-2.3.1/cravat/webresult/js/paramquery-pro-3/EULA.pdf`

 * *Files identical despite different names*

### Comparing `open-cravat-2.3.0/cravat/webresult/js/paramquery-pro-3/images/loading.gif` & `open-cravat-2.3.1/cravat/webresult/js/paramquery-pro-3/images/loading.gif`

 * *Files identical despite different names*

### Comparing `open-cravat-2.3.0/cravat/webresult/js/paramquery-pro-3/images/sprite.png` & `open-cravat-2.3.1/cravat/webresult/js/paramquery-pro-3/images/sprite.png`

 * *Files identical despite different names*

### Comparing `open-cravat-2.3.0/cravat/webresult/js/paramquery-pro-3/jsZip-2.5.0/MIT-License.txt` & `open-cravat-2.3.1/cravat/webresult/js/paramquery-pro-3/jsZip-2.5.0/MIT-License.txt`

 * *Files identical despite different names*

### Comparing `open-cravat-2.3.0/cravat/webresult/js/paramquery-pro-3/jsZip-2.5.0/jszip.min.js` & `open-cravat-2.3.1/cravat/webresult/js/paramquery-pro-3/jsZip-2.5.0/jszip.min.js`

 * *Files identical despite different names*

### Comparing `open-cravat-2.3.0/cravat/webresult/js/paramquery-pro-3/localize/pq-localize-de.js` & `open-cravat-2.3.1/cravat/webresult/js/paramquery-pro-3/localize/pq-localize-de.js`

 * *Files identical despite different names*

### Comparing `open-cravat-2.3.0/cravat/webresult/js/paramquery-pro-3/localize/pq-localize-en.js` & `open-cravat-2.3.1/cravat/webresult/js/paramquery-pro-3/localize/pq-localize-en.js`

 * *Files identical despite different names*

### Comparing `open-cravat-2.3.0/cravat/webresult/js/paramquery-pro-3/localize/pq-localize-es.js` & `open-cravat-2.3.1/cravat/webresult/js/paramquery-pro-3/localize/pq-localize-es.js`

 * *Files identical despite different names*

### Comparing `open-cravat-2.3.0/cravat/webresult/js/paramquery-pro-3/localize/pq-localize-fr.js` & `open-cravat-2.3.1/cravat/webresult/js/paramquery-pro-3/localize/pq-localize-fr.js`

 * *Files identical despite different names*

### Comparing `open-cravat-2.3.0/cravat/webresult/js/paramquery-pro-3/localize/pq-localize-hu.js` & `open-cravat-2.3.1/cravat/webresult/js/paramquery-pro-3/localize/pq-localize-hu.js`

 * *Files identical despite different names*

### Comparing `open-cravat-2.3.0/cravat/webresult/js/paramquery-pro-3/localize/pq-localize-it.js` & `open-cravat-2.3.1/cravat/webresult/js/paramquery-pro-3/localize/pq-localize-it.js`

 * *Files identical despite different names*

### Comparing `open-cravat-2.3.0/cravat/webresult/js/paramquery-pro-3/localize/pq-localize-ja.js` & `open-cravat-2.3.1/cravat/webresult/js/paramquery-pro-3/localize/pq-localize-ja.js`

 * *Files identical despite different names*

### Comparing `open-cravat-2.3.0/cravat/webresult/js/paramquery-pro-3/localize/pq-localize-nl.js` & `open-cravat-2.3.1/cravat/webresult/js/paramquery-pro-3/localize/pq-localize-nl.js`

 * *Files identical despite different names*

### Comparing `open-cravat-2.3.0/cravat/webresult/js/paramquery-pro-3/localize/pq-localize-pl.js` & `open-cravat-2.3.1/cravat/webresult/js/paramquery-pro-3/localize/pq-localize-pl.js`

 * *Files identical despite different names*

### Comparing `open-cravat-2.3.0/cravat/webresult/js/paramquery-pro-3/localize/pq-localize-pt.js` & `open-cravat-2.3.1/cravat/webresult/js/paramquery-pro-3/localize/pq-localize-pt.js`

 * *Files identical despite different names*

### Comparing `open-cravat-2.3.0/cravat/webresult/js/paramquery-pro-3/localize/pq-localize-tr.js` & `open-cravat-2.3.1/cravat/webresult/js/paramquery-pro-3/localize/pq-localize-tr.js`

 * *Files identical despite different names*

### Comparing `open-cravat-2.3.0/cravat/webresult/js/paramquery-pro-3/localize/pq-localize-zh.js` & `open-cravat-2.3.1/cravat/webresult/js/paramquery-pro-3/localize/pq-localize-zh.js`

 * *Files identical despite different names*

### Comparing `open-cravat-2.3.0/cravat/webresult/js/paramquery-pro-3/pqSelect/ChangeLog.txt` & `open-cravat-2.3.1/cravat/webresult/js/paramquery-pro-3/pqSelect/ChangeLog.txt`

 * *Files identical despite different names*

### Comparing `open-cravat-2.3.0/cravat/webresult/js/paramquery-pro-3/pqSelect/pqselect.bootstrap.dev.css` & `open-cravat-2.3.1/cravat/webresult/js/paramquery-pro-3/pqSelect/pqselect.bootstrap.dev.css`

 * *Files identical despite different names*

### Comparing `open-cravat-2.3.0/cravat/webresult/js/paramquery-pro-3/pqSelect/pqselect.bootstrap.min.css` & `open-cravat-2.3.1/cravat/webresult/js/paramquery-pro-3/pqSelect/pqselect.bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `open-cravat-2.3.0/cravat/webresult/js/paramquery-pro-3/pqSelect/pqselect.dev.css` & `open-cravat-2.3.1/cravat/webresult/js/paramquery-pro-3/pqSelect/pqselect.dev.css`

 * *Files identical despite different names*

### Comparing `open-cravat-2.3.0/cravat/webresult/js/paramquery-pro-3/pqSelect/pqselect.dev.js` & `open-cravat-2.3.1/cravat/webresult/js/paramquery-pro-3/pqSelect/pqselect.dev.js`

 * *Files identical despite different names*

### Comparing `open-cravat-2.3.0/cravat/webresult/js/paramquery-pro-3/pqSelect/pqselect.min.css` & `open-cravat-2.3.1/cravat/webresult/js/paramquery-pro-3/pqSelect/pqselect.min.css`

 * *Files identical despite different names*

### Comparing `open-cravat-2.3.0/cravat/webresult/js/paramquery-pro-3/pqSelect/pqselect.min.js` & `open-cravat-2.3.1/cravat/webresult/js/paramquery-pro-3/pqSelect/pqselect.min.js`

 * *Files identical despite different names*

### Comparing `open-cravat-2.3.0/cravat/webresult/js/paramquery-pro-3/pqgrid.bootstrap.dev.css` & `open-cravat-2.3.1/cravat/webresult/js/paramquery-pro-3/pqgrid.bootstrap.dev.css`

 * *Files identical despite different names*

### Comparing `open-cravat-2.3.0/cravat/webresult/js/paramquery-pro-3/pqgrid.bootstrap.min.css` & `open-cravat-2.3.1/cravat/webresult/js/paramquery-pro-3/pqgrid.bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `open-cravat-2.3.0/cravat/webresult/js/paramquery-pro-3/pqgrid.dev.css` & `open-cravat-2.3.1/cravat/webresult/js/paramquery-pro-3/pqgrid.dev.css`

 * *Files identical despite different names*

### Comparing `open-cravat-2.3.0/cravat/webresult/js/paramquery-pro-3/pqgrid.dev.js` & `open-cravat-2.3.1/cravat/webresult/js/paramquery-pro-3/pqgrid.dev.js`

 * *Files identical despite different names*

### Comparing `open-cravat-2.3.0/cravat/webresult/js/paramquery-pro-3/pqgrid.min.css` & `open-cravat-2.3.1/cravat/webresult/js/paramquery-pro-3/pqgrid.min.css`

 * *Files identical despite different names*

### Comparing `open-cravat-2.3.0/cravat/webresult/js/paramquery-pro-3/pqgrid.min.js` & `open-cravat-2.3.1/cravat/webresult/js/paramquery-pro-3/pqgrid.min.js`

 * *Files identical despite different names*

### Comparing `open-cravat-2.3.0/cravat/webresult/js/paramquery-pro-3/pqgrid.ui.dev.css` & `open-cravat-2.3.1/cravat/webresult/js/paramquery-pro-3/pqgrid.ui.dev.css`

 * *Files identical despite different names*

### Comparing `open-cravat-2.3.0/cravat/webresult/js/paramquery-pro-3/pqgrid.ui.min.css` & `open-cravat-2.3.1/cravat/webresult/js/paramquery-pro-3/pqgrid.ui.min.css`

 * *Files identical despite different names*

### Comparing `open-cravat-2.3.0/cravat/webresult/js/paramquery-pro-3/readme.txt` & `open-cravat-2.3.1/cravat/webresult/js/paramquery-pro-3/readme.txt`

 * *Files identical despite different names*

### Comparing `open-cravat-2.3.0/cravat/webresult/js/paramquery-pro-3/themes/bootstrap/pqgrid.css` & `open-cravat-2.3.1/cravat/webresult/js/paramquery-pro-3/themes/bootstrap/pqgrid.css`

 * *Files identical despite different names*

### Comparing `open-cravat-2.3.0/cravat/webresult/js/paramquery-pro-3/themes/brown/pqgrid.css` & `open-cravat-2.3.1/cravat/webresult/js/paramquery-pro-3/themes/brown/pqgrid.css`

 * *Files identical despite different names*

### Comparing `open-cravat-2.3.0/cravat/webresult/js/paramquery-pro-3/themes/chocolate/pqgrid.css` & `open-cravat-2.3.1/cravat/webresult/js/paramquery-pro-3/themes/chocolate/pqgrid.css`

 * *Files identical despite different names*

### Comparing `open-cravat-2.3.0/cravat/webresult/js/paramquery-pro-3/themes/cocoa/pqgrid.css` & `open-cravat-2.3.1/cravat/webresult/js/paramquery-pro-3/themes/cocoa/pqgrid.css`

 * *Files identical despite different names*

### Comparing `open-cravat-2.3.0/cravat/webresult/js/paramquery-pro-3/themes/crimson/pqgrid.css` & `open-cravat-2.3.1/cravat/webresult/js/paramquery-pro-3/themes/crimson/pqgrid.css`

 * *Files identical despite different names*

### Comparing `open-cravat-2.3.0/cravat/webresult/js/paramquery-pro-3/themes/gray/pqgrid.css` & `open-cravat-2.3.1/cravat/webresult/js/paramquery-pro-3/themes/gray/pqgrid.css`

 * *Files identical despite different names*

### Comparing `open-cravat-2.3.0/cravat/webresult/js/paramquery-pro-3/themes/indigo/pqgrid.css` & `open-cravat-2.3.1/cravat/webresult/js/paramquery-pro-3/themes/indigo/pqgrid.css`

 * *Files identical despite different names*

### Comparing `open-cravat-2.3.0/cravat/webresult/js/paramquery-pro-3/themes/office/pqgrid.css` & `open-cravat-2.3.1/cravat/webresult/js/paramquery-pro-3/themes/office/pqgrid.css`

 * *Files identical despite different names*

### Comparing `open-cravat-2.3.0/cravat/webresult/js/paramquery-pro-3/themes/purple/pqgrid.css` & `open-cravat-2.3.1/cravat/webresult/js/paramquery-pro-3/themes/purple/pqgrid.css`

 * *Files identical despite different names*

### Comparing `open-cravat-2.3.0/cravat/webresult/js/paramquery-pro-3/themes/red/pqgrid.css` & `open-cravat-2.3.1/cravat/webresult/js/paramquery-pro-3/themes/red/pqgrid.css`

 * *Files identical despite different names*

### Comparing `open-cravat-2.3.0/cravat/webresult/js/paramquery-pro-3/themes/rosybrown/pqgrid.css` & `open-cravat-2.3.1/cravat/webresult/js/paramquery-pro-3/themes/rosybrown/pqgrid.css`

 * *Files identical despite different names*

### Comparing `open-cravat-2.3.0/cravat/webresult/js/paramquery-pro-3/themes/sandybrown/pqgrid.css` & `open-cravat-2.3.1/cravat/webresult/js/paramquery-pro-3/themes/sandybrown/pqgrid.css`

 * *Files identical despite different names*

### Comparing `open-cravat-2.3.0/cravat/webresult/js/paramquery-pro-3/themes/steelblue/pqgrid.css` & `open-cravat-2.3.1/cravat/webresult/js/paramquery-pro-3/themes/steelblue/pqgrid.css`

 * *Files identical despite different names*

### Comparing `open-cravat-2.3.0/cravat/webresult/js/paramquery-pro-3/themes/tan/pqgrid.css` & `open-cravat-2.3.1/cravat/webresult/js/paramquery-pro-3/themes/tan/pqgrid.css`

 * *Files identical despite different names*

### Comparing `open-cravat-2.3.0/cravat/webresult/js/paramquery-pro-3/themes/violet/pqgrid.css` & `open-cravat-2.3.1/cravat/webresult/js/paramquery-pro-3/themes/violet/pqgrid.css`

 * *Files identical despite different names*

### Comparing `open-cravat-2.3.0/cravat/webresult/js/paramquery-pro-3/touch-punch/ChangeLog.txt` & `open-cravat-2.3.1/cravat/webresult/js/paramquery-pro-3/touch-punch/ChangeLog.txt`

 * *Files identical despite different names*

### Comparing `open-cravat-2.3.0/cravat/webresult/js/paramquery-pro-3/touch-punch/MIT-LICENSE.txt` & `open-cravat-2.3.1/cravat/webresult/js/paramquery-pro-3/touch-punch/MIT-LICENSE.txt`

 * *Files identical despite different names*

### Comparing `open-cravat-2.3.0/cravat/webresult/js/paramquery-pro-3/touch-punch/README.md` & `open-cravat-2.3.1/cravat/webresult/js/paramquery-pro-3/touch-punch/README.md`

 * *Files identical despite different names*

### Comparing `open-cravat-2.3.0/cravat/webresult/js/paramquery-pro-3/touch-punch/touch-punch.dev.js` & `open-cravat-2.3.1/cravat/webresult/js/paramquery-pro-3/touch-punch/touch-punch.dev.js`

 * *Files identical despite different names*

### Comparing `open-cravat-2.3.0/cravat/webresult/js/paramquery-pro-3/touch-punch/touch-punch.min.js` & `open-cravat-2.3.1/cravat/webresult/js/paramquery-pro-3/touch-punch/touch-punch.min.js`

 * *Files identical despite different names*

### Comparing `open-cravat-2.3.0/cravat/webresult/js/pqselect.min.js` & `open-cravat-2.3.1/cravat/webresult/js/pqselect.min.js`

 * *Files identical despite different names*

### Comparing `open-cravat-2.3.0/cravat/webresult/js/raphael-min.js` & `open-cravat-2.3.1/cravat/webresult/js/raphael-min.js`

 * *Files identical despite different names*

### Comparing `open-cravat-2.3.0/cravat/webresult/jsonreporter.py` & `open-cravat-2.3.1/cravat/webresult/jsonreporter.py`

 * *Files identical despite different names*

### Comparing `open-cravat-2.3.0/cravat/webresult/nocache/css/singlevariantpage.css` & `open-cravat-2.3.1/cravat/webresult/nocache/css/singlevariantpage.css`

 * *Files identical despite different names*

### Comparing `open-cravat-2.3.0/cravat/webresult/nocache/css/style.css` & `open-cravat-2.3.1/cravat/webresult/nocache/css/style.css`

 * *Files identical despite different names*

### Comparing `open-cravat-2.3.0/cravat/webresult/nocache/css/widget.css` & `open-cravat-2.3.1/cravat/webresult/nocache/css/widget.css`

 * *Files identical despite different names*

### Comparing `open-cravat-2.3.0/cravat/webresult/nocache/js/filter.js` & `open-cravat-2.3.1/cravat/webresult/nocache/js/filter.js`

 * *Files identical despite different names*

### Comparing `open-cravat-2.3.0/cravat/webresult/nocache/js/infomgr.js` & `open-cravat-2.3.1/cravat/webresult/nocache/js/infomgr.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -16,26 +16,35 @@
 }
 
 InfoMgr.prototype.getStatus = function(jobId) {
     var self = this;
     self.jobId = jobId;
 }
 
-InfoMgr.prototype.count = function(dbPath, tabName, callback) {
+InfoMgr.prototype.count = function(dbPath, tabName, callback, retries) {
     const data = {
         username: username,
         job_id: jobId,
         tab: tabName,
         dbpath: dbPath,
         filter: JSON.stringify(filterJson),
     };
     $.post('/result/service/count', data).done(function(jsonResponseData) {
-        var msg = jsonResponseData['n'] + ' variants meet the criteria';
-        callback(msg, jsonResponseData);
-    });
+            var msg = jsonResponseData['n'] + ' variants meet the criteria';
+            callback(msg, jsonResponseData);
+        })
+        .fail(function(jsonResponseData) {
+            var msg = JSON.parse(jsonResponseData.responseText)['msg']
+            if (msg === 'database is locked' && retries !== undefined && retries > 0) {
+                retries = retries - 1;
+                infomgr.count(dbPath, tabName, callback, retries);
+            } else {
+                callback('Error ' + msg + ' Please try again in a few minutes.');
+            }
+        });
 }
 
 InfoMgr.prototype.load = function(jobId, tabName, callback, callbackArgs, fJson, fetchtype) {
     var self = this;
     if (fetchtype == 'job') {
         if (jobDataLoadingDiv == null) {
             drawingRetrievingDataDiv(tabName);
```

### Comparing `open-cravat-2.3.0/cravat/webresult/nocache/js/main.js` & `open-cravat-2.3.1/cravat/webresult/nocache/js/main.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -654,15 +654,18 @@
                 }
                 removeLoadingDiv();
                 firstLoad = true;
                 return;
             }
             if (filterJson.length != 0) {
                 infomgr.count(dbPath, 'variant', function(numvar) {
-                    if (numvar > NUMVAR_LIMIT) {
+                    if (numvar.includes('Error')) {
+                        removeLoadingDiv();
+                        alert(numvar);
+                    } else if (numvar > NUMVAR_LIMIT) {
                         lockTabs();
                         flagNotifyToUseFilter = true;
                         if (document.getElementById('infonoticediv')) {
                             notifyToUseFilter();
                             flagNotifyToUseFilter = false;
                         } else {
                             flagNotifyToUseFilter = true;
@@ -673,15 +676,15 @@
                         if (flagNotifyToUseFilter) {
                             notifyOfReadyToLoad();
                             flagNotifyToUseFilter = false;
                         }
                         //removeLoadingDiv();
                         callLoadVariant();
                     }
-                });
+                }, 5);
             } else {
                 if (flagNotifyToUseFilter) {
                     notifyOfReadyToLoad();
                     flagNotifyToUseFilter = false;
                 }
                 //removeLoadingDiv();
                 callLoadVariant();
@@ -1124,15 +1127,33 @@
     $.get('/result/service/variantcols', {
         job_id: jobId,
         username: username,
         dbpath: dbPath,
         confpath: confPath,
         filter: JSON.stringify(filterJson)
     }).done(function(jsonResponseData) {
-        filterCols = jsonResponseData['columns']['variant'];
+        allVarCols = JSON.parse(JSON.stringify(jsonResponseData['columns']['variant']));
+        filterCols = [];
+        for (let colGroup of allVarCols) {
+            if (colGroup.name === 'vcfinfo') {
+                let filterableCols = [];
+                for (let col of colGroup.colModel) {
+                    if (col.filterable) {
+                        filterableCols.push(col);
+                    }
+                }
+                if (filterableCols.length > 0) {
+                    filterCols.push(colGroup);
+                    filterCols.slice(-1)[0].colModel = filterableCols;
+                }
+            } else {
+                filterCols.push(colGroup)
+            }
+
+        }
         usedAnnotators = {};
         var cols = jsonResponseData['columns']['variant'];
         usedAnnotators['variant'] = [];
         usedAnnotators['info'] = [];
         for (var i = 0; i < cols.length; i++) {
             var col = cols[i];
             var annotator = col.colModel[0].colgroupkey;
@@ -1140,14 +1161,21 @@
             usedAnnotators['info'].push(annotator);
         }
         if (jsonResponseData['columns']['gene']) {
             var cols = jsonResponseData['columns']['gene'];
             usedAnnotators['gene'] = [];
             for (var i = 0; i < cols.length; i++) {
                 var col = cols[i];
+                if (col.name === 'base') {
+                    for (let subCol of col.colModel) {
+                        if (subCol.col === 'base__note_gene') {
+                            filterCols[0].colModel.push(subCol)
+                        }
+                    }
+                }
                 var annotator = col.colModel[0].colgroupkey;
                 usedAnnotators['gene'].push(annotator);
                 usedAnnotators['info'].push(annotator);
             }
         }
         firstLoadData();
     });
```

### Comparing `open-cravat-2.3.0/cravat/webresult/nocache/js/setup.js` & `open-cravat-2.3.1/cravat/webresult/nocache/js/setup.js`

 * *Files identical despite different names*

### Comparing `open-cravat-2.3.0/cravat/webresult/nocache/js/showvariant.js` & `open-cravat-2.3.1/cravat/webresult/nocache/js/showvariant.js`

 * *Files identical despite different names*

### Comparing `open-cravat-2.3.0/cravat/webresult/nocache/js/singlevariantpage.js` & `open-cravat-2.3.1/cravat/webresult/nocache/js/singlevariantpage.js`

 * *Files identical despite different names*

### Comparing `open-cravat-2.3.0/cravat/webresult/nocache/js/util.js` & `open-cravat-2.3.1/cravat/webresult/nocache/js/util.js`

 * *Files identical despite different names*

### Comparing `open-cravat-2.3.0/cravat/webresult/nocache/js/variables.js` & `open-cravat-2.3.1/cravat/webresult/nocache/js/variables.js`

 * *Files identical despite different names*

### Comparing `open-cravat-2.3.0/cravat/webresult/nocache/js/widgethelper.js` & `open-cravat-2.3.1/cravat/webresult/nocache/js/widgethelper.js`

 * *Files identical despite different names*

### Comparing `open-cravat-2.3.0/cravat/webresult/nocache/variant.html` & `open-cravat-2.3.1/cravat/webresult/nocache/variant.html`

 * *Files identical despite different names*

### Comparing `open-cravat-2.3.0/cravat/webresult/question.png` & `open-cravat-2.3.1/cravat/webresult/question.png`

 * *Files identical despite different names*

### Comparing `open-cravat-2.3.0/cravat/webresult/webresult.py` & `open-cravat-2.3.1/cravat/webresult/webresult.py`

 * *Files identical despite different names*

### Comparing `open-cravat-2.3.0/cravat/webstore/cravat_store.css` & `open-cravat-2.3.1/cravat/webstore/cravat_store.css`

 * *Files identical despite different names*

### Comparing `open-cravat-2.3.0/cravat/webstore/favicon.ico` & `open-cravat-2.3.1/cravat/webstore/favicon.ico`

 * *Files identical despite different names*

### Comparing `open-cravat-2.3.0/cravat/webstore/images/chat-dots.svg` & `open-cravat-2.3.1/cravat/webstore/images/chat-dots.svg`

 * *Files identical despite different names*

### Comparing `open-cravat-2.3.0/cravat/webstore/images/chat-left-text.svg` & `open-cravat-2.3.1/cravat/webstore/images/chat-left-text.svg`

 * *Files identical despite different names*

### Comparing `open-cravat-2.3.0/cravat/webstore/images/done.png` & `open-cravat-2.3.1/cravat/webstore/images/done.png`

 * *Files identical despite different names*

### Comparing `open-cravat-2.3.0/cravat/webstore/images/email.png` & `open-cravat-2.3.1/cravat/webstore/images/email.png`

 * *Files identical despite different names*

### Comparing `open-cravat-2.3.0/cravat/webstore/images/empty.png` & `open-cravat-2.3.1/cravat/webstore/images/empty.png`

 * *Files identical despite different names*

### Comparing `open-cravat-2.3.0/cravat/webstore/images/favicon.png` & `open-cravat-2.3.1/cravat/webstore/images/favicon.png`

 * *Files identical despite different names*

### Comparing `open-cravat-2.3.0/cravat/webstore/images/folder.png` & `open-cravat-2.3.1/cravat/webstore/images/folder.png`

 * *Files identical despite different names*

### Comparing `open-cravat-2.3.0/cravat/webstore/images/genericmodulelogo.png` & `open-cravat-2.3.1/cravat/webstore/images/genericmodulelogo.png`

 * *Files identical despite different names*

### Comparing `open-cravat-2.3.0/cravat/webstore/images/hamburger.png` & `open-cravat-2.3.1/cravat/webstore/images/hamburger.png`

 * *Files identical despite different names*

### Comparing `open-cravat-2.3.0/cravat/webstore/images/left_arrow.png` & `open-cravat-2.3.1/cravat/webstore/images/left_arrow.png`

 * *Files identical despite different names*

### Comparing `open-cravat-2.3.0/cravat/webstore/images/logo.png` & `open-cravat-2.3.1/cravat/webstore/images/logo.png`

 * *Files identical despite different names*

### Comparing `open-cravat-2.3.0/cravat/webstore/images/new.png` & `open-cravat-2.3.1/cravat/webstore/images/new.png`

 * *Files identical despite different names*

### Comparing `open-cravat-2.3.0/cravat/webstore/images/question.png` & `open-cravat-2.3.1/cravat/webstore/images/question.png`

 * *Files identical despite different names*

### Comparing `open-cravat-2.3.0/cravat/webstore/images/right_arrow.png` & `open-cravat-2.3.1/cravat/webstore/images/right_arrow.png`

 * *Files identical despite different names*

### Comparing `open-cravat-2.3.0/cravat/webstore/jquery-3.3.1.min.js` & `open-cravat-2.3.1/cravat/webstore/jquery-3.3.1.min.js`

 * *Files identical despite different names*

### Comparing `open-cravat-2.3.0/cravat/webstore/js/showdown-1.9.1.min.js` & `open-cravat-2.3.1/cravat/webstore/js/showdown-1.9.1.min.js`

 * *Files identical despite different names*

### Comparing `open-cravat-2.3.0/cravat/webstore/js/showdown.min.js.map` & `open-cravat-2.3.1/cravat/webstore/js/showdown.min.js.map`

 * *Files identical despite different names*

### Comparing `open-cravat-2.3.0/cravat/webstore/nocache/webstore.css` & `open-cravat-2.3.1/cravat/webstore/nocache/webstore.css`

 * *Files identical despite different names*

### Comparing `open-cravat-2.3.0/cravat/webstore/nocache/webstore.js` & `open-cravat-2.3.1/cravat/webstore/nocache/webstore.js`

 * *Files identical despite different names*

### Comparing `open-cravat-2.3.0/cravat/webstore/sse.py` & `open-cravat-2.3.1/cravat/webstore/sse.py`

 * *Files identical despite different names*

### Comparing `open-cravat-2.3.0/cravat/webstore/store_handlers.py` & `open-cravat-2.3.1/cravat/webstore/store_handlers.py`

 * *Files identical despite different names*

### Comparing `open-cravat-2.3.0/cravat/webstore/webstore.py` & `open-cravat-2.3.1/cravat/webstore/webstore.py`

 * *Files identical despite different names*

### Comparing `open-cravat-2.3.0/cravat/webstore/ws.js` & `open-cravat-2.3.1/cravat/webstore/ws.js`

 * *Files identical despite different names*

### Comparing `open-cravat-2.3.0/cravat/websubmit/Chart.bundle.min.js` & `open-cravat-2.3.1/cravat/websubmit/Chart.bundle.min.js`

 * *Files identical despite different names*

### Comparing `open-cravat-2.3.0/cravat/websubmit/arrow.png` & `open-cravat-2.3.1/cravat/websubmit/arrow.png`

 * *Files identical despite different names*

### Comparing `open-cravat-2.3.0/cravat/websubmit/down.png` & `open-cravat-2.3.1/cravat/websubmit/down.png`

 * *Files identical despite different names*

### Comparing `open-cravat-2.3.0/cravat/websubmit/email.png` & `open-cravat-2.3.1/cravat/websubmit/email.png`

 * *Files identical despite different names*

### Comparing `open-cravat-2.3.0/cravat/websubmit/favicon.ico` & `open-cravat-2.3.1/cravat/websubmit/favicon.ico`

 * *Files identical despite different names*

### Comparing `open-cravat-2.3.0/cravat/websubmit/favicon.png` & `open-cravat-2.3.1/cravat/websubmit/favicon.png`

 * *Files identical despite different names*

### Comparing `open-cravat-2.3.0/cravat/websubmit/help.png` & `open-cravat-2.3.1/cravat/websubmit/help.png`

 * *Files identical despite different names*

### Comparing `open-cravat-2.3.0/cravat/websubmit/input-examples/cravat.hg18.txt` & `open-cravat-2.3.1/cravat/websubmit/input-examples/cravat.hg18.txt`

 * *Files identical despite different names*

### Comparing `open-cravat-2.3.0/cravat/websubmit/input-examples/cravat.hg19.txt` & `open-cravat-2.3.1/cravat/websubmit/input-examples/cravat.hg19.txt`

 * *Files identical despite different names*

### Comparing `open-cravat-2.3.0/cravat/websubmit/input-examples/cravat.hg38.txt` & `open-cravat-2.3.1/cravat/websubmit/input-examples/cravat.hg38.txt`

 * *Files identical despite different names*

### Comparing `open-cravat-2.3.0/cravat/websubmit/input-examples/vcf.hg18.txt` & `open-cravat-2.3.1/cravat/websubmit/input-examples/vcf.hg18.txt`

 * *Files identical despite different names*

### Comparing `open-cravat-2.3.0/cravat/websubmit/input-examples/vcf.hg19.txt` & `open-cravat-2.3.1/cravat/websubmit/input-examples/vcf.hg19.txt`

 * *Files identical despite different names*

### Comparing `open-cravat-2.3.0/cravat/websubmit/input-examples/vcf.hg38.txt` & `open-cravat-2.3.1/cravat/websubmit/input-examples/vcf.hg38.txt`

 * *Files identical despite different names*

### Comparing `open-cravat-2.3.0/cravat/websubmit/jquery-3.3.1.min.js` & `open-cravat-2.3.1/cravat/websubmit/jquery-3.3.1.min.js`

 * *Files identical despite different names*

### Comparing `open-cravat-2.3.0/cravat/websubmit/logo.png` & `open-cravat-2.3.1/cravat/websubmit/logo.png`

 * *Files identical despite different names*

### Comparing `open-cravat-2.3.0/cravat/websubmit/logo_transparent.png` & `open-cravat-2.3.1/cravat/websubmit/logo_transparent.png`

 * *Files identical despite different names*

### Comparing `open-cravat-2.3.0/cravat/websubmit/nocache/broken_wheel.gif` & `open-cravat-2.3.1/cravat/websubmit/nocache/broken_wheel.gif`

 * *Files identical despite different names*

### Comparing `open-cravat-2.3.0/cravat/websubmit/nocache/index.html` & `open-cravat-2.3.1/cravat/websubmit/nocache/index.html`

 * *Files identical despite different names*

### Comparing `open-cravat-2.3.0/cravat/websubmit/nocache/websubmit.css` & `open-cravat-2.3.1/cravat/websubmit/nocache/websubmit.css`

 * *Files identical despite different names*

### Comparing `open-cravat-2.3.0/cravat/websubmit/nocache/websubmit.js` & `open-cravat-2.3.1/cravat/websubmit/nocache/websubmit.js`

 * *Files identical despite different names*

### Comparing `open-cravat-2.3.0/cravat/websubmit/nointernet.png` & `open-cravat-2.3.1/cravat/websubmit/nointernet.png`

 * *Files identical despite different names*

### Comparing `open-cravat-2.3.0/cravat/websubmit/pqselect.dev.customforsubmit.js` & `open-cravat-2.3.1/cravat/websubmit/pqselect.dev.customforsubmit.js`

 * *Files identical despite different names*

### Comparing `open-cravat-2.3.0/cravat/websubmit/question.png` & `open-cravat-2.3.1/cravat/websubmit/question.png`

 * *Files identical despite different names*

### Comparing `open-cravat-2.3.0/cravat/websubmit/refresh.png` & `open-cravat-2.3.1/cravat/websubmit/refresh.png`

 * *Files identical despite different names*

### Comparing `open-cravat-2.3.0/cravat/websubmit/websubmit.py` & `open-cravat-2.3.1/cravat/websubmit/websubmit.py`

 * *Files identical despite different names*

### Comparing `open-cravat-2.3.0/cravat/wincravat.pyw` & `open-cravat-2.3.1/cravat/wincravat.pyw`

 * *Files identical despite different names*

### Comparing `open-cravat-2.3.0/open_cravat.egg-info/PKG-INFO` & `open-cravat-2.3.1/open_cravat.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: open-cravat
-Version: 2.3.0
+Version: 2.3.1
 Summary: OpenCRAVAT - variant analysis toolkit
 Home-page: https://www.opencravat.org
 Author: RyangGuk Kim, Kyle Moad, Mike Ryan, and Rachel Karchin
 Author-email: support@opencravat.org
 Requires-Python: >=3.8
 License-File: LICENSE
```

### Comparing `open-cravat-2.3.0/open_cravat.egg-info/SOURCES.txt` & `open-cravat-2.3.1/open_cravat.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -280,8 +280,9 @@
 cravat/websubmit/nocache/websubmit.css
 cravat/websubmit/nocache/websubmit.js
 open_cravat.egg-info/PKG-INFO
 open_cravat.egg-info/SOURCES.txt
 open_cravat.egg-info/dependency_links.txt
 open_cravat.egg-info/entry_points.txt
 open_cravat.egg-info/requires.txt
-open_cravat.egg-info/top_level.txt
+open_cravat.egg-info/top_level.txt
+tests/test_admin_util.py
```

### Comparing `open-cravat-2.3.0/setup.py` & `open-cravat-2.3.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,15 +53,15 @@
 for root, dirs, files in os.walk(os.path.join('cravat', 'websubmit')):
     root_files = [os.path.join('..', root, f) for f in files]
     data_files.extend(root_files)
 
 setup(
     name='open-cravat',
     packages=['cravat'],
-    version='2.3.0',
+    version='2.3.1',
     description='OpenCRAVAT - variant analysis toolkit',
     long_description=readme(),
     author='RyangGuk Kim, Kyle Moad, Mike Ryan, and Rachel Karchin',
     author_email='support@opencravat.org',
     url='https://www.opencravat.org',
     license='',
     package_data={
```

