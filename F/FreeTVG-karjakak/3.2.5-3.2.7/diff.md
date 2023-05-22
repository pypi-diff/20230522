# Comparing `tmp/FreeTVG-karjakak-3.2.5.tar.gz` & `tmp/FreeTVG-karjakak-3.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FreeTVG-karjakak-3.2.5.tar", last modified: Sun May 21 17:23:38 2023, max compression
+gzip compressed data, was "FreeTVG-karjakak-3.2.7.tar", last modified: Mon May 22 01:46:46 2023, max compression
```

## Comparing `FreeTVG-karjakak-3.2.5.tar` & `FreeTVG-karjakak-3.2.7.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 karja      (501) staff       (20)        0 2023-05-21 17:23:38.492163 FreeTVG-karjakak-3.2.5/
-drwxr-xr-x   0 karja      (501) staff       (20)        0 2023-05-21 17:23:38.488989 FreeTVG-karjakak-3.2.5/FreeTVG_karjakak.egg-info/
--rw-r--r--   0 karja      (501) staff       (20)     1448 2023-05-21 17:23:38.000000 FreeTVG-karjakak-3.2.5/FreeTVG_karjakak.egg-info/PKG-INFO
--rw-r--r--   0 karja      (501) staff       (20)      463 2023-05-21 17:23:38.000000 FreeTVG-karjakak-3.2.5/FreeTVG_karjakak.egg-info/SOURCES.txt
--rw-r--r--   0 karja      (501) staff       (20)        1 2023-05-21 17:23:38.000000 FreeTVG-karjakak-3.2.5/FreeTVG_karjakak.egg-info/dependency_links.txt
--rw-r--r--   0 karja      (501) staff       (20)       29 2023-05-21 17:23:38.000000 FreeTVG-karjakak-3.2.5/FreeTVG_karjakak.egg-info/entry_points.txt
--rw-r--r--   0 karja      (501) staff       (20)      151 2023-05-21 17:23:38.000000 FreeTVG-karjakak-3.2.5/FreeTVG_karjakak.egg-info/requires.txt
--rw-r--r--   0 karja      (501) staff       (20)        4 2023-05-21 17:23:38.000000 FreeTVG-karjakak-3.2.5/FreeTVG_karjakak.egg-info/top_level.txt
--rw-r--r--   0 karja      (501) staff       (20)     1082 2021-04-02 20:37:42.000000 FreeTVG-karjakak-3.2.5/LICENSE.txt
--rw-r--r--   0 karja      (501) staff       (20)     1448 2023-05-21 17:23:38.492231 FreeTVG-karjakak-3.2.5/PKG-INFO
--rw-r--r--   0 karja      (501) staff       (20)      821 2022-12-10 03:07:59.000000 FreeTVG-karjakak-3.2.5/README.md
-drwxr-xr-x   0 karja      (501) staff       (20)        0 2023-05-21 17:23:38.490491 FreeTVG-karjakak-3.2.5/TVG/
--rw-r--r--   0 karja      (501) staff       (20)   146288 2023-05-21 17:12:07.000000 FreeTVG-karjakak-3.2.5/TVG/FreeTVG.py
--rw-r--r--   0 karja      (501) staff       (20)   360883 2023-05-17 06:38:49.000000 FreeTVG-karjakak-3.2.5/TVG/Tutorial TVG.pdf
--rw-r--r--   0 karja      (501) staff       (20)       46 2022-11-22 15:46:43.000000 FreeTVG-karjakak-3.2.5/TVG/__init__.py
-drwxr-xr-x   0 karja      (501) staff       (20)        0 2023-05-21 17:23:38.491031 FreeTVG-karjakak-3.2.5/TVG/structure/
--rw-r--r--   0 karja      (501) staff       (20)       82 2023-05-14 08:59:37.000000 FreeTVG-karjakak-3.2.5/TVG/structure/__init__.py
--rw-r--r--   0 karja      (501) staff       (20)    14894 2023-05-16 16:03:03.000000 FreeTVG-karjakak-3.2.5/TVG/structure/frame_layouts.py
-drwxr-xr-x   0 karja      (501) staff       (20)        0 2023-05-21 17:23:38.492054 FreeTVG-karjakak-3.2.5/TVG/utility/
--rw-r--r--   0 karja      (501) staff       (20)      923 2023-05-16 14:56:03.000000 FreeTVG-karjakak-3.2.5/TVG/utility/RegMail.py
--rw-r--r--   0 karja      (501) staff       (20)       84 2023-05-15 12:31:08.000000 FreeTVG-karjakak-3.2.5/TVG/utility/__init__.py
--rw-r--r--   0 karja      (501) staff       (20)     6682 2023-05-21 17:22:10.000000 FreeTVG-karjakak-3.2.5/TVG/utility/mdh.py
--rw-r--r--   0 karja      (501) staff       (20)      103 2021-11-12 16:03:29.000000 FreeTVG-karjakak-3.2.5/pyproject.toml
--rw-r--r--   0 karja      (501) staff       (20)      976 2023-05-21 17:23:38.492501 FreeTVG-karjakak-3.2.5/setup.cfg
+drwxr-xr-x   0 karja      (501) staff       (20)        0 2023-05-22 01:46:46.507913 FreeTVG-karjakak-3.2.7/
+drwxr-xr-x   0 karja      (501) staff       (20)        0 2023-05-22 01:46:46.504094 FreeTVG-karjakak-3.2.7/FreeTVG_karjakak.egg-info/
+-rw-r--r--   0 karja      (501) staff       (20)     1448 2023-05-22 01:46:46.000000 FreeTVG-karjakak-3.2.7/FreeTVG_karjakak.egg-info/PKG-INFO
+-rw-r--r--   0 karja      (501) staff       (20)      463 2023-05-22 01:46:46.000000 FreeTVG-karjakak-3.2.7/FreeTVG_karjakak.egg-info/SOURCES.txt
+-rw-r--r--   0 karja      (501) staff       (20)        1 2023-05-22 01:46:46.000000 FreeTVG-karjakak-3.2.7/FreeTVG_karjakak.egg-info/dependency_links.txt
+-rw-r--r--   0 karja      (501) staff       (20)       29 2023-05-22 01:46:46.000000 FreeTVG-karjakak-3.2.7/FreeTVG_karjakak.egg-info/entry_points.txt
+-rw-r--r--   0 karja      (501) staff       (20)      151 2023-05-22 01:46:46.000000 FreeTVG-karjakak-3.2.7/FreeTVG_karjakak.egg-info/requires.txt
+-rw-r--r--   0 karja      (501) staff       (20)        4 2023-05-22 01:46:46.000000 FreeTVG-karjakak-3.2.7/FreeTVG_karjakak.egg-info/top_level.txt
+-rw-r--r--   0 karja      (501) staff       (20)     1082 2021-04-02 20:37:42.000000 FreeTVG-karjakak-3.2.7/LICENSE.txt
+-rw-r--r--   0 karja      (501) staff       (20)     1448 2023-05-22 01:46:46.507990 FreeTVG-karjakak-3.2.7/PKG-INFO
+-rw-r--r--   0 karja      (501) staff       (20)      821 2022-12-10 03:07:59.000000 FreeTVG-karjakak-3.2.7/README.md
+drwxr-xr-x   0 karja      (501) staff       (20)        0 2023-05-22 01:46:46.506291 FreeTVG-karjakak-3.2.7/TVG/
+-rw-r--r--   0 karja      (501) staff       (20)   146320 2023-05-22 01:33:43.000000 FreeTVG-karjakak-3.2.7/TVG/FreeTVG.py
+-rw-r--r--   0 karja      (501) staff       (20)   360883 2023-05-17 06:38:49.000000 FreeTVG-karjakak-3.2.7/TVG/Tutorial TVG.pdf
+-rw-r--r--   0 karja      (501) staff       (20)       46 2022-11-22 15:46:43.000000 FreeTVG-karjakak-3.2.7/TVG/__init__.py
+drwxr-xr-x   0 karja      (501) staff       (20)        0 2023-05-22 01:46:46.506805 FreeTVG-karjakak-3.2.7/TVG/structure/
+-rw-r--r--   0 karja      (501) staff       (20)       82 2023-05-14 08:59:37.000000 FreeTVG-karjakak-3.2.7/TVG/structure/__init__.py
+-rw-r--r--   0 karja      (501) staff       (20)    14894 2023-05-16 16:03:03.000000 FreeTVG-karjakak-3.2.7/TVG/structure/frame_layouts.py
+drwxr-xr-x   0 karja      (501) staff       (20)        0 2023-05-22 01:46:46.507662 FreeTVG-karjakak-3.2.7/TVG/utility/
+-rw-r--r--   0 karja      (501) staff       (20)      923 2023-05-16 14:56:03.000000 FreeTVG-karjakak-3.2.7/TVG/utility/RegMail.py
+-rw-r--r--   0 karja      (501) staff       (20)       84 2023-05-15 12:31:08.000000 FreeTVG-karjakak-3.2.7/TVG/utility/__init__.py
+-rw-r--r--   0 karja      (501) staff       (20)     6654 2023-05-22 01:10:09.000000 FreeTVG-karjakak-3.2.7/TVG/utility/mdh.py
+-rw-r--r--   0 karja      (501) staff       (20)      103 2021-11-12 16:03:29.000000 FreeTVG-karjakak-3.2.7/pyproject.toml
+-rw-r--r--   0 karja      (501) staff       (20)      976 2023-05-22 01:46:46.508275 FreeTVG-karjakak-3.2.7/setup.cfg
```

### Comparing `FreeTVG-karjakak-3.2.5/FreeTVG_karjakak.egg-info/PKG-INFO` & `FreeTVG-karjakak-3.2.7/FreeTVG_karjakak.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FreeTVG-karjakak
-Version: 3.2.5
+Version: 3.2.7
 Summary: Tree View Gui for outline treeview note.
 Home-page: https://github.com/kakkarja/FreeTVG#latest-notice
 Author: karjakak
 Author-email: kakkarja.github@gmail.com
 License: MIT License
 Classifier: Environment :: Win32 (MS Windows)
 Classifier: Environment :: MacOS X
```

### Comparing `FreeTVG-karjakak-3.2.5/LICENSE.txt` & `FreeTVG-karjakak-3.2.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `FreeTVG-karjakak-3.2.5/PKG-INFO` & `FreeTVG-karjakak-3.2.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FreeTVG-karjakak
-Version: 3.2.5
+Version: 3.2.7
 Summary: Tree View Gui for outline treeview note.
 Home-page: https://github.com/kakkarja/FreeTVG#latest-notice
 Author: karjakak
 Author-email: kakkarja.github@gmail.com
 License: MIT License
 Classifier: Environment :: Win32 (MS Windows)
 Classifier: Environment :: MacOS X
```

### Comparing `FreeTVG-karjakak-3.2.5/README.md` & `FreeTVG-karjakak-3.2.7/README.md`

 * *Files identical despite different names*

### Comparing `FreeTVG-karjakak-3.2.5/TVG/FreeTVG.py` & `FreeTVG-karjakak-3.2.7/TVG/FreeTVG.py`

 * *Files 0% similar despite different names*

```diff
@@ -1727,14 +1727,15 @@
                 fon = f"{add}{fon}"
 
             ans = messagebox.askyesno(
                 "Preview",
                 "Do you want to preview? ('no' will go to web for printing)",
                 parent=self.root,
             )
+            style = None
             if ans:
                 style = convhtml(
                     self._utilspdf(),
                     self.filename,
                     fon,
                     self.text.cget("background")[1:],
                     self.text.cget("foreground"),
@@ -1746,15 +1747,15 @@
                     self._utilspdf(),
                     self.filename,
                     fon,
                     self.text.cget("background")[1:],
                     self.text.cget("foreground"),
                     preview=False,
                 )
-            del px, ck, sty, add, fon
+            del px, ck, sty, add, fon, style
 
     def spaces(self):
         """Mostly used by other functions to clear an obselete spaces.
         To appropriate the display better.
         """
 
         self.hidcheck()
@@ -3183,15 +3184,15 @@
             self.__setattr__("labcop", None)
             d = MyDialog(self.root)
             self.lock = False
             self.root.update()
             self.unlock = True
             self.FREEZE = True
             self.__delattr__("labcop")
-            del wid, lab, d, err, stor_entry
+            del wid, lab, d, err, stor_tuple
         else:
             messagebox.showinfo(
                 "TreeViewGui", "Only work for Editor mode", parent=self.root
             )
 
     def _indconv(self, n: int):
         return f"{float(n)}", f"{float(n + 1)}"
```

### Comparing `FreeTVG-karjakak-3.2.5/TVG/Tutorial TVG.pdf` & `FreeTVG-karjakak-3.2.7/TVG/Tutorial TVG.pdf`

 * *Files identical despite different names*

### Comparing `FreeTVG-karjakak-3.2.5/TVG/structure/frame_layouts.py` & `FreeTVG-karjakak-3.2.7/TVG/structure/frame_layouts.py`

 * *Files identical despite different names*

### Comparing `FreeTVG-karjakak-3.2.5/TVG/utility/RegMail.py` & `FreeTVG-karjakak-3.2.7/TVG/utility/RegMail.py`

 * *Files identical despite different names*

### Comparing `FreeTVG-karjakak-3.2.5/TVG/utility/mdh.py` & `FreeTVG-karjakak-3.2.7/TVG/utility/mdh.py`

 * *Files 0% similar despite different names*

```diff
@@ -238,11 +238,10 @@
             printed,
             nxt,
             pro,
             startupinfo,
             pointer_event,
             window,
             preview,
-            pointer_event,
             width,
             height,
         )
```

### Comparing `FreeTVG-karjakak-3.2.5/setup.cfg` & `FreeTVG-karjakak-3.2.7/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = FreeTVG-karjakak
-version = 3.2.5
+version = 3.2.7
 author = karjakak
 author_email = kakkarja.github@gmail.com
 description = Tree View Gui for outline treeview note.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/kakkarja/FreeTVG#latest-notice
 license = MIT License
```

