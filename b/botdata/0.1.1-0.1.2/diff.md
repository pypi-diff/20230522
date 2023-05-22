# Comparing `tmp/botdata-0.1.1.tar.gz` & `tmp/botdata-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botdata-0.1.1.tar", last modified: Wed Apr  5 10:55:48 2023, max compression
+gzip compressed data, was "botdata-0.1.2.tar", last modified: Mon May 22 05:07:46 2023, max compression
```

## Comparing `botdata-0.1.1.tar` & `botdata-0.1.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 10:55:48.655165 botdata-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-04-05 10:55:27.000000 botdata-0.1.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      889 2023-04-05 10:55:48.655165 botdata-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-04-05 10:55:27.000000 botdata-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 10:55:48.655165 botdata-0.1.1/botdata/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-05 10:55:27.000000 botdata-0.1.1/botdata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-05 10:55:27.000000 botdata-0.1.1/botdata/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-04-05 10:55:27.000000 botdata-0.1.1/botdata/holiday.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 10:55:48.655165 botdata-0.1.1/botdata.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      889 2023-04-05 10:55:48.000000 botdata-0.1.1/botdata.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-04-05 10:55:48.000000 botdata-0.1.1/botdata.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-05 10:55:48.000000 botdata-0.1.1/botdata.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-05 10:55:48.000000 botdata-0.1.1/botdata.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-05 10:55:48.000000 botdata-0.1.1/botdata.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-04-05 10:55:48.655165 botdata-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-04-05 10:55:27.000000 botdata-0.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 10:55:48.655165 botdata-0.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3644 2023-04-05 10:55:27.000000 botdata-0.1.1/tests/test_holiday.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 05:07:46.347811 botdata-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-05-22 05:07:31.000000 botdata-0.1.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2023-05-22 05:07:46.347811 botdata-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-05-22 05:07:31.000000 botdata-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 05:07:46.347811 botdata-0.1.2/botdata/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-22 05:07:31.000000 botdata-0.1.2/botdata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-22 05:07:31.000000 botdata-0.1.2/botdata/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-05-22 05:07:31.000000 botdata-0.1.2/botdata/holiday.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 05:07:46.347811 botdata-0.1.2/botdata.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2023-05-22 05:07:46.000000 botdata-0.1.2/botdata.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-05-22 05:07:46.000000 botdata-0.1.2/botdata.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 05:07:46.000000 botdata-0.1.2/botdata.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-22 05:07:46.000000 botdata-0.1.2/botdata.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-22 05:07:46.000000 botdata-0.1.2/botdata.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-22 05:07:46.347811 botdata-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-05-22 05:07:31.000000 botdata-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 05:07:46.347811 botdata-0.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2775 2023-05-22 05:07:31.000000 botdata-0.1.2/tests/test_holiday.py
```

### Comparing `botdata-0.1.1/LICENSE.txt` & `botdata-0.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `botdata-0.1.1/PKG-INFO` & `botdata-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botdata
-Version: 0.1.1
+Version: 0.1.2
 Summary: BOT Data is a Python package for retrieving data from the website of the Bank of Thailand
 Home-page: https://github.com/ezyquant/BOT-Data
 Author: Fintech (Thailand) Company Limited
 Author-email: admin@fintech.co.th
 Maintainer: Fintech (Thailand) Company Limited
 Maintainer-email: admin@fintech.co.th
 License: The MIT License (MIT)
```

### Comparing `botdata-0.1.1/botdata/holiday.py` & `botdata-0.1.2/botdata/holiday.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from datetime import date, datetime, timedelta
 from functools import lru_cache
 from typing import List, TypeVar
 
 import pandas as pd
+import requests
 from pandas.tseries.offsets import CustomBusinessDay
 
 """
 Holiday
 """
 
 
@@ -36,27 +37,25 @@
         Year
 
     Returns
     -------
     pd.Series
         Series of holidays
     """
-    # df should contains the following columns: Index, Day of week, Day of month, Month, Description
-    df = pd.read_html(
-        f"https://www.bot.or.th/English/FinancialInstitutions/FIholiday/Pages/{year}.aspx"
-    )[0]
-
-    # Drop incorrect row usually from recursive
-    df = df.dropna(axis=0, how="any", subset=[2, 3])
-    # Drop cancelled holiday
-    df = df[~df[4].str.contains("cancelled", case=False, na=False)]
-    # Concat Day, Month, Year
-    date_str_ser = df[2].astype(str).str[:-2] + " " + df[3] + " " + str(year)
-    # Remove non-ascii characters usually unicode
-    date_str_ser = date_str_ser.str.encode("ascii", "ignore").str.decode("ascii")
+    # Send a GET request to the website
+    url = f"https://www.bot.or.th/content/bot/en/financial-institutions-holiday/jcr:content/root/container/holidaycalendar.model.{year}.json"
+    response = requests.get(url)
+    data = response.json()
+    if "holidayCalendarLists" not in data:
+        raise ValueError(f"Year {year} is not available")
+
+    # df columns 'holidayDescription', 'date', 'month', 'year'
+    df = pd.DataFrame(data["holidayCalendarLists"])
+
+    date_str_ser = df["date"] + " " + df["month"] + " " + df["year"]
 
     return pd.to_datetime(date_str_ser)
 
 
 def is_holiday(date_: date) -> bool:
     """Check if date is holiday
 
@@ -110,15 +109,15 @@
     Returns
     -------
     date
         Date of next business day
     """
     holidays = get_holidays_series(date_.year).tolist()
 
-    next_date = date_ + timedelta(n + 5 if n > 0 else n - 5)
+    next_date = date_ + timedelta(n + 5 if n >= 0 else n - 5)
 
     if next_date.year != date_.year:
         holidays += get_holidays_series(next_date.year).tolist()
 
     bd = CustomBusinessDay(n, holidays=holidays)
 
     ts = date_ + bd
```

### Comparing `botdata-0.1.1/botdata.egg-info/PKG-INFO` & `botdata-0.1.2/botdata.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botdata
-Version: 0.1.1
+Version: 0.1.2
 Summary: BOT Data is a Python package for retrieving data from the website of the Bank of Thailand
 Home-page: https://github.com/ezyquant/BOT-Data
 Author: Fintech (Thailand) Company Limited
 Author-email: admin@fintech.co.th
 Maintainer: Fintech (Thailand) Company Limited
 Maintainer-email: admin@fintech.co.th
 License: The MIT License (MIT)
```

### Comparing `botdata-0.1.1/setup.py` & `botdata-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     long_description="BOT Data is a Python package for retrieving data from the website of the Bank of Thailand",
     author="Fintech (Thailand) Company Limited",
     author_email="admin@fintech.co.th",
     url="https://github.com/ezyquant/BOT-Data",
     maintainer="Fintech (Thailand) Company Limited",
     maintainer_email="admin@fintech.co.th",
     python_requires=">=3.8",
-    install_requires=["pandas>=1.3", "lxml>=4.0"],
+    install_requires=["pandas>=1.2", "requests>=2.0"],
     license="The MIT License (MIT)",
     classifiers=[
         "Intended Audience :: Financial and Insurance Industry",
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
     ],
     project_urls={
```

### Comparing `botdata-0.1.1/tests/test_holiday.py` & `botdata-0.1.2/tests/test_holiday.py`

 * *Files 24% similar despite different names*

```diff
@@ -7,38 +7,14 @@
 import botdata as bd
 
 
 @pytest.mark.parametrize(
     ("year", "expected"),
     [
         (
-            2020,
-            [
-                date(2020, 1, 1),
-                date(2020, 2, 10),
-                date(2020, 4, 6),
-                date(2020, 5, 1),
-                date(2020, 5, 4),
-                date(2020, 5, 6),
-                date(2020, 6, 3),
-                date(2020, 7, 6),
-                date(2020, 7, 27),
-                date(2020, 7, 28),
-                date(2020, 8, 12),
-                date(2020, 9, 4),
-                date(2020, 9, 7),
-                date(2020, 10, 13),
-                date(2020, 10, 23),
-                date(2020, 12, 7),
-                date(2020, 12, 10),
-                date(2020, 12, 11),
-                date(2020, 12, 31),
-            ],
-        ),
-        (
             2022,
             [
                 date(2022, 1, 3),
                 date(2022, 2, 16),
                 date(2022, 4, 6),
                 date(2022, 4, 13),
                 date(2022, 4, 14),
@@ -54,82 +30,77 @@
                 date(2022, 10, 13),
                 date(2022, 10, 14),
                 date(2022, 10, 24),
                 date(2022, 12, 5),
                 date(2022, 12, 12),
             ],
         ),
-        (2000, [ANY] * 13),
-        (2005, [ANY] * 15),
-        (2010, [ANY] * 19),
-        (2015, [ANY] * 18),
-        (2021, [ANY] * 20),
         (2023, ANY),
     ],
 )
 def test_get_holidays(year: int, expected: list):
     # Test
     result = bd.get_holidays(year)
 
     # Check
     assert result == expected
 
 
 @pytest.mark.parametrize(
     (("date_", "expected")),
     [
-        (date(2020, 1, 1), True),
-        (date(2020, 1, 2), False),
+        (date(2022, 1, 3), True),
+        (date(2022, 1, 4), False),
     ],
 )
 def test_is_holiday(date_: date, expected: bool):
     # Test
     result = bd.is_holiday(date_)
 
     # Check
     assert result is expected
 
 
 @pytest.mark.parametrize(
     (("date_", "expected")),
     [
-        (date(2020, 1, 1), False),
-        (date(2020, 1, 2), True),
-        (date(2020, 1, 3), True),
-        (date(2020, 1, 4), False),
-        (date(2020, 1, 5), False),
+        (date(2022, 1, 1), False),
+        (date(2022, 1, 2), False),
+        (date(2022, 1, 3), False),
+        (date(2022, 1, 4), True),
+        (date(2022, 1, 5), True),
     ],
 )
 def test_is_business_day(date_: date, expected: bool):
     # Test
     result = bd.is_business_day(date_)
 
     # Check
     assert result is expected
 
 
 @pytest.mark.parametrize(
     (("date_", "n", "expected")),
     [
         # test date
-        (date(2020, 1, 1), 1, date(2020, 1, 2)),
-        (date(2020, 1, 2), 1, date(2020, 1, 3)),
-        (date(2020, 1, 3), 1, date(2020, 1, 6)),
-        (date(2020, 1, 4), 1, date(2020, 1, 6)),
-        (date(2020, 1, 5), 1, date(2020, 1, 6)),
+        (date(2022, 1, 1), 1, date(2022, 1, 4)),
+        (date(2022, 1, 2), 1, date(2022, 1, 4)),
+        (date(2022, 1, 3), 1, date(2022, 1, 4)),
+        (date(2022, 1, 4), 1, date(2022, 1, 5)),
+        (date(2022, 1, 5), 1, date(2022, 1, 6)),
         # test n
-        (date(2020, 1, 1), 0, date(2020, 1, 2)),
-        (date(2020, 1, 2), 0, date(2020, 1, 2)),
-        (date(2020, 1, 1), -1, date(2019, 12, 30)),
-        (date(2020, 1, 2), -1, date(2019, 12, 30)),
-        (date(2020, 12, 30), 1, date(2021, 1, 4)),
-        (date(2020, 12, 31), 1, date(2021, 1, 4)),
+        (date(2022, 1, 1), 0, date(2022, 1, 4)),
+        (date(2022, 1, 2), 0, date(2022, 1, 4)),
+        (date(2023, 1, 1), -1, date(2022, 12, 30)),
+        (date(2023, 1, 2), -1, date(2022, 12, 30)),
+        (date(2022, 12, 30), 1, date(2023, 1, 3)),
+        (date(2022, 12, 31), 1, date(2023, 1, 3)),
         # test datatype
-        (datetime(2020, 1, 1), 1, datetime(2020, 1, 2)),
-        (pd.Timestamp(2020, 1, 1), 1, pd.Timestamp(2020, 1, 2)),
+        (datetime(2022, 1, 1), 1, datetime(2022, 1, 4)),
+        (pd.Timestamp(2022, 1, 1), 1, pd.Timestamp(2022, 1, 4)),
     ],
 )
 def test_next_business_day(date_: date, n: int, expected: bool):
     # Test
     result = bd.next_business_day(date_=date_, n=n)
 
     # Check
```

