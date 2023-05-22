# Comparing `tmp/flet_ivid-1.1.tar.gz` & `tmp/flet_ivid-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flet_ivid-1.1.tar", last modified: Mon May 22 09:54:03 2023, max compression
+gzip compressed data, was "flet_ivid-1.2.tar", last modified: Mon May 22 16:53:49 2023, max compression
```

## Comparing `flet_ivid-1.1.tar` & `flet_ivid-1.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 09:54:03.057237 flet_ivid-1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-05-22 09:53:52.000000 flet_ivid-1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-22 09:53:52.000000 flet_ivid-1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-05-22 09:54:03.057237 flet_ivid-1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-05-22 09:53:52.000000 flet_ivid-1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 09:54:03.057237 flet_ivid-1.1/flet_ivid/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-22 09:53:52.000000 flet_ivid-1.1/flet_ivid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7936 2023-05-22 09:53:52.000000 flet_ivid-1.1/flet_ivid/video_container.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 09:54:03.057237 flet_ivid-1.1/flet_ivid.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-05-22 09:54:03.000000 flet_ivid-1.1/flet_ivid.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-05-22 09:54:03.000000 flet_ivid-1.1/flet_ivid.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 09:54:03.000000 flet_ivid-1.1/flet_ivid.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-22 09:54:03.000000 flet_ivid-1.1/flet_ivid.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-22 09:54:03.000000 flet_ivid-1.1/flet_ivid.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-22 09:53:52.000000 flet_ivid-1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 09:54:03.057237 flet_ivid-1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      671 2023-05-22 09:53:52.000000 flet_ivid-1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:53:49.129397 flet_ivid-1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-05-22 16:53:38.000000 flet_ivid-1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-22 16:53:38.000000 flet_ivid-1.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-05-22 16:53:49.129397 flet_ivid-1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-05-22 16:53:38.000000 flet_ivid-1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:53:49.125397 flet_ivid-1.2/flet_ivid/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-22 16:53:38.000000 flet_ivid-1.2/flet_ivid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9158 2023-05-22 16:53:38.000000 flet_ivid-1.2/flet_ivid/video_container.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:53:49.129397 flet_ivid-1.2/flet_ivid.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-05-22 16:53:49.000000 flet_ivid-1.2/flet_ivid.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-05-22 16:53:49.000000 flet_ivid-1.2/flet_ivid.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 16:53:49.000000 flet_ivid-1.2/flet_ivid.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-22 16:53:49.000000 flet_ivid-1.2/flet_ivid.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-22 16:53:49.000000 flet_ivid-1.2/flet_ivid.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-22 16:53:38.000000 flet_ivid-1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 16:53:49.129397 flet_ivid-1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      671 2023-05-22 16:53:38.000000 flet_ivid-1.2/setup.py
```

### Comparing `flet_ivid-1.1/LICENSE` & `flet_ivid-1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `flet_ivid-1.1/PKG-INFO` & `flet_ivid-1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flet_ivid
-Version: 1.1
+Version: 1.2
 Summary: A package tool that provide basic video player for flet.
 Home-page: https://github.com/SKbarbon/flet_ived
 Author: SKbarbon
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
```

### Comparing `flet_ivid-1.1/README.md` & `flet_ivid-1.2/README.md`

 * *Files identical despite different names*

### Comparing `flet_ivid-1.1/flet_ivid/video_container.py` & `flet_ivid-1.2/flet_ivid/video_container.py`

 * *Files 14% similar despite different names*

```diff
@@ -21,23 +21,22 @@
 from moviepy.editor import VideoFileClip
 import base64
 import time
 
 
 class VideoContainer (Container):
     """This will show a video you choose."""
-    def __init__(self, video_path:str, play_after_loading=False, video_frame_fit_type:flet.ImageFit=None, content= None, ref = None, key = None, width = None, height= None, left = None, top = None, right = None, bottom= None, expand= None, col = None, opacity= None, rotate= None, scale= None, offset= None, aspect_ratio= None, animate_opacity= None, animate_size = None, animate_position= None, animate_rotation= None, animate_scale= None, animate_offset = None, on_animation_end=None, tooltip = None, visible = None, disabled= None, data = None, padding= None, margin= None, alignment = None, bgcolor= None, gradient= None, blend_mode=BlendMode.NONE, border= None, border_radius= None, image_src= None, image_src_base64= None, image_repeat=None, image_fit=None, image_opacity: OptionalNumber = None, shape=None, clip_behavior= None, ink= None, animate=None, blur=None, shadow= None, url=None, url_target=None, theme=None, theme_mode= None, on_click=None, on_long_press=None, on_hover=None):
+    def __init__(self, video_path:str, play_after_loading=False, video_frame_fit_type:flet.ImageFit=None, video_progress_bar=True, content= None, ref = None, key = None, width = None, height= None, left = None, top = None, right = None, bottom= None, expand= None, col = None, opacity= None, rotate= None, scale= None, offset= None, aspect_ratio= None, animate_opacity= None, animate_size = None, animate_position= None, animate_rotation= None, animate_scale= None, animate_offset = None, on_animation_end=None, tooltip = None, visible = None, disabled= None, data = None, padding= None, margin= None, alignment = None, bgcolor= None, gradient= None, blend_mode=BlendMode.NONE, border= None, border_radius= None, image_src= None, image_src_base64= None, image_repeat=None, image_fit=None, image_opacity: OptionalNumber = None, shape=None, clip_behavior= None, ink= None, animate=None, blur=None, shadow= None, url=None, url_target=None, theme=None, theme_mode= None, on_click=None, on_long_press=None, on_hover=None):
         super().__init__(content, ref, key, width, height, left, top, right, bottom, expand, col, opacity, rotate, scale, offset, aspect_ratio, animate_opacity, animate_size, animate_position, animate_rotation, animate_scale, animate_offset, on_animation_end, tooltip, visible, disabled, data, padding, margin, alignment, bgcolor, gradient, blend_mode, border, border_radius, image_src, image_src_base64, image_repeat, image_fit, image_opacity, shape, clip_behavior, ink, animate, blur, shadow, url, url_target, theme, theme_mode, on_click, on_long_press, on_hover)
         if not os.path.isfile (video_path):
             raise FileNotFoundError ("Cannot find the video at the path you set.")
 
-        self.__video_is_full_loaded = False
         self.__all_frames_of_video = []
-        self.__audio_path = self.convert_video_to_audio (video_path=video_path)
         self.__video_played = False
+        self.video_progress_bar = video_progress_bar
 
         if video_frame_fit_type == None:
             self.video_frame_fit_type = flet.ImageFit.CONTAIN
 
         # generate the UI
         self.__ui ()
 
@@ -45,32 +44,55 @@
         if play_after_loading:
             print("Please wait the video is loading..\nThis will take a time based on your video size...")
             self.read_the_video(video_path)
         else:
             threading.Thread(target=self.read_the_video, args=[video_path], daemon=True).start()
 
         # setup the video audio
-        self.audio_path = self.convert_video_to_audio (video_path)
-        self.get_audio_info(self.audio_path)
+        try:
+            self.audio_path = self.convert_video_to_audio (video_path)
+            self.__audio_path = self.audio_path
+            self.get_audio_info(self.audio_path)
+        except:
+            self.audio_path = None
+            self.__audio_path = None
 
         # get video info
         self.get_video_duration(video_path)
         self.__frame_per_sleep = 1.0 / self.fps
     
     def __ui (self):
         # the video tools control
         self.video_tool_stack = Stack(expand=True)
         self.content = self.video_tool_stack
 
         self.image_frames_viewer = Image(expand=True, visible=False, fit=self.video_frame_fit_type)
         self.video_tool_stack.controls.append(Row([self.image_frames_viewer], alignment="center"))
+
+        self.__video_progress_bar = Container(height=2, width=100, bgcolor=flet.colors.BLUE_200)
+        self.video_tool_stack.controls.append(Row([self.__video_progress_bar], alignment=flet.MainAxisAlignment.START))
+
+        if self.video_progress_bar == False:
+            self.__video_progress_bar.visible = False
+    
+
+    def update_video_progress (self, frame_number):
+        if self.video_progress_bar == False: return
+        percent_of_progress = frame_number / self.video_frames * 1
+        
+        try:
+            self.__video_progress_bar.width = percent_of_progress * 1 * self.width
+        except:
+            self.__video_progress_bar.width = percent_of_progress * 1 * self.page.width
+        if self.__video_progress_bar.page != None: self.__video_progress_bar.update ()
     
 
     def update(self):
         self.image_frames_viewer.fit = self.video_frame_fit_type
+        self.__video_progress_bar.visible = self.video_progress_bar
         return super().update()
         
 
     def play (self, *args):
         """Play the video. (its not bloking, becuase its on thread)."""
         if self.page == None:
             raise Exception("The control must be on page first.")
@@ -78,38 +100,44 @@
         self.__video_played = True
         threading.Thread(target=self.__play, daemon=True).start()
         
     def __play (self):
         # -------
         self.image_frames_viewer.visible = True
         
-        # Initialize Pygame
-        pygame.mixer.init()
-        # Load the audio file
-        audio = pygame.mixer.Sound(self.__audio_path)
-        # Play the audio file
-        audio_state = audio.play()
+        if self.__audio_path != None:
+            # Initialize Pygame
+            pygame.mixer.init()
+            # Load the audio file
+            audio = pygame.mixer.Sound(self.__audio_path)
+            # Play the audio file
+            audio_state = audio.play()
         num = 0
         start_time = time.time()
 
         for I in self.__all_frames_of_video:
             if self.__video_played == False: break
+            # update video progress bar
+            threading.Thread (target=self.update_video_progress, args=[num], daemon=True).start()
+
             self.image_frames_viewer.src_base64 = I
             self.image_frames_viewer.update()
 
             elapsed_time = time.time() - start_time  # Calculate elapsed time
             # Calculate the desired time for the next frame update
             desired_time = (num + 1) * self.__frame_per_sleep
             
             # Calculate the remaining time to sleep
             sleep_time = max(0, desired_time - elapsed_time)
             time.sleep(sleep_time)
             # time.sleep(round(self.__frame_per_sleep, 3))
             num = num + 1
-        pygame.mixer.quit()
+        
+        if self.__audio_path != None:
+            pygame.mixer.quit()
 
         if len(self.__all_frames_of_video) != int(self.video_frames):
             print("WARNING: Your device cant stream all video data and load it at the same time!, please set 'VideoContainer(play_after_loading=True)' to fix this issue.")
     
 
     def pause (self, *args):
         self.__video_played = False
```

### Comparing `flet_ivid-1.1/flet_ivid.egg-info/PKG-INFO` & `flet_ivid-1.2/flet_ivid.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flet-ivid
-Version: 1.1
+Version: 1.2
 Summary: A package tool that provide basic video player for flet.
 Home-page: https://github.com/SKbarbon/flet_ived
 Author: SKbarbon
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
```

### Comparing `flet_ivid-1.1/setup.py` & `flet_ivid-1.2/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", encoding="utf-8") as f:
     long_des = str(f.read())
 
 setup(
     name='flet_ivid',
-    version='1.1',
+    version='1.2',
     author='SKbarbon',
     description='A package tool that provide basic video player for flet.',
     long_description=long_des,
     long_description_content_type='text/markdown',
     url='https://github.com/SKbarbon/flet_ived',
     install_requires=["flet", "pygame", "moviepy", "opencv-python"],
     packages=find_packages(),
```

