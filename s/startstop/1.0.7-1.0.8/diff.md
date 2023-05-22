# Comparing `tmp/startstop-1.0.7.tar.gz` & `tmp/startstop-1.0.8.tar.gz`

## Comparing `startstop-1.0.7.tar` & `startstop-1.0.8.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 startstop-1.0.7/.DS_Store
--rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 startstop-1.0.7/example.py
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 startstop-1.0.7/.vscode/settings.json
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 startstop-1.0.7/startstop/__about__.py
--rw-r--r--   0        0        0     2123 2020-02-02 00:00:00.000000 startstop-1.0.7/startstop/__init__.py
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 startstop-1.0.7/.gitignore
--rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 startstop-1.0.7/LICENSE.txt
--rw-r--r--   0        0        0     1254 2020-02-02 00:00:00.000000 startstop-1.0.7/README.md
--rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 startstop-1.0.7/pyproject.toml
--rw-r--r--   0        0        0     1574 2020-02-02 00:00:00.000000 startstop-1.0.7/PKG-INFO
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 startstop-1.0.8/.DS_Store
+-rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 startstop-1.0.8/example.py
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 startstop-1.0.8/.vscode/settings.json
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 startstop-1.0.8/startstop/__about__.py
+-rw-r--r--   0        0        0     2110 2020-02-02 00:00:00.000000 startstop-1.0.8/startstop/__init__.py
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 startstop-1.0.8/.gitignore
+-rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 startstop-1.0.8/LICENSE.txt
+-rw-r--r--   0        0        0     1254 2020-02-02 00:00:00.000000 startstop-1.0.8/README.md
+-rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 startstop-1.0.8/pyproject.toml
+-rw-r--r--   0        0        0     1574 2020-02-02 00:00:00.000000 startstop-1.0.8/PKG-INFO
```

### Comparing `startstop-1.0.7/.DS_Store` & `startstop-1.0.8/.DS_Store`

 * *Files identical despite different names*

### Comparing `startstop-1.0.7/example.py` & `startstop-1.0.8/example.py`

 * *Files identical despite different names*

### Comparing `startstop-1.0.7/startstop/__init__.py` & `startstop-1.0.8/startstop/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -54,14 +54,16 @@
             if self.label:
                 text = f" {self.label}"
             else:
                 text = ""
 
             print(f"TIMER{text}: {self.end - self.start :.{self.precision}f} sec")
 
+            return round(self.end - self.start, precision)
+
 
 t = StartStopTimer()
 
 
 class StartStopTimerContext:
     def __init__(self, label: str = "", precision: int = 3):
         self.label = label
@@ -75,13 +77,10 @@
 
         if self.label:
             text = f" {self.label}"
         else:
             text = ""
 
         print(f"TIMER{text}: {self.end - self.start :.{self.precision}f} sec")
-        
-        return round(self.end - self.start, precision)
-        
 
 
 tc = StartStopTimerContext
```

### Comparing `startstop-1.0.7/.gitignore` & `startstop-1.0.8/.gitignore`

 * *Files identical despite different names*

### Comparing `startstop-1.0.7/LICENSE.txt` & `startstop-1.0.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `startstop-1.0.7/README.md` & `startstop-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `startstop-1.0.7/PKG-INFO` & `startstop-1.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: startstop
-Version: 1.0.7
+Version: 1.0.8
 Summary: Start and stop a python profiler
 Project-URL: homepage, https://github.com/1081/startstop
 License-Expression: MIT
 License-File: LICENSE.txt
 Keywords: profiler,simple
 Requires-Python: >=3.7
 Requires-Dist: pyinstrument
```

