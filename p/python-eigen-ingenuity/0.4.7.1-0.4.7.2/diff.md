# Comparing `tmp/python-eigen-ingenuity-0.4.7.1.tar.gz` & `tmp/python-eigen-ingenuity-0.4.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-eigen-ingenuity-0.4.7.1.tar", last modified: Wed May 17 14:56:58 2023, max compression
+gzip compressed data, was "python-eigen-ingenuity-0.4.7.2.tar", last modified: Mon May 22 09:52:48 2023, max compression
```

## Comparing `python-eigen-ingenuity-0.4.7.1.tar` & `python-eigen-ingenuity-0.4.7.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 berhic     (501) staff       (20)        0 2023-05-17 14:56:58.463388 python-eigen-ingenuity-0.4.7.1/
--rw-r--r--   0 berhic     (501) staff       (20)      578 2022-08-16 09:33:43.000000 python-eigen-ingenuity-0.4.7.1/LICENSE
--rw-r--r--   0 berhic     (501) staff       (20)       70 2022-11-30 15:55:19.000000 python-eigen-ingenuity-0.4.7.1/MANIFEST.in
--rw-r--r--   0 berhic     (501) staff       (20)    11665 2023-05-17 14:56:58.463167 python-eigen-ingenuity-0.4.7.1/PKG-INFO
--rw-r--r--   0 berhic     (501) staff       (20)    11343 2022-08-16 09:33:43.000000 python-eigen-ingenuity-0.4.7.1/README.md
-drwxr-xr-x   0 berhic     (501) staff       (20)        0 2023-05-17 14:56:58.461864 python-eigen-ingenuity-0.4.7.1/eigeningenuity/
--rw-r--r--   0 berhic     (501) staff       (20)     1203 2023-04-06 15:03:48.000000 python-eigen-ingenuity-0.4.7.1/eigeningenuity/__init__.py
--rw-r--r--   0 berhic     (501) staff       (20)    15882 2023-05-17 13:44:01.000000 python-eigen-ingenuity-0.4.7.1/eigeningenuity/assetmodel.py
-drwxr-xr-x   0 berhic     (501) staff       (20)        0 2023-05-17 14:56:58.462176 python-eigen-ingenuity-0.4.7.1/eigeningenuity/core/
--rw-r--r--   0 berhic     (501) staff       (20)     7715 2023-04-06 10:18:46.000000 python-eigen-ingenuity-0.4.7.1/eigeningenuity/core/__init__.py
--rw-r--r--   0 berhic     (501) staff       (20)     1146 2022-08-16 09:33:43.000000 python-eigen-ingenuity-0.4.7.1/eigeningenuity/core/debug.py
--rw-r--r--   0 berhic     (501) staff       (20)     6250 2023-05-17 13:22:24.000000 python-eigen-ingenuity-0.4.7.1/eigeningenuity/elastic.py
--rw-r--r--   0 berhic     (501) staff       (20)     3054 2023-05-17 13:22:33.000000 python-eigen-ingenuity-0.4.7.1/eigeningenuity/events.py
--rw-r--r--   0 berhic     (501) staff       (20)    36199 2023-05-17 13:47:31.000000 python-eigen-ingenuity-0.4.7.1/eigeningenuity/historian.py
--rw-r--r--   0 berhic     (501) staff       (20)     2843 2023-05-17 13:22:46.000000 python-eigen-ingenuity-0.4.7.1/eigeningenuity/smartdash.py
--rw-r--r--   0 berhic     (501) staff       (20)     4081 2023-05-17 13:22:51.000000 python-eigen-ingenuity-0.4.7.1/eigeningenuity/sql.py
--rw-r--r--   0 berhic     (501) staff       (20)    11952 2023-05-17 14:56:30.000000 python-eigen-ingenuity-0.4.7.1/eigeningenuity/util.py
--rw-r--r--   0 berhic     (501) staff       (20)       92 2022-08-16 09:33:43.000000 python-eigen-ingenuity-0.4.7.1/pyproject.toml
-drwxr-xr-x   0 berhic     (501) staff       (20)        0 2023-05-17 14:56:58.462955 python-eigen-ingenuity-0.4.7.1/python_eigen_ingenuity.egg-info/
--rw-r--r--   0 berhic     (501) staff       (20)    11665 2023-05-17 14:56:58.000000 python-eigen-ingenuity-0.4.7.1/python_eigen_ingenuity.egg-info/PKG-INFO
--rw-r--r--   0 berhic     (501) staff       (20)      551 2023-05-17 14:56:58.000000 python-eigen-ingenuity-0.4.7.1/python_eigen_ingenuity.egg-info/SOURCES.txt
--rw-r--r--   0 berhic     (501) staff       (20)        1 2023-05-17 14:56:58.000000 python-eigen-ingenuity-0.4.7.1/python_eigen_ingenuity.egg-info/dependency_links.txt
--rw-r--r--   0 berhic     (501) staff       (20)       24 2023-05-17 14:56:58.000000 python-eigen-ingenuity-0.4.7.1/python_eigen_ingenuity.egg-info/requires.txt
--rw-r--r--   0 berhic     (501) staff       (20)       15 2023-05-17 14:56:58.000000 python-eigen-ingenuity-0.4.7.1/python_eigen_ingenuity.egg-info/top_level.txt
--rw-r--r--   0 berhic     (501) staff       (20)       38 2023-05-17 14:56:58.463441 python-eigen-ingenuity-0.4.7.1/setup.cfg
--rw-r--r--   0 berhic     (501) staff       (20)      691 2023-05-17 14:56:45.000000 python-eigen-ingenuity-0.4.7.1/setup.py
+drwxr-xr-x   0 berhic     (501) staff       (20)        0 2023-05-22 09:52:48.960212 python-eigen-ingenuity-0.4.7.2/
+-rw-r--r--   0 berhic     (501) staff       (20)      578 2022-08-16 09:33:43.000000 python-eigen-ingenuity-0.4.7.2/LICENSE
+-rw-r--r--   0 berhic     (501) staff       (20)       70 2022-11-30 15:55:19.000000 python-eigen-ingenuity-0.4.7.2/MANIFEST.in
+-rw-r--r--   0 berhic     (501) staff       (20)    11665 2023-05-22 09:52:48.959975 python-eigen-ingenuity-0.4.7.2/PKG-INFO
+-rw-r--r--   0 berhic     (501) staff       (20)    11343 2022-08-16 09:33:43.000000 python-eigen-ingenuity-0.4.7.2/README.md
+drwxr-xr-x   0 berhic     (501) staff       (20)        0 2023-05-22 09:52:48.958306 python-eigen-ingenuity-0.4.7.2/eigeningenuity/
+-rw-r--r--   0 berhic     (501) staff       (20)     1203 2023-04-06 15:03:48.000000 python-eigen-ingenuity-0.4.7.2/eigeningenuity/__init__.py
+-rw-r--r--   0 berhic     (501) staff       (20)    16232 2023-05-18 14:59:11.000000 python-eigen-ingenuity-0.4.7.2/eigeningenuity/assetmodel.py
+drwxr-xr-x   0 berhic     (501) staff       (20)        0 2023-05-22 09:52:48.958725 python-eigen-ingenuity-0.4.7.2/eigeningenuity/core/
+-rw-r--r--   0 berhic     (501) staff       (20)     7715 2023-04-06 10:18:46.000000 python-eigen-ingenuity-0.4.7.2/eigeningenuity/core/__init__.py
+-rw-r--r--   0 berhic     (501) staff       (20)     1146 2022-08-16 09:33:43.000000 python-eigen-ingenuity-0.4.7.2/eigeningenuity/core/debug.py
+-rw-r--r--   0 berhic     (501) staff       (20)     6250 2023-05-17 13:22:24.000000 python-eigen-ingenuity-0.4.7.2/eigeningenuity/elastic.py
+-rw-r--r--   0 berhic     (501) staff       (20)     3054 2023-05-17 13:22:33.000000 python-eigen-ingenuity-0.4.7.2/eigeningenuity/events.py
+-rw-r--r--   0 berhic     (501) staff       (20)    36279 2023-05-22 09:51:56.000000 python-eigen-ingenuity-0.4.7.2/eigeningenuity/historian.py
+-rw-r--r--   0 berhic     (501) staff       (20)     2843 2023-05-17 13:22:46.000000 python-eigen-ingenuity-0.4.7.2/eigeningenuity/smartdash.py
+-rw-r--r--   0 berhic     (501) staff       (20)     4081 2023-05-17 13:22:51.000000 python-eigen-ingenuity-0.4.7.2/eigeningenuity/sql.py
+-rw-r--r--   0 berhic     (501) staff       (20)    12181 2023-05-18 15:50:36.000000 python-eigen-ingenuity-0.4.7.2/eigeningenuity/util.py
+-rw-r--r--   0 berhic     (501) staff       (20)       92 2022-08-16 09:33:43.000000 python-eigen-ingenuity-0.4.7.2/pyproject.toml
+drwxr-xr-x   0 berhic     (501) staff       (20)        0 2023-05-22 09:52:48.959744 python-eigen-ingenuity-0.4.7.2/python_eigen_ingenuity.egg-info/
+-rw-r--r--   0 berhic     (501) staff       (20)    11665 2023-05-22 09:52:48.000000 python-eigen-ingenuity-0.4.7.2/python_eigen_ingenuity.egg-info/PKG-INFO
+-rw-r--r--   0 berhic     (501) staff       (20)      551 2023-05-22 09:52:48.000000 python-eigen-ingenuity-0.4.7.2/python_eigen_ingenuity.egg-info/SOURCES.txt
+-rw-r--r--   0 berhic     (501) staff       (20)        1 2023-05-22 09:52:48.000000 python-eigen-ingenuity-0.4.7.2/python_eigen_ingenuity.egg-info/dependency_links.txt
+-rw-r--r--   0 berhic     (501) staff       (20)       24 2023-05-22 09:52:48.000000 python-eigen-ingenuity-0.4.7.2/python_eigen_ingenuity.egg-info/requires.txt
+-rw-r--r--   0 berhic     (501) staff       (20)       15 2023-05-22 09:52:48.000000 python-eigen-ingenuity-0.4.7.2/python_eigen_ingenuity.egg-info/top_level.txt
+-rw-r--r--   0 berhic     (501) staff       (20)       38 2023-05-22 09:52:48.960267 python-eigen-ingenuity-0.4.7.2/setup.cfg
+-rw-r--r--   0 berhic     (501) staff       (20)      691 2023-05-22 09:52:27.000000 python-eigen-ingenuity-0.4.7.2/setup.py
```

### Comparing `python-eigen-ingenuity-0.4.7.1/LICENSE` & `python-eigen-ingenuity-0.4.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `python-eigen-ingenuity-0.4.7.1/PKG-INFO` & `python-eigen-ingenuity-0.4.7.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-eigen-ingenuity
-Version: 0.4.7.1
+Version: 0.4.7.2
 Summary: A python library used to query data from the Eigen Ingenuity system
 Home-page: https://www.eigen.co/
 Author: Murray Callander
 Author-email: info@eigen.co
 License: Apache License 2.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `python-eigen-ingenuity-0.4.7.1/README.md` & `python-eigen-ingenuity-0.4.7.2/README.md`

 * *Files identical despite different names*

### Comparing `python-eigen-ingenuity-0.4.7.1/eigeningenuity/__init__.py` & `python-eigen-ingenuity-0.4.7.2/eigeningenuity/__init__.py`

 * *Files identical despite different names*

### Comparing `python-eigen-ingenuity-0.4.7.1/eigeningenuity/assetmodel.py` & `python-eigen-ingenuity-0.4.7.2/eigeningenuity/assetmodel.py`

 * *Files 3% similar despite different names*

```diff
@@ -104,25 +104,37 @@
 
         """
         args = {"asset": node}
 
         response = self._doJsonCommonMenuRequest("relatedAssets", args)
         relatedassets = response["relatedAssets"]["graphapi"]
 
+        newAssets=[]
+
+        for item in relatedassets:
+            relations = item["relations"]
+            for relation in relations:
+                newItem = {"asset": item["asset"]}
+                newItem["relationName"] = relation["relationName"]
+                newItem["direction"] = relation["direction"]
+                newAssets.append(newItem)
+
+
+
         if output == "raw":
             return response
         if output == "json":
-            return relatedassets
+            return newAssets
         if output == "df":
-            return pd.json_normalize(relatedassets).drop(columns=["asset.externalId"])
+            return pd.json_normalize(newAssets).drop(columns=["asset.externalId"])
         if output == "file":
             if filepath is None:
                 filepath = node + "-RelatedAssets-" + str(dt.datetime.now().strftime("%Y-%m-%dT%H:%M:%S"))
             with open(filepath + ".json", "w") as f:
-                f.write(json.dumps(relatedassets, indent=4))
+                f.write(json.dumps(newAssets, indent=4))
 
     def getRelatedMeasurementsCypher(self, query:str, prop:str="code", measurement:str="", output="json"):
         """
         Return all measurement tags directly related to a given asset via the AssetModel API.
 
         Args: 
             nodes: The value of the property to match
```

### Comparing `python-eigen-ingenuity-0.4.7.1/eigeningenuity/core/__init__.py` & `python-eigen-ingenuity-0.4.7.2/eigeningenuity/core/__init__.py`

 * *Files identical despite different names*

### Comparing `python-eigen-ingenuity-0.4.7.1/eigeningenuity/core/debug.py` & `python-eigen-ingenuity-0.4.7.2/eigeningenuity/core/debug.py`

 * *Files identical despite different names*

### Comparing `python-eigen-ingenuity-0.4.7.1/eigeningenuity/elastic.py` & `python-eigen-ingenuity-0.4.7.2/eigeningenuity/elastic.py`

 * *Files identical despite different names*

### Comparing `python-eigen-ingenuity-0.4.7.1/eigeningenuity/events.py` & `python-eigen-ingenuity-0.4.7.2/eigeningenuity/events.py`

 * *Files identical despite different names*

### Comparing `python-eigen-ingenuity-0.4.7.1/eigeningenuity/historian.py` & `python-eigen-ingenuity-0.4.7.2/eigeningenuity/historian.py`

 * *Files 1% similar despite different names*

```diff
@@ -373,15 +373,15 @@
             if len(force_list(tags)) == 1:
                 return response[tags]
             else:
                 return response
         elif output == "string":
             return json.dumps(response)
         elif output == "df":
-            return aggToDf(response)
+            return aggToDf(response,fields)
         elif output == "csv":
             order = ["tag","start","end","min","max","avg","var","stddev","count","numgood","numbad"]
             return csvWriter(response,self.historian,filepath,multi_csv,"GetAggregates",order,True)
         return None
 
 
     def getAggregateIntervals(self, tags, start: Union[int, float, str, datetime],
@@ -448,15 +448,15 @@
             if len(force_list(tags)) == 1:
                 return response[tags]
             else:
                 return response
         elif output == "string":
             return json.dumps(response)
         elif output == "df":
-            return aggToDf(response)
+            return aggToDf(response,fields)
         elif output == "csv":
             order = ["tag","start","end","min","max","avg","var","stddev","count","numgood","numbad"]
             return csvWriter(response,self.historian,filepath,multi_csv,"GetAggregateIntervals",order,True)
 
 
     def countPoints(self, tags, start, end, output="json"):
         """
@@ -584,15 +584,15 @@
         Args:
             filepaths: The paths to one or more csv files. CSV Layouts must be as follows, with one point per line: tag,value,timestamp,status,units,description
 
         Returns:
             Success: A boolean representing the successful push of data. True means all csvs were successfully imported, False means at least one csv failed.
         """
         success = []
-        for filepath in filepaths:
+        for filepath in force_list(filepaths):
             with open(filepath, "r") as file:
                 csv_reader = csv.reader(file, delimiter=',')
                 data = list(csv_reader)
                 # Upload in batches of 500 to avoid API timeouts/throttling
                 chunks = divide_chunks(data, 500)
                 for chunk in chunks:
                     datapoints = {}
@@ -658,16 +658,16 @@
             self.status = "OK"
         elif status == "OK" or self.status == "BAD":
             self.status = status
         else:
             raise EigenException("Unrecognised Status")
 
         # Convert timestamp from python datetime or tuple into python floating point epoch seconds
-        self.datetime = datetime.fromtimestamp(timestamp)
-        self.timestamp = pythonTimeToFloatingSecs(timestamp)
+        self.datetime = datetime.fromtimestamp(time_to_epoch_millis(timestamp)/1000)
+        self.timestamp = pythonTimeToFloatingSecs(time_to_epoch_millis(timestamp)/1000)
 
 
     def __str__(self):
         """Return a nicely formatted version of the datapoint"""
         val = self.value
         if type(val) != str:
             val = str(number_to_string(val))
```

### Comparing `python-eigen-ingenuity-0.4.7.1/eigeningenuity/smartdash.py` & `python-eigen-ingenuity-0.4.7.2/eigeningenuity/smartdash.py`

 * *Files identical despite different names*

### Comparing `python-eigen-ingenuity-0.4.7.1/eigeningenuity/sql.py` & `python-eigen-ingenuity-0.4.7.2/eigeningenuity/sql.py`

 * *Files identical despite different names*

### Comparing `python-eigen-ingenuity-0.4.7.1/eigeningenuity/util.py` & `python-eigen-ingenuity-0.4.7.2/eigeningenuity/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,14 +28,15 @@
                         else:
                             e = str(e)
                     requesturl += sep + urlquote(k) + "=" + urlquote(e.encode("UTF8"))
 
                     sep = "&"
 
 
+
     _debug("DEBUG",requesturl)
     if 'DEBUG' in os.environ and os.environ['DEBUG']:
         print("DEBUG: [" + requesturl + "]", file=sys.stderr)
 
     try:
         data = requests.get(requesturl, verify=False)
     except ConnectionError as e:
@@ -84,17 +85,20 @@
     elif type(t) == int and t > 100000000000:
         epochmillis = t
     elif type(t) == int:
         epochmillis = t*1000
     elif type(t) == float and t > 100000000000:
         epochmillis = int(t)
     elif type(t) == float:
-        epochmillis = int(t)*1000
+        epochmillis = round(int(t)*1000)
     elif type(t) == str:
-        epochmillis = get_timestamp(t)
+        if "ago" in t or "now" in t:
+            return t
+        else:
+            epochmillis = get_timestamp(t)
     else:
         raise EigenException("Unknown time format " + str(type(t)))
     return int(round(epochmillis))
 
 def get_time_tuple(floatingpointepochsecs):
     time_tuple = time.gmtime(floatingpointepochsecs)
     return time_tuple
@@ -104,36 +108,36 @@
     s = datetime.fromtimestamp(t).strftime(pattern)
     return s
 
 def get_timestamp(t):
     if type(t) == str:
         try:
             pattern = '%Y-%m-%d %H:%M:%S.%f'
-            epochmillis = time.mktime(time.strptime(t, pattern))
+            epochmillis = int(time.mktime(time.strptime(t, pattern)))
         except ValueError:
             try:
                 pattern = '%Y-%m-%dT%H:%M:%S.%f%z'
-                epochmillis = time.mktime(time.strptime(t, pattern))
+                epochmillis = int(time.mktime(time.strptime(t, pattern)))
             except ValueError:
                 try:
                     pattern = '%Y-%m-%d %H:%M:%S'
-                    epochmillis = time.mktime(time.strptime(t, pattern))
+                    epochmillis = int(time.mktime(time.strptime(t, pattern)))
                 except ValueError:
                     try:
                         pattern = '%Y-%m-%d'
-                        epochmillis = time.mktime(time.strptime(t, pattern))
+                        epochmillis = int(time.mktime(time.strptime(t, pattern)))
                     except ValueError:
                         try:
                             epochmillis = int(t)
                         except ValueError:
                             raise EigenException("Unknown time format " + str(type(t)))
 
     else:
-        epochmillis = time_to_epoch_millis(t)
-    return epochmillis
+        return(time_to_epoch_millis(t))
+    return int(round(epochmillis))
 
 
 
 def get_datetime(t):
     timestamp = get_timestamp(t)
     return datetime.fromtimestamp(timestamp)
 
@@ -278,17 +282,20 @@
     return points
 
 def aggMap(x):
     for k in x[1]:
         k["tag"] = x[0]
     return x[1]
 
-def aggToDf(x):
+def aggToDf(x,cols):
     y = flattenList(list(map(aggMap,x.items())))
-    cols = ["tag", "start", "end", "min", "max", "avg", "var", "stddev", "numgood", "numbad"]
+    if cols is None:
+        cols = ["tag", "start", "end", "min", "max", "avg", "var", "stddev", "numgood", "numbad"]
+    else:
+        cols = ["tag", "start", "end"] + cols
     df = pd.DataFrame(y)
     df = df[cols]
     try:
         df["start"] = pd.to_datetime(df["start"], unit="ms")
         df["end"] = pd.to_datetime(df["end"], unit="ms")
     except ValueError:
         df["start"] = pd.to_datetime(df["start"], format="ISO8601")
@@ -297,15 +304,16 @@
     return(df)
 
 def get_eigenserver(url):
     split_url = urlsplit(url)
     return split_url.scheme + "://" + split_url.netloc
 
 def constructURL(y,x):
-    x["url"] = y + x["url"]
+    if "//" not in x["url"]:
+        x["url"] = y + x["url"]
     k = {"fileName": x["fileName"], "description": x["description"], "url": x["url"]}
     return k
 
 def parseEvents(events):
     if type(events) == dict or type(events) == list:
         events = events
     elif type(events) == str:
```

### Comparing `python-eigen-ingenuity-0.4.7.1/python_eigen_ingenuity.egg-info/PKG-INFO` & `python-eigen-ingenuity-0.4.7.2/python_eigen_ingenuity.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-eigen-ingenuity
-Version: 0.4.7.1
+Version: 0.4.7.2
 Summary: A python library used to query data from the Eigen Ingenuity system
 Home-page: https://www.eigen.co/
 Author: Murray Callander
 Author-email: info@eigen.co
 License: Apache License 2.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `python-eigen-ingenuity-0.4.7.1/python_eigen_ingenuity.egg-info/SOURCES.txt` & `python-eigen-ingenuity-0.4.7.2/python_eigen_ingenuity.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `python-eigen-ingenuity-0.4.7.1/setup.py` & `python-eigen-ingenuity-0.4.7.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 README = (HERE / "README.md").read_text()
 
 pkgname = 'python-eigen-ingenuity'
 
 # Invoke setup
 setup(
     name=pkgname,
-    version='0.4.7.1',
+    version='0.4.7.2',
     author='Murray Callander',
     author_email='info@eigen.co',
     url='https://www.eigen.co/',
     description="A python library used to query data from the Eigen Ingenuity system",
     long_description=README,
     long_description_content_type="text/markdown",
     packages=find_packages("."),
```

