# Comparing `tmp/pybi-next-0.4.5.tar.gz` & `tmp/pybi-next-0.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybi-next-0.4.5.tar", last modified: Thu May 18 04:03:18 2023, max compression
+gzip compressed data, was "pybi-next-0.4.6.tar", last modified: Mon May 22 12:11:37 2023, max compression
```

## Comparing `pybi-next-0.4.5.tar` & `pybi-next-0.4.6.tar`

### file list

```diff
@@ -1,89 +1,89 @@
-drwxrwxrwx   0        0        0        0 2023-05-18 04:03:18.167691 pybi-next-0.4.5/
--rw-rw-rw-   0        0        0     1088 2022-03-21 14:09:44.000000 pybi-next-0.4.5/LICENSE
--rw-rw-rw-   0        0        0      477 2023-05-18 04:03:18.166674 pybi-next-0.4.5/PKG-INFO
--rw-rw-rw-   0        0        0     2112 2023-03-15 11:07:57.000000 pybi-next-0.4.5/README.md
-drwxrwxrwx   0        0        0        0 2023-05-18 04:03:18.012608 pybi-next-0.4.5/pybi/
--rw-rw-rw-   0        0        0     1686 2023-04-18 11:27:51.000000 pybi-next-0.4.5/pybi/__index.py
--rw-rw-rw-   0        0        0       49 2023-05-18 04:02:44.000000 pybi-next-0.4.5/pybi/__init__.py
--rw-rw-rw-   0        0        0    22181 2023-05-11 07:46:26.000000 pybi-next-0.4.5/pybi/app.py
-drwxrwxrwx   0        0        0        0 2023-05-18 04:03:18.023160 pybi-next-0.4.5/pybi/core/
--rw-rw-rw-   0        0        0       81 2023-03-15 11:07:57.000000 pybi-next-0.4.5/pybi/core/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-18 04:03:18.035154 pybi-next-0.4.5/pybi/core/components/
--rw-rw-rw-   0        0        0      630 2023-04-18 11:30:38.000000 pybi-next-0.4.5/pybi/core/components/__init__.py
--rw-rw-rw-   0        0        0     2675 2023-04-16 15:41:13.000000 pybi-next-0.4.5/pybi/core/components/component.py
--rw-rw-rw-   0        0        0      553 2023-04-16 15:41:13.000000 pybi-next-0.4.5/pybi/core/components/componentTag.py
--rw-rw-rw-   0        0        0    11672 2023-05-18 03:58:25.000000 pybi-next-0.4.5/pybi/core/components/containerComponent.py
--rw-rw-rw-   0        0        0      406 2023-03-29 16:16:41.000000 pybi-next-0.4.5/pybi/core/components/mermaid.py
-drwxrwxrwx   0        0        0        0 2023-05-18 04:03:18.056071 pybi-next-0.4.5/pybi/core/components/reactiveComponent/
--rw-rw-rw-   0        0        0      214 2023-03-30 06:02:37.000000 pybi-next-0.4.5/pybi/core/components/reactiveComponent/__init__.py
--rw-rw-rw-   0        0        0     1341 2023-03-15 11:07:57.000000 pybi-next-0.4.5/pybi/core/components/reactiveComponent/base.py
--rw-rw-rw-   0        0        0     5142 2023-04-11 10:54:25.000000 pybi-next-0.4.5/pybi/core/components/reactiveComponent/echarts.py
--rw-rw-rw-   0        0        0      695 2023-03-29 18:02:26.000000 pybi-next-0.4.5/pybi/core/components/reactiveComponent/input.py
--rw-rw-rw-   0        0        0      695 2023-03-15 11:07:57.000000 pybi-next-0.4.5/pybi/core/components/reactiveComponent/markdown.py
--rw-rw-rw-   0        0        0      644 2023-03-30 06:02:37.000000 pybi-next-0.4.5/pybi/core/components/reactiveComponent/numberSlider.py
--rw-rw-rw-   0        0        0      930 2023-03-15 11:07:57.000000 pybi-next-0.4.5/pybi/core/components/reactiveComponent/slicer.py
--rw-rw-rw-   0        0        0     1224 2023-03-15 11:07:57.000000 pybi-next-0.4.5/pybi/core/components/reactiveComponent/table.py
--rw-rw-rw-   0        0        0      428 2023-03-15 11:07:57.000000 pybi-next-0.4.5/pybi/core/components/reactiveComponent/textValue.py
--rw-rw-rw-   0        0        0     1882 2023-04-16 15:41:13.000000 pybi-next-0.4.5/pybi/core/components/staticComponent.py
--rw-rw-rw-   0        0        0     6135 2023-04-21 15:56:29.000000 pybi-next-0.4.5/pybi/core/dataSource.py
--rw-rw-rw-   0        0        0     5349 2023-04-11 10:54:25.000000 pybi-next-0.4.5/pybi/core/sql.py
-drwxrwxrwx   0        0        0        0 2023-05-18 04:03:18.064082 pybi-next-0.4.5/pybi/core/styles/
--rw-rw-rw-   0        0        0      714 2023-02-15 14:58:33.000000 pybi-next-0.4.5/pybi/core/styles/__init__.py
--rw-rw-rw-   0        0        0      535 2023-04-17 04:53:14.000000 pybi-next-0.4.5/pybi/core/styles/styleTag.py
--rw-rw-rw-   0        0        0     3552 2023-02-15 04:29:42.000000 pybi-next-0.4.5/pybi/core/styles/styles.py
-drwxrwxrwx   0        0        0        0 2023-05-18 04:03:18.074050 pybi-next-0.4.5/pybi/core/styles/tailwindStyles/
--rw-rw-rw-   0        0        0        0 2023-02-15 15:24:16.000000 pybi-next-0.4.5/pybi/core/styles/tailwindStyles/__init__.py
--rw-rw-rw-   0        0        0     1069 2023-02-15 14:58:33.000000 pybi-next-0.4.5/pybi/core/styles/tailwindStyles/boxShadow.py
--rw-rw-rw-   0        0        0      578 2023-02-15 14:58:33.000000 pybi-next-0.4.5/pybi/core/styles/tailwindStyles/textAlign.py
--rw-rw-rw-   0        0        0    21147 2023-02-15 14:58:33.000000 pybi-next-0.4.5/pybi/core/styles/tailwindStyles/textColor.py
--rw-rw-rw-   0        0        0     1458 2023-02-15 14:58:33.000000 pybi-next-0.4.5/pybi/core/styles/tailwindStyles/textSize.py
--rw-rw-rw-   0        0        0       95 2023-01-31 06:42:57.000000 pybi-next-0.4.5/pybi/core/styles/utils.py
--rw-rw-rw-   0        0        0     3602 2023-04-11 10:54:25.000000 pybi-next-0.4.5/pybi/core/uiResource.py
--rw-rw-rw-   0        0        0     1461 2023-04-11 10:54:25.000000 pybi-next-0.4.5/pybi/core/webResources.py
-drwxrwxrwx   0        0        0        0 2023-05-18 04:03:18.094262 pybi-next-0.4.5/pybi/easyEcharts/
--rw-rw-rw-   0        0        0     3756 2023-04-15 13:47:38.000000 pybi-next-0.4.5/pybi/easyEcharts/__init__.py
--rw-rw-rw-   0        0        0     3350 2023-04-13 15:22:20.000000 pybi-next-0.4.5/pybi/easyEcharts/bar.py
--rw-rw-rw-   0        0        0     3531 2023-05-11 08:03:21.000000 pybi-next-0.4.5/pybi/easyEcharts/base.py
--rw-rw-rw-   0        0        0     2686 2023-04-15 13:47:38.000000 pybi-next-0.4.5/pybi/easyEcharts/candlestick.py
--rw-rw-rw-   0        0        0     3462 2023-04-13 15:22:20.000000 pybi-next-0.4.5/pybi/easyEcharts/line.py
--rw-rw-rw-   0        0        0     1723 2023-04-11 10:54:25.000000 pybi-next-0.4.5/pybi/easyEcharts/map.py
--rw-rw-rw-   0        0        0     2468 2023-04-11 11:04:47.000000 pybi-next-0.4.5/pybi/easyEcharts/pie.py
--rw-rw-rw-   0        0        0     2766 2023-04-15 13:47:38.000000 pybi-next-0.4.5/pybi/easyEcharts/radar.py
--rw-rw-rw-   0        0        0     1965 2023-04-11 11:04:51.000000 pybi-next-0.4.5/pybi/easyEcharts/scatter.py
--rw-rw-rw-   0        0        0     2598 2023-04-11 11:03:46.000000 pybi-next-0.4.5/pybi/easyEcharts/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-18 04:03:18.099249 pybi-next-0.4.5/pybi/icons/
--rw-rw-rw-   0        0        0        0 2023-04-11 10:54:25.000000 pybi-next-0.4.5/pybi/icons/__init__.py
--rw-rw-rw-   0        0        0      700 2023-04-11 10:54:25.000000 pybi-next-0.4.5/pybi/icons/iconManager.py
--rw-rw-rw-   0        0        0   923783 2023-04-11 10:54:25.000000 pybi-next-0.4.5/pybi/icons/material_icons.py
-drwxrwxrwx   0        0        0        0 2023-05-18 04:03:18.133767 pybi-next-0.4.5/pybi/static/
--rw-rw-rw-   0        0        0  1022898 2023-03-14 04:09:02.000000 pybi-next-0.4.5/pybi/static/echarts.min.js
--rw-rw-rw-   0        0        0      464 2023-05-16 11:55:50.000000 pybi-next-0.4.5/pybi/static/echartsCps-style.css
--rw-rw-rw-   0        0        0    27689 2023-05-16 11:55:50.000000 pybi-next-0.4.5/pybi/static/echartsCps.iife.js
--rw-rw-rw-   0        0        0   119843 2023-05-16 11:55:50.000000 pybi-next-0.4.5/pybi/static/elementCps-style.css
--rw-rw-rw-   0        0        0   349594 2023-05-16 11:55:50.000000 pybi-next-0.4.5/pybi/static/elementCps.iife.js
--rw-rw-rw-   0        0        0  2778175 2023-05-16 11:55:50.000000 pybi-next-0.4.5/pybi/static/mermaidCps.iife.js
--rw-rw-rw-   0        0        0   582522 2023-04-06 17:22:15.000000 pybi-next-0.4.5/pybi/static/province_map_full.json
--rw-rw-rw-   0        0        0     2419 2023-05-16 11:55:50.000000 pybi-next-0.4.5/pybi/static/sysApp-style.css
--rw-rw-rw-   0        0        0  1012609 2023-05-16 11:55:50.000000 pybi-next-0.4.5/pybi/static/sysApp.iife.js
--rw-rw-rw-   0        0        0   125849 2023-03-23 06:49:54.000000 pybi-next-0.4.5/pybi/static/vue.global.prod.min.js
-drwxrwxrwx   0        0        0        0 2023-05-18 04:03:18.135757 pybi-next-0.4.5/pybi/template/
--rw-rw-rw-   0        0        0     1535 2023-04-11 10:54:25.000000 pybi-next-0.4.5/pybi/template/index.html
-drwxrwxrwx   0        0        0        0 2023-05-18 04:03:18.152688 pybi-next-0.4.5/pybi/utils/
--rw-rw-rw-   0        0        0        0 2022-05-17 15:58:12.000000 pybi-next-0.4.5/pybi/utils/__init__.py
--rw-rw-rw-   0        0        0     1545 2023-02-16 03:08:31.000000 pybi-next-0.4.5/pybi/utils/dataSourceUtils.py
--rw-rw-rw-   0        0        0     3056 2023-03-29 14:36:39.000000 pybi-next-0.4.5/pybi/utils/data_gen.py
--rw-rw-rw-   0        0        0     1624 2023-02-11 14:46:57.000000 pybi-next-0.4.5/pybi/utils/dictUtils.py
--rw-rw-rw-   0        0        0     1931 2023-03-18 09:54:06.000000 pybi-next-0.4.5/pybi/utils/echarts_opts_utils.py
--rw-rw-rw-   0        0        0      851 2022-05-17 15:58:12.000000 pybi-next-0.4.5/pybi/utils/helper.py
--rw-rw-rw-   0        0        0   116803 2022-05-17 15:58:12.000000 pybi-next-0.4.5/pybi/utils/markdown2.py
--rw-rw-rw-   0        0        0     2883 2023-03-15 11:07:57.000000 pybi-next-0.4.5/pybi/utils/pyecharts_utils.py
--rw-rw-rw-   0        0        0     1398 2023-03-15 11:07:57.000000 pybi-next-0.4.5/pybi/utils/sql.py
-drwxrwxrwx   0        0        0        0 2023-05-18 04:03:18.164656 pybi-next-0.4.5/pybi_next.egg-info/
--rw-rw-rw-   0        0        0      477 2023-05-18 04:03:17.000000 pybi-next-0.4.5/pybi_next.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2288 2023-05-18 04:03:17.000000 pybi-next-0.4.5/pybi_next.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-18 04:03:17.000000 pybi-next-0.4.5/pybi_next.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-02-15 04:57:05.000000 pybi-next-0.4.5/pybi_next.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       25 2023-05-18 04:03:17.000000 pybi-next-0.4.5/pybi_next.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-05-18 04:03:17.000000 pybi-next-0.4.5/pybi_next.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-18 04:03:18.167691 pybi-next-0.4.5/setup.cfg
--rw-rw-rw-   0        0        0     1590 2023-03-29 14:36:39.000000 pybi-next-0.4.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-22 12:11:37.785869 pybi-next-0.4.6/
+-rw-rw-rw-   0        0        0     1088 2022-03-21 14:09:44.000000 pybi-next-0.4.6/LICENSE
+-rw-rw-rw-   0        0        0      477 2023-05-22 12:11:37.784908 pybi-next-0.4.6/PKG-INFO
+-rw-rw-rw-   0        0        0     2112 2023-03-15 11:07:57.000000 pybi-next-0.4.6/README.md
+drwxrwxrwx   0        0        0        0 2023-05-22 12:11:37.514984 pybi-next-0.4.6/pybi/
+-rw-rw-rw-   0        0        0     1686 2023-04-18 11:27:51.000000 pybi-next-0.4.6/pybi/__index.py
+-rw-rw-rw-   0        0        0       49 2023-05-22 12:07:58.000000 pybi-next-0.4.6/pybi/__init__.py
+-rw-rw-rw-   0        0        0    22181 2023-05-11 07:46:26.000000 pybi-next-0.4.6/pybi/app.py
+drwxrwxrwx   0        0        0        0 2023-05-22 12:11:37.526692 pybi-next-0.4.6/pybi/core/
+-rw-rw-rw-   0        0        0       81 2023-03-15 11:07:57.000000 pybi-next-0.4.6/pybi/core/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-22 12:11:37.554121 pybi-next-0.4.6/pybi/core/components/
+-rw-rw-rw-   0        0        0      630 2023-04-18 11:30:38.000000 pybi-next-0.4.6/pybi/core/components/__init__.py
+-rw-rw-rw-   0        0        0     2675 2023-04-16 15:41:13.000000 pybi-next-0.4.6/pybi/core/components/component.py
+-rw-rw-rw-   0        0        0      553 2023-04-16 15:41:13.000000 pybi-next-0.4.6/pybi/core/components/componentTag.py
+-rw-rw-rw-   0        0        0    11672 2023-05-18 03:58:25.000000 pybi-next-0.4.6/pybi/core/components/containerComponent.py
+-rw-rw-rw-   0        0        0      406 2023-03-29 16:16:41.000000 pybi-next-0.4.6/pybi/core/components/mermaid.py
+drwxrwxrwx   0        0        0        0 2023-05-22 12:11:37.609831 pybi-next-0.4.6/pybi/core/components/reactiveComponent/
+-rw-rw-rw-   0        0        0      214 2023-03-30 06:02:37.000000 pybi-next-0.4.6/pybi/core/components/reactiveComponent/__init__.py
+-rw-rw-rw-   0        0        0     1341 2023-03-15 11:07:57.000000 pybi-next-0.4.6/pybi/core/components/reactiveComponent/base.py
+-rw-rw-rw-   0        0        0     5142 2023-04-11 10:54:25.000000 pybi-next-0.4.6/pybi/core/components/reactiveComponent/echarts.py
+-rw-rw-rw-   0        0        0      695 2023-03-29 18:02:26.000000 pybi-next-0.4.6/pybi/core/components/reactiveComponent/input.py
+-rw-rw-rw-   0        0        0      695 2023-03-15 11:07:57.000000 pybi-next-0.4.6/pybi/core/components/reactiveComponent/markdown.py
+-rw-rw-rw-   0        0        0      644 2023-03-30 06:02:37.000000 pybi-next-0.4.6/pybi/core/components/reactiveComponent/numberSlider.py
+-rw-rw-rw-   0        0        0      930 2023-03-15 11:07:57.000000 pybi-next-0.4.6/pybi/core/components/reactiveComponent/slicer.py
+-rw-rw-rw-   0        0        0     1224 2023-03-15 11:07:57.000000 pybi-next-0.4.6/pybi/core/components/reactiveComponent/table.py
+-rw-rw-rw-   0        0        0      428 2023-03-15 11:07:57.000000 pybi-next-0.4.6/pybi/core/components/reactiveComponent/textValue.py
+-rw-rw-rw-   0        0        0     1882 2023-04-16 15:41:13.000000 pybi-next-0.4.6/pybi/core/components/staticComponent.py
+-rw-rw-rw-   0        0        0     6135 2023-04-21 15:56:29.000000 pybi-next-0.4.6/pybi/core/dataSource.py
+-rw-rw-rw-   0        0        0     5349 2023-04-11 10:54:25.000000 pybi-next-0.4.6/pybi/core/sql.py
+drwxrwxrwx   0        0        0        0 2023-05-22 12:11:37.625788 pybi-next-0.4.6/pybi/core/styles/
+-rw-rw-rw-   0        0        0      714 2023-02-15 14:58:33.000000 pybi-next-0.4.6/pybi/core/styles/__init__.py
+-rw-rw-rw-   0        0        0      535 2023-04-17 04:53:14.000000 pybi-next-0.4.6/pybi/core/styles/styleTag.py
+-rw-rw-rw-   0        0        0     3552 2023-02-15 04:29:42.000000 pybi-next-0.4.6/pybi/core/styles/styles.py
+drwxrwxrwx   0        0        0        0 2023-05-22 12:11:37.639751 pybi-next-0.4.6/pybi/core/styles/tailwindStyles/
+-rw-rw-rw-   0        0        0        0 2023-02-15 15:24:16.000000 pybi-next-0.4.6/pybi/core/styles/tailwindStyles/__init__.py
+-rw-rw-rw-   0        0        0     1069 2023-02-15 14:58:33.000000 pybi-next-0.4.6/pybi/core/styles/tailwindStyles/boxShadow.py
+-rw-rw-rw-   0        0        0      578 2023-02-15 14:58:33.000000 pybi-next-0.4.6/pybi/core/styles/tailwindStyles/textAlign.py
+-rw-rw-rw-   0        0        0    21147 2023-02-15 14:58:33.000000 pybi-next-0.4.6/pybi/core/styles/tailwindStyles/textColor.py
+-rw-rw-rw-   0        0        0     1458 2023-02-15 14:58:33.000000 pybi-next-0.4.6/pybi/core/styles/tailwindStyles/textSize.py
+-rw-rw-rw-   0        0        0       95 2023-01-31 06:42:57.000000 pybi-next-0.4.6/pybi/core/styles/utils.py
+-rw-rw-rw-   0        0        0     3602 2023-04-11 10:54:25.000000 pybi-next-0.4.6/pybi/core/uiResource.py
+-rw-rw-rw-   0        0        0     1461 2023-04-11 10:54:25.000000 pybi-next-0.4.6/pybi/core/webResources.py
+drwxrwxrwx   0        0        0        0 2023-05-22 12:11:37.659697 pybi-next-0.4.6/pybi/easyEcharts/
+-rw-rw-rw-   0        0        0     3756 2023-04-15 13:47:38.000000 pybi-next-0.4.6/pybi/easyEcharts/__init__.py
+-rw-rw-rw-   0        0        0     3300 2023-05-22 12:03:15.000000 pybi-next-0.4.6/pybi/easyEcharts/bar.py
+-rw-rw-rw-   0        0        0     3689 2023-05-22 12:03:15.000000 pybi-next-0.4.6/pybi/easyEcharts/base.py
+-rw-rw-rw-   0        0        0     2636 2023-05-22 12:03:15.000000 pybi-next-0.4.6/pybi/easyEcharts/candlestick.py
+-rw-rw-rw-   0        0        0     3415 2023-05-22 12:03:15.000000 pybi-next-0.4.6/pybi/easyEcharts/line.py
+-rw-rw-rw-   0        0        0     1678 2023-05-22 12:03:15.000000 pybi-next-0.4.6/pybi/easyEcharts/map.py
+-rw-rw-rw-   0        0        0     2423 2023-05-22 12:03:15.000000 pybi-next-0.4.6/pybi/easyEcharts/pie.py
+-rw-rw-rw-   0        0        0     2716 2023-05-22 12:03:15.000000 pybi-next-0.4.6/pybi/easyEcharts/radar.py
+-rw-rw-rw-   0        0        0     1920 2023-05-22 12:03:15.000000 pybi-next-0.4.6/pybi/easyEcharts/scatter.py
+-rw-rw-rw-   0        0        0     2598 2023-04-11 11:03:46.000000 pybi-next-0.4.6/pybi/easyEcharts/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-22 12:11:37.665684 pybi-next-0.4.6/pybi/icons/
+-rw-rw-rw-   0        0        0        0 2023-04-11 10:54:25.000000 pybi-next-0.4.6/pybi/icons/__init__.py
+-rw-rw-rw-   0        0        0      700 2023-04-11 10:54:25.000000 pybi-next-0.4.6/pybi/icons/iconManager.py
+-rw-rw-rw-   0        0        0   923783 2023-04-11 10:54:25.000000 pybi-next-0.4.6/pybi/icons/material_icons.py
+drwxrwxrwx   0        0        0        0 2023-05-22 12:11:37.734006 pybi-next-0.4.6/pybi/static/
+-rw-rw-rw-   0        0        0  1022898 2023-03-14 04:09:02.000000 pybi-next-0.4.6/pybi/static/echarts.min.js
+-rw-rw-rw-   0        0        0      464 2023-05-16 11:55:50.000000 pybi-next-0.4.6/pybi/static/echartsCps-style.css
+-rw-rw-rw-   0        0        0    27689 2023-05-16 11:55:50.000000 pybi-next-0.4.6/pybi/static/echartsCps.iife.js
+-rw-rw-rw-   0        0        0   119843 2023-05-16 11:55:50.000000 pybi-next-0.4.6/pybi/static/elementCps-style.css
+-rw-rw-rw-   0        0        0   349594 2023-05-16 11:55:50.000000 pybi-next-0.4.6/pybi/static/elementCps.iife.js
+-rw-rw-rw-   0        0        0  2778175 2023-05-16 11:55:50.000000 pybi-next-0.4.6/pybi/static/mermaidCps.iife.js
+-rw-rw-rw-   0        0        0   582522 2023-04-06 17:22:15.000000 pybi-next-0.4.6/pybi/static/province_map_full.json
+-rw-rw-rw-   0        0        0     2419 2023-05-16 11:55:50.000000 pybi-next-0.4.6/pybi/static/sysApp-style.css
+-rw-rw-rw-   0        0        0  1012609 2023-05-16 11:55:50.000000 pybi-next-0.4.6/pybi/static/sysApp.iife.js
+-rw-rw-rw-   0        0        0   125849 2023-03-23 06:49:54.000000 pybi-next-0.4.6/pybi/static/vue.global.prod.min.js
+drwxrwxrwx   0        0        0        0 2023-05-22 12:11:37.736998 pybi-next-0.4.6/pybi/template/
+-rw-rw-rw-   0        0        0     1535 2023-04-11 10:54:25.000000 pybi-next-0.4.6/pybi/template/index.html
+drwxrwxrwx   0        0        0        0 2023-05-22 12:11:37.752956 pybi-next-0.4.6/pybi/utils/
+-rw-rw-rw-   0        0        0        0 2022-05-17 15:58:12.000000 pybi-next-0.4.6/pybi/utils/__init__.py
+-rw-rw-rw-   0        0        0     1545 2023-02-16 03:08:31.000000 pybi-next-0.4.6/pybi/utils/dataSourceUtils.py
+-rw-rw-rw-   0        0        0     3056 2023-03-29 14:36:39.000000 pybi-next-0.4.6/pybi/utils/data_gen.py
+-rw-rw-rw-   0        0        0     1624 2023-02-11 14:46:57.000000 pybi-next-0.4.6/pybi/utils/dictUtils.py
+-rw-rw-rw-   0        0        0     1931 2023-03-18 09:54:06.000000 pybi-next-0.4.6/pybi/utils/echarts_opts_utils.py
+-rw-rw-rw-   0        0        0      851 2022-05-17 15:58:12.000000 pybi-next-0.4.6/pybi/utils/helper.py
+-rw-rw-rw-   0        0        0   116803 2022-05-17 15:58:12.000000 pybi-next-0.4.6/pybi/utils/markdown2.py
+-rw-rw-rw-   0        0        0     2883 2023-03-15 11:07:57.000000 pybi-next-0.4.6/pybi/utils/pyecharts_utils.py
+-rw-rw-rw-   0        0        0     1398 2023-03-15 11:07:57.000000 pybi-next-0.4.6/pybi/utils/sql.py
+drwxrwxrwx   0        0        0        0 2023-05-22 12:11:37.782876 pybi-next-0.4.6/pybi_next.egg-info/
+-rw-rw-rw-   0        0        0      477 2023-05-22 12:11:36.000000 pybi-next-0.4.6/pybi_next.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2288 2023-05-22 12:11:36.000000 pybi-next-0.4.6/pybi_next.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-22 12:11:36.000000 pybi-next-0.4.6/pybi_next.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-02-15 04:57:05.000000 pybi-next-0.4.6/pybi_next.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       25 2023-05-22 12:11:36.000000 pybi-next-0.4.6/pybi_next.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-05-22 12:11:36.000000 pybi-next-0.4.6/pybi_next.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-22 12:11:37.786866 pybi-next-0.4.6/setup.cfg
+-rw-rw-rw-   0        0        0     1590 2023-03-29 14:36:39.000000 pybi-next-0.4.6/setup.py
```

### Comparing `pybi-next-0.4.5/LICENSE` & `pybi-next-0.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pybi-next-0.4.5/README.md` & `pybi-next-0.4.6/README.md`

 * *Files identical despite different names*

### Comparing `pybi-next-0.4.5/pybi/__index.py` & `pybi-next-0.4.6/pybi/__index.py`

 * *Files identical despite different names*

### Comparing `pybi-next-0.4.5/pybi/app.py` & `pybi-next-0.4.6/pybi/app.py`

 * *Files identical despite different names*

### Comparing `pybi-next-0.4.5/pybi/core/components/__init__.py` & `pybi-next-0.4.6/pybi/core/components/__init__.py`

 * *Files identical despite different names*

### Comparing `pybi-next-0.4.5/pybi/core/components/component.py` & `pybi-next-0.4.6/pybi/core/components/component.py`

 * *Files identical despite different names*

### Comparing `pybi-next-0.4.5/pybi/core/components/componentTag.py` & `pybi-next-0.4.6/pybi/core/components/componentTag.py`

 * *Files identical despite different names*

### Comparing `pybi-next-0.4.5/pybi/core/components/containerComponent.py` & `pybi-next-0.4.6/pybi/core/components/containerComponent.py`

 * *Files identical despite different names*

### Comparing `pybi-next-0.4.5/pybi/core/components/reactiveComponent/base.py` & `pybi-next-0.4.6/pybi/core/components/reactiveComponent/base.py`

 * *Files identical despite different names*

### Comparing `pybi-next-0.4.5/pybi/core/components/reactiveComponent/echarts.py` & `pybi-next-0.4.6/pybi/core/components/reactiveComponent/echarts.py`

 * *Files identical despite different names*

### Comparing `pybi-next-0.4.5/pybi/core/components/reactiveComponent/input.py` & `pybi-next-0.4.6/pybi/core/components/reactiveComponent/input.py`

 * *Files identical despite different names*

### Comparing `pybi-next-0.4.5/pybi/core/components/reactiveComponent/markdown.py` & `pybi-next-0.4.6/pybi/core/components/reactiveComponent/markdown.py`

 * *Files identical despite different names*

### Comparing `pybi-next-0.4.5/pybi/core/components/reactiveComponent/numberSlider.py` & `pybi-next-0.4.6/pybi/core/components/reactiveComponent/numberSlider.py`

 * *Files identical despite different names*

### Comparing `pybi-next-0.4.5/pybi/core/components/reactiveComponent/slicer.py` & `pybi-next-0.4.6/pybi/core/components/reactiveComponent/slicer.py`

 * *Files identical despite different names*

### Comparing `pybi-next-0.4.5/pybi/core/components/reactiveComponent/table.py` & `pybi-next-0.4.6/pybi/core/components/reactiveComponent/table.py`

 * *Files identical despite different names*

### Comparing `pybi-next-0.4.5/pybi/core/components/staticComponent.py` & `pybi-next-0.4.6/pybi/core/components/staticComponent.py`

 * *Files identical despite different names*

### Comparing `pybi-next-0.4.5/pybi/core/dataSource.py` & `pybi-next-0.4.6/pybi/core/dataSource.py`

 * *Files identical despite different names*

### Comparing `pybi-next-0.4.5/pybi/core/sql.py` & `pybi-next-0.4.6/pybi/core/sql.py`

 * *Files identical despite different names*

### Comparing `pybi-next-0.4.5/pybi/core/styles/__init__.py` & `pybi-next-0.4.6/pybi/core/styles/__init__.py`

 * *Files identical despite different names*

### Comparing `pybi-next-0.4.5/pybi/core/styles/styleTag.py` & `pybi-next-0.4.6/pybi/core/styles/styleTag.py`

 * *Files identical despite different names*

### Comparing `pybi-next-0.4.5/pybi/core/styles/styles.py` & `pybi-next-0.4.6/pybi/core/styles/styles.py`

 * *Files identical despite different names*

### Comparing `pybi-next-0.4.5/pybi/core/styles/tailwindStyles/boxShadow.py` & `pybi-next-0.4.6/pybi/core/styles/tailwindStyles/boxShadow.py`

 * *Files identical despite different names*

### Comparing `pybi-next-0.4.5/pybi/core/styles/tailwindStyles/textAlign.py` & `pybi-next-0.4.6/pybi/core/styles/tailwindStyles/textAlign.py`

 * *Files identical despite different names*

### Comparing `pybi-next-0.4.5/pybi/core/styles/tailwindStyles/textColor.py` & `pybi-next-0.4.6/pybi/core/styles/tailwindStyles/textColor.py`

 * *Files identical despite different names*

### Comparing `pybi-next-0.4.5/pybi/core/styles/tailwindStyles/textSize.py` & `pybi-next-0.4.6/pybi/core/styles/tailwindStyles/textSize.py`

 * *Files identical despite different names*

### Comparing `pybi-next-0.4.5/pybi/core/uiResource.py` & `pybi-next-0.4.6/pybi/core/uiResource.py`

 * *Files identical despite different names*

### Comparing `pybi-next-0.4.5/pybi/core/webResources.py` & `pybi-next-0.4.6/pybi/core/webResources.py`

 * *Files identical despite different names*

### Comparing `pybi-next-0.4.5/pybi/easyEcharts/__init__.py` & `pybi-next-0.4.6/pybi/easyEcharts/__init__.py`

 * *Files identical despite different names*

### Comparing `pybi-next-0.4.5/pybi/easyEcharts/bar.py` & `pybi-next-0.4.6/pybi/easyEcharts/bar.py`

 * *Files 4% similar despite different names*

```diff
@@ -39,15 +39,15 @@
     def _create_default_click_filter(self):
         valueType, field = "x", self.x
         if self._reverse_axis:
             valueType, field = "y", self.y
 
         self.click_filter(valueType, self.data, self.x)
 
-    def get_options_infos(self):
+    def _create_options_ex(self):
         opts = super().get_options()
 
         base_opt = {
             "xAxis": [
                 {
                     "type": "",
                     # "data": [],
@@ -101,10 +101,8 @@
 
         catAxis["data"] = pbi.sql(
             f"select distinct {self.x} from {dv} order by {self.order}"
         ).toflatlist()
         catAxis["type"] = "category"
         valueAxis["type"] = "value"
 
-        base_opt = self._post_options(base_opt)
-
         return base_opt, self._updateInfos, []
```

### Comparing `pybi-next-0.4.5/pybi/easyEcharts/base.py` & `pybi-next-0.4.6/pybi/easyEcharts/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,37 +11,36 @@
 if TYPE_CHECKING:
     pass
 
 
 class BaseChart:
     def __init__(self) -> None:
         self.__base_opt = {
-            "legend": {},
+            "legend": [{}],
             "series": [],
-            "title": {},
-            "grid": {"containLabel": True},
-            "tooltip": {},
+            "title": [{}],
+            "grid": [{"containLabel": True}],
+            "tooltip": [{}],
         }
         self._merge_opt = {}
         self._updateInfos: List[EChartUpdateInfo] = []
         self._prop_by_paths: List[Tuple[str, Any]] = []
 
     def __add__(self, other: BaseChart):
         return ChartCollector().append(self).append(other)
 
     def merge(self, options: Dict):
-        self._merge_opt = options
+        self._merge_opt.update(options)
         return self
 
     def get_options(self):
         return copy.deepcopy(self.__base_opt)
 
     def set_title(self, text: str):
-        opt_title: Dict = self.__base_opt["title"]
-        opt_title["text"] = text
+        self.merge({"title": {"text": text}})
 
         return self
 
     def hover_filter(
         self, value_type: str, table: Union[str, DataSourceTable], field: str
     ):
         """
@@ -83,18 +82,23 @@
 
     def remove_all_click_filter(self):
         return self._remove_filters("click")
 
     def _create_default_click_filter(self):
         pass
 
+    def _create_options_ex(self):
+        raise NotImplementedError
+
     def get_options_infos(
         self,
     ) -> Tuple[Dict, List[EChartUpdateInfo], List[str]]:
-        raise NotImplementedError
+        opts, updateInfos, mapIds = self._create_options_ex()
+        opts = self._post_options(opts)
+        return opts, updateInfos, mapIds
 
     def set_prop_by_path(self, path: str, value):
         """
         >>> .set_prop_by_path('xAxis[0].axisLabel.interval',1)
         """
         self._prop_by_paths.append((path, value))
         return self
```

### Comparing `pybi-next-0.4.5/pybi/easyEcharts/candlestick.py` & `pybi-next-0.4.6/pybi/easyEcharts/candlestick.py`

 * *Files 12% similar despite different names*

```diff
@@ -31,15 +31,15 @@
         self.open = open
         self.highest = highest
         self._series_configs = {}
 
     def _create_default_click_filter(self):
         pass
 
-    def get_options_infos(self):
+    def _create_options_ex(self):
         opts = super().get_options()
 
         base_opt = {
             "xAxis": [{}],
             "yAxis": [{}],
             "series": [],
             "dataZoom": [
@@ -77,10 +77,8 @@
             }
         )
 
         base_opt["xAxis"][0]["data"] = pbi.sql(
             f"select distinct {self.date} from {self.data} order by {self.date}"
         ).toflatlist()
 
-        base_opt = self._post_options(base_opt)
-
         return base_opt, self._updateInfos, []
```

### Comparing `pybi-next-0.4.5/pybi/easyEcharts/line.py` & `pybi-next-0.4.6/pybi/easyEcharts/line.py`

 * *Files 5% similar despite different names*

```diff
@@ -43,15 +43,15 @@
     def _create_default_click_filter(self):
         self.click_filter("x", self.data, self.x)
 
     def set_xAxis(self, value):
         self._xAxis = value
         return self
 
-    def get_options_infos(self):
+    def _create_options_ex(self):
         opts = super().get_options()
 
         base_opt = {
             "xAxis": [
                 {
                     "type": "",
                     "data": [],
@@ -105,10 +105,8 @@
         valueAxis["type"] = "value"
 
         opts["tooltip"] = {
             "trigger": "axis",
             "axisPointer": {"type": "cross", "label": {"backgroundColor": "#6a7985"}},
         }
 
-        self._update_props_by_path(base_opt)
-
         return base_opt, self._updateInfos, []
```

### Comparing `pybi-next-0.4.5/pybi/easyEcharts/map.py` & `pybi-next-0.4.6/pybi/easyEcharts/map.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     def __init__(self, map_name: str):
         super().__init__()
         self.map_name = map_name
 
     def _create_default_click_filter(self):
         pass
 
-    def get_options_infos(self):
+    def _create_options_ex(self):
         opts = super().get_options()
 
         geo = {
             "map": self.map_name,
             "roam": True,
             "label": {"show": True, "position": "top"},
             "itemStyle": {
@@ -51,9 +51,8 @@
             "geoIndex": 0,
         }
 
         base_opt["series"].append(series_config)
 
         # opts["tooltip"] = {"trigger": "item"}
 
-        self._update_props_by_path(base_opt)
         return base_opt, self._updateInfos, [self.map_name]
```

### Comparing `pybi-next-0.4.5/pybi/easyEcharts/pie.py` & `pybi-next-0.4.6/pybi/easyEcharts/pie.py`

 * *Files 5% similar despite different names*

```diff
@@ -38,15 +38,15 @@
         }
 
         return self
 
     def _create_default_click_filter(self):
         self.click_filter("name", self.data, self.name)
 
-    def get_options_infos(self):
+    def _create_options_ex(self):
         opts = super().get_options()
 
         base_opt = {
             "xAxis": None,
             "yAxis": None,
             "series": [],
         }
@@ -74,9 +74,8 @@
 
         series_config["data"] = sql
 
         base_opt["series"].append(series_config)
 
         opts["tooltip"] = {"trigger": "item"}
 
-        self._update_props_by_path(base_opt)
         return base_opt, self._updateInfos, []
```

### Comparing `pybi-next-0.4.5/pybi/easyEcharts/radar.py` & `pybi-next-0.4.6/pybi/easyEcharts/radar.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,15 +28,15 @@
         self.name = name
         self.agg = agg
         self._series_configs = {}
 
     def _create_default_click_filter(self):
         pass
 
-    def get_options_infos(self):
+    def _create_options_ex(self):
         opts = super().get_options()
 
         agg_field = f"{sqlUtils.apply_agg(self.agg, self.value)} as value"
 
         dv_summary = pbi.set_dataView(
             f"select {self.name} as name,{self.indicator} as indicator,{agg_field} from {self.data} group by {self.name},{self.indicator}"
         )
@@ -90,10 +90,8 @@
                 "type": "radar",
                 "data": data_query,
                 # "universalTransition": {"enabled": True, "divideShape": "clone"},
                 "areaStyle": {"opacity": 0.1},
             }
         )
 
-        base_opt = self._post_options(base_opt)
-
         return base_opt, self._updateInfos, []
```

### Comparing `pybi-next-0.4.5/pybi/easyEcharts/scatter.py` & `pybi-next-0.4.6/pybi/easyEcharts/scatter.py`

 * *Files 18% similar despite different names*

```diff
@@ -28,15 +28,15 @@
         self.agg = agg
         self._series_configs = {}
 
     def _create_default_click_filter(self):
         # TODO:
         self.click_filter("x", self.data, self.x)
 
-    def get_options_infos(self):
+    def _create_options_ex(self):
         opts = super().get_options()
 
         base_opt = {
             "xAxis": {},
             "yAxis": {},
             "series": [],
         }
@@ -61,9 +61,8 @@
         else:
             sql = pbi.sql(f"select {self.x},{self.y} from {self.data}").toflatlist()
             series = {"type": "scatter", "symbolSize": 15, "data": sql}
             base_opt["series"].append(series)
 
         opts["tooltip"] = {"trigger": "item"}
 
-        self._update_props_by_path(base_opt)
         return base_opt, self._updateInfos, []
```

### Comparing `pybi-next-0.4.5/pybi/easyEcharts/utils.py` & `pybi-next-0.4.6/pybi/easyEcharts/utils.py`

 * *Files identical despite different names*

### Comparing `pybi-next-0.4.5/pybi/icons/iconManager.py` & `pybi-next-0.4.6/pybi/icons/iconManager.py`

 * *Files identical despite different names*

### Comparing `pybi-next-0.4.5/pybi/icons/material_icons.py` & `pybi-next-0.4.6/pybi/icons/material_icons.py`

 * *Files identical despite different names*

### Comparing `pybi-next-0.4.5/pybi/static/echarts.min.js` & `pybi-next-0.4.6/pybi/static/echarts.min.js`

 * *Files identical despite different names*

### Comparing `pybi-next-0.4.5/pybi/static/echartsCps.iife.js` & `pybi-next-0.4.6/pybi/static/echartsCps.iife.js`

 * *Files identical despite different names*

### Comparing `pybi-next-0.4.5/pybi/static/elementCps-style.css` & `pybi-next-0.4.6/pybi/static/elementCps-style.css`

 * *Files identical despite different names*

### Comparing `pybi-next-0.4.5/pybi/static/elementCps.iife.js` & `pybi-next-0.4.6/pybi/static/elementCps.iife.js`

 * *Files identical despite different names*

### Comparing `pybi-next-0.4.5/pybi/static/mermaidCps.iife.js` & `pybi-next-0.4.6/pybi/static/mermaidCps.iife.js`

 * *Files identical despite different names*

### Comparing `pybi-next-0.4.5/pybi/static/province_map_full.json` & `pybi-next-0.4.6/pybi/static/province_map_full.json`

 * *Files identical despite different names*

### Comparing `pybi-next-0.4.5/pybi/static/sysApp-style.css` & `pybi-next-0.4.6/pybi/static/sysApp-style.css`

 * *Files identical despite different names*

### Comparing `pybi-next-0.4.5/pybi/static/sysApp.iife.js` & `pybi-next-0.4.6/pybi/static/sysApp.iife.js`

 * *Files identical despite different names*

### Comparing `pybi-next-0.4.5/pybi/static/vue.global.prod.min.js` & `pybi-next-0.4.6/pybi/static/vue.global.prod.min.js`

 * *Files identical despite different names*

### Comparing `pybi-next-0.4.5/pybi/template/index.html` & `pybi-next-0.4.6/pybi/template/index.html`

 * *Files identical despite different names*

### Comparing `pybi-next-0.4.5/pybi/utils/dataSourceUtils.py` & `pybi-next-0.4.6/pybi/utils/dataSourceUtils.py`

 * *Files identical despite different names*

### Comparing `pybi-next-0.4.5/pybi/utils/data_gen.py` & `pybi-next-0.4.6/pybi/utils/data_gen.py`

 * *Files identical despite different names*

### Comparing `pybi-next-0.4.5/pybi/utils/dictUtils.py` & `pybi-next-0.4.6/pybi/utils/dictUtils.py`

 * *Files identical despite different names*

### Comparing `pybi-next-0.4.5/pybi/utils/echarts_opts_utils.py` & `pybi-next-0.4.6/pybi/utils/echarts_opts_utils.py`

 * *Files identical despite different names*

### Comparing `pybi-next-0.4.5/pybi/utils/helper.py` & `pybi-next-0.4.6/pybi/utils/helper.py`

 * *Files identical despite different names*

### Comparing `pybi-next-0.4.5/pybi/utils/markdown2.py` & `pybi-next-0.4.6/pybi/utils/markdown2.py`

 * *Files identical despite different names*

### Comparing `pybi-next-0.4.5/pybi/utils/pyecharts_utils.py` & `pybi-next-0.4.6/pybi/utils/pyecharts_utils.py`

 * *Files identical despite different names*

### Comparing `pybi-next-0.4.5/pybi/utils/sql.py` & `pybi-next-0.4.6/pybi/utils/sql.py`

 * *Files identical despite different names*

### Comparing `pybi-next-0.4.5/pybi_next.egg-info/SOURCES.txt` & `pybi-next-0.4.6/pybi_next.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pybi-next-0.4.5/setup.py` & `pybi-next-0.4.6/setup.py`

 * *Files identical despite different names*

