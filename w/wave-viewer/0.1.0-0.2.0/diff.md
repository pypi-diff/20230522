# Comparing `tmp/wave_viewer-0.1.0.tar.gz` & `tmp/wave_viewer-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wave_viewer-0.1.0.tar", max compression
+gzip compressed data, was "wave_viewer-0.2.0.tar", max compression
```

## Comparing `wave_viewer-0.1.0.tar` & `wave_viewer-0.2.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1067 2023-05-18 02:42:58.397916 wave_viewer-0.1.0/LICENSE
--rw-r--r--   0        0        0      417 2023-05-18 02:43:50.675253 wave_viewer-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1061 2023-05-18 02:38:54.638436 wave_viewer-0.1.0/README.md
--rw-r--r--   0        0        0      414 2023-05-18 02:28:38.749597 wave_viewer-0.1.0/wave_viewer/__init__.py
--rw-r--r--   0        0        0     4245 2023-05-18 02:34:00.545357 wave_viewer-0.1.0/wave_viewer/_controller.py
--rw-r--r--   0        0        0     6246 2023-05-18 02:21:29.099933 wave_viewer-0.1.0/wave_viewer/_viewer.py
--rw-r--r--   0        0        0     1626 1970-01-01 00:00:00.000000 wave_viewer-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-05-18 02:42:58.397916 wave_viewer-0.2.0/LICENSE
+-rw-r--r--   0        0        0      837 2023-05-22 20:05:58.786520 wave_viewer-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1061 2023-05-18 02:38:54.638436 wave_viewer-0.2.0/README.md
+-rw-r--r--   0        0        0      714 2023-05-22 20:04:53.097291 wave_viewer-0.2.0/wave_viewer/__init__.py
+-rw-r--r--   0        0        0     4878 2023-05-22 20:04:53.098329 wave_viewer-0.2.0/wave_viewer/_controller.py
+-rw-r--r--   0        0        0     6048 2023-05-22 20:04:53.099012 wave_viewer-0.2.0/wave_viewer/_viewer.py
+-rw-r--r--   0        0        0     1859 1970-01-01 00:00:00.000000 wave_viewer-0.2.0/PKG-INFO
```

### Comparing `wave_viewer-0.1.0/LICENSE` & `wave_viewer-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `wave_viewer-0.1.0/README.md` & `wave_viewer-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `wave_viewer-0.1.0/wave_viewer/_controller.py` & `wave_viewer-0.2.0/wave_viewer/_controller.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,30 +11,41 @@
 
 
 class WaveViewer:
     """A simple GUI for viewing waveforms.
 
     It plots the waveform with vispy in a separate process. The GUI is built with
     PySide6.
+
+
+    Parameters
+    ----------
+    daemon : bool, optional
+        If True, the viewer process is a daemon process. This means that the
+        process will be terminated when the main process exits. If False, the
+        viewer process will continue to run after the main process exits. In this
+        case, the viewer process must be closed manually by calling the `close`
+        method. The default is True.
     """
 
-    def __init__(self) -> None:
+    def __init__(self, daemon: bool = True) -> None:
         self._rconn, self._wconn = mp.Pipe(duplex=False)
-        self._process = mp.Process(target=main, args=(self._rconn,))
+        self._process = mp.Process(target=main, args=(self._rconn,), daemon=daemon)
         self._process.start()
 
     def _ensure_open(self) -> None:
         if not self._process.is_alive():
             raise RuntimeError("WaveViewer is closed")
 
     def add_line(self, name: str, t: np.ndarray, ys: list, offset: float) -> None:
         """Add a line to the plot.
 
         The method accepts a list of y values and plots them against the time axis.
-        The y values are plotted with different colors.
+        The y values are plotted with different colors. The name will also be added
+        to the right of the line.
 
         If a line with the same name already exists, it is replaced.
 
         Parameters
         ----------
         name : str
             The name of the line.
@@ -134,7 +145,11 @@
 
     def close(self) -> None:
         """Close the WaveViewer."""
         self._process.terminate()
         self._process.join()
         self._wconn.close()
         self._rconn.close()
+
+    def wait(self) -> None:
+        """Wait for the WaveViewer to close."""
+        self._process.join()
```

### Comparing `wave_viewer-0.1.0/wave_viewer/_viewer.py` & `wave_viewer-0.2.0/wave_viewer/_viewer.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 """
 
 from multiprocessing.connection import Connection
 
 import numpy as np
 from PySide6.QtCore import QObject, Qt, QThread, Signal, Slot
 from PySide6.QtWidgets import QMainWindow
-from vispy import app, scene
+from vispy import scene
 from vispy.app import use_app
 
 
 class CanvasWrapper:
     def __init__(self):
         self._initialize_canvas()
         self.lines = {}
@@ -187,16 +187,7 @@
     window.closing.connect(source.stop, Qt.DirectConnection)
     source.finished.connect(thread.quit, Qt.DirectConnection)
     thread.finished.connect(source.deleteLater)
     window.show()
     thread.start()
     app.run()
     thread.wait(5000)
-
-
-if __name__ == "__main__":
-    app = use_app("PySide6")
-    app.create()
-    canvas_wrapper = CanvasWrapper()
-    win = WaveViewerWindow(canvas_wrapper)
-    win.show()
-    app.run()
```

### Comparing `wave_viewer-0.1.0/PKG-INFO` & `wave_viewer-0.2.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,23 +1,27 @@
 Metadata-Version: 2.1
 Name: wave-viewer
-Version: 0.1.0
+Version: 0.2.0
 Summary: A simple GUI for viewing waveforms.
+Home-page: https://github.com/kahojyun/wave-viewer
 License: MIT
 Author: Jiahao Yuan
 Author-email: kaho0769@qq.com
-Requires-Python: >=3.8,<3.12
+Requires-Python: >=3.7,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: importlib-metadata (>=1.0) ; python_version < "3.8"
 Requires-Dist: pyside6 (>=6.5.0,<7.0.0)
 Requires-Dist: vispy (>=0.13.0,<0.14.0)
+Project-URL: Repository, https://github.com/kahojyun/wave-viewer
 Description-Content-Type: text/markdown
 
 # Wave Viewer
 
 A simple GUI for viewing waveforms. It plots the waveform with vispy in a
 separate process. The GUI is built with PySide6.
```

