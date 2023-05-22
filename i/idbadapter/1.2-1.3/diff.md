# Comparing `tmp/idbadapter-1.2.tar.gz` & `tmp/idbadapter-1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idbadapter-1.2.tar", last modified: Mon May 15 10:45:54 2023, max compression
+gzip compressed data, was "idbadapter-1.3.tar", last modified: Mon May 22 10:10:40 2023, max compression
```

## Comparing `idbadapter-1.2.tar` & `idbadapter-1.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-15 10:45:54.086416 idbadapter-1.2/
--rw-rw-rw-   0        0        0    11558 2023-05-15 08:54:26.000000 idbadapter-1.2/LICENSE
--rw-rw-rw-   0        0        0      695 2023-05-15 10:45:54.086416 idbadapter-1.2/PKG-INFO
--rw-rw-rw-   0        0        0      182 2023-05-15 08:54:26.000000 idbadapter-1.2/README.md
-drwxrwxrwx   0        0        0        0 2023-05-15 10:45:54.074418 idbadapter-1.2/idbadapter/
--rw-rw-rw-   0        0        0       61 2023-05-15 08:54:26.000000 idbadapter-1.2/idbadapter/__init__.py
--rw-rw-rw-   0        0        0     6086 2023-05-15 10:36:39.000000 idbadapter-1.2/idbadapter/schedule_loader.py
-drwxrwxrwx   0        0        0        0 2023-05-15 10:45:54.084416 idbadapter-1.2/idbadapter.egg-info/
--rw-rw-rw-   0        0        0      695 2023-05-15 10:45:53.000000 idbadapter-1.2/idbadapter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      258 2023-05-15 10:45:54.000000 idbadapter-1.2/idbadapter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-15 10:45:53.000000 idbadapter-1.2/idbadapter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-05-15 10:45:53.000000 idbadapter-1.2/idbadapter.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-05-15 10:45:53.000000 idbadapter-1.2/idbadapter.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-15 10:45:54.087416 idbadapter-1.2/setup.cfg
--rw-rw-rw-   0        0        0      987 2023-05-15 10:44:01.000000 idbadapter-1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-22 10:10:40.402476 idbadapter-1.3/
+-rw-rw-rw-   0        0        0    11558 2023-05-02 13:28:55.000000 idbadapter-1.3/LICENSE
+-rw-rw-rw-   0        0        0      695 2023-05-22 10:10:40.402476 idbadapter-1.3/PKG-INFO
+-rw-rw-rw-   0        0        0      182 2023-05-05 13:33:15.000000 idbadapter-1.3/README.md
+drwxrwxrwx   0        0        0        0 2023-05-22 10:10:40.385041 idbadapter-1.3/idbadapter/
+-rw-rw-rw-   0        0        0       61 2023-05-22 08:18:39.000000 idbadapter-1.3/idbadapter/__init__.py
+-rw-rw-rw-   0        0        0     6806 2023-05-22 10:04:07.000000 idbadapter-1.3/idbadapter/schedule_loader.py
+drwxrwxrwx   0        0        0        0 2023-05-22 10:10:40.401477 idbadapter-1.3/idbadapter.egg-info/
+-rw-rw-rw-   0        0        0      695 2023-05-22 10:10:40.000000 idbadapter-1.3/idbadapter.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      258 2023-05-22 10:10:40.000000 idbadapter-1.3/idbadapter.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-22 10:10:40.000000 idbadapter-1.3/idbadapter.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-05-22 10:10:40.000000 idbadapter-1.3/idbadapter.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-05-22 10:10:40.000000 idbadapter-1.3/idbadapter.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-22 10:10:40.403476 idbadapter-1.3/setup.cfg
+-rw-rw-rw-   0        0        0      987 2023-05-22 10:07:35.000000 idbadapter-1.3/setup.py
```

### Comparing `idbadapter-1.2/LICENSE` & `idbadapter-1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `idbadapter-1.2/PKG-INFO` & `idbadapter-1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idbadapter
-Version: 1.2
+Version: 1.3
 Summary: Сache module for batch loading of data
 Home-page: https://github.com/AnatolyPershinov/gpn_cache_module
 Download-URL: https://github.com/AnatolyPershinov/gpn_cache_module/archive/master.zip
 Author: Anatoly Pershinov
 Author-email: anatoliypershinov@gmail.com
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `idbadapter-1.2/idbadapter/schedule_loader.py` & `idbadapter-1.3/idbadapter/schedule_loader.py`

 * *Files 14% similar despite different names*

```diff
@@ -42,28 +42,35 @@
         self.ceil_limit = ceil_limit
         self.works_list = works_list
         self.resource_list = resource_list
         self.objects = list({*self._get_objects_by_resource(), *self._get_objects_by_works()})
 
         return self
     
-    def from_names(self, works: list[str], resources: list[str] = [], ceil_limit: int = 1_000):
+    def from_names(self, works: list[str], resources: list[str] = [], ceil_limit: int = 1_000, objects_limit: int = 1, crossing=False):
         """method for getting schedules by works names list
 
         Args:
             work_name_list (list[str]): lists of basic works names 
             ceil_limit (int, optional): limit of records in one dataframe. Defaults to 1_000.
         """
         if len(works) == 0 and len(resources) == 0:
             raise Exception("Empty works list")
         self.ceil_limit = ceil_limit
+        self.objects_limit = objects_limit
         self.works_list = self._get_works_ids_by_names(works)
         self.resource_list = self._get_resource_ids_by_names(resources)
         
-        self.objects = list({*self._get_objects_by_resource(), *self._get_objects_by_works()})
+        if crossing:
+            self.objects =list(set(self._get_objects_by_resource()).intersection(set(self._get_objects_by_works())))
+        else:        
+            self.objects = list({*self._get_objects_by_resource(), *self._get_objects_by_works()})
+            
+        if len(self.objects) == 0:
+            raise Exception("Objects not found")
         
         return self
            
     def _get_works_ids_by_names(self, work_name_list):
         data = json.dumps(work_name_list)
         response = self.session.post(urllib.parse.urljoin(self.url, "work/get_basic_works_ids"), data=data)
         if "detail" in response.json(): 
@@ -90,63 +97,70 @@
         if len(self.works_list) == 0:
             return []
         data = json.dumps(self.works_list)
         response = self.session.post(urllib.parse.urljoin(self.url, "work/schedule_ids"), data=data)
         return response.json()
    
     def __iter__(self):
-        return SchedulesIterator(self.objects, self.session, self.url, self.ceil_limit)
+        return SchedulesIterator(self.objects, self.session, self.url, self.ceil_limit, self.objects_limit)
 
 
 class SchedulesIterator:
-    def __init__(self, objects, session, url, ceil_limit):
+    def __init__(self, objects, session, url, ceil_limit, objects_limit):
         self.objects = objects
         self.session = session
+        self.objects_limit = objects_limit if objects_limit != -1 else len(objects)
         self.url = url
         self.ceil_limit = ceil_limit
         self.index = 0
         self.start_date = "1970-1-1"
+        self.object_slice = self.objects[self.index:self.index+self.objects_limit]
 
     def _select_works_from_db(self):
         data = json.dumps({
-            "object_id": self.objects[self.index],
+            "object_id": self.object_slice,
             "start_date": self.start_date,
             "max_work_statuses": self.ceil_limit
         })
+
         response = self.session.post(urllib.parse.urljoin(self.url, "schedule/works_by_schedule"), data=data)
         works = response.json()
         df = pd.DataFrame(works)       
-        
+
         return df
 
     def _select_resources_from_db(self, start_date, finish_date):
         data = json.dumps({
-            "object_id": self.objects[self.index],
+            "object_id": self.object_slice,
             "start_date": start_date,
             "finish_date": finish_date
         })
         response = self.session.post(urllib.parse.urljoin(self.url, "schedule/resources_by_schedule"), data=data)
         resources = response.json()
+
         df = pd.DataFrame(resources)
         
         return df
     
     def __next__(self):
+        if len(self.object_slice) == 0:
+            raise StopIteration
+        
         try:
             works_df = self._select_works_from_db()
             if len(works_df) == self.ceil_limit:
                 self.start_date = works_df.date.max()
                 works_df = works_df[works_df.date != self.start_date]
                 res_df = self._select_resources_from_db(works_df["date"].min(), works_df["date"].max())    
             else:
                 res_df = self._select_resources_from_db(works_df["date"].min(), works_df["date"].max())  
-                self.index += 1
                 self.start_date = "1970-1-1"
-                
-            
+                self.index += self.objects_limit
+                self.object_slice = self.objects[self.index:self.index+self.objects_limit]
+                    
         except IndexError:
             raise StopIteration
         
         df = pd.concat([works_df, res_df])
 
         df = self.convert_df(df)
```

### Comparing `idbadapter-1.2/idbadapter.egg-info/PKG-INFO` & `idbadapter-1.3/idbadapter.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idbadapter
-Version: 1.2
+Version: 1.3
 Summary: Сache module for batch loading of data
 Home-page: https://github.com/AnatolyPershinov/gpn_cache_module
 Download-URL: https://github.com/AnatolyPershinov/gpn_cache_module/archive/master.zip
 Author: Anatoly Pershinov
 Author-email: anatoliypershinov@gmail.com
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `idbadapter-1.2/setup.py` & `idbadapter-1.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 #!/usr/bin/env python
 
 from distutils.core import setup
 
-version = '1.1'
+version = '1.3'
 
 long_description = "Сache module for batch loading of data"
 
 setup(name='idbadapter',
-      version='1.2',
+      version='1.3',
       description='Сache module for batch loading of data',
       long_description=long_description,
       url="https://github.com/AnatolyPershinov/gpn_cache_module",
       download_url='https://github.com/AnatolyPershinov/gpn_cache_module/archive/master.zip',
       author='Anatoly Pershinov',
       author_email='anatoliypershinov@gmail.com',
       packages=['idbadapter'],
```

