# Comparing `tmp/easy_gtfs-0.1.0.3.tar.gz` & `tmp/easy_gtfs-0.1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easy_gtfs-0.1.0.3.tar", max compression
+gzip compressed data, was "easy_gtfs-0.1.0.4.tar", max compression
```

## Comparing `easy_gtfs-0.1.0.3.tar` & `easy_gtfs-0.1.0.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0       23 2023-05-15 16:28:56.423189 easy_gtfs-0.1.0.3/easy_gtfs/__init__.py
--rw-r--r--   0        0        0      113 2023-05-19 15:27:42.521125 easy_gtfs-0.1.0.3/easy_gtfs/agency.txt
--rw-r--r--   0        0        0        0 2023-05-15 16:24:21.223177 easy_gtfs-0.1.0.3/easy_gtfs/managers/__init__.py
--rw-r--r--   0        0        0      192 2023-05-17 19:43:33.659534 easy_gtfs-0.1.0.3/easy_gtfs/managers/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     5502 2023-05-19 20:03:36.971506 easy_gtfs-0.1.0.3/easy_gtfs/managers/__pycache__/agencymanager.cpython-39.pyc
--rw-r--r--   0        0        0     1477 2023-05-19 20:03:36.961011 easy_gtfs-0.1.0.3/easy_gtfs/managers/__pycache__/errormanager.cpython-39.pyc
--rw-r--r--   0        0        0     2875 2023-05-19 20:03:36.951409 easy_gtfs-0.1.0.3/easy_gtfs/managers/__pycache__/gtfsmanager.cpython-39.pyc
--rw-r--r--   0        0        0     7039 2023-05-19 20:30:44.809385 easy_gtfs-0.1.0.3/easy_gtfs/managers/agencymanager.py
--rw-r--r--   0        0        0      828 2023-05-19 19:59:56.002870 easy_gtfs-0.1.0.3/easy_gtfs/managers/errormanager.py
--rw-r--r--   0        0        0     5819 2023-05-19 20:57:22.548209 easy_gtfs-0.1.0.3/easy_gtfs/managers/gtfsmanager.py
--rw-r--r--   0        0        0     6683 2023-05-19 20:38:50.085033 easy_gtfs-0.1.0.3/easy_gtfs/managers/stopmanager.py
--rw-r--r--   0        0        0        0 2023-05-15 16:24:14.442747 easy_gtfs-0.1.0.3/easy_gtfs/models/__init__.py
--rw-r--r--   0        0        0      190 2023-05-19 15:28:11.632756 easy_gtfs-0.1.0.3/easy_gtfs/models/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     1267 2023-05-19 20:03:36.979111 easy_gtfs-0.1.0.3/easy_gtfs/models/__pycache__/errors.cpython-39.pyc
--rw-r--r--   0        0        0      995 2023-05-19 20:52:02.586564 easy_gtfs-0.1.0.3/easy_gtfs/models/errors.py
--rw-r--r--   0        0        0     6955 2023-05-19 20:08:49.060106 easy_gtfs-0.1.0.3/easy_gtfs/models/models.py
--rw-r--r--   0        0        0        0 2023-05-15 14:09:30.614598 easy_gtfs-0.1.0.3/easy_gtfs/objects/__init__.py
--rw-r--r--   0        0        0      191 2023-05-15 16:32:34.727557 easy_gtfs-0.1.0.3/easy_gtfs/objects/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     2398 2023-05-15 16:32:34.737067 easy_gtfs-0.1.0.3/easy_gtfs/objects/__pycache__/agency.cpython-39.pyc
--rw-r--r--   0        0        0     2762 2023-05-15 16:31:14.415464 easy_gtfs-0.1.0.3/easy_gtfs/objects/agency.py
--rw-r--r--   0        0        0     6437 2023-05-19 20:26:24.793506 easy_gtfs-0.1.0.3/easy_gtfs/objects/stop.py
--rw-r--r--   0        0        0     3217 2023-05-17 19:26:25.836427 easy_gtfs-0.1.0.3/easy_gtfs/sample-feed.zip
--rw-r--r--   0        0        0     1277 2023-05-17 19:43:57.791496 easy_gtfs-0.1.0.3/easy_gtfs/utility.py
--rw-r--r--   0        0        0     1423 2023-05-19 17:52:23.436347 easy_gtfs-0.1.0.3/easy_gtfs/variables.py
--rw-r--r--   0        0        0      343 2023-05-15 16:29:16.528178 easy_gtfs-0.1.0.3/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-15 14:06:25.799294 easy_gtfs-0.1.0.3/README.md
--rw-r--r--   0        0        0      411 1970-01-01 00:00:00.000000 easy_gtfs-0.1.0.3/PKG-INFO
+-rw-r--r--   0        0        0       23 2023-05-15 16:28:56.423189 easy_gtfs-0.1.0.4/easy_gtfs/__init__.py
+-rw-r--r--   0        0        0      113 2023-05-19 15:27:42.521125 easy_gtfs-0.1.0.4/easy_gtfs/agency.txt
+-rw-r--r--   0        0        0        0 2023-05-15 16:24:21.223177 easy_gtfs-0.1.0.4/easy_gtfs/managers/__init__.py
+-rw-r--r--   0        0        0      192 2023-05-17 19:43:33.659534 easy_gtfs-0.1.0.4/easy_gtfs/managers/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     5502 2023-05-19 20:03:36.971506 easy_gtfs-0.1.0.4/easy_gtfs/managers/__pycache__/agencymanager.cpython-39.pyc
+-rw-r--r--   0        0        0     1477 2023-05-19 20:03:36.961011 easy_gtfs-0.1.0.4/easy_gtfs/managers/__pycache__/errormanager.cpython-39.pyc
+-rw-r--r--   0        0        0     2875 2023-05-19 20:03:36.951409 easy_gtfs-0.1.0.4/easy_gtfs/managers/__pycache__/gtfsmanager.cpython-39.pyc
+-rw-r--r--   0        0        0     8676 2023-05-20 19:24:43.773731 easy_gtfs-0.1.0.4/easy_gtfs/managers/agencymanager.py
+-rw-r--r--   0        0        0      828 2023-05-19 19:59:56.002870 easy_gtfs-0.1.0.4/easy_gtfs/managers/errormanager.py
+-rw-r--r--   0        0        0     5913 2023-05-22 17:51:48.104965 easy_gtfs-0.1.0.4/easy_gtfs/managers/gtfsmanager.py
+-rw-r--r--   0        0        0    12695 2023-05-22 17:58:48.718294 easy_gtfs-0.1.0.4/easy_gtfs/managers/stopmanager.py
+-rw-r--r--   0        0        0        0 2023-05-15 16:24:14.442747 easy_gtfs-0.1.0.4/easy_gtfs/models/__init__.py
+-rw-r--r--   0        0        0      190 2023-05-19 15:28:11.632756 easy_gtfs-0.1.0.4/easy_gtfs/models/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     1267 2023-05-19 20:03:36.979111 easy_gtfs-0.1.0.4/easy_gtfs/models/__pycache__/errors.cpython-39.pyc
+-rw-r--r--   0        0        0     2377 2023-05-22 17:47:57.212218 easy_gtfs-0.1.0.4/easy_gtfs/models/errors.py
+-rw-r--r--   0        0        0     6955 2023-05-19 20:08:49.060106 easy_gtfs-0.1.0.4/easy_gtfs/models/models.py
+-rw-r--r--   0        0        0        0 2023-05-15 14:09:30.614598 easy_gtfs-0.1.0.4/easy_gtfs/objects/__init__.py
+-rw-r--r--   0        0        0      191 2023-05-15 16:32:34.727557 easy_gtfs-0.1.0.4/easy_gtfs/objects/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     2398 2023-05-15 16:32:34.737067 easy_gtfs-0.1.0.4/easy_gtfs/objects/__pycache__/agency.cpython-39.pyc
+-rw-r--r--   0        0        0     2762 2023-05-15 16:31:14.415464 easy_gtfs-0.1.0.4/easy_gtfs/objects/agency.py
+-rw-r--r--   0        0        0     6437 2023-05-19 20:26:24.793506 easy_gtfs-0.1.0.4/easy_gtfs/objects/stop.py
+-rw-r--r--   0        0        0     3217 2023-05-17 19:26:25.836427 easy_gtfs-0.1.0.4/easy_gtfs/sample-feed.zip
+-rw-r--r--   0        0        0     1277 2023-05-17 19:43:57.791496 easy_gtfs-0.1.0.4/easy_gtfs/utility.py
+-rw-r--r--   0        0        0     1423 2023-05-19 17:52:23.436347 easy_gtfs-0.1.0.4/easy_gtfs/variables.py
+-rw-r--r--   0        0        0      487 2023-05-19 21:06:06.562370 easy_gtfs-0.1.0.4/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-15 14:06:25.799294 easy_gtfs-0.1.0.4/README.md
+-rw-r--r--   0        0        0      479 1970-01-01 00:00:00.000000 easy_gtfs-0.1.0.4/PKG-INFO
```

### Comparing `easy_gtfs-0.1.0.3/easy_gtfs/managers/__pycache__/agencymanager.cpython-39.pyc` & `easy_gtfs-0.1.0.4/easy_gtfs/managers/__pycache__/agencymanager.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `easy_gtfs-0.1.0.3/easy_gtfs/managers/__pycache__/errormanager.cpython-39.pyc` & `easy_gtfs-0.1.0.4/easy_gtfs/managers/__pycache__/errormanager.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `easy_gtfs-0.1.0.3/easy_gtfs/managers/__pycache__/gtfsmanager.cpython-39.pyc` & `easy_gtfs-0.1.0.4/easy_gtfs/managers/__pycache__/gtfsmanager.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `easy_gtfs-0.1.0.3/easy_gtfs/managers/agencymanager.py` & `easy_gtfs-0.1.0.4/easy_gtfs/managers/agencymanager.py`

 * *Files 17% similar despite different names*

```diff
@@ -55,17 +55,29 @@
             file = self.file
 
 
         headers: list = [variable for variable in agencies[0].dict(exclude_unset=False).keys()] # create a list of the headers for the csv file
         rows: list = []
         
         agencies_ids = [] # this list stores the ids of all the agencies that will be written to the file so we can verify that no agencies have the same id
+        agencies_timezones = [] # stores the timezone of all the agencies as they have to be the same
         for obj in agencies:
             obj_as_dict = obj.dict(exclude_unset=False)
             agencies_ids.append(obj_as_dict["agency_id"]) # add the id of the agency to our ids list for verification later on
+            agencies_timezones.append(obj_as_dict["agency_timezone"])
+            if len(agencies_timezones) > 0:
+                if obj_as_dict["agency_timezone"] != agencies_timezones[0]:
+                    if self.error_manager.is_silent_errors():
+                        self.error_manager.add_error(AgencyError(
+                            error_type=ErrorTypes.AgencyErrorTimezonesNotSame,
+                            message="If multiple agencies are present, they must have the same timezone!",
+                            value = [obj_as_dict]
+                        ))
+                    else:
+                        raise ValueError(f"If multiple agencies are present, they must have the same timezone! \n {obj_as_dict}")
             rows.append(obj_as_dict) # add the agency as json to our rows that will be written to the csv file
 
         if len(agencies_ids) > 1:
             duplicates = [k for k, v in Counter(agencies_ids).items() if v>1] # returns a list with all duplicate ids; if the id '123' was for example at least 2 times in the ids list the output would be: ['123']
             if len(duplicates) > 0:
                 if self.error_manager.is_silent_errors():
                     self.error_manager.add_error(AgencyError(
@@ -73,14 +85,19 @@
                         error_type=ErrorTypes.AgencyErrorDuplicateID,
                         message="Multiple agencies cannot have the same id!",
                         values = duplicates
                     ))
                     return False
                 else:
                     raise ValueError(f"Multiple agencies cannot have the same id! Got the following duplicate ids: {duplicates}")
+                
+
+        
+                
+        
             
 
         with open(file, "w", newline='') as _file:
             csvwriter = csv.DictWriter(_file, fieldnames=headers)
             csvwriter.writeheader()
             csvwriter.writerows(rows)
 
@@ -131,27 +148,40 @@
 
         with open(file, "r") as _file:
             csvreader = list(csv.DictReader(_file)) # gives a list of dictionaries where each dict is a json representation of an agency
 
         agencies = self.parse(csvreader)
 
         agencies_ids = []
+        agencies_timezones = []
 
         for agency in agencies:
             if agency.agency_id in agencies_ids:
                 if self.error_manager.is_silent_errors():
                     self.error_manager.add_error(AgencyError(
                         caller = "AgencyManager",
                         error_type = ErrorTypes.AgencyErrorDuplicateID,
                         message="Cannot have multiple agencies with the same id!",
                         values = [agency.agency_id]
                     ))
                     return False
                 else:
                     raise ValueError("Cannot have multiple agencies with the same id!")
+            
+            if len(agencies_timezones) > 0:
+                if agency.agency_timezone != agencies_timezones[0]:
+                    if self.error_manager.is_silent_errors():
+                        self.error_manager.add_error(AgencyError(
+                            error_type=ErrorTypes.AgencyErrorTimezonesNotSame,
+                            message="If multiple agencies are present, they must have the same timezone!",
+                            value = [agency]
+                        ))
+                    else:
+                        raise ValueError(f"If multiple agencies are present, they must have the same timezone! \n {agency}")
+                    
             agencies_ids.append(agency.agency_id)
 
         return agencies
 
         
     def is_valid_agency(self, agency: dict) -> bool:
         """
```

### Comparing `easy_gtfs-0.1.0.3/easy_gtfs/managers/errormanager.py` & `easy_gtfs-0.1.0.4/easy_gtfs/managers/errormanager.py`

 * *Files identical despite different names*

### Comparing `easy_gtfs-0.1.0.3/easy_gtfs/managers/gtfsmanager.py` & `easy_gtfs-0.1.0.4/easy_gtfs/managers/gtfsmanager.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 """
     This class handles all the other managers (altough they each work on their own).
     You can use this class to quickly read a gtfs dataset or create one from your data without calling each single manager by hand.
 """
 
 import os
 from zipfile import ZipFile
-import csv
-import io
-import codecs
 
 
 from ..utility import get_error_manager
 from ..variables import FILES, OUTPUT_FOLDER
 from .agencymanager import Agencies
 from .stopmanager import Stops
 from ..models.errors import ErrorTypes, GTFSError
 
 
+"""
+    TODO: Need to check if stop id in route corresponds to an actual stop in stops.txt, same for agency id and other ids
+"""
 
 class GTFSManager():
     def __init__(self, silent_errors: bool = False) -> None:
         self.silent_errors = silent_errors
         self.error_manager = get_error_manager()
         self.error_manager.set_silent_errors(self.silent_errors)
```

### Comparing `easy_gtfs-0.1.0.3/easy_gtfs/models/__pycache__/errors.cpython-39.pyc` & `easy_gtfs-0.1.0.4/easy_gtfs/models/__pycache__/errors.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `easy_gtfs-0.1.0.3/easy_gtfs/models/models.py` & `easy_gtfs-0.1.0.4/easy_gtfs/models/models.py`

 * *Files identical despite different names*

### Comparing `easy_gtfs-0.1.0.3/easy_gtfs/objects/__pycache__/agency.cpython-39.pyc` & `easy_gtfs-0.1.0.4/easy_gtfs/objects/__pycache__/agency.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `easy_gtfs-0.1.0.3/easy_gtfs/objects/agency.py` & `easy_gtfs-0.1.0.4/easy_gtfs/objects/agency.py`

 * *Files identical despite different names*

### Comparing `easy_gtfs-0.1.0.3/easy_gtfs/objects/stop.py` & `easy_gtfs-0.1.0.4/easy_gtfs/objects/stop.py`

 * *Files identical despite different names*

### Comparing `easy_gtfs-0.1.0.3/easy_gtfs/sample-feed.zip` & `easy_gtfs-0.1.0.4/easy_gtfs/sample-feed.zip`

 * *Files identical despite different names*

### Comparing `easy_gtfs-0.1.0.3/easy_gtfs/utility.py` & `easy_gtfs-0.1.0.4/easy_gtfs/utility.py`

 * *Files identical despite different names*

### Comparing `easy_gtfs-0.1.0.3/easy_gtfs/variables.py` & `easy_gtfs-0.1.0.4/easy_gtfs/variables.py`

 * *Files identical despite different names*

