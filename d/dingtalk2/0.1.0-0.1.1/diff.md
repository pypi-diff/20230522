# Comparing `tmp/dingtalk2-0.1.0.tar.gz` & `tmp/dingtalk2-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dingtalk2-0.1.0.tar", max compression
+gzip compressed data, was "dingtalk2-0.1.1.tar", max compression
```

## Comparing `dingtalk2-0.1.0.tar` & `dingtalk2-0.1.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1066 2023-04-25 16:05:24.322545 dingtalk2-0.1.0/LICENSE
--rw-r--r--   0        0        0      904 2023-04-25 16:05:24.322749 dingtalk2-0.1.0/README.md
--rw-r--r--   0        0        0      114 2023-05-22 15:07:23.625826 dingtalk2-0.1.0/dingtalk2/__init__.py
--rw-r--r--   0        0        0    11032 2023-05-22 15:14:50.042924 dingtalk2-0.1.0/dingtalk2/dingtalk.py
--rw-r--r--   0        0        0       98 2021-11-22 11:13:38.082454 dingtalk2-0.1.0/dingtalk2/exceptions.py
--rw-r--r--   0        0        0     5373 2023-05-22 15:14:59.343673 dingtalk2-0.1.0/dingtalk2/items.py
--rw-r--r--   0        0        0      298 2023-05-22 15:14:12.650930 dingtalk2-0.1.0/dingtalk2/logger.py
--rw-r--r--   0        0        0     1707 2023-05-22 15:15:17.893651 dingtalk2-0.1.0/dingtalk2/request.py
--rw-r--r--   0        0        0      419 2021-11-22 11:13:38.082852 dingtalk2-0.1.0/dingtalk2/utils.py
--rw-r--r--   0        0        0      872 2023-05-22 15:07:23.622469 dingtalk2-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1370 1970-01-01 00:00:00.000000 dingtalk2-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-04-25 16:05:24.322545 dingtalk2-0.1.1/LICENSE
+-rw-r--r--   0        0        0      904 2023-04-25 16:05:24.322749 dingtalk2-0.1.1/README.md
+-rw-r--r--   0        0        0      114 2023-05-22 15:29:39.421324 dingtalk2-0.1.1/dingtalk2/__init__.py
+-rw-r--r--   0        0        0    10480 2023-05-22 15:26:01.155034 dingtalk2-0.1.1/dingtalk2/dingtalk.py
+-rw-r--r--   0        0        0       98 2021-11-22 11:13:38.082454 dingtalk2-0.1.1/dingtalk2/exceptions.py
+-rw-r--r--   0        0        0     5373 2023-05-22 15:14:59.343673 dingtalk2-0.1.1/dingtalk2/items.py
+-rw-r--r--   0        0        0      298 2023-05-22 15:14:12.650930 dingtalk2-0.1.1/dingtalk2/logger.py
+-rw-r--r--   0        0        0     1661 2023-05-22 15:27:29.054233 dingtalk2-0.1.1/dingtalk2/request.py
+-rw-r--r--   0        0        0      419 2021-11-22 11:13:38.082852 dingtalk2-0.1.1/dingtalk2/utils.py
+-rw-r--r--   0        0        0      872 2023-05-22 15:29:39.443474 dingtalk2-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1370 1970-01-01 00:00:00.000000 dingtalk2-0.1.1/PKG-INFO
```

### Comparing `dingtalk2-0.1.0/LICENSE` & `dingtalk2-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dingtalk2-0.1.0/README.md` & `dingtalk2-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `dingtalk2-0.1.0/dingtalk2/dingtalk.py` & `dingtalk2-0.1.1/dingtalk2/dingtalk.py`

 * *Files 3% similar despite different names*

```diff
@@ -77,20 +77,19 @@
         :param at: 被@人的手机号（注意：可以在msg内容里自定义@手机号的位置，也支持同时@多个手机号，可选）
         :param at_ids: 被@人的dingtalkId（可选）
         :param auto_at: 是否自动在msg内容末尾添加@手机号，默认自动添加，可设置为False取消（可选）
         :return: 返回消息发送结果
         """
         data = {'msgtype': 'text', 'at': {}}
 
-        if is_not_null_and_blank_str(msg):
-            data['text'] = {'content': msg}
-        else:
-            logger.error('text类型，消息内容不能为空！')
+        if not is_not_null_and_blank_str(msg):
             raise ValueError('text类型，消息内容不能为空！')
 
+        data['text'] = {'content': msg}
+
         if at_all:
             data['at']['isAtAll'] = at_all
 
         if at:
             at = list(map(str, at))
             data['at']['atMobiles'] = at
 
@@ -112,15 +111,14 @@
         :return: 返回消息发送结果
         """
         if is_not_null_and_blank_str(pic_url):
             data = {'msgtype': 'image', 'image': {'picURL': pic_url}}
             logger.debug('image类型：%s' % data)
             return self._request(data)
 
-        logger.error('image类型中图片链接不能为空！')
         raise ValueError('image类型中图片链接不能为空！')
 
     def link(self, title, text, message_url, pic_url=''):
         """ link类型
         :param title: 消息标题
         :param text: 消息内容（如果太长自动省略显示）
         :param message_url: 点击消息触发的URL
@@ -138,15 +136,14 @@
                     'messageUrl': self._open_type(message_url)
                 }
             }
 
             logger.debug('link类型：%s' % data)
             return self._request(data)
 
-        logger.error('link类型中消息标题或内容或链接不能为空！')
         raise ValueError('link类型中消息标题或内容或链接不能为空！')
 
     def markdown(self, title, text, is_at_all=False, at_mobiles=None, at_dingtalk_ids=None, is_auto_at=True):
         """ markdown类型
         :param title: 首屏会话透出的展示内容
         :param text: markdown格式的消息内容
         :param is_at_all: @所有人时：true，否则为：false（可选）
@@ -180,15 +177,14 @@
             if at_dingtalk_ids:
                 at_dingtalk_ids = list(map(str, at_dingtalk_ids))
                 data['at']['atDingtalkIds'] = at_dingtalk_ids
 
             logger.debug('markdown类型：%s' % data)
             return self._request(data)
 
-        logger.error('markdown类型中消息标题或内容不能为空！')
         raise ValueError('markdown类型中消息标题或内容不能为空！')
 
     def action(self, action_card):
         """ ActionCard类型
         :param action_card: 整体跳转ActionCard类型实例或独立跳转ActionCard类型实例
         :return: 返回消息发送结果
         """
@@ -200,15 +196,14 @@
             elif 'btns' in data['actionCard']:
                 for btn in data['actionCard']['btns']:
                     btn['actionURL'] = self._open_type(btn['actionURL'])
 
             logger.debug('ActionCard类型：%s' % data)
             return self._request(data)
 
-        logger.error(f'ActionCard类型：传入的实例类型不正确，内容为：{str(action_card)}')
         raise TypeError(f'ActionCard类型：传入的实例类型不正确，内容为：{str(action_card)}')
 
     def feed(self, links):
         """ FeedCard类型
         :param links: FeedLink实例列表 or CardItem实例列表
         :return: 返回消息发送结果
         """
@@ -221,15 +216,14 @@
         for link in links:
             # 兼容：1、传入FeedLink实例列表；2、CardItem实例列表；
             if isinstance(link, FeedLink) or isinstance(link, CardItem):
                 link = link.get_data()
                 link['messageURL'] = self._open_type(link['messageURL'])
                 link_list.append(link)
             else:
-                logger.error(f'FeedLink类型，传入的数据格式不正确，内容为：{str(link)}')
                 raise ValueError(f'FeedLink类型，传入的数据格式不正确，内容为：{str(link)}')
 
         data = {'msgtype': 'feedCard', 'feedCard': {'links': link_list}}
         logger.debug('FeedCard类型：%s' % data)
 
         return self._request(data)
 
@@ -251,16 +245,14 @@
         if self.queue.full():
             elapse_time = now - self.queue.get()
             if elapse_time < 60:
                 sleep_time = int(60 - elapse_time) + 1
                 logger.debug(f'钉钉官方限制机器人每分钟最多发送20条，当前发送频率已达限制条件，休眠 {str(sleep_time)}s')
                 time.sleep(sleep_time)
 
-        logger.debug(data)
-
         return self.session.post(data)
 
     def send(self, action='text', **kwargs):
         """
         发送消息
 
         :param action:
```

### Comparing `dingtalk2-0.1.0/dingtalk2/items.py` & `dingtalk2-0.1.1/dingtalk2/items.py`

 * *Files identical despite different names*

### Comparing `dingtalk2-0.1.0/dingtalk2/request.py` & `dingtalk2-0.1.1/dingtalk2/request.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,20 +13,19 @@
     def get(self, payloads=None):
         return self.request(method='GET', data=payloads)
 
     def post(self, payloads):
         return self.request(method='POST', data=payloads)
 
     def request(self, method='GET', data: dict = None):
-        logger.warning(self.webhook)
+        logger.debug(self.webhook)
 
         try:
             response = self.session.request(method=method, url=self.webhook, headers=self.headers, json=data, params=self.options)
             response.raise_for_status()
-            logger.warning(response.json())
             return response.json()
         except requests.exceptions.HTTPError as exc:
             logger.warning(f'Error response {exc.response.status_code} while requesting {exc.request.url!r}.')
             logger.error(f'消息发送失败， HTTP error: {exc.response.status_code:d}, reason: {exc}')
             logger.exception(exc)
             return exc.response.json()
         except requests.exceptions.ConnectTimeout:
```

### Comparing `dingtalk2-0.1.0/pyproject.toml` & `dingtalk2-0.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dingtalk2"
-version = "0.1.0"
+version = "0.1.1"
 description = ""
 authors = ["bopo <ibopo@126.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 requests = "^2.28.2"
@@ -24,15 +24,15 @@
 python_files = ["tests.py", "test_*.py", "*_tests.py"]
 addopts = "-p no:warnings"
 
 log_cli = 0
 log_cli_level = "DEBUG"
 
 [tool.commitizen]
-version = "0.1.0"
+version = "0.1.1"
 tag_format = "v$version"
 
 update_changelog_on_bump = true
 changelog_file = "HISTORY.md"
 annotated_tag = true
 
 version_files = [
```

### Comparing `dingtalk2-0.1.0/PKG-INFO` & `dingtalk2-0.1.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dingtalk2
-Version: 0.1.0
+Version: 0.1.1
 Summary: 
 Author: bopo
 Author-email: ibopo@126.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

