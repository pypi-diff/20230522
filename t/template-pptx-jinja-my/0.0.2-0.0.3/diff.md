# Comparing `tmp/template-pptx-jinja-my-0.0.2.tar.gz` & `tmp/template-pptx-jinja-my-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "template-pptx-jinja-my-0.0.2.tar", last modified: Thu May 18 09:08:27 2023, max compression
+gzip compressed data, was "template-pptx-jinja-my-0.0.3.tar", last modified: Mon May 22 02:05:12 2023, max compression
```

## Comparing `template-pptx-jinja-my-0.0.2.tar` & `template-pptx-jinja-my-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 wangguangyu   (501) staff       (20)        0 2023-05-18 09:08:27.411393 template-pptx-jinja-my-0.0.2/
--rw-r--r--   0 wangguangyu   (501) staff       (20)    35149 2023-05-18 06:21:21.000000 template-pptx-jinja-my-0.0.2/LICENSE
--rw-r--r--   0 wangguangyu   (501) staff       (20)     1042 2023-05-18 09:08:27.410899 template-pptx-jinja-my-0.0.2/PKG-INFO
--rw-r--r--   0 wangguangyu   (501) staff       (20)       38 2023-05-18 09:08:27.411482 template-pptx-jinja-my-0.0.2/setup.cfg
--rw-r--r--   0 wangguangyu   (501) staff       (20)      926 2023-05-18 09:08:15.000000 template-pptx-jinja-my-0.0.2/setup.py
-drwxr-xr-x   0 wangguangyu   (501) staff       (20)        0 2023-05-18 09:08:27.408225 template-pptx-jinja-my-0.0.2/template_pptx_jinja/
--rw-r--r--   0 wangguangyu   (501) staff       (20)        0 2023-05-18 06:21:21.000000 template-pptx-jinja-my-0.0.2/template_pptx_jinja/__init__.py
--rw-r--r--   0 wangguangyu   (501) staff       (20)      649 2023-05-18 07:18:43.000000 template-pptx-jinja-my-0.0.2/template_pptx_jinja/pictures.py
--rw-r--r--   0 wangguangyu   (501) staff       (20)     2714 2023-05-18 08:26:06.000000 template-pptx-jinja-my-0.0.2/template_pptx_jinja/render.py
-drwxr-xr-x   0 wangguangyu   (501) staff       (20)        0 2023-05-18 09:08:27.410257 template-pptx-jinja-my-0.0.2/template_pptx_jinja_my.egg-info/
--rw-r--r--   0 wangguangyu   (501) staff       (20)     1042 2023-05-18 09:08:27.000000 template-pptx-jinja-my-0.0.2/template_pptx_jinja_my.egg-info/PKG-INFO
--rw-r--r--   0 wangguangyu   (501) staff       (20)      339 2023-05-18 09:08:27.000000 template-pptx-jinja-my-0.0.2/template_pptx_jinja_my.egg-info/SOURCES.txt
--rw-r--r--   0 wangguangyu   (501) staff       (20)        1 2023-05-18 09:08:27.000000 template-pptx-jinja-my-0.0.2/template_pptx_jinja_my.egg-info/dependency_links.txt
--rw-r--r--   0 wangguangyu   (501) staff       (20)       34 2023-05-18 09:08:27.000000 template-pptx-jinja-my-0.0.2/template_pptx_jinja_my.egg-info/requires.txt
--rw-r--r--   0 wangguangyu   (501) staff       (20)       20 2023-05-18 09:08:27.000000 template-pptx-jinja-my-0.0.2/template_pptx_jinja_my.egg-info/top_level.txt
+drwxr-xr-x   0 wangguangyu   (501) staff       (20)        0 2023-05-22 02:05:12.899815 template-pptx-jinja-my-0.0.3/
+-rw-r--r--   0 wangguangyu   (501) staff       (20)    35149 2023-05-18 06:21:21.000000 template-pptx-jinja-my-0.0.3/LICENSE
+-rw-r--r--   0 wangguangyu   (501) staff       (20)     1042 2023-05-22 02:05:12.899540 template-pptx-jinja-my-0.0.3/PKG-INFO
+-rw-r--r--   0 wangguangyu   (501) staff       (20)       38 2023-05-22 02:05:12.899898 template-pptx-jinja-my-0.0.3/setup.cfg
+-rw-r--r--   0 wangguangyu   (501) staff       (20)      926 2023-05-22 02:04:55.000000 template-pptx-jinja-my-0.0.3/setup.py
+drwxr-xr-x   0 wangguangyu   (501) staff       (20)        0 2023-05-22 02:05:12.896121 template-pptx-jinja-my-0.0.3/template_pptx_jinja/
+-rw-r--r--   0 wangguangyu   (501) staff       (20)        0 2023-05-18 06:21:21.000000 template-pptx-jinja-my-0.0.3/template_pptx_jinja/__init__.py
+-rw-r--r--   0 wangguangyu   (501) staff       (20)      648 2023-05-22 02:04:12.000000 template-pptx-jinja-my-0.0.3/template_pptx_jinja/pictures.py
+-rw-r--r--   0 wangguangyu   (501) staff       (20)     2536 2023-05-22 02:04:12.000000 template-pptx-jinja-my-0.0.3/template_pptx_jinja/render.py
+drwxr-xr-x   0 wangguangyu   (501) staff       (20)        0 2023-05-22 02:05:12.899000 template-pptx-jinja-my-0.0.3/template_pptx_jinja_my.egg-info/
+-rw-r--r--   0 wangguangyu   (501) staff       (20)     1042 2023-05-22 02:05:12.000000 template-pptx-jinja-my-0.0.3/template_pptx_jinja_my.egg-info/PKG-INFO
+-rw-r--r--   0 wangguangyu   (501) staff       (20)      339 2023-05-22 02:05:12.000000 template-pptx-jinja-my-0.0.3/template_pptx_jinja_my.egg-info/SOURCES.txt
+-rw-r--r--   0 wangguangyu   (501) staff       (20)        1 2023-05-22 02:05:12.000000 template-pptx-jinja-my-0.0.3/template_pptx_jinja_my.egg-info/dependency_links.txt
+-rw-r--r--   0 wangguangyu   (501) staff       (20)       54 2023-05-22 02:05:12.000000 template-pptx-jinja-my-0.0.3/template_pptx_jinja_my.egg-info/requires.txt
+-rw-r--r--   0 wangguangyu   (501) staff       (20)       20 2023-05-22 02:05:12.000000 template-pptx-jinja-my-0.0.3/template_pptx_jinja_my.egg-info/top_level.txt
```

### Comparing `template-pptx-jinja-my-0.0.2/LICENSE` & `template-pptx-jinja-my-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `template-pptx-jinja-my-0.0.2/PKG-INFO` & `template-pptx-jinja-my-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: template-pptx-jinja-my
-Version: 0.0.2
+Version: 0.0.3
 Summary: PowerPoint presentation builder from template using Jinja2
 Home-page: https://github.com/macheal/template-pptx-jinja
 Author: macheal
 Author-email: xinyukc01@icloud.com
 Keywords: powerpoint,ppt,pptx,template
 Classifier: Development Status :: 4 - Beta
 Classifier: Topic :: Utilities
```

### Comparing `template-pptx-jinja-my-0.0.2/setup.py` & `template-pptx-jinja-my-0.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 def read(filename):
     with open(filename, 'r', encoding='utf-8') as myfile:
         return myfile.read()
 
 
 setup(name='template-pptx-jinja-my',
-    version="0.0.2",
+    version="0.0.3",
     description='PowerPoint presentation builder from template using Jinja2',
     long_description=read('readme.md'),
     long_description_content_type='text/markdown',
     url='https://github.com/macheal/template-pptx-jinja',
     author='macheal',
     author_email='xinyukc01@icloud.com',
     install_requires=read('requirements.txt').split(),
```

### Comparing `template-pptx-jinja-my-0.0.2/template_pptx_jinja/pictures.py` & `template-pptx-jinja-my-0.0.3/template_pptx_jinja/pictures.py`

 * *Files 20% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 # See https://github.com/scanny/python-pptx/issues/116
 def replace_img_slide(slide, img, img_path):
     # Replace the picture in the shape object (img) with the image in img_path.
 
     imgPic = img._pic
     imgRID = imgPic.xpath('./p:blipFill/a:blip/@r:embed')[0]
-    # imgPart = slide.part.related_parts[imgRID]
-    imgPart = slide.part.get_image(imgRID)
+    imgPart = slide.part.related_parts[imgRID]
+    #imgPart = slide.part.get_image(imgRID)
 
     with open(img_path, 'rb') as f:
         rImgBlob = f.read()
 
     # replace
     imgPart._blob = rImgBlob
```

### Comparing `template-pptx-jinja-my-0.0.2/template_pptx_jinja/render.py` & `template-pptx-jinja-my-0.0.3/template_pptx_jinja/render.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 from  jinja2 import exceptions, Environment
 
-
 from pptx import Presentation
 from pptx.enum.shapes import MSO_SHAPE_TYPE
-from pptx.parts.image import Image
-
 
 from template_pptx_jinja import pictures
+import templatepptx
 
 
 class PPTXRendering:
     def __init__(self, input_path, data, output_path, env=None):
         self.input_path = input_path
         self.model = data['model']
         if 'pictures' in data:
@@ -31,14 +29,17 @@
 
     def process(self):
         ppt = Presentation(self.input_path)
         for slide in ppt.slides:
             self.current_slide = slide
             self._render_slide(slide)
         ppt.save(self.output_path)
+        powerpoint = templatepptx.templatePptx(self.output_path, self.model, self.output_path, "$")
+        # Parses and exports the PowerPoint with filled out values and pictures
+        powerpoint.parse_template_pptx()
         return self.message
 
     def _render_slide(self, slide):
         for shape in slide.shapes:
             self.current_shape = shape
             self._render_shape(shape)
 
@@ -48,41 +49,31 @@
         if shape.has_table:
             self._render_table(shape.table)
         if shape.shape_type == MSO_SHAPE_TYPE.PICTURE:
             self._render_picture(shape)
 
     def _render_picture(self, shape):
         for picture in self.pictures:
-            if pictures.get_hash(picture) == shape.image.sha1:
+            if picture == shape.name:
                 pictures.replace_img_slide(
                     self.current_slide, shape, self.pictures[picture]
                 )
-
     def _render_text_frame(self, text_frame):
-        for paragraph in text_frame.paragraphs:
-            self._render_paragraph(paragraph)
-
-    def _render_paragraph(self, paragraph):
-        for run in paragraph.runs:
-            self._render_run(run)
-
-    def _render_table(self, table):
-        for cell in table.iter_cells():
-            self._render_cell(cell)
-
-    def _render_cell(self, cell):
-        # cell.text_frame.text  Size {% for row in sizeList %}
-        # Size 
-        # {% for row in sizeList %} ->_render_run()
-        self._render_text_frame(cell.text_frame)
-
-    def _render_run(self, run):
-        template = self.env.from_string(str(run.text))
+        template = self.env.from_string(str(text_frame.text))
         try:
             rendered = template.render(self.model)
         except exceptions.UndefinedError as error:
             self.message += str(error) + '\n'
         except exceptions.TemplateSyntaxError as error:
             self.message += str(error) + \
                 '\nyou should re-write the whole {{}} tag\n'
         else:
-            run.text = rendered
+            text_frame.text = rendered
+
+    def _render_table(self, table):
+        for cell in table.iter_cells():
+            self._render_cell(cell)
+
+    def _render_cell(self, cell):
+        self._render_text_frame(cell.text_frame)
+
+
```

### Comparing `template-pptx-jinja-my-0.0.2/template_pptx_jinja_my.egg-info/PKG-INFO` & `template-pptx-jinja-my-0.0.3/template_pptx_jinja_my.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: template-pptx-jinja-my
-Version: 0.0.2
+Version: 0.0.3
 Summary: PowerPoint presentation builder from template using Jinja2
 Home-page: https://github.com/macheal/template-pptx-jinja
 Author: macheal
 Author-email: xinyukc01@icloud.com
 Keywords: powerpoint,ppt,pptx,template
 Classifier: Development Status :: 4 - Beta
 Classifier: Topic :: Utilities
```

