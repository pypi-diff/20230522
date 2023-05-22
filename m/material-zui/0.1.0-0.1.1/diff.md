# Comparing `tmp/material_zui-0.1.0.tar.gz` & `tmp/material_zui-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "material_zui-0.1.0.tar", max compression
+gzip compressed data, was "material_zui-0.1.1.tar", max compression
```

## Comparing `material_zui-0.1.0.tar` & `material_zui-0.1.1.tar`

### file list

```diff
@@ -1,53 +1,79 @@
--rw-r--r--   0        0        0      822 2023-05-15 09:25:51.263824 material_zui-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      260 2023-05-01 15:33:57.972869 material_zui-0.1.0/src/material_zui/.pypirc
--rw-r--r--   0        0        0      555 2023-03-21 08:40:33.421115 material_zui-0.1.0/src/material_zui/ResizeImage.py
--rw-r--r--   0        0        0       38 2023-05-15 08:52:40.288888 material_zui-0.1.0/src/material_zui/bard/__init__.py
--rw-r--r--   0        0        0      543 2023-05-15 09:14:12.082997 material_zui-0.1.0/src/material_zui/bard/google_bard.py
--rw-r--r--   0        0        0       77 2023-05-15 09:15:57.588848 material_zui-0.1.0/src/material_zui/bard/index.py
--rw-r--r--   0        0        0       42 2023-05-07 05:09:56.400820 material_zui-0.1.0/src/material_zui/compress/__init__.py
--rw-r--r--   0        0        0       74 2023-05-07 05:16:12.115224 material_zui-0.1.0/src/material_zui/compress/index.py
--rw-r--r--   0        0        0     2131 2023-05-07 05:22:45.101162 material_zui-0.1.0/src/material_zui/compress/text.py
--rw-r--r--   0        0        0       36 2023-05-02 13:44:44.126257 material_zui-0.1.0/src/material_zui/crawl/__init__.py
--rw-r--r--   0        0        0        0 2023-05-02 13:44:44.126257 material_zui-0.1.0/src/material_zui/crawl/index.py
--rw-r--r--   0        0        0       41 2023-05-11 04:24:47.172982 material_zui-0.1.0/src/material_zui/crontab/__init__.py
--rw-r--r--   0        0        0      638 2023-05-11 04:23:06.569200 material_zui-0.1.0/src/material_zui/crontab/index.py
--rw-r--r--   0        0        0       43 2023-05-07 14:15:59.556081 material_zui-0.1.0/src/material_zui/date_time/__init__.py
--rw-r--r--   0        0        0       60 2023-05-07 14:15:59.604081 material_zui-0.1.0/src/material_zui/date_time/date_time.py
--rw-r--r--   0        0        0       49 2023-05-07 14:16:28.308295 material_zui-0.1.0/src/material_zui/date_time/index.py
--rw-r--r--   0        0        0      692 2023-05-07 14:16:10.888166 material_zui-0.1.0/src/material_zui/date_time/time.py
--rw-r--r--   0        0        0       37 2023-05-15 08:36:55.132989 material_zui-0.1.0/src/material_zui/env/__init__.py
--rw-r--r--   0        0        0      183 2023-05-15 09:09:28.356336 material_zui-0.1.0/src/material_zui/env/env.py
--rw-r--r--   0        0        0       52 2023-05-15 08:46:26.760087 material_zui-0.1.0/src/material_zui/env/index.py
--rw-r--r--   0        0        0       37 2023-05-15 08:50:53.425688 material_zui-0.1.0/src/material_zui/gpt/__init__.py
--rw-r--r--   0        0        0     1057 2023-05-15 05:15:31.650338 material_zui-0.1.0/src/material_zui/gpt/gpt_vietnam.py
--rw-r--r--   0        0        0       62 2023-05-15 08:50:53.385689 material_zui-0.1.0/src/material_zui/gpt/index.py
--rw-r--r--   0        0        0      216 2023-05-11 09:54:07.451440 material_zui-0.1.0/src/material_zui/image/__init__.py
--rw-r--r--   0        0        0     2199 2023-05-05 09:48:58.874264 material_zui-0.1.0/src/material_zui/image/colorization.py
--rw-r--r--   0        0        0     2921 2023-05-11 09:52:23.138728 material_zui-0.1.0/src/material_zui/image/combine.py
--rw-r--r--   0        0        0     5490 2023-05-11 10:24:19.669145 material_zui-0.1.0/src/material_zui/image/common.py
--rw-r--r--   0        0        0     2808 2023-05-11 10:13:26.444992 material_zui-0.1.0/src/material_zui/image/convert.py
--rw-r--r--   0        0        0       78 2023-05-06 06:26:57.697131 material_zui-0.1.0/src/material_zui/image/data.py
--rw-r--r--   0        0        0      461 2023-05-11 10:14:50.303432 material_zui-0.1.0/src/material_zui/image/index.py
--rw-r--r--   0        0        0     9945 2023-05-05 03:49:43.138352 material_zui-0.1.0/src/material_zui/image/model/colorization_deploy_v2.prototxt
--rw-r--r--   0        0        0     5088 2023-05-05 03:49:53.225773 material_zui-0.1.0/src/material_zui/image/model/pts_in_hull.npy
--rw-r--r--   0        0        0      782 2023-05-11 04:50:18.808963 material_zui-0.1.0/src/material_zui/image/remove_background.py
--rw-r--r--   0        0        0     6445 2023-05-06 08:59:41.215230 material_zui-0.1.0/src/material_zui/image/to_svg.py
--rw-r--r--   0        0        0      520 2023-05-11 09:48:54.829117 material_zui-0.1.0/src/material_zui/image/transparent_background.py
--rw-r--r--   0        0        0      249 2023-04-28 09:24:02.020353 material_zui-0.1.0/src/material_zui/image/type.py
--rw-r--r--   0        0        0     4779 2023-05-11 10:15:27.410813 material_zui-0.1.0/src/material_zui/image/upscale.py
--rw-r--r--   0        0        0       37 2023-04-30 11:48:06.179161 material_zui-0.1.0/src/material_zui/log/__init__.py
--rw-r--r--   0        0        0       83 2023-05-11 10:20:42.114888 material_zui-0.1.0/src/material_zui/log/index.py
--rw-r--r--   0        0        0      559 2023-05-11 10:19:34.415566 material_zui-0.1.0/src/material_zui/log/log.py
--rw-r--r--   0        0        0     1011 2023-05-15 09:24:15.658964 material_zui-0.1.0/src/material_zui/readme.md
--rw-r--r--   0        0        0       39 2023-05-02 05:15:13.799596 material_zui-0.1.0/src/material_zui/regex/__init__.py
--rw-r--r--   0        0        0     5344 2023-05-02 05:18:47.668155 material_zui-0.1.0/src/material_zui/regex/index.py
--rw-r--r--   0        0        0       43 2023-04-30 11:47:27.662335 material_zui-0.1.0/src/material_zui/replicate/__init__.py
--rw-r--r--   0        0        0     2481 2023-05-01 15:33:18.205379 material_zui-0.1.0/src/material_zui/replicate/index.py
--rw-r--r--   0        0        0      895 2023-05-11 10:31:29.010961 material_zui-0.1.0/src/material_zui/setup.py
--rw-r--r--   0        0        0       46 2023-05-02 13:44:38.645684 material_zui-0.1.0/src/material_zui/telegram_bot/__init__.py
--rw-r--r--   0        0        0      432 2023-05-07 05:43:32.880583 material_zui-0.1.0/src/material_zui/telegram_bot/index.py
--rw-r--r--   0        0        0       36 2023-04-30 11:48:06.223146 material_zui-0.1.0/src/material_zui/tmp/__init__.py
--rw-r--r--   0        0        0        0 2023-04-28 03:39:00.036364 material_zui-0.1.0/src/material_zui/tmp/index.py
--rw-r--r--   0        0        0       36 2023-05-01 14:11:23.375942 material_zui-0.1.0/src/material_zui/validate/__init__.py
--rw-r--r--   0        0        0        0 2023-05-01 14:11:23.379941 material_zui-0.1.0/src/material_zui/validate/index.py
--rw-r--r--   0        0        0     2022 1970-01-01 00:00:00.000000 material_zui-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1014 2023-05-22 02:20:08.172393 material_zui-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      260 2023-05-01 15:33:57.972869 material_zui-0.1.1/src/material_zui/.pypirc
+-rw-r--r--   0        0        0      555 2023-03-21 08:40:33.421115 material_zui-0.1.1/src/material_zui/ResizeImage.py
+-rw-r--r--   0        0        0       39 2023-05-21 04:19:03.692146 material_zui-0.1.1/src/material_zui/array/__init__.py
+-rw-r--r--   0        0        0      188 2023-05-21 04:22:47.696141 material_zui-0.1.1/src/material_zui/array/common.py
+-rw-r--r--   0        0        0       71 2023-05-21 04:23:10.983205 material_zui-0.1.1/src/material_zui/array/index.py
+-rw-r--r--   0        0        0     2405 2023-05-20 11:57:06.283965 material_zui-0.1.1/src/material_zui/automation/Constant.py
+-rw-r--r--   0        0        0       44 2023-05-21 02:36:24.004618 material_zui-0.1.1/src/material_zui/automation/__init__.py
+-rw-r--r--   0        0        0      110 2023-05-21 04:26:37.532312 material_zui-0.1.1/src/material_zui/automation/index.py
+-rw-r--r--   0        0        0        0 2023-05-21 02:38:12.347239 material_zui-0.1.1/src/material_zui/automation/pinterest.py
+-rw-r--r--   0        0        0     5167 2023-05-21 12:06:03.029430 material_zui-0.1.1/src/material_zui/automation/tiktok.py
+-rw-r--r--   0        0        0      310 2023-05-21 14:22:10.812226 material_zui-0.1.1/src/material_zui/automation/type.py
+-rw-r--r--   0        0        0     8776 2023-05-22 02:09:15.260250 material_zui-0.1.1/src/material_zui/automation/youtube.py
+-rw-r--r--   0        0        0       38 2023-05-15 08:52:40.288888 material_zui-0.1.1/src/material_zui/bard/__init__.py
+-rw-r--r--   0        0        0      543 2023-05-15 09:14:12.082997 material_zui-0.1.1/src/material_zui/bard/google_bard.py
+-rw-r--r--   0        0        0       77 2023-05-15 09:15:57.588848 material_zui-0.1.1/src/material_zui/bard/index.py
+-rw-r--r--   0        0        0       42 2023-05-07 05:09:56.400820 material_zui-0.1.1/src/material_zui/compress/__init__.py
+-rw-r--r--   0        0        0       74 2023-05-07 05:16:12.115224 material_zui-0.1.1/src/material_zui/compress/index.py
+-rw-r--r--   0        0        0     2131 2023-05-07 05:22:45.101162 material_zui-0.1.1/src/material_zui/compress/text.py
+-rw-r--r--   0        0        0       36 2023-05-02 13:44:44.126257 material_zui-0.1.1/src/material_zui/crawl/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-02 13:44:44.126257 material_zui-0.1.1/src/material_zui/crawl/index.py
+-rw-r--r--   0        0        0       41 2023-05-11 04:24:47.172982 material_zui-0.1.1/src/material_zui/crontab/__init__.py
+-rw-r--r--   0        0        0      638 2023-05-11 04:23:06.569200 material_zui-0.1.1/src/material_zui/crontab/index.py
+-rw-r--r--   0        0        0       43 2023-05-07 14:15:59.556081 material_zui-0.1.1/src/material_zui/date_time/__init__.py
+-rw-r--r--   0        0        0       60 2023-05-07 14:15:59.604081 material_zui-0.1.1/src/material_zui/date_time/date_time.py
+-rw-r--r--   0        0        0       49 2023-05-07 14:16:28.308295 material_zui-0.1.1/src/material_zui/date_time/index.py
+-rw-r--r--   0        0        0      692 2023-05-07 14:16:10.888166 material_zui-0.1.1/src/material_zui/date_time/time.py
+-rw-r--r--   0        0        0       36 2023-05-21 13:41:44.819759 material_zui-0.1.1/src/material_zui/dict/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-21 13:45:02.045051 material_zui-0.1.1/src/material_zui/dict/common.py
+-rw-r--r--   0        0        0        0 2023-05-21 13:41:44.819759 material_zui-0.1.1/src/material_zui/dict/index.py
+-rw-r--r--   0        0        0       37 2023-05-15 08:36:55.132989 material_zui-0.1.1/src/material_zui/env/__init__.py
+-rw-r--r--   0        0        0      183 2023-05-15 09:09:28.356336 material_zui-0.1.1/src/material_zui/env/env.py
+-rw-r--r--   0        0        0       52 2023-05-15 08:46:26.760087 material_zui-0.1.1/src/material_zui/env/index.py
+-rw-r--r--   0        0        0       38 2023-05-19 02:12:30.886319 material_zui-0.1.1/src/material_zui/fake/__init__.py
+-rw-r--r--   0        0        0       62 2023-05-19 02:24:23.295278 material_zui-0.1.1/src/material_zui/fake/index.py
+-rw-r--r--   0        0        0      254 2023-05-21 05:39:54.079978 material_zui-0.1.1/src/material_zui/fake/number.py
+-rw-r--r--   0        0        0       38 2023-05-21 03:57:08.912678 material_zui-0.1.1/src/material_zui/file/__init__.py
+-rw-r--r--   0        0        0      946 2023-05-21 13:48:05.374204 material_zui-0.1.1/src/material_zui/file/download.py
+-rw-r--r--   0        0        0       83 2023-05-21 13:48:26.988466 material_zui-0.1.1/src/material_zui/file/index.py
+-rw-r--r--   0        0        0       37 2023-05-15 08:50:53.425688 material_zui-0.1.1/src/material_zui/gpt/__init__.py
+-rw-r--r--   0        0        0     1057 2023-05-15 05:15:31.650338 material_zui-0.1.1/src/material_zui/gpt/gpt_vietnam.py
+-rw-r--r--   0        0        0       62 2023-05-15 08:50:53.385689 material_zui-0.1.1/src/material_zui/gpt/index.py
+-rw-r--r--   0        0        0      216 2023-05-11 09:54:07.451440 material_zui-0.1.1/src/material_zui/image/__init__.py
+-rw-r--r--   0        0        0     2199 2023-05-05 09:48:58.874264 material_zui-0.1.1/src/material_zui/image/colorization.py
+-rw-r--r--   0        0        0     2921 2023-05-11 09:52:23.138728 material_zui-0.1.1/src/material_zui/image/combine.py
+-rw-r--r--   0        0        0     5490 2023-05-11 10:24:19.669145 material_zui-0.1.1/src/material_zui/image/common.py
+-rw-r--r--   0        0        0     2808 2023-05-11 10:13:26.444992 material_zui-0.1.1/src/material_zui/image/convert.py
+-rw-r--r--   0        0        0       78 2023-05-06 06:26:57.697131 material_zui-0.1.1/src/material_zui/image/data.py
+-rw-r--r--   0        0        0      461 2023-05-11 10:14:50.303432 material_zui-0.1.1/src/material_zui/image/index.py
+-rw-r--r--   0        0        0     9945 2023-05-05 03:49:43.138352 material_zui-0.1.1/src/material_zui/image/model/colorization_deploy_v2.prototxt
+-rw-r--r--   0        0        0     5088 2023-05-05 03:49:53.225773 material_zui-0.1.1/src/material_zui/image/model/pts_in_hull.npy
+-rw-r--r--   0        0        0      782 2023-05-11 04:50:18.808963 material_zui-0.1.1/src/material_zui/image/remove_background.py
+-rw-r--r--   0        0        0     6445 2023-05-06 08:59:41.215230 material_zui-0.1.1/src/material_zui/image/to_svg.py
+-rw-r--r--   0        0        0      520 2023-05-11 09:48:54.829117 material_zui-0.1.1/src/material_zui/image/transparent_background.py
+-rw-r--r--   0        0        0      249 2023-04-28 09:24:02.020353 material_zui-0.1.1/src/material_zui/image/type.py
+-rw-r--r--   0        0        0     4779 2023-05-11 10:15:27.410813 material_zui-0.1.1/src/material_zui/image/upscale.py
+-rw-r--r--   0        0        0       37 2023-04-30 11:48:06.179161 material_zui-0.1.1/src/material_zui/log/__init__.py
+-rw-r--r--   0        0        0       83 2023-05-11 10:20:42.114888 material_zui-0.1.1/src/material_zui/log/index.py
+-rw-r--r--   0        0        0      559 2023-05-11 10:19:34.415566 material_zui-0.1.1/src/material_zui/log/log.py
+-rw-r--r--   0        0        0       36 2023-05-20 14:09:01.119097 material_zui-0.1.1/src/material_zui/os/__init__.py
+-rw-r--r--   0        0        0       38 2023-05-20 14:09:01.031103 material_zui-0.1.1/src/material_zui/os/index.py
+-rw-r--r--   0        0        0      188 2023-05-20 14:09:01.199091 material_zui-0.1.1/src/material_zui/os/os.py
+-rw-r--r--   0        0        0     1140 2023-05-22 02:19:02.483823 material_zui-0.1.1/src/material_zui/readme.md
+-rw-r--r--   0        0        0       39 2023-05-02 05:15:13.799596 material_zui-0.1.1/src/material_zui/regex/__init__.py
+-rw-r--r--   0        0        0     5344 2023-05-02 05:18:47.668155 material_zui-0.1.1/src/material_zui/regex/index.py
+-rw-r--r--   0        0        0       43 2023-04-30 11:47:27.662335 material_zui-0.1.1/src/material_zui/replicate/__init__.py
+-rw-r--r--   0        0        0     2481 2023-05-01 15:33:18.205379 material_zui-0.1.1/src/material_zui/replicate/index.py
+-rw-r--r--   0        0        0       42 2023-05-18 03:46:44.861073 material_zui-0.1.1/src/material_zui/selenium/__init__.py
+-rw-r--r--   0        0        0     1726 2023-05-22 02:05:38.471188 material_zui-0.1.1/src/material_zui/selenium/chrome.py
+-rw-r--r--   0        0        0      257 2023-05-22 02:03:22.582766 material_zui-0.1.1/src/material_zui/selenium/common.py
+-rw-r--r--   0        0        0      120 2023-05-22 02:03:54.393486 material_zui-0.1.1/src/material_zui/selenium/index.py
+-rw-r--r--   0        0        0      895 2023-05-11 10:31:29.010961 material_zui-0.1.1/src/material_zui/setup.py
+-rw-r--r--   0        0        0       46 2023-05-02 13:44:38.645684 material_zui-0.1.1/src/material_zui/telegram_bot/__init__.py
+-rw-r--r--   0        0        0      432 2023-05-07 05:43:32.880583 material_zui-0.1.1/src/material_zui/telegram_bot/index.py
+-rw-r--r--   0        0        0       36 2023-04-30 11:48:06.223146 material_zui-0.1.1/src/material_zui/tmp/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-28 03:39:00.036364 material_zui-0.1.1/src/material_zui/tmp/index.py
+-rw-r--r--   0        0        0       36 2023-05-01 14:11:23.375942 material_zui-0.1.1/src/material_zui/validate/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-01 14:11:23.379941 material_zui-0.1.1/src/material_zui/validate/index.py
+-rw-r--r--   0        0        0     2491 1970-01-01 00:00:00.000000 material_zui-0.1.1/PKG-INFO
```

### Comparing `material_zui-0.1.0/pyproject.toml` & `material_zui-0.1.1/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "material_zui"
-version = "0.1.0"
+version = "0.1.1"
 description = "Material Zui"
 authors = ["chauhmnguyen <chauhoangminhnguyen@gmail.com>"]
 readme = "src/material_zui/readme.md"
 keywords = [
 	"material",
 	"zui",
 	"material zui",
@@ -26,11 +26,18 @@
 pandas = "^2.0.1"
 pythonlangutil = "^0.1"
 python-crontab = "^2.7.1"
 rembg = "^2.0.36"
 pytelegrambotapi = "^4.11.0"
 bardapi = "^0.1.2"
 python-dotenv = "^1.0.0"
+youtube-uploader-selenium = "^0.1.0"
+selenium-firefox = "^2.0.7"
+selenium = "^4.9.1"
+selenium-browser = "^0.0.15"
+bot-studio = "^1.4.0"
+webdriver-manager = "^3.8.6"
+beautifulsoup4 = "^4.12.2"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `material_zui-0.1.0/src/material_zui/ResizeImage.py` & `material_zui-0.1.1/src/material_zui/ResizeImage.py`

 * *Files identical despite different names*

### Comparing `material_zui-0.1.0/src/material_zui/bard/google_bard.py` & `material_zui-0.1.1/src/material_zui/bard/google_bard.py`

 * *Files identical despite different names*

### Comparing `material_zui-0.1.0/src/material_zui/compress/text.py` & `material_zui-0.1.1/src/material_zui/compress/text.py`

 * *Files identical despite different names*

### Comparing `material_zui-0.1.0/src/material_zui/crontab/index.py` & `material_zui-0.1.1/src/material_zui/crontab/index.py`

 * *Files identical despite different names*

### Comparing `material_zui-0.1.0/src/material_zui/date_time/time.py` & `material_zui-0.1.1/src/material_zui/date_time/time.py`

 * *Files identical despite different names*

### Comparing `material_zui-0.1.0/src/material_zui/gpt/gpt_vietnam.py` & `material_zui-0.1.1/src/material_zui/gpt/gpt_vietnam.py`

 * *Files identical despite different names*

### Comparing `material_zui-0.1.0/src/material_zui/image/colorization.py` & `material_zui-0.1.1/src/material_zui/image/colorization.py`

 * *Files identical despite different names*

### Comparing `material_zui-0.1.0/src/material_zui/image/combine.py` & `material_zui-0.1.1/src/material_zui/image/combine.py`

 * *Files identical despite different names*

### Comparing `material_zui-0.1.0/src/material_zui/image/common.py` & `material_zui-0.1.1/src/material_zui/image/common.py`

 * *Files identical despite different names*

### Comparing `material_zui-0.1.0/src/material_zui/image/convert.py` & `material_zui-0.1.1/src/material_zui/image/convert.py`

 * *Files identical despite different names*

### Comparing `material_zui-0.1.0/src/material_zui/image/model/colorization_deploy_v2.prototxt` & `material_zui-0.1.1/src/material_zui/image/model/colorization_deploy_v2.prototxt`

 * *Files identical despite different names*

### Comparing `material_zui-0.1.0/src/material_zui/image/model/pts_in_hull.npy` & `material_zui-0.1.1/src/material_zui/image/model/pts_in_hull.npy`

 * *Files identical despite different names*

### Comparing `material_zui-0.1.0/src/material_zui/image/remove_background.py` & `material_zui-0.1.1/src/material_zui/image/remove_background.py`

 * *Files identical despite different names*

### Comparing `material_zui-0.1.0/src/material_zui/image/to_svg.py` & `material_zui-0.1.1/src/material_zui/image/to_svg.py`

 * *Files identical despite different names*

### Comparing `material_zui-0.1.0/src/material_zui/image/transparent_background.py` & `material_zui-0.1.1/src/material_zui/image/transparent_background.py`

 * *Files identical despite different names*

### Comparing `material_zui-0.1.0/src/material_zui/image/upscale.py` & `material_zui-0.1.1/src/material_zui/image/upscale.py`

 * *Files identical despite different names*

### Comparing `material_zui-0.1.0/src/material_zui/log/log.py` & `material_zui-0.1.1/src/material_zui/log/log.py`

 * *Files identical despite different names*

### Comparing `material_zui-0.1.0/src/material_zui/readme.md` & `material_zui-0.1.1/src/material_zui/readme.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,31 +1,38 @@
 # Modules
 
 <ol>
+  <li>array</li>
+  <li>automation</li>
   <li>bard</li>
   <li>compress</li>
   <li>crawl</li>
   <li>crontab</li>
   <li>date_time</li>
   <li>env</li>
+  <li>fake</li>
+  <li>file</li>
   <li>gpt</li>
   <li>
     image
     <ul>
       <li>grayscale</li>
       <li>colorization</li>
       <li>sketch</li>
       <li>transparent background</li>
       <li>upscale</li>
       <li>convert to jpg/png</li>
     </ul>
   </li>
-  <li><a href="#log">Log</a></li>
+  <!-- <li><a href="#log">Log</a></li> -->
+  <li>log</li>
+  <li>os</li>
   <li>regex</li>
   <li>replicate: AI Platform API</li>
+  <li>selenium</li>
   <li>telegram_bot</li>
   <li>validate</li>
 </ol>
 
 # Log
 
 - Example:
```

#### html2text {}

```diff
@@ -1,26 +1,32 @@
 # Modules
-   1. bard
-   2. compress
-   3. crawl
-   4. crontab
-   5. date_time
-   6. env
-   7. gpt
-   8. image
+   1. array
+   2. automation
+   3. bard
+   4. compress
+   5. crawl
+   6. crontab
+   7. date_time
+   8. env
+   9. fake
+  10. file
+  11. gpt
+  12. image
           o grayscale
           o colorization
           o sketch
           o transparent background
           o upscale
           o convert to jpg/png
-   9. Log
-  10. regex
-  11. replicate: AI Platform API
-  12. telegram_bot
-  13. validate
+  13. log
+  14. os
+  15. regex
+  16. replicate: AI Platform API
+  17. selenium
+  18. telegram_bot
+  19. validate
 # Log - Example: ```py from material_zui.log import debug, info, warning,
 error, critical, printTable debug('This is a debug message') info('This is an
 info message') warning('This is a warning message') error('This is an error
 message') critical('This is a critical message') printTable({ 'Name': ['Alice',
 'Bob', 'Charlie', 'Dave'], 'Age': [25, 31, 35, 19], 'Score': [85, 94, 76, 95]
 }) ```  # Package - https://pypi.org/project/material-zui
```

### Comparing `material_zui-0.1.0/src/material_zui/regex/index.py` & `material_zui-0.1.1/src/material_zui/regex/index.py`

 * *Files identical despite different names*

### Comparing `material_zui-0.1.0/src/material_zui/replicate/index.py` & `material_zui-0.1.1/src/material_zui/replicate/index.py`

 * *Files identical despite different names*

### Comparing `material_zui-0.1.0/src/material_zui/setup.py` & `material_zui-0.1.1/src/material_zui/setup.py`

 * *Files identical despite different names*

### Comparing `material_zui-0.1.0/PKG-INFO` & `material_zui-0.1.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,58 +1,72 @@
 Metadata-Version: 2.1
 Name: material-zui
-Version: 0.1.0
+Version: 0.1.1
 Summary: Material Zui
 Keywords: material,zui,material zui,zui material
 Author: chauhmnguyen
 Author-email: chauhoangminhnguyen@gmail.com
 Requires-Python: >=3.10,<3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: bardapi (>=0.1.2,<0.2.0)
+Requires-Dist: beautifulsoup4 (>=4.12.2,<5.0.0)
+Requires-Dist: bot-studio (>=1.4.0,<2.0.0)
 Requires-Dist: flask (>=2.3.2,<3.0.0)
 Requires-Dist: matplotlib (>=3.7.1,<4.0.0)
 Requires-Dist: multipledispatch (>=0.6.0,<0.7.0)
 Requires-Dist: numpy (>=1.24.3,<2.0.0)
 Requires-Dist: opencv-python (>=4.7.0.72,<5.0.0.0)
 Requires-Dist: pandas (>=2.0.1,<3.0.0)
 Requires-Dist: pillow (>=9.5.0,<10.0.0)
 Requires-Dist: pytelegrambotapi (>=4.11.0,<5.0.0)
 Requires-Dist: python-crontab (>=2.7.1,<3.0.0)
 Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
 Requires-Dist: pythonlangutil (>=0.1,<0.2)
 Requires-Dist: rembg (>=2.0.36,<3.0.0)
 Requires-Dist: replicate (>=0.8.1,<0.9.0)
 Requires-Dist: requests (>=2.30.0,<3.0.0)
+Requires-Dist: selenium (>=4.9.1,<5.0.0)
+Requires-Dist: selenium-browser (>=0.0.15,<0.0.16)
+Requires-Dist: selenium-firefox (>=2.0.7,<3.0.0)
+Requires-Dist: webdriver-manager (>=3.8.6,<4.0.0)
+Requires-Dist: youtube-uploader-selenium (>=0.1.0,<0.2.0)
 Description-Content-Type: text/markdown
 
 # Modules
 
 <ol>
+  <li>array</li>
+  <li>automation</li>
   <li>bard</li>
   <li>compress</li>
   <li>crawl</li>
   <li>crontab</li>
   <li>date_time</li>
   <li>env</li>
+  <li>fake</li>
+  <li>file</li>
   <li>gpt</li>
   <li>
     image
     <ul>
       <li>grayscale</li>
       <li>colorization</li>
       <li>sketch</li>
       <li>transparent background</li>
       <li>upscale</li>
       <li>convert to jpg/png</li>
     </ul>
   </li>
-  <li><a href="#log">Log</a></li>
+  <!-- <li><a href="#log">Log</a></li> -->
+  <li>log</li>
+  <li>os</li>
   <li>regex</li>
   <li>replicate: AI Platform API</li>
+  <li>selenium</li>
   <li>telegram_bot</li>
   <li>validate</li>
 </ol>
 
 # Log
 
 - Example:
```

#### html2text {}

```diff
@@ -1,39 +1,49 @@
-Metadata-Version: 2.1 Name: material-zui Version: 0.1.0 Summary: Material Zui
+Metadata-Version: 2.1 Name: material-zui Version: 0.1.1 Summary: Material Zui
 Keywords: material,zui,material zui,zui material Author: chauhmnguyen Author-
 email: chauhoangminhnguyen@gmail.com Requires-Python: >=3.10,<3.11 Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
-:: 3.10 Requires-Dist: bardapi (>=0.1.2,<0.2.0) Requires-Dist: flask
-(>=2.3.2,<3.0.0) Requires-Dist: matplotlib (>=3.7.1,<4.0.0) Requires-Dist:
-multipledispatch (>=0.6.0,<0.7.0) Requires-Dist: numpy (>=1.24.3,<2.0.0)
+:: 3.10 Requires-Dist: bardapi (>=0.1.2,<0.2.0) Requires-Dist: beautifulsoup4
+(>=4.12.2,<5.0.0) Requires-Dist: bot-studio (>=1.4.0,<2.0.0) Requires-Dist:
+flask (>=2.3.2,<3.0.0) Requires-Dist: matplotlib (>=3.7.1,<4.0.0) Requires-
+Dist: multipledispatch (>=0.6.0,<0.7.0) Requires-Dist: numpy (>=1.24.3,<2.0.0)
 Requires-Dist: opencv-python (>=4.7.0.72,<5.0.0.0) Requires-Dist: pandas
 (>=2.0.1,<3.0.0) Requires-Dist: pillow (>=9.5.0,<10.0.0) Requires-Dist:
 pytelegrambotapi (>=4.11.0,<5.0.0) Requires-Dist: python-crontab
 (>=2.7.1,<3.0.0) Requires-Dist: python-dotenv (>=1.0.0,<2.0.0) Requires-Dist:
 pythonlangutil (>=0.1,<0.2) Requires-Dist: rembg (>=2.0.36,<3.0.0) Requires-
 Dist: replicate (>=0.8.1,<0.9.0) Requires-Dist: requests (>=2.30.0,<3.0.0)
-Description-Content-Type: text/markdown # Modules
-   1. bard
-   2. compress
-   3. crawl
-   4. crontab
-   5. date_time
-   6. env
-   7. gpt
-   8. image
+Requires-Dist: selenium (>=4.9.1,<5.0.0) Requires-Dist: selenium-browser
+(>=0.0.15,<0.0.16) Requires-Dist: selenium-firefox (>=2.0.7,<3.0.0) Requires-
+Dist: webdriver-manager (>=3.8.6,<4.0.0) Requires-Dist: youtube-uploader-
+selenium (>=0.1.0,<0.2.0) Description-Content-Type: text/markdown # Modules
+   1. array
+   2. automation
+   3. bard
+   4. compress
+   5. crawl
+   6. crontab
+   7. date_time
+   8. env
+   9. fake
+  10. file
+  11. gpt
+  12. image
           o grayscale
           o colorization
           o sketch
           o transparent background
           o upscale
           o convert to jpg/png
-   9. Log
-  10. regex
-  11. replicate: AI Platform API
-  12. telegram_bot
-  13. validate
+  13. log
+  14. os
+  15. regex
+  16. replicate: AI Platform API
+  17. selenium
+  18. telegram_bot
+  19. validate
 # Log - Example: ```py from material_zui.log import debug, info, warning,
 error, critical, printTable debug('This is a debug message') info('This is an
 info message') warning('This is a warning message') error('This is an error
 message') critical('This is a critical message') printTable({ 'Name': ['Alice',
 'Bob', 'Charlie', 'Dave'], 'Age': [25, 31, 35, 19], 'Score': [85, 94, 76, 95]
 }) ```  # Package - https://pypi.org/project/material-zui
```

