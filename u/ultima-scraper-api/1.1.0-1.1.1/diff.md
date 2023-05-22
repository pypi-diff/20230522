# Comparing `tmp/ultima_scraper_api-1.1.0.tar.gz` & `tmp/ultima_scraper_api-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ultima_scraper_api-1.1.0.tar", max compression
+gzip compressed data, was "ultima_scraper_api-1.1.1.tar", max compression
```

## Comparing `ultima_scraper_api-1.1.0.tar` & `ultima_scraper_api-1.1.1.tar`

### file list

```diff
@@ -1,59 +1,59 @@
--rw-r--r--   0        0        0     1193 2023-05-14 20:18:01.670537 ultima_scraper_api-1.1.0/pyproject.toml
--rw-r--r--   0        0        0      175 2022-12-03 17:24:36.799421 ultima_scraper_api-1.1.0/ultima_scraper_api/.readthedocs.yaml
--rw-r--r--   0        0        0     2286 2023-05-13 21:02:27.542962 ultima_scraper_api-1.1.0/ultima_scraper_api/__init__.py
--rw-r--r--   0        0        0        0 2022-12-04 09:00:20.736402 ultima_scraper_api-1.1.0/ultima_scraper_api/__main__.py
--rw-r--r--   0        0        0        0 2022-12-04 15:38:35.491230 ultima_scraper_api-1.1.0/ultima_scraper_api/apis/__init__.py
--rw-r--r--   0        0        0     6875 2023-05-10 16:14:24.886974 ultima_scraper_api-1.1.0/ultima_scraper_api/apis/api_helper.py
--rw-r--r--   0        0        0     3348 2023-05-08 16:02:24.472891 ultima_scraper_api-1.1.0/ultima_scraper_api/apis/api_streamliner.py
--rw-r--r--   0        0        0      696 2022-12-02 16:36:46.812390 ultima_scraper_api-1.1.0/ultima_scraper_api/apis/background_tasks.py
--rw-r--r--   0        0        0     2895 2023-05-09 15:10:07.346536 ultima_scraper_api-1.1.0/ultima_scraper_api/apis/fansly/__init__.py
--rw-r--r--   0        0        0      189 2023-05-13 20:33:08.152436 ultima_scraper_api-1.1.0/ultima_scraper_api/apis/fansly/classes/__init__.py
--rw-r--r--   0        0        0    19412 2023-05-14 02:46:17.178578 ultima_scraper_api-1.1.0/ultima_scraper_api/apis/fansly/classes/auth_model.py
--rw-r--r--   0        0        0     6511 2023-04-10 15:12:02.910813 ultima_scraper_api-1.1.0/ultima_scraper_api/apis/fansly/classes/collection_model.py
--rw-r--r--   0        0        0    11370 2023-04-11 14:57:48.165435 ultima_scraper_api-1.1.0/ultima_scraper_api/apis/fansly/classes/extras.py
--rw-r--r--   0        0        0      472 2022-01-17 19:20:07.000000 ultima_scraper_api-1.1.0/ultima_scraper_api/apis/fansly/classes/hightlight_model.py
--rw-r--r--   0        0        0     6463 2023-05-13 21:26:45.672240 ultima_scraper_api-1.1.0/ultima_scraper_api/apis/fansly/classes/message_model.py
--rw-r--r--   0        0        0     6918 2023-04-09 17:42:13.567826 ultima_scraper_api-1.1.0/ultima_scraper_api/apis/fansly/classes/post_model.py
--rw-r--r--   0        0        0     3210 2023-05-14 02:55:01.328937 ultima_scraper_api-1.1.0/ultima_scraper_api/apis/fansly/classes/story_model.py
--rw-r--r--   0        0        0      862 2023-05-14 01:36:53.261674 ultima_scraper_api-1.1.0/ultima_scraper_api/apis/fansly/classes/subscription_model.py
--rw-r--r--   0        0        0    27819 2023-05-14 01:25:40.886202 ultima_scraper_api-1.1.0/ultima_scraper_api/apis/fansly/classes/user_model.py
--rw-r--r--   0        0        0        0 2022-01-17 19:20:07.000000 ultima_scraper_api-1.1.0/ultima_scraper_api/apis/fansly/decorators/decorators.py
--rw-r--r--   0        0        0     2651 2023-05-14 13:27:19.560917 ultima_scraper_api-1.1.0/ultima_scraper_api/apis/fansly/fansly.py
--rw-r--r--   0        0        0     2784 2023-05-10 22:02:50.317100 ultima_scraper_api-1.1.0/ultima_scraper_api/apis/onlyfans/__init__.py
--rw-r--r--   0        0        0      191 2023-05-11 21:59:14.648026 ultima_scraper_api-1.1.0/ultima_scraper_api/apis/onlyfans/classes/__init__.py
--rw-r--r--   0        0        0    18865 2023-05-14 01:48:23.829859 ultima_scraper_api-1.1.0/ultima_scraper_api/apis/onlyfans/classes/auth_model.py
--rw-r--r--   0        0        0    11378 2023-05-10 21:08:35.574644 ultima_scraper_api-1.1.0/ultima_scraper_api/apis/onlyfans/classes/extras.py
--rw-r--r--   0        0        0      686 2023-03-25 19:37:35.462288 ultima_scraper_api-1.1.0/ultima_scraper_api/apis/onlyfans/classes/hightlight_model.py
--rw-r--r--   0        0        0     2971 2023-05-10 21:01:08.286698 ultima_scraper_api-1.1.0/ultima_scraper_api/apis/onlyfans/classes/message_model.py
--rw-r--r--   0        0        0     5698 2023-05-10 22:20:10.202315 ultima_scraper_api-1.1.0/ultima_scraper_api/apis/onlyfans/classes/only_drm.py
--rw-r--r--   0        0        0     3375 2023-03-27 00:23:55.042753 ultima_scraper_api-1.1.0/ultima_scraper_api/apis/onlyfans/classes/post_model.py
--rw-r--r--   0        0        0     1318 2023-04-09 10:09:44.773447 ultima_scraper_api-1.1.0/ultima_scraper_api/apis/onlyfans/classes/story_model.py
--rw-r--r--   0        0        0     1623 2023-05-13 21:04:18.608237 ultima_scraper_api-1.1.0/ultima_scraper_api/apis/onlyfans/classes/subscription_model.py
--rw-r--r--   0        0        0    28372 2023-05-10 19:46:18.928115 ultima_scraper_api-1.1.0/ultima_scraper_api/apis/onlyfans/classes/user_model.py
--rw-r--r--   0        0        0        0 2022-01-17 19:20:07.000000 ultima_scraper_api-1.1.0/ultima_scraper_api/apis/onlyfans/decorators/decorators.py
--rw-r--r--   0        0        0     2932 2023-05-14 13:27:38.918048 ultima_scraper_api-1.1.0/ultima_scraper_api/apis/onlyfans/onlyfans.py
--rw-r--r--   0        0        0     2763 2023-05-05 07:56:21.734680 ultima_scraper_api-1.1.0/ultima_scraper_api/apis/user_streamliner.py
--rw-r--r--   0        0        0        0 2022-12-04 09:59:08.749358 ultima_scraper_api-1.1.0/ultima_scraper_api/classes/__init__.py
--rw-r--r--   0        0        0    13187 2023-03-24 22:26:49.870986 ultima_scraper_api-1.1.0/ultima_scraper_api/classes/make_settings.py
--rw-r--r--   0        0        0     3977 2023-03-12 11:46:35.721289 ultima_scraper_api-1.1.0/ultima_scraper_api/classes/prepare_directories.py
--rw-r--r--   0        0        0      340 2022-01-17 19:20:07.000000 ultima_scraper_api-1.1.0/ultima_scraper_api/classes/prepare_download.py
--rw-r--r--   0        0        0    13410 2023-05-07 21:56:21.760084 ultima_scraper_api-1.1.0/ultima_scraper_api/classes/prepare_metadata.py
--rw-r--r--   0        0        0      630 2022-01-17 19:20:07.000000 ultima_scraper_api-1.1.0/ultima_scraper_api/classes/prepare_webhooks.py
--rw-r--r--   0        0        0      638 2022-12-03 12:11:12.443198 ultima_scraper_api-1.1.0/ultima_scraper_api/docs/Makefile
--rw-r--r--   0        0        0      804 2022-12-03 12:11:12.443198 ultima_scraper_api-1.1.0/ultima_scraper_api/docs/make.bat
--rw-r--r--   0        0        0       21 2022-12-03 17:06:06.309429 ultima_scraper_api-1.1.0/ultima_scraper_api/docs/requirements.txt
--rw-r--r--   0        0        0     1318 2022-12-03 18:16:52.399681 ultima_scraper_api-1.1.0/ultima_scraper_api/docs/source/conf.py
--rw-r--r--   0        0        0      464 2022-12-03 17:00:27.610084 ultima_scraper_api-1.1.0/ultima_scraper_api/docs/source/index.rst
--rw-r--r--   0        0        0        0 2022-12-04 09:51:18.483387 ultima_scraper_api-1.1.0/ultima_scraper_api/helpers/__init__.py
--rw-r--r--   0        0        0    11324 2023-05-09 19:08:54.838979 ultima_scraper_api-1.1.0/ultima_scraper_api/helpers/main_helper.py
--rw-r--r--   0        0        0        0 2023-01-26 05:39:16.747803 ultima_scraper_api-1.1.0/ultima_scraper_api/managers/__init__.py
--rw-r--r--   0        0        0        0 2023-01-22 17:41:52.794214 ultima_scraper_api-1.1.0/ultima_scraper_api/managers/job_manager/__init__.py
--rw-r--r--   0        0        0     1792 2023-05-13 20:28:21.224283 ultima_scraper_api-1.1.0/ultima_scraper_api/managers/job_manager/job_manager.py
--rw-r--r--   0        0        0        0 2023-01-22 17:42:18.641239 ultima_scraper_api-1.1.0/ultima_scraper_api/managers/job_manager/jobs/__init__.py
--rw-r--r--   0        0        0      767 2023-05-12 15:00:15.819155 ultima_scraper_api-1.1.0/ultima_scraper_api/managers/job_manager/jobs/custom_job.py
--rw-r--r--   0        0        0     2181 2023-03-27 18:00:12.375116 ultima_scraper_api-1.1.0/ultima_scraper_api/managers/scrape_manager.py
--rw-r--r--   0        0        0    17572 2023-05-13 13:21:06.845191 ultima_scraper_api-1.1.0/ultima_scraper_api/managers/session_manager.py
--rw-r--r--   0        0        0        0 2023-05-09 14:42:23.613712 ultima_scraper_api-1.1.0/ultima_scraper_api/models/__init__.py
--rw-r--r--   0        0        0      677 2023-05-11 21:44:11.005112 ultima_scraper_api-1.1.0/ultima_scraper_api/models/subscription_model.py
--rw-r--r--   0        0        0        0 2022-12-04 16:42:28.821209 ultima_scraper_api-1.1.0/ultima_scraper_api/py.typed
--rw-r--r--   0        0        0     1052 1970-01-01 00:00:00.000000 ultima_scraper_api-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1193 2023-05-22 11:06:13.714856 ultima_scraper_api-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0      175 2022-12-03 17:24:36.799421 ultima_scraper_api-1.1.1/ultima_scraper_api/.readthedocs.yaml
+-rw-r--r--   0        0        0     2286 2023-05-13 21:02:27.542962 ultima_scraper_api-1.1.1/ultima_scraper_api/__init__.py
+-rw-r--r--   0        0        0        0 2022-12-04 09:00:20.736402 ultima_scraper_api-1.1.1/ultima_scraper_api/__main__.py
+-rw-r--r--   0        0        0        0 2022-12-04 15:38:35.491230 ultima_scraper_api-1.1.1/ultima_scraper_api/apis/__init__.py
+-rw-r--r--   0        0        0     6875 2023-05-10 16:14:24.886974 ultima_scraper_api-1.1.1/ultima_scraper_api/apis/api_helper.py
+-rw-r--r--   0        0        0     3348 2023-05-22 07:12:01.748229 ultima_scraper_api-1.1.1/ultima_scraper_api/apis/api_streamliner.py
+-rw-r--r--   0        0        0      696 2022-12-02 16:36:46.812390 ultima_scraper_api-1.1.1/ultima_scraper_api/apis/background_tasks.py
+-rw-r--r--   0        0        0     2895 2023-05-09 15:10:07.346536 ultima_scraper_api-1.1.1/ultima_scraper_api/apis/fansly/__init__.py
+-rw-r--r--   0        0        0      189 2023-05-13 20:33:08.152436 ultima_scraper_api-1.1.1/ultima_scraper_api/apis/fansly/classes/__init__.py
+-rw-r--r--   0        0        0    19475 2023-05-22 10:26:50.629643 ultima_scraper_api-1.1.1/ultima_scraper_api/apis/fansly/classes/auth_model.py
+-rw-r--r--   0        0        0     6511 2023-04-10 15:12:02.910813 ultima_scraper_api-1.1.1/ultima_scraper_api/apis/fansly/classes/collection_model.py
+-rw-r--r--   0        0        0    11481 2023-05-22 10:32:32.883960 ultima_scraper_api-1.1.1/ultima_scraper_api/apis/fansly/classes/extras.py
+-rw-r--r--   0        0        0      472 2022-01-17 19:20:07.000000 ultima_scraper_api-1.1.1/ultima_scraper_api/apis/fansly/classes/hightlight_model.py
+-rw-r--r--   0        0        0     6463 2023-05-13 21:26:45.672240 ultima_scraper_api-1.1.1/ultima_scraper_api/apis/fansly/classes/message_model.py
+-rw-r--r--   0        0        0     6918 2023-04-09 17:42:13.567826 ultima_scraper_api-1.1.1/ultima_scraper_api/apis/fansly/classes/post_model.py
+-rw-r--r--   0        0        0     3210 2023-05-14 02:55:01.328937 ultima_scraper_api-1.1.1/ultima_scraper_api/apis/fansly/classes/story_model.py
+-rw-r--r--   0        0        0      862 2023-05-14 01:36:53.261674 ultima_scraper_api-1.1.1/ultima_scraper_api/apis/fansly/classes/subscription_model.py
+-rw-r--r--   0        0        0    27593 2023-05-22 08:33:43.650098 ultima_scraper_api-1.1.1/ultima_scraper_api/apis/fansly/classes/user_model.py
+-rw-r--r--   0        0        0        0 2022-01-17 19:20:07.000000 ultima_scraper_api-1.1.1/ultima_scraper_api/apis/fansly/decorators/decorators.py
+-rw-r--r--   0        0        0     2961 2023-05-22 10:30:47.276706 ultima_scraper_api-1.1.1/ultima_scraper_api/apis/fansly/fansly.py
+-rw-r--r--   0        0        0     2784 2023-05-10 22:02:50.317100 ultima_scraper_api-1.1.1/ultima_scraper_api/apis/onlyfans/__init__.py
+-rw-r--r--   0        0        0      191 2023-05-11 21:59:14.648026 ultima_scraper_api-1.1.1/ultima_scraper_api/apis/onlyfans/classes/__init__.py
+-rw-r--r--   0        0        0    19161 2023-05-22 10:10:45.530951 ultima_scraper_api-1.1.1/ultima_scraper_api/apis/onlyfans/classes/auth_model.py
+-rw-r--r--   0        0        0    11385 2023-05-22 06:26:19.792870 ultima_scraper_api-1.1.1/ultima_scraper_api/apis/onlyfans/classes/extras.py
+-rw-r--r--   0        0        0      686 2023-03-25 19:37:35.462288 ultima_scraper_api-1.1.1/ultima_scraper_api/apis/onlyfans/classes/hightlight_model.py
+-rw-r--r--   0        0        0     2971 2023-05-10 21:01:08.286698 ultima_scraper_api-1.1.1/ultima_scraper_api/apis/onlyfans/classes/message_model.py
+-rw-r--r--   0        0        0     5863 2023-05-22 05:00:15.206814 ultima_scraper_api-1.1.1/ultima_scraper_api/apis/onlyfans/classes/only_drm.py
+-rw-r--r--   0        0        0     3375 2023-03-27 00:23:55.042753 ultima_scraper_api-1.1.1/ultima_scraper_api/apis/onlyfans/classes/post_model.py
+-rw-r--r--   0        0        0     1318 2023-04-09 10:09:44.773447 ultima_scraper_api-1.1.1/ultima_scraper_api/apis/onlyfans/classes/story_model.py
+-rw-r--r--   0        0        0     1623 2023-05-13 21:04:18.608237 ultima_scraper_api-1.1.1/ultima_scraper_api/apis/onlyfans/classes/subscription_model.py
+-rw-r--r--   0        0        0    28146 2023-05-22 08:33:34.023692 ultima_scraper_api-1.1.1/ultima_scraper_api/apis/onlyfans/classes/user_model.py
+-rw-r--r--   0        0        0        0 2022-01-17 19:20:07.000000 ultima_scraper_api-1.1.1/ultima_scraper_api/apis/onlyfans/decorators/decorators.py
+-rw-r--r--   0        0        0     3242 2023-05-22 07:26:53.595528 ultima_scraper_api-1.1.1/ultima_scraper_api/apis/onlyfans/onlyfans.py
+-rw-r--r--   0        0        0     2763 2023-05-05 07:56:21.734680 ultima_scraper_api-1.1.1/ultima_scraper_api/apis/user_streamliner.py
+-rw-r--r--   0        0        0        0 2022-12-04 09:59:08.749358 ultima_scraper_api-1.1.1/ultima_scraper_api/classes/__init__.py
+-rw-r--r--   0        0        0    13187 2023-03-24 22:26:49.870986 ultima_scraper_api-1.1.1/ultima_scraper_api/classes/make_settings.py
+-rw-r--r--   0        0        0     3977 2023-03-12 11:46:35.721289 ultima_scraper_api-1.1.1/ultima_scraper_api/classes/prepare_directories.py
+-rw-r--r--   0        0        0      340 2022-01-17 19:20:07.000000 ultima_scraper_api-1.1.1/ultima_scraper_api/classes/prepare_download.py
+-rw-r--r--   0        0        0    13410 2023-05-07 21:56:21.760084 ultima_scraper_api-1.1.1/ultima_scraper_api/classes/prepare_metadata.py
+-rw-r--r--   0        0        0      630 2022-01-17 19:20:07.000000 ultima_scraper_api-1.1.1/ultima_scraper_api/classes/prepare_webhooks.py
+-rw-r--r--   0        0        0      638 2022-12-03 12:11:12.443198 ultima_scraper_api-1.1.1/ultima_scraper_api/docs/Makefile
+-rw-r--r--   0        0        0      804 2022-12-03 12:11:12.443198 ultima_scraper_api-1.1.1/ultima_scraper_api/docs/make.bat
+-rw-r--r--   0        0        0       21 2022-12-03 17:06:06.309429 ultima_scraper_api-1.1.1/ultima_scraper_api/docs/requirements.txt
+-rw-r--r--   0        0        0     1318 2022-12-03 18:16:52.399681 ultima_scraper_api-1.1.1/ultima_scraper_api/docs/source/conf.py
+-rw-r--r--   0        0        0      464 2022-12-03 17:00:27.610084 ultima_scraper_api-1.1.1/ultima_scraper_api/docs/source/index.rst
+-rw-r--r--   0        0        0        0 2022-12-04 09:51:18.483387 ultima_scraper_api-1.1.1/ultima_scraper_api/helpers/__init__.py
+-rw-r--r--   0        0        0    11324 2023-05-09 19:08:54.838979 ultima_scraper_api-1.1.1/ultima_scraper_api/helpers/main_helper.py
+-rw-r--r--   0        0        0        0 2023-01-26 05:39:16.747803 ultima_scraper_api-1.1.1/ultima_scraper_api/managers/__init__.py
+-rw-r--r--   0        0        0        0 2023-01-22 17:41:52.794214 ultima_scraper_api-1.1.1/ultima_scraper_api/managers/job_manager/__init__.py
+-rw-r--r--   0        0        0     1792 2023-05-13 20:28:21.224283 ultima_scraper_api-1.1.1/ultima_scraper_api/managers/job_manager/job_manager.py
+-rw-r--r--   0        0        0        0 2023-01-22 17:42:18.641239 ultima_scraper_api-1.1.1/ultima_scraper_api/managers/job_manager/jobs/__init__.py
+-rw-r--r--   0        0        0      767 2023-05-12 15:00:15.819155 ultima_scraper_api-1.1.1/ultima_scraper_api/managers/job_manager/jobs/custom_job.py
+-rw-r--r--   0        0        0     2181 2023-03-27 18:00:12.375116 ultima_scraper_api-1.1.1/ultima_scraper_api/managers/scrape_manager.py
+-rw-r--r--   0        0        0    17695 2023-05-22 11:09:54.319065 ultima_scraper_api-1.1.1/ultima_scraper_api/managers/session_manager.py
+-rw-r--r--   0        0        0        0 2023-05-09 14:42:23.613712 ultima_scraper_api-1.1.1/ultima_scraper_api/models/__init__.py
+-rw-r--r--   0        0        0      677 2023-05-11 21:44:11.005112 ultima_scraper_api-1.1.1/ultima_scraper_api/models/subscription_model.py
+-rw-r--r--   0        0        0        0 2022-12-04 16:42:28.821209 ultima_scraper_api-1.1.1/ultima_scraper_api/py.typed
+-rw-r--r--   0        0        0     1052 1970-01-01 00:00:00.000000 ultima_scraper_api-1.1.1/PKG-INFO
```

### Comparing `ultima_scraper_api-1.1.0/pyproject.toml` & `ultima_scraper_api-1.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ultima-scraper-api"
-version = "1.1.0"
+version = "1.1.1"
 description = ""
 authors = [
     "DIGITALCRIMINALS <89371864+digitalcriminals@users.noreply.github.com>",
 ]
 packages = [{include = "ultima_scraper_api"}]
 include = ["ultima_scraper_api/py.typed"]
```

### Comparing `ultima_scraper_api-1.1.0/ultima_scraper_api/__init__.py` & `ultima_scraper_api-1.1.1/ultima_scraper_api/__init__.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-1.1.0/ultima_scraper_api/apis/api_helper.py` & `ultima_scraper_api-1.1.1/ultima_scraper_api/apis/api_helper.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-1.1.0/ultima_scraper_api/apis/api_streamliner.py` & `ultima_scraper_api-1.1.1/ultima_scraper_api/apis/api_streamliner.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-1.1.0/ultima_scraper_api/apis/background_tasks.py` & `ultima_scraper_api-1.1.1/ultima_scraper_api/apis/background_tasks.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-1.1.0/ultima_scraper_api/apis/fansly/__init__.py` & `ultima_scraper_api-1.1.1/ultima_scraper_api/apis/fansly/__init__.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-1.1.0/ultima_scraper_api/apis/fansly/classes/auth_model.py` & `ultima_scraper_api-1.1.1/ultima_scraper_api/apis/fansly/classes/auth_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,35 +1,34 @@
 from __future__ import annotations
 
 import asyncio
 from datetime import datetime
-from itertools import chain, product
-from typing import TYPE_CHECKING, Any, Dict, Optional, Union
+from itertools import product
+from typing import TYPE_CHECKING, Any, Dict, Optional
 
 from dateutil.relativedelta import relativedelta
+from user_agent import generate_user_agent
+
 from ultima_scraper_api.apis import api_helper
+from ultima_scraper_api.apis.fansly import SubscriptionType
 from ultima_scraper_api.apis.fansly.classes.extras import (
     AuthDetails,
     ErrorDetails,
     create_headers,
     endpoint_links,
 )
 from ultima_scraper_api.apis.fansly.classes.message_model import create_message
 from ultima_scraper_api.apis.fansly.classes.post_model import create_post
 from ultima_scraper_api.apis.fansly.classes.subscription_model import SubscriptionModel
 from ultima_scraper_api.apis.fansly.classes.user_model import create_user
 from ultima_scraper_api.managers.session_manager import SessionManager
-from user_agent import generate_user_agent
-from ultima_scraper_api.apis.fansly import SubscriptionType
 
 if TYPE_CHECKING:
-    from ultima_scraper_api.apis.onlyfans.classes.only_drm import OnlyDRM
     from ultima_scraper_api.apis.fansly.fansly import FanslyAPI
-
-from typing import TYPE_CHECKING, Any, Dict, Optional, Union
+    from ultima_scraper_api.apis.onlyfans.classes.only_drm import OnlyDRM
 
 
 class create_auth(create_user):
     def __init__(
         self,
         api: FanslyAPI,
         option: dict[str, Any] = {},
@@ -48,16 +47,16 @@
         self.subscriptions: list[SubscriptionModel] = []
         self.followed_users: list[create_user] = []
         self.chats = None
         self.archived_stories = {}
         self.mass_messages = []
         self.paid_content: list[create_message | create_post] = []
         self.auth_attempt = 0
+        self.max_attempts = 10
         self.guest = False
-        self.active: bool = False
         self.errors: list[ErrorDetails] = []
         self.extras: dict[str, Any] = {}
         self.blacklist: list[str] = []
         self.drm: OnlyDRM | None = None
 
     class _SessionManager(SessionManager):
         def __init__(
@@ -86,30 +85,30 @@
         if not data["username"]:
             data["username"] = f"u{data['id']}"
         for key, value in data.items():
             found_attr = hasattr(self, key)
             if found_attr:
                 setattr(self, key, value)
 
-    async def login(self, max_attempts: int = 10, guest: bool = False):
+    async def login(self, guest: bool = False):
         auth_items = self.auth_details
         if not auth_items:
             return self
         if guest and auth_items:
             auth_items.user_agent = generate_user_agent()
         link = endpoint_links().customer
         user_agent = auth_items.user_agent
         dynamic_rules = self.session_manager.dynamic_rules
         a: list[Any] = [dynamic_rules, user_agent, link]
         self.session_manager.headers = create_headers(*a)
         if guest:
             self.guest = True
             return self
 
-        while self.auth_attempt < max_attempts + 1:
+        while self.auth_attempt < self.max_attempts:
             await self.process_auth()
             self.auth_attempt += 1
 
             async def resolve_auth(auth: create_auth):
                 if self.errors:
                     error = self.errors[-1]
                     print(error.message)
@@ -134,52 +133,52 @@
                                     print("Success")
                                     auth.active = False
                                     auth.errors.remove(error)
                                     await self.process_auth()
                                     break
 
             await resolve_auth(self)
-            if not self.active:
+            if not self.check_authed():
                 if self.errors:
                     error = self.errors[-1]
                     error_message = error.message
                     if "token" in error_message:
                         break
                     if "Code wrong" in error_message:
                         break
                     if "Please refresh" in error_message:
                         break
                 else:
                     print("Auth 404'ed")
                 continue
             else:
                 break
-        if not self.active:
+        if not self.check_authed():
             user = await self.get_user(self.id)
             if isinstance(user, create_user):
                 self.update(user.__dict__)
         return self
 
     async def process_auth(self):
-        if not self.active:
+        if not self.maxed_out_auth_attempts():
             link = endpoint_links().settings
             response = await self.session_manager.json_request(link)
             if isinstance(response, dict):
                 final_response: dict[str, Any] = response
                 link = endpoint_links(final_response["response"]["accountId"]).customer
                 final_response = await self.session_manager.json_request(link)
                 await self.resolve_auth_errors(final_response)
                 if not self.errors:
-                    # merged = self.__dict__ | final_response
-                    # self = create_auth(merged,self.pool,self.session_manager.max_threads)
-                    self.active = True
+                    self.auth_details.active = True
                     self.update(final_response)
+                else:
+                    self.auth_details.active = False
             else:
                 # 404'ed
-                self.active = False
+                self.auth_details.active = False
         return self
 
     async def resolve_auth_errors(self, response: ErrorDetails | dict[str, Any]):
         # Adds an error object to self.auth.errors
         if isinstance(response, ErrorDetails):
             error = response
         elif "error" in response:
@@ -489,7 +488,13 @@
         return user
 
     async def get_scrapable_users(self):
         followed_users = self.followed_users
         subscription_users = [x.user for x in self.subscriptions]
         unique_users = list(set(followed_users) | set(subscription_users))
         return unique_users
+
+    def maxed_out_auth_attempts(self):
+        return True if self.auth_attempt >= self.max_attempts else False
+
+    def check_authed(self):
+        return self.auth_details.active
```

### Comparing `ultima_scraper_api-1.1.0/ultima_scraper_api/apis/fansly/classes/collection_model.py` & `ultima_scraper_api-1.1.1/ultima_scraper_api/apis/fansly/classes/collection_model.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-1.1.0/ultima_scraper_api/apis/fansly/classes/extras.py` & `ultima_scraper_api-1.1.1/ultima_scraper_api/apis/fansly/classes/extras.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,25 @@
 import math
 from itertools import chain
 from pathlib import Path
 from typing import Any, Literal, Optional, Union
 
 
 class AuthDetails:
-    def __init__(self, username:str="", authorization:str="", user_agent:str="",email:str="", password:str="", hashed:bool=False,support_2fa:bool=True, active:bool=True) -> None:
+    def __init__(
+        self,
+        username: str = "",
+        authorization: str = "",
+        user_agent: str = "",
+        email: str = "",
+        password: str = "",
+        hashed: bool = False,
+        support_2fa: bool = True,
+        active: bool | None = None,
+    ) -> None:
         self.username = username
         self.authorization = authorization
         self.user_agent = user_agent
         self.email = email
         self.password = password
         self.hashed = hashed
         self.support_2fa = support_2fa
@@ -149,15 +159,14 @@
         self.favorite = f"https://onlyfans.com/api2/v2/{identifier}/{identifier2}/favorites/{identifier3}"
         self.transactions = (
             f"https://onlyfans.com/api2/v2/payments/all/transactions?limit=10&offset=0"
         )
         self.two_factor = f"https://onlyfans.com/api2/v2/users/otp/check"
 
     def list_followings(self, identifier: int, offset: int = 0):
-
         return f"{self.full_url_path}/account/{identifier}/following?before=0&after=0&limit=100&offset={offset}"
 
     def list_users(self, identifiers: list[int | str] | list[int] | list[str]):
         identifier_type = "ids"
         if all(isinstance(x, str) and x.isalpha() for x in identifiers):
             identifier_type = "usernames"
         link = ""
```

### Comparing `ultima_scraper_api-1.1.0/ultima_scraper_api/apis/fansly/classes/message_model.py` & `ultima_scraper_api-1.1.1/ultima_scraper_api/apis/fansly/classes/message_model.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-1.1.0/ultima_scraper_api/apis/fansly/classes/post_model.py` & `ultima_scraper_api-1.1.1/ultima_scraper_api/apis/fansly/classes/post_model.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-1.1.0/ultima_scraper_api/apis/fansly/classes/story_model.py` & `ultima_scraper_api-1.1.1/ultima_scraper_api/apis/fansly/classes/story_model.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-1.1.0/ultima_scraper_api/apis/fansly/classes/subscription_model.py` & `ultima_scraper_api-1.1.1/ultima_scraper_api/apis/fansly/classes/subscription_model.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-1.1.0/ultima_scraper_api/apis/fansly/classes/user_model.py` & `ultima_scraper_api-1.1.1/ultima_scraper_api/apis/fansly/classes/user_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,14 @@
 
 class create_user(StreamlinedUser):
     def __init__(
         self,
         option: dict[str, Any],
         authed: create_auth,
     ) -> None:
-
         self.avatar: Any = option.get("avatar")
         self.avatarThumbs: Any = option.get("avatarThumbs")
         self.header: Any = option.get("banner")
         self.headerSize: Any = option.get("headerSize")
         self.headerThumbs: Any = option.get("headerThumbs")
         self.id: int = option.get("id")
         self.name: str = option.get("name")
@@ -226,23 +225,14 @@
         authed.users.add(self)
         self.download_info: dict[str, Any] = {}
         self.duplicate_media = []
         self.scrape_manager = ScrapeManager(authed.session_manager)
         self.__raw__ = option
         StreamlinedUser.__init__(self, authed)
 
-    def __eq__(self, other: Any):
-        if isinstance(self, create_user):
-            if self.id == other.id:
-                return True
-        return False
-
-    def __hash__(self) -> int:
-        return hash((self.id))
-
     def get_link(self):
         link = f"https://fansly.com/{self.username}"
         return link
 
     def is_me(self) -> bool:
         status = False
         if self.email:
```

### Comparing `ultima_scraper_api-1.1.0/ultima_scraper_api/apis/fansly/fansly.py` & `ultima_scraper_api-1.1.1/ultima_scraper_api/apis/fansly/fansly.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,14 +22,23 @@
                 final_auth = auth
             elif auth.username == identifier:
                 final_auth = auth
             if final_auth:
                 break
         return final_auth
 
+    async def remove_invalid_auths(self):
+        for auth in self.auths.copy():
+            if not auth.check_authed():
+                await self.remove_auth(auth)
+
+    async def remove_auth(self, auth: create_auth):
+        await auth.session_manager.active_session.close()
+        self.auths.remove(auth)
+
     def create_auth_details(self, auth_json: dict[str, Any] = {}) -> AuthDetails:
         """If you've got a auth.json file, you can load it into python and pass it through here.
 
         Args:
             auth_json (dict[str, Any], optional): [description]. Defaults to {}.
 
         Returns:
```

### Comparing `ultima_scraper_api-1.1.0/ultima_scraper_api/apis/onlyfans/__init__.py` & `ultima_scraper_api-1.1.1/ultima_scraper_api/apis/onlyfans/__init__.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-1.1.0/ultima_scraper_api/apis/onlyfans/classes/auth_model.py` & `ultima_scraper_api-1.1.1/ultima_scraper_api/apis/onlyfans/classes/auth_model.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,29 +2,29 @@
 
 import asyncio
 import math
 from itertools import chain, product
 from typing import TYPE_CHECKING, Any, Dict, Optional
 
 from ultima_scraper_api.apis import api_helper
+from ultima_scraper_api.apis.onlyfans import SubscriptionType
 from ultima_scraper_api.apis.onlyfans.classes.extras import (
     AuthDetails,
     ErrorDetails,
     create_headers,
     endpoint_links,
 )
 from ultima_scraper_api.apis.onlyfans.classes.message_model import create_message
 from ultima_scraper_api.apis.onlyfans.classes.post_model import create_post
-from ultima_scraper_api.apis.onlyfans.classes.user_model import create_user
-from ultima_scraper_api.managers.session_manager import SessionManager
-from user_agent import generate_user_agent
-from ultima_scraper_api.apis.onlyfans import SubscriptionType
 from ultima_scraper_api.apis.onlyfans.classes.subscription_model import (
     SubscriptionModel,
 )
+from ultima_scraper_api.apis.onlyfans.classes.user_model import create_user
+from ultima_scraper_api.managers.session_manager import SessionManager
+from user_agent import generate_user_agent
 
 if TYPE_CHECKING:
     from ultima_scraper_api.apis.onlyfans.classes.only_drm import OnlyDRM
     from ultima_scraper_api.apis.onlyfans.onlyfans import OnlyFansAPI
 
 # auth_model.py handles functions that only relate to the authenticated user
 # We can create a auth_streamliner that has a parent class of create_user instead
@@ -49,16 +49,16 @@
         self.links = api.ContentTypes()
         self.subscriptions: list[SubscriptionModel] = []
         self.chats = None
         self.archived_stories = {}
         self.mass_messages = []
         self.paid_content: list[create_message | create_post] = []
         self.auth_attempt = 0
+        self.max_attempts = 10
         self.guest = False
-        self.active: bool = False
         self.errors: list[ErrorDetails] = []
         self.extras: dict[str, Any] = {}
         self.blacklist: list[str] = []
         self.drm: OnlyDRM | None = None
 
     class _SessionManager(SessionManager):
         def __init__(
@@ -86,15 +86,15 @@
         if not data["username"]:
             data["username"] = f"u{data['id']}"
         for key, value in data.items():
             found_attr = hasattr(self, key)
             if found_attr:
                 setattr(self, key, value)
 
-    async def login(self, max_attempts: int = 10, guest: bool = False):
+    async def login(self, guest: bool = False):
         auth_items = self.auth_details
         if not auth_items:
             return self
         if guest and auth_items:
             auth_items.cookie.auth_id = "0"
             auth_items.user_agent = generate_user_agent()
         link = endpoint_links().customer
@@ -104,15 +104,15 @@
         dynamic_rules = self.session_manager.dynamic_rules
         a: list[Any] = [dynamic_rules, auth_id, auth_items.x_bc, user_agent, link]
         self.session_manager.headers = create_headers(*a)
         if guest:
             self.guest = True
             return self
 
-        while self.auth_attempt < max_attempts:
+        while self.auth_attempt < self.max_attempts:
             await self.process_auth()
             self.auth_attempt += 1
 
             async def resolve_auth(auth: create_auth):
                 if self.errors:
                     error = self.errors[-1]
                     if error.code == 101:
@@ -136,45 +136,47 @@
                                     print("Success")
                                     auth.active = False
                                     auth.errors.remove(error)
                                     await self.process_auth()
                                     break
 
             await resolve_auth(self)
-            if not self.active:
+            if not self.check_authed():
                 if self.errors:
                     error = self.errors[-1]
                     error_message = error.message
                     if "token" in error_message:
                         break
                     if "Code wrong" in error_message:
                         break
                     if "Please refresh" in error_message:
                         break
                 continue
             else:
                 break
-        if not self.active:
+        if not self.check_authed():
             user = await self.get_user(auth_id)
             if isinstance(user, create_user):
                 self.update(user.__dict__)
         return self
 
     async def process_auth(self):
-        if not self.active:
+        if not self.maxed_out_auth_attempts():
             link = endpoint_links().customer
             json_resp = await self.session_manager.json_request(link)
             if json_resp:
                 await self.resolve_auth_errors(json_resp)
                 if not self.errors:
-                    self.active = True
+                    self.auth_details.active = True
                     self.update(json_resp)
+                else:
+                    self.auth_details.active = False
             else:
                 # 404'ed
-                self.active = False
+                self.auth_details.active = False
         return self
 
     async def resolve_auth_errors(self, response: ErrorDetails | dict[str, Any]):
         # Adds an error object to self.auth.errors
         if isinstance(response, ErrorDetails):
             error = response
         elif "error" in response:
@@ -483,7 +485,13 @@
             if not isinstance(post, ErrorDetails):
                 user = post.author
         return user
 
     async def get_scrapable_users(self):
         subscription_users = [x.user for x in self.subscriptions]
         return subscription_users
+
+    def maxed_out_auth_attempts(self):
+        return True if self.auth_attempt >= self.max_attempts else False
+
+    def check_authed(self):
+        return self.auth_details.active
```

### Comparing `ultima_scraper_api-1.1.0/ultima_scraper_api/apis/onlyfans/classes/extras.py` & `ultima_scraper_api-1.1.1/ultima_scraper_api/apis/onlyfans/classes/extras.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 import copy
 import math
 from itertools import chain
 from pathlib import Path
 from typing import Any, Literal, Optional, Union
-from urllib.parse import urlparse, parse_qs
+from urllib.parse import parse_qs, urlparse
 
 
 class AuthDetails:
     def __init__(
         self,
         username: str = "",
         cookie: str = "",
         x_bc: str = "",
         user_agent: str = "",
         email: str = "",
         password: str = "",
         hashed: bool = False,
         support_2fa: bool = True,
-        active: bool = True,
+        active: bool | None = None,
     ) -> None:
         self.username = username
         self.cookie = cookie_parser(cookie)
         self.x_bc = x_bc
         self.user_agent = user_agent
         self.email = email
         self.password = password
```

### Comparing `ultima_scraper_api-1.1.0/ultima_scraper_api/apis/onlyfans/classes/hightlight_model.py` & `ultima_scraper_api-1.1.1/ultima_scraper_api/apis/onlyfans/classes/hightlight_model.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-1.1.0/ultima_scraper_api/apis/onlyfans/classes/message_model.py` & `ultima_scraper_api-1.1.1/ultima_scraper_api/apis/onlyfans/classes/message_model.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-1.1.0/ultima_scraper_api/apis/onlyfans/classes/only_drm.py` & `ultima_scraper_api-1.1.1/ultima_scraper_api/apis/onlyfans/classes/only_drm.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,26 @@
+import platform
+import re
+import subprocess
 from pathlib import Path
+from typing import TYPE_CHECKING, Any
 
+import orjson
+import xmltodict
 from pywidevine.cdm import Cdm
 from pywidevine.device import Device
 from pywidevine.pssh import PSSH
-from typing import TYPE_CHECKING, Any
-import orjson
-import xmltodict
-import re
+
 from ultima_scraper_api.apis.onlyfans.classes.extras import endpoint_links
-import subprocess
 
 if TYPE_CHECKING:
     import ultima_scraper_api
 
     auth_types = ultima_scraper_api.auth_types
-
+os_name = platform.system()
 # Replace authed with your ClientSession
 # Replace endpoint_links.drm_server with "https://onlyfans.com/api2/v2/users/media/{MEDIA_ID}/drm/post/{POST_ID}?type=widevine"
 # media_item is a Post's media from the "https://onlyfans.com/api2/v2/posts/{USER_ID}?skip_users=all" api
 
 
 class OnlyDRM:
     def __init__(
@@ -133,17 +135,20 @@
         directory_url = self.extract_directory_from_url(dash_url)
         base_url = mpd["MPD"]["Period"]["AdaptationSet"][1]["Representation"]["BaseURL"]
         media_url = f"https://cdn3.onlyfans.com/dash/files/{directory_url}/{base_url}"
         return media_url
 
     def decrypt_file(self, filepath: Path, key: str):
         output_filepath = Path(filepath.as_posix().replace("enc", "dec"))
+        mp4decrypt_path = "./mp4decrypt"
+        if os_name == "Windows":
+            mp4decrypt_path = ".\\mp4decrypt"
         pid = subprocess.Popen(
             [
-                "./mp4decrypt",
+                mp4decrypt_path,
                 f"{filepath.as_posix()}",
                 f"{output_filepath.as_posix()}",
                 "--key",
                 key,
             ],
             stdout=subprocess.PIPE,
             stderr=subprocess.PIPE,
```

### Comparing `ultima_scraper_api-1.1.0/ultima_scraper_api/apis/onlyfans/classes/post_model.py` & `ultima_scraper_api-1.1.1/ultima_scraper_api/apis/onlyfans/classes/post_model.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-1.1.0/ultima_scraper_api/apis/onlyfans/classes/story_model.py` & `ultima_scraper_api-1.1.1/ultima_scraper_api/apis/onlyfans/classes/story_model.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-1.1.0/ultima_scraper_api/apis/onlyfans/classes/subscription_model.py` & `ultima_scraper_api-1.1.1/ultima_scraper_api/apis/onlyfans/classes/subscription_model.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-1.1.0/ultima_scraper_api/apis/onlyfans/classes/user_model.py` & `ultima_scraper_api-1.1.1/ultima_scraper_api/apis/onlyfans/classes/user_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,14 @@
 if TYPE_CHECKING:
     from ultima_scraper_api.apis.onlyfans.classes.auth_model import create_auth
     from ultima_scraper_api.apis.onlyfans.classes.post_model import create_post
 
 
 class create_user(StreamlinedUser):
     def __init__(self, option: dict[str, Any], authed: create_auth) -> None:
-
         self.avatar: Optional[str] = option.get("avatar")
         self.avatarThumbs: Optional[list[str]] = option.get("avatarThumbs")
         self.header: Optional[str] = option.get("header")
         self.headerSize: Optional[dict[str, int]] = option.get("headerSize")
         self.headerThumbs: Optional[list[str]] = option.get("headerThumbs")
         self.id: int = option.get("id")
         self.name: str = option.get("name")
@@ -215,23 +214,14 @@
         authed.users.add(self)
         self.download_info: dict[str, Any] = {}
         self.duplicate_media = []
         self.scrape_manager = ScrapeManager(authed.session_manager)
         self.__raw__ = option
         StreamlinedUser.__init__(self, authed)
 
-    def __eq__(self, other: Any):
-        if isinstance(self, create_user):
-            if self.id == other.id:
-                return True
-        return False
-
-    def __hash__(self) -> int:
-        return hash((self.id))
-
     def get_link(self):
         link = f"https://onlyfans.com/{self.username}"
         return link
 
     def is_me(self) -> bool:
         status = False
         if self.email:
```

### Comparing `ultima_scraper_api-1.1.0/ultima_scraper_api/apis/onlyfans/onlyfans.py` & `ultima_scraper_api-1.1.1/ultima_scraper_api/apis/onlyfans/onlyfans.py`

 * *Files 5% similar despite different names*

```diff
@@ -25,14 +25,23 @@
                 final_auth = auth
             elif auth.username == identifier:
                 final_auth = auth
             if final_auth:
                 break
         return final_auth
 
+    async def remove_invalid_auths(self):
+        for auth in self.auths.copy():
+            if not auth.check_authed():
+                await self.remove_auth(auth)
+
+    async def remove_auth(self, auth: create_auth):
+        await auth.session_manager.active_session.close()
+        self.auths.remove(auth)
+
     def create_auth_details(self, auth_json: dict[str, Any] = {}) -> AuthDetails:
         """If you've got a auth.json file, you can load it into python and pass it through here.
 
         Args:
             auth_json (dict[str, Any], optional): [description]. Defaults to {}.
 
         Returns:
```

### Comparing `ultima_scraper_api-1.1.0/ultima_scraper_api/apis/user_streamliner.py` & `ultima_scraper_api-1.1.1/ultima_scraper_api/apis/user_streamliner.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-1.1.0/ultima_scraper_api/classes/make_settings.py` & `ultima_scraper_api-1.1.1/ultima_scraper_api/classes/make_settings.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-1.1.0/ultima_scraper_api/classes/prepare_directories.py` & `ultima_scraper_api-1.1.1/ultima_scraper_api/classes/prepare_directories.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-1.1.0/ultima_scraper_api/classes/prepare_metadata.py` & `ultima_scraper_api-1.1.1/ultima_scraper_api/classes/prepare_metadata.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-1.1.0/ultima_scraper_api/classes/prepare_webhooks.py` & `ultima_scraper_api-1.1.1/ultima_scraper_api/classes/prepare_webhooks.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-1.1.0/ultima_scraper_api/docs/Makefile` & `ultima_scraper_api-1.1.1/ultima_scraper_api/docs/Makefile`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-1.1.0/ultima_scraper_api/docs/make.bat` & `ultima_scraper_api-1.1.1/ultima_scraper_api/docs/make.bat`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-1.1.0/ultima_scraper_api/docs/source/conf.py` & `ultima_scraper_api-1.1.1/ultima_scraper_api/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-1.1.0/ultima_scraper_api/helpers/main_helper.py` & `ultima_scraper_api-1.1.1/ultima_scraper_api/helpers/main_helper.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-1.1.0/ultima_scraper_api/managers/job_manager/job_manager.py` & `ultima_scraper_api-1.1.1/ultima_scraper_api/managers/job_manager/job_manager.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-1.1.0/ultima_scraper_api/managers/job_manager/jobs/custom_job.py` & `ultima_scraper_api-1.1.1/ultima_scraper_api/managers/job_manager/jobs/custom_job.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-1.1.0/ultima_scraper_api/managers/scrape_manager.py` & `ultima_scraper_api-1.1.1/ultima_scraper_api/managers/scrape_manager.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-1.1.0/ultima_scraper_api/managers/session_manager.py` & `ultima_scraper_api-1.1.1/ultima_scraper_api/managers/session_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -142,17 +142,19 @@
         connector = (
             self.proxy_manager.create_connection(proxy)
             if self.proxies
             else aiohttp.TCPConnector(limit=limit)
         )
         final_cookies = self.get_cookies()
         # Had to remove final_cookies and cookies=final_cookies due to it conflicting with headers
+        timeout = aiohttp.ClientTimeout(total=None, connect=10, sock_connect=10, sock_read=30)
         client_session = ClientSession(
             connector=connector,
             cookies=final_cookies,
+            timeout=timeout
         )
         return client_session
 
     def get_proxy(self) -> str:
         proxies = self.proxies
         proxy = self.proxies[randint(0, len(proxies) - 1)] if proxies else ""
         return proxy
```

### Comparing `ultima_scraper_api-1.1.0/ultima_scraper_api/models/subscription_model.py` & `ultima_scraper_api-1.1.1/ultima_scraper_api/models/subscription_model.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-1.1.0/PKG-INFO` & `ultima_scraper_api-1.1.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ultima-scraper-api
-Version: 1.1.0
+Version: 1.1.1
 Summary: 
 Author: DIGITALCRIMINALS
 Author-email: 89371864+digitalcriminals@users.noreply.github.com
 Requires-Python: >=3.10,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

