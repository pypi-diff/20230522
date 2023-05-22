# Comparing `tmp/spotON_sdk-0.0.4.7.tar.gz` & `tmp/spotON_sdk-0.0.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spotON_sdk-0.0.4.7.tar", last modified: Mon May 22 18:14:01 2023, max compression
+gzip compressed data, was "spotON_sdk-0.0.4.8.tar", last modified: Mon May 22 18:47:32 2023, max compression
```

## Comparing `spotON_sdk-0.0.4.7.tar` & `spotON_sdk-0.0.4.8.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     6184 2023-05-21 14:30:18.248848 spotON_sdk-0.0.4.7/.gitignore
--rw-r--r--   0        0        0     1085 2023-05-06 14:04:24.538041 spotON_sdk-0.0.4.7/LICENSE
--rw-r--r--   0        0        0      355 2023-05-21 15:19:16.024161 spotON_sdk-0.0.4.7/pyproject.toml
--rw-r--r--   0        0        0      468 2023-05-22 17:37:16.929836 spotON_sdk-0.0.4.7/spotON_sdk/Logic/Feedback/Feedback.py
--rw-r--r--   0        0        0      122 2023-05-13 12:18:00.893425 spotON_sdk-0.0.4.7/spotON_sdk/Logic/Feedback/Sensors.py
--rw-r--r--   0        0        0      429 2023-05-13 11:38:31.810517 spotON_sdk-0.0.4.7/spotON_sdk/Logic/Feedback/Units.py
--rw-r--r--   0        0        0      145 2023-05-22 08:52:45.547083 spotON_sdk-0.0.4.7/spotON_sdk/Logic/Feedback/__init__.py
--rw-r--r--   0        0        0       93 2023-05-22 16:38:29.648297 spotON_sdk-0.0.4.7/spotON_sdk/Logic/Output/Switchtypes.py
--rw-r--r--   0        0        0      104 2023-05-22 08:52:50.913401 spotON_sdk-0.0.4.7/spotON_sdk/Logic/Output/__init__.py
--rw-r--r--   0        0        0     3285 2023-05-22 09:14:50.783679 spotON_sdk-0.0.4.7/spotON_sdk/Logic/Price/Price_Logic.py
--rw-r--r--   0        0        0      182 2023-05-22 17:37:25.105808 spotON_sdk-0.0.4.7/spotON_sdk/Logic/Price/__init__.py
--rw-r--r--   0        0        0      745 2023-05-08 10:18:24.622068 spotON_sdk-0.0.4.7/spotON_sdk/Logic/Price/bidding_zones.py
--rw-r--r--   0        0        0     4709 2023-05-22 09:10:42.883983 spotON_sdk-0.0.4.7/spotON_sdk/Logic/Price/countries.py
--rw-r--r--   0        0        0     2282 2023-05-22 09:10:36.501033 spotON_sdk-0.0.4.7/spotON_sdk/Logic/Price/markets.py
--rw-r--r--   0        0        0     6957 2023-05-17 21:52:50.903007 spotON_sdk-0.0.4.7/spotON_sdk/Logic/Price/spotON_Areas.py
--rw-r--r--   0        0        0      144 2023-05-22 18:00:58.368103 spotON_sdk-0.0.4.7/spotON_sdk/Logic/__init__.py
--rw-r--r--   0        0        0      458 2023-05-22 18:13:16.726672 spotON_sdk-0.0.4.7/spotON_sdk/__init__.py
--rw-r--r--   0        0        0      714 2023-05-22 18:11:54.358565 spotON_sdk-0.0.4.7/spotON_sdk/data_helpers/BestHour.py
--rw-r--r--   0        0        0      136 2023-05-22 08:52:16.359432 spotON_sdk-0.0.4.7/spotON_sdk/data_helpers/__init__.py
--rw-r--r--   0        0        0     1378 2023-05-22 08:52:33.315148 spotON_sdk-0.0.4.7/spotON_sdk/data_helpers/dataframe_modifier.py
--rw-r--r--   0        0        0      336 2023-05-22 18:01:04.746198 spotON_sdk-0.0.4.7/spotON_sdk/spotON_controller.py
--rw-r--r--   0        0        0      250 1970-01-01 00:00:00.000000 spotON_sdk-0.0.4.7/PKG-INFO
+-rw-r--r--   0        0        0     6184 2023-05-21 14:30:18.248848 spotON_sdk-0.0.4.8/.gitignore
+-rw-r--r--   0        0        0     1085 2023-05-06 14:04:24.538041 spotON_sdk-0.0.4.8/LICENSE
+-rw-r--r--   0        0        0      355 2023-05-21 15:19:16.024161 spotON_sdk-0.0.4.8/pyproject.toml
+-rw-r--r--   0        0        0      468 2023-05-22 17:37:16.929836 spotON_sdk-0.0.4.8/spotON_sdk/Logic/Feedback/Feedback.py
+-rw-r--r--   0        0        0      122 2023-05-13 12:18:00.893425 spotON_sdk-0.0.4.8/spotON_sdk/Logic/Feedback/Sensors.py
+-rw-r--r--   0        0        0      429 2023-05-13 11:38:31.810517 spotON_sdk-0.0.4.8/spotON_sdk/Logic/Feedback/Units.py
+-rw-r--r--   0        0        0      145 2023-05-22 08:52:45.547083 spotON_sdk-0.0.4.8/spotON_sdk/Logic/Feedback/__init__.py
+-rw-r--r--   0        0        0       93 2023-05-22 16:38:29.648297 spotON_sdk-0.0.4.8/spotON_sdk/Logic/Output/Switchtypes.py
+-rw-r--r--   0        0        0      104 2023-05-22 08:52:50.913401 spotON_sdk-0.0.4.8/spotON_sdk/Logic/Output/__init__.py
+-rw-r--r--   0        0        0     3323 2023-05-22 18:47:21.679789 spotON_sdk-0.0.4.8/spotON_sdk/Logic/Price/Price_Logic.py
+-rw-r--r--   0        0        0      182 2023-05-22 17:37:25.105808 spotON_sdk-0.0.4.8/spotON_sdk/Logic/Price/__init__.py
+-rw-r--r--   0        0        0      745 2023-05-08 10:18:24.622068 spotON_sdk-0.0.4.8/spotON_sdk/Logic/Price/bidding_zones.py
+-rw-r--r--   0        0        0     4709 2023-05-22 09:10:42.883983 spotON_sdk-0.0.4.8/spotON_sdk/Logic/Price/countries.py
+-rw-r--r--   0        0        0     2282 2023-05-22 09:10:36.501033 spotON_sdk-0.0.4.8/spotON_sdk/Logic/Price/markets.py
+-rw-r--r--   0        0        0     6957 2023-05-17 21:52:50.903007 spotON_sdk-0.0.4.8/spotON_sdk/Logic/Price/spotON_Areas.py
+-rw-r--r--   0        0        0      144 2023-05-22 18:00:58.368103 spotON_sdk-0.0.4.8/spotON_sdk/Logic/__init__.py
+-rw-r--r--   0        0        0      458 2023-05-22 18:47:28.039092 spotON_sdk-0.0.4.8/spotON_sdk/__init__.py
+-rw-r--r--   0        0        0      714 2023-05-22 18:11:54.358565 spotON_sdk-0.0.4.8/spotON_sdk/data_helpers/BestHour.py
+-rw-r--r--   0        0        0      136 2023-05-22 08:52:16.359432 spotON_sdk-0.0.4.8/spotON_sdk/data_helpers/__init__.py
+-rw-r--r--   0        0        0     1378 2023-05-22 08:52:33.315148 spotON_sdk-0.0.4.8/spotON_sdk/data_helpers/dataframe_modifier.py
+-rw-r--r--   0        0        0      336 2023-05-22 18:01:04.746198 spotON_sdk-0.0.4.8/spotON_sdk/spotON_controller.py
+-rw-r--r--   0        0        0      250 1970-01-01 00:00:00.000000 spotON_sdk-0.0.4.8/PKG-INFO
```

### Comparing `spotON_sdk-0.0.4.7/.gitignore` & `spotON_sdk-0.0.4.8/.gitignore`

 * *Files identical despite different names*

### Comparing `spotON_sdk-0.0.4.7/LICENSE` & `spotON_sdk-0.0.4.8/LICENSE`

 * *Files identical despite different names*

### Comparing `spotON_sdk-0.0.4.7/spotON_sdk/Logic/Price/Price_Logic.py` & `spotON_sdk-0.0.4.8/spotON_sdk/Logic/Price/Price_Logic.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,24 +14,26 @@
             return ""
 
 class TimeFrame_Type(Flag):
     WHOLE_DAY = auto()
     TIMEFRAME = auto()
 
 class Timeframe(BaseModel):
+    start_hour : int 
+    end_hour : int 
     possibel_hours : List[int] = Field(default_factory=list)
 
 
 
 class Wholeday(Timeframe):
+    start_hour = 0
+    end_hour = 24 
     possibel_hours : List[int] = Field(default_factory=lambda :  [*range(0,24)])
 
 class Timeframe_as_Int(Timeframe):
-    start_hour : int 
-    end_hour : int 
 
     # validate start_hour and end_hour is not negative or greater than 24
     @validator('start_hour','end_hour')
     def start_hour_and_end_hour_must_be_between_0_and_24(cls, v):
         if v < 0 or v > 24:
             raise ValueError('start_hour and end_hour must be between 0 and 24')
         return v
```

### Comparing `spotON_sdk-0.0.4.7/spotON_sdk/Logic/Price/bidding_zones.py` & `spotON_sdk-0.0.4.8/spotON_sdk/Logic/Price/bidding_zones.py`

 * *Files identical despite different names*

### Comparing `spotON_sdk-0.0.4.7/spotON_sdk/Logic/Price/countries.py` & `spotON_sdk-0.0.4.8/spotON_sdk/Logic/Price/countries.py`

 * *Files identical despite different names*

### Comparing `spotON_sdk-0.0.4.7/spotON_sdk/Logic/Price/markets.py` & `spotON_sdk-0.0.4.8/spotON_sdk/Logic/Price/markets.py`

 * *Files identical despite different names*

### Comparing `spotON_sdk-0.0.4.7/spotON_sdk/Logic/Price/spotON_Areas.py` & `spotON_sdk-0.0.4.8/spotON_sdk/Logic/Price/spotON_Areas.py`

 * *Files identical despite different names*

### Comparing `spotON_sdk-0.0.4.7/spotON_sdk/data_helpers/BestHour.py` & `spotON_sdk-0.0.4.8/spotON_sdk/data_helpers/BestHour.py`

 * *Files identical despite different names*

### Comparing `spotON_sdk-0.0.4.7/spotON_sdk/data_helpers/dataframe_modifier.py` & `spotON_sdk-0.0.4.8/spotON_sdk/data_helpers/dataframe_modifier.py`

 * *Files identical despite different names*

