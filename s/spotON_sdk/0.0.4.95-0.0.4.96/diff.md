# Comparing `tmp/spotON_sdk-0.0.4.95.tar.gz` & `tmp/spotON_sdk-0.0.4.96.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spotON_sdk-0.0.4.95.tar", last modified: Mon May 22 19:43:31 2023, max compression
+gzip compressed data, was "spotON_sdk-0.0.4.96.tar", last modified: Mon May 22 20:36:19 2023, max compression
```

## Comparing `spotON_sdk-0.0.4.95.tar` & `spotON_sdk-0.0.4.96.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     6184 2023-05-21 14:30:18.248848 spotON_sdk-0.0.4.95/.gitignore
--rw-r--r--   0        0        0     1085 2023-05-06 14:04:24.538041 spotON_sdk-0.0.4.95/LICENSE
--rw-r--r--   0        0        0      355 2023-05-21 15:19:16.024161 spotON_sdk-0.0.4.95/pyproject.toml
--rw-r--r--   0        0        0      468 2023-05-22 17:37:16.929836 spotON_sdk-0.0.4.95/spotON_sdk/Logic/Feedback/Feedback.py
--rw-r--r--   0        0        0      122 2023-05-13 12:18:00.893425 spotON_sdk-0.0.4.95/spotON_sdk/Logic/Feedback/Sensors.py
--rw-r--r--   0        0        0      429 2023-05-13 11:38:31.810517 spotON_sdk-0.0.4.95/spotON_sdk/Logic/Feedback/Units.py
--rw-r--r--   0        0        0      145 2023-05-22 08:52:45.547083 spotON_sdk-0.0.4.95/spotON_sdk/Logic/Feedback/__init__.py
--rw-r--r--   0        0        0       93 2023-05-22 16:38:29.648297 spotON_sdk-0.0.4.95/spotON_sdk/Logic/Output/Switchtypes.py
--rw-r--r--   0        0        0      104 2023-05-22 08:52:50.913401 spotON_sdk-0.0.4.95/spotON_sdk/Logic/Output/__init__.py
--rw-r--r--   0        0        0     3561 2023-05-22 19:43:20.660487 spotON_sdk-0.0.4.95/spotON_sdk/Logic/Price/Price_Logic.py
--rw-r--r--   0        0        0      182 2023-05-22 17:37:25.105808 spotON_sdk-0.0.4.95/spotON_sdk/Logic/Price/__init__.py
--rw-r--r--   0        0        0      745 2023-05-08 10:18:24.622068 spotON_sdk-0.0.4.95/spotON_sdk/Logic/Price/bidding_zones.py
--rw-r--r--   0        0        0     4709 2023-05-22 09:10:42.883983 spotON_sdk-0.0.4.95/spotON_sdk/Logic/Price/countries.py
--rw-r--r--   0        0        0     2282 2023-05-22 09:10:36.501033 spotON_sdk-0.0.4.95/spotON_sdk/Logic/Price/markets.py
--rw-r--r--   0        0        0     6957 2023-05-17 21:52:50.903007 spotON_sdk-0.0.4.95/spotON_sdk/Logic/Price/spotON_Areas.py
--rw-r--r--   0        0        0      144 2023-05-22 18:00:58.368103 spotON_sdk-0.0.4.95/spotON_sdk/Logic/__init__.py
--rw-r--r--   0        0        0      460 2023-05-22 19:43:25.219917 spotON_sdk-0.0.4.95/spotON_sdk/__init__.py
--rw-r--r--   0        0        0      714 2023-05-22 18:11:54.358565 spotON_sdk-0.0.4.95/spotON_sdk/data_helpers/BestHour.py
--rw-r--r--   0        0        0      136 2023-05-22 08:52:16.359432 spotON_sdk-0.0.4.95/spotON_sdk/data_helpers/__init__.py
--rw-r--r--   0        0        0     1378 2023-05-22 08:52:33.315148 spotON_sdk-0.0.4.95/spotON_sdk/data_helpers/dataframe_modifier.py
--rw-r--r--   0        0        0      336 2023-05-22 18:01:04.746198 spotON_sdk-0.0.4.95/spotON_sdk/spotON_controller.py
--rw-r--r--   0        0        0      251 1970-01-01 00:00:00.000000 spotON_sdk-0.0.4.95/PKG-INFO
+-rw-r--r--   0        0        0     6184 2023-05-21 14:30:18.248848 spotON_sdk-0.0.4.96/.gitignore
+-rw-r--r--   0        0        0     1085 2023-05-06 14:04:24.538041 spotON_sdk-0.0.4.96/LICENSE
+-rw-r--r--   0        0        0      355 2023-05-21 15:19:16.024161 spotON_sdk-0.0.4.96/pyproject.toml
+-rw-r--r--   0        0        0      468 2023-05-22 17:37:16.929836 spotON_sdk-0.0.4.96/spotON_sdk/Logic/Feedback/Feedback.py
+-rw-r--r--   0        0        0      122 2023-05-13 12:18:00.893425 spotON_sdk-0.0.4.96/spotON_sdk/Logic/Feedback/Sensors.py
+-rw-r--r--   0        0        0      429 2023-05-13 11:38:31.810517 spotON_sdk-0.0.4.96/spotON_sdk/Logic/Feedback/Units.py
+-rw-r--r--   0        0        0      145 2023-05-22 08:52:45.547083 spotON_sdk-0.0.4.96/spotON_sdk/Logic/Feedback/__init__.py
+-rw-r--r--   0        0        0       93 2023-05-22 16:38:29.648297 spotON_sdk-0.0.4.96/spotON_sdk/Logic/Output/Switchtypes.py
+-rw-r--r--   0        0        0      104 2023-05-22 08:52:50.913401 spotON_sdk-0.0.4.96/spotON_sdk/Logic/Output/__init__.py
+-rw-r--r--   0        0        0     3782 2023-05-22 20:31:00.223696 spotON_sdk-0.0.4.96/spotON_sdk/Logic/Price/Price_Logic.py
+-rw-r--r--   0        0        0      182 2023-05-22 17:37:25.105808 spotON_sdk-0.0.4.96/spotON_sdk/Logic/Price/__init__.py
+-rw-r--r--   0        0        0      745 2023-05-08 10:18:24.622068 spotON_sdk-0.0.4.96/spotON_sdk/Logic/Price/bidding_zones.py
+-rw-r--r--   0        0        0     4709 2023-05-22 09:10:42.883983 spotON_sdk-0.0.4.96/spotON_sdk/Logic/Price/countries.py
+-rw-r--r--   0        0        0     2282 2023-05-22 09:10:36.501033 spotON_sdk-0.0.4.96/spotON_sdk/Logic/Price/markets.py
+-rw-r--r--   0        0        0     6957 2023-05-17 21:52:50.903007 spotON_sdk-0.0.4.96/spotON_sdk/Logic/Price/spotON_Areas.py
+-rw-r--r--   0        0        0      144 2023-05-22 18:00:58.368103 spotON_sdk-0.0.4.96/spotON_sdk/Logic/__init__.py
+-rw-r--r--   0        0        0      460 2023-05-22 20:36:14.746669 spotON_sdk-0.0.4.96/spotON_sdk/__init__.py
+-rw-r--r--   0        0        0      714 2023-05-22 18:11:54.358565 spotON_sdk-0.0.4.96/spotON_sdk/data_helpers/BestHour.py
+-rw-r--r--   0        0        0      136 2023-05-22 08:52:16.359432 spotON_sdk-0.0.4.96/spotON_sdk/data_helpers/__init__.py
+-rw-r--r--   0        0        0     1378 2023-05-22 08:52:33.315148 spotON_sdk-0.0.4.96/spotON_sdk/data_helpers/dataframe_modifier.py
+-rw-r--r--   0        0        0      336 2023-05-22 18:01:04.746198 spotON_sdk-0.0.4.96/spotON_sdk/spotON_controller.py
+-rw-r--r--   0        0        0      251 1970-01-01 00:00:00.000000 spotON_sdk-0.0.4.96/PKG-INFO
```

### Comparing `spotON_sdk-0.0.4.95/.gitignore` & `spotON_sdk-0.0.4.96/.gitignore`

 * *Files identical despite different names*

### Comparing `spotON_sdk-0.0.4.95/LICENSE` & `spotON_sdk-0.0.4.96/LICENSE`

 * *Files identical despite different names*

### Comparing `spotON_sdk-0.0.4.95/spotON_sdk/Logic/Price/Price_Logic.py` & `spotON_sdk-0.0.4.96/spotON_sdk/Logic/Price/Price_Logic.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,34 +1,20 @@
+from email.mime import base
 from typing import List, Optional,Union
 from pydantic import BaseModel, Field, validator, root_validator
 from enum import Flag, auto
 from dataclasses import dataclass, field
 from .markets import Markets,Market
 
 
-
-
-class TimeFrame_Type(Flag):
-    WHOLE_DAY = auto()
-    TIMEFRAME = auto()
-
 class Timeframe(BaseModel):
-    possibel_hours : List[int] = Field(default_factory=list)
-
-
-
-class Wholeday(Timeframe):
     start_hour :int = field(default=0)
     end_hour :int = field(default=24)
-    possibel_hours : List[int] = Field(default_factory=lambda :  [*range(0,24)])
+    possibel_hours : List[int] = Field(default_factory=list,init=False)
 
-class Timeframe_as_Int(Timeframe):
-
-    start_hour :int = field(default=0)
-    end_hour :int = field(default=24)
     # validate start_hour and end_hour is not negative or greater than 24
     @validator('start_hour','end_hour')
     def start_hour_and_end_hour_must_be_between_0_and_24(cls, v):
         if v < 0 or v > 24:
             raise ValueError('start_hour and end_hour must be between 0 and 24')
         return v
 
@@ -42,17 +28,28 @@
             
         if start < end:
             loop_Hours(start,end)
         elif start > end :
             loop_Hours(start,25)
             loop_Hours(0,end)
 
+class Wholeday(Timeframe):
+    possibel_hours : List[int] = Field(default_factory=lambda :  [*range(0,24)],init=False)
+
 
-class Segmented(Timeframe):
-    timeframe : List[Timeframe_as_Int] = Field(default_factory=list)
+class On_Hours(BaseModel):
+    timeframes_list : List[Timeframe] = Field(default_factory=list)
+    first_timeframe : Timeframe = Field(default_factory=lambda: Wholeday())
+
+    # add root validator that adds a variable first_timeframe that retrieves the first timeframe in the timeframes_list
+    @root_validator(pre=True)
+    def set_first_timeframe(cls, values):
+        values["first_timeframe"] = values["timeframes_list"][0]
+        return values
+    
     pass
 
 class Pricefinding(BaseModel):
     pass
 
 class Interrupted(Pricefinding):
     pass
@@ -60,15 +57,15 @@
 class Continuous(Pricefinding):
     week :int = Field(default=None)
     bestHour :int = Field(default=None)
 
 class Price_Logic(BaseModel):
     nr_of_hours_on: int
     market: Union[str, Market] 
-    timeframe: Timeframe = Field(default_factory=lambda: Wholeday())
+    on_hours: On_Hours = Field(default_factory=lambda: On_Hours())
     pricefinding : Continuous | Interrupted = Field(default_factory=lambda: Interrupted())
 
     resolution: float = Field(default=1)
     timeframe_longer_than_nr_of_hours_on :bool = Field(default=False)
     # root validator to set the market to the correct market object if it is a string
     @root_validator(pre=True)
     def set_market_to_market_object(cls, values):
@@ -83,19 +80,19 @@
     
     @validator('nr_of_hours_on')
     def nr_of_hours_on_must_be_greater_than_0(cls, v):
         if v == 0:
             raise ValueError('nr_of_hours_on must be greater than 0')
         return v
     
-    @root_validator(pre=True)
+    '''@root_validator(pre=True)
     def set_timeframe_type_to_whole_day_if_possible_hours_is_24(cls, values):
         if values["timeframe"].possibel_hours == [*range(0,24)]:
             values["timeframe_type"] = TimeFrame_Type.WHOLE_DAY
         return values
-
+'''
     # Validate that the timeframe is not shorter than the nr_of_hours_on
     @validator('timeframe')
     def timeframe_must_be_longer_than_nr_of_hours_on(cls, v, values):
         if values["nr_of_hours_on"] > len(v.possibel_hours):
             timeframe_longer_than_nr_of_hours_on = True
         return v
```

### Comparing `spotON_sdk-0.0.4.95/spotON_sdk/Logic/Price/bidding_zones.py` & `spotON_sdk-0.0.4.96/spotON_sdk/Logic/Price/bidding_zones.py`

 * *Files identical despite different names*

### Comparing `spotON_sdk-0.0.4.95/spotON_sdk/Logic/Price/countries.py` & `spotON_sdk-0.0.4.96/spotON_sdk/Logic/Price/countries.py`

 * *Files identical despite different names*

### Comparing `spotON_sdk-0.0.4.95/spotON_sdk/Logic/Price/markets.py` & `spotON_sdk-0.0.4.96/spotON_sdk/Logic/Price/markets.py`

 * *Files identical despite different names*

### Comparing `spotON_sdk-0.0.4.95/spotON_sdk/Logic/Price/spotON_Areas.py` & `spotON_sdk-0.0.4.96/spotON_sdk/Logic/Price/spotON_Areas.py`

 * *Files identical despite different names*

### Comparing `spotON_sdk-0.0.4.95/spotON_sdk/data_helpers/BestHour.py` & `spotON_sdk-0.0.4.96/spotON_sdk/data_helpers/BestHour.py`

 * *Files identical despite different names*

### Comparing `spotON_sdk-0.0.4.95/spotON_sdk/data_helpers/dataframe_modifier.py` & `spotON_sdk-0.0.4.96/spotON_sdk/data_helpers/dataframe_modifier.py`

 * *Files identical despite different names*

