# Comparing `tmp/requests_html2-1.0.4.tar.gz` & `tmp/requests_html2-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "requests_html2-1.0.4.tar", last modified: Sat May 20 17:42:09 2023, max compression
+gzip compressed data, was "requests_html2-1.0.5.tar", last modified: Mon May 22 15:08:07 2023, max compression
```

## Comparing `requests_html2-1.0.4.tar` & `requests_html2-1.0.5.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0      709 2023-05-20 14:05:30.323790 requests_html2-1.0.4/README.md
--rw-r--r--   0        0        0      706 2023-05-20 17:42:09.655456 requests_html2-1.0.4/pyproject.toml
--rw-r--r--   0        0        0    34914 2023-05-20 17:38:47.085425 requests_html2-1.0.4/requests_html2.py
--rw-r--r--   0        0        0     1265 1970-01-01 00:00:00.000000 requests_html2-1.0.4/PKG-INFO
+-rw-r--r--   0        0        0      709 2023-05-20 14:05:30.323790 requests_html2-1.0.5/README.md
+-rw-r--r--   0        0        0      706 2023-05-22 15:08:06.998629 requests_html2-1.0.5/pyproject.toml
+-rw-r--r--   0        0        0    36333 2023-05-22 15:07:20.639865 requests_html2-1.0.5/requests_html2.py
+-rw-r--r--   0        0        0     1265 1970-01-01 00:00:00.000000 requests_html2-1.0.5/PKG-INFO
```

### Comparing `requests_html2-1.0.4/README.md` & `requests_html2-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `requests_html2-1.0.4/pyproject.toml` & `requests_html2-1.0.5/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "requests_html2"
-version = "1.0.4"
+version = "1.0.5"
 description = "HTML Parsing for Humans"
 authors = [
     { name = "Bevis", email = "alonefire@foxmail.com" },
 ]
 dependencies = [
     "requests>=2.27.1",
     "pyquery>=1.4.3",
```

### Comparing `requests_html2-1.0.4/requests_html2.py` & `requests_html2-1.0.5/requests_html2.py`

 * *Files 10% similar despite different names*

```diff
@@ -891,14 +891,23 @@
 
 
 def mock_user_agent(style=None) -> _UserAgent:
     """
     生成 FakeUserAgent
     Returns an apparently legit user-agent, if not requested one of a specific
     style. Defaults to a Chrome-style User-Agent.
+    :param style:
+        -  random （默认）：随机返回用户代理字符串。
+        -  firefox ：返回自带版本信息的 Firefox 用户代理字符串。
+        -  safari ：返回自带版本信息的 Safari 用户代理字符串。
+        -  internetexplorer 或 ie ：返回自带版本信息的 Internet Explorer 用户代理字符串。
+        -  opera ：返回自带版本信息的 Opera 用户代理字符串。
+        -  chrome ：返回自带版本信息的 Chrome 用户代理字符串。
+        -  google ：返回自带版本信息的 Google（Chrome）用户代理字符串。
+        -  phantomjs ：返回自带版本信息的 PhantomJS 用户代理字符串。
     """
     global useragent
     if (not useragent) and style:
         useragent = UserAgent()
 
     return useragent[style] if style and style != "default" else DEFAULT_USER_AGENT
 
@@ -928,14 +937,22 @@
         browser_args: dict = {"headless": True, "args": ["--no-sandbox"]},
         cookies: dict = {},
         proxies: dict = {},
     ):
         """
         :param user_agent: 设置 User-Agent
         :param mock_browser_style: Mock User-Agent （set 'default' use DEFAULT_USER_AGENT）
+            -  random （默认）：随机返回用户代理字符串。
+            -  firefox ：返回自带版本信息的 Firefox 用户代理字符串。
+            -  safari ：返回自带版本信息的 Safari 用户代理字符串。
+            -  internetexplorer 或 ie ：返回自带版本信息的 Internet Explorer 用户代理字符串。
+            -  opera ：返回自带版本信息的 Opera 用户代理字符串。
+            -  chrome ：返回自带版本信息的 Chrome 用户代理字符串。
+            -  google ：返回自带版本信息的 Google（Chrome）用户代理字符串。
+            -  phantomjs ：返回自带版本信息的 PhantomJS 用户代理字符串。
         :param verify: 控制是否验证证书
         :param browser_args: 浏览器初始化参数
             -  headless ：设置是否为无头模式，默认为  True 。
             -  defaultViewport：设置默认窗口大小
             -  args ：设置 Chrome 启动时的参数列表，传入一个 List。
             -  executablePath ：设置可执行文件的路径。
             -  slowMo ：将操作延迟指定毫秒数，用于调试。
@@ -946,15 +963,15 @@
         :param proxies: 设置代理
         """
         super().__init__()
 
         # Mock a web browser's user agent.
 
         if mock_browser_style:
-            self.headers["User-Agent"] = user_agent(mock_browser_style)
+            self.headers["User-Agent"] = mock_user_agent(mock_browser_style)
 
         if user_agent:
             self.headers["User-Agent"] = user_agent
 
         if cookies:
             self.cookies = cookiejar_from_dict(cookies)
```

### Comparing `requests_html2-1.0.4/PKG-INFO` & `requests_html2-1.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: requests-html2
-Version: 1.0.4
+Version: 1.0.5
 Summary: HTML Parsing for Humans
 Author-Email: Bevis <alonefire@foxmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/AloneFire/requests_html2
 Project-URL: Bug tracker, https://github.com/AloneFire/requests_html2
 Requires-Python: >=3.7
 Requires-Dist: requests>=2.27.1
```

