# Comparing `tmp/nonebot_plugin_githubcard-0.1.3.tar.gz` & `tmp/nonebot_plugin_githubcard-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_githubcard-0.1.3.tar", max compression
+gzip compressed data, was "nonebot_plugin_githubcard-0.1.4.tar", max compression
```

## Comparing `nonebot_plugin_githubcard-0.1.3.tar` & `nonebot_plugin_githubcard-0.1.4.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1063 2023-03-16 13:13:09.152445 nonebot_plugin_githubcard-0.1.3/LICENSE
--rw-r--r--   0        0        0      717 2023-05-22 04:13:54.015382 nonebot_plugin_githubcard-0.1.3/nonebot_plugin_githubcard/__init__.py
--rw-r--r--   0        0        0      226 2023-05-22 06:52:59.170503 nonebot_plugin_githubcard-0.1.3/nonebot_plugin_githubcard/config.py
--rw-r--r--   0        0        0     1118 2023-05-22 09:05:58.946492 nonebot_plugin_githubcard-0.1.3/nonebot_plugin_githubcard/data_source.py
--rw-r--r--   0        0        0      672 2023-05-22 06:10:17.412992 nonebot_plugin_githubcard-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     1772 2023-05-22 05:59:58.394889 nonebot_plugin_githubcard-0.1.3/README.md
--rw-r--r--   0        0        0     2657 1970-01-01 00:00:00.000000 nonebot_plugin_githubcard-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-03-16 13:13:09.152445 nonebot_plugin_githubcard-0.1.4/LICENSE
+-rw-r--r--   0        0        0      717 2023-05-22 04:13:54.015382 nonebot_plugin_githubcard-0.1.4/nonebot_plugin_githubcard/__init__.py
+-rw-r--r--   0        0        0      272 2023-05-22 10:35:39.369190 nonebot_plugin_githubcard-0.1.4/nonebot_plugin_githubcard/config.py
+-rw-r--r--   0        0        0     1335 2023-05-22 11:01:06.788568 nonebot_plugin_githubcard-0.1.4/nonebot_plugin_githubcard/data_source.py
+-rw-r--r--   0        0        0      693 2023-05-22 10:35:34.586215 nonebot_plugin_githubcard-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     1712 2023-05-22 10:36:44.967843 nonebot_plugin_githubcard-0.1.4/README.md
+-rw-r--r--   0        0        0     2638 1970-01-01 00:00:00.000000 nonebot_plugin_githubcard-0.1.4/PKG-INFO
```

### Comparing `nonebot_plugin_githubcard-0.1.3/LICENSE` & `nonebot_plugin_githubcard-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_githubcard-0.1.3/nonebot_plugin_githubcard/__init__.py` & `nonebot_plugin_githubcard-0.1.4/nonebot_plugin_githubcard/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_githubcard-0.1.3/nonebot_plugin_githubcard/data_source.py` & `nonebot_plugin_githubcard-0.1.4/nonebot_plugin_githubcard/data_source.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,25 @@
 import aiohttp
 from .config import githubcard_config
 
 
 token = githubcard_config.github_token
 
-Headers = {"Authorization": f"Bearer {token}", "Accept": "application/vnd.github+json", "user-agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/92.0.4515.107 Safari/537.36"}
+Headers1 = {"user-agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/92.0.4515.107 Safari/537.36"}
+Headers2 = {"Authorization": f"Bearer {token}", "Accept": "application/vnd.github+json", "user-agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/92.0.4515.107 Safari/537.36"}
 
+if token is None:
+    headers=Headers1
+else:
+    headers=Headers2
 
 async def get_github_reposity_information(url: str) -> str:
     try:
         UserName, RepoName = url.replace("https://github.com/", "").split("/")
     except:
         UserName, RepoName = url.replace("github.com/", "").split("/")
     async with aiohttp.ClientSession() as session:
-        async with session.get(f"https://api.github.com/users/{UserName}", headers=Headers, timeout=5) as response:
+        async with session.get(f"https://api.github.com/users/{UserName}", headers=headers, timeout=5) as response:
             RawData = await response.json()  
             AvatarUrl = RawData["avatar_url"]
             ImageUrl = f"https://image.thum.io/get/width/1280/crop/640/viewportWidth/1280/png/noanimate/https://socialify.git.ci/{UserName}/{RepoName}/image?description=1&font=Rokkitt&language=1&name=1&owner=1&pattern=Circuit%20Board&theme=Light&logo={AvatarUrl}"
             return ImageUrl
```

### Comparing `nonebot_plugin_githubcard-0.1.3/pyproject.toml` & `nonebot_plugin_githubcard-0.1.4/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 [tool.poetry]
 name = "nonebot-plugin-githubcard"
-version = "0.1.3"
+version = "0.1.4"
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
 aiohttp = "^3.7.4"
+pydantic = "^1.5.0"
 
 [tool.poetry.dev-dependencies]
 pytest = "^5.2"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `nonebot_plugin_githubcard-0.1.3/README.md` & `nonebot_plugin_githubcard-0.1.4/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -32,23 +32,15 @@
 
 ## ⚙️ 配置
 
 在 nonebot2 项目的`.env`文件中添加下表中的必填配置
 
 | 配置项 | 必填 | 默认值 | 说明 |
 |:-----:|:----:|:----:|:----:|
-| github_token | 是 | 无 | ghp_xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx |
-
-如：
-
-```
-github_token = ghp_xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
-```
-
-
+| github_token | 否 | 无 | github_token = ghp_xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx |
 
 ## 🎉 使用
 ### 指令表
 | 指令 | 权限 | 需要@ | 说明 |
 |:-----:|:----:|:----:|:----:|
 | (https://)github.com/xxx/xxx | 所有人 | 否 | GitHub仓库链接 |
 ### 效果图
```

#### html2text {}

```diff
@@ -3,13 +3,13 @@
                        # nonebot-plugin-githubcard _â¨
      æ£æµGitHubä»åºé¾æ¥å¹¶èªå¨åéå¡çä¿¡æ¯ï¼éç¨äºOnebot
                     V11ï¼â¨_ [license][NoneBot] [python]
 ## ð ä»ç» æ£æµGitHubä»åºé¾æ¥å¹¶èªå¨åéå¡çä¿¡æ¯ ## ð¿
 å®è£  ä½¿ç¨PIPå®è£ pip install nonebot-plugin-githubcard  ## âï¸ éç½®
 å¨ nonebot2 é¡¹ç®ç`.env`æä»¶ä¸­æ·»å ä¸è¡¨ä¸­çå¿å¡«éç½® | éç½®é¡¹
 | å¿å¡« | é»è®¤å¼ | è¯´æ | |:-----:|:----:|:----:|:----:| | github_token |
-æ¯ | æ  | ghp_xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx | å¦ï¼ ``` github_token
-= ghp_xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx ``` ## ð ä½¿ç¨ ### æä»¤è¡¨ |
-æä»¤ | æé | éè¦@ | è¯´æ | |:-----:|:----:|:----:|:----:| | (https://
-)github.com/xxx/xxx | ææäºº | å¦ | GitHubä»åºé¾æ¥ | ### ææå¾
+å¦ | æ  | github_token = ghp_xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx | ## ð
+ä½¿ç¨ ### æä»¤è¡¨ | æä»¤ | æé | éè¦@ | è¯´æ | |:-----:|:----:|:--
+--:|:----:| | (https://)github.com/xxx/xxx | ææäºº | å¦ |
+GitHubä»åºé¾æ¥ | ### ææå¾
 [https://s1.vika.cn/space/2023/05/21/
 f6b1a891001346fe90ac398eb2f2f26a?attname=test.png]
```

### Comparing `nonebot_plugin_githubcard-0.1.3/PKG-INFO` & `nonebot_plugin_githubcard-0.1.4/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-githubcard
-Version: 0.1.3
+Version: 0.1.4
 Summary: 检测GitHub仓库链接并自动发送卡片信息（适用于Onebot V11）
 Home-page: https://github.com/ElainaFanBoy/nonebot_plugin_githubcard
 License: MIT
 Author: ElainaFanBoy
 Author-email: demo0929@vip.qq.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -12,14 +12,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aiohttp (>=3.7.4,<4.0.0)
 Requires-Dist: nonebot-adapter-onebot (>=2.1.1,<3.0.0)
 Requires-Dist: nonebot2 (>=2.0.0rc1,<3.0.0)
+Requires-Dist: pydantic (>=1.5.0,<2.0.0)
 Project-URL: Repository, https://github.com/ElainaFanBoy/nonebot_plugin_githubcard
 Description-Content-Type: text/markdown
 
 <div align="center">
   <a href="https://v2.nonebot.dev/store"><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/nbp_logo.png" width="180" height="180" alt="NoneBotPluginLogo"></a>
   <br>
   <p><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/NoneBotPlugin.svg" width="240" alt="NoneBotPluginText"></p>
@@ -53,23 +54,15 @@
 
 ## ⚙️ 配置
 
 在 nonebot2 项目的`.env`文件中添加下表中的必填配置
 
 | 配置项 | 必填 | 默认值 | 说明 |
 |:-----:|:----:|:----:|:----:|
-| github_token | 是 | 无 | ghp_xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx |
-
-如：
-
-```
-github_token = ghp_xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
-```
-
-
+| github_token | 否 | 无 | github_token = ghp_xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx |
 
 ## 🎉 使用
 ### 指令表
 | 指令 | 权限 | 需要@ | 说明 |
 |:-----:|:----:|:----:|:----:|
 | (https://)github.com/xxx/xxx | 所有人 | 否 | GitHub仓库链接 |
 ### 效果图
```

#### html2text {}

```diff
@@ -1,27 +1,28 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-githubcard Version: 0.1.3 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-githubcard Version: 0.1.4 Summary:
 æ£æµGitHubä»åºé¾æ¥å¹¶èªå¨åéå¡çä¿¡æ¯ï¼éç¨äºOnebot V11ï¼
 Home-page: https://github.com/ElainaFanBoy/nonebot_plugin_githubcard License:
 MIT Author: ElainaFanBoy Author-email: demo0929@vip.qq.com Requires-Python:
 >=3.8,<4.0 Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Requires-Dist: aiohttp (>=3.7.4,<4.0.0) Requires-Dist: nonebot-
 adapter-onebot (>=2.1.1,<3.0.0) Requires-Dist: nonebot2 (>=2.0.0rc1,<3.0.0)
-Project-URL: Repository, https://github.com/ElainaFanBoy/
-nonebot_plugin_githubcard Description-Content-Type: text/markdown
+Requires-Dist: pydantic (>=1.5.0,<2.0.0) Project-URL: Repository, https://
+github.com/ElainaFanBoy/nonebot_plugin_githubcard Description-Content-Type:
+text/markdown
                              [NoneBotPluginLogo]
                               [NoneBotPluginText]
                        # nonebot-plugin-githubcard _â¨
      æ£æµGitHubä»åºé¾æ¥å¹¶èªå¨åéå¡çä¿¡æ¯ï¼éç¨äºOnebot
                     V11ï¼â¨_ [license][NoneBot] [python]
 ## ð ä»ç» æ£æµGitHubä»åºé¾æ¥å¹¶èªå¨åéå¡çä¿¡æ¯ ## ð¿
 å®è£  ä½¿ç¨PIPå®è£ pip install nonebot-plugin-githubcard  ## âï¸ éç½®
 å¨ nonebot2 é¡¹ç®ç`.env`æä»¶ä¸­æ·»å ä¸è¡¨ä¸­çå¿å¡«éç½® | éç½®é¡¹
 | å¿å¡« | é»è®¤å¼ | è¯´æ | |:-----:|:----:|:----:|:----:| | github_token |
-æ¯ | æ  | ghp_xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx | å¦ï¼ ``` github_token
-= ghp_xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx ``` ## ð ä½¿ç¨ ### æä»¤è¡¨ |
-æä»¤ | æé | éè¦@ | è¯´æ | |:-----:|:----:|:----:|:----:| | (https://
-)github.com/xxx/xxx | ææäºº | å¦ | GitHubä»åºé¾æ¥ | ### ææå¾
+å¦ | æ  | github_token = ghp_xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx | ## ð
+ä½¿ç¨ ### æä»¤è¡¨ | æä»¤ | æé | éè¦@ | è¯´æ | |:-----:|:----:|:--
+--:|:----:| | (https://)github.com/xxx/xxx | ææäºº | å¦ |
+GitHubä»åºé¾æ¥ | ### ææå¾
 [https://s1.vika.cn/space/2023/05/21/
 f6b1a891001346fe90ac398eb2f2f26a?attname=test.png]
```

