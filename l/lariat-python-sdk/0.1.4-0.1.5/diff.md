# Comparing `tmp/lariat_python_sdk-0.1.4.tar.gz` & `tmp/lariat_python_sdk-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lariat_python_sdk-0.1.4.tar", last modified: Tue May  9 14:33:32 2023, max compression
+gzip compressed data, was "lariat_python_sdk-0.1.5.tar", last modified: Mon May 22 19:49:25 2023, max compression
```

## Comparing `lariat_python_sdk-0.1.4.tar` & `lariat_python_sdk-0.1.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 vikas      (501) staff       (20)        0 2023-05-09 14:33:32.300390 lariat_python_sdk-0.1.4/
--rw-r--r--   0 vikas      (501) staff       (20)     1498 2023-05-05 03:34:47.000000 lariat_python_sdk-0.1.4/LICENSE
--rw-r--r--   0 vikas      (501) staff       (20)     2403 2023-05-09 14:33:32.300240 lariat_python_sdk-0.1.4/PKG-INFO
--rw-r--r--   0 vikas      (501) staff       (20)     1423 2023-05-09 13:33:08.000000 lariat_python_sdk-0.1.4/README.md
-drwxr-xr-x   0 vikas      (501) staff       (20)        0 2023-05-09 14:33:32.298936 lariat_python_sdk-0.1.4/lariat_client/
--rw-r--r--   0 vikas      (501) staff       (20)      332 2023-05-05 03:34:47.000000 lariat_python_sdk-0.1.4/lariat_client/__init__.py
--rw-r--r--   0 vikas      (501) staff       (20)    20104 2023-05-09 14:26:22.000000 lariat_python_sdk-0.1.4/lariat_client/lariat_client.py
-drwxr-xr-x   0 vikas      (501) staff       (20)        0 2023-05-09 14:33:32.299839 lariat_python_sdk-0.1.4/lariat_python_sdk.egg-info/
--rw-r--r--   0 vikas      (501) staff       (20)     2403 2023-05-09 14:33:32.000000 lariat_python_sdk-0.1.4/lariat_python_sdk.egg-info/PKG-INFO
--rw-r--r--   0 vikas      (501) staff       (20)      321 2023-05-09 14:33:32.000000 lariat_python_sdk-0.1.4/lariat_python_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 vikas      (501) staff       (20)        1 2023-05-09 14:33:32.000000 lariat_python_sdk-0.1.4/lariat_python_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 vikas      (501) staff       (20)       43 2023-05-09 14:33:32.000000 lariat_python_sdk-0.1.4/lariat_python_sdk.egg-info/requires.txt
--rw-r--r--   0 vikas      (501) staff       (20)       14 2023-05-09 14:33:32.000000 lariat_python_sdk-0.1.4/lariat_python_sdk.egg-info/top_level.txt
--rw-r--r--   0 vikas      (501) staff       (20)     1102 2023-05-09 14:28:41.000000 lariat_python_sdk-0.1.4/pyproject.toml
--rw-r--r--   0 vikas      (501) staff       (20)       38 2023-05-09 14:33:32.300434 lariat_python_sdk-0.1.4/setup.cfg
-drwxr-xr-x   0 vikas      (501) staff       (20)        0 2023-05-09 14:33:32.299973 lariat_python_sdk-0.1.4/tests/
--rw-r--r--   0 vikas      (501) staff       (20)     6746 2023-05-05 03:34:47.000000 lariat_python_sdk-0.1.4/tests/test_lariat_client.py
+drwxr-xr-x   0 vikas      (501) staff       (20)        0 2023-05-22 19:49:25.382398 lariat_python_sdk-0.1.5/
+-rw-r--r--   0 vikas      (501) staff       (20)     1498 2023-05-05 03:34:47.000000 lariat_python_sdk-0.1.5/LICENSE
+-rw-r--r--   0 vikas      (501) staff       (20)     3290 2023-05-22 19:49:25.382254 lariat_python_sdk-0.1.5/PKG-INFO
+-rw-r--r--   0 vikas      (501) staff       (20)     2310 2023-05-22 19:38:49.000000 lariat_python_sdk-0.1.5/README.md
+drwxr-xr-x   0 vikas      (501) staff       (20)        0 2023-05-22 19:49:25.380870 lariat_python_sdk-0.1.5/lariat_client/
+-rw-r--r--   0 vikas      (501) staff       (20)      346 2023-05-22 19:38:49.000000 lariat_python_sdk-0.1.5/lariat_client/__init__.py
+-rw-r--r--   0 vikas      (501) staff       (20)    23214 2023-05-22 19:38:49.000000 lariat_python_sdk-0.1.5/lariat_client/lariat_client.py
+drwxr-xr-x   0 vikas      (501) staff       (20)        0 2023-05-22 19:49:25.381808 lariat_python_sdk-0.1.5/lariat_python_sdk.egg-info/
+-rw-r--r--   0 vikas      (501) staff       (20)     3290 2023-05-22 19:49:25.000000 lariat_python_sdk-0.1.5/lariat_python_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 vikas      (501) staff       (20)      321 2023-05-22 19:49:25.000000 lariat_python_sdk-0.1.5/lariat_python_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 vikas      (501) staff       (20)        1 2023-05-22 19:49:25.000000 lariat_python_sdk-0.1.5/lariat_python_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 vikas      (501) staff       (20)       43 2023-05-22 19:49:25.000000 lariat_python_sdk-0.1.5/lariat_python_sdk.egg-info/requires.txt
+-rw-r--r--   0 vikas      (501) staff       (20)       14 2023-05-22 19:49:25.000000 lariat_python_sdk-0.1.5/lariat_python_sdk.egg-info/top_level.txt
+-rw-r--r--   0 vikas      (501) staff       (20)     1102 2023-05-22 19:49:03.000000 lariat_python_sdk-0.1.5/pyproject.toml
+-rw-r--r--   0 vikas      (501) staff       (20)       38 2023-05-22 19:49:25.382440 lariat_python_sdk-0.1.5/setup.cfg
+drwxr-xr-x   0 vikas      (501) staff       (20)        0 2023-05-22 19:49:25.381959 lariat_python_sdk-0.1.5/tests/
+-rw-r--r--   0 vikas      (501) staff       (20)     6746 2023-05-05 03:34:47.000000 lariat_python_sdk-0.1.5/tests/test_lariat_client.py
```

### Comparing `lariat_python_sdk-0.1.4/LICENSE` & `lariat_python_sdk-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `lariat_python_sdk-0.1.4/PKG-INFO` & `lariat_python_sdk-0.1.5/lariat_python_sdk.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: lariat_python_sdk
-Version: 0.1.4
+Name: lariat-python-sdk
+Version: 0.1.5
 Summary: A Python module to interact with Lariat API to access data quality metrics and diagnostics
 Author-email: Lariat Data Team <info@lariatdata.com>
 License: BSD-3-Clause
 Project-URL: homepage, https://www.lariatdata.com
 Project-URL: documentation, https://lariat-python-sdk.readthedocs.io/en/latest/
 Project-URL: repository, https://github.com/lariat-data/lariat-python-sdk
 Classifier: Development Status :: 3 - Alpha
@@ -76,18 +76,45 @@
 
 Query an indicator:
 
 ```python
 from_ts = datetime.datetime(2022, 1, 1)
 to_ts = datetime.datetime(2022, 2, 1)
 group_by = ["country"]
-filter_clause = FilterClause(field="country", operator="in", values="US,UK"])
+filter_clause = FilterClause(field="country", operator="in", values="US,UK")
 query_filter = Filter(clauses=[filter_clause], operator="and")
 
-results = query(indicator["id"], from_ts, to_ts, group_by, query_filter=query_filter)
+results = query(indicator.id, from_ts, to_ts, group_by, query_filter=query_filter)
 
 # Convert results to a DataFrame
 results_df = results.to_df()
 
 # Save results to a CSV file
 results.to_csv("results.csv")
 ```
+
+Use the `RawQuery` interface to add additional query arguments
+_Note: Query arguments attached via the RawQuery interface are subject to changes in their backend interpretation. Use with caution_
+
+```python
+import lariat_client
+import datetime
+
+lariat_client.configure(api_key="some_key", application_key="some_other_key")
+indicator = lariat_client.get_indicator(id=1234)
+from_ts = datetime.datetime(2023, 5, 1)
+to_ts = datetime.datetime(2023, 5, 10)
+
+filter_clause = lariat_client.FilterClause(field="country", operator="in", values="USA")
+query_filter = lariat_client.Filter(clauses=[filter_clause], operator="and")
+
+raw_query = lariat_client.RawQuery(
+        indicator_id=indicator.id,
+        from_ts=from_ts,
+        to_ts=to_ts,
+        aggregate="distinct",
+        query_filter=query_filter
+)
+
+raw_query.add_query_argument("x_axis", "custom_x_axis")
+records = raw_query.send()
+```
```

### Comparing `lariat_python_sdk-0.1.4/README.md` & `lariat_python_sdk-0.1.5/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -54,18 +54,45 @@
 
 Query an indicator:
 
 ```python
 from_ts = datetime.datetime(2022, 1, 1)
 to_ts = datetime.datetime(2022, 2, 1)
 group_by = ["country"]
-filter_clause = FilterClause(field="country", operator="in", values="US,UK"])
+filter_clause = FilterClause(field="country", operator="in", values="US,UK")
 query_filter = Filter(clauses=[filter_clause], operator="and")
 
-results = query(indicator["id"], from_ts, to_ts, group_by, query_filter=query_filter)
+results = query(indicator.id, from_ts, to_ts, group_by, query_filter=query_filter)
 
 # Convert results to a DataFrame
 results_df = results.to_df()
 
 # Save results to a CSV file
 results.to_csv("results.csv")
 ```
+
+Use the `RawQuery` interface to add additional query arguments
+_Note: Query arguments attached via the RawQuery interface are subject to changes in their backend interpretation. Use with caution_
+
+```python
+import lariat_client
+import datetime
+
+lariat_client.configure(api_key="some_key", application_key="some_other_key")
+indicator = lariat_client.get_indicator(id=1234)
+from_ts = datetime.datetime(2023, 5, 1)
+to_ts = datetime.datetime(2023, 5, 10)
+
+filter_clause = lariat_client.FilterClause(field="country", operator="in", values="USA")
+query_filter = lariat_client.Filter(clauses=[filter_clause], operator="and")
+
+raw_query = lariat_client.RawQuery(
+        indicator_id=indicator.id,
+        from_ts=from_ts,
+        to_ts=to_ts,
+        aggregate="distinct",
+        query_filter=query_filter
+)
+
+raw_query.add_query_argument("x_axis", "custom_x_axis")
+records = raw_query.send()
+```
```

### Comparing `lariat_python_sdk-0.1.4/lariat_client/lariat_client.py` & `lariat_python_sdk-0.1.5/lariat_client/lariat_client.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,16 +21,16 @@
 application_key = os.getenv("LARIAT_APPLICATION_KEY")
 
 logger = logging.getLogger(__name__)
 
 s = requests.Session()
 s.headers.update(
     {
-        "X-Lariat-Application-Key": api_key,
-        "X-Lariat-Api-Key": application_key,
+        "X-Lariat-Application-Key": application_key,
+        "X-Lariat-Api-Key": api_key,
     }
 )
 
 
 def configure(api_key: str, application_key: str):
     """
     Configures the Lariat API credentials.
@@ -327,14 +327,106 @@
                     output_array.append(field)
                 writer.writerow(output_array)
             for record in self.records:
                 vals = record.to_dict()
                 writer.writerow([vals[field] for field in output_array])
 
 
+class RawQuery:
+    """A class representing a RawQuery to the Lariat metrics store.
+
+    A RawQuery may be sent to the API via `raw_query.send()` to retrive a `MetricRecordList`
+    """
+
+    def __init__(
+        self,
+        indicator_id: int,
+        from_ts: datetime.datetime,
+        to_ts: datetime.datetime = None,
+        group_by: List[str] = None,
+        aggregate: str = None,
+        query_filter: Filter = None,
+        extra_args: Dict = None,
+    ):
+        self.indicator_id = indicator_id
+        self.from_ts = from_ts
+        self.to_ts = to_ts
+        self.group_by = group_by
+        self.aggregate = aggregate
+        self.query_filter = query_filter
+        self.metric_query_extra_args = extra_args or {}
+
+    def add_query_argument(self, key: str, value: str):
+        self.metric_query_extra_args.update({key: value})
+
+    def to_json(self) -> Dict:
+        indicator_id = self.indicator_id
+        from_ts = self.from_ts
+        to_ts = self.to_ts
+        group_by = self.group_by
+        aggregate = self.aggregate
+        query_filter = self.query_filter
+
+        metric_query_extra_args = self.metric_query_extra_args
+
+        if to_ts is None:
+            to_ts = datetime.datetime.now()
+        data_filter = {"operator": "or", "filters": []}
+        if group_by:
+            data_filter["group_by_clauses"] = group_by
+        else:
+            group_by = []
+        if query_filter:
+            data_filter["operator"] = query_filter.operator
+            data_filter["filters"] = [
+                {
+                    "field": clause.field,
+                    "operator": clause.operator,
+                    "value": clause.values,
+                }
+                for clause in query_filter.clauses
+            ]
+        data = {
+            "indicator_id": indicator_id,
+            "metric_query": {
+                "time_range": {
+                    "from_ts": int(from_ts.timestamp() * 1000),
+                    "to_ts": int(to_ts.timestamp() * 1000),
+                },
+                "query": data_filter,
+            },
+        }
+
+        if metric_query_extra_args:
+            for key, value in metric_query_extra_args.items():
+                data["metric_query"][key] = value
+
+        if aggregate:
+            data["aggregation"] = aggregate
+
+        return data
+
+    def send(self) -> MetricRecordList:
+        try:
+            body = self.to_json()
+            group_by = self.group_by or []
+            r = s.get(url=f"{LARIAT_PUBLIC_API_ENDPOINT}/query-metrics-raw", json=body)
+            r.raise_for_status()
+            records = r.json()["records"]
+            return MetricRecordList(group_by, records)
+        except requests.exceptions.HTTPError as errh:
+            logging.error(f"Http Error: {errh}")
+        except requests.exceptions.ConnectionError as errc:
+            logging.error(f"Error Connecting: {errc}")
+        except requests.exceptions.Timeout as errt:
+            logging.error(f"Timeout Error: {errt}")
+        except requests.exceptions.RequestException as err:
+            logging.error(f"Something went wrong: {err}")
+
+
 def get_raw_datasets(dataset_ids: List[int]) -> List[RawDataset]:
     """
     Gets the raw datasets given a list of dataset ids.
 
     Args:
         dataset_ids (list): A list of dataset ids to filter on.
```

### Comparing `lariat_python_sdk-0.1.4/lariat_python_sdk.egg-info/PKG-INFO` & `lariat_python_sdk-0.1.5/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: lariat-python-sdk
-Version: 0.1.4
+Name: lariat_python_sdk
+Version: 0.1.5
 Summary: A Python module to interact with Lariat API to access data quality metrics and diagnostics
 Author-email: Lariat Data Team <info@lariatdata.com>
 License: BSD-3-Clause
 Project-URL: homepage, https://www.lariatdata.com
 Project-URL: documentation, https://lariat-python-sdk.readthedocs.io/en/latest/
 Project-URL: repository, https://github.com/lariat-data/lariat-python-sdk
 Classifier: Development Status :: 3 - Alpha
@@ -76,18 +76,45 @@
 
 Query an indicator:
 
 ```python
 from_ts = datetime.datetime(2022, 1, 1)
 to_ts = datetime.datetime(2022, 2, 1)
 group_by = ["country"]
-filter_clause = FilterClause(field="country", operator="in", values="US,UK"])
+filter_clause = FilterClause(field="country", operator="in", values="US,UK")
 query_filter = Filter(clauses=[filter_clause], operator="and")
 
-results = query(indicator["id"], from_ts, to_ts, group_by, query_filter=query_filter)
+results = query(indicator.id, from_ts, to_ts, group_by, query_filter=query_filter)
 
 # Convert results to a DataFrame
 results_df = results.to_df()
 
 # Save results to a CSV file
 results.to_csv("results.csv")
 ```
+
+Use the `RawQuery` interface to add additional query arguments
+_Note: Query arguments attached via the RawQuery interface are subject to changes in their backend interpretation. Use with caution_
+
+```python
+import lariat_client
+import datetime
+
+lariat_client.configure(api_key="some_key", application_key="some_other_key")
+indicator = lariat_client.get_indicator(id=1234)
+from_ts = datetime.datetime(2023, 5, 1)
+to_ts = datetime.datetime(2023, 5, 10)
+
+filter_clause = lariat_client.FilterClause(field="country", operator="in", values="USA")
+query_filter = lariat_client.Filter(clauses=[filter_clause], operator="and")
+
+raw_query = lariat_client.RawQuery(
+        indicator_id=indicator.id,
+        from_ts=from_ts,
+        to_ts=to_ts,
+        aggregate="distinct",
+        query_filter=query_filter
+)
+
+raw_query.add_query_argument("x_axis", "custom_x_axis")
+records = raw_query.send()
+```
```

### Comparing `lariat_python_sdk-0.1.4/pyproject.toml` & `lariat_python_sdk-0.1.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "lariat_python_sdk"
-version = "0.1.4"
+version = "0.1.5"
 description = "A Python module to interact with Lariat API to access data quality metrics and diagnostics"
 readme = "README.md"
 authors = [
     { name = "Lariat Data Team", email = "info@lariatdata.com"}
 ]
 license = {text = "BSD-3-Clause"}
 dependencies = [
```

### Comparing `lariat_python_sdk-0.1.4/tests/test_lariat_client.py` & `lariat_python_sdk-0.1.5/tests/test_lariat_client.py`

 * *Files identical despite different names*

