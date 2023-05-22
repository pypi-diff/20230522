# Comparing `tmp/nonebot_plugin_githubcard-0.1.0.tar.gz` & `tmp/nonebot_plugin_githubcard-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_githubcard-0.1.0.tar", max compression
+gzip compressed data, was "nonebot_plugin_githubcard-0.1.1.tar", max compression
```

## Comparing `nonebot_plugin_githubcard-0.1.0.tar` & `nonebot_plugin_githubcard-0.1.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1063 2023-03-16 13:13:09.152445 nonebot_plugin_githubcard-0.1.0/LICENSE
--rw-r--r--   0        0        0      741 2023-05-21 04:37:46.171345 nonebot_plugin_githubcard-0.1.0/nonebot_plugin_githubcard/__init__.py
--rw-r--r--   0        0        0      111 2023-05-21 04:37:46.171345 nonebot_plugin_githubcard-0.1.0/nonebot_plugin_githubcard/config.py
--rw-r--r--   0        0        0     1002 2023-05-21 04:37:46.171345 nonebot_plugin_githubcard-0.1.0/nonebot_plugin_githubcard/data_source.py
--rw-r--r--   0        0        0      654 2023-05-21 05:02:39.711872 nonebot_plugin_githubcard-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1442 2023-05-21 05:02:55.461238 nonebot_plugin_githubcard-0.1.0/README.md
--rw-r--r--   0        0        0     2289 1970-01-01 00:00:00.000000 nonebot_plugin_githubcard-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-03-16 13:13:09.152445 nonebot_plugin_githubcard-0.1.1/LICENSE
+-rw-r--r--   0        0        0      741 2023-05-21 04:37:46.171345 nonebot_plugin_githubcard-0.1.1/nonebot_plugin_githubcard/__init__.py
+-rw-r--r--   0        0        0      111 2023-05-21 04:37:46.171345 nonebot_plugin_githubcard-0.1.1/nonebot_plugin_githubcard/config.py
+-rw-r--r--   0        0        0     1002 2023-05-21 04:37:46.171345 nonebot_plugin_githubcard-0.1.1/nonebot_plugin_githubcard/data_source.py
+-rw-r--r--   0        0        0      652 2023-05-22 00:43:55.472788 nonebot_plugin_githubcard-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1440 2023-05-22 00:37:58.698833 nonebot_plugin_githubcard-0.1.1/README.md
+-rw-r--r--   0        0        0     2285 1970-01-01 00:00:00.000000 nonebot_plugin_githubcard-0.1.1/PKG-INFO
```

### Comparing `nonebot_plugin_githubcard-0.1.0/LICENSE` & `nonebot_plugin_githubcard-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_githubcard-0.1.0/nonebot_plugin_githubcard/__init__.py` & `nonebot_plugin_githubcard-0.1.1/nonebot_plugin_githubcard/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_githubcard-0.1.0/nonebot_plugin_githubcard/data_source.py` & `nonebot_plugin_githubcard-0.1.1/nonebot_plugin_githubcard/data_source.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_githubcard-0.1.0/pyproject.toml` & `nonebot_plugin_githubcard-0.1.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "nonebot-plugin-githubcard"
-version = "0.1.0"
-description = "检测GitHub仓库链接并自动发送卡片信息（适用于Nonebot2 V11）"
+version = "0.1.1"
+description = "检测GitHub仓库链接并自动发送卡片信息（适用于Onebot V11）"
 authors = ["ElainaFanBoy <demo0929@vip.qq.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/ElainaFanBoy/nonebot_plugin_githubcard"
 repository = "https://github.com/ElainaFanBoy/nonebot_plugin_githubcard"
 
 [tool.poetry.dependencies]
```

### Comparing `nonebot_plugin_githubcard-0.1.0/README.md` & `nonebot_plugin_githubcard-0.1.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   <p><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/NoneBotPlugin.svg" width="240" alt="NoneBotPluginText"></p>
 </div>
 
 <div align="center">
 
 # nonebot-plugin-githubcard
 
-_✨ 检测GitHub仓库链接并自动发送卡片信息（适用于Nonebot2 V11）✨_
+_✨ 检测GitHub仓库链接并自动发送卡片信息（适用于Onebot V11）✨_
 
 <a href="./LICENSE">
     <img src="https://camo.githubusercontent.com/6849e28a50157229c6a1426570610ecbe589c68bd7c806f4f7513d7265db8cf2/68747470733a2f2f696d672e736869656c64732e696f2f6769746875622f6c6963656e73652f6e6f6e65706c7567696e2f6e6f6e65626f742d706c7567696e2d706574706574" alt="license">
 </a><img src="https://img.shields.io/badge/nonebot-2.0.0rc1+-red.svg" alt="NoneBot">
 <img src="https://img.shields.io/badge/python-3.8+-blue.svg" alt="python">
 
 </div>
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
                              [NoneBotPluginLogo]
                               [NoneBotPluginText]
                        # nonebot-plugin-githubcard _â¨
-    æ£æµGitHubä»åºé¾æ¥å¹¶èªå¨åéå¡çä¿¡æ¯ï¼éç¨äºNonebot2
+     æ£æµGitHubä»åºé¾æ¥å¹¶èªå¨åéå¡çä¿¡æ¯ï¼éç¨äºOnebot
                     V11ï¼â¨_ [license][NoneBot] [python]
 ## ð ä»ç» æ£æµGitHubä»åºé¾æ¥å¹¶èªå¨åéå¡çä¿¡æ¯ ## ð¿
 å®è£  ä½¿ç¨PIPå®è£ pip install nonebot-plugin-githubcard  ## ð ä½¿ç¨
 ### æä»¤è¡¨ | æä»¤ | æé | éè¦@ | èå´ | |:-----:|:----:|:----:|:--
 --:| | GitHubä»åºé¾æ¥ | ææäºº | å¦ | ç¾¤è | ### ææå¾
 [https://s1.vika.cn/space/2023/05/21/
 f6b1a891001346fe90ac398eb2f2f26a?attname=test.png]
```

### Comparing `nonebot_plugin_githubcard-0.1.0/PKG-INFO` & `nonebot_plugin_githubcard-0.1.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-githubcard
-Version: 0.1.0
-Summary: 检测GitHub仓库链接并自动发送卡片信息（适用于Nonebot2 V11）
+Version: 0.1.1
+Summary: 检测GitHub仓库链接并自动发送卡片信息（适用于Onebot V11）
 Home-page: https://github.com/ElainaFanBoy/nonebot_plugin_githubcard
 License: MIT
 Author: ElainaFanBoy
 Author-email: demo0929@vip.qq.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -24,15 +24,15 @@
   <p><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/NoneBotPlugin.svg" width="240" alt="NoneBotPluginText"></p>
 </div>
 
 <div align="center">
 
 # nonebot-plugin-githubcard
 
-_✨ 检测GitHub仓库链接并自动发送卡片信息（适用于Nonebot2 V11）✨_
+_✨ 检测GitHub仓库链接并自动发送卡片信息（适用于Onebot V11）✨_
 
 <a href="./LICENSE">
     <img src="https://camo.githubusercontent.com/6849e28a50157229c6a1426570610ecbe589c68bd7c806f4f7513d7265db8cf2/68747470733a2f2f696d672e736869656c64732e696f2f6769746875622f6c6963656e73652f6e6f6e65706c7567696e2f6e6f6e65626f742d706c7567696e2d706574706574" alt="license">
 </a><img src="https://img.shields.io/badge/nonebot-2.0.0rc1+-red.svg" alt="NoneBot">
 <img src="https://img.shields.io/badge/python-3.8+-blue.svg" alt="python">
 
 </div>
```

#### html2text {}

```diff
@@ -1,22 +1,22 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-githubcard Version: 0.1.0 Summary:
-æ£æµGitHubä»åºé¾æ¥å¹¶èªå¨åéå¡çä¿¡æ¯ï¼éç¨äºNonebot2 V11ï¼
+Metadata-Version: 2.1 Name: nonebot-plugin-githubcard Version: 0.1.1 Summary:
+æ£æµGitHubä»åºé¾æ¥å¹¶èªå¨åéå¡çä¿¡æ¯ï¼éç¨äºOnebot V11ï¼
 Home-page: https://github.com/ElainaFanBoy/nonebot_plugin_githubcard License:
 MIT Author: ElainaFanBoy Author-email: demo0929@vip.qq.com Requires-Python:
 >=3.8,<4.0 Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Requires-Dist: nonebot-adapter-onebot (>=2.1.1,<3.0.0) Requires-
 Dist: nonebot2 (>=2.0.0rc1,<3.0.0) Project-URL: Repository, https://github.com/
 ElainaFanBoy/nonebot_plugin_githubcard Description-Content-Type: text/markdown
                              [NoneBotPluginLogo]
                               [NoneBotPluginText]
                        # nonebot-plugin-githubcard _â¨
-    æ£æµGitHubä»åºé¾æ¥å¹¶èªå¨åéå¡çä¿¡æ¯ï¼éç¨äºNonebot2
+     æ£æµGitHubä»åºé¾æ¥å¹¶èªå¨åéå¡çä¿¡æ¯ï¼éç¨äºOnebot
                     V11ï¼â¨_ [license][NoneBot] [python]
 ## ð ä»ç» æ£æµGitHubä»åºé¾æ¥å¹¶èªå¨åéå¡çä¿¡æ¯ ## ð¿
 å®è£  ä½¿ç¨PIPå®è£ pip install nonebot-plugin-githubcard  ## ð ä½¿ç¨
 ### æä»¤è¡¨ | æä»¤ | æé | éè¦@ | èå´ | |:-----:|:----:|:----:|:--
 --:| | GitHubä»åºé¾æ¥ | ææäºº | å¦ | ç¾¤è | ### ææå¾
 [https://s1.vika.cn/space/2023/05/21/
 f6b1a891001346fe90ac398eb2f2f26a?attname=test.png]
```

