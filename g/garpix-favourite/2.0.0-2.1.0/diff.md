# Comparing `tmp/garpix_favourite-2.0.0.tar.gz` & `tmp/garpix_favourite-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "garpix_favourite-2.0.0.tar", last modified: Wed May 10 16:12:26 2023, max compression
+gzip compressed data, was "garpix_favourite-2.1.0.tar", last modified: Mon May 22 08:13:51 2023, max compression
```

## Comparing `garpix_favourite-2.0.0.tar` & `garpix_favourite-2.1.0.tar`

### file list

```diff
@@ -1,35 +1,41 @@
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-10 16:12:26.662539 garpix_favourite-2.0.0/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)       36 2023-05-10 16:12:26.000000 garpix_favourite-2.0.0/MANIFEST.in
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1814 2023-05-10 16:12:26.662370 garpix_favourite-2.0.0/PKG-INFO
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-10 16:12:26.653899 garpix_favourite-2.0.0/garpix_favourite/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      181 2023-05-10 16:11:01.000000 garpix_favourite-2.0.0/garpix_favourite/CHANGELOG.md
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1020 2023-05-10 16:11:01.000000 garpix_favourite-2.0.0/garpix_favourite/CONTRIBUTING.md
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)       36 2022-11-08 08:54:41.000000 garpix_favourite-2.0.0/garpix_favourite/MANIFEST.in
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1241 2023-05-10 16:11:01.000000 garpix_favourite-2.0.0/garpix_favourite/README.md
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)       67 2022-11-08 08:54:41.000000 garpix_favourite-2.0.0/garpix_favourite/__init__.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-10 16:12:26.662154 garpix_favourite-2.0.0/garpix_favourite/__pycache__/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      241 2022-11-14 21:15:49.000000 garpix_favourite-2.0.0/garpix_favourite/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      451 2022-11-14 21:15:49.000000 garpix_favourite-2.0.0/garpix_favourite/__pycache__/apps.cpython-38.pyc
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1672 2023-05-10 16:11:24.000000 garpix_favourite-2.0.0/garpix_favourite/__pycache__/models.cpython-38.pyc
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      361 2022-11-14 21:16:38.000000 garpix_favourite-2.0.0/garpix_favourite/__pycache__/routers.cpython-38.pyc
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     3556 2023-05-10 16:11:26.000000 garpix_favourite-2.0.0/garpix_favourite/__pycache__/serializers.cpython-38.pyc
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      411 2023-05-10 16:11:26.000000 garpix_favourite-2.0.0/garpix_favourite/__pycache__/urls.cpython-38.pyc
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1940 2023-05-10 16:11:26.000000 garpix_favourite-2.0.0/garpix_favourite/__pycache__/views.cpython-38.pyc
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      143 2022-11-08 08:54:41.000000 garpix_favourite-2.0.0/garpix_favourite/apps.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1327 2023-05-10 16:11:01.000000 garpix_favourite-2.0.0/garpix_favourite/models.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      180 2022-11-08 08:54:41.000000 garpix_favourite-2.0.0/garpix_favourite/routers.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     3405 2023-05-10 16:11:01.000000 garpix_favourite-2.0.0/garpix_favourite/serializers.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1095 2023-05-10 16:12:24.000000 garpix_favourite-2.0.0/garpix_favourite/setup.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     2299 2022-11-08 08:54:41.000000 garpix_favourite-2.0.0/garpix_favourite/tests.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      289 2023-05-10 16:11:01.000000 garpix_favourite-2.0.0/garpix_favourite/urls.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      848 2022-11-08 08:54:41.000000 garpix_favourite-2.0.0/garpix_favourite/utils.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1574 2023-05-10 16:11:01.000000 garpix_favourite-2.0.0/garpix_favourite/views.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-10 16:12:26.660895 garpix_favourite-2.0.0/garpix_favourite.egg-info/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1814 2023-05-10 16:12:26.000000 garpix_favourite-2.0.0/garpix_favourite.egg-info/PKG-INFO
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1007 2023-05-10 16:12:26.000000 garpix_favourite-2.0.0/garpix_favourite.egg-info/SOURCES.txt
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)        1 2023-05-10 16:12:26.000000 garpix_favourite-2.0.0/garpix_favourite.egg-info/dependency_links.txt
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)        1 2023-05-10 16:12:26.000000 garpix_favourite-2.0.0/garpix_favourite.egg-info/not-zip-safe
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)       17 2023-05-10 16:12:26.000000 garpix_favourite-2.0.0/garpix_favourite.egg-info/requires.txt
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)       17 2023-05-10 16:12:26.000000 garpix_favourite-2.0.0/garpix_favourite.egg-info/top_level.txt
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)       38 2023-05-10 16:12:26.662581 garpix_favourite-2.0.0/setup.cfg
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1095 2023-05-10 16:12:26.000000 garpix_favourite-2.0.0/setup.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-22 08:13:51.186458 garpix_favourite-2.1.0/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)       36 2023-05-22 08:13:51.000000 garpix_favourite-2.1.0/MANIFEST.in
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1814 2023-05-22 08:13:51.186318 garpix_favourite-2.1.0/PKG-INFO
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-22 08:13:51.184070 garpix_favourite-2.1.0/garpix_favourite/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      464 2023-05-22 08:13:34.000000 garpix_favourite-2.1.0/garpix_favourite/CHANGELOG.md
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1020 2023-05-10 16:11:01.000000 garpix_favourite-2.1.0/garpix_favourite/CONTRIBUTING.md
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)       36 2022-11-08 08:54:41.000000 garpix_favourite-2.1.0/garpix_favourite/MANIFEST.in
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1241 2023-05-10 16:11:01.000000 garpix_favourite-2.1.0/garpix_favourite/README.md
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)       67 2022-11-08 08:54:41.000000 garpix_favourite-2.1.0/garpix_favourite/__init__.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-22 08:13:51.185698 garpix_favourite-2.1.0/garpix_favourite/__pycache__/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      241 2022-11-14 21:15:49.000000 garpix_favourite-2.1.0/garpix_favourite/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      451 2022-11-14 21:15:49.000000 garpix_favourite-2.1.0/garpix_favourite/__pycache__/apps.cpython-38.pyc
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     2527 2023-05-22 08:13:50.000000 garpix_favourite-2.1.0/garpix_favourite/__pycache__/models.cpython-38.pyc
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      361 2022-11-14 21:16:38.000000 garpix_favourite-2.1.0/garpix_favourite/__pycache__/routers.cpython-38.pyc
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     3600 2023-05-22 08:13:51.000000 garpix_favourite-2.1.0/garpix_favourite/__pycache__/serializers.cpython-38.pyc
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      411 2023-05-10 16:11:26.000000 garpix_favourite-2.1.0/garpix_favourite/__pycache__/urls.cpython-38.pyc
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1864 2023-05-22 08:13:51.000000 garpix_favourite-2.1.0/garpix_favourite/__pycache__/views.cpython-38.pyc
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-22 08:13:51.185915 garpix_favourite-2.1.0/garpix_favourite/admin/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)       35 2023-05-22 08:11:02.000000 garpix_favourite-2.1.0/garpix_favourite/admin/__init__.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-22 08:13:51.186159 garpix_favourite-2.1.0/garpix_favourite/admin/__pycache__/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      226 2023-05-22 08:13:50.000000 garpix_favourite-2.1.0/garpix_favourite/admin/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      466 2023-05-22 08:13:50.000000 garpix_favourite-2.1.0/garpix_favourite/admin/__pycache__/favorite.cpython-38.pyc
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      138 2023-05-22 08:11:02.000000 garpix_favourite-2.1.0/garpix_favourite/admin/favorite.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      143 2022-11-08 08:54:41.000000 garpix_favourite-2.1.0/garpix_favourite/apps.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     2155 2023-05-22 08:11:02.000000 garpix_favourite-2.1.0/garpix_favourite/models.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      180 2022-11-08 08:54:41.000000 garpix_favourite-2.1.0/garpix_favourite/routers.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     3463 2023-05-22 08:11:02.000000 garpix_favourite-2.1.0/garpix_favourite/serializers.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1095 2023-05-22 08:11:25.000000 garpix_favourite-2.1.0/garpix_favourite/setup.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     2312 2023-05-22 08:11:02.000000 garpix_favourite-2.1.0/garpix_favourite/tests.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      289 2023-05-10 16:11:01.000000 garpix_favourite-2.1.0/garpix_favourite/urls.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      848 2022-11-08 08:54:41.000000 garpix_favourite-2.1.0/garpix_favourite/utils.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1499 2023-05-22 08:11:02.000000 garpix_favourite-2.1.0/garpix_favourite/views.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-22 08:13:51.184890 garpix_favourite-2.1.0/garpix_favourite.egg-info/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1814 2023-05-22 08:13:51.000000 garpix_favourite-2.1.0/garpix_favourite.egg-info/PKG-INFO
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1195 2023-05-22 08:13:51.000000 garpix_favourite-2.1.0/garpix_favourite.egg-info/SOURCES.txt
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)        1 2023-05-22 08:13:51.000000 garpix_favourite-2.1.0/garpix_favourite.egg-info/dependency_links.txt
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)        1 2023-05-22 08:13:51.000000 garpix_favourite-2.1.0/garpix_favourite.egg-info/not-zip-safe
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)       17 2023-05-22 08:13:51.000000 garpix_favourite-2.1.0/garpix_favourite.egg-info/requires.txt
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)       17 2023-05-22 08:13:51.000000 garpix_favourite-2.1.0/garpix_favourite.egg-info/top_level.txt
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)       38 2023-05-22 08:13:51.186502 garpix_favourite-2.1.0/setup.cfg
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1095 2023-05-22 08:13:51.000000 garpix_favourite-2.1.0/setup.py
```

### Comparing `garpix_favourite-2.0.0/PKG-INFO` & `garpix_favourite-2.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: garpix_favourite
-Version: 2.0.0
+Version: 2.1.0
 Home-page: https://github.com/garpixcms/garpix_favourite
 Author: Garpix LTD
 Author-email: info@garpix.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
```

### Comparing `garpix_favourite-2.0.0/garpix_favourite/CONTRIBUTING.md` & `garpix_favourite-2.1.0/garpix_favourite/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `garpix_favourite-2.0.0/garpix_favourite/README.md` & `garpix_favourite-2.1.0/garpix_favourite/README.md`

 * *Files identical despite different names*

### Comparing `garpix_favourite-2.0.0/garpix_favourite/__pycache__/serializers.cpython-38.pyc` & `garpix_favourite-2.1.0/garpix_favourite/__pycache__/serializers.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Wed May 10 16:11:01 2023 UTC, .py size: 3405 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 15c2 5b64 4d0d 0000  U.........[dM...
+00000000: 550d 0d0a 0000 0000 9623 6b64 870d 0000  U........#kd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0008 0000 0040 0000 0073 c600 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 0100 6400 6403 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
 00000050: 0100 6400 6404 6c06 6d07 5a07 0100 6400  ..d.d.l.m.Z...d.
 00000060: 6405 6c08 6d09 5a0a 0100 6400 6406 6c0b  d.l.m.Z...d.d.l.
 00000070: 6d0c 5a0c 0100 6400 6407 6c0d 6d0e 5a0e  m.Z...d.d.l.m.Z.
@@ -39,185 +39,187 @@
 00000260: 6974 652f 6261 636b 656e 642f 6761 7270  ite/backend/garp
 00000270: 6978 5f66 6176 6f75 7269 7465 2f73 6572  ix_favourite/ser
 00000280: 6961 6c69 7a65 7273 2e70 79da 1f5f 6765  ializers.py.._ge
 00000290: 745f 636f 6e74 656e 745f 7479 7065 5f62  t_content_type_b
 000002a0: 795f 6d6f 6465 6c5f 6e61 6d65 1900 0000  y_model_name....
 000002b0: 7304 0000 0000 0108 0272 1400 0000 6300  s........r....c.
 000002c0: 0000 0000 0000 0000 0000 0000 0000 0005  ................
-000002d0: 0000 0000 0000 0073 7400 0000 6500 5a01  .......st...e.Z.
+000002d0: 0000 0000 0000 0073 8000 0000 6500 5a01  .......s....e.Z.
 000002e0: 6400 5a02 6401 5a03 6504 6a05 6402 6402  d.Z.d.Z.e.j.d.d.
 000002f0: 6403 6404 8d03 5a06 6504 6a07 6402 6405  d.d...Z.e.j.d.d.
-00000300: 8d01 5a08 6406 6407 8400 5a09 650a 650b  ..Z.d.d...Z.e.e.
-00000310: 1900 6408 9c01 6409 640a 8404 5a0c 640b  ..d...d.d...Z.d.
-00000320: 640c 8400 5a0d 640d 640e 8400 5a0e 8700  d...Z.d.d...Z...
-00000330: 6601 640f 6410 8408 5a0f 4700 6411 6412  f.d.d...Z.G.d.d.
-00000340: 8400 6412 8302 5a10 8700 0400 5a11 5300  ..d...Z.....Z.S.
-00000350: 2913 da12 4661 766f 7269 7465 5365 7269  )...FavoriteSeri
-00000360: 616c 697a 6572 7543 0000 000a 2020 2020  alizeruC....    
-00000370: 2020 2020 d0a1 d0b5 d180 d0b8 d0b0 d0bb      ............
-00000380: d0b8 d0b7 d0b0 d182 d0be d180 20d0 b4d0  ............ ...
-00000390: bbd1 8f20 d0b8 d0b7 d0b1 d180 d0b0 d0bd  ... ............
-000003a0: d0bd d0be d0b3 d0be 2e0a 2020 2020 54e9  ..........    T.
-000003b0: 6400 0000 2903 da08 7265 7175 6972 6564  d...)...required
-000003c0: da0a 7772 6974 655f 6f6e 6c79 da0a 6d61  ..write_only..ma
-000003d0: 785f 6c65 6e67 7468 2901 da09 7265 6164  x_length)...read
-000003e0: 5f6f 6e6c 7963 0100 0000 0000 0000 0000  _onlyc..........
-000003f0: 0000 0100 0000 0300 0000 4300 0000 730c  ..........C...s.
-00000400: 0000 007c 006a 00a0 0164 01a1 0153 0029  ...|.j...d...S.)
-00000410: 024e da07 7265 7175 6573 7429 02da 0763  .N..request)...c
-00000420: 6f6e 7465 7874 7211 0000 0029 01da 0473  ontextr....)...s
-00000430: 656c 6672 1200 0000 7212 0000 0072 1300  elfr....r....r..
-00000440: 0000 da0c 5f67 6574 5f72 6571 7565 7374  ...._get_request
-00000450: 2a00 0000 7302 0000 0000 017a 1f46 6176  *...s......z.Fav
-00000460: 6f72 6974 6553 6572 6961 6c69 7a65 722e  oriteSerializer.
-00000470: 5f67 6574 5f72 6571 7565 7374 2901 720d  _get_request).r.
-00000480: 0000 0063 0200 0000 0000 0000 0000 0000  ...c............
-00000490: 0200 0000 0800 0000 4300 0000 734a 0000  ........C...sJ..
-000004a0: 007a 167c 00a0 00a1 00a0 017c 016a 02a0  .z.|.......|.j..
-000004b0: 03a1 00a1 0157 0053 0004 0074 046b 0a72  .....W.S...t.k.r
-000004c0: 4401 0001 0001 0074 05a0 0674 0764 017c  D......t...t.d.|
-000004d0: 016a 026a 086a 0916 0083 01a1 0101 0059  .j.j.j.........Y
-000004e0: 0064 0253 0058 0064 0253 0029 0375 6400  .d.S.X.d.S.).ud.
-000004f0: 0000 0a20 2020 2020 2020 2020 2020 20d0  ...            .
-00000500: 92d0 bed0 b7d0 b2d1 80d0 b0d1 89d0 b0d0  ................
-00000510: b5d1 8220 d0bf d0be d0bb d0bd d18b d0b9  ... ............
-00000520: 20d0 bfd1 83d1 82d1 8c20 d0b4 d0be 20d0   ........ .... .
-00000530: bed0 b1d1 8ad0 b5d0 bad1 82d0 b020 636f  ............. co
-00000540: 6e74 656e 745f 6f62 6a65 6374 2e0a 2020  ntent_object..  
-00000550: 2020 2020 2020 75b4 0000 00d0 9cd0 bed0        u.........
-00000560: b4d0 b5d0 bbd1 8c20 2225 7322 20d0 bdd0  ....... "%s" ...
-00000570: b520 d0b8 d0bc d0b5 d0b5 d182 2067 6574  . .......... get
-00000580: 5f61 6273 6f6c 7574 655f 7572 6c28 292e  _absolute_url().
-00000590: 0a66 6176 6f72 6974 655f 7572 6c20 d0b1  .favorite_url ..
-000005a0: d183 d0b4 d0b5 d182 20d0 bed0 b1d0 bed0  ........ .......
-000005b0: b7d0 bdd0 b0d1 87d0 b5d0 bd2c 20d0 bad0  ..........., ...
-000005c0: b0d0 ba20 4e6f 6e65 2e0a 4661 766f 7269  ... None..Favori
-000005d0: 7465 4d69 7869 6e20 d0be d0b1 d18f d0b7  teMixin ........
-000005e0: d0b0 d182 d0b5 d0bb d0b5 d0bd 20d0 b4d0  ............ ...
-000005f0: bbd1 8f20 d0b8 d181 d0bf d0be d0bb d18c  ... ............
-00000600: d0b7 d0be d0b2 d0b0 d0bd d0b8 d18f 2e4e  ...............N
-00000610: 290a 721e 0000 00da 1262 7569 6c64 5f61  ).r......build_a
-00000620: 6273 6f6c 7574 655f 7572 69da 0e63 6f6e  bsolute_uri..con
-00000630: 7465 6e74 5f6f 626a 6563 74da 1067 6574  tent_object..get
-00000640: 5f61 6273 6f6c 7574 655f 7572 6cda 0e41  _absolute_url..A
-00000650: 7474 7269 6275 7465 4572 726f 72da 066c  ttributeError..l
-00000660: 6f67 6765 72da 0565 7272 6f72 da01 5fda  ogger..error.._.
-00000670: 095f 5f63 6c61 7373 5f5f da08 5f5f 6e61  .__class__..__na
-00000680: 6d65 5f5f 2902 721d 0000 00da 0869 6e73  me__).r......ins
-00000690: 7461 6e63 6572 1200 0000 7212 0000 0072  tancer....r....r
-000006a0: 1300 0000 da10 6765 745f 6661 766f 7269  ......get_favori
-000006b0: 7465 5f75 726c 2d00 0000 731a 0000 0000  te_url-...s.....
-000006c0: 0502 0108 0108 ff06 030e 0104 0102 0102  ................
-000006d0: 0308 fd02 ff02 ff04 087a 2346 6176 6f72  .........z#Favor
-000006e0: 6974 6553 6572 6961 6c69 7a65 722e 6765  iteSerializer.ge
-000006f0: 745f 6661 766f 7269 7465 5f75 726c 6302  t_favorite_urlc.
-00000700: 0000 0000 0000 0000 0000 0008 0000 0006  ................
-00000710: 0000 0043 0000 0073 8e00 0000 7400 a001  ...C...s....t...
-00000720: 7c00 a002 a100 a101 7d02 7c01 6401 1900  |.......}.|.d...
-00000730: 7d03 7c01 6402 1900 7d04 7403 7c03 8301  }.|.d...}.t.|...
-00000740: 7d05 7c00 6a04 6a05 7d06 7c05 a006 a100  }.|.j.j.}.|.....
-00000750: 0400 7d07 7264 7c07 6a07 6a08 7c04 6403  ..}.rd|.j.j.|.d.
-00000760: 8d01 a009 a100 7364 740a 6404 740b 6405  ......sdt.d.t.d.
-00000770: 7c03 7c04 6602 1600 8301 6901 8301 8201  |.|.f.....i.....
-00000780: 7c06 6a07 6a08 7c02 7c05 7c04 6406 8d03  |.j.j.|.|.|.d...
-00000790: a009 a100 728a 740a 6404 740b 6407 8301  ....r.t.d.t.d...
-000007a0: 6901 8301 8201 7c01 5300 2908 4e72 0c00  i.....|.S.).Nr..
-000007b0: 0000 da09 6f62 6a65 6374 5f69 6429 01da  ....object_id)..
-000007c0: 0269 6472 2400 0000 7a1e 2573 2077 6974  .idr$...z.%s wit
-000007d0: 6820 6964 2025 6920 646f 6573 206e 6f74  h id %i does not
-000007e0: 2065 7869 7374 732e 2903 da0c 7573 6572   exists.)...user
-000007f0: 5f73 6573 7369 6f6e da0c 636f 6e74 656e  _session..conten
-00000800: 745f 7479 7065 722a 0000 007a 2f54 6865  t_typer*...z/The
-00000810: 206f 626a 6563 7420 6861 7320 616c 7265   object has alre
-00000820: 6164 7920 6265 656e 2061 6464 6564 2074  ady been added t
-00000830: 6f20 6661 766f 7269 7465 732e 290c 7207  o favorites.).r.
-00000840: 0000 00da 1a67 6574 5f6f 725f 6372 6561  .....get_or_crea
-00000850: 7465 5f75 7365 725f 7365 7373 696f 6e72  te_user_sessionr
-00000860: 1e00 0000 7214 0000 00da 044d 6574 6172  ....r......Metar
-00000870: 0e00 0000 da0b 6d6f 6465 6c5f 636c 6173  ......model_clas
-00000880: 7372 1000 0000 da06 6669 6c74 6572 da06  sr......filter..
-00000890: 6578 6973 7473 7209 0000 0072 2500 0000  existsr....r%...
-000008a0: 2908 721d 0000 00da 0561 7474 7273 da04  ).r......attrs..
-000008b0: 7573 6572 720c 0000 0072 2a00 0000 722d  userr....r*...r-
-000008c0: 0000 0072 0e00 0000 7230 0000 0072 1200  ...r....r0...r..
-000008d0: 0000 7212 0000 0072 1300 0000 da08 7661  ..r....r......va
-000008e0: 6c69 6461 7465 4100 0000 7326 0000 0000  lidateA...s&....
-000008f0: 010e 0108 0108 0108 0108 020c 0112 0102  ................
-00000900: 0112 ff04 0406 0102 0102 0102 fd0a 0502  ................
-00000910: 010a ff04 047a 1b46 6176 6f72 6974 6553  .....z.FavoriteS
-00000920: 6572 6961 6c69 7a65 722e 7661 6c69 6461  erializer.valida
-00000930: 7465 6302 0000 0000 0000 0000 0000 0002  tec.............
-00000940: 0000 0006 0000 0043 0000 0073 2200 0000  .......C...s"...
-00000950: 7c01 7400 6b07 721e 7401 7402 6401 6402  |.t.k.r.t.t.d.d.
-00000960: a003 7400 a101 1600 8301 8301 8201 7c01  ..t...........|.
-00000970: 5300 2903 4e7a 144d 6f64 656c 206d 7573  S.).Nz.Model mus
-00000980: 7420 6265 2069 6e3a 2025 737a 022c 2029  t be in: %sz., )
-00000990: 04da 1841 4343 4550 5445 445f 4641 564f  ...ACCEPTED_FAVO
-000009a0: 5249 5445 5f4d 4f44 454c 5372 0900 0000  RITE_MODELSr....
-000009b0: 7225 0000 00da 046a 6f69 6e29 0272 1d00  r%.....join).r..
-000009c0: 0000 da05 7661 6c75 6572 1200 0000 7212  ....valuer....r.
-000009d0: 0000 0072 1300 0000 da13 7661 6c69 6461  ...r......valida
-000009e0: 7465 5f6d 6f64 656c 5f6e 616d 6559 0000  te_model_nameY..
-000009f0: 0073 0a00 0000 0001 0801 0201 10ff 0403  .s..............
-00000a00: 7a26 4661 766f 7269 7465 5365 7269 616c  z&FavoriteSerial
-00000a10: 697a 6572 2e76 616c 6964 6174 655f 6d6f  izer.validate_mo
-00000a20: 6465 6c5f 6e61 6d65 6302 0000 0000 0000  del_namec.......
-00000a30: 0000 0000 0004 0000 0004 0000 0003 0000  ................
-00000a40: 0073 2c00 0000 7c01 a000 6401 a101 7d02  .s,...|...d...}.
-00000a50: 7401 7c02 8301 7d03 7c01 a002 6402 7c03  t.|...}.|...d.|.
-00000a60: 6901 a101 0100 7403 8300 a004 7c01 a101  i.....t.....|...
-00000a70: 5300 2903 4e72 0c00 0000 722d 0000 0029  S.).Nr....r-...)
-00000a80: 05da 0370 6f70 7214 0000 00da 0675 7064  ...popr......upd
-00000a90: 6174 65da 0573 7570 6572 da06 6372 6561  ate..super..crea
-00000aa0: 7465 2904 721d 0000 00da 0e76 616c 6964  te).r......valid
-00000ab0: 6174 6564 5f64 6174 6172 0c00 0000 722d  ated_datar....r-
-00000ac0: 0000 00a9 0172 2600 0000 7212 0000 0072  .....r&...r....r
-00000ad0: 1300 0000 723d 0000 0060 0000 0073 0e00  ....r=...`...s..
-00000ae0: 0000 0001 0a01 0802 0401 0200 02ff 0604  ................
-00000af0: 7a19 4661 766f 7269 7465 5365 7269 616c  z.FavoriteSerial
-00000b00: 697a 6572 2e63 7265 6174 6563 0000 0000  izer.createc....
-00000b10: 0000 0000 0000 0000 0000 0000 0100 0000  ................
-00000b20: 4000 0000 7314 0000 0065 005a 0164 005a  @...s....e.Z.d.Z
-00000b30: 0265 035a 0464 015a 0564 0253 0029 037a  .e.Z.d.Z.d.S.).z
-00000b40: 1746 6176 6f72 6974 6553 6572 6961 6c69  .FavoriteSeriali
-00000b50: 7a65 722e 4d65 7461 2901 722c 0000 004e  zer.Meta).r,...N
-00000b60: 2906 7227 0000 00da 0a5f 5f6d 6f64 756c  ).r'.....__modul
-00000b70: 655f 5fda 0c5f 5f71 7561 6c6e 616d 655f  e__..__qualname_
-00000b80: 5f72 0b00 0000 720e 0000 00da 0765 7863  _r....r......exc
-00000b90: 6c75 6465 7212 0000 0072 1200 0000 7212  luder....r....r.
-00000ba0: 0000 0072 1300 0000 722f 0000 006a 0000  ...r....r/...j..
-00000bb0: 0073 0400 0000 0801 0401 722f 0000 0029  .s........r/...)
-00000bc0: 1272 2700 0000 7240 0000 0072 4100 0000  .r'...r@...rA...
-00000bd0: da07 5f5f 646f 635f 5f72 0800 0000 da09  ..__doc__r......
-00000be0: 4368 6172 4669 656c 6472 0c00 0000 da15  CharFieldr......
-00000bf0: 5365 7269 616c 697a 6572 4d65 7468 6f64  SerializerMethod
-00000c00: 4669 656c 645a 0c66 6176 6f72 6974 655f  FieldZ.favorite_
-00000c10: 7572 6c72 1e00 0000 7203 0000 00da 0373  urlr....r......s
-00000c20: 7472 7229 0000 0072 3500 0000 7239 0000  trr)...r5...r9..
-00000c30: 0072 3d00 0000 722f 0000 00da 0d5f 5f63  .r=...r/.....__c
-00000c40: 6c61 7373 6365 6c6c 5f5f 7212 0000 0072  lasscell__r....r
-00000c50: 1200 0000 723f 0000 0072 1300 0000 7215  ....r?...r....r.
-00000c60: 0000 001f 0000 0073 1e00 0000 0801 0403  .......s........
-00000c70: 0401 0200 0200 02ff 0603 0401 02ff 0604  ................
-00000c80: 0803 1214 0818 0807 0c0a 7215 0000 004e  ..........r....N
-00000c90: 291b da07 6c6f 6767 696e 6772 0200 0000  )...loggingr....
-00000ca0: da06 7479 7069 6e67 7203 0000 00da 0b64  ..typingr......d
-00000cb0: 6a61 6e67 6f2e 636f 6e66 7204 0000 00da  jango.confr.....
-00000cc0: 2264 6a61 6e67 6f2e 636f 6e74 7269 622e  "django.contrib.
-00000cd0: 636f 6e74 656e 7474 7970 6573 2e6d 6f64  contenttypes.mod
-00000ce0: 656c 7372 0500 0000 da18 646a 616e 676f  elsr......django
-00000cf0: 2e75 7469 6c73 2e74 7261 6e73 6c61 7469  .utils.translati
-00000d00: 6f6e 7206 0000 0072 2500 0000 da12 6761  onr....r%.....ga
-00000d10: 7270 6978 5f75 7365 722e 6d6f 6465 6c73  rpix_user.models
-00000d20: 7207 0000 00da 0e72 6573 745f 6672 616d  r......rest_fram
-00000d30: 6577 6f72 6b72 0800 0000 5a19 7265 7374  eworkr....Z.rest
-00000d40: 5f66 7261 6d65 776f 726b 2e65 7863 6570  _framework.excep
-00000d50: 7469 6f6e 7372 0900 0000 da06 6d6f 6465  tionsr......mode
-00000d60: 6c73 720b 0000 0072 3600 0000 7222 0000  lsr....r6...r"..
-00000d70: 0072 2700 0000 7223 0000 0072 4600 0000  .r'...r#...rF...
-00000d80: 7214 0000 00da 0f4d 6f64 656c 5365 7269  r......ModelSeri
-00000d90: 616c 697a 6572 7215 0000 0072 1200 0000  alizerr....r....
-00000da0: 7212 0000 0072 1200 0000 7213 0000 00da  r....r....r.....
-00000db0: 083c 6d6f 6475 6c65 3e01 0000 0073 2200  .<module>....s".
-00000dc0: 0000 0c02 0c02 0c01 0c01 0c01 0c02 0c01  ................
-00000dd0: 0c02 0c02 0201 0a01 0e01 0201 06ff 0a04  ................
-00000de0: 0803 1006                                ....
+00000300: 8d01 5a08 6504 6a09 6406 6407 8d01 5a0a  ..Z.e.j.d.d...Z.
+00000310: 6408 6409 8400 5a0b 650c 650d 1900 640a  d.d...Z.e.e...d.
+00000320: 9c01 640b 640c 8404 5a0e 640d 640e 8400  ..d.d...Z.d.d...
+00000330: 5a0f 640f 6410 8400 5a10 8700 6601 6411  Z.d.d...Z...f.d.
+00000340: 6412 8408 5a11 4700 6413 6414 8400 6414  d...Z.G.d.d...d.
+00000350: 8302 5a12 8700 0400 5a13 5300 2915 da12  ..Z.....Z.S.)...
+00000360: 4661 766f 7269 7465 5365 7269 616c 697a  FavoriteSerializ
+00000370: 6572 7543 0000 000a 2020 2020 2020 2020  eruC....        
+00000380: d0a1 d0b5 d180 d0b8 d0b0 d0bb d0b8 d0b7  ................
+00000390: d0b0 d182 d0be d180 20d0 b4d0 bbd1 8f20  ........ ...... 
+000003a0: d0b8 d0b7 d0b1 d180 d0b0 d0bd d0bd d0be  ................
+000003b0: d0b3 d0be 2e0a 2020 2020 54e9 6400 0000  ......    T.d...
+000003c0: 2903 da08 7265 7175 6972 6564 da0a 7772  )...required..wr
+000003d0: 6974 655f 6f6e 6c79 da0a 6d61 785f 6c65  ite_only..max_le
+000003e0: 6e67 7468 2901 da09 7265 6164 5f6f 6e6c  ngth)...read_onl
+000003f0: 794e 2901 da07 6465 6661 756c 7463 0100  yN)...defaultc..
+00000400: 0000 0000 0000 0000 0000 0100 0000 0300  ................
+00000410: 0000 4300 0000 730c 0000 007c 006a 00a0  ..C...s....|.j..
+00000420: 0164 01a1 0153 0029 024e da07 7265 7175  .d...S.).N..requ
+00000430: 6573 7429 02da 0763 6f6e 7465 7874 7211  est)...contextr.
+00000440: 0000 0029 01da 0473 656c 6672 1200 0000  ...)...selfr....
+00000450: 7212 0000 0072 1300 0000 da0c 5f67 6574  r....r......_get
+00000460: 5f72 6571 7565 7374 2c00 0000 7302 0000  _request,...s...
+00000470: 0000 017a 1f46 6176 6f72 6974 6553 6572  ...z.FavoriteSer
+00000480: 6961 6c69 7a65 722e 5f67 6574 5f72 6571  ializer._get_req
+00000490: 7565 7374 2901 720d 0000 0063 0200 0000  uest).r....c....
+000004a0: 0000 0000 0000 0000 0200 0000 0800 0000  ................
+000004b0: 4300 0000 734a 0000 007a 167c 00a0 00a1  C...sJ...z.|....
+000004c0: 00a0 017c 016a 02a0 03a1 00a1 0157 0053  ...|.j.......W.S
+000004d0: 0004 0074 046b 0a72 4401 0001 0001 0074  ...t.k.rD......t
+000004e0: 05a0 0674 0764 017c 016a 026a 086a 0916  ...t.d.|.j.j.j..
+000004f0: 0083 01a1 0101 0059 0064 0253 0058 0064  .......Y.d.S.X.d
+00000500: 0253 0029 0375 6400 0000 0a20 2020 2020  .S.).ud....     
+00000510: 2020 2020 2020 20d0 92d0 bed0 b7d0 b2d1         .........
+00000520: 80d0 b0d1 89d0 b0d0 b5d1 8220 d0bf d0be  ........... ....
+00000530: d0bb d0bd d18b d0b9 20d0 bfd1 83d1 82d1  ........ .......
+00000540: 8c20 d0b4 d0be 20d0 bed0 b1d1 8ad0 b5d0  . .... .........
+00000550: bad1 82d0 b020 636f 6e74 656e 745f 6f62  ..... content_ob
+00000560: 6a65 6374 2e0a 2020 2020 2020 2020 75b4  ject..        u.
+00000570: 0000 00d0 9cd0 bed0 b4d0 b5d0 bbd1 8c20  ............... 
+00000580: 2225 7322 20d0 bdd0 b520 d0b8 d0bc d0b5  "%s" .... ......
+00000590: d0b5 d182 2067 6574 5f61 6273 6f6c 7574  .... get_absolut
+000005a0: 655f 7572 6c28 292e 0a66 6176 6f72 6974  e_url()..favorit
+000005b0: 655f 7572 6c20 d0b1 d183 d0b4 d0b5 d182  e_url ..........
+000005c0: 20d0 bed0 b1d0 bed0 b7d0 bdd0 b0d1 87d0   ...............
+000005d0: b5d0 bd2c 20d0 bad0 b0d0 ba20 4e6f 6e65  ..., ...... None
+000005e0: 2e0a 4661 766f 7269 7465 4d69 7869 6e20  ..FavoriteMixin 
+000005f0: d0be d0b1 d18f d0b7 d0b0 d182 d0b5 d0bb  ................
+00000600: d0b5 d0bd 20d0 b4d0 bbd1 8f20 d0b8 d181  .... ...... ....
+00000610: d0bf d0be d0bb d18c d0b7 d0be d0b2 d0b0  ................
+00000620: d0bd d0b8 d18f 2e4e 290a 721f 0000 00da  .......N).r.....
+00000630: 1262 7569 6c64 5f61 6273 6f6c 7574 655f  .build_absolute_
+00000640: 7572 69da 0e63 6f6e 7465 6e74 5f6f 626a  uri..content_obj
+00000650: 6563 74da 1067 6574 5f61 6273 6f6c 7574  ect..get_absolut
+00000660: 655f 7572 6cda 0e41 7474 7269 6275 7465  e_url..Attribute
+00000670: 4572 726f 72da 066c 6f67 6765 72da 0565  Error..logger..e
+00000680: 7272 6f72 da01 5fda 095f 5f63 6c61 7373  rror.._..__class
+00000690: 5f5f da08 5f5f 6e61 6d65 5f5f 2902 721e  __..__name__).r.
+000006a0: 0000 00da 0869 6e73 7461 6e63 6572 1200  .....instancer..
+000006b0: 0000 7212 0000 0072 1300 0000 da10 6765  ..r....r......ge
+000006c0: 745f 6661 766f 7269 7465 5f75 726c 2f00  t_favorite_url/.
+000006d0: 0000 731a 0000 0000 0502 0108 0108 ff06  ..s.............
+000006e0: 030e 0104 0102 0102 0308 fd02 ff02 ff04  ................
+000006f0: 087a 2346 6176 6f72 6974 6553 6572 6961  .z#FavoriteSeria
+00000700: 6c69 7a65 722e 6765 745f 6661 766f 7269  lizer.get_favori
+00000710: 7465 5f75 726c 6302 0000 0000 0000 0000  te_urlc.........
+00000720: 0000 0008 0000 0006 0000 0043 0000 0073  ...........C...s
+00000730: 8e00 0000 7400 a001 7c00 a002 a100 a101  ....t...|.......
+00000740: 7d02 7c01 6401 1900 7d03 7c01 6402 1900  }.|.d...}.|.d...
+00000750: 7d04 7403 7c03 8301 7d05 7c00 6a04 6a05  }.t.|...}.|.j.j.
+00000760: 7d06 7c05 a006 a100 0400 7d07 7264 7c07  }.|.......}.rd|.
+00000770: 6a07 6a08 7c04 6403 8d01 a009 a100 7364  j.j.|.d.......sd
+00000780: 740a 6404 740b 6405 7c03 7c04 6602 1600  t.d.t.d.|.|.f...
+00000790: 8301 6901 8301 8201 7c06 6a07 6a08 7c02  ..i.....|.j.j.|.
+000007a0: 7c05 7c04 6406 8d03 a009 a100 728a 740a  |.|.d.......r.t.
+000007b0: 6404 740b 6407 8301 6901 8301 8201 7c01  d.t.d...i.....|.
+000007c0: 5300 2908 4e72 0c00 0000 da09 6f62 6a65  S.).Nr......obje
+000007d0: 6374 5f69 6429 01da 0269 6472 2500 0000  ct_id)...idr%...
+000007e0: 7a1e 2573 2077 6974 6820 6964 2025 6920  z.%s with id %i 
+000007f0: 646f 6573 206e 6f74 2065 7869 7374 732e  does not exists.
+00000800: 2903 da0c 7573 6572 5f73 6573 7369 6f6e  )...user_session
+00000810: da0c 636f 6e74 656e 745f 7479 7065 722b  ..content_typer+
+00000820: 0000 007a 2f54 6865 206f 626a 6563 7420  ...z/The object 
+00000830: 6861 7320 616c 7265 6164 7920 6265 656e  has already been
+00000840: 2061 6464 6564 2074 6f20 6661 766f 7269   added to favori
+00000850: 7465 732e 290c 7207 0000 00da 1a67 6574  tes.).r......get
+00000860: 5f6f 725f 6372 6561 7465 5f75 7365 725f  _or_create_user_
+00000870: 7365 7373 696f 6e72 1f00 0000 7214 0000  sessionr....r...
+00000880: 00da 044d 6574 6172 0e00 0000 da0b 6d6f  ...Metar......mo
+00000890: 6465 6c5f 636c 6173 7372 1000 0000 da06  del_classr......
+000008a0: 6669 6c74 6572 da06 6578 6973 7473 7209  filter..existsr.
+000008b0: 0000 0072 2600 0000 2908 721e 0000 00da  ...r&...).r.....
+000008c0: 0561 7474 7273 da04 7573 6572 720c 0000  .attrs..userr...
+000008d0: 0072 2b00 0000 722e 0000 0072 0e00 0000  .r+...r....r....
+000008e0: 7231 0000 0072 1200 0000 7212 0000 0072  r1...r....r....r
+000008f0: 1300 0000 da08 7661 6c69 6461 7465 4300  ......validateC.
+00000900: 0000 7326 0000 0000 010e 0108 0108 0108  ..s&............
+00000910: 0108 020c 0112 0102 0112 ff04 0406 0102  ................
+00000920: 0102 0102 fd0a 0502 010a ff04 047a 1b46  .............z.F
+00000930: 6176 6f72 6974 6553 6572 6961 6c69 7a65  avoriteSerialize
+00000940: 722e 7661 6c69 6461 7465 6302 0000 0000  r.validatec.....
+00000950: 0000 0000 0000 0002 0000 0006 0000 0043  ...............C
+00000960: 0000 0073 2200 0000 7c01 7400 6b07 721e  ...s"...|.t.k.r.
+00000970: 7401 7402 6401 6402 a003 7400 a101 1600  t.t.d.d...t.....
+00000980: 8301 8301 8201 7c01 5300 2903 4e7a 144d  ......|.S.).Nz.M
+00000990: 6f64 656c 206d 7573 7420 6265 2069 6e3a  odel must be in:
+000009a0: 2025 737a 022c 2029 04da 1841 4343 4550   %sz., )...ACCEP
+000009b0: 5445 445f 4641 564f 5249 5445 5f4d 4f44  TED_FAVORITE_MOD
+000009c0: 454c 5372 0900 0000 7226 0000 00da 046a  ELSr....r&.....j
+000009d0: 6f69 6e29 0272 1e00 0000 da05 7661 6c75  oin).r......valu
+000009e0: 6572 1200 0000 7212 0000 0072 1300 0000  er....r....r....
+000009f0: da13 7661 6c69 6461 7465 5f6d 6f64 656c  ..validate_model
+00000a00: 5f6e 616d 655b 0000 0073 0a00 0000 0001  _name[...s......
+00000a10: 0801 0201 10ff 0403 7a26 4661 766f 7269  ........z&Favori
+00000a20: 7465 5365 7269 616c 697a 6572 2e76 616c  teSerializer.val
+00000a30: 6964 6174 655f 6d6f 6465 6c5f 6e61 6d65  idate_model_name
+00000a40: 6302 0000 0000 0000 0000 0000 0004 0000  c...............
+00000a50: 0004 0000 0003 0000 0073 2c00 0000 7c01  .........s,...|.
+00000a60: a000 6401 a101 7d02 7401 7c02 8301 7d03  ..d...}.t.|...}.
+00000a70: 7c01 a002 6402 7c03 6901 a101 0100 7403  |...d.|.i.....t.
+00000a80: 8300 a004 7c01 a101 5300 2903 4e72 0c00  ....|...S.).Nr..
+00000a90: 0000 722e 0000 0029 05da 0370 6f70 7214  ..r....)...popr.
+00000aa0: 0000 00da 0675 7064 6174 65da 0573 7570  .....update..sup
+00000ab0: 6572 da06 6372 6561 7465 2904 721e 0000  er..create).r...
+00000ac0: 00da 0e76 616c 6964 6174 6564 5f64 6174  ...validated_dat
+00000ad0: 6172 0c00 0000 722e 0000 00a9 0172 2700  ar....r......r'.
+00000ae0: 0000 7212 0000 0072 1300 0000 723e 0000  ..r....r....r>..
+00000af0: 0062 0000 0073 0e00 0000 0001 0a01 0802  .b...s..........
+00000b00: 0401 0200 02ff 0604 7a19 4661 766f 7269  ........z.Favori
+00000b10: 7465 5365 7269 616c 697a 6572 2e63 7265  teSerializer.cre
+00000b20: 6174 6563 0000 0000 0000 0000 0000 0000  atec............
+00000b30: 0000 0000 0100 0000 4000 0000 7314 0000  ........@...s...
+00000b40: 0065 005a 0164 005a 0265 035a 0464 015a  .e.Z.d.Z.e.Z.d.Z
+00000b50: 0564 0253 0029 037a 1746 6176 6f72 6974  .d.S.).z.Favorit
+00000b60: 6553 6572 6961 6c69 7a65 722e 4d65 7461  eSerializer.Meta
+00000b70: 2901 722d 0000 004e 2906 7228 0000 00da  ).r-...N).r(....
+00000b80: 0a5f 5f6d 6f64 756c 655f 5fda 0c5f 5f71  .__module__..__q
+00000b90: 7561 6c6e 616d 655f 5f72 0b00 0000 720e  ualname__r....r.
+00000ba0: 0000 00da 0765 7863 6c75 6465 7212 0000  .....excluder...
+00000bb0: 0072 1200 0000 7212 0000 0072 1300 0000  .r....r....r....
+00000bc0: 7230 0000 006c 0000 0073 0400 0000 0801  r0...l...s......
+00000bd0: 0401 7230 0000 0029 1472 2800 0000 7241  ..r0...).r(...rA
+00000be0: 0000 0072 4200 0000 da07 5f5f 646f 635f  ...rB.....__doc_
+00000bf0: 5f72 0800 0000 da09 4368 6172 4669 656c  _r......CharFiel
+00000c00: 6472 0c00 0000 da15 5365 7269 616c 697a  dr......Serializ
+00000c10: 6572 4d65 7468 6f64 4669 656c 645a 0c66  erMethodFieldZ.f
+00000c20: 6176 6f72 6974 655f 7572 6cda 0b48 6964  avorite_url..Hid
+00000c30: 6465 6e46 6965 6c64 722e 0000 0072 1f00  denFieldr....r..
+00000c40: 0000 7203 0000 00da 0373 7472 722a 0000  ..r......strr*..
+00000c50: 0072 3600 0000 723a 0000 0072 3e00 0000  .r6...r:...r>...
+00000c60: 7230 0000 00da 0d5f 5f63 6c61 7373 6365  r0.....__classce
+00000c70: 6c6c 5f5f 7212 0000 0072 1200 0000 7240  ll__r....r....r@
+00000c80: 0000 0072 1300 0000 7215 0000 001f 0000  ...r....r.......
+00000c90: 0073 2000 0000 0801 0403 0401 0200 0200  .s .............
+00000ca0: 02ff 0603 0401 02ff 0604 0c02 0803 1214  ................
+00000cb0: 0818 0807 0c0a 7215 0000 004e 291b da07  ......r....N)...
+00000cc0: 6c6f 6767 696e 6772 0200 0000 da06 7479  loggingr......ty
+00000cd0: 7069 6e67 7203 0000 00da 0b64 6a61 6e67  pingr......djang
+00000ce0: 6f2e 636f 6e66 7204 0000 00da 2264 6a61  o.confr....."dja
+00000cf0: 6e67 6f2e 636f 6e74 7269 622e 636f 6e74  ngo.contrib.cont
+00000d00: 656e 7474 7970 6573 2e6d 6f64 656c 7372  enttypes.modelsr
+00000d10: 0500 0000 da18 646a 616e 676f 2e75 7469  ......django.uti
+00000d20: 6c73 2e74 7261 6e73 6c61 7469 6f6e 7206  ls.translationr.
+00000d30: 0000 0072 2600 0000 da12 6761 7270 6978  ...r&.....garpix
+00000d40: 5f75 7365 722e 6d6f 6465 6c73 7207 0000  _user.modelsr...
+00000d50: 00da 0e72 6573 745f 6672 616d 6577 6f72  ...rest_framewor
+00000d60: 6b72 0800 0000 5a19 7265 7374 5f66 7261  kr....Z.rest_fra
+00000d70: 6d65 776f 726b 2e65 7863 6570 7469 6f6e  mework.exception
+00000d80: 7372 0900 0000 da06 6d6f 6465 6c73 720b  sr......modelsr.
+00000d90: 0000 0072 3700 0000 7223 0000 0072 2800  ...r7...r#...r(.
+00000da0: 0000 7224 0000 0072 4800 0000 7214 0000  ..r$...rH...r...
+00000db0: 00da 0f4d 6f64 656c 5365 7269 616c 697a  ...ModelSerializ
+00000dc0: 6572 7215 0000 0072 1200 0000 7212 0000  err....r....r...
+00000dd0: 0072 1200 0000 7213 0000 00da 083c 6d6f  .r....r......<mo
+00000de0: 6475 6c65 3e01 0000 0073 2200 0000 0c02  dule>....s".....
+00000df0: 0c02 0c01 0c01 0c01 0c02 0c01 0c02 0c02  ................
+00000e00: 0201 0a01 0e01 0201 06ff 0a04 0803 1006  ................
```

### Comparing `garpix_favourite-2.0.0/garpix_favourite/__pycache__/views.cpython-38.pyc` & `garpix_favourite-2.1.0/garpix_favourite/__pycache__/views.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Wed May 10 16:11:01 2023 UTC, .py size: 1574 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 26% similar despite different names*

```diff
@@ -1,122 +1,117 @@
-00000000: 550d 0d0a 0000 0000 15c2 5b64 2606 0000  U.........[d&...
+00000000: 550d 0d0a 0000 0000 9623 6b64 db05 0000  U........#kd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0007 0000 0040 0000 0073 a000 0000 6400  .....@...s....d.
+00000020: 0007 0000 0040 0000 0073 9400 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 0100 6400 6403 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
 00000050: 0100 6400 6404 6c06 6d07 5a07 6d08 5a08  ..d.d.l.m.Z.m.Z.
 00000060: 6d09 5a09 0100 6400 6405 6c0a 6d0b 5a0b  m.Z...d.d.l.m.Z.
-00000070: 0100 6400 6406 6c0c 6d0d 5a0d 0100 6400  ..d.d.l.m.Z...d.
-00000080: 6407 6c0e 6d0f 5a0f 0100 6408 6409 6c10  d.l.m.Z...d.d.l.
-00000090: 6d11 5a11 0100 6408 640a 6c12 6d13 5a13  m.Z...d.d.l.m.Z.
-000000a0: 0100 6501 6505 8300 6701 640b 8d01 4700  ..e.e...g.d...G.
-000000b0: 640c 640d 8400 640d 6508 6a14 6508 6a15  d.d...d.e.j.e.j.
-000000c0: 6507 6a16 8305 8301 5a17 640e 5300 290f  e.j.....Z.d.S.).
-000000d0: e900 0000 0029 01da 0d65 7874 656e 645f  .....)...extend_
-000000e0: 7363 6865 6d61 2901 da0b 5573 6572 5365  schema)...UserSe
-000000f0: 7373 696f 6e29 01da 2375 7365 725f 7365  ssion)..#user_se
-00000100: 7373 696f 6e5f 746f 6b65 6e5f 6865 6164  ssion_token_head
-00000110: 6572 5f70 6172 616d 6574 6572 2903 da08  er_parameter)...
-00000120: 7669 6577 7365 7473 da06 6d69 7869 6e73  viewsets..mixins
-00000130: da06 7374 6174 7573 2901 da06 6163 7469  ..status)...acti
-00000140: 6f6e 2901 da0f 4973 4175 7468 656e 7469  on)...IsAuthenti
-00000150: 6361 7465 6429 01da 0852 6573 706f 6e73  cated)...Respons
-00000160: 65e9 0100 0000 2901 da08 4661 766f 7269  e.....)...Favori
-00000170: 7465 2901 da12 4661 766f 7269 7465 5365  te)...FavoriteSe
-00000180: 7269 616c 697a 6572 2901 da0a 7061 7261  rializer)...para
-00000190: 6d65 7465 7273 6300 0000 0000 0000 0000  metersc.........
-000001a0: 0000 0000 0000 0005 0000 0040 0000 0073  ...........@...s
-000001b0: 3800 0000 6500 5a01 6400 5a02 6503 5a04  8...e.Z.d.Z.e.Z.
-000001c0: 6401 6402 8400 5a05 6403 6404 8400 5a06  d.d...Z.d.d...Z.
-000001d0: 6507 6405 6701 6406 6407 6408 8d03 6409  e.d.g.d.d.d...d.
-000001e0: 640a 8400 8301 5a08 640b 5300 290c da0f  d.....Z.d.S.)...
-000001f0: 4661 766f 7269 7465 5669 6577 5365 7463  FavoriteViewSetc
-00000200: 0100 0000 0000 0000 0000 0000 0200 0000  ................
-00000210: 0300 0000 4300 0000 731a 0000 0074 00a0  ....C...s....t..
-00000220: 017c 006a 02a1 017d 0174 036a 046a 057c  .|.j...}.t.j.j.|
-00000230: 0164 018d 0153 00a9 024e 2901 da0c 7573  .d...S...N)...us
-00000240: 6572 5f73 6573 7369 6f6e 2906 7203 0000  er_session).r...
-00000250: 00da 1a67 6574 5f6f 725f 6372 6561 7465  ...get_or_create
-00000260: 5f75 7365 725f 7365 7373 696f 6eda 0772  _user_session..r
-00000270: 6571 7565 7374 720c 0000 00da 076f 626a  equestr......obj
-00000280: 6563 7473 da06 6669 6c74 6572 2902 da04  ects..filter)...
-00000290: 7365 6c66 da04 7573 6572 a900 7218 0000  self..user..r...
-000002a0: 00fa 512f 5573 6572 732f 7669 6b74 6f72  ..Q/Users/viktor
-000002b0: 6961 7265 7365 746f 7661 2f47 4152 5049  iaresetova/GARPI
-000002c0: 582f 6761 7270 6978 5f66 6176 6f75 7269  X/garpix_favouri
-000002d0: 7465 2f62 6163 6b65 6e64 2f67 6172 7069  te/backend/garpi
-000002e0: 785f 6661 766f 7572 6974 652f 7669 6577  x_favourite/view
-000002f0: 732e 7079 da0c 6765 745f 7175 6572 7973  s.py..get_querys
-00000300: 6574 1700 0000 7308 0000 0000 010c 0106  et....s.........
-00000310: 0102 ff7a 1c46 6176 6f72 6974 6556 6965  ...z.FavoriteVie
-00000320: 7753 6574 2e67 6574 5f71 7565 7279 7365  wSet.get_queryse
-00000330: 7463 0200 0000 0000 0000 0000 0000 0300  tc..............
-00000340: 0000 0300 0000 4300 0000 731c 0000 0074  ......C...s....t
-00000350: 00a0 017c 006a 02a1 017d 027c 016a 037c  ...|.j...}.|.j.|
-00000360: 0264 018d 0101 0064 0053 0072 1000 0000  .d.....d.S.r....
-00000370: 2904 7203 0000 0072 1200 0000 7213 0000  ).r....r....r...
-00000380: 00da 0473 6176 6529 0372 1600 0000 da0a  ...save).r......
-00000390: 7365 7269 616c 697a 6572 7217 0000 0072  serializerr....r
-000003a0: 1800 0000 7218 0000 0072 1900 0000 da0e  ....r....r......
-000003b0: 7065 7266 6f72 6d5f 6372 6561 7465 1d00  perform_create..
-000003c0: 0000 7308 0000 0000 010c 0104 0102 ff7a  ..s............z
-000003d0: 1e46 6176 6f72 6974 6556 6965 7753 6574  .FavoriteViewSet
-000003e0: 2e70 6572 666f 726d 5f63 7265 6174 65da  .perform_create.
-000003f0: 0347 4554 46da 0763 7572 7265 6e74 2903  .GETF..current).
-00000400: da07 6d65 7468 6f64 73da 0664 6574 6169  ..methods..detai
-00000410: 6cda 0875 726c 5f70 6174 6863 0200 0000  l..url_pathc....
-00000420: 0000 0000 0000 0000 0500 0000 0400 0000  ................
-00000430: 4300 0000 7358 0000 007c 00a0 007c 00a0  C...sX...|...|..
-00000440: 01a1 00a1 017d 027c 00a0 027c 02a1 017d  .....}.|...|...}
-00000450: 037c 0364 006b 0972 3a7c 006a 037c 0364  .|.d.k.r:|.j.|.d
-00000460: 0164 028d 027d 047c 00a0 047c 046a 05a1  .d...}.|...|.j..
-00000470: 0153 007c 006a 037c 0264 0164 028d 027d  .S.|.j.|.d.d...}
-00000480: 0474 067c 046a 0574 076a 0864 038d 0253  .t.|.j.t.j.d...S
-00000490: 0029 044e 5429 01da 046d 616e 7929 0172  .).NT)...many).r
-000004a0: 0700 0000 2909 da0f 6669 6c74 6572 5f71  ....)...filter_q
-000004b0: 7565 7279 7365 7472 1a00 0000 da11 7061  uerysetr......pa
-000004c0: 6769 6e61 7465 5f71 7565 7279 7365 74da  ginate_queryset.
-000004d0: 0e67 6574 5f73 6572 6961 6c69 7a65 72da  .get_serializer.
-000004e0: 1667 6574 5f70 6167 696e 6174 6564 5f72  .get_paginated_r
-000004f0: 6573 706f 6e73 65da 0464 6174 6172 0a00  esponse..datar..
-00000500: 0000 7207 0000 00da 0b48 5454 505f 3230  ..r......HTTP_20
-00000510: 305f 4f4b 2905 7216 0000 0072 1300 0000  0_OK).r....r....
-00000520: da08 7175 6572 7973 6574 da04 7061 6765  ..queryset..page
-00000530: 721c 0000 0072 1800 0000 7218 0000 0072  r....r....r....r
-00000540: 1900 0000 da12 6765 745f 7573 6572 5f66  ......get_user_f
-00000550: 6176 6f72 6974 6573 2300 0000 730e 0000  avorites#...s...
-00000560: 0000 020e 020a 0108 010e 010c 020e 017a  ...............z
-00000570: 2246 6176 6f72 6974 6556 6965 7753 6574  "FavoriteViewSet
-00000580: 2e67 6574 5f75 7365 725f 6661 766f 7269  .get_user_favori
-00000590: 7465 734e 2909 da08 5f5f 6e61 6d65 5f5f  tesN)...__name__
-000005a0: da0a 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f  ..__module__..__
-000005b0: 7175 616c 6e61 6d65 5f5f 720d 0000 00da  qualname__r.....
-000005c0: 1073 6572 6961 6c69 7a65 725f 636c 6173  .serializer_clas
-000005d0: 7372 1a00 0000 721d 0000 0072 0800 0000  sr....r....r....
-000005e0: 722c 0000 0072 1800 0000 7218 0000 0072  r,...r....r....r
-000005f0: 1800 0000 7219 0000 0072 0f00 0000 0d00  ....r....r......
-00000600: 0000 730a 0000 0008 0804 0208 0608 060e  ..s.............
-00000610: 0172 0f00 0000 4e29 18da 1564 7266 5f73  .r....N)...drf_s
-00000620: 7065 6374 6163 756c 6172 2e75 7469 6c73  pectacular.utils
-00000630: 7202 0000 00da 1267 6172 7069 785f 7573  r......garpix_us
-00000640: 6572 2e6d 6f64 656c 7372 0300 0000 da21  er.modelsr.....!
-00000650: 6761 7270 6978 5f75 7365 722e 7574 696c  garpix_user.util
-00000660: 732e 6472 665f 7370 6563 7461 6375 6c61  s.drf_spectacula
-00000670: 7272 0400 0000 da0e 7265 7374 5f66 7261  rr......rest_fra
-00000680: 6d65 776f 726b 7205 0000 0072 0600 0000  meworkr....r....
-00000690: 7207 0000 00da 1972 6573 745f 6672 616d  r......rest_fram
-000006a0: 6577 6f72 6b2e 6465 636f 7261 746f 7273  ework.decorators
-000006b0: 7208 0000 00da 1a72 6573 745f 6672 616d  r......rest_fram
-000006c0: 6577 6f72 6b2e 7065 726d 6973 7369 6f6e  ework.permission
-000006d0: 7372 0900 0000 da17 7265 7374 5f66 7261  sr......rest_fra
-000006e0: 6d65 776f 726b 2e72 6573 706f 6e73 6572  mework.responser
-000006f0: 0a00 0000 da06 6d6f 6465 6c73 720c 0000  ......modelsr...
-00000700: 00da 0b73 6572 6961 6c69 7a65 7273 720d  ...serializersr.
-00000710: 0000 00da 1043 7265 6174 654d 6f64 656c  .....CreateModel
-00000720: 4d69 7869 6eda 1144 6573 7472 6f79 4d6f  Mixin..DestroyMo
-00000730: 6465 6c4d 6978 696e da0e 4765 6e65 7269  delMixin..Generi
-00000740: 6356 6965 7753 6574 720f 0000 0072 1800  cViewSetr....r..
-00000750: 0000 7218 0000 0072 1800 0000 7219 0000  ..r....r....r...
-00000760: 00da 083c 6d6f 6475 6c65 3e01 0000 0073  ...<module>....s
-00000770: 2000 0000 0c01 0c01 0c01 1401 0c01 0c01   ...............
-00000780: 0c02 0c01 0c03 0202 04ff 02ff 0405 0e01  ................
-00000790: 0401 04fe                                ....
+00000070: 0100 6400 6406 6c0c 6d0d 5a0d 0100 6407  ..d.d.l.m.Z...d.
+00000080: 6408 6c0e 6d0f 5a0f 0100 6407 6409 6c10  d.l.m.Z...d.d.l.
+00000090: 6d11 5a11 0100 6501 6505 8300 6701 640a  m.Z...e.e...g.d.
+000000a0: 8d01 4700 640b 640c 8400 640c 6508 6a12  ..G.d.d...d.e.j.
+000000b0: 6508 6a13 6507 6a14 8305 8301 5a15 640d  e.j.e.j.....Z.d.
+000000c0: 5300 290e e900 0000 0029 01da 0d65 7874  S.)......)...ext
+000000d0: 656e 645f 7363 6865 6d61 2901 da0b 5573  end_schema)...Us
+000000e0: 6572 5365 7373 696f 6e29 01da 2375 7365  erSession)..#use
+000000f0: 725f 7365 7373 696f 6e5f 746f 6b65 6e5f  r_session_token_
+00000100: 6865 6164 6572 5f70 6172 616d 6574 6572  header_parameter
+00000110: 2903 da08 7669 6577 7365 7473 da06 6d69  )...viewsets..mi
+00000120: 7869 6e73 da06 7374 6174 7573 2901 da06  xins..status)...
+00000130: 6163 7469 6f6e 2901 da08 5265 7370 6f6e  action)...Respon
+00000140: 7365 e901 0000 0029 01da 0846 6176 6f72  se.....)...Favor
+00000150: 6974 6529 01da 1246 6176 6f72 6974 6553  ite)...FavoriteS
+00000160: 6572 6961 6c69 7a65 7229 01da 0a70 6172  erializer)...par
+00000170: 616d 6574 6572 7363 0000 0000 0000 0000  ametersc........
+00000180: 0000 0000 0000 0000 0500 0000 4000 0000  ............@...
+00000190: 7338 0000 0065 005a 0164 005a 0265 035a  s8...e.Z.d.Z.e.Z
+000001a0: 0464 0164 0284 005a 0564 0364 0484 005a  .d.d...Z.d.d...Z
+000001b0: 0665 0764 0567 0164 0664 0764 088d 0364  .e.d.g.d.d.d...d
+000001c0: 0964 0a84 0083 015a 0864 0b53 0029 0cda  .d.....Z.d.S.)..
+000001d0: 0f46 6176 6f72 6974 6556 6965 7753 6574  .FavoriteViewSet
+000001e0: 6301 0000 0000 0000 0000 0000 0002 0000  c...............
+000001f0: 0003 0000 0043 0000 0073 1a00 0000 7400  .....C...s....t.
+00000200: a001 7c00 6a02 a101 7d01 7403 6a04 6a05  ..|.j...}.t.j.j.
+00000210: 7c01 6401 8d01 5300 a902 4e29 01da 0c75  |.d...S...N)...u
+00000220: 7365 725f 7365 7373 696f 6e29 0672 0300  ser_session).r..
+00000230: 0000 da10 6765 745f 6672 6f6d 5f72 6571  ....get_from_req
+00000240: 7565 7374 da07 7265 7175 6573 7472 0b00  uest..requestr..
+00000250: 0000 da07 6f62 6a65 6374 73da 0666 696c  ....objects..fil
+00000260: 7465 7229 02da 0473 656c 66da 0475 7365  ter)...self..use
+00000270: 72a9 0072 1700 0000 fa51 2f55 7365 7273  r..r.....Q/Users
+00000280: 2f76 696b 746f 7269 6172 6573 6574 6f76  /viktoriaresetov
+00000290: 612f 4741 5250 4958 2f67 6172 7069 785f  a/GARPIX/garpix_
+000002a0: 6661 766f 7572 6974 652f 6261 636b 656e  favourite/backen
+000002b0: 642f 6761 7270 6978 5f66 6176 6f75 7269  d/garpix_favouri
+000002c0: 7465 2f76 6965 7773 2e70 79da 0c67 6574  te/views.py..get
+000002d0: 5f71 7565 7279 7365 7416 0000 0073 0800  _queryset....s..
+000002e0: 0000 0001 0c01 0601 02ff 7a1c 4661 766f  ..........z.Favo
+000002f0: 7269 7465 5669 6577 5365 742e 6765 745f  riteViewSet.get_
+00000300: 7175 6572 7973 6574 6302 0000 0000 0000  querysetc.......
+00000310: 0000 0000 0003 0000 0003 0000 0043 0000  .............C..
+00000320: 0073 1c00 0000 7400 a001 7c00 6a02 a101  .s....t...|.j...
+00000330: 7d02 7c01 6a03 7c02 6401 8d01 0100 6400  }.|.j.|.d.....d.
+00000340: 5300 720f 0000 0029 0472 0300 0000 7211  S.r....).r....r.
+00000350: 0000 0072 1200 0000 da04 7361 7665 2903  ...r......save).
+00000360: 7215 0000 00da 0a73 6572 6961 6c69 7a65  r......serialize
+00000370: 7272 1600 0000 7217 0000 0072 1700 0000  rr....r....r....
+00000380: 7218 0000 00da 0e70 6572 666f 726d 5f63  r......perform_c
+00000390: 7265 6174 651c 0000 0073 0800 0000 0001  reate....s......
+000003a0: 0c01 0401 02ff 7a1e 4661 766f 7269 7465  ......z.Favorite
+000003b0: 5669 6577 5365 742e 7065 7266 6f72 6d5f  ViewSet.perform_
+000003c0: 6372 6561 7465 da03 4745 5446 da07 6375  create..GETF..cu
+000003d0: 7272 656e 7429 03da 076d 6574 686f 6473  rrent)...methods
+000003e0: da06 6465 7461 696c da08 7572 6c5f 7061  ..detail..url_pa
+000003f0: 7468 6302 0000 0000 0000 0000 0000 0005  thc.............
+00000400: 0000 0004 0000 0043 0000 0073 5800 0000  .......C...sX...
+00000410: 7c00 a000 7c00 a001 a100 a101 7d02 7c00  |...|.......}.|.
+00000420: a002 7c02 a101 7d03 7c03 6400 6b09 723a  ..|...}.|.d.k.r:
+00000430: 7c00 6a03 7c03 6401 6402 8d02 7d04 7c00  |.j.|.d.d...}.|.
+00000440: a004 7c04 6a05 a101 5300 7c00 6a03 7c02  ..|.j...S.|.j.|.
+00000450: 6401 6402 8d02 7d04 7406 7c04 6a05 7407  d.d...}.t.|.j.t.
+00000460: 6a08 6403 8d02 5300 2904 4e54 2901 da04  j.d...S.).NT)...
+00000470: 6d61 6e79 2901 7207 0000 0029 09da 0f66  many).r....)...f
+00000480: 696c 7465 725f 7175 6572 7973 6574 7219  ilter_querysetr.
+00000490: 0000 00da 1170 6167 696e 6174 655f 7175  .....paginate_qu
+000004a0: 6572 7973 6574 da0e 6765 745f 7365 7269  eryset..get_seri
+000004b0: 616c 697a 6572 da16 6765 745f 7061 6769  alizer..get_pagi
+000004c0: 6e61 7465 645f 7265 7370 6f6e 7365 da04  nated_response..
+000004d0: 6461 7461 7209 0000 0072 0700 0000 da0b  datar....r......
+000004e0: 4854 5450 5f32 3030 5f4f 4b29 0572 1500  HTTP_200_OK).r..
+000004f0: 0000 7212 0000 00da 0871 7565 7279 7365  ..r......queryse
+00000500: 74da 0470 6167 6572 1b00 0000 7217 0000  t..pager....r...
+00000510: 0072 1700 0000 7218 0000 00da 1267 6574  .r....r......get
+00000520: 5f75 7365 725f 6661 766f 7269 7465 7322  _user_favorites"
+00000530: 0000 0073 0e00 0000 0002 0e02 0a01 0801  ...s............
+00000540: 0e01 0c02 0e01 7a22 4661 766f 7269 7465  ......z"Favorite
+00000550: 5669 6577 5365 742e 6765 745f 7573 6572  ViewSet.get_user
+00000560: 5f66 6176 6f72 6974 6573 4e29 09da 085f  _favoritesN)..._
+00000570: 5f6e 616d 655f 5fda 0a5f 5f6d 6f64 756c  _name__..__modul
+00000580: 655f 5fda 0c5f 5f71 7561 6c6e 616d 655f  e__..__qualname_
+00000590: 5f72 0c00 0000 da10 7365 7269 616c 697a  _r......serializ
+000005a0: 6572 5f63 6c61 7373 7219 0000 0072 1c00  er_classr....r..
+000005b0: 0000 7208 0000 0072 2b00 0000 7217 0000  ..r....r+...r...
+000005c0: 0072 1700 0000 7217 0000 0072 1800 0000  .r....r....r....
+000005d0: 720e 0000 000c 0000 0073 0a00 0000 0808  r........s......
+000005e0: 0402 0806 0806 0e01 720e 0000 004e 2916  ........r....N).
+000005f0: da15 6472 665f 7370 6563 7461 6375 6c61  ..drf_spectacula
+00000600: 722e 7574 696c 7372 0200 0000 da12 6761  r.utilsr......ga
+00000610: 7270 6978 5f75 7365 722e 6d6f 6465 6c73  rpix_user.models
+00000620: 7203 0000 00da 2167 6172 7069 785f 7573  r.....!garpix_us
+00000630: 6572 2e75 7469 6c73 2e64 7266 5f73 7065  er.utils.drf_spe
+00000640: 6374 6163 756c 6172 7204 0000 00da 0e72  ctacularr......r
+00000650: 6573 745f 6672 616d 6577 6f72 6b72 0500  est_frameworkr..
+00000660: 0000 7206 0000 0072 0700 0000 da19 7265  ..r....r......re
+00000670: 7374 5f66 7261 6d65 776f 726b 2e64 6563  st_framework.dec
+00000680: 6f72 6174 6f72 7372 0800 0000 da17 7265  oratorsr......re
+00000690: 7374 5f66 7261 6d65 776f 726b 2e72 6573  st_framework.res
+000006a0: 706f 6e73 6572 0900 0000 da06 6d6f 6465  ponser......mode
+000006b0: 6c73 720b 0000 00da 0b73 6572 6961 6c69  lsr......seriali
+000006c0: 7a65 7273 720c 0000 00da 1043 7265 6174  zersr......Creat
+000006d0: 654d 6f64 656c 4d69 7869 6eda 1144 6573  eModelMixin..Des
+000006e0: 7472 6f79 4d6f 6465 6c4d 6978 696e da0e  troyModelMixin..
+000006f0: 4765 6e65 7269 6356 6965 7753 6574 720e  GenericViewSetr.
+00000700: 0000 0072 1700 0000 7217 0000 0072 1700  ...r....r....r..
+00000710: 0000 7218 0000 00da 083c 6d6f 6475 6c65  ..r......<module
+00000720: 3e01 0000 0073 1e00 0000 0c01 0c01 0c01  >....s..........
+00000730: 1401 0c01 0c02 0c01 0c03 0202 04ff 02ff  ................
+00000740: 0405 0e01 0401 04fe                      ........
```

### Comparing `garpix_favourite-2.0.0/garpix_favourite/models.py` & `garpix_favourite-2.1.0/garpix_favourite/models.py`

 * *Files 26% similar despite different names*

```diff
@@ -8,32 +8,60 @@
 class Favorite(models.Model):
     """
         Модель "Избранное" для пользователя.
     """
 
     user_session = models.ForeignKey(
         UserSession, on_delete=models.CASCADE, verbose_name=_('User'),
-        related_name='favorites', editable=False
+        related_name='favorites'
     )
     object_id = models.PositiveIntegerField(
         verbose_name=_('Object ID')
     )
     content_type = models.ForeignKey(
-        ContentType, on_delete=models.CASCADE, verbose_name=_('Content type'),
-        editable=False,
+        ContentType, on_delete=models.CASCADE, verbose_name=_('Content type')
     )
     content_object = GenericForeignKey(
         'content_type', 'object_id'
     )
     created_at = models.DateTimeField(
         auto_now_add=True, verbose_name=_('Created at')
     )
 
+    @property
+    def entity(self):
+        return self.content_type.get_object_for_this_type(pk=self.object_id)
+
+    @classmethod
+    def get_favorite_by_request(cls, request):
+        user_session = UserSession.get_from_request(request)
+        elements = Favorite.objects.filter(
+            user_session=user_session
+        )
+
+        return elements
+
+    @classmethod
+    def get_entity_by_request(cls, request, obj_id, model_name):
+        """
+        Will return the favorite entities for the current user or None
+        """
+        elements = cls.get_favorite_by_request(request)
+        model_type = ContentType.objects.filter(model=model_name).first()
+        if model_type is None:
+            return None
+        el = elements.filter(
+            object_id=obj_id,
+            content_type__pk=model_type.pk,
+        ).first()
+
+        return el
+
     def __str__(self):
-        return 'User %i | Favorite: %s %s' % (
+        return 'User session %i | Favorite: %s %s' % (
             self.user_session.id, self.object_id, self.content_object.__class__.__name__
         )
 
     class Meta:
         ordering = ('id',)
         verbose_name = _('Favorite')
         verbose_name_plural = _('Favorites')
```

### Comparing `garpix_favourite-2.0.0/garpix_favourite/serializers.py` & `garpix_favourite-2.1.0/garpix_favourite/serializers.py`

 * *Files 5% similar despite different names*

```diff
@@ -35,14 +35,16 @@
     model_name = serializers.CharField(
         required=True, write_only=True, max_length=100
     )
     favorite_url = serializers.SerializerMethodField(
         read_only=True
     )
 
+    content_type = serializers.HiddenField(default=None)
+
     def _get_request(self):
         return self.context.get('request')
 
     def get_favorite_url(self, instance) -> Optional[str]:
         """
             Возвращает полный путь до объекта content_object.
         """
```

### Comparing `garpix_favourite-2.0.0/garpix_favourite/setup.py` & `garpix_favourite-2.1.0/garpix_favourite/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 here = path.join(path.abspath(path.dirname(__file__)), 'garpix_favourite')
 
 with open(path.join(here, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='garpix_favourite',
-    version='2.0.0',
+    version='2.1.0',
     description='',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/garpixcms/garpix_favourite',
     author='Garpix LTD',
     author_email='info@garpix.com',
     license='MIT',
```

### Comparing `garpix_favourite-2.0.0/garpix_favourite/tests.py` & `garpix_favourite-2.1.0/garpix_favourite/tests.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,63 +1,66 @@
+import uuid
 from django.conf import settings
 from django.contrib.auth import get_user_model
 from django.urls import reverse
+from django.contrib.contenttypes.models import ContentType
 
 from rest_framework import status
 from rest_framework.authtoken.models import Token
 from rest_framework.test import APITestCase
+from .models import Favorite
+from garpix_user.models import UserSession
 
 User = get_user_model()
 
 
 class FavoriteTestCase(APITestCase):
     def setUp(self) -> None:
         self.password = '12345'
         self.username = 'test'
 
+        self.username2 = 'test2'
+
         self.user = User.objects.create_user(username=self.username, email='user@site.com', password=self.password)
+        self.user2 = User.objects.create_user(username=self.username2, email='user2@site.com', password=self.password)
         self.token = Token.objects.create(user=self.user)
-        self.favorite_url = reverse('favorite-list')
+        self.favorite_url = reverse('garpix_favourite:favorite-list')
+        self.favorite_url_user = reverse('garpix_favourite:favorite-get-user-favorites')
+
+        session_key = uuid.uuid4()
+
+        self.header = {'HTTP_USER_SESSION_TOKEN': str(session_key)}
+
+        self.user_session = UserSession.objects.create(user=self.user, token_number=session_key)
+        model_type = ContentType.objects.get_for_model(User)
 
-    def test_user_favorite_list_as_unauthorized(self):
-        response = self.client.get(self.favorite_url)
+        self.favorite = Favorite.objects.create(
+            user_session=self.user_session,
+            object_id=self.user.pk,
+            content_type=model_type
+        )
 
-        self.assertEqual(response.status_code, status.HTTP_401_UNAUTHORIZED)
-        self.assertDictEqual(response.json(), {'detail': 'Учетные данные не были предоставлены.'})
+    def test_entity(self):
+        self.assertEqual(self.favorite.entity.pk, self.user.pk)
 
-    def test_create_favorite_as_authorized(self):
+    def test_create_favorite(self):
         settings.ACCEPTED_FAVORITE_MODELS += ['User']
-        self._make_authentication()
 
         data = {
-            'object_id': 1,
+            'object_id': self.user2.pk,
             'model_name': 'User'
         }
 
-        response = self.client.post(self.favorite_url, data=data)
+        response = self.client.post(self.favorite_url, data=data, **self.header)
         response_json = response.json()
-        response_json.pop('created_at')
+        print(response_json, 'response_json')
 
         self.assertEqual(response.status_code, status.HTTP_201_CREATED)
-        self.assertDictEqual(response_json, {'id': 1, 'object_id': 1, 'favorite_url': None, 'content_type': 33})
 
-    def test_create_favorite_as_unauthorized(self):
-        response = self.client.post(self.favorite_url)
-
-        self.assertEqual(response.status_code, status.HTTP_401_UNAUTHORIZED)
-
-    def _make_authentication(self) -> None:
-        if settings.ENABLE_GARPIX_AUTH:
-            response = self.client.post(
-                reverse('garpix_auth:api_login'),
-                {
-                    'username': self.username,
-                    'password': self.password,
-                },
-                HTTP_ACCEPT='application/json'
-            )
+    def test_favorite_list(self):
+        settings.ACCEPTED_FAVORITE_MODELS += ['User']
 
-            access_token = response.json()['access_token']
-            self.client.credentials(HTTP_AUTHORIZATION='Bearer ' + access_token)
+        response = self.client.get(self.favorite_url_user, **self.header)
+        response_json = response.json()
+        self.assertEqual(len(response_json), 1)
 
-        else:
-            self.client.credentials(HTTP_AUTHORIZATION='Token ' + self.token.key)
+        self.assertEqual(response.status_code, status.HTTP_200_OK)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `garpix_favourite-2.0.0/garpix_favourite/utils.py` & `garpix_favourite-2.1.0/garpix_favourite/utils.py`

 * *Files identical despite different names*

### Comparing `garpix_favourite-2.0.0/garpix_favourite/views.py` & `garpix_favourite-2.1.0/garpix_favourite/views.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from drf_spectacular.utils import extend_schema
 from garpix_user.models import UserSession
 from garpix_user.utils.drf_spectacular import user_session_token_header_parameter
 from rest_framework import viewsets, mixins, status
 from rest_framework.decorators import action
-from rest_framework.permissions import IsAuthenticated
 from rest_framework.response import Response
 
 from .models import Favorite
 from .serializers import FavoriteSerializer
 
 
 @extend_schema(
@@ -17,21 +16,21 @@
 )
 class FavoriteViewSet(mixins.CreateModelMixin,
                       mixins.DestroyModelMixin,
                       viewsets.GenericViewSet):
     serializer_class = FavoriteSerializer
 
     def get_queryset(self):
-        user = UserSession.get_or_create_user_session(self.request)
+        user = UserSession.get_from_request(self.request)
         return Favorite.objects.filter(
             user_session=user
         )
 
     def perform_create(self, serializer):
-        user = UserSession.get_or_create_user_session(self.request)
+        user = UserSession.get_from_request(self.request)
         serializer.save(
             user_session=user
         )
 
     @action(methods=['GET'], detail=False, url_path='current')
     def get_user_favorites(self, request):
         queryset = self.filter_queryset(self.get_queryset())
```

### Comparing `garpix_favourite-2.0.0/garpix_favourite.egg-info/PKG-INFO` & `garpix_favourite-2.1.0/garpix_favourite.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: garpix-favourite
-Version: 2.0.0
+Version: 2.1.0
 Home-page: https://github.com/garpixcms/garpix_favourite
 Author: Garpix LTD
 Author-email: info@garpix.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
```

### Comparing `garpix_favourite-2.0.0/garpix_favourite.egg-info/SOURCES.txt` & `garpix_favourite-2.1.0/garpix_favourite.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -22,8 +22,12 @@
 garpix_favourite.egg-info/top_level.txt
 garpix_favourite/__pycache__/__init__.cpython-38.pyc
 garpix_favourite/__pycache__/apps.cpython-38.pyc
 garpix_favourite/__pycache__/models.cpython-38.pyc
 garpix_favourite/__pycache__/routers.cpython-38.pyc
 garpix_favourite/__pycache__/serializers.cpython-38.pyc
 garpix_favourite/__pycache__/urls.cpython-38.pyc
-garpix_favourite/__pycache__/views.cpython-38.pyc
+garpix_favourite/__pycache__/views.cpython-38.pyc
+garpix_favourite/admin/__init__.py
+garpix_favourite/admin/favorite.py
+garpix_favourite/admin/__pycache__/__init__.cpython-38.pyc
+garpix_favourite/admin/__pycache__/favorite.cpython-38.pyc
```

### Comparing `garpix_favourite-2.0.0/setup.py` & `garpix_favourite-2.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 here = path.join(path.abspath(path.dirname(__file__)), 'garpix_favourite')
 
 with open(path.join(here, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='garpix_favourite',
-    version='2.0.0',
+    version='2.1.0',
     description='',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/garpixcms/garpix_favourite',
     author='Garpix LTD',
     author_email='info@garpix.com',
     license='MIT',
```

