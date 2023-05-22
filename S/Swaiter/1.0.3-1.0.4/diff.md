# Comparing `tmp/Swaiter-1.0.3.tar.gz` & `tmp/Swaiter-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Swaiter-1.0.3.tar", last modified: Tue May 16 09:02:29 2023, max compression
+gzip compressed data, was "Swaiter-1.0.4.tar", last modified: Mon May 22 04:04:03 2023, max compression
```

## Comparing `Swaiter-1.0.3.tar` & `Swaiter-1.0.4.tar`

### file list

```diff
@@ -1,12 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-05-16 09:02:29.017407 Swaiter-1.0.3/
--rw-rw-rw-   0        0        0     3190 2023-05-16 09:02:29.015511 Swaiter-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     2878 2023-05-16 08:57:31.000000 Swaiter-1.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-05-16 09:02:29.015511 Swaiter-1.0.3/Swaiter.egg-info/
--rw-rw-rw-   0        0        0     3190 2023-05-16 09:02:28.000000 Swaiter-1.0.3/Swaiter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      188 2023-05-16 09:02:28.000000 Swaiter-1.0.3/Swaiter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-16 09:02:28.000000 Swaiter-1.0.3/Swaiter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       30 2023-05-16 09:02:28.000000 Swaiter-1.0.3/Swaiter.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-16 09:02:28.000000 Swaiter-1.0.3/Swaiter.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     4209 2023-05-16 07:13:32.000000 Swaiter-1.0.3/Waiter.py
--rw-rw-rw-   0        0        0      405 2023-05-16 09:00:17.000000 Swaiter-1.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-16 09:02:29.017407 Swaiter-1.0.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-22 04:04:03.441853 Swaiter-1.0.4/
+-rw-rw-rw-   0        0        0     1081 2023-05-16 09:14:50.000000 Swaiter-1.0.4/LICENSE
+-rw-rw-rw-   0        0        0     3396 2023-05-22 04:04:03.440849 Swaiter-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     3061 2023-05-22 03:57:38.000000 Swaiter-1.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-05-22 04:04:03.439856 Swaiter-1.0.4/Swaiter.egg-info/
+-rw-rw-rw-   0        0        0     3396 2023-05-22 04:04:03.000000 Swaiter-1.0.4/Swaiter.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      196 2023-05-22 04:04:03.000000 Swaiter-1.0.4/Swaiter.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-22 04:04:03.000000 Swaiter-1.0.4/Swaiter.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       30 2023-05-22 04:04:03.000000 Swaiter-1.0.4/Swaiter.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-22 04:04:03.000000 Swaiter-1.0.4/Swaiter.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     6174 2023-05-22 03:54:14.000000 Swaiter-1.0.4/Waiter.py
+-rw-rw-rw-   0        0        0      405 2023-05-22 03:59:30.000000 Swaiter-1.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-22 04:04:03.441853 Swaiter-1.0.4/setup.cfg
```

### Comparing `Swaiter-1.0.3/PKG-INFO` & `Swaiter-1.0.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: Swaiter
-Version: 1.0.3
+Version: 1.0.4
 Summary: The loop waits until the selenium element has loaded.
 Author-email: Beier <1601684622@qq.com>
 Project-URL: github, https://github.com/srx-2000/Swaiter
 Keywords: selenium,crawler
-Requires-Python: >=3.8
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 # Swaiter
 
 ​	项目名字取自：Selenium+waiter
 
 ​	作为一个爬虫人，在使用selenium进行爬虫时，时长会遇到由于网络等原因导致无法及时获取一些元素，从而导致程序报错。此时聪明的小伙伴就会说了：加个`time.sleep()`不就好了。事实上这个方法确实可以解决绝大部分问题，但其也有一个比较尴尬的问题：到底要“睡”多久合适？长了耽误爬取效率，短了又怕没有作用，所以这个库就是为了解决上述问题而存在的。
 
@@ -80,15 +81,25 @@
 >
 > selenium>=4.9.0
 >
 > loguru>=0.7.0
 
 ## 版本
 
+#### 2023.5.22
+
+**Version-1.0.4**
+
+- 添加select组件的搜索器
+  - 添加获取组件所有选项
+  - 添加向select组件中输入值
+
+[1.0.4](https://pypi.org/project/Swaiter/1.0.4/)
+
 #### 2023.5.16
 
 **Version-1.0.3**
 
 完成基础功能
 
-​	[1.0.3](https://pypi.org/manage/project/Swaiter/release/1.0.3/)
+[1.0.3](https://pypi.org/project/Swaiter/1.0.3/)
```

### Comparing `Swaiter-1.0.3/README.md` & `Swaiter-1.0.4/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -70,15 +70,25 @@
 >
 > selenium>=4.9.0
 >
 > loguru>=0.7.0
 
 ## 版本
 
+#### 2023.5.22
+
+**Version-1.0.4**
+
+- 添加select组件的搜索器
+  - 添加获取组件所有选项
+  - 添加向select组件中输入值
+
+[1.0.4](https://pypi.org/project/Swaiter/1.0.4/)
+
 #### 2023.5.16
 
 **Version-1.0.3**
 
 完成基础功能
 
-​	[1.0.3](https://pypi.org/manage/project/Swaiter/release/1.0.3/)
+[1.0.3](https://pypi.org/project/Swaiter/1.0.3/)
```

### Comparing `Swaiter-1.0.3/Swaiter.egg-info/PKG-INFO` & `Swaiter-1.0.4/Swaiter.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: Swaiter
-Version: 1.0.3
+Version: 1.0.4
 Summary: The loop waits until the selenium element has loaded.
 Author-email: Beier <1601684622@qq.com>
 Project-URL: github, https://github.com/srx-2000/Swaiter
 Keywords: selenium,crawler
-Requires-Python: >=3.8
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 # Swaiter
 
 ​	项目名字取自：Selenium+waiter
 
 ​	作为一个爬虫人，在使用selenium进行爬虫时，时长会遇到由于网络等原因导致无法及时获取一些元素，从而导致程序报错。此时聪明的小伙伴就会说了：加个`time.sleep()`不就好了。事实上这个方法确实可以解决绝大部分问题，但其也有一个比较尴尬的问题：到底要“睡”多久合适？长了耽误爬取效率，短了又怕没有作用，所以这个库就是为了解决上述问题而存在的。
 
@@ -80,15 +81,25 @@
 >
 > selenium>=4.9.0
 >
 > loguru>=0.7.0
 
 ## 版本
 
+#### 2023.5.22
+
+**Version-1.0.4**
+
+- 添加select组件的搜索器
+  - 添加获取组件所有选项
+  - 添加向select组件中输入值
+
+[1.0.4](https://pypi.org/project/Swaiter/1.0.4/)
+
 #### 2023.5.16
 
 **Version-1.0.3**
 
 完成基础功能
 
-​	[1.0.3](https://pypi.org/manage/project/Swaiter/release/1.0.3/)
+[1.0.3](https://pypi.org/project/Swaiter/1.0.3/)
```

