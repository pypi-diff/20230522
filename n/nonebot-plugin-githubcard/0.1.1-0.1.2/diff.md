# Comparing `tmp/nonebot_plugin_githubcard-0.1.1.tar.gz` & `tmp/nonebot_plugin_githubcard-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_githubcard-0.1.1.tar", max compression
+gzip compressed data, was "nonebot_plugin_githubcard-0.1.2.tar", max compression
```

## Comparing `nonebot_plugin_githubcard-0.1.1.tar` & `nonebot_plugin_githubcard-0.1.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1063 2023-03-16 13:13:09.152445 nonebot_plugin_githubcard-0.1.1/LICENSE
--rw-r--r--   0        0        0      741 2023-05-21 04:37:46.171345 nonebot_plugin_githubcard-0.1.1/nonebot_plugin_githubcard/__init__.py
--rw-r--r--   0        0        0      111 2023-05-21 04:37:46.171345 nonebot_plugin_githubcard-0.1.1/nonebot_plugin_githubcard/config.py
--rw-r--r--   0        0        0     1002 2023-05-21 04:37:46.171345 nonebot_plugin_githubcard-0.1.1/nonebot_plugin_githubcard/data_source.py
--rw-r--r--   0        0        0      652 2023-05-22 00:43:55.472788 nonebot_plugin_githubcard-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1440 2023-05-22 00:37:58.698833 nonebot_plugin_githubcard-0.1.1/README.md
--rw-r--r--   0        0        0     2285 1970-01-01 00:00:00.000000 nonebot_plugin_githubcard-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-03-16 13:13:09.152445 nonebot_plugin_githubcard-0.1.2/LICENSE
+-rw-r--r--   0        0        0      741 2023-05-21 04:37:46.171345 nonebot_plugin_githubcard-0.1.2/nonebot_plugin_githubcard/__init__.py
+-rw-r--r--   0        0        0      111 2023-05-21 04:37:46.171345 nonebot_plugin_githubcard-0.1.2/nonebot_plugin_githubcard/config.py
+-rw-r--r--   0        0        0     1002 2023-05-21 04:37:46.171345 nonebot_plugin_githubcard-0.1.2/nonebot_plugin_githubcard/data_source.py
+-rw-r--r--   0        0        0      692 2023-05-22 01:04:46.894632 nonebot_plugin_githubcard-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1440 2023-05-22 00:37:58.698833 nonebot_plugin_githubcard-0.1.2/README.md
+-rw-r--r--   0        0        0     2365 1970-01-01 00:00:00.000000 nonebot_plugin_githubcard-0.1.2/PKG-INFO
```

### Comparing `nonebot_plugin_githubcard-0.1.1/LICENSE` & `nonebot_plugin_githubcard-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_githubcard-0.1.1/nonebot_plugin_githubcard/__init__.py` & `nonebot_plugin_githubcard-0.1.2/nonebot_plugin_githubcard/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_githubcard-0.1.1/nonebot_plugin_githubcard/data_source.py` & `nonebot_plugin_githubcard-0.1.2/nonebot_plugin_githubcard/data_source.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_githubcard-0.1.1/pyproject.toml` & `nonebot_plugin_githubcard-0.1.2/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 [tool.poetry]
 name = "nonebot-plugin-githubcard"
-version = "0.1.1"
+version = "0.1.2"
 description = "检测GitHub仓库链接并自动发送卡片信息（适用于Onebot V11）"
 authors = ["ElainaFanBoy <demo0929@vip.qq.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/ElainaFanBoy/nonebot_plugin_githubcard"
 repository = "https://github.com/ElainaFanBoy/nonebot_plugin_githubcard"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 nonebot2 = "^2.0.0rc1"
 nonebot-adapter-onebot = "^2.1.1"
+aiohttp = "^3.7.4"
+asyncio = "^3.4.3"
 
 [tool.poetry.dev-dependencies]
 pytest = "^5.2"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `nonebot_plugin_githubcard-0.1.1/README.md` & `nonebot_plugin_githubcard-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_githubcard-0.1.1/PKG-INFO` & `nonebot_plugin_githubcard-0.1.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-githubcard
-Version: 0.1.1
+Version: 0.1.2
 Summary: 检测GitHub仓库链接并自动发送卡片信息（适用于Onebot V11）
 Home-page: https://github.com/ElainaFanBoy/nonebot_plugin_githubcard
 License: MIT
 Author: ElainaFanBoy
 Author-email: demo0929@vip.qq.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: aiohttp (>=3.7.4,<4.0.0)
+Requires-Dist: asyncio (>=3.4.3,<4.0.0)
 Requires-Dist: nonebot-adapter-onebot (>=2.1.1,<3.0.0)
 Requires-Dist: nonebot2 (>=2.0.0rc1,<3.0.0)
 Project-URL: Repository, https://github.com/ElainaFanBoy/nonebot_plugin_githubcard
 Description-Content-Type: text/markdown
 
 <div align="center">
   <a href="https://v2.nonebot.dev/store"><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/nbp_logo.png" width="180" height="180" alt="NoneBotPluginLogo"></a>
```

#### html2text {}

```diff
@@ -1,18 +1,20 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-githubcard Version: 0.1.1 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-githubcard Version: 0.1.2 Summary:
 æ£æµGitHubä»åºé¾æ¥å¹¶èªå¨åéå¡çä¿¡æ¯ï¼éç¨äºOnebot V11ï¼
 Home-page: https://github.com/ElainaFanBoy/nonebot_plugin_githubcard License:
 MIT Author: ElainaFanBoy Author-email: demo0929@vip.qq.com Requires-Python:
 >=3.8,<4.0 Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
-Python :: 3.11 Requires-Dist: nonebot-adapter-onebot (>=2.1.1,<3.0.0) Requires-
-Dist: nonebot2 (>=2.0.0rc1,<3.0.0) Project-URL: Repository, https://github.com/
-ElainaFanBoy/nonebot_plugin_githubcard Description-Content-Type: text/markdown
+Python :: 3.11 Requires-Dist: aiohttp (>=3.7.4,<4.0.0) Requires-Dist: asyncio
+(>=3.4.3,<4.0.0) Requires-Dist: nonebot-adapter-onebot (>=2.1.1,<3.0.0)
+Requires-Dist: nonebot2 (>=2.0.0rc1,<3.0.0) Project-URL: Repository, https://
+github.com/ElainaFanBoy/nonebot_plugin_githubcard Description-Content-Type:
+text/markdown
                              [NoneBotPluginLogo]
                               [NoneBotPluginText]
                        # nonebot-plugin-githubcard _â¨
      æ£æµGitHubä»åºé¾æ¥å¹¶èªå¨åéå¡çä¿¡æ¯ï¼éç¨äºOnebot
                     V11ï¼â¨_ [license][NoneBot] [python]
 ## ð ä»ç» æ£æµGitHubä»åºé¾æ¥å¹¶èªå¨åéå¡çä¿¡æ¯ ## ð¿
 å®è£  ä½¿ç¨PIPå®è£ pip install nonebot-plugin-githubcard  ## ð ä½¿ç¨
```

