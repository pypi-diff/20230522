# Comparing `tmp/tkintertools-2.6.1.1.tar.gz` & `tmp/tkintertools-2.6.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tkintertools-2.6.1.1.tar", last modified: Sun May 21 10:08:41 2023, max compression
+gzip compressed data, was "tkintertools-2.6.1.2.tar", last modified: Mon May 22 14:07:59 2023, max compression
```

## Comparing `tkintertools-2.6.1.1.tar` & `tkintertools-2.6.1.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-21 10:08:41.589826 tkintertools-2.6.1.1/
--rw-rw-rw-   0        0        0     7548 2023-05-20 23:03:00.000000 tkintertools-2.6.1.1/LICENSE
--rw-rw-rw-   0        0        0    26443 2023-05-21 10:08:41.588826 tkintertools-2.6.1.1/PKG-INFO
--rw-rw-rw-   0        0        0    25936 2023-05-21 09:54:32.000000 tkintertools-2.6.1.1/README.md
--rw-rw-rw-   0        0        0       42 2023-05-21 10:08:41.589826 tkintertools-2.6.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1208 2023-05-21 10:07:51.000000 tkintertools-2.6.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-21 10:08:41.580824 tkintertools-2.6.1.1/tkintertools/
--rw-rw-rw-   0        0        0     1877 2023-05-20 20:35:35.000000 tkintertools-2.6.1.1/tkintertools/__init__.py
--rw-rw-rw-   0        0        0    60750 2023-05-21 10:02:16.000000 tkintertools-2.6.1.1/tkintertools/__main__.py
--rw-rw-rw-   0        0        0     1295 2023-05-20 20:58:40.000000 tkintertools-2.6.1.1/tkintertools/constants.py
--rw-rw-rw-   0        0        0      870 2023-05-14 13:27:34.000000 tkintertools-2.6.1.1/tkintertools/md.py
-drwxrwxrwx   0        0        0        0 2023-05-21 10:08:41.586825 tkintertools-2.6.1.1/tkintertools.egg-info/
--rw-rw-rw-   0        0        0    26443 2023-05-21 10:08:41.000000 tkintertools-2.6.1.1/tkintertools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      265 2023-05-21 10:08:41.000000 tkintertools-2.6.1.1/tkintertools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-21 10:08:41.000000 tkintertools-2.6.1.1/tkintertools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-05-21 10:08:41.000000 tkintertools-2.6.1.1/tkintertools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-22 14:07:59.974072 tkintertools-2.6.1.2/
+-rw-rw-rw-   0        0        0     7548 2023-05-20 23:03:00.000000 tkintertools-2.6.1.2/LICENSE
+-rw-rw-rw-   0        0        0    26354 2023-05-22 14:07:59.973072 tkintertools-2.6.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0    25847 2023-05-21 10:18:49.000000 tkintertools-2.6.1.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-22 14:07:59.974072 tkintertools-2.6.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1208 2023-05-22 14:07:49.000000 tkintertools-2.6.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-22 14:07:59.965072 tkintertools-2.6.1.2/tkintertools/
+-rw-rw-rw-   0        0        0     1877 2023-05-20 20:35:35.000000 tkintertools-2.6.1.2/tkintertools/__init__.py
+-rw-rw-rw-   0        0        0    60774 2023-05-22 14:06:41.000000 tkintertools-2.6.1.2/tkintertools/__main__.py
+-rw-rw-rw-   0        0        0     1295 2023-05-22 14:06:44.000000 tkintertools-2.6.1.2/tkintertools/constants.py
+-rw-rw-rw-   0        0        0      870 2023-05-14 13:27:34.000000 tkintertools-2.6.1.2/tkintertools/md.py
+drwxrwxrwx   0        0        0        0 2023-05-22 14:07:59.971075 tkintertools-2.6.1.2/tkintertools.egg-info/
+-rw-rw-rw-   0        0        0    26354 2023-05-22 14:07:59.000000 tkintertools-2.6.1.2/tkintertools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      265 2023-05-22 14:07:59.000000 tkintertools-2.6.1.2/tkintertools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-22 14:07:59.000000 tkintertools-2.6.1.2/tkintertools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-05-22 14:07:59.000000 tkintertools-2.6.1.2/tkintertools.egg-info/top_level.txt
```

### Comparing `tkintertools-2.6.1.1/LICENSE` & `tkintertools-2.6.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tkintertools-2.6.1.1/PKG-INFO` & `tkintertools-2.6.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tkintertools
-Version: 2.6.1.1
+Version: 2.6.1.2
 Summary: An auxiliary module of the tkinder module
 Home-page: https://gitcode.net/weixin_62651706/tkintertools
 Author: Xiaokang2022
 Author-email: 2951256653@qq.com
 License: MulanPSL-2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Mulan Permissive Software License v2 (MulanPSL-2.0)
@@ -582,11 +582,8 @@
 
 > GitHub(Mirror/镜像):  
 > https://github.com/XiaoKang2022-CSDN/tkintertools
 
 > Column/专栏:  
 > https://blog.csdn.net/weixin_62651706/category_11600888.html
 
-> Tutorials/教程:  
-> https://xiaokang2022.blog.csdn.net/article/details/127374661
-
 还有更多内容请在 [源代码](./tkintertools/) 中探索！
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: tkintertools Version: 2.6.1.1 Summary: An auxiliary
+Metadata-Version: 2.1 Name: tkintertools Version: 2.6.1.2 Summary: An auxiliary
 module of the tkinder module Home-page: https://gitcode.net/weixin_62651706/
 tkintertools Author: Xiaokang2022 Author-email: 2951256653@qq.com License:
 MulanPSL-2.0 Classifier: Programming Language :: Python :: 3 Classifier:
 License :: OSI Approved :: Mulan Permissive Software License v2 (MulanPSL-2.0)
 Classifier: Operating System :: OS Independent Description-Content-Type: text/
 markdown License-File: LICENSE
                       ****** ðtkintertoolsð ******
@@ -267,10 +267,9 @@
 v2.6.0ï¼çé¢éå¸¸ç¨³å®ï¼å ä¹æ²¡æ bugï¼å®å¨éç¨ tkintertools
 çæ§ä»¶ï¼é¢å¼å¾é«ï¼çé¢éå¸¸æµçãä½ç°äº tkintertools
 æ¨¡åä¸ tkinter æ¨¡åç¸æ¯å¨æ§è½ä¸çä¼è¶æ§ï¼
 [client.png] [client.png]
 More/æ´å¤ --------- > GitCode: > https://gitcode.net/weixin_62651706/
 tkintertools > GitHub(Mirror/éå): > https://github.com/XiaoKang2022-CSDN/
 tkintertools > Column/ä¸æ : > https://blog.csdn.net/weixin_62651706/
-category_11600888.html > Tutorials/æç¨: > https://
-xiaokang2022.blog.csdn.net/article/details/127374661 è¿ææ´å¤åå®¹è¯·å¨
-[æºä»£ç ](./tkintertools/) ä¸­æ¢ç´¢ï¼
+category_11600888.html è¿ææ´å¤åå®¹è¯·å¨ [æºä»£ç ](./tkintertools/
+) ä¸­æ¢ç´¢ï¼
```

### Comparing `tkintertools-2.6.1.1/README.md` & `tkintertools-2.6.1.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -568,11 +568,8 @@
 
 > GitHub(Mirror/镜像):  
 > https://github.com/XiaoKang2022-CSDN/tkintertools
 
 > Column/专栏:  
 > https://blog.csdn.net/weixin_62651706/category_11600888.html
 
-> Tutorials/教程:  
-> https://xiaokang2022.blog.csdn.net/article/details/127374661
-
 还有更多内容请在 [源代码](./tkintertools/) 中探索！
```

#### html2text {}

```diff
@@ -260,10 +260,9 @@
 v2.6.0ï¼çé¢éå¸¸ç¨³å®ï¼å ä¹æ²¡æ bugï¼å®å¨éç¨ tkintertools
 çæ§ä»¶ï¼é¢å¼å¾é«ï¼çé¢éå¸¸æµçãä½ç°äº tkintertools
 æ¨¡åä¸ tkinter æ¨¡åç¸æ¯å¨æ§è½ä¸çä¼è¶æ§ï¼
 [client.png] [client.png]
 More/æ´å¤ --------- > GitCode: > https://gitcode.net/weixin_62651706/
 tkintertools > GitHub(Mirror/éå): > https://github.com/XiaoKang2022-CSDN/
 tkintertools > Column/ä¸æ : > https://blog.csdn.net/weixin_62651706/
-category_11600888.html > Tutorials/æç¨: > https://
-xiaokang2022.blog.csdn.net/article/details/127374661 è¿ææ´å¤åå®¹è¯·å¨
-[æºä»£ç ](./tkintertools/) ä¸­æ¢ç´¢ï¼
+category_11600888.html è¿ææ´å¤åå®¹è¯·å¨ [æºä»£ç ](./tkintertools/
+) ä¸­æ¢ç´¢ï¼
```

### Comparing `tkintertools-2.6.1.1/setup.py` & `tkintertools-2.6.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """ 上传 pypi """
 
 import setuptools
 
 
 setuptools.setup(
     name='tkintertools',
-    version="2.6.1.1",
+    version="2.6.1.2",
     author='Xiaokang2022',
     license='MulanPSL-2.0',
     author_email='2951256653@qq.com',
     description='An auxiliary module of the tkinder module',
     long_description=open('README.md', encoding='utf-8').read(),
     long_description_content_type='text/markdown',
     url='https://gitcode.net/weixin_62651706/tkintertools',
```

### Comparing `tkintertools-2.6.1.1/tkintertools/__init__.py` & `tkintertools-2.6.1.2/tkintertools/__init__.py`

 * *Files identical despite different names*

### Comparing `tkintertools-2.6.1.1/tkintertools/__main__.py` & `tkintertools-2.6.1.2/tkintertools/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -183,15 +183,15 @@
             self, master, width=width, height=height, highlightthickness=0, **kw)
 
         if not (kw.get('bg', None) or kw.get('background', None)):
             # Linux 系统上背景默认值不是 #F1F1F1，影响模块默认值的效果
             self.configure(bg=BACKGROUND)
 
         master._canvas.append(self)  # 将实例添加到 Tk 的画布列表中
-        if x and y:
+        if x is not None and y is not None:
             self.place(x=x, y=y)
 
         self.bind('<Motion>', self.__touch)  # 绑定鼠标触碰控件
         self.bind('<Any-Key>', self.__input)  # 绑定键盘输入字符（和Ctrl+v的代码顺序不可错）
         self.bind('<Button-1>', self.__click)  # 绑定鼠标左键按下
         self.bind('<B1-Motion>', self.__click)  # 绑定鼠标左键按下移动
         self.bind('<MouseWheel>', self.__mousewheel)  # 绑定鼠标滚轮滚动
```

### Comparing `tkintertools-2.6.1.1/tkintertools/constants.py` & `tkintertools-2.6.1.2/tkintertools/constants.py`

 * *Files identical despite different names*

### Comparing `tkintertools-2.6.1.1/tkintertools/md.py` & `tkintertools-2.6.1.2/tkintertools/md.py`

 * *Files identical despite different names*

### Comparing `tkintertools-2.6.1.1/tkintertools.egg-info/PKG-INFO` & `tkintertools-2.6.1.2/tkintertools.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tkintertools
-Version: 2.6.1.1
+Version: 2.6.1.2
 Summary: An auxiliary module of the tkinder module
 Home-page: https://gitcode.net/weixin_62651706/tkintertools
 Author: Xiaokang2022
 Author-email: 2951256653@qq.com
 License: MulanPSL-2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Mulan Permissive Software License v2 (MulanPSL-2.0)
@@ -582,11 +582,8 @@
 
 > GitHub(Mirror/镜像):  
 > https://github.com/XiaoKang2022-CSDN/tkintertools
 
 > Column/专栏:  
 > https://blog.csdn.net/weixin_62651706/category_11600888.html
 
-> Tutorials/教程:  
-> https://xiaokang2022.blog.csdn.net/article/details/127374661
-
 还有更多内容请在 [源代码](./tkintertools/) 中探索！
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: tkintertools Version: 2.6.1.1 Summary: An auxiliary
+Metadata-Version: 2.1 Name: tkintertools Version: 2.6.1.2 Summary: An auxiliary
 module of the tkinder module Home-page: https://gitcode.net/weixin_62651706/
 tkintertools Author: Xiaokang2022 Author-email: 2951256653@qq.com License:
 MulanPSL-2.0 Classifier: Programming Language :: Python :: 3 Classifier:
 License :: OSI Approved :: Mulan Permissive Software License v2 (MulanPSL-2.0)
 Classifier: Operating System :: OS Independent Description-Content-Type: text/
 markdown License-File: LICENSE
                       ****** ðtkintertoolsð ******
@@ -267,10 +267,9 @@
 v2.6.0ï¼çé¢éå¸¸ç¨³å®ï¼å ä¹æ²¡æ bugï¼å®å¨éç¨ tkintertools
 çæ§ä»¶ï¼é¢å¼å¾é«ï¼çé¢éå¸¸æµçãä½ç°äº tkintertools
 æ¨¡åä¸ tkinter æ¨¡åç¸æ¯å¨æ§è½ä¸çä¼è¶æ§ï¼
 [client.png] [client.png]
 More/æ´å¤ --------- > GitCode: > https://gitcode.net/weixin_62651706/
 tkintertools > GitHub(Mirror/éå): > https://github.com/XiaoKang2022-CSDN/
 tkintertools > Column/ä¸æ : > https://blog.csdn.net/weixin_62651706/
-category_11600888.html > Tutorials/æç¨: > https://
-xiaokang2022.blog.csdn.net/article/details/127374661 è¿ææ´å¤åå®¹è¯·å¨
-[æºä»£ç ](./tkintertools/) ä¸­æ¢ç´¢ï¼
+category_11600888.html è¿ææ´å¤åå®¹è¯·å¨ [æºä»£ç ](./tkintertools/
+) ä¸­æ¢ç´¢ï¼
```

