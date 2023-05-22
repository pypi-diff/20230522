# Comparing `tmp/spotON_sdk-0.0.4.8.tar.gz` & `tmp/spotON_sdk-0.0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spotON_sdk-0.0.4.8.tar", last modified: Mon May 22 18:47:32 2023, max compression
+gzip compressed data, was "spotON_sdk-0.0.4.9.tar", last modified: Mon May 22 18:55:07 2023, max compression
```

## Comparing `spotON_sdk-0.0.4.8.tar` & `spotON_sdk-0.0.4.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     6184 2023-05-21 14:30:18.248848 spotON_sdk-0.0.4.8/.gitignore
--rw-r--r--   0        0        0     1085 2023-05-06 14:04:24.538041 spotON_sdk-0.0.4.8/LICENSE
--rw-r--r--   0        0        0      355 2023-05-21 15:19:16.024161 spotON_sdk-0.0.4.8/pyproject.toml
--rw-r--r--   0        0        0      468 2023-05-22 17:37:16.929836 spotON_sdk-0.0.4.8/spotON_sdk/Logic/Feedback/Feedback.py
--rw-r--r--   0        0        0      122 2023-05-13 12:18:00.893425 spotON_sdk-0.0.4.8/spotON_sdk/Logic/Feedback/Sensors.py
--rw-r--r--   0        0        0      429 2023-05-13 11:38:31.810517 spotON_sdk-0.0.4.8/spotON_sdk/Logic/Feedback/Units.py
--rw-r--r--   0        0        0      145 2023-05-22 08:52:45.547083 spotON_sdk-0.0.4.8/spotON_sdk/Logic/Feedback/__init__.py
--rw-r--r--   0        0        0       93 2023-05-22 16:38:29.648297 spotON_sdk-0.0.4.8/spotON_sdk/Logic/Output/Switchtypes.py
--rw-r--r--   0        0        0      104 2023-05-22 08:52:50.913401 spotON_sdk-0.0.4.8/spotON_sdk/Logic/Output/__init__.py
--rw-r--r--   0        0        0     3323 2023-05-22 18:47:21.679789 spotON_sdk-0.0.4.8/spotON_sdk/Logic/Price/Price_Logic.py
--rw-r--r--   0        0        0      182 2023-05-22 17:37:25.105808 spotON_sdk-0.0.4.8/spotON_sdk/Logic/Price/__init__.py
--rw-r--r--   0        0        0      745 2023-05-08 10:18:24.622068 spotON_sdk-0.0.4.8/spotON_sdk/Logic/Price/bidding_zones.py
--rw-r--r--   0        0        0     4709 2023-05-22 09:10:42.883983 spotON_sdk-0.0.4.8/spotON_sdk/Logic/Price/countries.py
--rw-r--r--   0        0        0     2282 2023-05-22 09:10:36.501033 spotON_sdk-0.0.4.8/spotON_sdk/Logic/Price/markets.py
--rw-r--r--   0        0        0     6957 2023-05-17 21:52:50.903007 spotON_sdk-0.0.4.8/spotON_sdk/Logic/Price/spotON_Areas.py
--rw-r--r--   0        0        0      144 2023-05-22 18:00:58.368103 spotON_sdk-0.0.4.8/spotON_sdk/Logic/__init__.py
--rw-r--r--   0        0        0      458 2023-05-22 18:47:28.039092 spotON_sdk-0.0.4.8/spotON_sdk/__init__.py
--rw-r--r--   0        0        0      714 2023-05-22 18:11:54.358565 spotON_sdk-0.0.4.8/spotON_sdk/data_helpers/BestHour.py
--rw-r--r--   0        0        0      136 2023-05-22 08:52:16.359432 spotON_sdk-0.0.4.8/spotON_sdk/data_helpers/__init__.py
--rw-r--r--   0        0        0     1378 2023-05-22 08:52:33.315148 spotON_sdk-0.0.4.8/spotON_sdk/data_helpers/dataframe_modifier.py
--rw-r--r--   0        0        0      336 2023-05-22 18:01:04.746198 spotON_sdk-0.0.4.8/spotON_sdk/spotON_controller.py
--rw-r--r--   0        0        0      250 1970-01-01 00:00:00.000000 spotON_sdk-0.0.4.8/PKG-INFO
+-rw-r--r--   0        0        0     6184 2023-05-21 14:30:18.248848 spotON_sdk-0.0.4.9/.gitignore
+-rw-r--r--   0        0        0     1085 2023-05-06 14:04:24.538041 spotON_sdk-0.0.4.9/LICENSE
+-rw-r--r--   0        0        0      355 2023-05-21 15:19:16.024161 spotON_sdk-0.0.4.9/pyproject.toml
+-rw-r--r--   0        0        0      468 2023-05-22 17:37:16.929836 spotON_sdk-0.0.4.9/spotON_sdk/Logic/Feedback/Feedback.py
+-rw-r--r--   0        0        0      122 2023-05-13 12:18:00.893425 spotON_sdk-0.0.4.9/spotON_sdk/Logic/Feedback/Sensors.py
+-rw-r--r--   0        0        0      429 2023-05-13 11:38:31.810517 spotON_sdk-0.0.4.9/spotON_sdk/Logic/Feedback/Units.py
+-rw-r--r--   0        0        0      145 2023-05-22 08:52:45.547083 spotON_sdk-0.0.4.9/spotON_sdk/Logic/Feedback/__init__.py
+-rw-r--r--   0        0        0       93 2023-05-22 16:38:29.648297 spotON_sdk-0.0.4.9/spotON_sdk/Logic/Output/Switchtypes.py
+-rw-r--r--   0        0        0      104 2023-05-22 08:52:50.913401 spotON_sdk-0.0.4.9/spotON_sdk/Logic/Output/__init__.py
+-rw-r--r--   0        0        0     3474 2023-05-22 18:54:53.721491 spotON_sdk-0.0.4.9/spotON_sdk/Logic/Price/Price_Logic.py
+-rw-r--r--   0        0        0      182 2023-05-22 17:37:25.105808 spotON_sdk-0.0.4.9/spotON_sdk/Logic/Price/__init__.py
+-rw-r--r--   0        0        0      745 2023-05-08 10:18:24.622068 spotON_sdk-0.0.4.9/spotON_sdk/Logic/Price/bidding_zones.py
+-rw-r--r--   0        0        0     4709 2023-05-22 09:10:42.883983 spotON_sdk-0.0.4.9/spotON_sdk/Logic/Price/countries.py
+-rw-r--r--   0        0        0     2282 2023-05-22 09:10:36.501033 spotON_sdk-0.0.4.9/spotON_sdk/Logic/Price/markets.py
+-rw-r--r--   0        0        0     6957 2023-05-17 21:52:50.903007 spotON_sdk-0.0.4.9/spotON_sdk/Logic/Price/spotON_Areas.py
+-rw-r--r--   0        0        0      144 2023-05-22 18:00:58.368103 spotON_sdk-0.0.4.9/spotON_sdk/Logic/__init__.py
+-rw-r--r--   0        0        0      458 2023-05-22 18:54:59.481862 spotON_sdk-0.0.4.9/spotON_sdk/__init__.py
+-rw-r--r--   0        0        0      714 2023-05-22 18:11:54.358565 spotON_sdk-0.0.4.9/spotON_sdk/data_helpers/BestHour.py
+-rw-r--r--   0        0        0      136 2023-05-22 08:52:16.359432 spotON_sdk-0.0.4.9/spotON_sdk/data_helpers/__init__.py
+-rw-r--r--   0        0        0     1378 2023-05-22 08:52:33.315148 spotON_sdk-0.0.4.9/spotON_sdk/data_helpers/dataframe_modifier.py
+-rw-r--r--   0        0        0      336 2023-05-22 18:01:04.746198 spotON_sdk-0.0.4.9/spotON_sdk/spotON_controller.py
+-rw-r--r--   0        0        0      250 1970-01-01 00:00:00.000000 spotON_sdk-0.0.4.9/PKG-INFO
```

### Comparing `spotON_sdk-0.0.4.8/.gitignore` & `spotON_sdk-0.0.4.9/.gitignore`

 * *Files identical despite different names*

### Comparing `spotON_sdk-0.0.4.8/LICENSE` & `spotON_sdk-0.0.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `spotON_sdk-0.0.4.8/spotON_sdk/Logic/Price/Price_Logic.py` & `spotON_sdk-0.0.4.9/spotON_sdk/Logic/Price/Price_Logic.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,36 +1,30 @@
 from typing import List, Optional,Union
 from pydantic import BaseModel, Field, validator, root_validator
 from enum import Flag, auto
 from dataclasses import dataclass, field
 from .markets import Markets,Market
 
-@dataclass
-class TimeFrameValidation():
-    passed :bool
-    def return_Validation_Result(self):
-        if self.passed == False:
-            return "<br> 🚨 <mark> Your Timeframe is SHORTER than your desired ON Time</mark> "
-        else:
-            return ""
+
+
 
 class TimeFrame_Type(Flag):
     WHOLE_DAY = auto()
     TIMEFRAME = auto()
 
 class Timeframe(BaseModel):
     start_hour : int 
     end_hour : int 
     possibel_hours : List[int] = Field(default_factory=list)
 
 
 
 class Wholeday(Timeframe):
-    start_hour = 0
-    end_hour = 24 
+    start_hour :int = field(default=0)
+    end_hour :int = field(default=24)
     possibel_hours : List[int] = Field(default_factory=lambda :  [*range(0,24)])
 
 class Timeframe_as_Int(Timeframe):
 
     # validate start_hour and end_hour is not negative or greater than 24
     @validator('start_hour','end_hour')
     def start_hour_and_end_hour_must_be_between_0_and_24(cls, v):
@@ -69,15 +63,15 @@
 class Price_Logic(BaseModel):
     nr_of_hours_on: int
     market: Union[str, Market] 
     timeframe: Timeframe = Field(default_factory=lambda: Wholeday())
     pricefinding : Pricefinding = Field(default_factory=lambda: Interrupted())
 
     resolution: float = Field(default=1)
-
+    timeframe_longer_than_nr_of_hours_on :bool = Field(default=False)
     # root validator to set the market to the correct market object if it is a string
     @root_validator(pre=True)
     def set_market_to_market_object(cls, values):
         if isinstance(values["market"], str):
             result = Markets.get_market_by_name(values["market"])
             result = Markets.get_market_by_code(values["market"])
             if result is None:
@@ -93,7 +87,14 @@
         return v
     
     @root_validator(pre=True)
     def set_timeframe_type_to_whole_day_if_possible_hours_is_24(cls, values):
         if values["timeframe"].possibel_hours == [*range(0,24)]:
             values["timeframe_type"] = TimeFrame_Type.WHOLE_DAY
         return values
+
+    # Validate that the timeframe is not shorter than the nr_of_hours_on
+    @validator('timeframe')
+    def timeframe_must_be_longer_than_nr_of_hours_on(cls, v, values):
+        if values["nr_of_hours_on"] > len(v.possibel_hours):
+            timeframe_longer_than_nr_of_hours_on = True
+        return v
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `spotON_sdk-0.0.4.8/spotON_sdk/Logic/Price/bidding_zones.py` & `spotON_sdk-0.0.4.9/spotON_sdk/Logic/Price/bidding_zones.py`

 * *Files identical despite different names*

### Comparing `spotON_sdk-0.0.4.8/spotON_sdk/Logic/Price/countries.py` & `spotON_sdk-0.0.4.9/spotON_sdk/Logic/Price/countries.py`

 * *Files identical despite different names*

### Comparing `spotON_sdk-0.0.4.8/spotON_sdk/Logic/Price/markets.py` & `spotON_sdk-0.0.4.9/spotON_sdk/Logic/Price/markets.py`

 * *Files identical despite different names*

### Comparing `spotON_sdk-0.0.4.8/spotON_sdk/Logic/Price/spotON_Areas.py` & `spotON_sdk-0.0.4.9/spotON_sdk/Logic/Price/spotON_Areas.py`

 * *Files identical despite different names*

### Comparing `spotON_sdk-0.0.4.8/spotON_sdk/data_helpers/BestHour.py` & `spotON_sdk-0.0.4.9/spotON_sdk/data_helpers/BestHour.py`

 * *Files identical despite different names*

### Comparing `spotON_sdk-0.0.4.8/spotON_sdk/data_helpers/dataframe_modifier.py` & `spotON_sdk-0.0.4.9/spotON_sdk/data_helpers/dataframe_modifier.py`

 * *Files identical despite different names*

