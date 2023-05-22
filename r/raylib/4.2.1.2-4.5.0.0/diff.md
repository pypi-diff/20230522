# Comparing `tmp/raylib-4.2.1.2.tar.gz` & `tmp/raylib-4.5.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "raylib-4.2.1.2.tar", last modified: Tue Oct 18 18:56:55 2022, max compression
+gzip compressed data, was "raylib-4.5.0.0.tar", last modified: Mon May 22 17:05:13 2023, max compression
```

## Comparing `raylib-4.2.1.2.tar` & `raylib-4.5.0.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-10-18 18:56:55.210680 raylib-4.2.1.2/
--rw-r--r--   0 runner    (1001) docker     (116)    14198 2022-10-18 18:55:00.000000 raylib-4.2.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (116)      178 2022-10-18 18:55:00.000000 raylib-4.2.1.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (116)     5357 2022-10-18 18:56:55.210680 raylib-4.2.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     4728 2022-10-18 18:55:00.000000 raylib-4.2.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-10-18 18:56:55.206680 raylib-4.2.1.2/pyray/
--rw-r--r--   0 runner    (1001) docker     (116)     4249 2022-10-18 18:55:00.000000 raylib-4.2.1.2/pyray/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)   156999 2022-10-18 18:55:00.000000 raylib-4.2.1.2/pyray/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-10-18 18:56:55.210680 raylib-4.2.1.2/raylib/
--rw-r--r--   0 runner    (1001) docker     (116)      919 2022-10-18 18:55:00.000000 raylib-4.2.1.2/raylib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)   144674 2022-10-18 18:55:00.000000 raylib-4.2.1.2/raylib/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (116)     7763 2022-10-18 18:55:00.000000 raylib-4.2.1.2/raylib/build.py
--rw-r--r--   0 runner    (1001) docker     (116)     1523 2022-10-18 18:55:00.000000 raylib-4.2.1.2/raylib/colors.py
--rw-r--r--   0 runner    (1001) docker     (116)      375 2022-10-18 18:55:00.000000 raylib-4.2.1.2/raylib/defines.py
--rw-r--r--   0 runner    (1001) docker     (116)    17057 2022-10-18 18:55:00.000000 raylib-4.2.1.2/raylib/enums.py
--rw-r--r--   0 runner    (1001) docker     (116)       23 2022-10-18 18:55:00.000000 raylib-4.2.1.2/raylib/version.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-10-18 18:56:55.210680 raylib-4.2.1.2/raylib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     5357 2022-10-18 18:56:55.000000 raylib-4.2.1.2/raylib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      359 2022-10-18 18:56:55.000000 raylib-4.2.1.2/raylib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2022-10-18 18:56:55.000000 raylib-4.2.1.2/raylib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)       24 2022-10-18 18:56:55.000000 raylib-4.2.1.2/raylib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)       13 2022-10-18 18:56:55.000000 raylib-4.2.1.2/raylib.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)       38 2022-10-18 18:56:55.210680 raylib-4.2.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     1404 2022-10-18 18:55:00.000000 raylib-4.2.1.2/setup.py
--rw-r--r--   0 runner    (1001) docker     (116)       23 2022-10-18 18:55:00.000000 raylib-4.2.1.2/version.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 17:05:13.748835 raylib-4.5.0.0/
+-rw-r--r--   0 runner    (1001) docker     (122)    14198 2023-05-22 17:03:48.000000 raylib-4.5.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      178 2023-05-22 17:03:48.000000 raylib-4.5.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     5408 2023-05-22 17:05:13.748835 raylib-4.5.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     4728 2023-05-22 17:03:48.000000 raylib-4.5.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 17:05:13.744835 raylib-4.5.0.0/pyray/
+-rw-r--r--   0 runner    (1001) docker     (122)     4249 2023-05-22 17:03:48.000000 raylib-4.5.0.0/pyray/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)   159246 2023-05-22 17:03:48.000000 raylib-4.5.0.0/pyray/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 17:05:13.744835 raylib-4.5.0.0/raylib/
+-rw-r--r--   0 runner    (1001) docker     (122)      919 2023-05-22 17:03:48.000000 raylib-4.5.0.0/raylib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)   147056 2023-05-22 17:03:48.000000 raylib-4.5.0.0/raylib/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (122)     7763 2023-05-22 17:03:48.000000 raylib-4.5.0.0/raylib/build.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1523 2023-05-22 17:03:48.000000 raylib-4.5.0.0/raylib/colors.py
+-rw-r--r--   0 runner    (1001) docker     (122)      375 2023-05-22 17:03:48.000000 raylib-4.5.0.0/raylib/defines.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17237 2023-05-22 17:03:48.000000 raylib-4.5.0.0/raylib/enums.py
+-rw-r--r--   0 runner    (1001) docker     (122)       23 2023-05-22 17:03:48.000000 raylib-4.5.0.0/raylib/version.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 17:05:13.748835 raylib-4.5.0.0/raylib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     5408 2023-05-22 17:05:13.000000 raylib-4.5.0.0/raylib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      359 2023-05-22 17:05:13.000000 raylib-4.5.0.0/raylib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-22 17:05:13.000000 raylib-4.5.0.0/raylib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       24 2023-05-22 17:05:13.000000 raylib-4.5.0.0/raylib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       13 2023-05-22 17:05:13.000000 raylib-4.5.0.0/raylib.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-22 17:05:13.748835 raylib-4.5.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1454 2023-05-22 17:03:48.000000 raylib-4.5.0.0/setup.py
+-rw-r--r--   0 runner    (1001) docker     (122)       23 2023-05-22 17:03:48.000000 raylib-4.5.0.0/version.py
```

### Comparing `raylib-4.2.1.2/LICENSE` & `raylib-4.5.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `raylib-4.2.1.2/PKG-INFO` & `raylib-4.5.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 Metadata-Version: 2.1
 Name: raylib
-Version: 4.2.1.2
+Version: 4.5.0.0
 Summary: Python CFFI bindings for Raylib
 Home-page: https://github.com/electronstudio/raylib-python-cffi
 Author: Electron Studio
 Author-email: github@electronstudio.co.uk
 License: EPL-2.0
 Classifier: License :: OSI Approved :: Eclipse Public License 2.0 (EPL-2.0)
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# Python Bindings for Raylib 4.2
+# Python Bindings for Raylib 4.5
 
 New CFFI API static bindings.
 * Automatically generated to be as close as possible to 
 original Raylib.
 * Faster, fewer bugs and easier to maintain than ctypes.
 * Commercial-friendly license.
 * Docstrings and auto-completion.
```

### Comparing `raylib-4.2.1.2/README.md` & `raylib-4.5.0.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Python Bindings for Raylib 4.2
+# Python Bindings for Raylib 4.5
 
 New CFFI API static bindings.
 * Automatically generated to be as close as possible to 
 original Raylib.
 * Faster, fewer bugs and easier to maintain than ctypes.
 * Commercial-friendly license.
 * Docstrings and auto-completion.
```

### Comparing `raylib-4.2.1.2/pyray/__init__.py` & `raylib-4.5.0.0/pyray/__init__.py`

 * *Files identical despite different names*

### Comparing `raylib-4.2.1.2/pyray/__init__.pyi` & `raylib-4.5.0.0/pyray/__init__.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 from typing import Any
 
 
 def pointer(struct):
     ...
 
+def attach_audio_mixed_processor(processor: Any,) -> None:
+        """Attach audio stream processor to the entire audio pipeline"""
+        ...
 def attach_audio_stream_processor(stream: AudioStream,processor: Any,) -> None:
         """Attach audio stream processor to stream"""
         ...
 def begin_blend_mode(mode: int,) -> None:
         """Begin blending mode (alpha, additive, multiplied, subtract, custom)"""
         ...
 def begin_drawing() -> None:
@@ -51,14 +54,17 @@
         ...
 def check_collision_point_circle(point: Vector2,center: Vector2,radius: float,) -> bool:
         """Check if point is inside circle"""
         ...
 def check_collision_point_line(point: Vector2,p1: Vector2,p2: Vector2,threshold: int,) -> bool:
         """Check if point belongs to line created between two points [p1] and [p2] with defined margin in pixels [threshold]"""
         ...
+def check_collision_point_poly(point: Vector2,points: Any,pointCount: int,) -> bool:
+        """Check if point is within a polygon described by array of vertices"""
+        ...
 def check_collision_point_rec(point: Vector2,rec: Rectangle,) -> bool:
         """Check if point is inside rectangle"""
         ...
 def check_collision_point_triangle(point: Vector2,p1: Vector2,p2: Vector2,p3: Vector2,) -> bool:
         """Check if point is inside a triangle"""
         ...
 def check_collision_recs(rec1: Rectangle,rec2: Rectangle,) -> bool:
@@ -85,32 +91,41 @@
         """void ClosePhysics();
 
 CFFI C function from raylib._raylib_cffi.lib"""
         ...
 def close_window() -> None:
         """Close window and unload OpenGL context"""
         ...
-def codepoint_to_utf8(codepoint: int,byteSize: Any,) -> str:
+def codepoint_to_utf8(codepoint: int,utf8Size: Any,) -> str:
         """Encode one codepoint into UTF-8 byte array (array length returned as parameter)"""
         ...
 def color_alpha(color: Color,alpha: float,) -> Color:
         """Get color with alpha applied, alpha goes from 0.0f to 1.0f"""
         ...
 def color_alpha_blend(dst: Color,src: Color,tint: Color,) -> Color:
         """Get src alpha-blended into dst color with tint"""
         ...
+def color_brightness(color: Color,factor: float,) -> Color:
+        """Get color with brightness correction, brightness factor goes from -1.0f to 1.0f"""
+        ...
+def color_contrast(color: Color,contrast: float,) -> Color:
+        """Get color with contrast correction, contrast values between -1.0f and 1.0f"""
+        ...
 def color_from_hsv(hue: float,saturation: float,value: float,) -> Color:
         """Get a Color from HSV values, hue [0..360], saturation/value [0..1]"""
         ...
 def color_from_normalized(normalized: Vector4,) -> Color:
         """Get Color from normalized values [0..1]"""
         ...
 def color_normalize(color: Color,) -> Vector4:
         """Get Color normalized as float [0..1]"""
         ...
+def color_tint(color: Color,tint: Color,) -> Color:
+        """Get color multiplied with another color"""
+        ...
 def color_to_hsv(color: Color,) -> Vector3:
         """Get HSV values for a Color, hue [0..360], saturation/value [0..1]"""
         ...
 def color_to_int(color: Color,) -> int:
         """Get hexadecimal value for a Color"""
         ...
 def compress_data(data: str,dataSize: int,compDataSize: Any,) -> str:
@@ -138,14 +153,17 @@
         """Decompress data (DEFLATE algorithm), memory must be MemFree()"""
         ...
 def destroy_physics_body(PhysicsBodyData_pointer_0: Any,) -> None:
         """void DestroyPhysicsBody(struct PhysicsBodyData *);
 
 CFFI C function from raylib._raylib_cffi.lib"""
         ...
+def detach_audio_mixed_processor(processor: Any,) -> None:
+        """Detach audio stream processor from the entire audio pipeline"""
+        ...
 def detach_audio_stream_processor(stream: AudioStream,processor: Any,) -> None:
         """Detach audio stream processor from stream"""
         ...
 def directory_exists(dirPath: str,) -> bool:
         """Check if a directory path exists"""
         ...
 def disable_cursor() -> None:
@@ -162,14 +180,20 @@
         ...
 def draw_billboard_rec(camera: Camera3D,texture: Texture,source: Rectangle,position: Vector3,size: Vector2,tint: Color,) -> None:
         """Draw a billboard texture defined by source"""
         ...
 def draw_bounding_box(box: BoundingBox,color: Color,) -> None:
         """Draw bounding box (wires)"""
         ...
+def draw_capsule(startPos: Vector3,endPos: Vector3,radius: float,slices: int,rings: int,color: Color,) -> None:
+        """Draw a capsule with the center of its sphere caps at startPos and endPos"""
+        ...
+def draw_capsule_wires(startPos: Vector3,endPos: Vector3,radius: float,slices: int,rings: int,color: Color,) -> None:
+        """Draw capsule wireframe with the center of its sphere caps at startPos and endPos"""
+        ...
 def draw_circle(centerX: int,centerY: int,radius: float,color: Color,) -> None:
         """Draw a color-filled circle"""
         ...
 def draw_circle_3d(center: Vector3,radius: float,rotationAxis: Vector3,rotationAngle: float,color: Color,) -> None:
         """Draw a circle in 3D world space"""
         ...
 def draw_circle_gradient(centerX: int,centerY: int,radius: float,color1: Color,color2: Color,) -> None:
@@ -186,20 +210,14 @@
         ...
 def draw_circle_v(center: Vector2,radius: float,color: Color,) -> None:
         """Draw a color-filled circle (Vector version)"""
         ...
 def draw_cube(position: Vector3,width: float,height: float,length: float,color: Color,) -> None:
         """Draw cube"""
         ...
-def draw_cube_texture(texture: Texture,position: Vector3,width: float,height: float,length: float,color: Color,) -> None:
-        """Draw cube textured"""
-        ...
-def draw_cube_texture_rec(texture: Texture,source: Rectangle,position: Vector3,width: float,height: float,length: float,color: Color,) -> None:
-        """Draw cube with a region of a texture"""
-        ...
 def draw_cube_v(position: Vector3,size: Vector3,color: Color,) -> None:
         """Draw cube (Vector version)"""
         ...
 def draw_cube_wires(position: Vector3,width: float,height: float,length: float,color: Color,) -> None:
         """Draw cube wires"""
         ...
 def draw_cube_wires_v(position: Vector3,size: Vector3,color: Color,) -> None:
@@ -363,29 +381,20 @@
         ...
 def draw_texture_ex(texture: Texture,position: Vector2,rotation: float,scale: float,tint: Color,) -> None:
         """Draw a Texture2D with extended parameters"""
         ...
 def draw_texture_n_patch(texture: Texture,nPatchInfo: NPatchInfo,dest: Rectangle,origin: Vector2,rotation: float,tint: Color,) -> None:
         """Draws a texture (or part of it) that stretches or shrinks nicely"""
         ...
-def draw_texture_poly(texture: Texture,center: Vector2,points: Any,texcoords: Any,pointCount: int,tint: Color,) -> None:
-        """Draw a textured polygon"""
-        ...
 def draw_texture_pro(texture: Texture,source: Rectangle,dest: Rectangle,origin: Vector2,rotation: float,tint: Color,) -> None:
         """Draw a part of a texture defined by a rectangle with 'pro' parameters"""
         ...
-def draw_texture_quad(texture: Texture,tiling: Vector2,offset: Vector2,quad: Rectangle,tint: Color,) -> None:
-        """Draw texture quad with tiling and offset parameters"""
-        ...
 def draw_texture_rec(texture: Texture,source: Rectangle,position: Vector2,tint: Color,) -> None:
         """Draw a part of a texture defined by a rectangle"""
         ...
-def draw_texture_tiled(texture: Texture,source: Rectangle,dest: Rectangle,origin: Vector2,rotation: float,scale: float,tint: Color,) -> None:
-        """Draw part of a texture (defined by a rectangle) with rotation and scale tiled into dest."""
-        ...
 def draw_texture_v(texture: Texture,position: Vector2,tint: Color,) -> None:
         """Draw a Texture2D with position defined as Vector2"""
         ...
 def draw_triangle(v1: Vector2,v2: Vector2,v3: Vector2,color: Color,) -> None:
         """Draw a color-filled triangle (vertex in counter-clockwise order!)"""
         ...
 def draw_triangle_3d(v1: Vector3,v2: Vector3,v3: Vector3,color: Color,) -> None:
@@ -485,14 +494,20 @@
         ...
 def gen_image_gradient_radial(width: int,height: int,density: float,inner: Color,outer: Color,) -> Image:
         """Generate image: radial gradient"""
         ...
 def gen_image_gradient_v(width: int,height: int,top: Color,bottom: Color,) -> Image:
         """Generate image: vertical gradient"""
         ...
+def gen_image_perlin_noise(width: int,height: int,offsetX: int,offsetY: int,scale: float,) -> Image:
+        """Generate image: perlin noise"""
+        ...
+def gen_image_text(width: int,height: int,text: str,) -> Image:
+        """Generate image: grayscale image from text data"""
+        ...
 def gen_image_white_noise(width: int,height: int,factor: float,) -> Image:
         """Generate image: white noise"""
         ...
 def gen_mesh_cone(radius: float,height: float,slices: int,) -> Mesh:
         """Generate cone/pyramid mesh"""
         ...
 def gen_mesh_cube(width: float,height: float,length: float,) -> Mesh:
@@ -542,20 +557,26 @@
         ...
 def get_char_pressed() -> int:
         """Get char pressed (unicode), call it multiple times for chars queued, returns 0 when the queue is empty"""
         ...
 def get_clipboard_text() -> str:
         """Get clipboard text content"""
         ...
-def get_codepoint(text: str,bytesProcessed: Any,) -> int:
+def get_codepoint(text: str,codepointSize: Any,) -> int:
         """Get next codepoint in a UTF-8 encoded string, 0x3f('?') is returned on failure"""
         ...
 def get_codepoint_count(text: str,) -> int:
         """Get total number of codepoints in a UTF-8 encoded string"""
         ...
+def get_codepoint_next(text: str,codepointSize: Any,) -> int:
+        """Get next codepoint in a UTF-8 encoded string, 0x3f('?') is returned on failure"""
+        ...
+def get_codepoint_previous(text: str,codepointSize: Any,) -> int:
+        """Get previous codepoint in a UTF-8 encoded string, 0x3f('?') is returned on failure"""
+        ...
 def get_collision_rec(rec1: Rectangle,rec2: Rectangle,) -> Rectangle:
         """Get collision rectangle for two rectangles collision"""
         ...
 def get_color(hexValue: int,) -> Color:
         """Get Color structure from hexadecimal value"""
         ...
 def get_current_monitor() -> int:
@@ -762,17 +783,14 @@
         ...
 def get_shader_location(shader: Shader,uniformName: str,) -> int:
         """Get shader uniform location"""
         ...
 def get_shader_location_attrib(shader: Shader,attribName: str,) -> int:
         """Get shader attribute location"""
         ...
-def get_sounds_playing() -> int:
-        """Get number of sounds playing in the multichannel"""
-        ...
 def get_time() -> float:
         """Get elapsed time in seconds since InitWindow()"""
         ...
 def get_touch_point_count() -> int:
         """Get number of touch points"""
         ...
 def get_touch_point_id(index: int,) -> int:
@@ -814,24 +832,14 @@
 CFFI C function from raylib._raylib_cffi.lib"""
         ...
 def gui_check_box(Rectangle_0: Rectangle,str_1: str,_Bool_2: bool,) -> bool:
         """_Bool GuiCheckBox(struct Rectangle, char *, _Bool);
 
 CFFI C function from raylib._raylib_cffi.lib"""
         ...
-def gui_check_icon_pixel(int_0: int,int_1: int,int_2: int,) -> bool:
-        """_Bool GuiCheckIconPixel(int, int, int);
-
-CFFI C function from raylib._raylib_cffi.lib"""
-        ...
-def gui_clear_icon_pixel(int_0: int,int_1: int,int_2: int,) -> None:
-        """void GuiClearIconPixel(int, int, int);
-
-CFFI C function from raylib._raylib_cffi.lib"""
-        ...
 def gui_color_bar_alpha(Rectangle_0: Rectangle,str_1: str,float_2: float,) -> float:
         """float GuiColorBarAlpha(struct Rectangle, char *, float);
 
 CFFI C function from raylib._raylib_cffi.lib"""
         ...
 def gui_color_bar_hue(Rectangle_0: Rectangle,str_1: str,float_2: float,) -> float:
         """float GuiColorBarHue(struct Rectangle, char *, float);
@@ -854,14 +862,19 @@
 CFFI C function from raylib._raylib_cffi.lib"""
         ...
 def gui_disable() -> None:
         """void GuiDisable();
 
 CFFI C function from raylib._raylib_cffi.lib"""
         ...
+def gui_disable_tooltip() -> None:
+        """void GuiDisableTooltip();
+
+CFFI C function from raylib._raylib_cffi.lib"""
+        ...
 def gui_draw_icon(int_0: int,int_1: int,int_2: int,int_3: int,Color_4: Color,) -> None:
         """void GuiDrawIcon(int, int, int, int, struct Color);
 
 CFFI C function from raylib._raylib_cffi.lib"""
         ...
 def gui_dropdown_box(Rectangle_0: Rectangle,str_1: str,int_pointer_2: Any,_Bool_3: bool,) -> bool:
         """_Bool GuiDropdownBox(struct Rectangle, char *, int *, _Bool);
@@ -874,29 +887,29 @@
 CFFI C function from raylib._raylib_cffi.lib"""
         ...
 def gui_enable() -> None:
         """void GuiEnable();
 
 CFFI C function from raylib._raylib_cffi.lib"""
         ...
+def gui_enable_tooltip() -> None:
+        """void GuiEnableTooltip();
+
+CFFI C function from raylib._raylib_cffi.lib"""
+        ...
 def gui_fade(float_0: float,) -> None:
         """void GuiFade(float);
 
 CFFI C function from raylib._raylib_cffi.lib"""
         ...
 def gui_get_font() -> Font:
         """struct Font GuiGetFont();
 
 CFFI C function from raylib._raylib_cffi.lib"""
         ...
-def gui_get_icon_data(int_0: int,) -> Any:
-        """unsigned int *GuiGetIconData(int);
-
-CFFI C function from raylib._raylib_cffi.lib"""
-        ...
 def gui_get_icons() -> Any:
         """unsigned int *GuiGetIcons();
 
 CFFI C function from raylib._raylib_cffi.lib"""
         ...
 def gui_get_state() -> int:
         """int GuiGetState();
@@ -949,14 +962,19 @@
 CFFI C function from raylib._raylib_cffi.lib"""
         ...
 def gui_list_view_ex(Rectangle_0: Rectangle,str_pointer_1: str,int_2: int,int_pointer_3: Any,int_pointer_4: Any,int_5: int,) -> int:
         """int GuiListViewEx(struct Rectangle, char * *, int, int *, int *, int);
 
 CFFI C function from raylib._raylib_cffi.lib"""
         ...
+def gui_load_icons(str_0: str,_Bool_1: bool,) -> str:
+        """char * *GuiLoadIcons(char *, _Bool);
+
+CFFI C function from raylib._raylib_cffi.lib"""
+        ...
 def gui_load_style(str_0: str,) -> None:
         """void GuiLoadStyle(char *);
 
 CFFI C function from raylib._raylib_cffi.lib"""
         ...
 def gui_load_style_default() -> None:
         """void GuiLoadStyleDefault();
@@ -989,39 +1007,34 @@
 CFFI C function from raylib._raylib_cffi.lib"""
         ...
 def gui_set_font(Font_0: Font,) -> None:
         """void GuiSetFont(struct Font);
 
 CFFI C function from raylib._raylib_cffi.lib"""
         ...
-def gui_set_icon_data(int_0: int,unsignedint_pointer_1: Any,) -> None:
-        """void GuiSetIconData(int, unsigned int *);
-
-CFFI C function from raylib._raylib_cffi.lib"""
-        ...
-def gui_set_icon_pixel(int_0: int,int_1: int,int_2: int,) -> None:
-        """void GuiSetIconPixel(int, int, int);
-
-CFFI C function from raylib._raylib_cffi.lib"""
-        ...
-def gui_set_icon_scale(unsignedint_0: int,) -> None:
-        """void GuiSetIconScale(unsigned int);
+def gui_set_icon_scale(int_0: int,) -> None:
+        """void GuiSetIconScale(int);
 
 CFFI C function from raylib._raylib_cffi.lib"""
         ...
 def gui_set_state(int_0: int,) -> None:
         """void GuiSetState(int);
 
 CFFI C function from raylib._raylib_cffi.lib"""
         ...
 def gui_set_style(int_0: int,int_1: int,int_2: int,) -> None:
         """void GuiSetStyle(int, int, int);
 
 CFFI C function from raylib._raylib_cffi.lib"""
         ...
+def gui_set_tooltip(str_0: str,) -> None:
+        """void GuiSetTooltip(char *);
+
+CFFI C function from raylib._raylib_cffi.lib"""
+        ...
 def gui_slider(Rectangle_0: Rectangle,str_1: str,str_2: str,float_3: float,float_4: float,float_5: float,) -> float:
         """float GuiSlider(struct Rectangle, char *, char *, float, float, float);
 
 CFFI C function from raylib._raylib_cffi.lib"""
         ...
 def gui_slider_bar(Rectangle_0: Rectangle,str_1: str,str_2: str,float_3: float,float_4: float,float_5: float,) -> float:
         """float GuiSliderBar(struct Rectangle, char *, char *, float, float, float);
@@ -1034,21 +1047,21 @@
 CFFI C function from raylib._raylib_cffi.lib"""
         ...
 def gui_status_bar(Rectangle_0: Rectangle,str_1: str,) -> None:
         """void GuiStatusBar(struct Rectangle, char *);
 
 CFFI C function from raylib._raylib_cffi.lib"""
         ...
-def gui_text_box(Rectangle_0: Rectangle,str_1: str,int_2: int,_Bool_3: bool,) -> bool:
-        """_Bool GuiTextBox(struct Rectangle, char *, int, _Bool);
+def gui_tab_bar(Rectangle_0: Rectangle,str_pointer_1: str,int_2: int,int_pointer_3: Any,) -> int:
+        """int GuiTabBar(struct Rectangle, char * *, int, int *);
 
 CFFI C function from raylib._raylib_cffi.lib"""
         ...
-def gui_text_box_multi(Rectangle_0: Rectangle,str_1: str,int_2: int,_Bool_3: bool,) -> bool:
-        """_Bool GuiTextBoxMulti(struct Rectangle, char *, int, _Bool);
+def gui_text_box(Rectangle_0: Rectangle,str_1: str,int_2: int,_Bool_3: bool,) -> bool:
+        """_Bool GuiTextBox(struct Rectangle, char *, int, _Bool);
 
 CFFI C function from raylib._raylib_cffi.lib"""
         ...
 def gui_text_input_box(Rectangle_0: Rectangle,str_1: str,str_2: str,str_3: str,str_4: str,int_5: int,int_pointer_6: Any,) -> int:
         """int GuiTextInputBox(struct Rectangle, char *, char *, char *, char *, int, int *);
 
 CFFI C function from raylib._raylib_cffi.lib"""
@@ -1089,14 +1102,17 @@
         ...
 def image_alpha_mask(image: Any,alphaMask: Image,) -> None:
         """Apply alpha mask to image"""
         ...
 def image_alpha_premultiply(image: Any,) -> None:
         """Premultiply alpha channel"""
         ...
+def image_blur_gaussian(image: Any,blurSize: int,) -> None:
+        """Apply Gaussian blur using a box blur approximation"""
+        ...
 def image_clear_background(dst: Any,color: Color,) -> None:
         """Clear image background with given color"""
         ...
 def image_color_brightness(image: Any,brightness: int,) -> None:
         """Modify image color: brightness (-255 to 255)"""
         ...
 def image_color_contrast(image: Any,contrast: float,) -> None:
@@ -1123,18 +1139,24 @@
 def image_dither(image: Any,rBpp: int,gBpp: int,bBpp: int,aBpp: int,) -> None:
         """Dither image data to 16bpp or lower (Floyd-Steinberg dithering)"""
         ...
 def image_draw(dst: Any,src: Image,srcRec: Rectangle,dstRec: Rectangle,tint: Color,) -> None:
         """Draw a source image within a destination image (tint applied to source)"""
         ...
 def image_draw_circle(dst: Any,centerX: int,centerY: int,radius: int,color: Color,) -> None:
-        """Draw circle within an image"""
+        """Draw a filled circle within an image"""
+        ...
+def image_draw_circle_lines(dst: Any,centerX: int,centerY: int,radius: int,color: Color,) -> None:
+        """Draw circle outline within an image"""
+        ...
+def image_draw_circle_lines_v(dst: Any,center: Vector2,radius: int,color: Color,) -> None:
+        """Draw circle outline within an image (Vector version)"""
         ...
 def image_draw_circle_v(dst: Any,center: Vector2,radius: int,color: Color,) -> None:
-        """Draw circle within an image (Vector version)"""
+        """Draw a filled circle within an image (Vector version)"""
         ...
 def image_draw_line(dst: Any,startPosX: int,startPosY: int,endPosX: int,endPosY: int,color: Color,) -> None:
         """Draw line within an image"""
         ...
 def image_draw_line_v(dst: Any,start: Vector2,end: Vector2,color: Color,) -> None:
         """Draw line within an image (Vector version)"""
         ...
@@ -1217,26 +1239,32 @@
         ...
 def is_audio_stream_playing(stream: AudioStream,) -> bool:
         """Check if audio stream is playing"""
         ...
 def is_audio_stream_processed(stream: AudioStream,) -> bool:
         """Check if any audio stream buffers requires refill"""
         ...
+def is_audio_stream_ready(stream: AudioStream,) -> bool:
+        """Checks if an audio stream is ready"""
+        ...
 def is_cursor_hidden() -> bool:
         """Check if cursor is not visible"""
         ...
 def is_cursor_on_screen() -> bool:
         """Check if cursor is on the screen"""
         ...
 def is_file_dropped() -> bool:
         """Check if a file has been dropped into window"""
         ...
 def is_file_extension(fileName: str,ext: str,) -> bool:
         """Check file extension (including point: .png, .wav)"""
         ...
+def is_font_ready(font: Font,) -> bool:
+        """Check if a font is ready"""
+        ...
 def is_gamepad_available(gamepad: int,) -> bool:
         """Check if a gamepad is available"""
         ...
 def is_gamepad_button_down(gamepad: int,button: int,) -> bool:
         """Check if a gamepad button is being pressed"""
         ...
 def is_gamepad_button_pressed(gamepad: int,button: int,) -> bool:
@@ -1247,50 +1275,77 @@
         ...
 def is_gamepad_button_up(gamepad: int,button: int,) -> bool:
         """Check if a gamepad button is NOT being pressed"""
         ...
 def is_gesture_detected(gesture: int,) -> bool:
         """Check if a gesture have been detected"""
         ...
+def is_image_ready(image: Image,) -> bool:
+        """Check if an image is ready"""
+        ...
 def is_key_down(key: int,) -> bool:
         """Check if a key is being pressed"""
         ...
 def is_key_pressed(key: int,) -> bool:
         """Check if a key has been pressed once"""
         ...
 def is_key_released(key: int,) -> bool:
         """Check if a key has been released once"""
         ...
 def is_key_up(key: int,) -> bool:
         """Check if a key is NOT being pressed"""
         ...
+def is_material_ready(material: Material,) -> bool:
+        """Check if a material is ready"""
+        ...
 def is_model_animation_valid(model: Model,anim: ModelAnimation,) -> bool:
         """Check model animation skeleton match"""
         ...
+def is_model_ready(model: Model,) -> bool:
+        """Check if a model is ready"""
+        ...
 def is_mouse_button_down(button: int,) -> bool:
         """Check if a mouse button is being pressed"""
         ...
 def is_mouse_button_pressed(button: int,) -> bool:
         """Check if a mouse button has been pressed once"""
         ...
 def is_mouse_button_released(button: int,) -> bool:
         """Check if a mouse button has been released once"""
         ...
 def is_mouse_button_up(button: int,) -> bool:
         """Check if a mouse button is NOT being pressed"""
         ...
+def is_music_ready(music: Music,) -> bool:
+        """Checks if a music stream is ready"""
+        ...
 def is_music_stream_playing(music: Music,) -> bool:
         """Check if music is playing"""
         ...
 def is_path_file(path: str,) -> bool:
         """Check if a given path is a file or a directory"""
         ...
+def is_render_texture_ready(target: RenderTexture,) -> bool:
+        """Check if a render texture is ready"""
+        ...
+def is_shader_ready(shader: Shader,) -> bool:
+        """Check if a shader is ready"""
+        ...
 def is_sound_playing(sound: Sound,) -> bool:
         """Check if a sound is currently playing"""
         ...
+def is_sound_ready(sound: Sound,) -> bool:
+        """Checks if a sound is ready"""
+        ...
+def is_texture_ready(texture: Texture,) -> bool:
+        """Check if a texture is ready"""
+        ...
+def is_wave_ready(wave: Wave,) -> bool:
+        """Checks if wave data is ready"""
+        ...
 def is_window_focused() -> bool:
         """Check if window is currently focused (only PLATFORM_DESKTOP)"""
         ...
 def is_window_fullscreen() -> bool:
         """Check if window is currently fullscreen"""
         ...
 def is_window_hidden() -> bool:
@@ -1417,14 +1472,17 @@
         ...
 def load_texture_cubemap(image: Image,layout: int,) -> Texture:
         """Load cubemap from image, multiple image cubemap layouts supported"""
         ...
 def load_texture_from_image(image: Image,) -> Texture:
         """Load texture from image data"""
         ...
+def load_utf8(codepoints: Any,length: int,) -> str:
+        """Load UTF-8 text encoded from codepoints array"""
+        ...
 def load_vr_stereo_config(device: VrDeviceInfo,) -> VrStereoConfig:
         """Load VR stereo config for VR simulator device parameters"""
         ...
 def load_wave(fileName: str,) -> Wave:
         """Load wave data from file"""
         ...
 def load_wave_from_memory(fileType: str,fileData: str,dataSize: int,) -> Wave:
@@ -1596,17 +1654,14 @@
         ...
 def play_music_stream(music: Music,) -> None:
         """Start music playing"""
         ...
 def play_sound(sound: Sound,) -> None:
         """Play a sound"""
         ...
-def play_sound_multi(sound: Sound,) -> None:
-        """Play a sound (using multichannel buffer pool)"""
-        ...
 def poll_input_events() -> None:
         """Register all input events"""
         ...
 def quaternion_add(Vector4_0: Vector4,Vector4_1: Vector4,) -> Vector4:
         """struct Vector4 QuaternionAdd(struct Vector4, struct Vector4);
 
 CFFI C function from raylib._raylib_cffi.lib"""
@@ -1763,29 +1818,14 @@
         ...
 def set_audio_stream_pitch(stream: AudioStream,pitch: float,) -> None:
         """Set pitch for audio stream (1.0 is base level)"""
         ...
 def set_audio_stream_volume(stream: AudioStream,volume: float,) -> None:
         """Set volume for audio stream (1.0 is max level)"""
         ...
-def set_camera_alt_control(keyAlt: int,) -> None:
-        """Set camera alt key to combine with mouse movement (free camera)"""
-        ...
-def set_camera_mode(camera: Camera3D,mode: int,) -> None:
-        """Set camera mode (multiple camera modes available)"""
-        ...
-def set_camera_move_controls(keyFront: int,keyBack: int,keyRight: int,keyLeft: int,keyUp: int,keyDown: int,) -> None:
-        """Set camera move controls (1st person and 3rd person cameras)"""
-        ...
-def set_camera_pan_control(keyPan: int,) -> None:
-        """Set camera pan key to combine with mouse movement (free camera)"""
-        ...
-def set_camera_smooth_zoom_control(keySmoothZoom: int,) -> None:
-        """Set camera smooth zoom key to combine with mouse (free camera)"""
-        ...
 def set_clipboard_text(text: str,) -> None:
         """Set clipboard text content"""
         ...
 def set_config_flags(flags: int,) -> None:
         """Setup init configuration flags (view FLAGS)"""
         ...
 def set_exit_key(key: int,) -> None:
@@ -1896,15 +1936,18 @@
 def set_trace_log_callback(callback: str,) -> None:
         """Set custom trace log"""
         ...
 def set_trace_log_level(logLevel: int,) -> None:
         """Set the current threshold (minimum) log level"""
         ...
 def set_window_icon(image: Image,) -> None:
-        """Set icon for window (only PLATFORM_DESKTOP)"""
+        """Set icon for window (single image, RGBA 32bit, only PLATFORM_DESKTOP)"""
+        ...
+def set_window_icons(images: Any,count: int,) -> None:
+        """Set icon for window (multiple images, RGBA 32bit, only PLATFORM_DESKTOP)"""
         ...
 def set_window_min_size(width: int,height: int,) -> None:
         """Set window minimum dimensions (for FLAG_WINDOW_RESIZABLE)"""
         ...
 def set_window_monitor(monitor: int,) -> None:
         """Set monitor for the current window (fullscreen mode)"""
         ...
@@ -1931,29 +1974,23 @@
         ...
 def stop_music_stream(music: Music,) -> None:
         """Stop music playing"""
         ...
 def stop_sound(sound: Sound,) -> None:
         """Stop playing a sound"""
         ...
-def stop_sound_multi() -> None:
-        """Stop any sound playing (using multichannel buffer pool)"""
-        ...
 def swap_screen_buffer() -> None:
         """Swap back buffer with front buffer (screen drawing)"""
         ...
 def take_screenshot(fileName: str,) -> None:
         """Takes a screenshot of current screen (filename extension defines format)"""
         ...
 def text_append(text: str,append: str,position: Any,) -> None:
         """Append text at specific position and move cursor!"""
         ...
-def text_codepoints_to_utf8(codepoints: Any,length: int,) -> str:
-        """Encode text as codepoints array into UTF-8 text string (WARNING: memory must be freed!)"""
-        ...
 def text_copy(dst: str,src: str,) -> int:
         """Copy one string to another, returns bytes copied"""
         ...
 def text_find_index(text: str,find: str,) -> int:
         """Find first text occurrence within a string"""
         ...
 def text_format(*args) -> str:
@@ -2042,17 +2079,14 @@
         ...
 def unload_model_animation(anim: ModelAnimation,) -> None:
         """Unload animation data"""
         ...
 def unload_model_animations(animations: Any,count: int,) -> None:
         """Unload animation array data"""
         ...
-def unload_model_keep_meshes(model: Model,) -> None:
-        """Unload model (but not meshes) from memory (RAM and/or VRAM)"""
-        ...
 def unload_music_stream(music: Music,) -> None:
         """Unload music stream"""
         ...
 def unload_render_texture(target: RenderTexture,) -> None:
         """Unload render texture from GPU memory (VRAM)"""
         ...
 def unload_shader(shader: Shader,) -> None:
@@ -2060,29 +2094,35 @@
         ...
 def unload_sound(sound: Sound,) -> None:
         """Unload sound"""
         ...
 def unload_texture(texture: Texture,) -> None:
         """Unload texture from GPU memory (VRAM)"""
         ...
+def unload_utf8(text: str,) -> None:
+        """Unload UTF-8 text encoded from codepoints array"""
+        ...
 def unload_vr_stereo_config(config: VrStereoConfig,) -> None:
         """Unload VR stereo config"""
         ...
 def unload_wave(wave: Wave,) -> None:
         """Unload wave data"""
         ...
 def unload_wave_samples(samples: Any,) -> None:
         """Unload samples data loaded with LoadWaveSamples()"""
         ...
 def update_audio_stream(stream: AudioStream,data: Any,frameCount: int,) -> None:
         """Update audio stream buffers with data"""
         ...
-def update_camera(camera: Any,) -> None:
+def update_camera(camera: Any,mode: int,) -> None:
         """Update camera position for selected mode"""
         ...
+def update_camera_pro(camera: Any,movement: Vector3,rotation: Vector3,zoom: float,) -> None:
+        """Update camera movement/rotation"""
+        ...
 def update_mesh_buffer(mesh: Mesh,index: int,data: Any,dataSize: int,offset: int,) -> None:
         """Update mesh vertex data in GPU for a specific buffer index"""
         ...
 def update_model_animation(model: Model,anim: ModelAnimation,frame: int,) -> None:
         """Update model animation pose"""
         ...
 def update_music_stream(music: Music,) -> None:
@@ -2171,14 +2211,19 @@
 CFFI C function from raylib._raylib_cffi.lib"""
         ...
 def vector2_lerp(Vector2_0: Vector2,Vector2_1: Vector2,float_2: float,) -> Vector2:
         """struct Vector2 Vector2Lerp(struct Vector2, struct Vector2, float);
 
 CFFI C function from raylib._raylib_cffi.lib"""
         ...
+def vector2_line_angle(Vector2_0: Vector2,Vector2_1: Vector2,) -> float:
+        """float Vector2LineAngle(struct Vector2, struct Vector2);
+
+CFFI C function from raylib._raylib_cffi.lib"""
+        ...
 def vector2_move_towards(Vector2_0: Vector2,Vector2_1: Vector2,float_2: float,) -> Vector2:
         """struct Vector2 Vector2MoveTowards(struct Vector2, struct Vector2, float);
 
 CFFI C function from raylib._raylib_cffi.lib"""
         ...
 def vector2_multiply(Vector2_0: Vector2,Vector2_1: Vector2,) -> Vector2:
         """struct Vector2 Vector2Multiply(struct Vector2, struct Vector2);
@@ -2441,16 +2486,16 @@
 CFFI C function from raylib._raylib_cffi.lib"""
         ...
 def rl_begin(int_0: int,) -> None:
         """void rlBegin(int);
 
 CFFI C function from raylib._raylib_cffi.lib"""
         ...
-def rl_bind_image_texture(unsignedint_0: int,unsignedint_1: int,unsignedint_2: int,int_3: int,) -> None:
-        """void rlBindImageTexture(unsigned int, unsigned int, unsigned int, int);
+def rl_bind_image_texture(unsignedint_0: int,unsignedint_1: int,int_2: int,_Bool_3: bool,) -> None:
+        """void rlBindImageTexture(unsigned int, unsigned int, int, _Bool);
 
 CFFI C function from raylib._raylib_cffi.lib"""
         ...
 def rl_bind_shader_buffer(unsignedint_0: int,unsignedint_1: int,) -> None:
         """void rlBindShaderBuffer(unsigned int, unsigned int);
 
 CFFI C function from raylib._raylib_cffi.lib"""
@@ -2496,16 +2541,21 @@
 CFFI C function from raylib._raylib_cffi.lib"""
         ...
 def rl_compute_shader_dispatch(unsignedint_0: int,unsignedint_1: int,unsignedint_2: int,) -> None:
         """void rlComputeShaderDispatch(unsigned int, unsigned int, unsigned int);
 
 CFFI C function from raylib._raylib_cffi.lib"""
         ...
-def rl_copy_buffers_elements(unsignedint_0: int,unsignedint_1: int,unsignedlonglong_2: int,unsignedlonglong_3: int,unsignedlonglong_4: int,) -> None:
-        """void rlCopyBuffersElements(unsigned int, unsigned int, unsigned long long, unsigned long long, unsigned long long);
+def rl_copy_shader_buffer(unsignedint_0: int,unsignedint_1: int,unsignedint_2: int,unsignedint_3: int,unsignedint_4: int,) -> None:
+        """void rlCopyShaderBuffer(unsigned int, unsigned int, unsigned int, unsigned int, unsigned int);
+
+CFFI C function from raylib._raylib_cffi.lib"""
+        ...
+def rl_cubemap_parameters(unsignedint_0: int,int_1: int,int_2: int,) -> None:
+        """void rlCubemapParameters(unsigned int, int, int);
 
 CFFI C function from raylib._raylib_cffi.lib"""
         ...
 def rl_disable_backface_culling() -> None:
         """void rlDisableBackfaceCulling();
 
 CFFI C function from raylib._raylib_cffi.lib"""
@@ -2777,15 +2827,15 @@
         ...
 def rl_get_pixel_format_name(unsignedint_0: int,) -> str:
         """char *rlGetPixelFormatName(unsigned int);
 
 CFFI C function from raylib._raylib_cffi.lib"""
         ...
 def rl_get_shader_buffer_size(unsignedint_0: int,) -> int:
-        """unsigned long long rlGetShaderBufferSize(unsigned int);
+        """unsigned int rlGetShaderBufferSize(unsigned int);
 
 CFFI C function from raylib._raylib_cffi.lib"""
         ...
 def rl_get_shader_id_default() -> int:
         """unsigned int rlGetShaderIdDefault();
 
 CFFI C function from raylib._raylib_cffi.lib"""
@@ -2841,16 +2891,16 @@
 CFFI C function from raylib._raylib_cffi.lib"""
         ...
 def rl_load_render_batch(int_0: int,int_1: int,) -> rlRenderBatch:
         """struct rlRenderBatch rlLoadRenderBatch(int, int);
 
 CFFI C function from raylib._raylib_cffi.lib"""
         ...
-def rl_load_shader_buffer(unsignedlonglong_0: int,void_pointer_1: Any,int_2: int,) -> int:
-        """unsigned int rlLoadShaderBuffer(unsigned long long, void *, int);
+def rl_load_shader_buffer(unsignedint_0: int,void_pointer_1: Any,int_2: int,) -> int:
+        """unsigned int rlLoadShaderBuffer(unsigned int, void *, int);
 
 CFFI C function from raylib._raylib_cffi.lib"""
         ...
 def rl_load_shader_code(str_0: str,str_1: str,) -> int:
         """unsigned int rlLoadShaderCode(char *, char *);
 
 CFFI C function from raylib._raylib_cffi.lib"""
@@ -2921,16 +2971,16 @@
 CFFI C function from raylib._raylib_cffi.lib"""
         ...
 def rl_read_screen_pixels(int_0: int,int_1: int,) -> str:
         """unsigned char *rlReadScreenPixels(int, int);
 
 CFFI C function from raylib._raylib_cffi.lib"""
         ...
-def rl_read_shader_buffer_elements(unsignedint_0: int,void_pointer_1: Any,unsignedlonglong_2: int,unsignedlonglong_3: int,) -> None:
-        """void rlReadShaderBufferElements(unsigned int, void *, unsigned long long, unsigned long long);
+def rl_read_shader_buffer(unsignedint_0: int,void_pointer_1: Any,unsignedint_2: int,unsignedint_3: int,) -> None:
+        """void rlReadShaderBuffer(unsigned int, void *, unsigned int, unsigned int);
 
 CFFI C function from raylib._raylib_cffi.lib"""
         ...
 def rl_read_texture_pixels(unsignedint_0: int,int_1: int,int_2: int,int_3: int,) -> Any:
         """void *rlReadTexturePixels(unsigned int, int, int, int);
 
 CFFI C function from raylib._raylib_cffi.lib"""
@@ -2951,19 +3001,29 @@
 CFFI C function from raylib._raylib_cffi.lib"""
         ...
 def rl_set_blend_factors(int_0: int,int_1: int,int_2: int,) -> None:
         """void rlSetBlendFactors(int, int, int);
 
 CFFI C function from raylib._raylib_cffi.lib"""
         ...
+def rl_set_blend_factors_separate(int_0: int,int_1: int,int_2: int,int_3: int,int_4: int,int_5: int,) -> None:
+        """void rlSetBlendFactorsSeparate(int, int, int, int, int, int);
+
+CFFI C function from raylib._raylib_cffi.lib"""
+        ...
 def rl_set_blend_mode(int_0: int,) -> None:
         """void rlSetBlendMode(int);
 
 CFFI C function from raylib._raylib_cffi.lib"""
         ...
+def rl_set_cull_face(int_0: int,) -> None:
+        """void rlSetCullFace(int);
+
+CFFI C function from raylib._raylib_cffi.lib"""
+        ...
 def rl_set_framebuffer_height(int_0: int,) -> None:
         """void rlSetFramebufferHeight(int);
 
 CFFI C function from raylib._raylib_cffi.lib"""
         ...
 def rl_set_framebuffer_width(int_0: int,) -> None:
         """void rlSetFramebufferWidth(int);
@@ -3086,16 +3146,16 @@
 CFFI C function from raylib._raylib_cffi.lib"""
         ...
 def rl_unload_vertex_buffer(unsignedint_0: int,) -> None:
         """void rlUnloadVertexBuffer(unsigned int);
 
 CFFI C function from raylib._raylib_cffi.lib"""
         ...
-def rl_update_shader_buffer_elements(unsignedint_0: int,void_pointer_1: Any,unsignedlonglong_2: int,unsignedlonglong_3: int,) -> None:
-        """void rlUpdateShaderBufferElements(unsigned int, void *, unsigned long long, unsigned long long);
+def rl_update_shader_buffer(unsignedint_0: int,void_pointer_1: Any,unsignedint_2: int,unsignedint_3: int,) -> None:
+        """void rlUpdateShaderBuffer(unsigned int, void *, unsigned int, unsigned int);
 
 CFFI C function from raylib._raylib_cffi.lib"""
         ...
 def rl_update_texture(unsignedint_0: int,int_1: int,int_2: int,int_3: int,int_4: int,int_5: int,void_pointer_6: Any,) -> None:
         """void rlUpdateTexture(unsigned int, int, int, int, int, int, void *);
 
 CFFI C function from raylib._raylib_cffi.lib"""
@@ -3831,14 +3891,15 @@
     BLEND_ALPHA = 0
     BLEND_ADDITIVE = 1
     BLEND_MULTIPLIED = 2
     BLEND_ADD_COLORS = 3
     BLEND_SUBTRACT_COLORS = 4
     BLEND_ALPHA_PREMULTIPLY = 5
     BLEND_CUSTOM = 6
+    BLEND_CUSTOM_SEPARATE = 7
 
 class Gesture(IntEnum):
     GESTURE_NONE = 0
     GESTURE_TAP = 1
     GESTURE_DOUBLETAP = 2
     GESTURE_HOLD = 4
     GESTURE_DRAG = 8
@@ -3946,14 +4007,17 @@
 class GuiDropdownBoxProperty(IntEnum):
     ARROW_PADDING = 16
     DROPDOWN_ITEMS_SPACING = 17
 
 class GuiTextBoxProperty(IntEnum):
     TEXT_INNER_PADDING = 16
     TEXT_LINES_SPACING = 17
+    TEXT_ALIGNMENT_VERTICAL = 18
+    TEXT_MULTILINE = 19
+    TEXT_WRAP_MODE = 20
 
 class GuiSpinnerProperty(IntEnum):
     SPIN_BUTTON_WIDTH = 16
     SPIN_BUTTON_SPACING = 17
 
 class GuiListViewProperty(IntEnum):
     LIST_ITEMS_HEIGHT = 16
@@ -4171,27 +4235,27 @@
     ICON_HIDPI = 199
     ICON_FILETYPE_BINARY = 200
     ICON_HEX = 201
     ICON_SHIELD = 202
     ICON_FILE_NEW = 203
     ICON_FOLDER_ADD = 204
     ICON_ALARM = 205
-    ICON_206 = 206
-    ICON_207 = 207
-    ICON_208 = 208
-    ICON_209 = 209
-    ICON_210 = 210
-    ICON_211 = 211
-    ICON_212 = 212
-    ICON_213 = 213
-    ICON_214 = 214
-    ICON_215 = 215
-    ICON_216 = 216
-    ICON_217 = 217
-    ICON_218 = 218
+    ICON_CPU = 206
+    ICON_ROM = 207
+    ICON_STEP_OVER = 208
+    ICON_STEP_INTO = 209
+    ICON_STEP_OUT = 210
+    ICON_RESTART = 211
+    ICON_BREAKPOINT_ON = 212
+    ICON_BREAKPOINT_OFF = 213
+    ICON_BURGER_MENU = 214
+    ICON_CASE_SENSITIVE = 215
+    ICON_REG_EXP = 216
+    ICON_FOLDER = 217
+    ICON_FILE = 218
     ICON_219 = 219
     ICON_220 = 220
     ICON_221 = 221
     ICON_222 = 222
     ICON_223 = 223
     ICON_224 = 224
     ICON_225 = 225
```

### Comparing `raylib-4.2.1.2/raylib/__init__.py` & `raylib-4.5.0.0/raylib/__init__.py`

 * *Files identical despite different names*

### Comparing `raylib-4.2.1.2/raylib/__init__.pyi` & `raylib-4.5.0.0/raylib/__init__.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,37 @@
 from typing import Any
 
+import _cffi_backend
+
+ffi: _cffi_backend.FFI
+rl: _cffi_backend.Lib
+
 class struct: ...
 
 
 ARROWS_SIZE: int
 ARROWS_VISIBLE: int
 ARROW_PADDING: int
+def AttachAudioMixedProcessor(processor: Any,) -> None:
+        """Attach audio stream processor to the entire audio pipeline"""
+        ...
 def AttachAudioStreamProcessor(stream: AudioStream,processor: Any,) -> None:
         """Attach audio stream processor to stream"""
         ...
 BACKGROUND_COLOR: int
 BASE_COLOR_DISABLED: int
 BASE_COLOR_FOCUSED: int
 BASE_COLOR_NORMAL: int
 BASE_COLOR_PRESSED: int
 BLEND_ADDITIVE: int
 BLEND_ADD_COLORS: int
 BLEND_ALPHA: int
 BLEND_ALPHA_PREMULTIPLY: int
 BLEND_CUSTOM: int
+BLEND_CUSTOM_SEPARATE: int
 BLEND_MULTIPLIED: int
 BLEND_SUBTRACT_COLORS: int
 BORDER_COLOR_DISABLED: int
 BORDER_COLOR_FOCUSED: int
 BORDER_COLOR_NORMAL: int
 BORDER_COLOR_PRESSED: int
 BORDER_WIDTH: int
@@ -91,14 +100,17 @@
         ...
 def CheckCollisionPointCircle(point: Vector2,center: Vector2,radius: float,) -> bool:
         """Check if point is inside circle"""
         ...
 def CheckCollisionPointLine(point: Vector2,p1: Vector2,p2: Vector2,threshold: int,) -> bool:
         """Check if point belongs to line created between two points [p1] and [p2] with defined margin in pixels [threshold]"""
         ...
+def CheckCollisionPointPoly(point: Vector2,points: Any,pointCount: int,) -> bool:
+        """Check if point is within a polygon described by array of vertices"""
+        ...
 def CheckCollisionPointRec(point: Vector2,rec: Rectangle,) -> bool:
         """Check if point is inside rectangle"""
         ...
 def CheckCollisionPointTriangle(point: Vector2,p1: Vector2,p2: Vector2,p3: Vector2,) -> bool:
         """Check if point is inside a triangle"""
         ...
 def CheckCollisionRecs(rec1: Rectangle,rec2: Rectangle,) -> bool:
@@ -125,32 +137,41 @@
         """void ClosePhysics();
 
 CFFI C function from raylib._raylib_cffi.lib"""
         ...
 def CloseWindow() -> None:
         """Close window and unload OpenGL context"""
         ...
-def CodepointToUTF8(codepoint: int,byteSize: Any,) -> str:
+def CodepointToUTF8(codepoint: int,utf8Size: Any,) -> str:
         """Encode one codepoint into UTF-8 byte array (array length returned as parameter)"""
         ...
 def ColorAlpha(color: Color,alpha: float,) -> Color:
         """Get color with alpha applied, alpha goes from 0.0f to 1.0f"""
         ...
 def ColorAlphaBlend(dst: Color,src: Color,tint: Color,) -> Color:
         """Get src alpha-blended into dst color with tint"""
         ...
+def ColorBrightness(color: Color,factor: float,) -> Color:
+        """Get color with brightness correction, brightness factor goes from -1.0f to 1.0f"""
+        ...
+def ColorContrast(color: Color,contrast: float,) -> Color:
+        """Get color with contrast correction, contrast values between -1.0f and 1.0f"""
+        ...
 def ColorFromHSV(hue: float,saturation: float,value: float,) -> Color:
         """Get a Color from HSV values, hue [0..360], saturation/value [0..1]"""
         ...
 def ColorFromNormalized(normalized: Vector4,) -> Color:
         """Get Color from normalized values [0..1]"""
         ...
 def ColorNormalize(color: Color,) -> Vector4:
         """Get Color normalized as float [0..1]"""
         ...
+def ColorTint(color: Color,tint: Color,) -> Color:
+        """Get color multiplied with another color"""
+        ...
 def ColorToHSV(color: Color,) -> Vector3:
         """Get HSV values for a Color, hue [0..360], saturation/value [0..1]"""
         ...
 def ColorToInt(color: Color,) -> int:
         """Get hexadecimal value for a Color"""
         ...
 def CompressData(data: str,dataSize: int,compDataSize: Any,) -> str:
@@ -181,14 +202,17 @@
         """Decompress data (DEFLATE algorithm), memory must be MemFree()"""
         ...
 def DestroyPhysicsBody(PhysicsBodyData_pointer_0: Any,) -> None:
         """void DestroyPhysicsBody(struct PhysicsBodyData *);
 
 CFFI C function from raylib._raylib_cffi.lib"""
         ...
+def DetachAudioMixedProcessor(processor: Any,) -> None:
+        """Detach audio stream processor from the entire audio pipeline"""
+        ...
 def DetachAudioStreamProcessor(stream: AudioStream,processor: Any,) -> None:
         """Detach audio stream processor from stream"""
         ...
 def DirectoryExists(dirPath: str,) -> bool:
         """Check if a directory path exists"""
         ...
 def DisableCursor() -> None:
@@ -205,14 +229,20 @@
         ...
 def DrawBillboardRec(camera: Camera3D,texture: Texture,source: Rectangle,position: Vector3,size: Vector2,tint: Color,) -> None:
         """Draw a billboard texture defined by source"""
         ...
 def DrawBoundingBox(box: BoundingBox,color: Color,) -> None:
         """Draw bounding box (wires)"""
         ...
+def DrawCapsule(startPos: Vector3,endPos: Vector3,radius: float,slices: int,rings: int,color: Color,) -> None:
+        """Draw a capsule with the center of its sphere caps at startPos and endPos"""
+        ...
+def DrawCapsuleWires(startPos: Vector3,endPos: Vector3,radius: float,slices: int,rings: int,color: Color,) -> None:
+        """Draw capsule wireframe with the center of its sphere caps at startPos and endPos"""
+        ...
 def DrawCircle(centerX: int,centerY: int,radius: float,color: Color,) -> None:
         """Draw a color-filled circle"""
         ...
 def DrawCircle3D(center: Vector3,radius: float,rotationAxis: Vector3,rotationAngle: float,color: Color,) -> None:
         """Draw a circle in 3D world space"""
         ...
 def DrawCircleGradient(centerX: int,centerY: int,radius: float,color1: Color,color2: Color,) -> None:
@@ -229,20 +259,14 @@
         ...
 def DrawCircleV(center: Vector2,radius: float,color: Color,) -> None:
         """Draw a color-filled circle (Vector version)"""
         ...
 def DrawCube(position: Vector3,width: float,height: float,length: float,color: Color,) -> None:
         """Draw cube"""
         ...
-def DrawCubeTexture(texture: Texture,position: Vector3,width: float,height: float,length: float,color: Color,) -> None:
-        """Draw cube textured"""
-        ...
-def DrawCubeTextureRec(texture: Texture,source: Rectangle,position: Vector3,width: float,height: float,length: float,color: Color,) -> None:
-        """Draw cube with a region of a texture"""
-        ...
 def DrawCubeV(position: Vector3,size: Vector3,color: Color,) -> None:
         """Draw cube (Vector version)"""
         ...
 def DrawCubeWires(position: Vector3,width: float,height: float,length: float,color: Color,) -> None:
         """Draw cube wires"""
         ...
 def DrawCubeWiresV(position: Vector3,size: Vector3,color: Color,) -> None:
@@ -406,29 +430,20 @@
         ...
 def DrawTextureEx(texture: Texture,position: Vector2,rotation: float,scale: float,tint: Color,) -> None:
         """Draw a Texture2D with extended parameters"""
         ...
 def DrawTextureNPatch(texture: Texture,nPatchInfo: NPatchInfo,dest: Rectangle,origin: Vector2,rotation: float,tint: Color,) -> None:
         """Draws a texture (or part of it) that stretches or shrinks nicely"""
         ...
-def DrawTexturePoly(texture: Texture,center: Vector2,points: Any,texcoords: Any,pointCount: int,tint: Color,) -> None:
-        """Draw a textured polygon"""
-        ...
 def DrawTexturePro(texture: Texture,source: Rectangle,dest: Rectangle,origin: Vector2,rotation: float,tint: Color,) -> None:
         """Draw a part of a texture defined by a rectangle with 'pro' parameters"""
         ...
-def DrawTextureQuad(texture: Texture,tiling: Vector2,offset: Vector2,quad: Rectangle,tint: Color,) -> None:
-        """Draw texture quad with tiling and offset parameters"""
-        ...
 def DrawTextureRec(texture: Texture,source: Rectangle,position: Vector2,tint: Color,) -> None:
         """Draw a part of a texture defined by a rectangle"""
         ...
-def DrawTextureTiled(texture: Texture,source: Rectangle,dest: Rectangle,origin: Vector2,rotation: float,scale: float,tint: Color,) -> None:
-        """Draw part of a texture (defined by a rectangle) with rotation and scale tiled into dest."""
-        ...
 def DrawTextureV(texture: Texture,position: Vector2,tint: Color,) -> None:
         """Draw a Texture2D with position defined as Vector2"""
         ...
 def DrawTriangle(v1: Vector2,v2: Vector2,v3: Vector2,color: Color,) -> None:
         """Draw a color-filled triangle (vertex in counter-clockwise order!)"""
         ...
 def DrawTriangle3D(v1: Vector3,v2: Vector3,v3: Vector3,color: Color,) -> None:
@@ -582,14 +597,20 @@
         ...
 def GenImageGradientRadial(width: int,height: int,density: float,inner: Color,outer: Color,) -> Image:
         """Generate image: radial gradient"""
         ...
 def GenImageGradientV(width: int,height: int,top: Color,bottom: Color,) -> Image:
         """Generate image: vertical gradient"""
         ...
+def GenImagePerlinNoise(width: int,height: int,offsetX: int,offsetY: int,scale: float,) -> Image:
+        """Generate image: perlin noise"""
+        ...
+def GenImageText(width: int,height: int,text: str,) -> Image:
+        """Generate image: grayscale image from text data"""
+        ...
 def GenImageWhiteNoise(width: int,height: int,factor: float,) -> Image:
         """Generate image: white noise"""
         ...
 def GenMeshCone(radius: float,height: float,slices: int,) -> Mesh:
         """Generate cone/pyramid mesh"""
         ...
 def GenMeshCube(width: float,height: float,length: float,) -> Mesh:
@@ -639,20 +660,26 @@
         ...
 def GetCharPressed() -> int:
         """Get char pressed (unicode), call it multiple times for chars queued, returns 0 when the queue is empty"""
         ...
 def GetClipboardText() -> str:
         """Get clipboard text content"""
         ...
-def GetCodepoint(text: str,bytesProcessed: Any,) -> int:
+def GetCodepoint(text: str,codepointSize: Any,) -> int:
         """Get next codepoint in a UTF-8 encoded string, 0x3f('?') is returned on failure"""
         ...
 def GetCodepointCount(text: str,) -> int:
         """Get total number of codepoints in a UTF-8 encoded string"""
         ...
+def GetCodepointNext(text: str,codepointSize: Any,) -> int:
+        """Get next codepoint in a UTF-8 encoded string, 0x3f('?') is returned on failure"""
+        ...
+def GetCodepointPrevious(text: str,codepointSize: Any,) -> int:
+        """Get previous codepoint in a UTF-8 encoded string, 0x3f('?') is returned on failure"""
+        ...
 def GetCollisionRec(rec1: Rectangle,rec2: Rectangle,) -> Rectangle:
         """Get collision rectangle for two rectangles collision"""
         ...
 def GetColor(hexValue: int,) -> Color:
         """Get Color structure from hexadecimal value"""
         ...
 def GetCurrentMonitor() -> int:
@@ -859,17 +886,14 @@
         ...
 def GetShaderLocation(shader: Shader,uniformName: str,) -> int:
         """Get shader uniform location"""
         ...
 def GetShaderLocationAttrib(shader: Shader,attribName: str,) -> int:
         """Get shader attribute location"""
         ...
-def GetSoundsPlaying() -> int:
-        """Get number of sounds playing in the multichannel"""
-        ...
 def GetTime() -> float:
         """Get elapsed time in seconds since InitWindow()"""
         ...
 def GetTouchPointCount() -> int:
         """Get number of touch points"""
         ...
 def GetTouchPointId(index: int,) -> int:
@@ -911,24 +935,14 @@
 CFFI C function from raylib._raylib_cffi.lib"""
         ...
 def GuiCheckBox(Rectangle_0: Rectangle,str_1: str,_Bool_2: bool,) -> bool:
         """_Bool GuiCheckBox(struct Rectangle, char *, _Bool);
 
 CFFI C function from raylib._raylib_cffi.lib"""
         ...
-def GuiCheckIconPixel(int_0: int,int_1: int,int_2: int,) -> bool:
-        """_Bool GuiCheckIconPixel(int, int, int);
-
-CFFI C function from raylib._raylib_cffi.lib"""
-        ...
-def GuiClearIconPixel(int_0: int,int_1: int,int_2: int,) -> None:
-        """void GuiClearIconPixel(int, int, int);
-
-CFFI C function from raylib._raylib_cffi.lib"""
-        ...
 def GuiColorBarAlpha(Rectangle_0: Rectangle,str_1: str,float_2: float,) -> float:
         """float GuiColorBarAlpha(struct Rectangle, char *, float);
 
 CFFI C function from raylib._raylib_cffi.lib"""
         ...
 def GuiColorBarHue(Rectangle_0: Rectangle,str_1: str,float_2: float,) -> float:
         """float GuiColorBarHue(struct Rectangle, char *, float);
@@ -951,14 +965,19 @@
 CFFI C function from raylib._raylib_cffi.lib"""
         ...
 def GuiDisable() -> None:
         """void GuiDisable();
 
 CFFI C function from raylib._raylib_cffi.lib"""
         ...
+def GuiDisableTooltip() -> None:
+        """void GuiDisableTooltip();
+
+CFFI C function from raylib._raylib_cffi.lib"""
+        ...
 def GuiDrawIcon(int_0: int,int_1: int,int_2: int,int_3: int,Color_4: Color,) -> None:
         """void GuiDrawIcon(int, int, int, int, struct Color);
 
 CFFI C function from raylib._raylib_cffi.lib"""
         ...
 def GuiDropdownBox(Rectangle_0: Rectangle,str_1: str,int_pointer_2: Any,_Bool_3: bool,) -> bool:
         """_Bool GuiDropdownBox(struct Rectangle, char *, int *, _Bool);
@@ -971,29 +990,29 @@
 CFFI C function from raylib._raylib_cffi.lib"""
         ...
 def GuiEnable() -> None:
         """void GuiEnable();
 
 CFFI C function from raylib._raylib_cffi.lib"""
         ...
+def GuiEnableTooltip() -> None:
+        """void GuiEnableTooltip();
+
+CFFI C function from raylib._raylib_cffi.lib"""
+        ...
 def GuiFade(float_0: float,) -> None:
         """void GuiFade(float);
 
 CFFI C function from raylib._raylib_cffi.lib"""
         ...
 def GuiGetFont() -> Font:
         """struct Font GuiGetFont();
 
 CFFI C function from raylib._raylib_cffi.lib"""
         ...
-def GuiGetIconData(int_0: int,) -> Any:
-        """unsigned int *GuiGetIconData(int);
-
-CFFI C function from raylib._raylib_cffi.lib"""
-        ...
 def GuiGetIcons() -> Any:
         """unsigned int *GuiGetIcons();
 
 CFFI C function from raylib._raylib_cffi.lib"""
         ...
 def GuiGetState() -> int:
         """int GuiGetState();
@@ -1046,14 +1065,19 @@
 CFFI C function from raylib._raylib_cffi.lib"""
         ...
 def GuiListViewEx(Rectangle_0: Rectangle,str_pointer_1: str,int_2: int,int_pointer_3: Any,int_pointer_4: Any,int_5: int,) -> int:
         """int GuiListViewEx(struct Rectangle, char * *, int, int *, int *, int);
 
 CFFI C function from raylib._raylib_cffi.lib"""
         ...
+def GuiLoadIcons(str_0: str,_Bool_1: bool,) -> str:
+        """char * *GuiLoadIcons(char *, _Bool);
+
+CFFI C function from raylib._raylib_cffi.lib"""
+        ...
 def GuiLoadStyle(str_0: str,) -> None:
         """void GuiLoadStyle(char *);
 
 CFFI C function from raylib._raylib_cffi.lib"""
         ...
 def GuiLoadStyleDefault() -> None:
         """void GuiLoadStyleDefault();
@@ -1086,39 +1110,34 @@
 CFFI C function from raylib._raylib_cffi.lib"""
         ...
 def GuiSetFont(Font_0: Font,) -> None:
         """void GuiSetFont(struct Font);
 
 CFFI C function from raylib._raylib_cffi.lib"""
         ...
-def GuiSetIconData(int_0: int,unsignedint_pointer_1: Any,) -> None:
-        """void GuiSetIconData(int, unsigned int *);
-
-CFFI C function from raylib._raylib_cffi.lib"""
-        ...
-def GuiSetIconPixel(int_0: int,int_1: int,int_2: int,) -> None:
-        """void GuiSetIconPixel(int, int, int);
-
-CFFI C function from raylib._raylib_cffi.lib"""
-        ...
-def GuiSetIconScale(unsignedint_0: int,) -> None:
-        """void GuiSetIconScale(unsigned int);
+def GuiSetIconScale(int_0: int,) -> None:
+        """void GuiSetIconScale(int);
 
 CFFI C function from raylib._raylib_cffi.lib"""
         ...
 def GuiSetState(int_0: int,) -> None:
         """void GuiSetState(int);
 
 CFFI C function from raylib._raylib_cffi.lib"""
         ...
 def GuiSetStyle(int_0: int,int_1: int,int_2: int,) -> None:
         """void GuiSetStyle(int, int, int);
 
 CFFI C function from raylib._raylib_cffi.lib"""
         ...
+def GuiSetTooltip(str_0: str,) -> None:
+        """void GuiSetTooltip(char *);
+
+CFFI C function from raylib._raylib_cffi.lib"""
+        ...
 def GuiSlider(Rectangle_0: Rectangle,str_1: str,str_2: str,float_3: float,float_4: float,float_5: float,) -> float:
         """float GuiSlider(struct Rectangle, char *, char *, float, float, float);
 
 CFFI C function from raylib._raylib_cffi.lib"""
         ...
 def GuiSliderBar(Rectangle_0: Rectangle,str_1: str,str_2: str,float_3: float,float_4: float,float_5: float,) -> float:
         """float GuiSliderBar(struct Rectangle, char *, char *, float, float, float);
@@ -1131,21 +1150,21 @@
 CFFI C function from raylib._raylib_cffi.lib"""
         ...
 def GuiStatusBar(Rectangle_0: Rectangle,str_1: str,) -> None:
         """void GuiStatusBar(struct Rectangle, char *);
 
 CFFI C function from raylib._raylib_cffi.lib"""
         ...
-def GuiTextBox(Rectangle_0: Rectangle,str_1: str,int_2: int,_Bool_3: bool,) -> bool:
-        """_Bool GuiTextBox(struct Rectangle, char *, int, _Bool);
+def GuiTabBar(Rectangle_0: Rectangle,str_pointer_1: str,int_2: int,int_pointer_3: Any,) -> int:
+        """int GuiTabBar(struct Rectangle, char * *, int, int *);
 
 CFFI C function from raylib._raylib_cffi.lib"""
         ...
-def GuiTextBoxMulti(Rectangle_0: Rectangle,str_1: str,int_2: int,_Bool_3: bool,) -> bool:
-        """_Bool GuiTextBoxMulti(struct Rectangle, char *, int, _Bool);
+def GuiTextBox(Rectangle_0: Rectangle,str_1: str,int_2: int,_Bool_3: bool,) -> bool:
+        """_Bool GuiTextBox(struct Rectangle, char *, int, _Bool);
 
 CFFI C function from raylib._raylib_cffi.lib"""
         ...
 def GuiTextInputBox(Rectangle_0: Rectangle,str_1: str,str_2: str,str_3: str,str_4: str,int_5: int,int_pointer_6: Any,) -> int:
         """int GuiTextInputBox(struct Rectangle, char *, char *, char *, char *, int, int *);
 
 CFFI C function from raylib._raylib_cffi.lib"""
@@ -1179,27 +1198,14 @@
 HUEBAR_SELECTOR_HEIGHT: int
 HUEBAR_SELECTOR_OVERFLOW: int
 HUEBAR_WIDTH: int
 def HideCursor() -> None:
         """Hides cursor"""
         ...
 ICON_1UP: int
-ICON_206: int
-ICON_207: int
-ICON_208: int
-ICON_209: int
-ICON_210: int
-ICON_211: int
-ICON_212: int
-ICON_213: int
-ICON_214: int
-ICON_215: int
-ICON_216: int
-ICON_217: int
-ICON_218: int
 ICON_219: int
 ICON_220: int
 ICON_221: int
 ICON_222: int
 ICON_223: int
 ICON_224: int
 ICON_225: int
@@ -1261,22 +1267,27 @@
 ICON_BOX_GRID_BIG: int
 ICON_BOX_LEFT: int
 ICON_BOX_MULTISIZE: int
 ICON_BOX_RIGHT: int
 ICON_BOX_TOP: int
 ICON_BOX_TOP_LEFT: int
 ICON_BOX_TOP_RIGHT: int
+ICON_BREAKPOINT_OFF: int
+ICON_BREAKPOINT_ON: int
 ICON_BRUSH_CLASSIC: int
 ICON_BRUSH_PAINTER: int
+ICON_BURGER_MENU: int
 ICON_CAMERA: int
+ICON_CASE_SENSITIVE: int
 ICON_CLOCK: int
 ICON_COIN: int
 ICON_COLOR_BUCKET: int
 ICON_COLOR_PICKER: int
 ICON_CORNER: int
+ICON_CPU: int
 ICON_CRACK: int
 ICON_CRACK_POINTS: int
 ICON_CROP: int
 ICON_CROP_ALPHA: int
 ICON_CROSS: int
 ICON_CROSSLINE: int
 ICON_CROSS_SMALL: int
@@ -1303,14 +1314,15 @@
 ICON_DOOR: int
 ICON_EMPTYBOX: int
 ICON_EMPTYBOX_SMALL: int
 ICON_EXIT: int
 ICON_EXPLOSION: int
 ICON_EYE_OFF: int
 ICON_EYE_ON: int
+ICON_FILE: int
 ICON_FILETYPE_ALPHA: int
 ICON_FILETYPE_AUDIO: int
 ICON_FILETYPE_BINARY: int
 ICON_FILETYPE_HOME: int
 ICON_FILETYPE_IMAGE: int
 ICON_FILETYPE_INFO: int
 ICON_FILETYPE_PLAY: int
@@ -1326,14 +1338,15 @@
 ICON_FILE_PASTE: int
 ICON_FILE_SAVE: int
 ICON_FILE_SAVE_CLASSIC: int
 ICON_FILTER: int
 ICON_FILTER_BILINEAR: int
 ICON_FILTER_POINT: int
 ICON_FILTER_TOP: int
+ICON_FOLDER: int
 ICON_FOLDER_ADD: int
 ICON_FOLDER_FILE_OPEN: int
 ICON_FOLDER_OPEN: int
 ICON_FOLDER_SAVE: int
 ICON_FOUR_BOXES: int
 ICON_FX: int
 ICON_GEAR: int
@@ -1386,29 +1399,35 @@
 ICON_PLAYER_PREVIOUS: int
 ICON_PLAYER_RECORD: int
 ICON_PLAYER_STOP: int
 ICON_POT: int
 ICON_PRINTER: int
 ICON_REDO: int
 ICON_REDO_FILL: int
+ICON_REG_EXP: int
 ICON_REPEAT: int
 ICON_REPEAT_FILL: int
 ICON_REREDO: int
 ICON_REREDO_FILL: int
 ICON_RESIZE: int
+ICON_RESTART: int
+ICON_ROM: int
 ICON_ROTATE: int
 ICON_ROTATE_FILL: int
 ICON_RUBBER: int
 ICON_SCALE: int
 ICON_SHIELD: int
 ICON_SHUFFLE: int
 ICON_SHUFFLE_FILL: int
 ICON_SPECIAL: int
 ICON_SQUARE_TOGGLE: int
 ICON_STAR: int
+ICON_STEP_INTO: int
+ICON_STEP_OUT: int
+ICON_STEP_OVER: int
 ICON_SUITCASE: int
 ICON_SUITCASE_ZIP: int
 ICON_SYMMETRY: int
 ICON_SYMMETRY_HORIZONTAL: int
 ICON_SYMMETRY_VERTICAL: int
 ICON_TARGET: int
 ICON_TARGET_BIG: int
@@ -1446,14 +1465,17 @@
         ...
 def ImageAlphaMask(image: Any,alphaMask: Image,) -> None:
         """Apply alpha mask to image"""
         ...
 def ImageAlphaPremultiply(image: Any,) -> None:
         """Premultiply alpha channel"""
         ...
+def ImageBlurGaussian(image: Any,blurSize: int,) -> None:
+        """Apply Gaussian blur using a box blur approximation"""
+        ...
 def ImageClearBackground(dst: Any,color: Color,) -> None:
         """Clear image background with given color"""
         ...
 def ImageColorBrightness(image: Any,brightness: int,) -> None:
         """Modify image color: brightness (-255 to 255)"""
         ...
 def ImageColorContrast(image: Any,contrast: float,) -> None:
@@ -1480,18 +1502,24 @@
 def ImageDither(image: Any,rBpp: int,gBpp: int,bBpp: int,aBpp: int,) -> None:
         """Dither image data to 16bpp or lower (Floyd-Steinberg dithering)"""
         ...
 def ImageDraw(dst: Any,src: Image,srcRec: Rectangle,dstRec: Rectangle,tint: Color,) -> None:
         """Draw a source image within a destination image (tint applied to source)"""
         ...
 def ImageDrawCircle(dst: Any,centerX: int,centerY: int,radius: int,color: Color,) -> None:
-        """Draw circle within an image"""
+        """Draw a filled circle within an image"""
+        ...
+def ImageDrawCircleLines(dst: Any,centerX: int,centerY: int,radius: int,color: Color,) -> None:
+        """Draw circle outline within an image"""
+        ...
+def ImageDrawCircleLinesV(dst: Any,center: Vector2,radius: int,color: Color,) -> None:
+        """Draw circle outline within an image (Vector version)"""
         ...
 def ImageDrawCircleV(dst: Any,center: Vector2,radius: int,color: Color,) -> None:
-        """Draw circle within an image (Vector version)"""
+        """Draw a filled circle within an image (Vector version)"""
         ...
 def ImageDrawLine(dst: Any,startPosX: int,startPosY: int,endPosX: int,endPosY: int,color: Color,) -> None:
         """Draw line within an image"""
         ...
 def ImageDrawLineV(dst: Any,start: Vector2,end: Vector2,color: Color,) -> None:
         """Draw line within an image (Vector version)"""
         ...
@@ -1574,26 +1602,32 @@
         ...
 def IsAudioStreamPlaying(stream: AudioStream,) -> bool:
         """Check if audio stream is playing"""
         ...
 def IsAudioStreamProcessed(stream: AudioStream,) -> bool:
         """Check if any audio stream buffers requires refill"""
         ...
+def IsAudioStreamReady(stream: AudioStream,) -> bool:
+        """Checks if an audio stream is ready"""
+        ...
 def IsCursorHidden() -> bool:
         """Check if cursor is not visible"""
         ...
 def IsCursorOnScreen() -> bool:
         """Check if cursor is on the screen"""
         ...
 def IsFileDropped() -> bool:
         """Check if a file has been dropped into window"""
         ...
 def IsFileExtension(fileName: str,ext: str,) -> bool:
         """Check file extension (including point: .png, .wav)"""
         ...
+def IsFontReady(font: Font,) -> bool:
+        """Check if a font is ready"""
+        ...
 def IsGamepadAvailable(gamepad: int,) -> bool:
         """Check if a gamepad is available"""
         ...
 def IsGamepadButtonDown(gamepad: int,button: int,) -> bool:
         """Check if a gamepad button is being pressed"""
         ...
 def IsGamepadButtonPressed(gamepad: int,button: int,) -> bool:
@@ -1604,50 +1638,77 @@
         ...
 def IsGamepadButtonUp(gamepad: int,button: int,) -> bool:
         """Check if a gamepad button is NOT being pressed"""
         ...
 def IsGestureDetected(gesture: int,) -> bool:
         """Check if a gesture have been detected"""
         ...
+def IsImageReady(image: Image,) -> bool:
+        """Check if an image is ready"""
+        ...
 def IsKeyDown(key: int,) -> bool:
         """Check if a key is being pressed"""
         ...
 def IsKeyPressed(key: int,) -> bool:
         """Check if a key has been pressed once"""
         ...
 def IsKeyReleased(key: int,) -> bool:
         """Check if a key has been released once"""
         ...
 def IsKeyUp(key: int,) -> bool:
         """Check if a key is NOT being pressed"""
         ...
+def IsMaterialReady(material: Material,) -> bool:
+        """Check if a material is ready"""
+        ...
 def IsModelAnimationValid(model: Model,anim: ModelAnimation,) -> bool:
         """Check model animation skeleton match"""
         ...
+def IsModelReady(model: Model,) -> bool:
+        """Check if a model is ready"""
+        ...
 def IsMouseButtonDown(button: int,) -> bool:
         """Check if a mouse button is being pressed"""
         ...
 def IsMouseButtonPressed(button: int,) -> bool:
         """Check if a mouse button has been pressed once"""
         ...
 def IsMouseButtonReleased(button: int,) -> bool:
         """Check if a mouse button has been released once"""
         ...
 def IsMouseButtonUp(button: int,) -> bool:
         """Check if a mouse button is NOT being pressed"""
         ...
+def IsMusicReady(music: Music,) -> bool:
+        """Checks if a music stream is ready"""
+        ...
 def IsMusicStreamPlaying(music: Music,) -> bool:
         """Check if music is playing"""
         ...
 def IsPathFile(path: str,) -> bool:
         """Check if a given path is a file or a directory"""
         ...
+def IsRenderTextureReady(target: RenderTexture,) -> bool:
+        """Check if a render texture is ready"""
+        ...
+def IsShaderReady(shader: Shader,) -> bool:
+        """Check if a shader is ready"""
+        ...
 def IsSoundPlaying(sound: Sound,) -> bool:
         """Check if a sound is currently playing"""
         ...
+def IsSoundReady(sound: Sound,) -> bool:
+        """Checks if a sound is ready"""
+        ...
+def IsTextureReady(texture: Texture,) -> bool:
+        """Check if a texture is ready"""
+        ...
+def IsWaveReady(wave: Wave,) -> bool:
+        """Checks if wave data is ready"""
+        ...
 def IsWindowFocused() -> bool:
         """Check if window is currently focused (only PLATFORM_DESKTOP)"""
         ...
 def IsWindowFullscreen() -> bool:
         """Check if window is currently fullscreen"""
         ...
 def IsWindowHidden() -> bool:
@@ -1897,14 +1958,17 @@
         ...
 def LoadTextureCubemap(image: Image,layout: int,) -> Texture:
         """Load cubemap from image, multiple image cubemap layouts supported"""
         ...
 def LoadTextureFromImage(image: Image,) -> Texture:
         """Load texture from image data"""
         ...
+def LoadUTF8(codepoints: Any,length: int,) -> str:
+        """Load UTF-8 text encoded from codepoints array"""
+        ...
 def LoadVrStereoConfig(device: VrDeviceInfo,) -> VrStereoConfig:
         """Load VR stereo config for VR simulator device parameters"""
         ...
 def LoadWave(fileName: str,) -> Wave:
         """Load wave data from file"""
         ...
 def LoadWaveFromMemory(fileType: str,fileData: str,dataSize: int,) -> Wave:
@@ -2072,19 +2136,14 @@
 NPATCH_THREE_PATCH_HORIZONTAL: int
 NPATCH_THREE_PATCH_VERTICAL: int
 def Normalize(float_0: float,float_1: float,float_2: float,) -> float:
         """float Normalize(float, float, float);
 
 CFFI C function from raylib._raylib_cffi.lib"""
         ...
-OPENGL_11: int
-OPENGL_21: int
-OPENGL_33: int
-OPENGL_43: int
-OPENGL_ES_20: int
 def OpenURL(url: str,) -> None:
         """Open URL with default system browser (if available)"""
         ...
 PHYSICS_CIRCLE: int
 PHYSICS_POLYGON: int
 PIXELFORMAT_COMPRESSED_ASTC_4x4_RGBA: int
 PIXELFORMAT_COMPRESSED_ASTC_8x8_RGBA: int
@@ -2138,17 +2197,14 @@
         ...
 def PlayMusicStream(music: Music,) -> None:
         """Start music playing"""
         ...
 def PlaySound(sound: Sound,) -> None:
         """Play a sound"""
         ...
-def PlaySoundMulti(sound: Sound,) -> None:
-        """Play a sound (using multichannel buffer pool)"""
-        ...
 def PollInputEvents() -> None:
         """Register all input events"""
         ...
 def QuaternionAdd(Vector4_0: Vector4,Vector4_1: Vector4,) -> Vector4:
         """struct Vector4 QuaternionAdd(struct Vector4, struct Vector4);
 
 CFFI C function from raylib._raylib_cffi.lib"""
@@ -2283,24 +2339,32 @@
 RL_ATTACHMENT_STENCIL: int
 RL_ATTACHMENT_TEXTURE2D: int
 RL_BLEND_ADDITIVE: int
 RL_BLEND_ADD_COLORS: int
 RL_BLEND_ALPHA: int
 RL_BLEND_ALPHA_PREMULTIPLY: int
 RL_BLEND_CUSTOM: int
+RL_BLEND_CUSTOM_SEPARATE: int
 RL_BLEND_MULTIPLIED: int
 RL_BLEND_SUBTRACT_COLORS: int
+RL_CULL_FACE_BACK: int
+RL_CULL_FACE_FRONT: int
 RL_LOG_ALL: int
 RL_LOG_DEBUG: int
 RL_LOG_ERROR: int
 RL_LOG_FATAL: int
 RL_LOG_INFO: int
 RL_LOG_NONE: int
 RL_LOG_TRACE: int
 RL_LOG_WARNING: int
+RL_OPENGL_11: int
+RL_OPENGL_21: int
+RL_OPENGL_33: int
+RL_OPENGL_43: int
+RL_OPENGL_ES_20: int
 RL_PIXELFORMAT_COMPRESSED_ASTC_4x4_RGBA: int
 RL_PIXELFORMAT_COMPRESSED_ASTC_8x8_RGBA: int
 RL_PIXELFORMAT_COMPRESSED_DXT1_RGB: int
 RL_PIXELFORMAT_COMPRESSED_DXT1_RGBA: int
 RL_PIXELFORMAT_COMPRESSED_DXT3_RGBA: int
 RL_PIXELFORMAT_COMPRESSED_DXT5_RGBA: int
 RL_PIXELFORMAT_COMPRESSED_ETC1_RGB: int
@@ -2462,29 +2526,14 @@
         ...
 def SetAudioStreamPitch(stream: AudioStream,pitch: float,) -> None:
         """Set pitch for audio stream (1.0 is base level)"""
         ...
 def SetAudioStreamVolume(stream: AudioStream,volume: float,) -> None:
         """Set volume for audio stream (1.0 is max level)"""
         ...
-def SetCameraAltControl(keyAlt: int,) -> None:
-        """Set camera alt key to combine with mouse movement (free camera)"""
-        ...
-def SetCameraMode(camera: Camera3D,mode: int,) -> None:
-        """Set camera mode (multiple camera modes available)"""
-        ...
-def SetCameraMoveControls(keyFront: int,keyBack: int,keyRight: int,keyLeft: int,keyUp: int,keyDown: int,) -> None:
-        """Set camera move controls (1st person and 3rd person cameras)"""
-        ...
-def SetCameraPanControl(keyPan: int,) -> None:
-        """Set camera pan key to combine with mouse movement (free camera)"""
-        ...
-def SetCameraSmoothZoomControl(keySmoothZoom: int,) -> None:
-        """Set camera smooth zoom key to combine with mouse (free camera)"""
-        ...
 def SetClipboardText(text: str,) -> None:
         """Set clipboard text content"""
         ...
 def SetConfigFlags(flags: int,) -> None:
         """Setup init configuration flags (view FLAGS)"""
         ...
 def SetExitKey(key: int,) -> None:
@@ -2595,15 +2644,18 @@
 def SetTraceLogCallback(callback: str,) -> None:
         """Set custom trace log"""
         ...
 def SetTraceLogLevel(logLevel: int,) -> None:
         """Set the current threshold (minimum) log level"""
         ...
 def SetWindowIcon(image: Image,) -> None:
-        """Set icon for window (only PLATFORM_DESKTOP)"""
+        """Set icon for window (single image, RGBA 32bit, only PLATFORM_DESKTOP)"""
+        ...
+def SetWindowIcons(images: Any,count: int,) -> None:
+        """Set icon for window (multiple images, RGBA 32bit, only PLATFORM_DESKTOP)"""
         ...
 def SetWindowMinSize(width: int,height: int,) -> None:
         """Set window minimum dimensions (for FLAG_WINDOW_RESIZABLE)"""
         ...
 def SetWindowMonitor(monitor: int,) -> None:
         """Set monitor for the current window (fullscreen mode)"""
         ...
@@ -2630,17 +2682,14 @@
         ...
 def StopMusicStream(music: Music,) -> None:
         """Stop music playing"""
         ...
 def StopSound(sound: Sound,) -> None:
         """Stop playing a sound"""
         ...
-def StopSoundMulti() -> None:
-        """Stop any sound playing (using multichannel buffer pool)"""
-        ...
 def SwapScreenBuffer() -> None:
         """Swap back buffer with front buffer (screen drawing)"""
         ...
 TEXTBOX: int
 TEXTURE_FILTER_ANISOTROPIC_16X: int
 TEXTURE_FILTER_ANISOTROPIC_4X: int
 TEXTURE_FILTER_ANISOTROPIC_8X: int
@@ -2648,36 +2697,36 @@
 TEXTURE_FILTER_POINT: int
 TEXTURE_FILTER_TRILINEAR: int
 TEXTURE_WRAP_CLAMP: int
 TEXTURE_WRAP_MIRROR_CLAMP: int
 TEXTURE_WRAP_MIRROR_REPEAT: int
 TEXTURE_WRAP_REPEAT: int
 TEXT_ALIGNMENT: int
+TEXT_ALIGNMENT_VERTICAL: int
 TEXT_ALIGN_CENTER: int
 TEXT_ALIGN_LEFT: int
 TEXT_ALIGN_RIGHT: int
 TEXT_COLOR_DISABLED: int
 TEXT_COLOR_FOCUSED: int
 TEXT_COLOR_NORMAL: int
 TEXT_COLOR_PRESSED: int
 TEXT_INNER_PADDING: int
 TEXT_LINES_SPACING: int
+TEXT_MULTILINE: int
 TEXT_PADDING: int
 TEXT_SIZE: int
 TEXT_SPACING: int
+TEXT_WRAP_MODE: int
 TOGGLE: int
 def TakeScreenshot(fileName: str,) -> None:
         """Takes a screenshot of current screen (filename extension defines format)"""
         ...
 def TextAppend(text: str,append: str,position: Any,) -> None:
         """Append text at specific position and move cursor!"""
         ...
-def TextCodepointsToUTF8(codepoints: Any,length: int,) -> str:
-        """Encode text as codepoints array into UTF-8 text string (WARNING: memory must be freed!)"""
-        ...
 def TextCopy(dst: str,src: str,) -> int:
         """Copy one string to another, returns bytes copied"""
         ...
 def TextFindIndex(text: str,find: str,) -> int:
         """Find first text occurrence within a string"""
         ...
 def TextFormat(*args) -> str:
@@ -2766,17 +2815,14 @@
         ...
 def UnloadModelAnimation(anim: ModelAnimation,) -> None:
         """Unload animation data"""
         ...
 def UnloadModelAnimations(animations: Any,count: int,) -> None:
         """Unload animation array data"""
         ...
-def UnloadModelKeepMeshes(model: Model,) -> None:
-        """Unload model (but not meshes) from memory (RAM and/or VRAM)"""
-        ...
 def UnloadMusicStream(music: Music,) -> None:
         """Unload music stream"""
         ...
 def UnloadRenderTexture(target: RenderTexture,) -> None:
         """Unload render texture from GPU memory (VRAM)"""
         ...
 def UnloadShader(shader: Shader,) -> None:
@@ -2784,29 +2830,35 @@
         ...
 def UnloadSound(sound: Sound,) -> None:
         """Unload sound"""
         ...
 def UnloadTexture(texture: Texture,) -> None:
         """Unload texture from GPU memory (VRAM)"""
         ...
+def UnloadUTF8(text: str,) -> None:
+        """Unload UTF-8 text encoded from codepoints array"""
+        ...
 def UnloadVrStereoConfig(config: VrStereoConfig,) -> None:
         """Unload VR stereo config"""
         ...
 def UnloadWave(wave: Wave,) -> None:
         """Unload wave data"""
         ...
 def UnloadWaveSamples(samples: Any,) -> None:
         """Unload samples data loaded with LoadWaveSamples()"""
         ...
 def UpdateAudioStream(stream: AudioStream,data: Any,frameCount: int,) -> None:
         """Update audio stream buffers with data"""
         ...
-def UpdateCamera(camera: Any,) -> None:
+def UpdateCamera(camera: Any,mode: int,) -> None:
         """Update camera position for selected mode"""
         ...
+def UpdateCameraPro(camera: Any,movement: Vector3,rotation: Vector3,zoom: float,) -> None:
+        """Update camera movement/rotation"""
+        ...
 def UpdateMeshBuffer(mesh: Mesh,index: int,data: Any,dataSize: int,offset: int,) -> None:
         """Update mesh vertex data in GPU for a specific buffer index"""
         ...
 def UpdateModelAnimation(model: Model,anim: ModelAnimation,frame: int,) -> None:
         """Update model animation pose"""
         ...
 def UpdateMusicStream(music: Music,) -> None:
@@ -2896,14 +2948,19 @@
 CFFI C function from raylib._raylib_cffi.lib"""
         ...
 def Vector2Lerp(Vector2_0: Vector2,Vector2_1: Vector2,float_2: float,) -> Vector2:
         """struct Vector2 Vector2Lerp(struct Vector2, struct Vector2, float);
 
 CFFI C function from raylib._raylib_cffi.lib"""
         ...
+def Vector2LineAngle(Vector2_0: Vector2,Vector2_1: Vector2,) -> float:
+        """float Vector2LineAngle(struct Vector2, struct Vector2);
+
+CFFI C function from raylib._raylib_cffi.lib"""
+        ...
 def Vector2MoveTowards(Vector2_0: Vector2,Vector2_1: Vector2,float_2: float,) -> Vector2:
         """struct Vector2 Vector2MoveTowards(struct Vector2, struct Vector2, float);
 
 CFFI C function from raylib._raylib_cffi.lib"""
         ...
 def Vector2Multiply(Vector2_0: Vector2,Vector2_1: Vector2,) -> Vector2:
         """struct Vector2 Vector2Multiply(struct Vector2, struct Vector2);
@@ -3166,16 +3223,16 @@
 CFFI C function from raylib._raylib_cffi.lib"""
         ...
 def rlBegin(int_0: int,) -> None:
         """void rlBegin(int);
 
 CFFI C function from raylib._raylib_cffi.lib"""
         ...
-def rlBindImageTexture(unsignedint_0: int,unsignedint_1: int,unsignedint_2: int,int_3: int,) -> None:
-        """void rlBindImageTexture(unsigned int, unsigned int, unsigned int, int);
+def rlBindImageTexture(unsignedint_0: int,unsignedint_1: int,int_2: int,_Bool_3: bool,) -> None:
+        """void rlBindImageTexture(unsigned int, unsigned int, int, _Bool);
 
 CFFI C function from raylib._raylib_cffi.lib"""
         ...
 def rlBindShaderBuffer(unsignedint_0: int,unsignedint_1: int,) -> None:
         """void rlBindShaderBuffer(unsigned int, unsigned int);
 
 CFFI C function from raylib._raylib_cffi.lib"""
@@ -3221,16 +3278,21 @@
 CFFI C function from raylib._raylib_cffi.lib"""
         ...
 def rlComputeShaderDispatch(unsignedint_0: int,unsignedint_1: int,unsignedint_2: int,) -> None:
         """void rlComputeShaderDispatch(unsigned int, unsigned int, unsigned int);
 
 CFFI C function from raylib._raylib_cffi.lib"""
         ...
-def rlCopyBuffersElements(unsignedint_0: int,unsignedint_1: int,unsignedlonglong_2: int,unsignedlonglong_3: int,unsignedlonglong_4: int,) -> None:
-        """void rlCopyBuffersElements(unsigned int, unsigned int, unsigned long long, unsigned long long, unsigned long long);
+def rlCopyShaderBuffer(unsignedint_0: int,unsignedint_1: int,unsignedint_2: int,unsignedint_3: int,unsignedint_4: int,) -> None:
+        """void rlCopyShaderBuffer(unsigned int, unsigned int, unsigned int, unsigned int, unsigned int);
+
+CFFI C function from raylib._raylib_cffi.lib"""
+        ...
+def rlCubemapParameters(unsignedint_0: int,int_1: int,int_2: int,) -> None:
+        """void rlCubemapParameters(unsigned int, int, int);
 
 CFFI C function from raylib._raylib_cffi.lib"""
         ...
 def rlDisableBackfaceCulling() -> None:
         """void rlDisableBackfaceCulling();
 
 CFFI C function from raylib._raylib_cffi.lib"""
@@ -3502,15 +3564,15 @@
         ...
 def rlGetPixelFormatName(unsignedint_0: int,) -> str:
         """char *rlGetPixelFormatName(unsigned int);
 
 CFFI C function from raylib._raylib_cffi.lib"""
         ...
 def rlGetShaderBufferSize(unsignedint_0: int,) -> int:
-        """unsigned long long rlGetShaderBufferSize(unsigned int);
+        """unsigned int rlGetShaderBufferSize(unsigned int);
 
 CFFI C function from raylib._raylib_cffi.lib"""
         ...
 def rlGetShaderIdDefault() -> int:
         """unsigned int rlGetShaderIdDefault();
 
 CFFI C function from raylib._raylib_cffi.lib"""
@@ -3566,16 +3628,16 @@
 CFFI C function from raylib._raylib_cffi.lib"""
         ...
 def rlLoadRenderBatch(int_0: int,int_1: int,) -> rlRenderBatch:
         """struct rlRenderBatch rlLoadRenderBatch(int, int);
 
 CFFI C function from raylib._raylib_cffi.lib"""
         ...
-def rlLoadShaderBuffer(unsignedlonglong_0: int,void_pointer_1: Any,int_2: int,) -> int:
-        """unsigned int rlLoadShaderBuffer(unsigned long long, void *, int);
+def rlLoadShaderBuffer(unsignedint_0: int,void_pointer_1: Any,int_2: int,) -> int:
+        """unsigned int rlLoadShaderBuffer(unsigned int, void *, int);
 
 CFFI C function from raylib._raylib_cffi.lib"""
         ...
 def rlLoadShaderCode(str_0: str,str_1: str,) -> int:
         """unsigned int rlLoadShaderCode(char *, char *);
 
 CFFI C function from raylib._raylib_cffi.lib"""
@@ -3646,16 +3708,16 @@
 CFFI C function from raylib._raylib_cffi.lib"""
         ...
 def rlReadScreenPixels(int_0: int,int_1: int,) -> str:
         """unsigned char *rlReadScreenPixels(int, int);
 
 CFFI C function from raylib._raylib_cffi.lib"""
         ...
-def rlReadShaderBufferElements(unsignedint_0: int,void_pointer_1: Any,unsignedlonglong_2: int,unsignedlonglong_3: int,) -> None:
-        """void rlReadShaderBufferElements(unsigned int, void *, unsigned long long, unsigned long long);
+def rlReadShaderBuffer(unsignedint_0: int,void_pointer_1: Any,unsignedint_2: int,unsignedint_3: int,) -> None:
+        """void rlReadShaderBuffer(unsigned int, void *, unsigned int, unsigned int);
 
 CFFI C function from raylib._raylib_cffi.lib"""
         ...
 def rlReadTexturePixels(unsignedint_0: int,int_1: int,int_2: int,int_3: int,) -> Any:
         """void *rlReadTexturePixels(unsigned int, int, int, int);
 
 CFFI C function from raylib._raylib_cffi.lib"""
@@ -3676,19 +3738,29 @@
 CFFI C function from raylib._raylib_cffi.lib"""
         ...
 def rlSetBlendFactors(int_0: int,int_1: int,int_2: int,) -> None:
         """void rlSetBlendFactors(int, int, int);
 
 CFFI C function from raylib._raylib_cffi.lib"""
         ...
+def rlSetBlendFactorsSeparate(int_0: int,int_1: int,int_2: int,int_3: int,int_4: int,int_5: int,) -> None:
+        """void rlSetBlendFactorsSeparate(int, int, int, int, int, int);
+
+CFFI C function from raylib._raylib_cffi.lib"""
+        ...
 def rlSetBlendMode(int_0: int,) -> None:
         """void rlSetBlendMode(int);
 
 CFFI C function from raylib._raylib_cffi.lib"""
         ...
+def rlSetCullFace(int_0: int,) -> None:
+        """void rlSetCullFace(int);
+
+CFFI C function from raylib._raylib_cffi.lib"""
+        ...
 def rlSetFramebufferHeight(int_0: int,) -> None:
         """void rlSetFramebufferHeight(int);
 
 CFFI C function from raylib._raylib_cffi.lib"""
         ...
 def rlSetFramebufferWidth(int_0: int,) -> None:
         """void rlSetFramebufferWidth(int);
@@ -3811,16 +3883,16 @@
 CFFI C function from raylib._raylib_cffi.lib"""
         ...
 def rlUnloadVertexBuffer(unsignedint_0: int,) -> None:
         """void rlUnloadVertexBuffer(unsigned int);
 
 CFFI C function from raylib._raylib_cffi.lib"""
         ...
-def rlUpdateShaderBufferElements(unsignedint_0: int,void_pointer_1: Any,unsignedlonglong_2: int,unsignedlonglong_3: int,) -> None:
-        """void rlUpdateShaderBufferElements(unsigned int, void *, unsigned long long, unsigned long long);
+def rlUpdateShaderBuffer(unsignedint_0: int,void_pointer_1: Any,unsignedint_2: int,unsignedint_3: int,) -> None:
+        """void rlUpdateShaderBuffer(unsigned int, void *, unsigned int, unsigned int);
 
 CFFI C function from raylib._raylib_cffi.lib"""
         ...
 def rlUpdateTexture(unsignedint_0: int,int_1: int,int_2: int,int_3: int,int_4: int,int_5: int,void_pointer_6: Any,) -> None:
         """void rlUpdateTexture(unsigned int, int, int, int, int, int, void *);
 
 CFFI C function from raylib._raylib_cffi.lib"""
@@ -3948,14 +4020,15 @@
 VrStereoConfig: struct
 Wave: struct
 float16: struct
 float3: struct
 rAudioBuffer: struct
 rAudioProcessor: struct
 rlBlendMode: int
+rlCullMode: int
 rlDrawCall: struct
 rlFramebufferAttachTextureType: int
 rlFramebufferAttachType: int
 rlGlVersion: int
 rlPixelFormat: int
 rlRenderBatch: struct
 rlShaderAttributeDataType: int
```

### Comparing `raylib-4.2.1.2/raylib/build.py` & `raylib-4.5.0.0/raylib/build.py`

 * *Files identical despite different names*

### Comparing `raylib-4.2.1.2/raylib/colors.py` & `raylib-4.5.0.0/raylib/colors.py`

 * *Files identical despite different names*

### Comparing `raylib-4.2.1.2/raylib/enums.py` & `raylib-4.5.0.0/raylib/enums.py`

 * *Files 4% similar despite different names*

```diff
@@ -301,14 +301,15 @@
     BLEND_ALPHA = 0
     BLEND_ADDITIVE = 1
     BLEND_MULTIPLIED = 2
     BLEND_ADD_COLORS = 3
     BLEND_SUBTRACT_COLORS = 4
     BLEND_ALPHA_PREMULTIPLY = 5
     BLEND_CUSTOM = 6
+    BLEND_CUSTOM_SEPARATE = 7
 
 class Gesture(IntEnum):
     GESTURE_NONE = 0
     GESTURE_TAP = 1
     GESTURE_DOUBLETAP = 2
     GESTURE_HOLD = 4
     GESTURE_DRAG = 8
@@ -416,14 +417,17 @@
 class GuiDropdownBoxProperty(IntEnum):
     ARROW_PADDING = 16
     DROPDOWN_ITEMS_SPACING = 17
 
 class GuiTextBoxProperty(IntEnum):
     TEXT_INNER_PADDING = 16
     TEXT_LINES_SPACING = 17
+    TEXT_ALIGNMENT_VERTICAL = 18
+    TEXT_MULTILINE = 19
+    TEXT_WRAP_MODE = 20
 
 class GuiSpinnerProperty(IntEnum):
     SPIN_BUTTON_WIDTH = 16
     SPIN_BUTTON_SPACING = 17
 
 class GuiListViewProperty(IntEnum):
     LIST_ITEMS_HEIGHT = 16
@@ -641,27 +645,27 @@
     ICON_HIDPI = 199
     ICON_FILETYPE_BINARY = 200
     ICON_HEX = 201
     ICON_SHIELD = 202
     ICON_FILE_NEW = 203
     ICON_FOLDER_ADD = 204
     ICON_ALARM = 205
-    ICON_206 = 206
-    ICON_207 = 207
-    ICON_208 = 208
-    ICON_209 = 209
-    ICON_210 = 210
-    ICON_211 = 211
-    ICON_212 = 212
-    ICON_213 = 213
-    ICON_214 = 214
-    ICON_215 = 215
-    ICON_216 = 216
-    ICON_217 = 217
-    ICON_218 = 218
+    ICON_CPU = 206
+    ICON_ROM = 207
+    ICON_STEP_OVER = 208
+    ICON_STEP_INTO = 209
+    ICON_STEP_OUT = 210
+    ICON_RESTART = 211
+    ICON_BREAKPOINT_ON = 212
+    ICON_BREAKPOINT_OFF = 213
+    ICON_BURGER_MENU = 214
+    ICON_CASE_SENSITIVE = 215
+    ICON_REG_EXP = 216
+    ICON_FOLDER = 217
+    ICON_FILE = 218
     ICON_219 = 219
     ICON_220 = 220
     ICON_221 = 221
     ICON_222 = 222
     ICON_223 = 223
     ICON_224 = 224
     ICON_225 = 225
```

### Comparing `raylib-4.2.1.2/raylib.egg-info/PKG-INFO` & `raylib-4.5.0.0/raylib.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 Metadata-Version: 2.1
 Name: raylib
-Version: 4.2.1.2
+Version: 4.5.0.0
 Summary: Python CFFI bindings for Raylib
 Home-page: https://github.com/electronstudio/raylib-python-cffi
 Author: Electron Studio
 Author-email: github@electronstudio.co.uk
 License: EPL-2.0
 Classifier: License :: OSI Approved :: Eclipse Public License 2.0 (EPL-2.0)
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# Python Bindings for Raylib 4.2
+# Python Bindings for Raylib 4.5
 
 New CFFI API static bindings.
 * Automatically generated to be as close as possible to 
 original Raylib.
 * Faster, fewer bugs and easier to maintain than ctypes.
 * Commercial-friendly license.
 * Docstrings and auto-completion.
```

### Comparing `raylib-4.2.1.2/setup.py` & `raylib-4.5.0.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,14 +26,15 @@
     url="https://github.com/electronstudio/raylib-python-cffi",
     author="Electron Studio",
     author_email="github@electronstudio.co.uk",
     license="EPL-2.0",
     classifiers=[
         "License :: OSI Approved :: Eclipse Public License 2.0 (EPL-2.0)",
         "Programming Language :: Python :: 3",
+        "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.7",
     ],
     packages=["raylib", "pyray"],
     include_package_data=True,
```

