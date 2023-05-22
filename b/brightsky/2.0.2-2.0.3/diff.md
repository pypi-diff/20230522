# Comparing `tmp/brightsky-2.0.2.tar.gz` & `tmp/brightsky-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "brightsky-2.0.2.tar", last modified: Tue May  9 10:05:25 2023, max compression
+gzip compressed data, was "brightsky-2.0.3.tar", last modified: Mon May 22 14:11:00 2023, max compression
```

## Comparing `brightsky-2.0.2.tar` & `brightsky-2.0.3.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 10:05:25.780775 brightsky-2.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-09 10:05:20.000000 brightsky-2.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8318 2023-05-09 10:05:25.780775 brightsky-2.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7713 2023-05-09 10:05:20.000000 brightsky-2.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 10:05:25.776775 brightsky-2.0.2/brightsky/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-09 10:05:20.000000 brightsky-2.0.2/brightsky/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-05-09 10:05:20.000000 brightsky-2.0.2/brightsky/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4898 2023-05-09 10:05:20.000000 brightsky-2.0.2/brightsky/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2578 2023-05-09 10:05:20.000000 brightsky-2.0.2/brightsky/db.py
--rw-r--r--   0 runner    (1001) docker     (123)     9369 2023-05-09 10:05:20.000000 brightsky-2.0.2/brightsky/export.py
--rw-r--r--   0 runner    (1001) docker     (123)     6033 2023-05-09 10:05:20.000000 brightsky-2.0.2/brightsky/parsers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4323 2023-05-09 10:05:20.000000 brightsky-2.0.2/brightsky/polling.py
--rw-r--r--   0 runner    (1001) docker     (123)    11309 2023-05-09 10:05:20.000000 brightsky-2.0.2/brightsky/query.py
--rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-05-09 10:05:20.000000 brightsky-2.0.2/brightsky/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     5001 2023-05-09 10:05:20.000000 brightsky-2.0.2/brightsky/tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-05-09 10:05:20.000000 brightsky-2.0.2/brightsky/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    12951 2023-05-09 10:05:20.000000 brightsky-2.0.2/brightsky/web.py
--rw-r--r--   0 runner    (1001) docker     (123)     2160 2023-05-09 10:05:20.000000 brightsky-2.0.2/brightsky/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 10:05:25.776775 brightsky-2.0.2/brightsky.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8318 2023-05-09 10:05:25.000000 brightsky-2.0.2/brightsky.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-05-09 10:05:25.000000 brightsky-2.0.2/brightsky.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 10:05:25.000000 brightsky-2.0.2/brightsky.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-09 10:05:25.000000 brightsky-2.0.2/brightsky.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-09 10:05:25.000000 brightsky-2.0.2/brightsky.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-09 10:05:20.000000 brightsky-2.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 10:05:25.780775 brightsky-2.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-05-09 10:05:20.000000 brightsky-2.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 10:05:25.780775 brightsky-2.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-09 10:05:20.000000 brightsky-2.0.2/tests/test_db.py
--rw-r--r--   0 runner    (1001) docker     (123)     5341 2023-05-09 10:05:20.000000 brightsky-2.0.2/tests/test_export.py
--rw-r--r--   0 runner    (1001) docker     (123)    14477 2023-05-09 10:05:20.000000 brightsky-2.0.2/tests/test_parsers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3430 2023-05-09 10:05:20.000000 brightsky-2.0.2/tests/test_polling.py
--rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-05-09 10:05:20.000000 brightsky-2.0.2/tests/test_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     3130 2023-05-09 10:05:20.000000 brightsky-2.0.2/tests/test_tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)      803 2023-05-09 10:05:20.000000 brightsky-2.0.2/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    18743 2023-05-09 10:05:20.000000 brightsky-2.0.2/tests/test_web.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 14:11:00.779039 brightsky-2.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-22 14:10:54.000000 brightsky-2.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8318 2023-05-22 14:11:00.779039 brightsky-2.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7713 2023-05-22 14:10:54.000000 brightsky-2.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 14:11:00.775040 brightsky-2.0.3/brightsky/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-22 14:10:54.000000 brightsky-2.0.3/brightsky/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-05-22 14:10:54.000000 brightsky-2.0.3/brightsky/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4898 2023-05-22 14:10:54.000000 brightsky-2.0.3/brightsky/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2578 2023-05-22 14:10:54.000000 brightsky-2.0.3/brightsky/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9369 2023-05-22 14:10:54.000000 brightsky-2.0.3/brightsky/export.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6033 2023-05-22 14:10:54.000000 brightsky-2.0.3/brightsky/parsers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4323 2023-05-22 14:10:54.000000 brightsky-2.0.3/brightsky/polling.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13658 2023-05-22 14:10:54.000000 brightsky-2.0.3/brightsky/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-05-22 14:10:54.000000 brightsky-2.0.3/brightsky/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5001 2023-05-22 14:10:54.000000 brightsky-2.0.3/brightsky/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-05-22 14:10:54.000000 brightsky-2.0.3/brightsky/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13263 2023-05-22 14:10:54.000000 brightsky-2.0.3/brightsky/web.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2160 2023-05-22 14:10:54.000000 brightsky-2.0.3/brightsky/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 14:11:00.775040 brightsky-2.0.3/brightsky.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8318 2023-05-22 14:11:00.000000 brightsky-2.0.3/brightsky.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-05-22 14:11:00.000000 brightsky-2.0.3/brightsky.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 14:11:00.000000 brightsky-2.0.3/brightsky.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-05-22 14:11:00.000000 brightsky-2.0.3/brightsky.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-22 14:11:00.000000 brightsky-2.0.3/brightsky.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-22 14:10:54.000000 brightsky-2.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 14:11:00.779039 brightsky-2.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-05-22 14:10:54.000000 brightsky-2.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 14:11:00.779039 brightsky-2.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-22 14:10:54.000000 brightsky-2.0.3/tests/test_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5341 2023-05-22 14:10:54.000000 brightsky-2.0.3/tests/test_export.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14477 2023-05-22 14:10:54.000000 brightsky-2.0.3/tests/test_parsers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3430 2023-05-22 14:10:54.000000 brightsky-2.0.3/tests/test_polling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-05-22 14:10:54.000000 brightsky-2.0.3/tests/test_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3130 2023-05-22 14:10:54.000000 brightsky-2.0.3/tests/test_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      803 2023-05-22 14:10:54.000000 brightsky-2.0.3/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20671 2023-05-22 14:10:54.000000 brightsky-2.0.3/tests/test_web.py
```

### Comparing `brightsky-2.0.2/LICENSE` & `brightsky-2.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `brightsky-2.0.2/PKG-INFO` & `brightsky-2.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brightsky
-Version: 2.0.2
+Version: 2.0.3
 Summary: JSON API for DWD's open weather data.
 Home-page: https://brightsky.dev/
 Author: Jakob de Maeyer
 Author-email: jakob@naboa.de
 Project-URL: Documentation, https://brightsky.dev/docs/
 Project-URL: Source, https://github.com/jdemaeyer/brightsky/
 Project-URL: Tracker, https://github.com/jdemaeyer/brightsky/issues/
```

### Comparing `brightsky-2.0.2/README.md` & `brightsky-2.0.3/README.md`

 * *Files identical despite different names*

### Comparing `brightsky-2.0.2/brightsky/__main__.py` & `brightsky-2.0.3/brightsky/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,10 +13,10 @@
     load_dotenv()
     configure_logging()
     if os.getenv('SENTRY_DSN'):
         import sentry_sdk
         sentry_sdk.init(
             dsn=os.getenv('SENTRY_DSN'),
             traces_sample_rate=_getenv_float('SENTRY_TRACES_SAMPLE_RATE'),
-            profiles_sample_rate=_getenv_float('PROFILES_TRACES_SAMPLE_RATE'),
+            profiles_sample_rate=_getenv_float('SENTRY_PROFILES_SAMPLE_RATE'),
         )
     cli(prog_name='python -m brightsky')
```

### Comparing `brightsky-2.0.2/brightsky/cli.py` & `brightsky-2.0.3/brightsky/cli.py`

 * *Files identical despite different names*

### Comparing `brightsky-2.0.2/brightsky/db.py` & `brightsky-2.0.3/brightsky/db.py`

 * *Files identical despite different names*

### Comparing `brightsky-2.0.2/brightsky/export.py` & `brightsky-2.0.3/brightsky/export.py`

 * *Files identical despite different names*

### Comparing `brightsky-2.0.2/brightsky/parsers.py` & `brightsky-2.0.3/brightsky/parsers.py`

 * *Files identical despite different names*

### Comparing `brightsky-2.0.2/brightsky/polling.py` & `brightsky-2.0.3/brightsky/polling.py`

 * *Files identical despite different names*

### Comparing `brightsky-2.0.2/brightsky/query.py` & `brightsky-2.0.3/brightsky/query.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import datetime
+from functools import cached_property
 
 import numpy as np
 from dateutil.tz import tzutc
 from isal import isal_zlib as zlib
+from pyproj import CRS, Transformer
 
 from brightsky.db import fetch
 
 
 def _make_dicts(rows):
     return [dict(row) for row in rows]
 
@@ -191,17 +193,39 @@
     }
     return {
         'weather': _make_dicts(fetch(sql, params)),
         'sources': _make_dicts(sources_rows),
     }
 
 
-def radar(date, last_date=None, fmt='compressed', bbox=None):
+def radar(
+        date, last_date=None, lat=None, lon=None, distance=200000,
+        fmt='compressed', bbox=None):
+    extra = {}
     if not last_date:
         last_date = date + datetime.timedelta(hours=2)
+    if lat or lon:
+        if not lat and lon:
+            raise ValueError("Please supply either both lat and lon, or none")
+        x, y = _transformer.to_xy(lat, lon)
+        if not -0.5 <= x <= 1099.5 or not -0.5 <= y <= 1199.5:
+            raise LookupError("lat/lon lies outside the radar data range")
+        center_x = int(round(x))
+        center_y = int(round(y))
+        pixels = distance // 1000
+        bbox = (
+            max(center_y - pixels, 0),
+            max(center_x - pixels, 0),
+            min(center_y + pixels, 1199),
+            min(center_x + pixels, 1099),
+        )
+        extra['latlon_position'] = {
+            'x': round(x - bbox[1], 3),
+            'y': round(y - bbox[0], 3),
+        }
     sql = """
         SELECT *
         FROM radar
         WHERE timestamp BETWEEN %(date)s AND %(last_date)s
         ORDER BY timestamp
         """
     params = {
@@ -222,14 +246,16 @@
             row['precipitation_5'] = zlib.compress(
                 _load_radar(row['precipitation_5'], bbox),
             )
     elif fmt != 'compressed':
         raise ValueError("Unknown format: '%s'" % fmt)
     return {
         'radar': _make_dicts(rows),
+        'geometry': _transformer.bbox_to_geometry(bbox),
+        **extra,
     }
 
 
 def _load_radar(raw, bbox, width=1100, height=1200):
     precip = np.frombuffer(
         zlib.decompress(raw),
         dtype='i2',
@@ -238,14 +264,63 @@
         top, left, bottom, right = bbox
         precip = precip[top:bottom+1, left:right+1]
         # Arrays must be C-contiguous for orjson and zlib
         precip = np.ascontiguousarray(precip).reshape(precip.shape)
     return precip
 
 
+class RadarCoordinatesTransformer:
+
+    PROJ_STR = (
+        "+proj=stere +lat_0=90 +lat_ts=60 +lon_0=10 +a=6378137 "
+        "+b=6356752.3142451802 +no_defs +x_0=543196.83521776402 "
+        "+y_0=3622588.8619310018"
+    )
+
+    @cached_property
+    def de1200(self):
+        return CRS.from_proj4(self.PROJ_STR)
+
+    @cached_property
+    def wgs84_to_de1200(self):
+        return Transformer.from_crs(4326, self.de1200)
+
+    @cached_property
+    def de1200_to_wgs84(self):
+        return Transformer.from_crs(self.de1200, 4326)
+
+    def to_xy(self, lat, lon):
+        x, y = self.wgs84_to_de1200.transform(lat, lon)
+        return round(x) / 1000, -round(y) / 1000
+
+    def to_latlon(self, x, y):
+        lat, lon = self.de1200_to_wgs84.transform(x * 1000, -y * 1000)
+        return round(lat, 5), round(lon, 5)
+
+    def to_lonlat(self, x, y):
+        return tuple(reversed(self.to_latlon(x, y)))
+
+    def bbox_to_geometry(self, bbox):
+        if not bbox:
+            bbox = (0, 0, 1199, 1099)
+        top, left, bottom, right = bbox
+        return {
+            'type': 'Geometry',
+            'coordinates': [
+                self.to_lonlat(left - .5, top - .5),
+                self.to_lonlat(left - .5, bottom + .5),
+                self.to_lonlat(right + .5, bottom + .5),
+                self.to_lonlat(right + .5, top - .5),
+            ],
+        }
+
+
+_transformer = RadarCoordinatesTransformer()
+
+
 def sources(
         lat=None, lon=None, dwd_station_id=None, wmo_station_id=None,
         source_id=None, observation_types=None, max_dist=50000,
         ignore_type=False, date=None, last_date=None):
     select = "*"
     order_by = "observation_type"
     params = {
```

### Comparing `brightsky-2.0.2/brightsky/settings.py` & `brightsky-2.0.3/brightsky/settings.py`

 * *Files identical despite different names*

### Comparing `brightsky-2.0.2/brightsky/tasks.py` & `brightsky-2.0.3/brightsky/tasks.py`

 * *Files identical despite different names*

### Comparing `brightsky-2.0.2/brightsky/utils.py` & `brightsky-2.0.3/brightsky/utils.py`

 * *Files identical despite different names*

### Comparing `brightsky-2.0.2/brightsky/web.py` & `brightsky-2.0.3/brightsky/web.py`

 * *Files 4% similar despite different names*

```diff
@@ -218,37 +218,50 @@
 
 
 class RadarResource(BrightskyResource):
 
     ALLOWED_FORMATS = ['compressed', 'bytes', 'plain']
 
     def on_get(self, req, resp):
+        lat, lon = self.parse_location(req)
+        distance = req.get_param_as_int(
+            'distance',
+            min_value=0,
+            default=200000,
+        )
         fmt = self.parse_format(req)
         if fmt == 'compressed':
             # Prevent traefik from gzipping the pre-compressed content
             resp.set_header('Content-Encoding', 'identity')
         else:
             self.force_compression(req)
         if not req.get_param('date'):
             date = fetch(
                 "select max(timestamp) - '3 hours'::interval from radar"
             )[0][0]
-            print(date)
             last_date = None
         else:
             date, last_date = self.parse_date_range(req)
         timezone = self.parse_timezone(req)
         if timezone:
             if not date.tzinfo:
                 date = date.replace(tzinfo=timezone)
             if last_date and not last_date.tzinfo:
                 last_date = last_date.replace(tzinfo=timezone)
         bbox = self.parse_bbox(req)
         with convert_exceptions():
-            result = query.radar(date, last_date=last_date, fmt=fmt, bbox=bbox)
+            result = query.radar(
+                date,
+                last_date=last_date,
+                lat=lat,
+                lon=lon,
+                distance=distance,
+                fmt=fmt,
+                bbox=bbox,
+            )
         for row in result['radar']:
             self.process_timestamp(row, 'timestamp', timezone)
         resp.media = result
 
     def force_compression(self, req):
         # traefik has no support for brotli or deflate
         if 'gzip' not in req.headers.get('ACCEPT-ENCODING', ''):
```

### Comparing `brightsky-2.0.2/brightsky/worker.py` & `brightsky-2.0.3/brightsky/worker.py`

 * *Files identical despite different names*

### Comparing `brightsky-2.0.2/brightsky.egg-info/PKG-INFO` & `brightsky-2.0.3/brightsky.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brightsky
-Version: 2.0.2
+Version: 2.0.3
 Summary: JSON API for DWD's open weather data.
 Home-page: https://brightsky.dev/
 Author: Jakob de Maeyer
 Author-email: jakob@naboa.de
 Project-URL: Documentation, https://brightsky.dev/docs/
 Project-URL: Source, https://github.com/jdemaeyer/brightsky/
 Project-URL: Tracker, https://github.com/jdemaeyer/brightsky/issues/
```

### Comparing `brightsky-2.0.2/brightsky.egg-info/SOURCES.txt` & `brightsky-2.0.3/brightsky.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `brightsky-2.0.2/setup.py` & `brightsky-2.0.3/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -36,13 +36,14 @@
         'gunicorn',
         'huey',
         'isal',
         'numpy',
         'orjson',
         'parsel',
         'psycopg2-binary',
+        'pyproj',
         'python-dateutil',
         'redis',
         'requests',
         'sentry-sdk',
     ],
 )
```

### Comparing `brightsky-2.0.2/tests/test_export.py` & `brightsky-2.0.3/tests/test_export.py`

 * *Files identical despite different names*

### Comparing `brightsky-2.0.2/tests/test_parsers.py` & `brightsky-2.0.3/tests/test_parsers.py`

 * *Files identical despite different names*

### Comparing `brightsky-2.0.2/tests/test_polling.py` & `brightsky-2.0.3/tests/test_polling.py`

 * *Files identical despite different names*

### Comparing `brightsky-2.0.2/tests/test_settings.py` & `brightsky-2.0.3/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `brightsky-2.0.2/tests/test_tasks.py` & `brightsky-2.0.3/tests/test_tasks.py`

 * *Files identical despite different names*

### Comparing `brightsky-2.0.2/tests/test_utils.py` & `brightsky-2.0.3/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `brightsky-2.0.2/tests/test_web.py` & `brightsky-2.0.3/tests/test_web.py`

 * *Files 9% similar despite different names*

```diff
@@ -521,14 +521,66 @@
 def test_radar_response_plain(radar_data, api):
     data = _get_radar_data(api, 'plain')
     _check_radar_data(data)
     clip = _get_radar_data(api, 'plain', bbox=True)
     _check_radar_data(clip)
 
 
+def test_radar_response_geometry(radar_data, api):
+    resp = api.simulate_get('/radar?date=2023-05-08T11:30')
+    assert resp.json['geometry']['type'] == 'Geometry'
+    assert 'latlon_position' not in resp.json
+    expected_coords = [
+        (1.4633, 55.86209),
+        (3.56699, 45.69643),
+        (16.58087, 45.68461),
+        (18.73162, 55.84544),
+    ]
+    for p, exp_p in zip(resp.json['geometry']['coordinates'], expected_coords):
+        assert p[0] == pytest.approx(exp_p[0])
+        assert p[1] == pytest.approx(exp_p[1])
+
+
+def test_radar_response_bbox_geometry(radar_data, api):
+    resp = api.simulate_get(
+        '/radar?date=2023-05-08T11:30&lat=52&lon=7.6&distance=200000',
+    )
+    assert resp.json['geometry']['type'] == 'Geometry'
+    expected_coords = [
+        (4.54411, 53.61306),
+        (5.04988, 50.17614),
+        (10.37685, 50.31264),
+        (10.41558, 53.76658),
+    ]
+    for p, exp_p in zip(resp.json['geometry']['coordinates'], expected_coords):
+        assert p[0] == pytest.approx(exp_p[0])
+        assert p[1] == pytest.approx(exp_p[1])
+    assert resp.json['latlon_position']['x'] == pytest.approx(200.244)
+    assert resp.json['latlon_position']['y'] == pytest.approx(200.088)
+
+
+def test_radar_response_bbox_geometry_near_edge(radar_data, api):
+    resp = api.simulate_get(
+        '/radar?date=2023-05-08T11:30&lat=52&lon=2.6&distance=200000'
+        '&fmt=plain',
+    )
+    assert resp.json['geometry']['type'] == 'Geometry'
+    expected_coords = [
+        (2.00507, 53.70663),
+        (2.74712, 50.28395),
+        (5.6003, 50.47017),
+        (5.14662, 53.91603),
+    ]
+    for p, exp_p in zip(resp.json['geometry']['coordinates'], expected_coords):
+        assert p[0] == pytest.approx(exp_p[0])
+        assert p[1] == pytest.approx(exp_p[1])
+    assert resp.json['latlon_position']['x'] == pytest.approx(14.326)
+    assert resp.json['latlon_position']['y'] == pytest.approx(200.489)
+
+
 def test_status_response(api):
     resp = api.simulate_get('/')
     assert resp.status_code == 200
     assert resp.json['name'] == 'brightsky'
     assert resp.json['version'] == brightsky.__version__
     assert resp.json['status'] == 'ok'
```

