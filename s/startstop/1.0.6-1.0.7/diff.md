# Comparing `tmp/startstop-1.0.6.tar.gz` & `tmp/startstop-1.0.7.tar.gz`

## Comparing `startstop-1.0.6.tar` & `startstop-1.0.7.tar`

### file list

```diff
@@ -1,9 +1,10 @@
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 startstop-1.0.6/.DS_Store
--rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 startstop-1.0.6/example.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 startstop-1.0.6/startstop/__about__.py
--rw-r--r--   0        0        0     2050 2020-02-02 00:00:00.000000 startstop-1.0.6/startstop/__init__.py
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 startstop-1.0.6/.gitignore
--rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 startstop-1.0.6/LICENSE.txt
--rw-r--r--   0        0        0     1240 2020-02-02 00:00:00.000000 startstop-1.0.6/README.md
--rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 startstop-1.0.6/pyproject.toml
--rw-r--r--   0        0        0     1560 2020-02-02 00:00:00.000000 startstop-1.0.6/PKG-INFO
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 startstop-1.0.7/.DS_Store
+-rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 startstop-1.0.7/example.py
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 startstop-1.0.7/.vscode/settings.json
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 startstop-1.0.7/startstop/__about__.py
+-rw-r--r--   0        0        0     2123 2020-02-02 00:00:00.000000 startstop-1.0.7/startstop/__init__.py
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 startstop-1.0.7/.gitignore
+-rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 startstop-1.0.7/LICENSE.txt
+-rw-r--r--   0        0        0     1254 2020-02-02 00:00:00.000000 startstop-1.0.7/README.md
+-rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 startstop-1.0.7/pyproject.toml
+-rw-r--r--   0        0        0     1574 2020-02-02 00:00:00.000000 startstop-1.0.7/PKG-INFO
```

### Comparing `startstop-1.0.6/.DS_Store` & `startstop-1.0.7/.DS_Store`

 * *Files 10% similar despite different names*

```diff
@@ -60,46 +60,46 @@
 000003b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000003c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000003d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000003e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000003f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000400: 0000 0000 0000 0000 0000 0010 0000 0004  ................
 00000410: 002e 0067 0069 0074 6c67 3153 636f 6d70  ...g.i.tlg1Scomp
-00000420: 0000 0000 0000 9059 0000 0004 002e 0067  .......Y.......g
+00000420: 0000 0000 0000 b8c1 0000 0004 002e 0067  ...............g
 00000430: 0069 0074 6d6f 4444 626c 6f62 0000 0008  .i.tmoDDblob....
-00000440: 3c4b 5f0c 60f0 c441 0000 0004 002e 0067  <K_.`..A.......g
+00000440: 5eb4 e211 e2f6 c441 0000 0004 002e 0067  ^......A.......g
 00000450: 0069 0074 6d6f 6444 626c 6f62 0000 0008  .i.tmodDblob....
-00000460: 3c4b 5f0c 60f0 c441 0000 0004 002e 0067  <K_.`..A.......g
+00000460: 5eb4 e211 e2f6 c441 0000 0004 002e 0067  ^......A.......g
 00000470: 0069 0074 7068 3153 636f 6d70 0000 0000  .i.tph1Scomp....
-00000480: 0004 2000 0000 0004 0064 0069 0073 0074  .. ......d.i.s.t
-00000490: 6c67 3153 636f 6d70 0000 0000 0000 6483  lg1Scomp......d.
+00000480: 0005 1000 0000 0004 0064 0069 0073 0074  .........d.i.s.t
+00000490: 6c67 3153 636f 6d70 0000 0000 0000 9742  lg1Scomp.......B
 000004a0: 0000 0004 0064 0069 0073 0074 6d6f 4444  .....d.i.s.tmoDD
-000004b0: 626c 6f62 0000 0008 aaa3 728d 5ff0 c441  blob......r._..A
+000004b0: 626c 6f62 0000 0008 34e6 c59a f0f4 c441  blob....4......A
 000004c0: 0000 0004 0064 0069 0073 0074 6d6f 6444  .....d.i.s.tmodD
-000004d0: 626c 6f62 0000 0008 aaa3 728d 5ff0 c441  blob......r._..A
+000004d0: 626c 6f62 0000 0008 34e6 c59a f0f4 c441  blob....4......A
 000004e0: 0000 0004 0064 0069 0073 0074 7068 3153  .....d.i.s.tph1S
-000004f0: 636f 6d70 0000 0000 0000 a000 0000 0009  comp............
+000004f0: 636f 6d70 0000 0000 0000 e000 0000 0009  comp............
 00000500: 0073 0074 0061 0072 0074 0073 0074 006f  .s.t.a.r.t.s.t.o
 00000510: 0070 6c67 3153 636f 6d70 0000 0000 0000  .plg1Scomp......
-00000520: 055c 0000 0009 0073 0074 0061 0072 0074  .\.....s.t.a.r.t
+00000520: 13ea 0000 0009 0073 0074 0061 0072 0074  .......s.t.a.r.t
 00000530: 0073 0074 006f 0070 6d6f 4444 626c 6f62  .s.t.o.pmoDDblob
-00000540: 0000 0008 30cc a76b 5ff0 c441 0000 0009  ....0..k_..A....
+00000540: 0000 0008 ef8b 1973 f0f4 c441 0000 0009  .......s...A....
 00000550: 0073 0074 0061 0072 0074 0073 0074 006f  .s.t.a.r.t.s.t.o
-00000560: 0070 6d6f 6444 626c 6f62 0000 0008 30cc  .pmodDblob....0.
-00000570: a76b 5ff0 c441 0000 0009 0073 0074 0061  .k_..A.....s.t.a
+00000560: 0070 6d6f 6444 626c 6f62 0000 0008 ef8b  .pmodDblob......
+00000570: 1973 f0f4 c441 0000 0009 0073 0074 0061  .s...A.....s.t.a
 00000580: 0072 0074 0073 0074 006f 0070 7068 3153  .r.t.s.t.o.pph1S
 00000590: 636f 6d70 0000 0000 0000 3000 0000 0004  comp......0.....
 000005a0: 0076 0065 006e 0076 6c67 3153 636f 6d70  .v.e.n.vlg1Scomp
-000005b0: 0000 0000 037b e326 0000 0004 0076 0065  .....{.&.....v.e
+000005b0: 0000 0000 037b fb2a 0000 0004 0076 0065  .....{.*.....v.e
 000005c0: 006e 0076 6d6f 4444 626c 6f62 0000 0008  .n.vmoDDblob....
-000005d0: 9190 0383 59f0 c441 0000 0004 0076 0065  ....Y..A.....v.e
+000005d0: ba70 e411 e2f6 c441 0000 0004 0076 0065  .p.....A.....v.e
 000005e0: 006e 0076 6d6f 6444 626c 6f62 0000 0008  .n.vmodDblob....
-000005f0: 9190 0383 59f0 c441 0000 0004 0076 0065  ....Y..A.....v.e
+000005f0: ba70 e411 e2f6 c441 0000 0004 0076 0065  .p.....A.....v.e
 00000600: 006e 0076 7068 3153 636f 6d70 0000 0000  .n.vph1Scomp....
-00000610: 040f b000 0000 0000 0000 0000 0000 0000  ................
+00000610: 040f d000 0000 0000 0000 0000 0000 0000  ................
 00000620: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000630: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000640: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000650: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000660: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000670: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000680: 0000 0000 0000 0000 0000 0000 0000 0000  ................
```

### Comparing `startstop-1.0.6/example.py` & `startstop-1.0.7/example.py`

 * *Files identical despite different names*

### Comparing `startstop-1.0.6/startstop/__init__.py` & `startstop-1.0.7/startstop/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -75,10 +75,13 @@
 
         if self.label:
             text = f" {self.label}"
         else:
             text = ""
 
         print(f"TIMER{text}: {self.end - self.start :.{self.precision}f} sec")
+        
+        return round(self.end - self.start, precision)
+        
 
 
 tc = StartStopTimerContext
```

### Comparing `startstop-1.0.6/.gitignore` & `startstop-1.0.7/.gitignore`

 * *Files identical despite different names*

### Comparing `startstop-1.0.6/LICENSE.txt` & `startstop-1.0.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `startstop-1.0.6/README.md` & `startstop-1.0.7/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,74 +1,87 @@
 # startstop
+
 A simple way to start and stop a Python profiler ([pyinstument](https://github.com/joerick/pyinstrument)) and view the results in the browser.
 
 [![PyPI - Version](https://img.shields.io/pypi/v/startstop.svg)](https://pypi.org/project/startstop)
 
 -----
 
 ## Installation
 
 ```console
 pip install startstop
 ```
 
 ## Usage
+
 ```python
 from startstop import t, tc, p, pc
 ```
 
 ### Simple timer
+
 ```python
 t()
 # This is where your code goes.
 t()
 ```
+
 TIMER: 0.024 sec
 
 ```python
 t(label="your label", precision=2)
 # This is where your code goes.
 t()
 ```
+
 TIMER your label: 0.02 sec
 
 ### Simple timer as contex manager
+
 ```python
 with tc():
     # This is where your code goes.
 ```
+
 TIMER: 0.024 sec
 
 ```python
 with tc(label="your label", precision=2):
     # This is where your code goes.
 ```
-TIMER your label: 0.02 sec
 
+TIMER your label: 0.02 sec
 
 ### Profiler
+
 ```python
 p()
 # This is where your code goes.
 p()
 ```
+
 --> Browser output
 
 ```python
 p(interval=0.01, async_mode="disabled")
 # This is where your code goes.
 p()
 ```
+
 --> Browser output
 
 ### Profiler as context manager
+
 ```python
 with pc():
     # This is where your code goes.
 ```
+
 --> Browser output
 
 ```python
 with pc(interval=0.002, async_mode="strict"):
     # This is where your code goes.
 ```
---> Browser output
+
+--> Browser output
```

### Comparing `startstop-1.0.6/PKG-INFO` & `startstop-1.0.7/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,86 +1,99 @@
 Metadata-Version: 2.1
 Name: startstop
-Version: 1.0.6
+Version: 1.0.7
 Summary: Start and stop a python profiler
 Project-URL: homepage, https://github.com/1081/startstop
 License-Expression: MIT
 License-File: LICENSE.txt
 Keywords: profiler,simple
 Requires-Python: >=3.7
 Requires-Dist: pyinstrument
 Description-Content-Type: text/markdown
 
 # startstop
+
 A simple way to start and stop a Python profiler ([pyinstument](https://github.com/joerick/pyinstrument)) and view the results in the browser.
 
 [![PyPI - Version](https://img.shields.io/pypi/v/startstop.svg)](https://pypi.org/project/startstop)
 
 -----
 
 ## Installation
 
 ```console
 pip install startstop
 ```
 
 ## Usage
+
 ```python
 from startstop import t, tc, p, pc
 ```
 
 ### Simple timer
+
 ```python
 t()
 # This is where your code goes.
 t()
 ```
+
 TIMER: 0.024 sec
 
 ```python
 t(label="your label", precision=2)
 # This is where your code goes.
 t()
 ```
+
 TIMER your label: 0.02 sec
 
 ### Simple timer as contex manager
+
 ```python
 with tc():
     # This is where your code goes.
 ```
+
 TIMER: 0.024 sec
 
 ```python
 with tc(label="your label", precision=2):
     # This is where your code goes.
 ```
-TIMER your label: 0.02 sec
 
+TIMER your label: 0.02 sec
 
 ### Profiler
+
 ```python
 p()
 # This is where your code goes.
 p()
 ```
+
 --> Browser output
 
 ```python
 p(interval=0.01, async_mode="disabled")
 # This is where your code goes.
 p()
 ```
+
 --> Browser output
 
 ### Profiler as context manager
+
 ```python
 with pc():
     # This is where your code goes.
 ```
+
 --> Browser output
 
 ```python
 with pc(interval=0.002, async_mode="strict"):
     # This is where your code goes.
 ```
---> Browser output
+
+--> Browser output
```

