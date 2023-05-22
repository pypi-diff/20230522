# Comparing `tmp/longitudinal_trends-0.1.7.tar.gz` & `tmp/longitudinal_trends-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "longitudinal_trends-0.1.7.tar", last modified: Wed May 17 16:31:31 2023, max compression
+gzip compressed data, was "longitudinal_trends-0.1.8.tar", last modified: Mon May 22 17:29:08 2023, max compression
```

## Comparing `longitudinal_trends-0.1.7.tar` & `longitudinal_trends-0.1.8.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0 msakir    (1000) msakir    (1000)        0 2023-05-17 16:31:31.356108 longitudinal_trends-0.1.7/
--rwxrwxrwx   0 msakir    (1000) msakir    (1000)     1104 2023-03-18 15:04:53.000000 longitudinal_trends-0.1.7/LICENSE
--rwxrwxrwx   0 msakir    (1000) msakir    (1000)       34 2023-03-18 16:38:44.000000 longitudinal_trends-0.1.7/MANIFEST.in
--rwxrwxrwx   0 msakir    (1000) msakir    (1000)    10290 2023-05-17 16:31:31.340478 longitudinal_trends-0.1.7/PKG-INFO
--rwxrwxrwx   0 msakir    (1000) msakir    (1000)     9719 2023-05-05 08:12:31.000000 longitudinal_trends-0.1.7/README.md
-drwxrwxrwx   0 msakir    (1000) msakir    (1000)        0 2023-05-17 16:31:30.991709 longitudinal_trends-0.1.7/longitudinal_trends/
--rwxrwxrwx   0 msakir    (1000) msakir    (1000)    19451 2023-05-16 17:25:26.000000 longitudinal_trends-0.1.7/longitudinal_trends/__init__.py
-drwxrwxrwx   0 msakir    (1000) msakir    (1000)        0 2023-05-17 16:31:31.277980 longitudinal_trends-0.1.7/longitudinal_trends.egg-info/
--rwxrwxrwx   0 msakir    (1000) msakir    (1000)    10290 2023-05-17 16:31:30.000000 longitudinal_trends-0.1.7/longitudinal_trends.egg-info/PKG-INFO
--rwxrwxrwx   0 msakir    (1000) msakir    (1000)      307 2023-05-17 16:31:30.000000 longitudinal_trends-0.1.7/longitudinal_trends.egg-info/SOURCES.txt
--rwxrwxrwx   0 msakir    (1000) msakir    (1000)        1 2023-05-17 16:31:30.000000 longitudinal_trends-0.1.7/longitudinal_trends.egg-info/dependency_links.txt
--rwxrwxrwx   0 msakir    (1000) msakir    (1000)       45 2023-05-17 16:31:30.000000 longitudinal_trends-0.1.7/longitudinal_trends.egg-info/requires.txt
--rwxrwxrwx   0 msakir    (1000) msakir    (1000)       20 2023-05-17 16:31:30.000000 longitudinal_trends-0.1.7/longitudinal_trends.egg-info/top_level.txt
--rwxrwxrwx   0 msakir    (1000) msakir    (1000)     1141 2023-05-17 16:30:52.000000 longitudinal_trends-0.1.7/pyproject.toml
--rwxrwxrwx   0 msakir    (1000) msakir    (1000)       44 2023-04-15 18:04:14.000000 longitudinal_trends-0.1.7/requirements.txt
--rwxrwxrwx   0 msakir    (1000) msakir    (1000)       38 2023-05-17 16:31:31.356108 longitudinal_trends-0.1.7/setup.cfg
+drwxrwxrwx   0 msakir    (1000) msakir    (1000)        0 2023-05-22 17:29:08.665490 longitudinal_trends-0.1.8/
+-rwxrwxrwx   0 msakir    (1000) msakir    (1000)     1104 2023-03-18 15:04:53.000000 longitudinal_trends-0.1.8/LICENSE
+-rwxrwxrwx   0 msakir    (1000) msakir    (1000)       34 2023-03-18 16:38:44.000000 longitudinal_trends-0.1.8/MANIFEST.in
+-rwxrwxrwx   0 msakir    (1000) msakir    (1000)    10905 2023-05-22 17:29:08.649851 longitudinal_trends-0.1.8/PKG-INFO
+-rwxrwxrwx   0 msakir    (1000) msakir    (1000)    10346 2023-05-22 16:11:36.000000 longitudinal_trends-0.1.8/README.md
+drwxrwxrwx   0 msakir    (1000) msakir    (1000)        0 2023-05-22 17:29:08.335440 longitudinal_trends-0.1.8/longitudinal_trends/
+-rwxrwxrwx   0 msakir    (1000) msakir    (1000)    17974 2023-05-22 16:05:00.000000 longitudinal_trends-0.1.8/longitudinal_trends/__init__.py
+drwxrwxrwx   0 msakir    (1000) msakir    (1000)        0 2023-05-22 17:29:08.586952 longitudinal_trends-0.1.8/longitudinal_trends.egg-info/
+-rwxrwxrwx   0 msakir    (1000) msakir    (1000)    10905 2023-05-22 17:29:07.000000 longitudinal_trends-0.1.8/longitudinal_trends.egg-info/PKG-INFO
+-rwxrwxrwx   0 msakir    (1000) msakir    (1000)      307 2023-05-22 17:29:08.000000 longitudinal_trends-0.1.8/longitudinal_trends.egg-info/SOURCES.txt
+-rwxrwxrwx   0 msakir    (1000) msakir    (1000)        1 2023-05-22 17:29:07.000000 longitudinal_trends-0.1.8/longitudinal_trends.egg-info/dependency_links.txt
+-rwxrwxrwx   0 msakir    (1000) msakir    (1000)       45 2023-05-22 17:29:07.000000 longitudinal_trends-0.1.8/longitudinal_trends.egg-info/requires.txt
+-rwxrwxrwx   0 msakir    (1000) msakir    (1000)       20 2023-05-22 17:29:07.000000 longitudinal_trends-0.1.8/longitudinal_trends.egg-info/top_level.txt
+-rwxrwxrwx   0 msakir    (1000) msakir    (1000)     1141 2023-05-22 16:11:52.000000 longitudinal_trends-0.1.8/pyproject.toml
+-rwxrwxrwx   0 msakir    (1000) msakir    (1000)       44 2023-04-15 18:04:14.000000 longitudinal_trends-0.1.8/requirements.txt
+-rwxrwxrwx   0 msakir    (1000) msakir    (1000)       38 2023-05-22 17:29:08.665490 longitudinal_trends-0.1.8/setup.cfg
```

### Comparing `longitudinal_trends-0.1.7/LICENSE` & `longitudinal_trends-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `longitudinal_trends-0.1.7/PKG-INFO` & `longitudinal_trends-0.1.8/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: longitudinal_trends
-Version: 0.1.7
+Version: 0.1.8
 Summary: Generate long-term longitudinal Google Trends Data
 Author: Mohammad Saleh Ahsan Sakir, Taeyong Park
 Author-email: ahsansakir506@gmail.com, taeyongp@andrew.cmu.edu
 License: MIT
 Project-URL: homepage, https://github.com/Mohammad-sakir/longitudinalTrends
 Keywords: longitudinal-trends longitudinal data python google-trends-api google-trends search-data
 Classifier: Programming Language :: Python :: 3
@@ -32,14 +32,15 @@
 
 ## Table of contents
 
 * Installation
 * Requirements
 * Initiate `longitudinal_trends`
 * Methods
+  * WARNING
   * `cross_section`
   * `time_series`
   * `concat_time_series`
   * `convert_cross_section`
   * `all_in_one_method`
 * Caveats
 * Credits
@@ -84,25 +85,36 @@
   - Date to end at
 - `data_format`
   - Time basis query
   - Can choose only one from the list: ['daily', 'weekly', 'monthly']
 
 ## Methods
 
+### WARNING
+
+Please make sure to run the methods in the following sequence:
+
+- `cross_section`
+- `time_series`
+- `concat_time_series`
+- `convert_time_series`
+
+We have noticed some unusual behaviors if not run in the given sequence. Firstly `concat_time_series` depends on `time_series` and `convert_cross_section` depends on all the three. We have noticed if `time_series` is ran before `cross_section` then sometimes the output gets incluenced by `time_series` parameters. We are troubleshooting the issue. Until then, please follow the sequence to attain the expected result.
+
 ### cross_section
 
 ```python
 day_data.cross_section(geo='US', resolution="REGION")
 ```
 
 This method will collect cross section data of the given keyword and timeline. It calls `pytrends.interest_by_region()` method from pytrends. The data is automatically saved in →  'folder_name'/'data_format'/by_region. Each file has data for the given region/countries all the country/state google trends index for 1 day/week/month. The filenames tells the date of the data time period and also has an indication of number of day/week/month.
 
 For more information on pytrends `interest_by_region()` method, [check here](https://pypi.org/project/pytrends/#interest-by-region).
 
-**PS**: *This method takes a long time to finish running. For example, it takes around 5 hours to collect 350 days of daily data. The time is mainly due to Google Trends API rate limit.*
+**PS**: *This method takes a long time to finish running. For example, it takes around 5 hours to collect 350 days of daily data. The time is mainly due to Google Trends API rate limit and resetting the limit.*
 
 **Parameters**
 
 - `geo`
   - Country/Region to collect data from. If left empty, then result will be worldwide i.e. data will be collected for all country. If left empty, defaults to worldwide country level.
 - `resolution`
   - 'COUNTRY' returns country level data
```

### Comparing `longitudinal_trends-0.1.7/README.md` & `longitudinal_trends-0.1.8/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 
 ## Table of contents
 
 * Installation
 * Requirements
 * Initiate `longitudinal_trends`
 * Methods
+  * WARNING
   * `cross_section`
   * `time_series`
   * `concat_time_series`
   * `convert_cross_section`
   * `all_in_one_method`
 * Caveats
 * Credits
@@ -66,25 +67,36 @@
   - Date to end at
 - `data_format`
   - Time basis query
   - Can choose only one from the list: ['daily', 'weekly', 'monthly']
 
 ## Methods
 
+### WARNING
+
+Please make sure to run the methods in the following sequence:
+
+- `cross_section`
+- `time_series`
+- `concat_time_series`
+- `convert_time_series`
+
+We have noticed some unusual behaviors if not run in the given sequence. Firstly `concat_time_series` depends on `time_series` and `convert_cross_section` depends on all the three. We have noticed if `time_series` is ran before `cross_section` then sometimes the output gets incluenced by `time_series` parameters. We are troubleshooting the issue. Until then, please follow the sequence to attain the expected result.
+
 ### cross_section
 
 ```python
 day_data.cross_section(geo='US', resolution="REGION")
 ```
 
 This method will collect cross section data of the given keyword and timeline. It calls `pytrends.interest_by_region()` method from pytrends. The data is automatically saved in →  'folder_name'/'data_format'/by_region. Each file has data for the given region/countries all the country/state google trends index for 1 day/week/month. The filenames tells the date of the data time period and also has an indication of number of day/week/month.
 
 For more information on pytrends `interest_by_region()` method, [check here](https://pypi.org/project/pytrends/#interest-by-region).
 
-**PS**: *This method takes a long time to finish running. For example, it takes around 5 hours to collect 350 days of daily data. The time is mainly due to Google Trends API rate limit.*
+**PS**: *This method takes a long time to finish running. For example, it takes around 5 hours to collect 350 days of daily data. The time is mainly due to Google Trends API rate limit and resetting the limit.*
 
 **Parameters**
 
 - `geo`
   - Country/Region to collect data from. If left empty, then result will be worldwide i.e. data will be collected for all country. If left empty, defaults to worldwide country level.
 - `resolution`
   - 'COUNTRY' returns country level data
```

### Comparing `longitudinal_trends-0.1.7/longitudinal_trends/__init__.py` & `longitudinal_trends-0.1.8/longitudinal_trends/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,36 +1,7 @@
-# # import datetime as dt
-
-# # from longitudinal_trends import RequestTrends
-
-# # day_data = RequestTrends('UBI', 'UBI', 'UBI_folder', dt.datetime(2012, 1, 1), dt.datetime(2022,12,31), 'daily') #4017 days
-
-# # day_data.time_series(reference_geo_code=" ")
-
-# import datetime as dt
-# from longitudinal_trends import RequestTrends
-
-# # # day_data = RequestTrends('Anxiety', '/m/0k_9', dt.datetime(2021, 11, 1), dt.datetime(2022,10,24), 'daily') #358 Days
-# # day_data = RequestTrends('UBI', 'UBI', 'UBI_folder', dt.datetime(2012, 1, 1), dt.datetime(2022,12,31), 'daily') #4017 days
-# # week_data = RequestTrends('Anxiety', '/m/0k_9', dt.datetime(2016,11,21), dt.datetime(2022,10,24), 'weekly') #2163 Days | 309 Weeks
-# month_data = RequestTrends('UBI', 'universal basic income', 'UBI_folder', dt.datetime(2012, 1, 1), dt.datetime(2022,12,31), 'monthly') #1890 Days | 63 Months
-
-# # day_data.cross_section('US')
-# # day_data.cross_section('US-AL')
-# # week_data.one_click_function('US-AL')
-# # week_data = RequestTrends('UBI', 'UBI', dt.datetime(2016,11,21), dt.datetime(2022,10,24), 'weekly') #2163 Days | 310 Weeks
-# # week_data.all_in_one_method()
-# # day_data.all_in_one_method(reference_geo_code="IT")
-# # week_data.convert_cross_section("US-AK")
-# # day_data.convert_cross_section("US-AL")
-# # day_data.time_series(reference_geo_code=" ")
-# # start, end = dt.datetime(2012, 1, 1), dt.datetime(2022,12,31)
-# # print(end-start)
-# month_data.time_series(reference_geo_code='IT')
-
 import pandas as pd
 import os
 import glob
 import json
 
 import requests
 from pytrends.exceptions import ResponseError
@@ -41,15 +12,15 @@
 import time
 
 import logging
 from rich.console import Console
 from rich.logging import RichHandler
 
 from math import ceil
-import random
+import platform
 
 console = Console()
 
 class RequestTrends:
 
     logging.basicConfig(
         level="INFO", format="%(message)s", datefmt="%d-%b-%Y %H:%M:%S", handlers=[RichHandler(rich_tracebacks=True)]
@@ -149,22 +120,21 @@
         self.__times[-1] = self.end_date
 
 
     def cross_section(self, geo: str="", resolution: str="COUNTRY"):
         self.__logger.info("Collecting Cross Section Data now")
 
         res = ["COUNTRY", "REGION", "CITY"]
+        if not geo.strip():
+            raise ValueError("geo cannot be empty. For worlwide data, geo='Worldwide'")
 
-        print(geo, " Before")
         if (not geo.strip() and resolution != "COUNTRY") or (geo.strip() and resolution not in res):
             self.__logger.info("Incorrect Resolution Provided. Defaulting to 'COUNTRY'")
             resolution = "COUNTRY" 
 
-        print(geo, " After")
-
         self.__create_required_directory("{}/{}/by_region".format(self.folder_name, self.data_format))
 
         if self.data_format == 'daily':
             chng_delta = relativedelta(days=1)
             end_delta = relativedelta(days=0)
             form = 'day'
         if self.data_format == 'weekly':
@@ -185,31 +155,27 @@
         with console.status("Collecting Data...") as stats:
             while True:
                 if (self.data_format == 'weekly' and current_time >= self.end_date) or (self.data_format != 'weekly' and current_time > self.end_date):
                     stats.stop()
                     break
 
                 current_end_time = current_time + end_delta
-                # print("{}/{}/by_region/{}_{}-{}-{}.csv".format(self.folder_name, self.data_format,  form, i+1, current_time.strftime("%Y%m%d"), current_end_time.strftime("%Y%m%d")))
                 if os.path.exists("{}/{}/by_region/{}_{}-{}-{}.csv".format(self.folder_name, self.data_format,  form, i+1, current_time.strftime("%Y%m%d"), current_end_time.strftime("%Y%m%d"))):
-                        # print('true')
                         self.__logger.info("Data for {}-{} already collected. Moving to next date...".format(current_time.strftime("%#d/%m/%#Y"), current_end_time.strftime("%#d/%m/%#Y")), extra={"markup": True})
                         current_time += chng_delta
                         i += 1
                 else:
                     try:
-                        print(geo, " Right Before")
                         self.__pytrend.build_payload(kw_list=[self.topic], geo=geo, 
                                                         timeframe='%s %s' % (current_time.strftime("%Y-%m-%d"), current_end_time.strftime("%Y-%m-%d"))) 
                         time.sleep(5)
                         df = self.__pytrend.interest_by_region(resolution=resolution, inc_geo_code=True, inc_low_vol=True)
                         df = df.rename(columns={self.topic:self.keyword})
                         i += 1
                     except ResponseError as e:
-
                         self.__logger.info("Please have patience as we reset rate limit ... ", extra={"markup": True})
                         time.sleep(5)
                         continue
                     except:
                         stats.stop() # Stop the animation
                         if not self.__in_notebook():
                             self.__logger.error("[bold red]Whoops![/]", exc_info=1, extra={"markup": True})
@@ -220,15 +186,15 @@
                             assert False
                         
                     time.sleep(5)
                     df.to_csv("{}/{}/by_region/{}_{}-{}-{}.csv".format(self.folder_name, self.data_format,  form, i, current_time.strftime("%Y%m%d"), current_end_time.strftime("%Y%m%d")))
 
                     current_time += chng_delta
 
-            self.__logger.info("[bold green]Successfully Collected Required Data![/]", extra={"markup": True})
+            self.__logger.info("[bold green]Successfully Collected Cross Section Data![/]", extra={"markup": True})
 
 
     # Time Series Data collection method for 'monthly'
     def __time_series_monthly(self, stats, reference_geo_code: str="US"):
         if os.path.exists("{}/{}/over_time/{}/{}-{}.csv".format(self.folder_name, self.data_format, reference_geo_code, self.start_date.strftime("%Y%m%d"), self.end_date.strftime("%Y%m%d"))):
             stats.stop()
             self.__logger.info("All Data for current request is already collected", extra={"markup": True})
@@ -299,14 +265,15 @@
             self.__create_required_directory('{}/{}/over_time'.format(self.folder_name, self.data_format))
             self.__create_required_directory('{}/{}/over_time/{}'.format(self.folder_name, self.data_format, reference_geo_code))
 
             if self.TIME_WINDOW:
                 self.__time_series_nmonthly(stats, reference_geo_code)
             else:
                 self.__time_series_monthly(stats, reference_geo_code)
+            self.__logger.info("[bold green]Successfully Collected Time Series Data![/]", extra={"markup": True})
 
 
     def concat_time_series(self, reference_geo_code: str="US", zero_replace: float=0.1):
         self.__logger.info("Concatenating Over Time data now", extra={"markup": True})
 
         # Create Folder to save the concatenated time series data
         self.__create_required_directory("{}/{}/concat_time_series".format(self.folder_name, self.data_format))
@@ -347,15 +314,18 @@
 
         with console.status("Converting...") as stats:
             for ind, row in time_series_concat.iterrows():
                 record = row['date'].strftime('%Y%m%d')
                 time_ind = float(row[self.keyword])
 
                 snap_file = glob.glob("{}/{}/by_region/*{}*.csv".format(self.folder_name, self.data_format, record))[0]
-                fl_name = snap_file.split("\\")[-1]
+                if platform.system() == "Windows":
+                    fl_name = snap_file.split("\\")[-1]
+                else:
+                    fl_name = snap_file.split("/")[-1]
                 col_name = fl_name.split('.')[0]
 
                 snap_df = pd.read_csv(snap_file, keep_default_na=False)
                 snap_df[self.keyword].replace(0, zero_replace, inplace=True)
 
                 ref_value = float(snap_df.loc[snap_df['geoCode'].str.contains(reference_geo_code)][self.keyword])
```

### Comparing `longitudinal_trends-0.1.7/longitudinal_trends.egg-info/PKG-INFO` & `longitudinal_trends-0.1.8/longitudinal_trends.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: longitudinal-trends
-Version: 0.1.7
+Version: 0.1.8
 Summary: Generate long-term longitudinal Google Trends Data
 Author: Mohammad Saleh Ahsan Sakir, Taeyong Park
 Author-email: ahsansakir506@gmail.com, taeyongp@andrew.cmu.edu
 License: MIT
 Project-URL: homepage, https://github.com/Mohammad-sakir/longitudinalTrends
 Keywords: longitudinal-trends longitudinal data python google-trends-api google-trends search-data
 Classifier: Programming Language :: Python :: 3
@@ -32,14 +32,15 @@
 
 ## Table of contents
 
 * Installation
 * Requirements
 * Initiate `longitudinal_trends`
 * Methods
+  * WARNING
   * `cross_section`
   * `time_series`
   * `concat_time_series`
   * `convert_cross_section`
   * `all_in_one_method`
 * Caveats
 * Credits
@@ -84,25 +85,36 @@
   - Date to end at
 - `data_format`
   - Time basis query
   - Can choose only one from the list: ['daily', 'weekly', 'monthly']
 
 ## Methods
 
+### WARNING
+
+Please make sure to run the methods in the following sequence:
+
+- `cross_section`
+- `time_series`
+- `concat_time_series`
+- `convert_time_series`
+
+We have noticed some unusual behaviors if not run in the given sequence. Firstly `concat_time_series` depends on `time_series` and `convert_cross_section` depends on all the three. We have noticed if `time_series` is ran before `cross_section` then sometimes the output gets incluenced by `time_series` parameters. We are troubleshooting the issue. Until then, please follow the sequence to attain the expected result.
+
 ### cross_section
 
 ```python
 day_data.cross_section(geo='US', resolution="REGION")
 ```
 
 This method will collect cross section data of the given keyword and timeline. It calls `pytrends.interest_by_region()` method from pytrends. The data is automatically saved in →  'folder_name'/'data_format'/by_region. Each file has data for the given region/countries all the country/state google trends index for 1 day/week/month. The filenames tells the date of the data time period and also has an indication of number of day/week/month.
 
 For more information on pytrends `interest_by_region()` method, [check here](https://pypi.org/project/pytrends/#interest-by-region).
 
-**PS**: *This method takes a long time to finish running. For example, it takes around 5 hours to collect 350 days of daily data. The time is mainly due to Google Trends API rate limit.*
+**PS**: *This method takes a long time to finish running. For example, it takes around 5 hours to collect 350 days of daily data. The time is mainly due to Google Trends API rate limit and resetting the limit.*
 
 **Parameters**
 
 - `geo`
   - Country/Region to collect data from. If left empty, then result will be worldwide i.e. data will be collected for all country. If left empty, defaults to worldwide country level.
 - `resolution`
   - 'COUNTRY' returns country level data
```

### Comparing `longitudinal_trends-0.1.7/pyproject.toml` & `longitudinal_trends-0.1.8/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]#, "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "longitudinal_trends"
-version='0.1.7'
+version='0.1.8'
 description="Generate long-term longitudinal Google Trends Data"
 urls = {homepage = "https://github.com/Mohammad-sakir/longitudinalTrends"}
 requires-python = ">=3.7"
 authors = [
     {name = "Mohammad Saleh Ahsan Sakir"},
     {name = "Taeyong Park"}, 
     {email="ahsansakir506@gmail.com"},
```

