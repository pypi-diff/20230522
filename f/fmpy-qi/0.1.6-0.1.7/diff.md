# Comparing `tmp/fmpy_qi-0.1.6.tar.gz` & `tmp/fmpy_qi-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fmpy_qi-0.1.6.tar", last modified: Fri May 19 15:35:04 2023, max compression
+gzip compressed data, was "fmpy_qi-0.1.7.tar", last modified: Mon May 22 19:23:45 2023, max compression
```

## Comparing `fmpy_qi-0.1.6.tar` & `fmpy_qi-0.1.7.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 nicolasthiery   (501) staff       (20)        0 2023-05-19 15:35:04.209633 fmpy_qi-0.1.6/
--rw-r--r--   0 nicolasthiery   (501) staff       (20)     1064 2023-04-22 15:25:00.000000 fmpy_qi-0.1.6/LICENSE
--rw-r--r--   0 nicolasthiery   (501) staff       (20)     2751 2023-05-19 15:35:04.209276 fmpy_qi-0.1.6/PKG-INFO
--rw-r--r--   0 nicolasthiery   (501) staff       (20)     2219 2023-05-14 19:24:52.000000 fmpy_qi-0.1.6/README.md
--rw-r--r--   0 nicolasthiery   (501) staff       (20)      741 2023-05-19 15:33:06.000000 fmpy_qi-0.1.6/pyproject.toml
--rw-r--r--   0 nicolasthiery   (501) staff       (20)       38 2023-05-19 15:35:04.209746 fmpy_qi-0.1.6/setup.cfg
-drwxr-xr-x   0 nicolasthiery   (501) staff       (20)        0 2023-05-19 15:35:04.204294 fmpy_qi-0.1.6/src/
--rw-r--r--   0 nicolasthiery   (501) staff       (20)        0 2023-04-30 21:24:30.000000 fmpy_qi-0.1.6/src/__init__.py
-drwxr-xr-x   0 nicolasthiery   (501) staff       (20)        0 2023-05-19 15:35:04.205575 fmpy_qi-0.1.6/src/fmpy/
--rw-r--r--   0 nicolasthiery   (501) staff       (20)        0 2023-04-22 15:25:28.000000 fmpy_qi-0.1.6/src/fmpy/__init__.py
--rw-r--r--   0 nicolasthiery   (501) staff       (20)    51492 2023-05-19 15:30:39.000000 fmpy_qi-0.1.6/src/fmpy/client.py
--rw-r--r--   0 nicolasthiery   (501) staff       (20)    12276 2023-05-19 13:07:09.000000 fmpy_qi-0.1.6/src/fmpy/urls.py
--rw-r--r--   0 nicolasthiery   (501) staff       (20)      526 2023-05-14 19:02:44.000000 fmpy_qi-0.1.6/src/fmpy/utils.py
-drwxr-xr-x   0 nicolasthiery   (501) staff       (20)        0 2023-05-19 15:35:04.208793 fmpy_qi-0.1.6/src/fmpy_qi.egg-info/
--rw-r--r--   0 nicolasthiery   (501) staff       (20)     2751 2023-05-19 15:35:04.000000 fmpy_qi-0.1.6/src/fmpy_qi.egg-info/PKG-INFO
--rw-r--r--   0 nicolasthiery   (501) staff       (20)      297 2023-05-19 15:35:04.000000 fmpy_qi-0.1.6/src/fmpy_qi.egg-info/SOURCES.txt
--rw-r--r--   0 nicolasthiery   (501) staff       (20)        1 2023-05-19 15:35:04.000000 fmpy_qi-0.1.6/src/fmpy_qi.egg-info/dependency_links.txt
--rw-r--r--   0 nicolasthiery   (501) staff       (20)       46 2023-05-19 15:35:04.000000 fmpy_qi-0.1.6/src/fmpy_qi.egg-info/requires.txt
--rw-r--r--   0 nicolasthiery   (501) staff       (20)       14 2023-05-19 15:35:04.000000 fmpy_qi-0.1.6/src/fmpy_qi.egg-info/top_level.txt
+drwxr-xr-x   0 nicolasthiery   (501) staff       (20)        0 2023-05-22 19:23:45.393560 fmpy_qi-0.1.7/
+-rw-r--r--   0 nicolasthiery   (501) staff       (20)     1064 2023-04-22 15:25:00.000000 fmpy_qi-0.1.7/LICENSE
+-rw-r--r--   0 nicolasthiery   (501) staff       (20)     2751 2023-05-22 19:23:45.393105 fmpy_qi-0.1.7/PKG-INFO
+-rw-r--r--   0 nicolasthiery   (501) staff       (20)     2219 2023-05-14 19:24:52.000000 fmpy_qi-0.1.7/README.md
+-rw-r--r--   0 nicolasthiery   (501) staff       (20)      741 2023-05-22 19:21:18.000000 fmpy_qi-0.1.7/pyproject.toml
+-rw-r--r--   0 nicolasthiery   (501) staff       (20)       38 2023-05-22 19:23:45.393826 fmpy_qi-0.1.7/setup.cfg
+drwxr-xr-x   0 nicolasthiery   (501) staff       (20)        0 2023-05-22 19:23:45.386965 fmpy_qi-0.1.7/src/
+-rw-r--r--   0 nicolasthiery   (501) staff       (20)        0 2023-04-30 21:24:30.000000 fmpy_qi-0.1.7/src/__init__.py
+drwxr-xr-x   0 nicolasthiery   (501) staff       (20)        0 2023-05-22 19:23:45.389507 fmpy_qi-0.1.7/src/fmpy/
+-rw-r--r--   0 nicolasthiery   (501) staff       (20)        0 2023-04-22 15:25:28.000000 fmpy_qi-0.1.7/src/fmpy/__init__.py
+-rw-r--r--   0 nicolasthiery   (501) staff       (20)    51599 2023-05-22 19:18:40.000000 fmpy_qi-0.1.7/src/fmpy/client.py
+-rw-r--r--   0 nicolasthiery   (501) staff       (20)    12276 2023-05-19 13:07:09.000000 fmpy_qi-0.1.7/src/fmpy/urls.py
+-rw-r--r--   0 nicolasthiery   (501) staff       (20)      526 2023-05-14 19:02:44.000000 fmpy_qi-0.1.7/src/fmpy/utils.py
+drwxr-xr-x   0 nicolasthiery   (501) staff       (20)        0 2023-05-22 19:23:45.392544 fmpy_qi-0.1.7/src/fmpy_qi.egg-info/
+-rw-r--r--   0 nicolasthiery   (501) staff       (20)     2751 2023-05-22 19:23:45.000000 fmpy_qi-0.1.7/src/fmpy_qi.egg-info/PKG-INFO
+-rw-r--r--   0 nicolasthiery   (501) staff       (20)      297 2023-05-22 19:23:45.000000 fmpy_qi-0.1.7/src/fmpy_qi.egg-info/SOURCES.txt
+-rw-r--r--   0 nicolasthiery   (501) staff       (20)        1 2023-05-22 19:23:45.000000 fmpy_qi-0.1.7/src/fmpy_qi.egg-info/dependency_links.txt
+-rw-r--r--   0 nicolasthiery   (501) staff       (20)       46 2023-05-22 19:23:45.000000 fmpy_qi-0.1.7/src/fmpy_qi.egg-info/requires.txt
+-rw-r--r--   0 nicolasthiery   (501) staff       (20)       14 2023-05-22 19:23:45.000000 fmpy_qi-0.1.7/src/fmpy_qi.egg-info/top_level.txt
```

### Comparing `fmpy_qi-0.1.6/LICENSE` & `fmpy_qi-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `fmpy_qi-0.1.6/PKG-INFO` & `fmpy_qi-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fmpy_qi
-Version: 0.1.6
+Version: 0.1.7
 Summary: A python wrapper for the Financial Modeling Prep API
 Author-email: Nicolas THIERY <nicles.thiery@gmail.com>
 Project-URL: Homepage, https://github.com/NicolasThiery/fmpy
 Project-URL: Bug Tracker, https://github.com/NicolasThiery/fmpy/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `fmpy_qi-0.1.6/README.md` & `fmpy_qi-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `fmpy_qi-0.1.6/pyproject.toml` & `fmpy_qi-0.1.7/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "fmpy_qi"
-version = "0.1.6"
+version = "0.1.7"
 authors = [
   { name="Nicolas THIERY", email="nicles.thiery@gmail.com" },
 ]
 description = "A python wrapper for the Financial Modeling Prep API"
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = [
```

### Comparing `fmpy_qi-0.1.6/src/fmpy/client.py` & `fmpy_qi-0.1.7/src/fmpy/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -168,58 +168,61 @@
         for data in raw_data[::-1]:
             for item in association_dict.keys():
                 data_dict[item].append(data[association_dict[item]])
         df = pd.DataFrame.from_dict(data_dict)
         df = df.iloc[::-1]
         if datetime_index:
             df['Date'] = pd.to_datetime(df['Date'])
-        return df.set_index('Date')
+        return df.set_index('Date').drop_duplicates()
 
     def _get_historical_url(self, symbol, period, start, end):
         params = {key: val for key, val in {'from': start, 'to': end}.items() if val}
         return f'{urls.HISTORICAL_PRICE_FULL}/{symbol}?{urllib.parse.urlencode(params)}' if period == '1d' else\
                    f'{urls.HISTORICAL_CHART}/{period}/{symbol}?{urllib.parse.urlencode(params)}'
 
     def _get_batch_historical_data(self, symbol, period, start, end):
         sanitize_start = start.split(' ')[0]
         sanitize_end = end.split(' ')[0]
         target_start_datetime = datetime.strptime(sanitize_start, '%Y-%m-%d')
         _end = sanitize_end
+        prev_data = None
         batch_data = []
         loop_index = 1
         prev_start = None
         while True:
             url = self._get_historical_url(symbol, period, sanitize_start, _end)
             data = self._request(url)
-            if not data:
+            if not data or prev_data == data:
                 return batch_data
             data_list = data if isinstance(data, list) else data['historical']
             new_start = data_list[-1]['date'].split(' ')[0]
             if prev_start == new_start:
                 break
             start_index = 0
             end_index = len(data_list)-1
             end_target_datetime = datetime.strptime(start, "%Y-%m-%d %H:%M:%S")
             for i, item in enumerate(data_list):
                 date = f'{item["date"]} 00:00:00' if len(item['date'].split(' ')) == 1 else item["date"]
+                date_datetime = datetime.strptime(date, "%Y-%m-%d %H:%M:%S")
                 if loop_index == 1:
                     start_target_datetime = datetime.strptime(end, "%Y-%m-%d %H:%M:%S")
-                    if datetime.strptime(date, "%Y-%m-%d %H:%M:%S") > start_target_datetime:
+                    if date_datetime > start_target_datetime:
                         start_index += 1
-                if end_target_datetime >= datetime.strptime(date, "%Y-%m-%d %H:%M:%S"):
+                if end_target_datetime > date_datetime:
                     end_index = i
                     break
                 if item['date'].split(' ')[0] == new_start:
                     end_index = i + 1
             sanitize_data = data_list[start_index:end_index][::-1]
             batch_data = sanitize_data + batch_data
             new_start_datetime = datetime.strptime(new_start, '%Y-%m-%d')
             if new_start_datetime <= target_start_datetime:
                 break
             _end = datetime.strftime(new_start_datetime - timedelta(days=1), "%Y-%m-%d")
+            prev_data = data
             prev_start = _end
             loop_index += 1
         return batch_data
 
     def download_historical_data_to_excel(self, symbol, file, period='1d', start=None, end=None, sheet_name=None):
         """
         Description
```

### Comparing `fmpy_qi-0.1.6/src/fmpy/urls.py` & `fmpy_qi-0.1.7/src/fmpy/urls.py`

 * *Files identical despite different names*

### Comparing `fmpy_qi-0.1.6/src/fmpy/utils.py` & `fmpy_qi-0.1.7/src/fmpy/utils.py`

 * *Files identical despite different names*

### Comparing `fmpy_qi-0.1.6/src/fmpy_qi.egg-info/PKG-INFO` & `fmpy_qi-0.1.7/src/fmpy_qi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fmpy-qi
-Version: 0.1.6
+Version: 0.1.7
 Summary: A python wrapper for the Financial Modeling Prep API
 Author-email: Nicolas THIERY <nicles.thiery@gmail.com>
 Project-URL: Homepage, https://github.com/NicolasThiery/fmpy
 Project-URL: Bug Tracker, https://github.com/NicolasThiery/fmpy/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

