# Comparing `tmp/irene_pro-0.0.40.tar.gz` & `tmp/irene_pro-0.0.41.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "irene_pro-0.0.40.tar", last modified: Mon May 22 08:24:27 2023, max compression
+gzip compressed data, was "irene_pro-0.0.41.tar", last modified: Mon May 22 09:36:48 2023, max compression
```

## Comparing `irene_pro-0.0.40.tar` & `irene_pro-0.0.41.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-22 08:24:27.734618 irene_pro-0.0.40/
--rw-rw-rw-   0        0        0      227 2023-05-04 09:47:29.000000 irene_pro-0.0.40/LICENSE
--rw-rw-rw-   0        0        0       14 2023-05-08 07:12:29.000000 irene_pro-0.0.40/MANIFEST.in
--rw-rw-rw-   0        0        0     1623 2023-05-22 08:24:27.699711 irene_pro-0.0.40/PKG-INFO
--rw-rw-rw-   0        0        0     1049 2023-05-22 08:23:51.000000 irene_pro-0.0.40/README.md
-drwxrwxrwx   0        0        0        0 2023-05-22 08:24:27.675782 irene_pro-0.0.40/irene_pro/
--rw-rw-rw-   0        0        0        0 2023-05-04 13:31:01.000000 irene_pro-0.0.40/irene_pro/__init__.py
--rw-rw-rw-   0        0        0     1445 2023-05-11 09:46:57.000000 irene_pro-0.0.40/irene_pro/logic.py
--rw-rw-rw-   0        0        0    30728 2023-05-22 08:22:42.000000 irene_pro-0.0.40/irene_pro/widgets.py
-drwxrwxrwx   0        0        0        0 2023-05-22 08:24:27.695722 irene_pro-0.0.40/irene_pro.egg-info/
--rw-rw-rw-   0        0        0     1623 2023-05-22 08:24:27.000000 irene_pro-0.0.40/irene_pro.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      264 2023-05-22 08:24:27.000000 irene_pro-0.0.40/irene_pro.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-22 08:24:27.000000 irene_pro-0.0.40/irene_pro.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       59 2023-05-22 08:24:27.000000 irene_pro-0.0.40/irene_pro.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-05-22 08:24:27.000000 irene_pro-0.0.40/irene_pro.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-22 08:24:27.735617 irene_pro-0.0.40/setup.cfg
--rw-rw-rw-   0        0        0     1164 2023-05-22 08:23:23.000000 irene_pro-0.0.40/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-22 09:36:48.422502 irene_pro-0.0.41/
+-rw-rw-rw-   0        0        0      227 2023-05-04 09:47:29.000000 irene_pro-0.0.41/LICENSE
+-rw-rw-rw-   0        0        0       14 2023-05-08 07:12:29.000000 irene_pro-0.0.41/MANIFEST.in
+-rw-rw-rw-   0        0        0     1623 2023-05-22 09:36:48.421505 irene_pro-0.0.41/PKG-INFO
+-rw-rw-rw-   0        0        0     1049 2023-05-22 08:23:51.000000 irene_pro-0.0.41/README.md
+drwxrwxrwx   0        0        0        0 2023-05-22 09:36:48.400478 irene_pro-0.0.41/irene_pro/
+-rw-rw-rw-   0        0        0        0 2023-05-04 13:31:01.000000 irene_pro-0.0.41/irene_pro/__init__.py
+-rw-rw-rw-   0        0        0     1445 2023-05-11 09:46:57.000000 irene_pro-0.0.41/irene_pro/logic.py
+-rw-rw-rw-   0        0        0    30607 2023-05-22 09:28:57.000000 irene_pro-0.0.41/irene_pro/widgets.py
+drwxrwxrwx   0        0        0        0 2023-05-22 09:36:48.418529 irene_pro-0.0.41/irene_pro.egg-info/
+-rw-rw-rw-   0        0        0     1623 2023-05-22 09:36:48.000000 irene_pro-0.0.41/irene_pro.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      264 2023-05-22 09:36:48.000000 irene_pro-0.0.41/irene_pro.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-22 09:36:48.000000 irene_pro-0.0.41/irene_pro.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       59 2023-05-22 09:36:48.000000 irene_pro-0.0.41/irene_pro.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-05-22 09:36:48.000000 irene_pro-0.0.41/irene_pro.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-22 09:36:48.423498 irene_pro-0.0.41/setup.cfg
+-rw-rw-rw-   0        0        0     1164 2023-05-22 09:33:31.000000 irene_pro-0.0.41/setup.py
```

### Comparing `irene_pro-0.0.40/PKG-INFO` & `irene_pro-0.0.41/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: irene_pro
-Version: 0.0.40
+Version: 0.0.41
 Summary: Use customized GUI
 Author: Irene coldsober
 Author-email: <irene.study.2023@gmail.com>
 Keywords: tkinter,widget,gui
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `irene_pro-0.0.40/README.md` & `irene_pro-0.0.41/README.md`

 * *Files identical despite different names*

### Comparing `irene_pro-0.0.40/irene_pro/logic.py` & `irene_pro-0.0.41/irene_pro/logic.py`

 * *Files identical despite different names*

### Comparing `irene_pro-0.0.40/irene_pro/widgets.py` & `irene_pro-0.0.41/irene_pro/widgets.py`

 * *Files 1% similar despite different names*

```diff
@@ -589,19 +589,19 @@
         cancel_btn.config(bg = "#600", fg = "#fff")
         cancel_btn.pack(side = RIGHT, padx = w(3), expand = True, fill = X)
     
     @property
     def Login_btn(self):
         return validate_btn
 
-    def validate_login(self, callback, *true_data):
+    def validate_login(self, callback, true_data):
         if (username.get(), password.get()) == true_data:
             callback()
-        else:
-            messagebox.showerror("Incorrect", "Username or password entered is incorrect")
+            return True
+        return False
 
     def signup(self):
         global confirm_btn, username, password, re_password
         for fr in self.signup_frame:
             fr.destroy()
             
         signup_fr = frame(self.base_frame)
@@ -650,16 +650,16 @@
     @property
     def Signup_btn(self):
         return confirm_btn
 
     def validate_signup(self, callback):
         if (re_password.get() == password.get() and len(password.get()) >= 8 and len(username.get()) >= 2):
             callback(data = [username.get(), password.get()])
-        else:
-            messagebox.showerror("Incorrect", "Username or password entered do not match")
+            return True
+        return False
 
 class Table_gui:
     def __init__(self, parent):
         self.rows = 1
         self.cols = 1
         self.data = []
         self.entries = []
```

### Comparing `irene_pro-0.0.40/irene_pro.egg-info/PKG-INFO` & `irene_pro-0.0.41/irene_pro.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: irene-pro
-Version: 0.0.40
+Version: 0.0.41
 Summary: Use customized GUI
 Author: Irene coldsober
 Author-email: <irene.study.2023@gmail.com>
 Keywords: tkinter,widget,gui
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `irene_pro-0.0.40/setup.py` & `irene_pro-0.0.41/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 00000090: 286f 732e 7061 7468 2e6a 6f69 6e28 6865  (os.path.join(he
 000000a0: 7265 2c20 2252 4541 444d 452e 6d64 2229  re, "README.md")
 000000b0: 2c20 656e 636f 6469 6e67 3d22 7574 662d  , encoding="utf-
 000000c0: 3822 2920 6173 2066 683a 0d0a 2020 2020  8") as fh:..    
 000000d0: 6c6f 6e67 5f64 6573 6372 6970 7469 6f6e  long_description
 000000e0: 203d 2022 5c6e 2220 2b20 6668 2e72 6561   = "\n" + fh.rea
 000000f0: 6428 290d 0a0d 0a56 4552 5349 4f4e 203d  d()....VERSION =
-00000100: 2027 302e 302e 3430 270d 0a44 4553 4352   '0.0.40'..DESCR
+00000100: 2027 302e 302e 3431 270d 0a44 4553 4352   '0.0.41'..DESCR
 00000110: 4950 5449 4f4e 203d 2027 5573 6520 6375  IPTION = 'Use cu
 00000120: 7374 6f6d 697a 6564 2047 5549 270d 0a4c  stomized GUI'..L
 00000130: 4f4e 475f 4445 5343 5249 5054 494f 4e20  ONG_DESCRIPTION 
 00000140: 3d20 2741 2070 6163 6b61 6765 2074 6861  = 'A package tha
 00000150: 7420 616c 6c6f 7773 2079 6f75 2074 6f20  t allows you to 
 00000160: 7573 6520 7374 796c 6573 2061 6e64 2077  use styles and w
 00000170: 6964 6765 7420 6f66 2073 7570 6572 206c  idget of super l
```

