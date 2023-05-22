# Comparing `tmp/py3d-0.0.90.tar.gz` & `tmp/py3d-0.0.91.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py3d-0.0.90.tar", last modified: Sun May 21 15:53:00 2023, max compression
+gzip compressed data, was "py3d-0.0.91.tar", last modified: Mon May 22 17:31:58 2023, max compression
```

## Comparing `py3d-0.0.90.tar` & `py3d-0.0.91.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-21 15:53:00.229894 py3d-0.0.90/
--rw-r--r--   0 runner    (1001) docker     (122)     2031 2023-05-21 15:53:00.229894 py3d-0.0.90/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1640 2023-05-21 15:52:48.000000 py3d-0.0.90/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-21 15:53:00.229894 py3d-0.0.90/py3d/
--rw-r--r--   0 runner    (1001) docker     (122)      178 2023-05-21 15:52:48.000000 py3d-0.0.90/py3d/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    26933 2023-05-21 15:52:48.000000 py3d-0.0.90/py3d/core.py
--rw-r--r--   0 runner    (1001) docker     (122)    22266 2023-05-21 15:52:48.000000 py3d-0.0.90/py3d/viewer.html
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-21 15:53:00.229894 py3d-0.0.90/py3d.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     2031 2023-05-21 15:53:00.000000 py3d-0.0.90/py3d.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      204 2023-05-21 15:53:00.000000 py3d-0.0.90/py3d.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-21 15:53:00.000000 py3d-0.0.90/py3d.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       26 2023-05-21 15:53:00.000000 py3d-0.0.90/py3d.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        5 2023-05-21 15:53:00.000000 py3d-0.0.90/py3d.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-21 15:53:00.229894 py3d-0.0.90/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1457 2023-05-21 15:52:48.000000 py3d-0.0.90/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 17:31:58.946662 py3d-0.0.91/
+-rw-r--r--   0 runner    (1001) docker     (122)     2031 2023-05-22 17:31:58.946662 py3d-0.0.91/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1640 2023-05-22 17:31:49.000000 py3d-0.0.91/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 17:31:58.946662 py3d-0.0.91/py3d/
+-rw-r--r--   0 runner    (1001) docker     (122)      178 2023-05-22 17:31:49.000000 py3d-0.0.91/py3d/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    26933 2023-05-22 17:31:49.000000 py3d-0.0.91/py3d/core.py
+-rw-r--r--   0 runner    (1001) docker     (122)    22511 2023-05-22 17:31:49.000000 py3d-0.0.91/py3d/viewer.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 17:31:58.946662 py3d-0.0.91/py3d.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     2031 2023-05-22 17:31:58.000000 py3d-0.0.91/py3d.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      204 2023-05-22 17:31:58.000000 py3d-0.0.91/py3d.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-22 17:31:58.000000 py3d-0.0.91/py3d.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       26 2023-05-22 17:31:58.000000 py3d-0.0.91/py3d.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        5 2023-05-22 17:31:58.000000 py3d-0.0.91/py3d.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-22 17:31:58.946662 py3d-0.0.91/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1457 2023-05-22 17:31:49.000000 py3d-0.0.91/setup.py
```

### Comparing `py3d-0.0.90/PKG-INFO` & `py3d-0.0.91/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py3d
-Version: 0.0.90
+Version: 0.0.91
 Summary: py3d is a 3d computational geometry library that deals with 3d data in batches. And it embedded an interactive viewer that can work in jupyter notebook.
 Home-page: https://tumiz.github.io/scenario/
 Author: Tumiz
 Author-email: hh11698@163.com
 License: GPL-3.0 License
 Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown
```

### Comparing `py3d-0.0.90/README.md` & `py3d-0.0.91/README.md`

 * *Files identical despite different names*

### Comparing `py3d-0.0.90/py3d/core.py` & `py3d-0.0.91/py3d/core.py`

 * *Files identical despite different names*

### Comparing `py3d-0.0.90/py3d/viewer.html` & `py3d-0.0.91/py3d/viewer.html`

 * *Files 2% similar despite different names*

```diff
@@ -17,16 +17,16 @@
                 0, 0, 1, 0,
                 0, 0, 0, 1]
         }
         static orthographic(fovy, aspect, near, far, distance) {
             return [
                 1 / aspect / distance / Math.tan(fovy / 2), 0, 0, 0,
                 0, 1 / distance / Math.tan(fovy / 2), 0, 0,
-                0, 0, -1 / (near - far), 0,
-                0, 0, -near / (far - near), 1]
+                0, 0, 1 / (near - far), 0,
+                0, 0, near / (far - near), 1]
         }
         static perspective(fovy, aspect, near, far) {
             const f = 1 / Math.tan(fovy / 2)
             return [
                 f / aspect, 0, 0, 0,
                 0, f, 0, 0,
                 0, 0, -(near + far) / (far - near), -1,
@@ -91,31 +91,30 @@
         }
         static vec3_range(array) {
             let x = array.filter((v, i) => i % 3 == 0)
             let y = array.filter((v, i) => i % 3 == 1)
             let z = array.filter((v, i) => i % 3 == 2)
             return [Math.min(...x), Math.max(...x), Math.min(...y), Math.max(...y), Math.min(...z), Math.max(...z)]
         }
-        static ticks(min, max) {
+        static ticks(min, max, step) {
             if (max <= min) {
                 return [[min], min, max, 0]
             }
-            let dig = Math.round(Math.log10((max - min) / 5))
-            let step = Math.pow(10, dig)
+            let dig = Math.round(Math.log10(step))
             let tick_min = min - min % step
             if (min < tick_min) {
                 tick_min -= step
             }
             let tick_max = max - max % step
             if (max > tick_max) {
                 tick_max += step
             }
             let size = Math.ceil((tick_max - tick_min) / step) + 1
-            let ticks = Array.from({ length: size }, (v, i) => (tick_min + step * i).toFixed(Math.max(-dig, 0)))
-            return [ticks, tick_min, tick_max, tick_max - tick_min]
+            let ticks = Array.from({ length: size }, (v, i) => Number((tick_min + step * i).toFixed(Math.max(-dig, 0))))
+            return [ticks, ticks[0], ticks[ticks.length - 1]]
         }
     }
     class Camera {
         PERSPECTIVE = "P"
         ORTHOGRAPHIC = "O"
         constructor(type, fovy, aspect, near, far, min, max) {
             this.fovy = fovy
@@ -124,15 +123,15 @@
             this.far = -far
             this.center = [(min[0] + max[0]) / 2, (min[1] + max[1]) / 2, (min[2] + max[2]) / 2]
             let ysize = Math.max((max[0] - min[0]) / this.aspect, max[1] - min[1]) + 2
             Object.defineProperty(this, "origin_translation", {
                 "value": [0, 0, ysize / 2 / Math.tan(this.fovy / 2)],
                 "writable": false
             })
-            this.translation = this.origin_translation
+            this.translation = structuredClone(this.origin_translation)
             this.rotation = mat.identity() // intrinsic
             this.type = type
             this.update_projection()
         }
         position() {
             let p = mat.vm(mat.vm(this.center, this.rotation), mat.translation(this.translation))
             return "camera position = " + p[0].toFixed(3) + ", " + p[1].toFixed(3) + ", " + p[2].toFixed(3)
@@ -142,18 +141,22 @@
                 this.fovy,
                 this.aspect,
                 this.near,
                 this.far,
                 this.translation[2]) : mat.perspective(this.fovy, this.aspect, this.near, this.far)
         }
         reset() {
-            this.translation = this.origin_translation
+            Object.assign(this.translation, this.origin_translation)
             this.rotation = mat.identity()
             this.update_projection()
         }
+        resolution(width) {
+            let p = mat.vm([1, 0, this.translation[2]], this.projection)
+            return Math.abs(2 * p[3] / p[0] / width)
+        }
         modelview() {
             return mat.mms(
                 mat.I(mat.translation(this.center)),
                 mat.I(this.rotation),
                 mat.I(mat.translation(this.translation)),
                 this.projection
             )
@@ -455,24 +458,26 @@
                         } else if (obj.mode) {
                             this.set_attribute("position", obj.vertex, 3)
                             this.set_attribute("color", obj.color, 4)
                             this.gl.drawArrays(this.gl[obj.mode], 0, obj.vertex.length / 3)
                         }
                     }
                     if (this.toolbar.btn_grid.style.background == "grey") {
-                        this.grid(this.min, this.max, modelview)
+                        let resolution = this.camera.resolution(this.canvas.width)
+                        this.grid(this.min, this.max, modelview, resolution)
                     }
                     break
                 }
             }
         }
-        grid(min, max, modelview) {
-            const [x_ticks, x_tick_min, x_tick_max, x_range] = mat.ticks(min[0], max[0])
-            const [y_ticks, y_tick_min, y_tick_max, y_range] = mat.ticks(min[1], max[1])
-            const [z_ticks, z_tick_min, z_tick_max, z_range] = mat.ticks(min[2], max[2])
+        grid(min, max, modelview, resolution) {
+            let step = 50 * resolution// meter per pixel
+            const [x_ticks, x_tick_min, x_tick_max] = mat.ticks(min[0], max[0], step)
+            const [y_ticks, y_tick_min, y_tick_max] = mat.ticks(min[1], max[1], step)
+            const [z_ticks, z_tick_min, z_tick_max] = mat.ticks(min[2], max[2], step)
             let lines = []
             for (let x of x_ticks) {
                 lines.push(x, y_tick_min, z_tick_min, x, y_tick_max, z_tick_min)
                 lines.push(x, y_tick_min, z_tick_min, x, y_tick_min, z_tick_max)
                 this.drawText(x, [x, y_tick_min, z_tick_min], "grey", modelview)
             }
             for (let y of y_ticks) {
@@ -481,16 +486,16 @@
                 this.drawText(y, [x_tick_min, y, z_tick_min], "grey", modelview)
             }
             for (let z of z_ticks) {
                 lines.push(x_tick_min, y_tick_min, z, x_tick_max, y_tick_min, z)
                 lines.push(x_tick_min, y_tick_min, z, x_tick_min, y_tick_max, z)
                 this.drawText(z, [x_tick_min, y_tick_min, z], "grey", modelview)
             }
-            this.drawText("X", [x_tick_max + x_range * 0.1, y_tick_min, z_tick_min], "grey", modelview)
-            this.drawText("Y", [x_tick_min, y_tick_max + y_range * 0.1, z_tick_min], "grey", modelview)
-            this.drawText("Z", [x_tick_min - x_range * 0.1, y_tick_min - y_range * 0.1, z_tick_max + z_range * 0.1], "grey", modelview)
+            this.drawText("X", [x_tick_max + step, y_tick_min, z_tick_min], "grey", modelview)
+            this.drawText("Y", [x_tick_min, y_tick_max + step, z_tick_min], "grey", modelview)
+            this.drawText("Z", [x_tick_min, y_tick_min, z_tick_max + step], "grey", modelview)
             this.set_attribute("position", lines, 3)
             this.set_attribute("color", Array.from({ length: lines.length / 3 * 4 }, (v, i) => i % 4 == 3 ? 1 : 0.5), 4)
             this.gl.drawArrays(this.gl.LINES, 0, lines.length / 3)
         }
     }
 </script>
```

### Comparing `py3d-0.0.90/py3d.egg-info/PKG-INFO` & `py3d-0.0.91/py3d.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py3d
-Version: 0.0.90
+Version: 0.0.91
 Summary: py3d is a 3d computational geometry library that deals with 3d data in batches. And it embedded an interactive viewer that can work in jupyter notebook.
 Home-page: https://tumiz.github.io/scenario/
 Author: Tumiz
 Author-email: hh11698@163.com
 License: GPL-3.0 License
 Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown
```

### Comparing `py3d-0.0.90/setup.py` & `py3d-0.0.91/setup.py`

 * *Files identical despite different names*

