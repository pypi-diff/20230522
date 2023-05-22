# Comparing `tmp/xzy-db-0.0.3.tar.gz` & `tmp/xzy-db-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xzy-db-0.0.3.tar", last modified: Sun May 14 02:29:14 2023, max compression
+gzip compressed data, was "xzy-db-0.0.4.tar", last modified: Mon May 22 08:11:27 2023, max compression
```

## Comparing `xzy-db-0.0.3.tar` & `xzy-db-0.0.4.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 liubola   (1000) liubola   (1000)        0 2023-05-14 02:29:14.074061 xzy-db-0.0.3/
--rw-r--r--   0 liubola   (1000) liubola   (1000)      523 2023-05-14 02:29:14.074061 xzy-db-0.0.3/PKG-INFO
--rw-r--r--   0 liubola   (1000) liubola   (1000)       40 2023-01-13 02:27:03.000000 xzy-db-0.0.3/README.md
--rw-r--r--   0 liubola   (1000) liubola   (1000)       38 2023-05-14 02:29:14.074061 xzy-db-0.0.3/setup.cfg
--rw-r--r--   0 liubola   (1000) liubola   (1000)      914 2023-05-14 02:29:13.000000 xzy-db-0.0.3/setup.py
-drwxr-xr-x   0 liubola   (1000) liubola   (1000)        0 2023-05-14 02:29:14.074061 xzy-db-0.0.3/xzy_db/
--rw-r--r--   0 liubola   (1000) liubola   (1000)       62 2023-05-13 00:53:10.000000 xzy-db-0.0.3/xzy_db/__init__.py
-drwxr-xr-x   0 liubola   (1000) liubola   (1000)        0 2023-05-14 02:29:14.074061 xzy-db-0.0.3/xzy_db/api/
--rw-r--r--   0 liubola   (1000) liubola   (1000)      322 2023-05-13 00:53:10.000000 xzy-db-0.0.3/xzy_db/api/__init__.py
--rw-r--r--   0 liubola   (1000) liubola   (1000)     2174 2023-05-14 02:23:05.000000 xzy-db-0.0.3/xzy_db/api/get_fund_data.py
--rw-r--r--   0 liubola   (1000) liubola   (1000)     2781 2023-05-13 00:53:10.000000 xzy-db-0.0.3/xzy_db/api/get_fund_list.py
--rw-r--r--   0 liubola   (1000) liubola   (1000)     3262 2023-05-13 00:53:10.000000 xzy-db-0.0.3/xzy_db/api/get_index_data.py
--rw-r--r--   0 liubola   (1000) liubola   (1000)     2021 2023-05-13 00:53:10.000000 xzy-db-0.0.3/xzy_db/api/get_index_weight.py
--rw-r--r--   0 liubola   (1000) liubola   (1000)     4470 2023-05-13 00:53:10.000000 xzy-db-0.0.3/xzy_db/api/get_industry.py
--rw-r--r--   0 liubola   (1000) liubola   (1000)     3534 2023-05-13 12:47:07.000000 xzy-db-0.0.3/xzy_db/api/get_ret.py
--rw-r--r--   0 liubola   (1000) liubola   (1000)     5755 2023-05-13 14:28:05.000000 xzy-db-0.0.3/xzy_db/api/get_universe.py
-drwxr-xr-x   0 liubola   (1000) liubola   (1000)        0 2023-05-14 02:29:14.074061 xzy-db-0.0.3/xzy_db/crawler/
--rw-r--r--   0 liubola   (1000) liubola   (1000)       46 2023-01-13 02:27:03.000000 xzy-db-0.0.3/xzy_db/crawler/__init__.py
-drwxr-xr-x   0 liubola   (1000) liubola   (1000)        0 2023-05-14 02:29:14.074061 xzy-db-0.0.3/xzy_db/crawler/futures/
--rw-r--r--   0 liubola   (1000) liubola   (1000)        0 2023-01-13 02:27:03.000000 xzy-db-0.0.3/xzy_db/crawler/futures/__init__.py
--rw-r--r--   0 liubola   (1000) liubola   (1000)    17469 2023-05-13 00:53:10.000000 xzy-db-0.0.3/xzy_db/crawler/futures/domestic.py
--rw-r--r--   0 liubola   (1000) liubola   (1000)     5254 2023-01-13 02:27:03.000000 xzy-db-0.0.3/xzy_db/crawler/futures/domestic_cons.py
-drwxr-xr-x   0 liubola   (1000) liubola   (1000)        0 2023-05-14 02:29:14.074061 xzy-db-0.0.3/xzy_db/hk_sangreal_calendar/
--rw-r--r--   0 liubola   (1000) liubola   (1000)      399 2023-05-13 00:53:10.000000 xzy-db-0.0.3/xzy_db/hk_sangreal_calendar/__init__.py
-drwxr-xr-x   0 liubola   (1000) liubola   (1000)        0 2023-05-14 02:29:14.074061 xzy-db-0.0.3/xzy_db/sangreal_calendar/
--rw-r--r--   0 liubola   (1000) liubola   (1000)      397 2023-05-13 12:44:00.000000 xzy-db-0.0.3/xzy_db/sangreal_calendar/__init__.py
-drwxr-xr-x   0 liubola   (1000) liubola   (1000)        0 2023-05-14 02:29:14.074061 xzy-db-0.0.3/xzy_db/utils/
--rw-r--r--   0 liubola   (1000) liubola   (1000)      112 2023-05-13 00:53:10.000000 xzy-db-0.0.3/xzy_db/utils/__init__.py
--rw-r--r--   0 liubola   (1000) liubola   (1000)     2277 2023-03-30 06:40:40.000000 xzy-db-0.0.3/xzy_db/utils/commons.py
--rw-r--r--   0 liubola   (1000) liubola   (1000)       93 2023-01-13 02:27:03.000000 xzy-db-0.0.3/xzy_db/utils/datetime_handle.py
--rw-r--r--   0 liubola   (1000) liubola   (1000)     2436 2023-05-13 12:36:51.000000 xzy-db-0.0.3/xzy_db/utils/engines.py
--rw-r--r--   0 liubola   (1000) liubola   (1000)      419 2023-01-13 02:27:03.000000 xzy-db-0.0.3/xzy_db/utils/fund_type.py
-drwxr-xr-x   0 liubola   (1000) liubola   (1000)        0 2023-05-14 02:29:14.074061 xzy-db-0.0.3/xzy_db.egg-info/
--rw-r--r--   0 liubola   (1000) liubola   (1000)      523 2023-05-14 02:29:13.000000 xzy-db-0.0.3/xzy_db.egg-info/PKG-INFO
--rw-r--r--   0 liubola   (1000) liubola   (1000)      746 2023-05-14 02:29:13.000000 xzy-db-0.0.3/xzy_db.egg-info/SOURCES.txt
--rw-r--r--   0 liubola   (1000) liubola   (1000)        1 2023-05-14 02:29:13.000000 xzy-db-0.0.3/xzy_db.egg-info/dependency_links.txt
--rw-r--r--   0 liubola   (1000) liubola   (1000)       55 2023-05-14 02:29:13.000000 xzy-db-0.0.3/xzy_db.egg-info/requires.txt
--rw-r--r--   0 liubola   (1000) liubola   (1000)        7 2023-05-14 02:29:13.000000 xzy-db-0.0.3/xzy_db.egg-info/top_level.txt
+drwxr-xr-x   0 liubola   (1000) liubola   (1000)        0 2023-05-22 08:11:27.029255 xzy-db-0.0.4/
+-rw-r--r--   0 liubola   (1000) liubola   (1000)      523 2023-05-22 08:11:27.029255 xzy-db-0.0.4/PKG-INFO
+-rw-r--r--   0 liubola   (1000) liubola   (1000)       40 2023-05-22 08:05:17.000000 xzy-db-0.0.4/README.md
+-rw-r--r--   0 liubola   (1000) liubola   (1000)       38 2023-05-22 08:11:27.029255 xzy-db-0.0.4/setup.cfg
+-rw-r--r--   0 liubola   (1000) liubola   (1000)      914 2023-05-22 08:11:26.000000 xzy-db-0.0.4/setup.py
+drwxr-xr-x   0 liubola   (1000) liubola   (1000)        0 2023-05-22 08:11:27.019255 xzy-db-0.0.4/xzy_db/
+-rw-r--r--   0 liubola   (1000) liubola   (1000)       62 2023-05-22 08:05:17.000000 xzy-db-0.0.4/xzy_db/__init__.py
+drwxr-xr-x   0 liubola   (1000) liubola   (1000)        0 2023-05-22 08:11:27.019255 xzy-db-0.0.4/xzy_db/api/
+-rw-r--r--   0 liubola   (1000) liubola   (1000)      322 2023-05-22 08:05:17.000000 xzy-db-0.0.4/xzy_db/api/__init__.py
+-rw-r--r--   0 liubola   (1000) liubola   (1000)     2174 2023-05-22 08:05:17.000000 xzy-db-0.0.4/xzy_db/api/get_fund_data.py
+-rw-r--r--   0 liubola   (1000) liubola   (1000)     2781 2023-05-22 08:05:17.000000 xzy-db-0.0.4/xzy_db/api/get_fund_list.py
+-rw-r--r--   0 liubola   (1000) liubola   (1000)     3262 2023-05-22 08:05:17.000000 xzy-db-0.0.4/xzy_db/api/get_index_data.py
+-rw-r--r--   0 liubola   (1000) liubola   (1000)     2021 2023-05-22 08:05:17.000000 xzy-db-0.0.4/xzy_db/api/get_index_weight.py
+-rw-r--r--   0 liubola   (1000) liubola   (1000)     4470 2023-05-22 08:05:17.000000 xzy-db-0.0.4/xzy_db/api/get_industry.py
+-rw-r--r--   0 liubola   (1000) liubola   (1000)     3534 2023-05-22 08:05:17.000000 xzy-db-0.0.4/xzy_db/api/get_ret.py
+-rw-r--r--   0 liubola   (1000) liubola   (1000)     5820 2023-05-22 08:10:07.000000 xzy-db-0.0.4/xzy_db/api/get_universe.py
+drwxr-xr-x   0 liubola   (1000) liubola   (1000)        0 2023-05-22 08:11:27.019255 xzy-db-0.0.4/xzy_db/crawler/
+-rw-r--r--   0 liubola   (1000) liubola   (1000)       46 2023-05-22 08:05:17.000000 xzy-db-0.0.4/xzy_db/crawler/__init__.py
+drwxr-xr-x   0 liubola   (1000) liubola   (1000)        0 2023-05-22 08:11:27.029255 xzy-db-0.0.4/xzy_db/crawler/futures/
+-rw-r--r--   0 liubola   (1000) liubola   (1000)        0 2023-05-22 08:05:17.000000 xzy-db-0.0.4/xzy_db/crawler/futures/__init__.py
+-rw-r--r--   0 liubola   (1000) liubola   (1000)    17469 2023-05-22 08:05:17.000000 xzy-db-0.0.4/xzy_db/crawler/futures/domestic.py
+-rw-r--r--   0 liubola   (1000) liubola   (1000)     5254 2023-05-22 08:05:17.000000 xzy-db-0.0.4/xzy_db/crawler/futures/domestic_cons.py
+drwxr-xr-x   0 liubola   (1000) liubola   (1000)        0 2023-05-22 08:11:27.029255 xzy-db-0.0.4/xzy_db/hk_sangreal_calendar/
+-rw-r--r--   0 liubola   (1000) liubola   (1000)      399 2023-05-22 08:05:17.000000 xzy-db-0.0.4/xzy_db/hk_sangreal_calendar/__init__.py
+drwxr-xr-x   0 liubola   (1000) liubola   (1000)        0 2023-05-22 08:11:27.029255 xzy-db-0.0.4/xzy_db/sangreal_calendar/
+-rw-r--r--   0 liubola   (1000) liubola   (1000)      397 2023-05-22 08:05:17.000000 xzy-db-0.0.4/xzy_db/sangreal_calendar/__init__.py
+drwxr-xr-x   0 liubola   (1000) liubola   (1000)        0 2023-05-22 08:11:27.029255 xzy-db-0.0.4/xzy_db/utils/
+-rw-r--r--   0 liubola   (1000) liubola   (1000)      112 2023-05-22 08:05:17.000000 xzy-db-0.0.4/xzy_db/utils/__init__.py
+-rw-r--r--   0 liubola   (1000) liubola   (1000)     2277 2023-05-22 08:05:17.000000 xzy-db-0.0.4/xzy_db/utils/commons.py
+-rw-r--r--   0 liubola   (1000) liubola   (1000)       93 2023-05-22 08:05:17.000000 xzy-db-0.0.4/xzy_db/utils/datetime_handle.py
+-rw-r--r--   0 liubola   (1000) liubola   (1000)     2436 2023-05-22 08:05:17.000000 xzy-db-0.0.4/xzy_db/utils/engines.py
+-rw-r--r--   0 liubola   (1000) liubola   (1000)      419 2023-05-22 08:05:17.000000 xzy-db-0.0.4/xzy_db/utils/fund_type.py
+drwxr-xr-x   0 liubola   (1000) liubola   (1000)        0 2023-05-22 08:11:27.019255 xzy-db-0.0.4/xzy_db.egg-info/
+-rw-r--r--   0 liubola   (1000) liubola   (1000)      523 2023-05-22 08:11:26.000000 xzy-db-0.0.4/xzy_db.egg-info/PKG-INFO
+-rw-r--r--   0 liubola   (1000) liubola   (1000)      746 2023-05-22 08:11:26.000000 xzy-db-0.0.4/xzy_db.egg-info/SOURCES.txt
+-rw-r--r--   0 liubola   (1000) liubola   (1000)        1 2023-05-22 08:11:26.000000 xzy-db-0.0.4/xzy_db.egg-info/dependency_links.txt
+-rw-r--r--   0 liubola   (1000) liubola   (1000)       55 2023-05-22 08:11:26.000000 xzy-db-0.0.4/xzy_db.egg-info/requires.txt
+-rw-r--r--   0 liubola   (1000) liubola   (1000)        7 2023-05-22 08:11:26.000000 xzy-db-0.0.4/xzy_db.egg-info/top_level.txt
```

### Comparing `xzy-db-0.0.3/PKG-INFO` & `xzy-db-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: xzy-db
-Version: 0.0.3
+Version: 0.0.4
 Summary: short cut api for wind
 Home-page: https://gitee.com/liubola/xzy-db
 Author: liubola
 Author-email: lby3523@gmail.com
 License: GNU General Public License v3.0
 Description: UNKNOWN
 Platform: all
```

### Comparing `xzy-db-0.0.3/setup.py` & `xzy-db-0.0.4/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from setuptools import setup, find_packages
 
 setup(
     name='xzy-db',
-    version='0.0.3',
+    version='0.0.4',
     description=('short cut api for wind'),
     install_requires=[
         'sangreal-db',
-        'sangreal-calendar >= 0.0.36',
+        'sangreal-calendar >= 0.0.46',
         'sqlalchemy',
         'attrs',
     ],
     # long_description=open('README.rst').read(),
     author='liubola',
     author_email='lby3523@gmail.com',
     # maintainer='<维护人员的名字>',
```

### Comparing `xzy-db-0.0.3/xzy_db/api/get_fund_data.py` & `xzy-db-0.0.4/xzy_db/api/get_fund_data.py`

 * *Files identical despite different names*

### Comparing `xzy-db-0.0.3/xzy_db/api/get_fund_list.py` & `xzy-db-0.0.4/xzy_db/api/get_fund_list.py`

 * *Files identical despite different names*

### Comparing `xzy-db-0.0.3/xzy_db/api/get_index_data.py` & `xzy-db-0.0.4/xzy_db/api/get_index_data.py`

 * *Files identical despite different names*

### Comparing `xzy-db-0.0.3/xzy_db/api/get_index_weight.py` & `xzy-db-0.0.4/xzy_db/api/get_index_weight.py`

 * *Files identical despite different names*

### Comparing `xzy-db-0.0.3/xzy_db/api/get_industry.py` & `xzy-db-0.0.4/xzy_db/api/get_industry.py`

 * *Files identical despite different names*

### Comparing `xzy-db-0.0.3/xzy_db/api/get_ret.py` & `xzy-db-0.0.4/xzy_db/api/get_ret.py`

 * *Files identical despite different names*

### Comparing `xzy-db-0.0.3/xzy_db/api/get_universe.py` & `xzy-db-0.0.4/xzy_db/api/get_universe.py`

 * *Files 2% similar despite different names*

```diff
@@ -187,15 +187,16 @@
             df = get_all_bond()
         elif self.index.endswith('HI'):
             df = get_all_hk(self.index)
         elif self.index != '':
             df = get_all_normal_index(self.index)
 
         trade_dt = dt_handle(trade_dt)
-        trade_dt = int(trade_dt)
+        if isinstance(df['entry_dt'].dropna().iloc[0], int):
+            trade_dt = int(trade_dt)
         df = df.loc[(df['entry_dt'] <= trade_dt) & (
             (df['out_dt'] >= trade_dt) | (df['out_dt'].isnull()))]
         return set(df.sid)
 
 
 if __name__ == '__main__':
     f_list = DynamicUniverse('HS300').preview('20180105')
```

### Comparing `xzy-db-0.0.3/xzy_db/crawler/futures/domestic.py` & `xzy-db-0.0.4/xzy_db/crawler/futures/domestic.py`

 * *Files identical despite different names*

### Comparing `xzy-db-0.0.3/xzy_db/crawler/futures/domestic_cons.py` & `xzy-db-0.0.4/xzy_db/crawler/futures/domestic_cons.py`

 * *Files identical despite different names*

### Comparing `xzy-db-0.0.3/xzy_db/utils/commons.py` & `xzy-db-0.0.4/xzy_db/utils/commons.py`

 * *Files identical despite different names*

### Comparing `xzy-db-0.0.3/xzy_db/utils/engines.py` & `xzy-db-0.0.4/xzy_db/utils/engines.py`

 * *Files identical despite different names*

### Comparing `xzy-db-0.0.3/xzy_db.egg-info/PKG-INFO` & `xzy-db-0.0.4/xzy_db.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: xzy-db
-Version: 0.0.3
+Version: 0.0.4
 Summary: short cut api for wind
 Home-page: https://gitee.com/liubola/xzy-db
 Author: liubola
 Author-email: lby3523@gmail.com
 License: GNU General Public License v3.0
 Description: UNKNOWN
 Platform: all
```

### Comparing `xzy-db-0.0.3/xzy_db.egg-info/SOURCES.txt` & `xzy-db-0.0.4/xzy_db.egg-info/SOURCES.txt`

 * *Files identical despite different names*

