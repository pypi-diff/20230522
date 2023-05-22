# Comparing `tmp/flet_ivid-1.0.tar.gz` & `tmp/flet_ivid-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flet_ivid-1.0.tar", last modified: Mon May 22 08:32:24 2023, max compression
+gzip compressed data, was "flet_ivid-1.1.tar", last modified: Mon May 22 09:54:03 2023, max compression
```

## Comparing `flet_ivid-1.0.tar` & `flet_ivid-1.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 yousifaladwani   (501) staff       (20)        0 2023-05-22 08:32:24.066204 flet_ivid-1.0/
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     1060 2023-05-22 08:17:53.000000 flet_ivid-1.0/LICENSE
--rw-r--r--   0 yousifaladwani   (501) staff       (20)       18 2023-05-22 08:19:20.000000 flet_ivid-1.0/MANIFEST.in
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     1395 2023-05-22 08:32:24.066073 flet_ivid-1.0/PKG-INFO
--rw-r--r--   0 yousifaladwani   (501) staff       (20)      998 2023-05-22 08:31:50.000000 flet_ivid-1.0/README.md
-drwxr-xr-x   0 yousifaladwani   (501) staff       (20)        0 2023-05-22 08:32:24.065204 flet_ivid-1.0/flet_ivid/
--rw-r--r--   0 yousifaladwani   (501) staff       (20)       44 2023-05-22 08:18:08.000000 flet_ivid-1.0/flet_ivid/__init__.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     8309 2023-05-22 08:18:08.000000 flet_ivid-1.0/flet_ivid/video_container.py
-drwxr-xr-x   0 yousifaladwani   (501) staff       (20)        0 2023-05-22 08:32:24.065868 flet_ivid-1.0/flet_ivid.egg-info/
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     1395 2023-05-22 08:32:24.000000 flet_ivid-1.0/flet_ivid.egg-info/PKG-INFO
--rw-r--r--   0 yousifaladwani   (501) staff       (20)      268 2023-05-22 08:32:24.000000 flet_ivid-1.0/flet_ivid.egg-info/SOURCES.txt
--rw-r--r--   0 yousifaladwani   (501) staff       (20)        1 2023-05-22 08:32:24.000000 flet_ivid-1.0/flet_ivid.egg-info/dependency_links.txt
--rw-r--r--   0 yousifaladwani   (501) staff       (20)       34 2023-05-22 08:32:24.000000 flet_ivid-1.0/flet_ivid.egg-info/requires.txt
--rw-r--r--   0 yousifaladwani   (501) staff       (20)       10 2023-05-22 08:32:24.000000 flet_ivid-1.0/flet_ivid.egg-info/top_level.txt
--rw-r--r--   0 yousifaladwani   (501) staff       (20)      103 2023-05-22 08:19:03.000000 flet_ivid-1.0/pyproject.toml
--rw-r--r--   0 yousifaladwani   (501) staff       (20)       38 2023-05-22 08:32:24.066249 flet_ivid-1.0/setup.cfg
--rw-r--r--   0 yousifaladwani   (501) staff       (20)      671 2023-05-22 08:22:51.000000 flet_ivid-1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 09:54:03.057237 flet_ivid-1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-05-22 09:53:52.000000 flet_ivid-1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-22 09:53:52.000000 flet_ivid-1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-05-22 09:54:03.057237 flet_ivid-1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-05-22 09:53:52.000000 flet_ivid-1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 09:54:03.057237 flet_ivid-1.1/flet_ivid/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-22 09:53:52.000000 flet_ivid-1.1/flet_ivid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7936 2023-05-22 09:53:52.000000 flet_ivid-1.1/flet_ivid/video_container.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 09:54:03.057237 flet_ivid-1.1/flet_ivid.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-05-22 09:54:03.000000 flet_ivid-1.1/flet_ivid.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-05-22 09:54:03.000000 flet_ivid-1.1/flet_ivid.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 09:54:03.000000 flet_ivid-1.1/flet_ivid.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-22 09:54:03.000000 flet_ivid-1.1/flet_ivid.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-22 09:54:03.000000 flet_ivid-1.1/flet_ivid.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-22 09:53:52.000000 flet_ivid-1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 09:54:03.057237 flet_ivid-1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      671 2023-05-22 09:53:52.000000 flet_ivid-1.1/setup.py
```

### Comparing `flet_ivid-1.0/LICENSE` & `flet_ivid-1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `flet_ivid-1.0/PKG-INFO` & `flet_ivid-1.1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flet_ivid
-Version: 1.0
+Version: 1.1
 Summary: A package tool that provide basic video player for flet.
 Home-page: https://github.com/SKbarbon/flet_ived
 Author: SKbarbon
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
@@ -37,9 +37,29 @@
     vc.play() # call `play` function to make the video start playing.
 
     # Call `vc.pause()` to stop the video from playing.
 
 flet.app(target=main)
 ```
 
+### ⚠️ If your device is old!
+This package can load the video from file source while show the video at the same time. But this is not so with old devices or the devices that have a weak performance, So you must set `play_after_loading` to true. For example:
+
+```python
+from flet_ivid import VideoContainer # import the package
+import flet
+
+
+def main (page:flet.Page):
+    page.bgcolor = "black"
+    vc = VideoContainer("yourvideo.mp4", play_after_loading=True, border_radius=18, expand=True) # This is a VideoContainer
+    page.add(flet.Row([vc], alignment="center"))
+
+    vc.play() # call `play` function to make the video start playing.
+
+    # Call `vc.pause()` to stop the video from playing.
+
+flet.app(target=main)
+```
+
 ## Note
-`Note`: **You should know that this built to be used for basic small or normal usage, its can NOT be used for big production cases, its a RAM consuming and slow for biger videos..**
+`Note`: **You should know that this built to be used for basic small or normal usage, its can NOT be used for big production cases, if you do so it will be a RAM consuming and slow for biger videos..**
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `flet_ivid-1.0/README.md` & `flet_ivid-1.1/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -25,9 +25,29 @@
     vc.play() # call `play` function to make the video start playing.
 
     # Call `vc.pause()` to stop the video from playing.
 
 flet.app(target=main)
 ```
 
+### ⚠️ If your device is old!
+This package can load the video from file source while show the video at the same time. But this is not so with old devices or the devices that have a weak performance, So you must set `play_after_loading` to true. For example:
+
+```python
+from flet_ivid import VideoContainer # import the package
+import flet
+
+
+def main (page:flet.Page):
+    page.bgcolor = "black"
+    vc = VideoContainer("yourvideo.mp4", play_after_loading=True, border_radius=18, expand=True) # This is a VideoContainer
+    page.add(flet.Row([vc], alignment="center"))
+
+    vc.play() # call `play` function to make the video start playing.
+
+    # Call `vc.pause()` to stop the video from playing.
+
+flet.app(target=main)
+```
+
 ## Note
-`Note`: **You should know that this built to be used for basic small or normal usage, its can NOT be used for big production cases, its a RAM consuming and slow for biger videos..**
+`Note`: **You should know that this built to be used for basic small or normal usage, its can NOT be used for big production cases, if you do so it will be a RAM consuming and slow for biger videos..**
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `flet_ivid-1.0/flet_ivid/video_container.py` & `flet_ivid-1.1/flet_ivid/video_container.py`

 * *Files 16% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 from moviepy.editor import VideoFileClip
 import base64
 import time
 
 
 class VideoContainer (Container):
     """This will show a video you choose."""
-    def __init__(self, video_path:str, video_frame_fit_type:flet.ImageFit=None, content: Control | None = None, ref: Ref | None = None, key: str | None = None, width: OptionalNumber = None, height: OptionalNumber = None, left: OptionalNumber = None, top: OptionalNumber = None, right: OptionalNumber = None, bottom: OptionalNumber = None, expand: bool | int | None = None, col: ResponsiveNumber | None = None, opacity: OptionalNumber = None, rotate: RotateValue = None, scale: ScaleValue = None, offset: OffsetValue = None, aspect_ratio: OptionalNumber = None, animate_opacity: AnimationValue = None, animate_size: AnimationValue = None, animate_position: AnimationValue = None, animate_rotation: AnimationValue = None, animate_scale: AnimationValue = None, animate_offset: AnimationValue = None, on_animation_end=None, tooltip: str | None = None, visible: bool | None = None, disabled: bool | None = None, data: Any = None, padding: PaddingValue = None, margin: MarginValue = None, alignment: Alignment | None = None, bgcolor: str | None = None, gradient: Gradient | None = None, blend_mode: BlendMode = BlendMode.NONE, border: Border | None = None, border_radius: BorderRadiusValue = None, image_src: str | None = None, image_src_base64: str | None = None, image_repeat: ImageRepeat | None = None, image_fit: ImageFit | None = None, image_opacity: OptionalNumber = None, shape: BoxShape | None = None, clip_behavior: ClipBehavior | None = None, ink: bool | None = None, animate: AnimationValue = None, blur: float | int | Tuple[float | int, float | int] | Blur | None = None, shadow: BoxShadow | List[BoxShadow] | None = None, url: str | None = None, url_target: str | None = None, theme: Theme | None = None, theme_mode: ThemeMode | None = None, on_click=None, on_long_press=None, on_hover=None):
+    def __init__(self, video_path:str, play_after_loading=False, video_frame_fit_type:flet.ImageFit=None, content= None, ref = None, key = None, width = None, height= None, left = None, top = None, right = None, bottom= None, expand= None, col = None, opacity= None, rotate= None, scale= None, offset= None, aspect_ratio= None, animate_opacity= None, animate_size = None, animate_position= None, animate_rotation= None, animate_scale= None, animate_offset = None, on_animation_end=None, tooltip = None, visible = None, disabled= None, data = None, padding= None, margin= None, alignment = None, bgcolor= None, gradient= None, blend_mode=BlendMode.NONE, border= None, border_radius= None, image_src= None, image_src_base64= None, image_repeat=None, image_fit=None, image_opacity: OptionalNumber = None, shape=None, clip_behavior= None, ink= None, animate=None, blur=None, shadow= None, url=None, url_target=None, theme=None, theme_mode= None, on_click=None, on_long_press=None, on_hover=None):
         super().__init__(content, ref, key, width, height, left, top, right, bottom, expand, col, opacity, rotate, scale, offset, aspect_ratio, animate_opacity, animate_size, animate_position, animate_rotation, animate_scale, animate_offset, on_animation_end, tooltip, visible, disabled, data, padding, margin, alignment, bgcolor, gradient, blend_mode, border, border_radius, image_src, image_src_base64, image_repeat, image_fit, image_opacity, shape, clip_behavior, ink, animate, blur, shadow, url, url_target, theme, theme_mode, on_click, on_long_press, on_hover)
         if not os.path.isfile (video_path):
             raise FileNotFoundError ("Cannot find the video at the path you set.")
 
         self.__video_is_full_loaded = False
         self.__all_frames_of_video = []
         self.__audio_path = self.convert_video_to_audio (video_path=video_path)
@@ -38,15 +38,19 @@
         if video_frame_fit_type == None:
             self.video_frame_fit_type = flet.ImageFit.CONTAIN
 
         # generate the UI
         self.__ui ()
 
         # start a video reader.
-        threading.Thread(target=self.read_the_video, args=[video_path], daemon=True).start()
+        if play_after_loading:
+            print("Please wait the video is loading..\nThis will take a time based on your video size...")
+            self.read_the_video(video_path)
+        else:
+            threading.Thread(target=self.read_the_video, args=[video_path], daemon=True).start()
 
         # setup the video audio
         self.audio_path = self.convert_video_to_audio (video_path)
         self.get_audio_info(self.audio_path)
 
         # get video info
         self.get_video_duration(video_path)
@@ -97,16 +101,18 @@
             desired_time = (num + 1) * self.__frame_per_sleep
             
             # Calculate the remaining time to sleep
             sleep_time = max(0, desired_time - elapsed_time)
             time.sleep(sleep_time)
             # time.sleep(round(self.__frame_per_sleep, 3))
             num = num + 1
-        
         pygame.mixer.quit()
+
+        if len(self.__all_frames_of_video) != int(self.video_frames):
+            print("WARNING: Your device cant stream all video data and load it at the same time!, please set 'VideoContainer(play_after_loading=True)' to fix this issue.")
     
 
     def pause (self, *args):
         self.__video_played = False
 
     def read_the_video(self, video_path):
         # Open the video file
```

### Comparing `flet_ivid-1.0/flet_ivid.egg-info/PKG-INFO` & `flet_ivid-1.1/flet_ivid.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flet-ivid
-Version: 1.0
+Version: 1.1
 Summary: A package tool that provide basic video player for flet.
 Home-page: https://github.com/SKbarbon/flet_ived
 Author: SKbarbon
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
@@ -37,9 +37,29 @@
     vc.play() # call `play` function to make the video start playing.
 
     # Call `vc.pause()` to stop the video from playing.
 
 flet.app(target=main)
 ```
 
+### ⚠️ If your device is old!
+This package can load the video from file source while show the video at the same time. But this is not so with old devices or the devices that have a weak performance, So you must set `play_after_loading` to true. For example:
+
+```python
+from flet_ivid import VideoContainer # import the package
+import flet
+
+
+def main (page:flet.Page):
+    page.bgcolor = "black"
+    vc = VideoContainer("yourvideo.mp4", play_after_loading=True, border_radius=18, expand=True) # This is a VideoContainer
+    page.add(flet.Row([vc], alignment="center"))
+
+    vc.play() # call `play` function to make the video start playing.
+
+    # Call `vc.pause()` to stop the video from playing.
+
+flet.app(target=main)
+```
+
 ## Note
-`Note`: **You should know that this built to be used for basic small or normal usage, its can NOT be used for big production cases, its a RAM consuming and slow for biger videos..**
+`Note`: **You should know that this built to be used for basic small or normal usage, its can NOT be used for big production cases, if you do so it will be a RAM consuming and slow for biger videos..**
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `flet_ivid-1.0/setup.py` & `flet_ivid-1.1/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", encoding="utf-8") as f:
     long_des = str(f.read())
 
 setup(
     name='flet_ivid',
-    version='1.0',
+    version='1.1',
     author='SKbarbon',
     description='A package tool that provide basic video player for flet.',
     long_description=long_des,
     long_description_content_type='text/markdown',
     url='https://github.com/SKbarbon/flet_ived',
     install_requires=["flet", "pygame", "moviepy", "opencv-python"],
     packages=find_packages(),
```

