# Comparing `tmp/textbsr-0.0.4.tar.gz` & `tmp/textbsr-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "textbsr-0.0.4.tar", last modified: Mon May 22 13:29:36 2023, max compression
+gzip compressed data, was "textbsr-0.0.6.tar", last modified: Mon May 22 13:33:57 2023, max compression
```

## Comparing `textbsr-0.0.4.tar` & `textbsr-0.0.6.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 xmli     (25167) xmli     (25167)        0 2023-05-22 13:29:36.000000 textbsr-0.0.4/
--rw-rw-r--   0 xmli     (25167) xmli     (25167)      399 2023-05-22 13:29:36.000000 textbsr-0.0.4/PKG-INFO
--rw-rw-r--   0 xmli     (25167) xmli     (25167)       38 2023-05-22 13:29:36.000000 textbsr-0.0.4/setup.cfg
--rw-rw-r--   0 xmli     (25167) xmli     (25167)     1169 2023-05-22 13:29:20.000000 textbsr-0.0.4/setup.py
-drwxrwxr-x   0 xmli     (25167) xmli     (25167)        0 2023-05-22 13:29:35.000000 textbsr-0.0.4/textbsr/
--rw-rw-r--   0 xmli     (25167) xmli     (25167)        0 2023-05-22 13:16:08.000000 textbsr-0.0.4/textbsr/__init__.py
-drwxrwxr-x   0 xmli     (25167) xmli     (25167)        0 2023-05-22 13:29:36.000000 textbsr-0.0.4/textbsr/checkpoints/
--rw-rw-r--   0 xmli     (25167) xmli     (25167)        0 2023-05-22 08:21:11.000000 textbsr-0.0.4/textbsr/checkpoints/__init__.py
-drwxrwxr-x   0 xmli     (25167) xmli     (25167)        0 2023-05-22 13:29:36.000000 textbsr-0.0.4/textbsr/models/
--rw-rw-r--   0 xmli     (25167) xmli     (25167)     9135 2023-05-22 12:18:52.000000 textbsr-0.0.4/textbsr/models/TextEnhancement.py
--rw-rw-r--   0 xmli     (25167) xmli     (25167)        0 2023-05-22 08:21:14.000000 textbsr-0.0.4/textbsr/models/__init__.py
--rw-rw-r--   0 xmli     (25167) xmli     (25167)     6241 2023-05-22 13:29:15.000000 textbsr-0.0.4/textbsr/textbsr.py
-drwxrwxr-x   0 xmli     (25167) xmli     (25167)        0 2023-05-22 13:29:36.000000 textbsr-0.0.4/textbsr/utils/
--rw-rw-r--   0 xmli     (25167) xmli     (25167)        0 2023-05-22 08:21:19.000000 textbsr-0.0.4/textbsr/utils/__init__.py
--rw-rw-r--   0 xmli     (25167) xmli     (25167)     2677 2023-05-22 08:56:38.000000 textbsr-0.0.4/textbsr/utils/utils_image.py
-drwxrwxr-x   0 xmli     (25167) xmli     (25167)        0 2023-05-22 13:29:35.000000 textbsr-0.0.4/textbsr.egg-info/
--rw-rw-r--   0 xmli     (25167) xmli     (25167)      399 2023-05-22 13:29:34.000000 textbsr-0.0.4/textbsr.egg-info/PKG-INFO
--rw-rw-r--   0 xmli     (25167) xmli     (25167)      349 2023-05-22 13:29:34.000000 textbsr-0.0.4/textbsr.egg-info/SOURCES.txt
--rw-rw-r--   0 xmli     (25167) xmli     (25167)        1 2023-05-22 13:29:34.000000 textbsr-0.0.4/textbsr.egg-info/dependency_links.txt
--rw-rw-r--   0 xmli     (25167) xmli     (25167)       50 2023-05-22 13:29:34.000000 textbsr-0.0.4/textbsr.egg-info/requires.txt
--rw-rw-r--   0 xmli     (25167) xmli     (25167)        8 2023-05-22 13:29:34.000000 textbsr-0.0.4/textbsr.egg-info/top_level.txt
+drwxrwxr-x   0 xmli     (25167) xmli     (25167)        0 2023-05-22 13:33:57.000000 textbsr-0.0.6/
+-rw-rw-r--   0 xmli     (25167) xmli     (25167)      399 2023-05-22 13:33:57.000000 textbsr-0.0.6/PKG-INFO
+-rw-rw-r--   0 xmli     (25167) xmli     (25167)       38 2023-05-22 13:33:57.000000 textbsr-0.0.6/setup.cfg
+-rw-rw-r--   0 xmli     (25167) xmli     (25167)     1169 2023-05-22 13:33:51.000000 textbsr-0.0.6/setup.py
+drwxrwxr-x   0 xmli     (25167) xmli     (25167)        0 2023-05-22 13:33:57.000000 textbsr-0.0.6/textbsr/
+-rw-rw-r--   0 xmli     (25167) xmli     (25167)        0 2023-05-22 13:16:08.000000 textbsr-0.0.6/textbsr/__init__.py
+drwxrwxr-x   0 xmli     (25167) xmli     (25167)        0 2023-05-22 13:33:57.000000 textbsr-0.0.6/textbsr/checkpoints/
+-rw-rw-r--   0 xmli     (25167) xmli     (25167)        0 2023-05-22 08:21:11.000000 textbsr-0.0.6/textbsr/checkpoints/__init__.py
+drwxrwxr-x   0 xmli     (25167) xmli     (25167)        0 2023-05-22 13:33:57.000000 textbsr-0.0.6/textbsr/models/
+-rw-rw-r--   0 xmli     (25167) xmli     (25167)     9135 2023-05-22 12:18:52.000000 textbsr-0.0.6/textbsr/models/TextEnhancement.py
+-rw-rw-r--   0 xmli     (25167) xmli     (25167)        0 2023-05-22 08:21:14.000000 textbsr-0.0.6/textbsr/models/__init__.py
+-rw-rw-r--   0 xmli     (25167) xmli     (25167)     6246 2023-05-22 13:33:41.000000 textbsr-0.0.6/textbsr/textbsr.py
+drwxrwxr-x   0 xmli     (25167) xmli     (25167)        0 2023-05-22 13:33:57.000000 textbsr-0.0.6/textbsr/utils/
+-rw-rw-r--   0 xmli     (25167) xmli     (25167)        0 2023-05-22 08:21:19.000000 textbsr-0.0.6/textbsr/utils/__init__.py
+-rw-rw-r--   0 xmli     (25167) xmli     (25167)     2677 2023-05-22 08:56:38.000000 textbsr-0.0.6/textbsr/utils/utils_image.py
+drwxrwxr-x   0 xmli     (25167) xmli     (25167)        0 2023-05-22 13:33:57.000000 textbsr-0.0.6/textbsr.egg-info/
+-rw-rw-r--   0 xmli     (25167) xmli     (25167)      399 2023-05-22 13:33:57.000000 textbsr-0.0.6/textbsr.egg-info/PKG-INFO
+-rw-rw-r--   0 xmli     (25167) xmli     (25167)      349 2023-05-22 13:33:57.000000 textbsr-0.0.6/textbsr.egg-info/SOURCES.txt
+-rw-rw-r--   0 xmli     (25167) xmli     (25167)        1 2023-05-22 13:33:57.000000 textbsr-0.0.6/textbsr.egg-info/dependency_links.txt
+-rw-rw-r--   0 xmli     (25167) xmli     (25167)       50 2023-05-22 13:33:57.000000 textbsr-0.0.6/textbsr.egg-info/requires.txt
+-rw-rw-r--   0 xmli     (25167) xmli     (25167)        8 2023-05-22 13:33:57.000000 textbsr-0.0.6/textbsr.egg-info/top_level.txt
```

### Comparing `textbsr-0.0.4/setup.py` & `textbsr-0.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     here = os.path.dirname(os.path.realpath(__file__))
     with open(os.path.join(here, filename), 'r') as f:
         requires = [line.replace('\n', '') for line in f.readlines()]
     return requires
 
 
 setup(name='textbsr',
-      version='0.0.4',
+      version='0.0.6',
       description='a simple version for blind text image super-resolution (current version is only for English and Chinese)',
       author='Xiaoming Li',
       author_email='csxmli@gmail.com',
       #requires= ['numpy','torch','cv2','time','argparse','torchvision'], # 定义依赖哪些模块
       packages=find_packages(),  # 系统自动从当前目录开始找包
       # 如果有的文件不用打包，则只能指定需要打包的文件
       #packages=['代码1','代码2','__init__']  #指定目录中需要打包的py文件，注意不要.py后缀
```

### Comparing `textbsr-0.0.4/textbsr/models/TextEnhancement.py` & `textbsr-0.0.6/textbsr/models/TextEnhancement.py`

 * *Files identical despite different names*

### Comparing `textbsr-0.0.4/textbsr/textbsr.py` & `textbsr-0.0.6/textbsr/textbsr.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,40 +29,40 @@
         filename = file_name
     cached_file = os.path.abspath(os.path.join(model_dir, filename))
     if not os.path.exists(cached_file):
         print(f'Downloading: "{url}" to {cached_file}\n')
         download_url_to_file(url, cached_file, hash_prefix=None, progress=progress)
     return cached_file
 
-def main(test_path, sr_path, save_path, is_aligned, save_text):
+def main(test_path, sr_path=None, save_path=None, is_aligned=False, save_text=False):
     if save_path is None:
         TIMESTAMP = time.strftime("%m-%d_%H-%M", time.localtime())
-        save_path = osp.join(args.test_path+'_'+TIMESTAMP+'_BSRGAN-Text')
+        save_path = osp.join(test_path+'_'+TIMESTAMP+'_BSRGAN-Text')
     os.makedirs(save_path, exist_ok=True)
 
     
     lq_imgs = []
     sq_imgs = []
     lq_imgs = util.get_image_paths(test_path)
     if len(lq_imgs) ==0:
         exit('No Image in the LR path.')
     if sr_path is not None:
         sq_imgs = util.get_image_paths(sr_path)
         if len(sq_imgs) != len(lq_imgs):
             exit('The LQ path has {} images, while the SR path has {} ones. Please check whether the two paths are consistent.'.format(lr_num, sr_num))
 
     #print('#'*64)
-    print('{:>25s} : {:s}'.format('Input Path', args.test_path))
+    print('{:>25s} : {:s}'.format('Input Path', test_path))
     print('{:>25s} : {:s}'.format('Save Path', save_path))
     print('{:>25s} : {:s}'.format('Background SR Path', sr_path if sr_path else 'None'))
-    if args.aligned:
+    if is_aligned:
         print('{:>25s} : {:s}'.format('Image Details', 'Aligned Text Layout. No text detection is used.'))
     else:
         print('{:>25s} : {:s}'.format('Image Details', 'UnAligned Text Image. It will crop text region using CnSTD, restore, and paste results back.'))
-    print('{:>25s} : {:s}'.format('Save LR & SR text layout', 'True' if args.save_text else 'False'))
+    print('{:>25s} : {:s}'.format('Save LR & SR text layout', 'True' if save_text else 'False'))
```

### Comparing `textbsr-0.0.4/textbsr/utils/utils_image.py` & `textbsr-0.0.6/textbsr/utils/utils_image.py`

 * *Files identical despite different names*

