# Comparing `tmp/textbsr-0.0.3.tar.gz` & `tmp/textbsr-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "textbsr-0.0.3.tar", last modified: Mon May 22 13:00:25 2023, max compression
+gzip compressed data, was "textbsr-0.0.4.tar", last modified: Mon May 22 13:29:36 2023, max compression
```

## Comparing `textbsr-0.0.3.tar` & `textbsr-0.0.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 xmli     (25167) xmli     (25167)        0 2023-05-22 13:00:25.000000 textbsr-0.0.3/
--rw-rw-r--   0 xmli     (25167) xmli     (25167)      399 2023-05-22 13:00:25.000000 textbsr-0.0.3/PKG-INFO
--rw-rw-r--   0 xmli     (25167) xmli     (25167)       38 2023-05-22 13:00:25.000000 textbsr-0.0.3/setup.cfg
--rw-rw-r--   0 xmli     (25167) xmli     (25167)     1169 2023-05-22 13:00:21.000000 textbsr-0.0.3/setup.py
-drwxrwxr-x   0 xmli     (25167) xmli     (25167)        0 2023-05-22 13:00:25.000000 textbsr-0.0.3/textbsr/
--rw-rw-r--   0 xmli     (25167) xmli     (25167)     5590 2023-05-22 12:57:45.000000 textbsr-0.0.3/textbsr/__init__.py
-drwxrwxr-x   0 xmli     (25167) xmli     (25167)        0 2023-05-22 13:00:25.000000 textbsr-0.0.3/textbsr/checkpoints/
--rw-rw-r--   0 xmli     (25167) xmli     (25167)        0 2023-05-22 08:21:11.000000 textbsr-0.0.3/textbsr/checkpoints/__init__.py
-drwxrwxr-x   0 xmli     (25167) xmli     (25167)        0 2023-05-22 13:00:25.000000 textbsr-0.0.3/textbsr/models/
--rw-rw-r--   0 xmli     (25167) xmli     (25167)     9135 2023-05-22 12:18:52.000000 textbsr-0.0.3/textbsr/models/TextEnhancement.py
--rw-rw-r--   0 xmli     (25167) xmli     (25167)        0 2023-05-22 08:21:14.000000 textbsr-0.0.3/textbsr/models/__init__.py
--rw-rw-r--   0 xmli     (25167) xmli     (25167)     6033 2023-05-22 12:54:43.000000 textbsr-0.0.3/textbsr/textbsr.py
-drwxrwxr-x   0 xmli     (25167) xmli     (25167)        0 2023-05-22 13:00:25.000000 textbsr-0.0.3/textbsr/utils/
--rw-rw-r--   0 xmli     (25167) xmli     (25167)        0 2023-05-22 08:21:19.000000 textbsr-0.0.3/textbsr/utils/__init__.py
--rw-rw-r--   0 xmli     (25167) xmli     (25167)     2677 2023-05-22 08:56:38.000000 textbsr-0.0.3/textbsr/utils/utils_image.py
-drwxrwxr-x   0 xmli     (25167) xmli     (25167)        0 2023-05-22 13:00:25.000000 textbsr-0.0.3/textbsr.egg-info/
--rw-rw-r--   0 xmli     (25167) xmli     (25167)      399 2023-05-22 13:00:25.000000 textbsr-0.0.3/textbsr.egg-info/PKG-INFO
--rw-rw-r--   0 xmli     (25167) xmli     (25167)      349 2023-05-22 13:00:25.000000 textbsr-0.0.3/textbsr.egg-info/SOURCES.txt
--rw-rw-r--   0 xmli     (25167) xmli     (25167)        1 2023-05-22 13:00:25.000000 textbsr-0.0.3/textbsr.egg-info/dependency_links.txt
--rw-rw-r--   0 xmli     (25167) xmli     (25167)       50 2023-05-22 13:00:25.000000 textbsr-0.0.3/textbsr.egg-info/requires.txt
--rw-rw-r--   0 xmli     (25167) xmli     (25167)        8 2023-05-22 13:00:25.000000 textbsr-0.0.3/textbsr.egg-info/top_level.txt
+drwxrwxr-x   0 xmli     (25167) xmli     (25167)        0 2023-05-22 13:29:36.000000 textbsr-0.0.4/
+-rw-rw-r--   0 xmli     (25167) xmli     (25167)      399 2023-05-22 13:29:36.000000 textbsr-0.0.4/PKG-INFO
+-rw-rw-r--   0 xmli     (25167) xmli     (25167)       38 2023-05-22 13:29:36.000000 textbsr-0.0.4/setup.cfg
+-rw-rw-r--   0 xmli     (25167) xmli     (25167)     1169 2023-05-22 13:29:20.000000 textbsr-0.0.4/setup.py
+drwxrwxr-x   0 xmli     (25167) xmli     (25167)        0 2023-05-22 13:29:35.000000 textbsr-0.0.4/textbsr/
+-rw-rw-r--   0 xmli     (25167) xmli     (25167)        0 2023-05-22 13:16:08.000000 textbsr-0.0.4/textbsr/__init__.py
+drwxrwxr-x   0 xmli     (25167) xmli     (25167)        0 2023-05-22 13:29:36.000000 textbsr-0.0.4/textbsr/checkpoints/
+-rw-rw-r--   0 xmli     (25167) xmli     (25167)        0 2023-05-22 08:21:11.000000 textbsr-0.0.4/textbsr/checkpoints/__init__.py
+drwxrwxr-x   0 xmli     (25167) xmli     (25167)        0 2023-05-22 13:29:36.000000 textbsr-0.0.4/textbsr/models/
+-rw-rw-r--   0 xmli     (25167) xmli     (25167)     9135 2023-05-22 12:18:52.000000 textbsr-0.0.4/textbsr/models/TextEnhancement.py
+-rw-rw-r--   0 xmli     (25167) xmli     (25167)        0 2023-05-22 08:21:14.000000 textbsr-0.0.4/textbsr/models/__init__.py
+-rw-rw-r--   0 xmli     (25167) xmli     (25167)     6241 2023-05-22 13:29:15.000000 textbsr-0.0.4/textbsr/textbsr.py
+drwxrwxr-x   0 xmli     (25167) xmli     (25167)        0 2023-05-22 13:29:36.000000 textbsr-0.0.4/textbsr/utils/
+-rw-rw-r--   0 xmli     (25167) xmli     (25167)        0 2023-05-22 08:21:19.000000 textbsr-0.0.4/textbsr/utils/__init__.py
+-rw-rw-r--   0 xmli     (25167) xmli     (25167)     2677 2023-05-22 08:56:38.000000 textbsr-0.0.4/textbsr/utils/utils_image.py
+drwxrwxr-x   0 xmli     (25167) xmli     (25167)        0 2023-05-22 13:29:35.000000 textbsr-0.0.4/textbsr.egg-info/
+-rw-rw-r--   0 xmli     (25167) xmli     (25167)      399 2023-05-22 13:29:34.000000 textbsr-0.0.4/textbsr.egg-info/PKG-INFO
+-rw-rw-r--   0 xmli     (25167) xmli     (25167)      349 2023-05-22 13:29:34.000000 textbsr-0.0.4/textbsr.egg-info/SOURCES.txt
+-rw-rw-r--   0 xmli     (25167) xmli     (25167)        1 2023-05-22 13:29:34.000000 textbsr-0.0.4/textbsr.egg-info/dependency_links.txt
+-rw-rw-r--   0 xmli     (25167) xmli     (25167)       50 2023-05-22 13:29:34.000000 textbsr-0.0.4/textbsr.egg-info/requires.txt
+-rw-rw-r--   0 xmli     (25167) xmli     (25167)        8 2023-05-22 13:29:34.000000 textbsr-0.0.4/textbsr.egg-info/top_level.txt
```

### Comparing `textbsr-0.0.3/setup.py` & `textbsr-0.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     here = os.path.dirname(os.path.realpath(__file__))
     with open(os.path.join(here, filename), 'r') as f:
         requires = [line.replace('\n', '') for line in f.readlines()]
     return requires
 
 
 setup(name='textbsr',
-      version='0.0.3',
+      version='0.0.4',
       description='a simple version for blind text image super-resolution (current version is only for English and Chinese)',
       author='Xiaoming Li',
       author_email='csxmli@gmail.com',
       #requires= ['numpy','torch','cv2','time','argparse','torchvision'], # 定义依赖哪些模块
       packages=find_packages(),  # 系统自动从当前目录开始找包
       # 如果有的文件不用打包，则只能指定需要打包的文件
       #packages=['代码1','代码2','__init__']  #指定目录中需要打包的py文件，注意不要.py后缀
```

### Comparing `textbsr-0.0.3/textbsr/__init__.py` & `textbsr-0.0.4/textbsr/textbsr.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+
 import torch
 from torch.hub import download_url_to_file, get_dir
 from utils import utils_image as util
 from models.TextEnhancement import TextRestoration as TextRestoration
 import cv2 
 import numpy as np
 import os.path
@@ -28,119 +29,121 @@
         filename = file_name
     cached_file = os.path.abspath(os.path.join(model_dir, filename))
     if not os.path.exists(cached_file):
         print(f'Downloading: "{url}" to {cached_file}\n')
         download_url_to_file(url, cached_file, hash_prefix=None, progress=progress)
     return cached_file
 
+def main(test_path, sr_path, save_path, is_aligned, save_text):
+    if save_path is None:
+        TIMESTAMP = time.strftime("%m-%d_%H-%M", time.localtime())
+        save_path = osp.join(args.test_path+'_'+TIMESTAMP+'_BSRGAN-Text')
+    os.makedirs(save_path, exist_ok=True)
 
-parser = argparse.ArgumentParser()
-parser.add_argument('-i', '--test_path', type=str, default='./testsets/LQ')
-parser.add_argument('-b', '--sr_path', type=str, default=None)
-parser.add_argument('-o', '--save_path', type=str, default=None)
-parser.add_argument('-a', '--aligned', action='store_true')
-parser.add_argument('-p', '--save_text', action='store_true')
-args = parser.parse_args()
-
-save_path = args.save_path
-test_path = args.test_path
-SaveText = args.save_text
-is_aligned = args.aligned
-sr_path = args.sr_path
-if save_path is None:
-    TIMESTAMP = time.strftime("%m-%d_%H-%M", time.localtime())
-    save_path = osp.join(args.test_path+'_'+TIMESTAMP+'_BSRGAN-Text')
-os.makedirs(save_path, exist_ok=True)
-
-
-lq_imgs = []
-sq_imgs = []
-lq_imgs = util.get_image_paths(test_path)
-if len(lq_imgs) ==0:
-    exit('No Image in the LR path.')
-if sr_path is not None:
-    sq_imgs = util.get_image_paths(sr_path)
-    if len(sq_imgs) != len(lq_imgs):
-        exit('The LQ path has {} images, while the SR path has {} ones. Please check whether the two paths are consistent.'.format(lr_num, sr_num))
-
-#print('#'*64)
-print('{:>25s} : {:s}'.format('Input Path', args.test_path))
-print('{:>25s} : {:s}'.format('Save Path', save_path))
-print('{:>25s} : {:s}'.format('Background SR Path', sr_path if sr_path else 'None'))
-if args.aligned:
-    print('{:>25s} : {:s}'.format('Image Details', 'Aligned Text Layout. No text detection is used.'))
-else:
-    print('{:>25s} : {:s}'.format('Image Details', 'UnAligned Text Image. It will crop text region using CnSTD, restore, and paste results back.'))
-print('{:>25s} : {:s}'.format('Save LR & SR text layout', 'True' if args.save_text else 'False'))
-
-
-
-scale_factor = 4 # upsample scale factor for the final output, fixed
-
-t = time.strftime("%m-%d_%H-%M", time.localtime()) 
-
-use_cuda = torch.cuda.is_available()
-device = torch.device('cuda' if use_cuda else 'cpu')
-weight_path = load_file_from_url(pretrain_model_url['x4'])
-TextModel = TextRestoration(ModelName='RRDB', TextModelPath=weight_path, device=device)
-
-print('{:>25s} : {:s}'.format('Model Name', 'BSRGAN'))
-if use_cuda:
-    print('{:>25s} : {:<d}'.format('GPU ID', torch.cuda.current_device()))
-else:
-    print('{:>25s} : {:s}'.format('GPU ID', 'No GPU is available. Use CPU instead.'))
-torch.cuda.empty_cache()
-
-#print('################################## Handling {:s} ##################################'.format(test_path))
-L_path = test_path
-E_path = save_path # save path
-print('{:>25s} : {:s}'.format('Input Path', L_path))
-print('{:>25s} : {:s}'.format('Output Path', E_path))
-idx = 0
-
-
-for img in lq_imgs:
-    ####################################
-    #####(1) Read Image
-    ####################################
-    idx += 1
-    img_name, ext = os.path.splitext(os.path.basename(img))
-    print('{:>20s} {:04d} : x{:<d} --> {:<s}'.format('Restoring ', idx, scale_factor, img_name+ext))
-
-    img_L = util.imread_uint(img, n_channels=3) #RGB 0~255
-    width_L = img_L.shape[1]
-    height_L = img_L.shape[0]
-
-    width_S, height_S = 0, 0
     
+    lq_imgs = []
+    sq_imgs = []
+    lq_imgs = util.get_image_paths(test_path)
+    if len(lq_imgs) ==0:
+        exit('No Image in the LR path.')
+    if sr_path is not None:
+        sq_imgs = util.get_image_paths(sr_path)
+        if len(sq_imgs) != len(lq_imgs):
+            exit('The LQ path has {} images, while the SR path has {} ones. Please check whether the two paths are consistent.'.format(lr_num, sr_num))
+
+    #print('#'*64)
+    print('{:>25s} : {:s}'.format('Input Path', args.test_path))
+    print('{:>25s} : {:s}'.format('Save Path', save_path))
+    print('{:>25s} : {:s}'.format('Background SR Path', sr_path if sr_path else 'None'))
+    if args.aligned:
+        print('{:>25s} : {:s}'.format('Image Details', 'Aligned Text Layout. No text detection is used.'))
+    else:
+        print('{:>25s} : {:s}'.format('Image Details', 'UnAligned Text Image. It will crop text region using CnSTD, restore, and paste results back.'))
+    print('{:>25s} : {:s}'.format('Save LR & SR text layout', 'True' if args.save_text else 'False'))
 
-    if len(sq_imgs) > 0:
-        sq_img = sq_imgs[idx-1]
-        img_E = util.imread_uint(sq_img, n_channels=3)
-        width_S = img_E.shape[1]
-        height_S = img_E.shape[0]
 
-    else:
-        img_E = img_L
-    img_E = cv2.resize(img_E, (width_L*scale_factor, height_L*scale_factor), interpolation = cv2.INTER_AREA)
-    
+
+
+
+
+
+    scale_factor = 4 # upsample scale factor for the final output, fixed
     
-    ####################################
-    #####(2) Restore Each Region and Paste to the whole image
-    ####################################
-    SQ, ori_texts, en_texts  = TextModel.handle_texts(img=img_L, bg=img_E, sf=scale_factor, is_aligned=is_aligned)
-    if not is_aligned:
-        if width_S == 0 or height_S == 0:
-            width_S = (width_L * scale_factor)
-            height_S = (height_L * scale_factor)
-        SQ = cv2.resize(SQ.astype(np.float32), (width_S, height_S), interpolation=cv2.INTER_AREA)
-        cv2.imwrite(os.path.join(E_path, img_name +'_BSRGANText.png'), SQ[:,:,::-1])
+    t = time.strftime("%m-%d_%H-%M", time.localtime()) 
+
+    use_cuda = torch.cuda.is_available()
+    device = torch.device('cuda' if use_cuda else 'cpu')
+    weight_path = load_file_from_url(pretrain_model_url['x4'])
+    TextModel = TextRestoration(ModelName='RRDB', TextModelPath=weight_path, device=device)
+
+    print('{:>25s} : {:s}'.format('Model Name', 'BSRGAN'))
+    if use_cuda:
+        print('{:>25s} : {:<d}'.format('GPU ID', torch.cuda.current_device()))
     else:
-        cv2.imwrite(os.path.join(E_path, img_name +'_BSRGANText.png'), en_texts[0])
-    ####################################
-    #####(3) Save Cropped Results
-    ####################################
-    if SaveText and not is_aligned:
-        for m, (et, ot) in enumerate(zip(en_texts, ori_texts)): ##save each face region
-            w, h, c = et.shape
-            ot = cv2.resize(ot, (h, w))
-            cv2.imwrite(os.path.join(E_path, img_name +'_patch_{}.png'.format(m)), np.hstack((ot, et)))
+        print('{:>25s} : {:s}'.format('GPU ID', 'No GPU is available. Use CPU instead.'))
+    torch.cuda.empty_cache()
+
+    #print('################################## Handling {:s} ##################################'.format(test_path))
+    L_path = test_path
+    E_path = save_path # save path
+    print('{:>25s} : {:s}'.format('Input Path', L_path))
+    print('{:>25s} : {:s}'.format('Output Path', E_path))
+    idx = 0
+
+    
+    for img in lq_imgs:
+        ####################################
+        #####(1) Read Image
+        ####################################
+        idx += 1
+        img_name, ext = os.path.splitext(os.path.basename(img))
+        print('{:>20s} {:04d} : x{:<d} --> {:<s}'.format('Restoring ', idx, scale_factor, img_name+ext))
+
+        img_L = util.imread_uint(img, n_channels=3) #RGB 0~255
+        width_L = img_L.shape[1]
+        height_L = img_L.shape[0]
+
+        width_S, height_S = 0, 0
+        
+
+        if len(sq_imgs) > 0:
+            sq_img = sq_imgs[idx-1]
+            img_E = util.imread_uint(sq_img, n_channels=3)
+            width_S = img_E.shape[1]
+            height_S = img_E.shape[0]
+
+        else:
+            img_E = img_L
+        img_E = cv2.resize(img_E, (width_L*scale_factor, height_L*scale_factor), interpolation = cv2.INTER_AREA)
+        
+        
+        ####################################
+        #####(2) Restore Each Region and Paste to the whole image
+        ####################################
+        SQ, ori_texts, en_texts  = TextModel.handle_texts(img=img_L, bg=img_E, sf=scale_factor, is_aligned=is_aligned)
+        if not is_aligned:
+            if width_S == 0 or height_S == 0:
+                width_S = (width_L * scale_factor)
+                height_S = (height_L * scale_factor)
+            SQ = cv2.resize(SQ.astype(np.float32), (width_S, height_S), interpolation=cv2.INTER_AREA)
+            cv2.imwrite(os.path.join(E_path, img_name +'_BSRGANText.png'), SQ[:,:,::-1])
+        else:
+            cv2.imwrite(os.path.join(E_path, img_name +'_BSRGANText.png'), en_texts[0])
+        ####################################
+        #####(3) Save Cropped Results
+        ####################################
+        if save_text and not is_aligned:
+            for m, (et, ot) in enumerate(zip(en_texts, ori_texts)): ##save each face region
+                w, h, c = et.shape
+                ot = cv2.resize(ot, (h, w))
+                cv2.imwrite(os.path.join(E_path, img_name +'_patch_{}.png'.format(m)), np.hstack((ot, et)))
+
+if __name__ == '__main__':
+    parser = argparse.ArgumentParser()
+    parser.add_argument('-i', '--test_path', type=str, default='./testsets/LQ', help='the lr image path')
+    parser.add_argument('-b', '--sr_path', type=str, default=None, help='the background sr path, default:None')
+    parser.add_argument('-o', '--save_path', type=str, default=None, help='the text sr save path')
+    parser.add_argument('-a', '--aligned', action='store_true', help='whether the input contains only text region, default:False')
+    parser.add_argument('-p', '--save_text', action='store_true', help='whether save the LR and SR text layout, default:False')
+    args = parser.parse_args()
+
+    main(args.test_path, args.sr_path, args.save_path, args.aligned, args.save_text)
```

### Comparing `textbsr-0.0.3/textbsr/models/TextEnhancement.py` & `textbsr-0.0.4/textbsr/models/TextEnhancement.py`

 * *Files identical despite different names*

### Comparing `textbsr-0.0.3/textbsr/utils/utils_image.py` & `textbsr-0.0.4/textbsr/utils/utils_image.py`

 * *Files identical despite different names*

