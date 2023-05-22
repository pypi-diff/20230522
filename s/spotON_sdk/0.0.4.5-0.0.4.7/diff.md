# Comparing `tmp/spotON_sdk-0.0.4.5.tar.gz` & `tmp/spotON_sdk-0.0.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spotON_sdk-0.0.4.5.tar", last modified: Wed May 17 21:54:13 2023, max compression
+gzip compressed data, was "spotON_sdk-0.0.4.7.tar", last modified: Mon May 22 18:14:01 2023, max compression
```

## Comparing `spotON_sdk-0.0.4.5.tar` & `spotON_sdk-0.0.4.7.tar`

### file list

```diff
@@ -1,23 +1,22 @@
--rw-r--r--   0        0        0     6178 2023-05-08 22:34:46.754824 spotON_sdk-0.0.4.5/.gitignore
--rw-r--r--   0        0        0     1085 2023-05-06 14:04:24.538041 spotON_sdk-0.0.4.5/LICENSE
--rw-r--r--   0        0        0      319 2023-05-17 20:34:33.623695 spotON_sdk-0.0.4.5/pyproject.toml
--rw-r--r--   0        0        0      447 2023-05-17 21:54:07.821850 spotON_sdk-0.0.4.5/spotON_sdk/__init__.py
--rw-r--r--   0        0        0      714 2023-05-09 15:29:09.049429 spotON_sdk-0.0.4.5/spotON_sdk/data_helpers/BestHour.py
--rw-r--r--   0        0        0      122 2023-05-17 20:39:45.544124 spotON_sdk-0.0.4.5/spotON_sdk/data_helpers/__init__.py
--rw-r--r--   0        0        0     1395 2023-05-09 09:59:06.668329 spotON_sdk-0.0.4.5/spotON_sdk/data_helpers/dataframe_modifier.py
--rw-r--r--   0        0        0     3477 2023-05-13 09:52:05.827466 spotON_sdk-0.0.4.5/spotON_sdk/data_helpers/entsoe_query.py
--rw-r--r--   0        0        0     3863 2023-05-16 22:30:07.960999 spotON_sdk-0.0.4.5/spotON_sdk/settings/Config/Config.py
--rw-r--r--   0        0        0      163 2023-05-13 12:09:52.903536 spotON_sdk-0.0.4.5/spotON_sdk/settings/Config/__init__.py
--rw-r--r--   0        0        0      745 2023-05-08 10:18:24.622068 spotON_sdk-0.0.4.5/spotON_sdk/settings/Config/bidding_zones.py
--rw-r--r--   0        0        0     4796 2023-05-17 20:32:32.318040 spotON_sdk-0.0.4.5/spotON_sdk/settings/Config/countries.py
--rw-r--r--   0        0        0     2351 2023-05-17 21:53:53.693111 spotON_sdk-0.0.4.5/spotON_sdk/settings/Config/markets.py
--rw-r--r--   0        0        0     6957 2023-05-17 21:52:50.903007 spotON_sdk-0.0.4.5/spotON_sdk/settings/Config/spotON_Areas.py
--rw-r--r--   0        0        0      424 2023-05-13 12:13:49.881633 spotON_sdk-0.0.4.5/spotON_sdk/settings/Feedback/Feedback.py
--rw-r--r--   0        0        0      122 2023-05-13 12:18:00.893425 spotON_sdk-0.0.4.5/spotON_sdk/settings/Feedback/Sensors.py
--rw-r--r--   0        0        0      429 2023-05-13 11:38:31.810517 spotON_sdk-0.0.4.5/spotON_sdk/settings/Feedback/Units.py
--rw-r--r--   0        0        0      132 2023-05-13 12:05:25.975505 spotON_sdk-0.0.4.5/spotON_sdk/settings/Feedback/__init__.py
--rw-r--r--   0        0        0       93 2023-05-16 22:28:41.467762 spotON_sdk-0.0.4.5/spotON_sdk/settings/Switchtypes/Switchtypes.py
--rw-r--r--   0        0        0       91 2023-05-13 12:09:16.378665 spotON_sdk-0.0.4.5/spotON_sdk/settings/Switchtypes/__init__.py
--rw-r--r--   0        0        0      137 2023-05-13 12:11:13.611869 spotON_sdk-0.0.4.5/spotON_sdk/settings/__init__.py
--rw-r--r--   0        0        0      342 2023-05-13 12:13:23.297526 spotON_sdk-0.0.4.5/spotON_sdk/spotON_controller.py
--rw-r--r--   0        0        0      218 1970-01-01 00:00:00.000000 spotON_sdk-0.0.4.5/PKG-INFO
+-rw-r--r--   0        0        0     6184 2023-05-21 14:30:18.248848 spotON_sdk-0.0.4.7/.gitignore
+-rw-r--r--   0        0        0     1085 2023-05-06 14:04:24.538041 spotON_sdk-0.0.4.7/LICENSE
+-rw-r--r--   0        0        0      355 2023-05-21 15:19:16.024161 spotON_sdk-0.0.4.7/pyproject.toml
+-rw-r--r--   0        0        0      468 2023-05-22 17:37:16.929836 spotON_sdk-0.0.4.7/spotON_sdk/Logic/Feedback/Feedback.py
+-rw-r--r--   0        0        0      122 2023-05-13 12:18:00.893425 spotON_sdk-0.0.4.7/spotON_sdk/Logic/Feedback/Sensors.py
+-rw-r--r--   0        0        0      429 2023-05-13 11:38:31.810517 spotON_sdk-0.0.4.7/spotON_sdk/Logic/Feedback/Units.py
+-rw-r--r--   0        0        0      145 2023-05-22 08:52:45.547083 spotON_sdk-0.0.4.7/spotON_sdk/Logic/Feedback/__init__.py
+-rw-r--r--   0        0        0       93 2023-05-22 16:38:29.648297 spotON_sdk-0.0.4.7/spotON_sdk/Logic/Output/Switchtypes.py
+-rw-r--r--   0        0        0      104 2023-05-22 08:52:50.913401 spotON_sdk-0.0.4.7/spotON_sdk/Logic/Output/__init__.py
+-rw-r--r--   0        0        0     3285 2023-05-22 09:14:50.783679 spotON_sdk-0.0.4.7/spotON_sdk/Logic/Price/Price_Logic.py
+-rw-r--r--   0        0        0      182 2023-05-22 17:37:25.105808 spotON_sdk-0.0.4.7/spotON_sdk/Logic/Price/__init__.py
+-rw-r--r--   0        0        0      745 2023-05-08 10:18:24.622068 spotON_sdk-0.0.4.7/spotON_sdk/Logic/Price/bidding_zones.py
+-rw-r--r--   0        0        0     4709 2023-05-22 09:10:42.883983 spotON_sdk-0.0.4.7/spotON_sdk/Logic/Price/countries.py
+-rw-r--r--   0        0        0     2282 2023-05-22 09:10:36.501033 spotON_sdk-0.0.4.7/spotON_sdk/Logic/Price/markets.py
+-rw-r--r--   0        0        0     6957 2023-05-17 21:52:50.903007 spotON_sdk-0.0.4.7/spotON_sdk/Logic/Price/spotON_Areas.py
+-rw-r--r--   0        0        0      144 2023-05-22 18:00:58.368103 spotON_sdk-0.0.4.7/spotON_sdk/Logic/__init__.py
+-rw-r--r--   0        0        0      458 2023-05-22 18:13:16.726672 spotON_sdk-0.0.4.7/spotON_sdk/__init__.py
+-rw-r--r--   0        0        0      714 2023-05-22 18:11:54.358565 spotON_sdk-0.0.4.7/spotON_sdk/data_helpers/BestHour.py
+-rw-r--r--   0        0        0      136 2023-05-22 08:52:16.359432 spotON_sdk-0.0.4.7/spotON_sdk/data_helpers/__init__.py
+-rw-r--r--   0        0        0     1378 2023-05-22 08:52:33.315148 spotON_sdk-0.0.4.7/spotON_sdk/data_helpers/dataframe_modifier.py
+-rw-r--r--   0        0        0      336 2023-05-22 18:01:04.746198 spotON_sdk-0.0.4.7/spotON_sdk/spotON_controller.py
+-rw-r--r--   0        0        0      250 1970-01-01 00:00:00.000000 spotON_sdk-0.0.4.7/PKG-INFO
```

### Comparing `spotON_sdk-0.0.4.5/.gitignore` & `spotON_sdk-0.0.4.7/.gitignore`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 spotOn-venv/
 tests/
+.venv
 
 # Byte-compiled / optimized / DLL files
 __pycache__/
 *.py[cod]
 *$py.class
 
 # C extensions
```

### Comparing `spotON_sdk-0.0.4.5/LICENSE` & `spotON_sdk-0.0.4.7/LICENSE`

 * *Files identical despite different names*

### Comparing `spotON_sdk-0.0.4.5/spotON_sdk/data_helpers/BestHour.py` & `spotON_sdk-0.0.4.7/spotON_sdk/data_helpers/BestHour.py`

 * *Files identical despite different names*

### Comparing `spotON_sdk-0.0.4.5/spotON_sdk/data_helpers/dataframe_modifier.py` & `spotON_sdk-0.0.4.7/spotON_sdk/data_helpers/dataframe_modifier.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,15 +7,14 @@
     df['Week'] = df.index.isocalendar().week
     df['Day'] = df.index.day
     df["Hour"] = df.index.hour
 
     # Calculate the daily average price and store it in a new DataFrame
     daily_avg = df.resample('D')['Price'].mean()
 
-    df,daily_avg
     # Merge the two DataFrames using the DateTime index with a left join
     merged_df = pd.merge(df, daily_avg, left_index=True, right_index=True, how='left', suffixes=('', '_daily_AVG'))
 
     # Forward fill the missing values in the 'EXXA Price_daily' column
     merged_df['Price_daily_AVG'].fillna(method='ffill', inplace=True)
     return merged_df
```

### Comparing `spotON_sdk-0.0.4.5/spotON_sdk/settings/Config/bidding_zones.py` & `spotON_sdk-0.0.4.7/spotON_sdk/Logic/Price/bidding_zones.py`

 * *Files identical despite different names*

### Comparing `spotON_sdk-0.0.4.5/spotON_sdk/settings/Config/countries.py` & `spotON_sdk-0.0.4.7/spotON_sdk/Logic/Price/countries.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,35 +1,40 @@
 from dataclasses import dataclass, field
 
 from typing import Any,Optional,List
 from .spotON_Areas import spotON_Area
+from typing import Tuple
 
 import pandas as pd
 import pytz
 
 def _country_code_to_emoji(country_code):
     OFFSET = 127397
     return ''.join(chr(ord(c) + OFFSET) for c in country_code.upper())
 
 @dataclass
 class Country:
     capital: str
     country_code: str
     country_name: str
-    UTC_time_difference: int = field(init=False)
+    UTC_time_difference: float = field(init=False)
     
-    def calculate_utc_time_difference(self) -> Optional[pd.Timedelta]:
+    def calculate_utc_time_difference(self) -> Tuple[pd.Timedelta,float]:
         try:
             timezone = f"Europe/{self.capital}"
             local_tz = pytz.timezone(timezone)
             utc_dt = pd.Timestamp.utcnow().to_pydatetime()
             local_dt = utc_dt.astimezone(local_tz)
-            UTC_time_difference = (local_dt.utcoffset().total_seconds()) // 3600
-            delta = pd.Timedelta(hours=UTC_time_difference)
-            return delta, UTC_time_difference
+            local_dt_Offset = local_dt.utcoffset()
+            if local_dt_Offset != None:
+                UTC_time_difference = (local_dt_Offset.total_seconds()) // 3600
+                delta = pd.Timedelta(hours=UTC_time_difference)
+                return delta, UTC_time_difference
+            else:
+                raise Exception
 
         except:
             print(f"{self.capital} not found in European capitals.")
             default_delta = pd.Timedelta(hours=0)
             default_UTC_time_difference = 0
             return default_delta, default_UTC_time_difference
 
@@ -87,18 +92,7 @@
     Sweden = Country(capital="Stockholm", country_code="SE", country_name="Sweden")
 
     return_List= [Austria, Belgium, Bulgaria, Croatia, Cyprus, Czech_republic, Denmark, Estonia, Finland, France, Germany, Greece, Hungary, Ireland, Italy, Latvia, Lithuania, Luxembourg, Netherlands, Poland, Portugal, Romania, Slovakia, Slovenia, Spain, Sweden]
 
 
 
 
-def return_All_Areas(filterstring:str ="MBA"):
-        
-    result = []
-    for area in spotON_Area:
-        #print (area.name, area.meaning)
-        if filterstring in area.meaning:
-            result.append(area)
-            print (area.name)
-
-    return result
-
```

### Comparing `spotON_sdk-0.0.4.5/spotON_sdk/settings/Config/markets.py` & `spotON_sdk-0.0.4.7/spotON_sdk/Logic/Price/markets.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from .countries import *
 from .bidding_zones import bidding_zones
 
 @dataclass
 class Market():
     area:Area_details
     country :Country
-    alias : List[str] | None = None
+    alias : str | None = None
     area_code :str = field(init=False)
     country_code : str = field(init=False)
     region_code : str | None = field(init=False,default=None)
     cities : str = field(init=False)
 
     def __post_init__(self):
         self.area_code = self.area.name
@@ -34,41 +34,40 @@
 
 
         self.name = f"{self.country.emoji} {self.country.country_name} {self.area_code} {self.cities}"
         self.name = f"{self.country.emoji} {self.country.country_name}"
 
         #self.get_Market_by_area_code(self.area.name)
 
-dataclass
+@dataclass
 class Markets():
     austria = Market(spotON_Area.AT,all_Countries.Austria)
     germany = Market(spotON_Area.DE_LU,all_Countries.Germany,alias="DE_LU")
     #luxembourg = Market(Area.DE_LU,Luxembourg)
     sweden1 = Market(spotON_Area.SE_1,all_Countries.Sweden)
     #sweden2 = Market(Area.SE_2,Sweden)
     #sweden3 = Market(Area.SE_3,Sweden)
     #sweden4 = Market(Area.SE_4,Sweden)
     markets_List = [value for key, value in vars().items() if isinstance(value, Market)]
     merged_Markets = []
 
     @staticmethod
-    def get_Market_by_area_code(area_code: str) -> Optional[Market]:
-        for country in Markets.markets_List:
-            #print (f"Try to find {area_code =} in {country}")
-            if country.country_code == area_code or country.alias == area_code:
-                return country
+    def get_market_by_name(name: str) -> Optional[Market]:
+        for market in Markets.markets_List:
+            if market.name == name:
+                return market
+
+        return None
+
+    @staticmethod
+    def get_market_by_code(area_code: str) -> Optional[Market]:
+        for market in Markets.markets_List:
+            #print (f"Try to find {area_code =} in {market}")
+            if market.country_code == area_code or market.alias == area_code:
+                return market
 
         return None
 
 
-def return_All_Areas(filterstring:str ="MBA"):
-        
-    result = []
-    for area in spotON_Area:
-        #print (area.name, area.meaning)
-        if filterstring in area.meaning:
-            result.append(area)
-            print (area.name)
 
-    return result
```

### Comparing `spotON_sdk-0.0.4.5/spotON_sdk/settings/Config/spotON_Areas.py` & `spotON_sdk-0.0.4.7/spotON_sdk/Logic/Price/spotON_Areas.py`

 * *Files identical despite different names*

