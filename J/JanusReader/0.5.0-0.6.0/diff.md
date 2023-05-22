# Comparing `tmp/JanusReader-0.5.0.tar.gz` & `tmp/JanusReader-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "JanusReader-0.5.0.tar", last modified: Wed May 10 08:10:10 2023, max compression
+gzip compressed data, was "JanusReader-0.6.0.tar", last modified: Mon May 22 13:31:29 2023, max compression
```

## Comparing `JanusReader-0.5.0.tar` & `JanusReader-0.6.0.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxr-xr-x   0 romolo.politi   (501) staff       (20)        0 2023-05-10 08:10:10.483035 JanusReader-0.5.0/
--rw-r--r--   0 romolo.politi   (501) staff       (20)      449 2023-05-10 08:10:10.482807 JanusReader-0.5.0/PKG-INFO
--rw-r--r--   0 romolo.politi   (501) staff       (20)      257 2023-05-10 08:09:29.000000 JanusReader-0.5.0/README.md
--rw-r--r--   0 romolo.politi   (501) staff       (20)      437 2023-05-10 08:08:52.000000 JanusReader-0.5.0/pyproject.toml
--rw-r--r--   0 romolo.politi   (501) staff       (20)       38 2023-05-10 08:10:10.483118 JanusReader-0.5.0/setup.cfg
-drwxr-xr-x   0 romolo.politi   (501) staff       (20)        0 2023-05-10 08:10:10.479426 JanusReader-0.5.0/src/
-drwxr-xr-x   0 romolo.politi   (501) staff       (20)        0 2023-05-10 08:10:10.481039 JanusReader-0.5.0/src/JanusReader/
--rw-r--r--   0 romolo.politi   (501) staff       (20)       88 2023-03-03 08:06:39.000000 JanusReader-0.5.0/src/JanusReader/__init__.py
--rw-r--r--   0 romolo.politi   (501) staff       (20)      103 2022-05-04 08:58:16.000000 JanusReader-0.5.0/src/JanusReader/exceptions.py
--rw-r--r--   0 romolo.politi   (501) staff       (20)    12458 2023-05-10 08:08:22.000000 JanusReader-0.5.0/src/JanusReader/janusReader.py
--rw-r--r--   0 romolo.politi   (501) staff       (20)     2302 2023-03-03 15:12:36.000000 JanusReader-0.5.0/src/JanusReader/vicar_head.py
-drwxr-xr-x   0 romolo.politi   (501) staff       (20)        0 2023-05-10 08:10:10.482456 JanusReader-0.5.0/src/JanusReader.egg-info/
--rw-r--r--   0 romolo.politi   (501) staff       (20)      449 2023-05-10 08:10:10.000000 JanusReader-0.5.0/src/JanusReader.egg-info/PKG-INFO
--rw-r--r--   0 romolo.politi   (501) staff       (20)      337 2023-05-10 08:10:10.000000 JanusReader-0.5.0/src/JanusReader.egg-info/SOURCES.txt
--rw-r--r--   0 romolo.politi   (501) staff       (20)        1 2023-05-10 08:10:10.000000 JanusReader-0.5.0/src/JanusReader.egg-info/dependency_links.txt
--rw-r--r--   0 romolo.politi   (501) staff       (20)       73 2023-05-10 08:10:10.000000 JanusReader-0.5.0/src/JanusReader.egg-info/requires.txt
--rw-r--r--   0 romolo.politi   (501) staff       (20)       12 2023-05-10 08:10:10.000000 JanusReader-0.5.0/src/JanusReader.egg-info/top_level.txt
+drwxr-xr-x   0 romolo.politi   (501) staff       (20)        0 2023-05-22 13:31:29.925830 JanusReader-0.6.0/
+-rw-r--r--   0 romolo.politi   (501) staff       (20)      449 2023-05-22 13:31:29.925626 JanusReader-0.6.0/PKG-INFO
+-rw-r--r--   0 romolo.politi   (501) staff       (20)      257 2023-05-10 08:09:29.000000 JanusReader-0.6.0/README.md
+-rw-r--r--   0 romolo.politi   (501) staff       (20)      437 2023-05-22 12:55:55.000000 JanusReader-0.6.0/pyproject.toml
+-rw-r--r--   0 romolo.politi   (501) staff       (20)       38 2023-05-22 13:31:29.925894 JanusReader-0.6.0/setup.cfg
+drwxr-xr-x   0 romolo.politi   (501) staff       (20)        0 2023-05-22 13:31:29.922310 JanusReader-0.6.0/src/
+drwxr-xr-x   0 romolo.politi   (501) staff       (20)        0 2023-05-22 13:31:29.924084 JanusReader-0.6.0/src/JanusReader/
+-rw-r--r--   0 romolo.politi   (501) staff       (20)       88 2023-03-03 08:06:39.000000 JanusReader-0.6.0/src/JanusReader/__init__.py
+-rw-r--r--   0 romolo.politi   (501) staff       (20)      103 2022-05-04 08:58:16.000000 JanusReader-0.6.0/src/JanusReader/exceptions.py
+-rw-r--r--   0 romolo.politi   (501) staff       (20)    13722 2023-05-22 13:19:55.000000 JanusReader-0.6.0/src/JanusReader/janusReader.py
+-rw-r--r--   0 romolo.politi   (501) staff       (20)     2302 2023-03-03 15:12:36.000000 JanusReader-0.6.0/src/JanusReader/vicar_head.py
+drwxr-xr-x   0 romolo.politi   (501) staff       (20)        0 2023-05-22 13:31:29.925333 JanusReader-0.6.0/src/JanusReader.egg-info/
+-rw-r--r--   0 romolo.politi   (501) staff       (20)      449 2023-05-22 13:31:29.000000 JanusReader-0.6.0/src/JanusReader.egg-info/PKG-INFO
+-rw-r--r--   0 romolo.politi   (501) staff       (20)      348 2023-05-22 13:31:29.000000 JanusReader-0.6.0/src/JanusReader.egg-info/SOURCES.txt
+-rw-r--r--   0 romolo.politi   (501) staff       (20)        1 2023-05-22 13:31:29.000000 JanusReader-0.6.0/src/JanusReader.egg-info/dependency_links.txt
+-rw-r--r--   0 romolo.politi   (501) staff       (20)       73 2023-05-22 13:31:29.000000 JanusReader-0.6.0/src/JanusReader.egg-info/requires.txt
+-rw-r--r--   0 romolo.politi   (501) staff       (20)       16 2023-05-22 13:31:29.000000 JanusReader-0.6.0/src/JanusReader.egg-info/top_level.txt
+-rwxr-xr-x   0 romolo.politi   (501) staff       (20)     1421 2023-05-22 11:20:37.000000 JanusReader-0.6.0/src/run.py
```

### Comparing `JanusReader-0.5.0/src/JanusReader/janusReader.py` & `JanusReader-0.6.0/src/JanusReader/janusReader.py`

 * *Files 8% similar despite different names*

```diff
@@ -78,15 +78,37 @@
         tb.add_row("Image Number","",str(self.imgNum))
         tb.add_row("Filter Number","", str(self.filtNumber))
         tb.add_row("Filter Name", "", self.filterName)
         tb.add_row("Filter Wheel Direction", "", self.filWheelDir)
         tb.add_row("Filter Snapin","", self.filSnapin)
         tb.add_row("Multifilter","", str(self.multifilter))
         return tb
-        
+
+class SubFrame:
+    def __init__(self,proc) -> None:
+        self.firstLine = int(getValue(proc, 'img:first_line'))
+        self.firstSample = int(getValue(proc, 'img:first_sample'))
+        self.lines = int(getValue(proc, 'img:lines'))
+        self.samples = int(getValue(proc, 'img:samples'))
+        self.subFrameType = getValue(proc, 'img:subframe_type')
+    
+    def Show(self):
+        tb = Table(expand=False, show_header=False,
+                   show_lines=False, box=box.SIMPLE_HEAD,
+                   title="SubFrame Parameters", title_style="italic yellow")
+        tb.add_column(style='yellow', justify='left')
+        tb.add_column()
+        tb.add_column()
+        tb.add_row("First Sample", "", str(self.firstSample))
+        tb.add_row("First Line", "", str(self.firstLine))
+        tb.add_row("Sample", "", str(self.samples))
+        tb.add_row("Lines", "", str(self.lines))
+        tb.add_row("Subframe Type", "", self.subFrameType)
+        return tb
+      
 class OnBoardProcessing:
     
     def __init__(self,proc):
         self.badPixelCorrection = int(getValue(
             proc, 'juice_janus:bad_pixel_correction'))
         self.badPixelMapName = getValue(
             proc, 'juice_janus:bad_pixel_map_name')
@@ -222,31 +244,36 @@
         obProc = getElement(idObs, "juice_janus:Onboard_Processing")
         self.onBoardProcessing=OnBoardProcessing(obProc)
         self.onGroundProcessing=None
         self.HK=None
         self.Downsamplig=None
         self.Exposure = float(getValue(idObs, 'img:exposure_duration'))
         self.onBoardCompression=None
-        self.subFrame=None
+        self.subFrame = SubFrame(getElement(doc, 'img:Subframe'))
         self.Header=None
         # self.image=None
         flObs = getElement(doc, 'pds:File_Area_Observational')
         img = getElement(flObs, "pds:Array_2D_Image")
         self.Offset = int(getValue(img, "pds:offset"))
         elem = img.getElementsByTagName("pds:Axis_Array")
         self.Samples = int(getValue(elem[1], "pds:elements"))
         self.Lines = int(getValue(elem[0], "pds:elements"))
         # console.print(timeCoord)
 
             
         # if self.Format == "HALF":
         if self.level.lower()=='raw':
+            self.console.print(self.Offset)
+            self.console.print(self.Lines, self.Samples)
+            self.console.print(self.fileName.stat().st_size)
+            self.console.print(self.Lines*self.Samples*2+self.Offset)
             with open(self.fileName, 'rb') as f:
                 f.seek(self.Offset)
-                self.image=np.reshape(np.frombuffer(f.read(), dtype=np.uint16),(self.Lines,self.Samples))
+                self.image = np.reshape(np.frombuffer(f.read(
+                    self.Lines * self.Samples * 2), dtype=np.uint16), (self.Lines, self.Samples))
         else:
             with open(self.fileName, 'rb') as f:
                 self.image = np.reshape(np.frombuffer(
                     f.read(), dtype=np.float32), (self.Lines, self.Samples))
             
         # np.reshape(self.image,(self.Nl,self.Ns))
         
@@ -280,15 +307,14 @@
         tb.add_section()
         # tb.add_row("On Board processing", "",str(self.onBoardProcessing))
         tb.add_row("On Ground Processing","",str(self.onGroundProcessing))
         tb.add_row("HK","",str(self.HK))
         tb.add_row("Downsampling","",str(self.Downsamplig))
         tb.add_row("Exposure","",str(self.Exposure))
         tb.add_row("On Board Compression","",str(self.onBoardCompression))
-        tb.add_row("SubFrame","",str(self.subFrame))
         tb.add_row("Header","", str(self.Header))
         # tb.add_row("Image","",str(self.image))
         if all:
-            col = Columns([tb, self.AcquisitionParameter.Show(), self.onBoardProcessing.Show()],expand=False)
+            col = Columns([tb, self.AcquisitionParameter.Show(), self.onBoardProcessing.Show(), self.subFrame.Show()],expand=False)
         else:
             col = tb
         self.console.print(Panel(col ,title=f"Label for {self.fileName.name}", border_style='yellow', expand=False))
```

### Comparing `JanusReader-0.5.0/src/JanusReader/vicar_head.py` & `JanusReader-0.6.0/src/JanusReader/vicar_head.py`

 * *Files identical despite different names*

