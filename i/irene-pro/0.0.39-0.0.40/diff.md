# Comparing `tmp/irene_pro-0.0.39.tar.gz` & `tmp/irene_pro-0.0.40.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "irene_pro-0.0.39.tar", last modified: Sun May 21 15:43:37 2023, max compression
+gzip compressed data, was "irene_pro-0.0.40.tar", last modified: Mon May 22 08:24:27 2023, max compression
```

## Comparing `irene_pro-0.0.39.tar` & `irene_pro-0.0.40.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-21 15:43:37.250042 irene_pro-0.0.39/
--rw-rw-rw-   0        0        0      227 2023-05-04 09:47:29.000000 irene_pro-0.0.39/LICENSE
--rw-rw-rw-   0        0        0       14 2023-05-08 07:12:29.000000 irene_pro-0.0.39/MANIFEST.in
--rw-rw-rw-   0        0        0     1613 2023-05-21 15:43:37.243061 irene_pro-0.0.39/PKG-INFO
--rw-rw-rw-   0        0        0     1039 2023-05-21 15:41:24.000000 irene_pro-0.0.39/README.md
-drwxrwxrwx   0        0        0        0 2023-05-21 15:43:37.154486 irene_pro-0.0.39/irene_pro/
--rw-rw-rw-   0        0        0        0 2023-05-04 13:31:01.000000 irene_pro-0.0.39/irene_pro/__init__.py
--rw-rw-rw-   0        0        0     1445 2023-05-11 09:46:57.000000 irene_pro-0.0.39/irene_pro/logic.py
--rw-rw-rw-   0        0        0    30352 2023-05-21 15:40:21.000000 irene_pro-0.0.39/irene_pro/widgets.py
-drwxrwxrwx   0        0        0        0 2023-05-21 15:43:37.237077 irene_pro-0.0.39/irene_pro.egg-info/
--rw-rw-rw-   0        0        0     1613 2023-05-21 15:43:36.000000 irene_pro-0.0.39/irene_pro.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      264 2023-05-21 15:43:37.000000 irene_pro-0.0.39/irene_pro.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-21 15:43:36.000000 irene_pro-0.0.39/irene_pro.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       59 2023-05-21 15:43:36.000000 irene_pro-0.0.39/irene_pro.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-05-21 15:43:36.000000 irene_pro-0.0.39/irene_pro.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-21 15:43:37.252037 irene_pro-0.0.39/setup.cfg
--rw-rw-rw-   0        0        0     1164 2023-05-21 15:41:02.000000 irene_pro-0.0.39/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-22 08:24:27.734618 irene_pro-0.0.40/
+-rw-rw-rw-   0        0        0      227 2023-05-04 09:47:29.000000 irene_pro-0.0.40/LICENSE
+-rw-rw-rw-   0        0        0       14 2023-05-08 07:12:29.000000 irene_pro-0.0.40/MANIFEST.in
+-rw-rw-rw-   0        0        0     1623 2023-05-22 08:24:27.699711 irene_pro-0.0.40/PKG-INFO
+-rw-rw-rw-   0        0        0     1049 2023-05-22 08:23:51.000000 irene_pro-0.0.40/README.md
+drwxrwxrwx   0        0        0        0 2023-05-22 08:24:27.675782 irene_pro-0.0.40/irene_pro/
+-rw-rw-rw-   0        0        0        0 2023-05-04 13:31:01.000000 irene_pro-0.0.40/irene_pro/__init__.py
+-rw-rw-rw-   0        0        0     1445 2023-05-11 09:46:57.000000 irene_pro-0.0.40/irene_pro/logic.py
+-rw-rw-rw-   0        0        0    30728 2023-05-22 08:22:42.000000 irene_pro-0.0.40/irene_pro/widgets.py
+drwxrwxrwx   0        0        0        0 2023-05-22 08:24:27.695722 irene_pro-0.0.40/irene_pro.egg-info/
+-rw-rw-rw-   0        0        0     1623 2023-05-22 08:24:27.000000 irene_pro-0.0.40/irene_pro.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      264 2023-05-22 08:24:27.000000 irene_pro-0.0.40/irene_pro.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-22 08:24:27.000000 irene_pro-0.0.40/irene_pro.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       59 2023-05-22 08:24:27.000000 irene_pro-0.0.40/irene_pro.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-05-22 08:24:27.000000 irene_pro-0.0.40/irene_pro.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-22 08:24:27.735617 irene_pro-0.0.40/setup.cfg
+-rw-rw-rw-   0        0        0     1164 2023-05-22 08:23:23.000000 irene_pro-0.0.40/setup.py
```

### Comparing `irene_pro-0.0.39/PKG-INFO` & `irene_pro-0.0.40/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: irene_pro
-Version: 0.0.39
+Version: 0.0.40
 Summary: Use customized GUI
 Author: Irene coldsober
 Author-email: <irene.study.2023@gmail.com>
 Keywords: tkinter,widget,gui
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
@@ -37,9 +37,9 @@
 # login and signup template has been added too
 sign = widgets.LoginSignup(master)
 # get the sign_in_btn
 login_btn = sign.Login_btn()
 # call a function if the validation is successfully
 login_btn.config(command = sign.validate_login(callback = func_to_call, saved_username, saved_password))
 
-# calendar issue fixed
+# login template validation done
```

### Comparing `irene_pro-0.0.39/README.md` & `irene_pro-0.0.40/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -20,9 +20,9 @@
 # login and signup template has been added too
 sign = widgets.LoginSignup(master)
 # get the sign_in_btn
 login_btn = sign.Login_btn()
 # call a function if the validation is successfully
 login_btn.config(command = sign.validate_login(callback = func_to_call, saved_username, saved_password))
 
-# calendar issue fixed
+# login template validation done
```

### Comparing `irene_pro-0.0.39/irene_pro/logic.py` & `irene_pro-0.0.40/irene_pro/logic.py`

 * *Files identical despite different names*

### Comparing `irene_pro-0.0.39/irene_pro/widgets.py` & `irene_pro-0.0.40/irene_pro/widgets.py`

 * *Files 1% similar despite different names*

```diff
@@ -525,15 +525,15 @@
         if dir_holder:
             dir_holder.delete(0, END)
             dir_holder.insert(END, dir)
         else:
             return dir
 
 class LoginSignup:
-    def __init__(self,master,width = w(350), height = h(250), login = False, frame_pack_side = TOP) -> None:
+    def __init__(self,master,width = w(450), height = h(250), login = False, frame_pack_side = TOP) -> None:
         self.base_frame = lframe(master, width = width, height = height)
         self.base_frame.config(bd = 1)
         self.base_frame.pack(side = frame_pack_side, padx = w(1), pady = h(1))
         self.base_frame.pack_propagate(False)
         self.base_frame.config(bg = "beige")
 
         self.login_frame = []
@@ -541,15 +541,15 @@
 
         if login:
             self.login()
         else:
             self.signup()
 
     def login(self):
-        global username, password, login_btn
+        global username, password, validate_btn
         for fr in self.login_frame:
             fr.destroy()
 
         login_fr = frame(self.base_frame)
         login_fr.pack(fill = BOTH, expand = True)
         self.login_frame.append(login_fr)
         self.signup_frame.append(login_fr)
@@ -577,30 +577,34 @@
         login_btn.config(bg = "#b04", fg = "#fff")
         login_btn.pack(side = LEFT, padx = w(3), expand = True, fill = X)
 
         signup_btn = btn(btns, text = "Sign up", command = self.signup)
         signup_btn.config(bg = "#023", fg = "#fff")
         signup_btn.pack(side = LEFT, padx = w(3), expand = True, fill = X)
 
+        validate_btn = btn(btns, text = "Next")
+        validate_btn.config(bg = "#023", fg = "#fff")
+        validate_btn.pack(side = LEFT, padx = w(3), expand = True, fill = X)
+
         cancel_btn = btn(btns, text = "cancel", command = lambda: self.base_frame.destroy())
         cancel_btn.config(bg = "#600", fg = "#fff")
         cancel_btn.pack(side = RIGHT, padx = w(3), expand = True, fill = X)
     
     @property
     def Login_btn(self):
-        return login_btn
+        return validate_btn
 
     def validate_login(self, callback, *true_data):
         if (username.get(), password.get()) == true_data:
             callback()
         else:
             messagebox.showerror("Incorrect", "Username or password entered is incorrect")
 
     def signup(self):
-        global signup_btn, username, password, re_password
+        global confirm_btn, username, password, re_password
         for fr in self.signup_frame:
             fr.destroy()
             
         signup_fr = frame(self.base_frame)
         signup_fr.pack(fill = BOTH, expand = True)
         signup_fr.pack_propagate(False)
         self.signup_frame.append(signup_fr)
@@ -631,21 +635,25 @@
         login_btn.config(bg = "#b04", fg = "#fff")
         login_btn.pack(side = LEFT, padx = w(1), expand = True, fill = X)
 
         signup_btn = btn(btns, text = "Sign up")
         signup_btn.config(bg = "#023", fg = "#fff")
         signup_btn.pack(side = LEFT, padx = w(1), expand = True, fill = X)
 
+        confirm_btn = btn(btns, text = "confirm")
+        confirm_btn.config(bg = "#023", fg = "#fff")
+        confirm_btn.pack(side = LEFT, padx = w(1), expand = True, fill = X)
+
         cancel_btn = btn(btns, text = "cancel", command = lambda: self.base_frame.destroy())
         cancel_btn.config(bg = "#600", fg = "#fff")
         cancel_btn.pack(side = LEFT, padx = w(1), expand = True, fill = X)
 
     @property
     def Signup_btn(self):
-        return signup_btn
+        return confirm_btn
 
     def validate_signup(self, callback):
         if (re_password.get() == password.get() and len(password.get()) >= 8 and len(username.get()) >= 2):
             callback(data = [username.get(), password.get()])
         else:
             messagebox.showerror("Incorrect", "Username or password entered do not match")
```

### Comparing `irene_pro-0.0.39/irene_pro.egg-info/PKG-INFO` & `irene_pro-0.0.40/irene_pro.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: irene-pro
-Version: 0.0.39
+Version: 0.0.40
 Summary: Use customized GUI
 Author: Irene coldsober
 Author-email: <irene.study.2023@gmail.com>
 Keywords: tkinter,widget,gui
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
@@ -37,9 +37,9 @@
 # login and signup template has been added too
 sign = widgets.LoginSignup(master)
 # get the sign_in_btn
 login_btn = sign.Login_btn()
 # call a function if the validation is successfully
 login_btn.config(command = sign.validate_login(callback = func_to_call, saved_username, saved_password))
 
-# calendar issue fixed
+# login template validation done
```

### Comparing `irene_pro-0.0.39/setup.py` & `irene_pro-0.0.40/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 00000090: 286f 732e 7061 7468 2e6a 6f69 6e28 6865  (os.path.join(he
 000000a0: 7265 2c20 2252 4541 444d 452e 6d64 2229  re, "README.md")
 000000b0: 2c20 656e 636f 6469 6e67 3d22 7574 662d  , encoding="utf-
 000000c0: 3822 2920 6173 2066 683a 0d0a 2020 2020  8") as fh:..    
 000000d0: 6c6f 6e67 5f64 6573 6372 6970 7469 6f6e  long_description
 000000e0: 203d 2022 5c6e 2220 2b20 6668 2e72 6561   = "\n" + fh.rea
 000000f0: 6428 290d 0a0d 0a56 4552 5349 4f4e 203d  d()....VERSION =
-00000100: 2027 302e 302e 3339 270d 0a44 4553 4352   '0.0.39'..DESCR
+00000100: 2027 302e 302e 3430 270d 0a44 4553 4352   '0.0.40'..DESCR
 00000110: 4950 5449 4f4e 203d 2027 5573 6520 6375  IPTION = 'Use cu
 00000120: 7374 6f6d 697a 6564 2047 5549 270d 0a4c  stomized GUI'..L
 00000130: 4f4e 475f 4445 5343 5249 5054 494f 4e20  ONG_DESCRIPTION 
 00000140: 3d20 2741 2070 6163 6b61 6765 2074 6861  = 'A package tha
 00000150: 7420 616c 6c6f 7773 2079 6f75 2074 6f20  t allows you to 
 00000160: 7573 6520 7374 796c 6573 2061 6e64 2077  use styles and w
 00000170: 6964 6765 7420 6f66 2073 7570 6572 206c  idget of super l
```

