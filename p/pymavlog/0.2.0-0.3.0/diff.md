# Comparing `tmp/pymavlog-0.2.0.tar.gz` & `tmp/pymavlog-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymavlog-0.2.0.tar", max compression
+gzip compressed data, was "pymavlog-0.3.0.tar", max compression
```

## Comparing `pymavlog-0.2.0.tar` & `pymavlog-0.3.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1073 2023-04-26 16:08:11.867424 pymavlog-0.2.0/LICENSE
--rw-r--r--   0        0        0     1890 2023-04-26 16:08:11.867424 pymavlog-0.2.0/README.md
--rw-r--r--   0        0        0      196 2023-04-26 16:08:11.871424 pymavlog-0.2.0/pymavlog/__init__.py
--rw-r--r--   0        0        0     8808 2023-04-26 16:08:11.871424 pymavlog-0.2.0/pymavlog/core.py
--rw-r--r--   0        0        0      137 2023-04-26 16:08:11.871424 pymavlog-0.2.0/pymavlog/errors.py
--rw-r--r--   0        0        0      121 2023-04-26 16:08:11.871424 pymavlog-0.2.0/pymavlog/helpers.py
--rw-r--r--   0        0        0     1072 2023-04-26 16:08:34.587891 pymavlog-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     3007 1970-01-01 00:00:00.000000 pymavlog-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-05-22 14:09:21.329705 pymavlog-0.3.0/LICENSE
+-rw-r--r--   0        0        0     1993 2023-05-22 14:09:21.329705 pymavlog-0.3.0/README.md
+-rw-r--r--   0        0        0      196 2023-05-22 14:09:21.329705 pymavlog-0.3.0/pymavlog/__init__.py
+-rw-r--r--   0        0        0     9086 2023-05-22 14:09:21.329705 pymavlog-0.3.0/pymavlog/core.py
+-rw-r--r--   0        0        0      137 2023-05-22 14:09:21.329705 pymavlog-0.3.0/pymavlog/errors.py
+-rw-r--r--   0        0        0      121 2023-05-22 14:09:21.329705 pymavlog-0.3.0/pymavlog/helpers.py
+-rw-r--r--   0        0        0     1072 2023-05-22 14:09:32.002008 pymavlog-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     3110 1970-01-01 00:00:00.000000 pymavlog-0.3.0/PKG-INFO
```

### Comparing `pymavlog-0.2.0/LICENSE` & `pymavlog-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pymavlog-0.2.0/README.md` & `pymavlog-0.3.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -74,14 +74,20 @@
 
 and do some calculations, for example calculating the average value:
 
 ```python
 avg_gyr_x = imu_messages["GyrX"].mean()
 ```
 
+alternatively, you can access a specific attribute like:
+
+```python
+gyr_y = mavlog["IMU"]["Gyrx"]
+```
+
 Pymavlog also supports telemetry log files. You can read a tlog file `.tlog` in a similar way as binary log files, like:
 
 ```python
 from pymavlog import MavTLog
 
 
 filepath = "foo/bar.tlog"
```

### Comparing `pymavlog-0.2.0/pymavlog/core.py` & `pymavlog-0.3.0/pymavlog/core.py`

 * *Files 3% similar despite different names*

```diff
@@ -48,22 +48,26 @@
         if self._to_datetime:
             self._types = [datetime]
         else:
             self._types = [float]
 
         self._columns.extend(columns)
         self._types.extend(types)
-        self._fields: t.Dict[str, t.List[datetime | int | float]] = {}
+        self._fields: t.Dict[str, t.List[t.Union[datetime, int, float]]] = {}
 
         self.__set_series()
 
     def __set_series(self):
         for c in self._columns:
             self._fields[self._column_alias.get(c, c)] = []
 
+    @property
+    def columns(self) -> t.List[str]:
+        return self._columns
+
     @classmethod
     def from_df_format(
         cls,
         fmt: DFFormat,
         column_alias: t.Dict[str, str] = {},
         msg_id: int = 1,
         convert_to_datetime: bool = False,
@@ -133,14 +137,17 @@
                 self._fields["timestamp"].append(datetime.fromtimestamp(timestamp))
             else:
                 self._fields["timestamp"].append(timestamp)
 
         for k, v in msg_dict.items():
             self._fields[self._column_alias.get(k, k)].append(v)
 
+    def __getitem__(self, item: str) -> np.ndarray:
+        return self._fields[item]
+
 
 class MavLogBase(object):
     def __init__(
         self,
         filepath: str,
         messages_to_ignore: t.List[str] = ["FMT", "FMTU"],
         types: t.List[str] = None,
@@ -153,14 +160,17 @@
         self._parsed_data: t.Dict[str, MavLinkMessageSeries] = {}
         self._msg_count = 0
         self._to_datetime = to_datetime
         self._map_columns = map_columns
         self._start_timestamp = None
         self._end_timestamp = None
 
+    def __getitem__(self, item: str) -> MavLinkMessageSeries:
+        return self._parsed_data[item]
+
     @property
     def parsed_data(self) -> t.Dict[str, MavLinkMessageSeries]:
         return self._parsed_data
 
     @property
     def message_count(self) -> int:
         return self._msg_count
```

### Comparing `pymavlog-0.2.0/pyproject.toml` & `pymavlog-0.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pymavlog"
-version = "0.2.0"
+version = "0.3.0"
 description = "A lightweight python library to parse MavLink log files"
 readme = "README.md"
 license = "MIT"
 authors = [
     "Ricardo Martinez <rik@rmargar.net>"
 ]
 classifiers = [
```

### Comparing `pymavlog-0.2.0/PKG-INFO` & `pymavlog-0.3.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymavlog
-Version: 0.2.0
+Version: 0.3.0
 Summary: A lightweight python library to parse MavLink log files
 Home-page: https://github.com/rmargar/pymavlog
 License: MIT
 Author: Ricardo Martinez
 Author-email: rik@rmargar.net
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 1 - Planning
@@ -102,14 +102,20 @@
 
 and do some calculations, for example calculating the average value:
 
 ```python
 avg_gyr_x = imu_messages["GyrX"].mean()
 ```
 
+alternatively, you can access a specific attribute like:
+
+```python
+gyr_y = mavlog["IMU"]["Gyrx"]
+```
+
 Pymavlog also supports telemetry log files. You can read a tlog file `.tlog` in a similar way as binary log files, like:
 
 ```python
 from pymavlog import MavTLog
 
 
 filepath = "foo/bar.tlog"
```

