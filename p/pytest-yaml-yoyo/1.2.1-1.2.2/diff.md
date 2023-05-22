# Comparing `tmp/pytest-yaml-yoyo-1.2.1.tar.gz` & `tmp/pytest-yaml-yoyo-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\pytest-yaml-yoyo-1.2.1.tar", last modified: Fri May 19 16:30:43 2023, max compression
+gzip compressed data, was "dist\pytest-yaml-yoyo-1.2.2.tar", last modified: Mon May 22 13:47:58 2023, max compression
```

## Comparing `pytest-yaml-yoyo-1.2.1.tar` & `pytest-yaml-yoyo-1.2.2.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxrwx   0        0        0        0 2023-05-19 16:30:42.997769 pytest-yaml-yoyo-1.2.1/
--rw-rw-rw-   0        0        0    23645 2023-05-19 16:30:42.997769 pytest-yaml-yoyo-1.2.1/PKG-INFO
--rw-rw-rw-   0        0        0    23146 2023-05-19 16:29:16.000000 pytest-yaml-yoyo-1.2.1/README.rst
--rw-rw-rw-   0        0        0       42 2023-05-19 16:30:42.997769 pytest-yaml-yoyo-1.2.1/setup.cfg
--rw-rw-rw-   0        0        0     1347 2023-05-19 16:29:16.000000 pytest-yaml-yoyo-1.2.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-19 16:30:42.963861 pytest-yaml-yoyo-1.2.1/src/
-drwxrwxrwx   0        0        0        0 2023-05-19 16:30:42.987797 pytest-yaml-yoyo-1.2.1/src/pytest_yaml_yoyo/
--rw-rw-rw-   0        0        0        0 2022-11-23 03:54:21.000000 pytest-yaml-yoyo-1.2.1/src/pytest_yaml_yoyo/__init__.py
--rw-rw-rw-   0        0        0     2874 2023-05-19 16:11:50.000000 pytest-yaml-yoyo-1.2.1/src/pytest_yaml_yoyo/create_funtion.py
--rw-rw-rw-   0        0        0     2057 2023-05-19 16:11:50.000000 pytest-yaml-yoyo-1.2.1/src/pytest_yaml_yoyo/db.py
--rw-rw-rw-   0        0        0      238 2023-05-19 16:11:50.000000 pytest-yaml-yoyo-1.2.1/src/pytest_yaml_yoyo/exceptions.py
--rw-rw-rw-   0        0        0     3741 2023-05-19 16:11:50.000000 pytest-yaml-yoyo-1.2.1/src/pytest_yaml_yoyo/extract.py
--rw-rw-rw-   0        0        0     2059 2023-05-19 16:11:50.000000 pytest-yaml-yoyo-1.2.1/src/pytest_yaml_yoyo/http_session.py
--rw-rw-rw-   0        0        0     2431 2023-05-19 16:11:50.000000 pytest-yaml-yoyo-1.2.1/src/pytest_yaml_yoyo/log.py
--rw-rw-rw-   0        0        0     2734 2023-05-19 16:25:21.000000 pytest-yaml-yoyo-1.2.1/src/pytest_yaml_yoyo/my_builtins.py
--rw-rw-rw-   0        0        0        0 2023-05-19 16:11:50.000000 pytest-yaml-yoyo-1.2.1/src/pytest_yaml_yoyo/parser.py
--rw-rw-rw-   0        0        0     9257 2023-05-19 16:11:50.000000 pytest-yaml-yoyo-1.2.1/src/pytest_yaml_yoyo/plugin.py
--rw-rw-rw-   0        0        0     4966 2023-05-19 16:25:21.000000 pytest-yaml-yoyo-1.2.1/src/pytest_yaml_yoyo/render_template_obj.py
--rw-rw-rw-   0        0        0     1854 2023-05-19 16:11:50.000000 pytest-yaml-yoyo-1.2.1/src/pytest_yaml_yoyo/report_notify.py
--rw-rw-rw-   0        0        0     1447 2023-05-19 16:11:50.000000 pytest-yaml-yoyo-1.2.1/src/pytest_yaml_yoyo/request_session.py
--rw-rw-rw-   0        0        0    28442 2023-05-19 16:19:35.000000 pytest-yaml-yoyo-1.2.1/src/pytest_yaml_yoyo/runner.py
--rw-rw-rw-   0        0        0     7722 2023-05-19 16:11:50.000000 pytest-yaml-yoyo-1.2.1/src/pytest_yaml_yoyo/swagger_parser.py
--rw-rw-rw-   0        0        0     3524 2023-05-19 16:11:50.000000 pytest-yaml-yoyo-1.2.1/src/pytest_yaml_yoyo/validate.py
-drwxrwxrwx   0        0        0        0 2023-05-19 16:30:42.995775 pytest-yaml-yoyo-1.2.1/src/pytest_yaml_yoyo.egg-info/
--rw-rw-rw-   0        0        0    23645 2023-05-19 16:30:42.000000 pytest-yaml-yoyo-1.2.1/src/pytest_yaml_yoyo.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      839 2023-05-19 16:30:42.000000 pytest-yaml-yoyo-1.2.1/src/pytest_yaml_yoyo.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-19 16:30:42.000000 pytest-yaml-yoyo-1.2.1/src/pytest_yaml_yoyo.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       54 2023-05-19 16:30:42.000000 pytest-yaml-yoyo-1.2.1/src/pytest_yaml_yoyo.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      188 2023-05-19 16:30:42.000000 pytest-yaml-yoyo-1.2.1/src/pytest_yaml_yoyo.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-05-19 16:30:42.000000 pytest-yaml-yoyo-1.2.1/src/pytest_yaml_yoyo.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-22 13:47:58.045463 pytest-yaml-yoyo-1.2.2/
+-rw-rw-rw-   0        0        0    23692 2023-05-22 13:47:58.044494 pytest-yaml-yoyo-1.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0    23193 2023-05-20 01:43:47.000000 pytest-yaml-yoyo-1.2.2/README.rst
+-rw-rw-rw-   0        0        0       42 2023-05-22 13:47:58.045463 pytest-yaml-yoyo-1.2.2/setup.cfg
+-rw-rw-rw-   0        0        0     1347 2023-05-22 13:47:47.000000 pytest-yaml-yoyo-1.2.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-22 13:47:57.809317 pytest-yaml-yoyo-1.2.2/src/
+drwxrwxrwx   0        0        0        0 2023-05-22 13:47:58.011555 pytest-yaml-yoyo-1.2.2/src/pytest_yaml_yoyo/
+-rw-rw-rw-   0        0        0        0 2022-11-23 03:54:21.000000 pytest-yaml-yoyo-1.2.2/src/pytest_yaml_yoyo/__init__.py
+-rw-rw-rw-   0        0        0     2874 2023-05-19 16:11:50.000000 pytest-yaml-yoyo-1.2.2/src/pytest_yaml_yoyo/create_funtion.py
+-rw-rw-rw-   0        0        0     2057 2023-05-19 16:11:50.000000 pytest-yaml-yoyo-1.2.2/src/pytest_yaml_yoyo/db.py
+-rw-rw-rw-   0        0        0      238 2023-05-19 16:11:50.000000 pytest-yaml-yoyo-1.2.2/src/pytest_yaml_yoyo/exceptions.py
+-rw-rw-rw-   0        0        0     3741 2023-05-19 16:11:50.000000 pytest-yaml-yoyo-1.2.2/src/pytest_yaml_yoyo/extract.py
+-rw-rw-rw-   0        0        0     2059 2023-05-19 16:11:50.000000 pytest-yaml-yoyo-1.2.2/src/pytest_yaml_yoyo/http_session.py
+-rw-rw-rw-   0        0        0     2431 2023-05-19 16:11:50.000000 pytest-yaml-yoyo-1.2.2/src/pytest_yaml_yoyo/log.py
+-rw-rw-rw-   0        0        0     2734 2023-05-19 16:25:21.000000 pytest-yaml-yoyo-1.2.2/src/pytest_yaml_yoyo/my_builtins.py
+-rw-rw-rw-   0        0        0        0 2023-05-19 16:11:50.000000 pytest-yaml-yoyo-1.2.2/src/pytest_yaml_yoyo/parser.py
+-rw-rw-rw-   0        0        0     9329 2023-05-22 13:47:16.000000 pytest-yaml-yoyo-1.2.2/src/pytest_yaml_yoyo/plugin.py
+-rw-rw-rw-   0        0        0     4966 2023-05-19 16:25:21.000000 pytest-yaml-yoyo-1.2.2/src/pytest_yaml_yoyo/render_template_obj.py
+-rw-rw-rw-   0        0        0     1854 2023-05-19 16:11:50.000000 pytest-yaml-yoyo-1.2.2/src/pytest_yaml_yoyo/report_notify.py
+-rw-rw-rw-   0        0        0     1447 2023-05-19 16:11:50.000000 pytest-yaml-yoyo-1.2.2/src/pytest_yaml_yoyo/request_session.py
+-rw-rw-rw-   0        0        0    28442 2023-05-19 16:19:35.000000 pytest-yaml-yoyo-1.2.2/src/pytest_yaml_yoyo/runner.py
+-rw-rw-rw-   0        0        0     7722 2023-05-19 16:11:50.000000 pytest-yaml-yoyo-1.2.2/src/pytest_yaml_yoyo/swagger_parser.py
+-rw-rw-rw-   0        0        0     3666 2023-05-22 13:47:47.000000 pytest-yaml-yoyo-1.2.2/src/pytest_yaml_yoyo/validate.py
+drwxrwxrwx   0        0        0        0 2023-05-22 13:47:58.042499 pytest-yaml-yoyo-1.2.2/src/pytest_yaml_yoyo.egg-info/
+-rw-rw-rw-   0        0        0    23692 2023-05-22 13:47:57.000000 pytest-yaml-yoyo-1.2.2/src/pytest_yaml_yoyo.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      839 2023-05-22 13:47:57.000000 pytest-yaml-yoyo-1.2.2/src/pytest_yaml_yoyo.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-22 13:47:57.000000 pytest-yaml-yoyo-1.2.2/src/pytest_yaml_yoyo.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       54 2023-05-22 13:47:57.000000 pytest-yaml-yoyo-1.2.2/src/pytest_yaml_yoyo.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      188 2023-05-22 13:47:57.000000 pytest-yaml-yoyo-1.2.2/src/pytest_yaml_yoyo.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-05-22 13:47:57.000000 pytest-yaml-yoyo-1.2.2/src/pytest_yaml_yoyo.egg-info/top_level.txt
```

### Comparing `pytest-yaml-yoyo-1.2.1/PKG-INFO` & `pytest-yaml-yoyo-1.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-yaml-yoyo
-Version: 1.2.1
+Version: 1.2.2
 Summary: http/https API run by yaml
 Home-page: https://github.com/yoyoketang/pytest-yaml-yoyo
 Author: 上海-悠悠
 Author-email: 283340479@qq.com
 License: proprietary
 Keywords: pytest,py.test,pytest-yaml,pytest-yaml-yoyo
 Classifier: Framework :: Pytest
@@ -132,45 +132,51 @@
 v1.1.3 发布时间 2022.12.17
 
 - 文件上传multipart/form-data 格式支持
 
 v1.1.4 发布时间 2023.2.13
 
 新增3个关键字
+
 - 1.sleep  添加用例之间的sleep 等待时间
 - 2.skip   跳过用例功能
 - 3.skipif   条件为真时跳过用例
 
 v1.1.5 发布时间 2023.2.16
 
 支持 2 中方式生成 yaml 用例
+
 - 1.本地 swagger.json 文件
 - 2.在线 swagger.json 地址
 
 v1.1.8 发布时间 2023.3.17
 
 int 转 str 类型
 
 v1.1.9 发布时间 2023-03-21
 
 做了以下优化
+
 - 1.validate 校验加了text 关键字获取全部body文本内容
 - 2.用例分层 api和 testcase 层 validate 校验优化，解决之前遗留的bug
 - 3.validate 校验方式更灵活，支持int类型校验字符长度和包含字符
 - 4.log 日志文件优化，只保留最近的5个日志文件
 
 v1.2.0 发布时间 2023-05-08
 
 优化以下问题
+
 - 1.断言的时候 None 和 'None' 可以判断是相等，在yaml中可以写null 或者 None, 不区分类型了
 - 2.添加局部变量variables
 - 3.优化request 下的hook 功能
 - 4.其它细节优化
 
-v1.2.1 发布
+v1.2.1 发布时间 2023-05-20
+
+优化以下问题
 
 1.兼容python3.8, python3.9, python3.10版本
 2.支持在case 用例中针对单个用例的参数化了
 3.参数化数据支持读取外部文件，文件格式可以支持：txt/csv/json/yaml
 4.函数的参数可以引用变量了，如: ${fun("hello ${key}")}
 5.内置to_json() 函数，字典转 json
```

### Comparing `pytest-yaml-yoyo-1.2.1/README.rst` & `pytest-yaml-yoyo-1.2.2/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -117,45 +117,51 @@
 v1.1.3 发布时间 2022.12.17
 
 - 文件上传multipart/form-data 格式支持
 
 v1.1.4 发布时间 2023.2.13
 
 新增3个关键字
+
 - 1.sleep  添加用例之间的sleep 等待时间
 - 2.skip   跳过用例功能
 - 3.skipif   条件为真时跳过用例
 
 v1.1.5 发布时间 2023.2.16
 
 支持 2 中方式生成 yaml 用例
+
 - 1.本地 swagger.json 文件
 - 2.在线 swagger.json 地址
 
 v1.1.8 发布时间 2023.3.17
 
 int 转 str 类型
 
 v1.1.9 发布时间 2023-03-21
 
 做了以下优化
+
 - 1.validate 校验加了text 关键字获取全部body文本内容
 - 2.用例分层 api和 testcase 层 validate 校验优化，解决之前遗留的bug
 - 3.validate 校验方式更灵活，支持int类型校验字符长度和包含字符
 - 4.log 日志文件优化，只保留最近的5个日志文件
 
 v1.2.0 发布时间 2023-05-08
 
 优化以下问题
+
 - 1.断言的时候 None 和 'None' 可以判断是相等，在yaml中可以写null 或者 None, 不区分类型了
 - 2.添加局部变量variables
 - 3.优化request 下的hook 功能
 - 4.其它细节优化
 
-v1.2.1 发布
+v1.2.1 发布时间 2023-05-20
+
+优化以下问题
 
 1.兼容python3.8, python3.9, python3.10版本
 2.支持在case 用例中针对单个用例的参数化了
 3.参数化数据支持读取外部文件，文件格式可以支持：txt/csv/json/yaml
 4.函数的参数可以引用变量了，如: ${fun("hello ${key}")}
 5.内置to_json() 函数，字典转 json
```

### Comparing `pytest-yaml-yoyo-1.2.1/setup.py` & `pytest-yaml-yoyo-1.2.2/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # 作者-上海悠悠 微信wx:283340479
 # blog地址 https://www.cnblogs.com/yoyoketang/
 """
 
 setup(
     name='pytest-yaml-yoyo',
     url='https://github.com/yoyoketang/pytest-yaml-yoyo',
-    version='v1.2.1',
+    version='v1.2.2',
     author="上海-悠悠",
     author_email='283340479@qq.com',
     description='http/https API run by yaml',
     long_description=open("README.rst", encoding='utf-8').read(),
     package_dir={"": "src"},
     packages=["pytest_yaml_yoyo"],
     classifiers=[
@@ -28,15 +28,15 @@
     python_requires=">=3.8",
     install_requires=[
         'Jinja2>=3.1.2',
         'jmespath>=0.9.5',
         'jsonpath>=0.82',
         'pytest>=7.2.0',
         'PyYAML>=6.0',
-        'requests>=2.18.4',
+        'requests>=2.28.1',
         'allure-pytest>=2.12.0',
         'pymysql>=1.0.2',
         'DingtalkChatbot>=1.5.7',
         'Faker>=15.3.4',
         'requests_toolbelt>=0.10.1',
     ],
     entry_points={
```

### Comparing `pytest-yaml-yoyo-1.2.1/src/pytest_yaml_yoyo/create_funtion.py` & `pytest-yaml-yoyo-1.2.2/src/pytest_yaml_yoyo/create_funtion.py`

 * *Files identical despite different names*

### Comparing `pytest-yaml-yoyo-1.2.1/src/pytest_yaml_yoyo/db.py` & `pytest-yaml-yoyo-1.2.2/src/pytest_yaml_yoyo/db.py`

 * *Files identical despite different names*

### Comparing `pytest-yaml-yoyo-1.2.1/src/pytest_yaml_yoyo/extract.py` & `pytest-yaml-yoyo-1.2.2/src/pytest_yaml_yoyo/extract.py`

 * *Files identical despite different names*

### Comparing `pytest-yaml-yoyo-1.2.1/src/pytest_yaml_yoyo/http_session.py` & `pytest-yaml-yoyo-1.2.2/src/pytest_yaml_yoyo/http_session.py`

 * *Files identical despite different names*

### Comparing `pytest-yaml-yoyo-1.2.1/src/pytest_yaml_yoyo/log.py` & `pytest-yaml-yoyo-1.2.2/src/pytest_yaml_yoyo/log.py`

 * *Files identical despite different names*

### Comparing `pytest-yaml-yoyo-1.2.1/src/pytest_yaml_yoyo/my_builtins.py` & `pytest-yaml-yoyo-1.2.2/src/pytest_yaml_yoyo/my_builtins.py`

 * *Files identical despite different names*

### Comparing `pytest-yaml-yoyo-1.2.1/src/pytest_yaml_yoyo/plugin.py` & `pytest-yaml-yoyo-1.2.2/src/pytest_yaml_yoyo/plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -132,21 +132,22 @@
 def pytest_addoption(parser):   # noqa
     # run env
     parser.addini('env', default=None, help='run environment by test or uat ...')
     parser.addoption(
         "--env", action="store", default=None, help="run environment by test or uat ..."
     )
     # base url
-    parser.addini("base_url", help="base url for the api test.")
-    parser.addoption(
-        "--base-url",
-        metavar="url",
-        default=os.getenv("PYTEST_BASE_URL", None),
-        help="base url for the api test.",
-    )
+    if 'base_url' not in parser._ininames:
+        parser.addini("base_url", help="base url for the api test.")
+        parser.addoption(
+            "--base-url",
+            metavar="url",
+            default=os.getenv("PYTEST_BASE_URL", None),
+            help="base url for the api test.",
+        )
     # proxies_ip
     parser.addini("proxies_ip", default=None, help="proxies_ip for the  test.")
     parser.addoption(
         "--proxies-ip",
         action="store", default=None,
         help="proxies_ip for the  test.",
     )
```

### Comparing `pytest-yaml-yoyo-1.2.1/src/pytest_yaml_yoyo/render_template_obj.py` & `pytest-yaml-yoyo-1.2.2/src/pytest_yaml_yoyo/render_template_obj.py`

 * *Files identical despite different names*

### Comparing `pytest-yaml-yoyo-1.2.1/src/pytest_yaml_yoyo/report_notify.py` & `pytest-yaml-yoyo-1.2.2/src/pytest_yaml_yoyo/report_notify.py`

 * *Files identical despite different names*

### Comparing `pytest-yaml-yoyo-1.2.1/src/pytest_yaml_yoyo/request_session.py` & `pytest-yaml-yoyo-1.2.2/src/pytest_yaml_yoyo/request_session.py`

 * *Files identical despite different names*

### Comparing `pytest-yaml-yoyo-1.2.1/src/pytest_yaml_yoyo/runner.py` & `pytest-yaml-yoyo-1.2.2/src/pytest_yaml_yoyo/runner.py`

 * *Files identical despite different names*

### Comparing `pytest-yaml-yoyo-1.2.1/src/pytest_yaml_yoyo/swagger_parser.py` & `pytest-yaml-yoyo-1.2.2/src/pytest_yaml_yoyo/swagger_parser.py`

 * *Files identical despite different names*

### Comparing `pytest-yaml-yoyo-1.2.1/src/pytest_yaml_yoyo/validate.py` & `pytest-yaml-yoyo-1.2.2/src/pytest_yaml_yoyo/validate.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,18 @@
 
 def string_equals(check_value, expect_value):
     assert str(check_value) == str(expect_value), f'{check_value} == {expect_value}'
 
 
 def length_equals(check_value, expect_value):
     expect_len = _cast_to_int(expect_value)
-    assert len(str(check_value)) == expect_len, f'{len(str(check_value))} == {expect_value}'
+    if isinstance(check_value, list):
+        assert len(check_value) == expect_len, f'{len(check_value)} == {expect_value}'
+    else:
+        assert len(str(check_value)) == expect_len, f'{len(str(check_value))} == {expect_value}'
 
 
 def length_greater_than(check_value, expect_value):
     expect_len = _cast_to_int(expect_value)
     assert len(check_value) > expect_len, f'{len(check_value)} > {expect_value}'
```

### Comparing `pytest-yaml-yoyo-1.2.1/src/pytest_yaml_yoyo.egg-info/PKG-INFO` & `pytest-yaml-yoyo-1.2.2/src/pytest_yaml_yoyo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-yaml-yoyo
-Version: 1.2.1
+Version: 1.2.2
 Summary: http/https API run by yaml
 Home-page: https://github.com/yoyoketang/pytest-yaml-yoyo
 Author: 上海-悠悠
 Author-email: 283340479@qq.com
 License: proprietary
 Keywords: pytest,py.test,pytest-yaml,pytest-yaml-yoyo
 Classifier: Framework :: Pytest
@@ -132,45 +132,51 @@
 v1.1.3 发布时间 2022.12.17
 
 - 文件上传multipart/form-data 格式支持
 
 v1.1.4 发布时间 2023.2.13
 
 新增3个关键字
+
 - 1.sleep  添加用例之间的sleep 等待时间
 - 2.skip   跳过用例功能
 - 3.skipif   条件为真时跳过用例
 
 v1.1.5 发布时间 2023.2.16
 
 支持 2 中方式生成 yaml 用例
+
 - 1.本地 swagger.json 文件
 - 2.在线 swagger.json 地址
 
 v1.1.8 发布时间 2023.3.17
 
 int 转 str 类型
 
 v1.1.9 发布时间 2023-03-21
 
 做了以下优化
+
 - 1.validate 校验加了text 关键字获取全部body文本内容
 - 2.用例分层 api和 testcase 层 validate 校验优化，解决之前遗留的bug
 - 3.validate 校验方式更灵活，支持int类型校验字符长度和包含字符
 - 4.log 日志文件优化，只保留最近的5个日志文件
 
 v1.2.0 发布时间 2023-05-08
 
 优化以下问题
+
 - 1.断言的时候 None 和 'None' 可以判断是相等，在yaml中可以写null 或者 None, 不区分类型了
 - 2.添加局部变量variables
 - 3.优化request 下的hook 功能
 - 4.其它细节优化
 
-v1.2.1 发布
+v1.2.1 发布时间 2023-05-20
+
+优化以下问题
 
 1.兼容python3.8, python3.9, python3.10版本
 2.支持在case 用例中针对单个用例的参数化了
 3.参数化数据支持读取外部文件，文件格式可以支持：txt/csv/json/yaml
 4.函数的参数可以引用变量了，如: ${fun("hello ${key}")}
 5.内置to_json() 函数，字典转 json
```

### Comparing `pytest-yaml-yoyo-1.2.1/src/pytest_yaml_yoyo.egg-info/SOURCES.txt` & `pytest-yaml-yoyo-1.2.2/src/pytest_yaml_yoyo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

