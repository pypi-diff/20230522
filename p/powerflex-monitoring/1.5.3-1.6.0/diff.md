# Comparing `tmp/powerflex-monitoring-1.5.3.tar.gz` & `tmp/powerflex-monitoring-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "powerflex-monitoring-1.5.3.tar", last modified: Mon May  1 17:58:26 2023, max compression
+gzip compressed data, was "powerflex-monitoring-1.6.0.tar", last modified: Mon May 22 19:09:11 2023, max compression
```

## Comparing `powerflex-monitoring-1.5.3.tar` & `powerflex-monitoring-1.6.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 mark.zanfardino   (501) staff       (20)        0 2023-05-01 17:58:26.588663 powerflex-monitoring-1.5.3/
--rw-r--r--   0 mark.zanfardino   (501) staff       (20)     5459 2023-05-01 17:58:26.588271 powerflex-monitoring-1.5.3/PKG-INFO
--rw-r--r--   0 mark.zanfardino   (501) staff       (20)     4504 2023-05-01 17:11:13.000000 powerflex-monitoring-1.5.3/README.md
--rw-r--r--   0 mark.zanfardino   (501) staff       (20)      100 2022-08-08 15:22:55.000000 powerflex-monitoring-1.5.3/pyproject.toml
--rw-r--r--   0 mark.zanfardino   (501) staff       (20)       38 2023-05-01 17:58:26.588882 powerflex-monitoring-1.5.3/setup.cfg
--rw-r--r--   0 mark.zanfardino   (501) staff       (20)     2050 2023-05-01 17:11:13.000000 powerflex-monitoring-1.5.3/setup.py
-drwxr-xr-x   0 mark.zanfardino   (501) staff       (20)        0 2023-05-01 17:58:26.554098 powerflex-monitoring-1.5.3/src/
-drwxr-xr-x   0 mark.zanfardino   (501) staff       (20)        0 2023-05-01 17:58:26.584193 powerflex-monitoring-1.5.3/src/powerflex_monitoring/
--rw-r--r--   0 mark.zanfardino   (501) staff       (20)        6 2023-05-01 17:24:25.000000 powerflex-monitoring-1.5.3/src/powerflex_monitoring/VERSION
--rw-r--r--   0 mark.zanfardino   (501) staff       (20)      171 2022-08-08 15:22:55.000000 powerflex-monitoring-1.5.3/src/powerflex_monitoring/__init__.py
--rw-r--r--   0 mark.zanfardino   (501) staff       (20)     2110 2023-05-01 17:11:13.000000 powerflex-monitoring-1.5.3/src/powerflex_monitoring/diagnostic_recorder.py
--rw-r--r--   0 mark.zanfardino   (501) staff       (20)      333 2022-08-08 15:22:55.000000 powerflex-monitoring-1.5.3/src/powerflex_monitoring/format_exception.py
--rw-r--r--   0 mark.zanfardino   (501) staff       (20)     1419 2023-05-01 17:11:13.000000 powerflex-monitoring-1.5.3/src/powerflex_monitoring/health_check.py
--rw-r--r--   0 mark.zanfardino   (501) staff       (20)     2466 2023-05-01 17:11:13.000000 powerflex-monitoring-1.5.3/src/powerflex_monitoring/monitoring.py
--rw-r--r--   0 mark.zanfardino   (501) staff       (20)     9687 2023-05-01 17:11:13.000000 powerflex-monitoring-1.5.3/src/powerflex_monitoring/nats_health_check.py
--rw-r--r--   0 mark.zanfardino   (501) staff       (20)     1549 2023-05-01 17:11:13.000000 powerflex-monitoring-1.5.3/src/powerflex_monitoring/prometheus_metrics.py
--rw-r--r--   0 mark.zanfardino   (501) staff       (20)        0 2022-08-10 21:43:07.000000 powerflex-monitoring-1.5.3/src/powerflex_monitoring/py.typed
--rw-r--r--   0 mark.zanfardino   (501) staff       (20)     4603 2023-05-01 17:11:13.000000 powerflex-monitoring-1.5.3/src/powerflex_monitoring/ready_check.py
--rw-r--r--   0 mark.zanfardino   (501) staff       (20)     9471 2023-05-01 17:11:13.000000 powerflex-monitoring-1.5.3/src/powerflex_monitoring/redis_health_check.py
--rw-r--r--   0 mark.zanfardino   (501) staff       (20)     1320 2022-08-10 21:43:07.000000 powerflex-monitoring-1.5.3/src/powerflex_monitoring/server_base.py
--rw-r--r--   0 mark.zanfardino   (501) staff       (20)     3119 2022-08-08 15:22:55.000000 powerflex-monitoring-1.5.3/src/powerflex_monitoring/wait_for_service_ready.py
-drwxr-xr-x   0 mark.zanfardino   (501) staff       (20)        0 2023-05-01 17:58:26.587256 powerflex-monitoring-1.5.3/src/powerflex_monitoring.egg-info/
--rw-r--r--   0 mark.zanfardino   (501) staff       (20)     5459 2023-05-01 17:58:26.000000 powerflex-monitoring-1.5.3/src/powerflex_monitoring.egg-info/PKG-INFO
--rw-r--r--   0 mark.zanfardino   (501) staff       (20)      863 2023-05-01 17:58:26.000000 powerflex-monitoring-1.5.3/src/powerflex_monitoring.egg-info/SOURCES.txt
--rw-r--r--   0 mark.zanfardino   (501) staff       (20)        1 2023-05-01 17:58:26.000000 powerflex-monitoring-1.5.3/src/powerflex_monitoring.egg-info/dependency_links.txt
--rw-r--r--   0 mark.zanfardino   (501) staff       (20)      149 2023-05-01 17:58:26.000000 powerflex-monitoring-1.5.3/src/powerflex_monitoring.egg-info/requires.txt
--rw-r--r--   0 mark.zanfardino   (501) staff       (20)       21 2023-05-01 17:58:26.000000 powerflex-monitoring-1.5.3/src/powerflex_monitoring.egg-info/top_level.txt
--rw-r--r--   0 mark.zanfardino   (501) staff       (20)        1 2022-08-08 15:26:44.000000 powerflex-monitoring-1.5.3/src/powerflex_monitoring.egg-info/zip-safe
+drwxr-xr-x   0 nico       (501) staff       (20)        0 2023-05-22 19:09:11.595299 powerflex-monitoring-1.6.0/
+-rw-r--r--   0 nico       (501) staff       (20)     5459 2023-05-22 19:09:11.594959 powerflex-monitoring-1.6.0/PKG-INFO
+-rw-r--r--   0 nico       (501) staff       (20)     4504 2023-04-26 12:47:58.000000 powerflex-monitoring-1.6.0/README.md
+-rw-r--r--   0 nico       (501) staff       (20)      100 2023-04-26 12:47:58.000000 powerflex-monitoring-1.6.0/pyproject.toml
+-rw-r--r--   0 nico       (501) staff       (20)       38 2023-05-22 19:09:11.595395 powerflex-monitoring-1.6.0/setup.cfg
+-rw-r--r--   0 nico       (501) staff       (20)     2050 2023-04-26 12:47:58.000000 powerflex-monitoring-1.6.0/setup.py
+drwxr-xr-x   0 nico       (501) staff       (20)        0 2023-05-22 19:09:11.582810 powerflex-monitoring-1.6.0/src/
+drwxr-xr-x   0 nico       (501) staff       (20)        0 2023-05-22 19:09:11.591800 powerflex-monitoring-1.6.0/src/powerflex_monitoring/
+-rw-r--r--   0 nico       (501) staff       (20)        6 2023-05-22 18:47:21.000000 powerflex-monitoring-1.6.0/src/powerflex_monitoring/VERSION
+-rw-r--r--   0 nico       (501) staff       (20)      171 2023-04-26 12:47:58.000000 powerflex-monitoring-1.6.0/src/powerflex_monitoring/__init__.py
+-rw-r--r--   0 nico       (501) staff       (20)     2110 2023-04-26 12:47:58.000000 powerflex-monitoring-1.6.0/src/powerflex_monitoring/diagnostic_recorder.py
+-rw-r--r--   0 nico       (501) staff       (20)      333 2023-04-26 12:47:58.000000 powerflex-monitoring-1.6.0/src/powerflex_monitoring/format_exception.py
+-rw-r--r--   0 nico       (501) staff       (20)     1419 2023-04-26 12:47:58.000000 powerflex-monitoring-1.6.0/src/powerflex_monitoring/health_check.py
+-rw-r--r--   0 nico       (501) staff       (20)     2466 2023-04-26 12:47:58.000000 powerflex-monitoring-1.6.0/src/powerflex_monitoring/monitoring.py
+-rw-r--r--   0 nico       (501) staff       (20)     9687 2023-05-18 16:44:23.000000 powerflex-monitoring-1.6.0/src/powerflex_monitoring/nats_health_check.py
+-rw-r--r--   0 nico       (501) staff       (20)     1549 2023-04-26 12:47:58.000000 powerflex-monitoring-1.6.0/src/powerflex_monitoring/prometheus_metrics.py
+-rw-r--r--   0 nico       (501) staff       (20)        0 2023-04-26 12:47:58.000000 powerflex-monitoring-1.6.0/src/powerflex_monitoring/py.typed
+-rw-r--r--   0 nico       (501) staff       (20)     4603 2023-04-26 12:47:58.000000 powerflex-monitoring-1.6.0/src/powerflex_monitoring/ready_check.py
+-rw-r--r--   0 nico       (501) staff       (20)    10200 2023-05-22 18:43:42.000000 powerflex-monitoring-1.6.0/src/powerflex_monitoring/redis_health_check.py
+-rw-r--r--   0 nico       (501) staff       (20)     1320 2023-04-26 12:47:58.000000 powerflex-monitoring-1.6.0/src/powerflex_monitoring/server_base.py
+-rw-r--r--   0 nico       (501) staff       (20)     3119 2023-04-26 12:47:58.000000 powerflex-monitoring-1.6.0/src/powerflex_monitoring/wait_for_service_ready.py
+drwxr-xr-x   0 nico       (501) staff       (20)        0 2023-05-22 19:09:11.594178 powerflex-monitoring-1.6.0/src/powerflex_monitoring.egg-info/
+-rw-r--r--   0 nico       (501) staff       (20)     5459 2023-05-22 19:09:11.000000 powerflex-monitoring-1.6.0/src/powerflex_monitoring.egg-info/PKG-INFO
+-rw-r--r--   0 nico       (501) staff       (20)      863 2023-05-22 19:09:11.000000 powerflex-monitoring-1.6.0/src/powerflex_monitoring.egg-info/SOURCES.txt
+-rw-r--r--   0 nico       (501) staff       (20)        1 2023-05-22 19:09:11.000000 powerflex-monitoring-1.6.0/src/powerflex_monitoring.egg-info/dependency_links.txt
+-rw-r--r--   0 nico       (501) staff       (20)      149 2023-05-22 19:09:11.000000 powerflex-monitoring-1.6.0/src/powerflex_monitoring.egg-info/requires.txt
+-rw-r--r--   0 nico       (501) staff       (20)       21 2023-05-22 19:09:11.000000 powerflex-monitoring-1.6.0/src/powerflex_monitoring.egg-info/top_level.txt
+-rw-r--r--   0 nico       (501) staff       (20)        1 2023-04-26 12:59:15.000000 powerflex-monitoring-1.6.0/src/powerflex_monitoring.egg-info/zip-safe
```

### Comparing `powerflex-monitoring-1.5.3/PKG-INFO` & `powerflex-monitoring-1.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: powerflex-monitoring
-Version: 1.5.3
+Version: 1.6.0
 Summary:  Tools to assist in monitoring a Python service.
 Home-page: https://github.com/edf-re/powerflex_python_monitoring
 Project-URL: Issue Tracker, https://github.com/edf-re/powerflex_python_monitoring/issues
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: Unix
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python
```

### Comparing `powerflex-monitoring-1.5.3/README.md` & `powerflex-monitoring-1.6.0/README.md`

 * *Files identical despite different names*

### Comparing `powerflex-monitoring-1.5.3/setup.py` & `powerflex-monitoring-1.6.0/setup.py`

 * *Files identical despite different names*

### Comparing `powerflex-monitoring-1.5.3/src/powerflex_monitoring/diagnostic_recorder.py` & `powerflex-monitoring-1.6.0/src/powerflex_monitoring/diagnostic_recorder.py`

 * *Files identical despite different names*

### Comparing `powerflex-monitoring-1.5.3/src/powerflex_monitoring/health_check.py` & `powerflex-monitoring-1.6.0/src/powerflex_monitoring/health_check.py`

 * *Files identical despite different names*

### Comparing `powerflex-monitoring-1.5.3/src/powerflex_monitoring/monitoring.py` & `powerflex-monitoring-1.6.0/src/powerflex_monitoring/monitoring.py`

 * *Files identical despite different names*

### Comparing `powerflex-monitoring-1.5.3/src/powerflex_monitoring/nats_health_check.py` & `powerflex-monitoring-1.6.0/src/powerflex_monitoring/nats_health_check.py`

 * *Files identical despite different names*

### Comparing `powerflex-monitoring-1.5.3/src/powerflex_monitoring/prometheus_metrics.py` & `powerflex-monitoring-1.6.0/src/powerflex_monitoring/prometheus_metrics.py`

 * *Files identical despite different names*

### Comparing `powerflex-monitoring-1.5.3/src/powerflex_monitoring/ready_check.py` & `powerflex-monitoring-1.6.0/src/powerflex_monitoring/ready_check.py`

 * *Files identical despite different names*

### Comparing `powerflex-monitoring-1.5.3/src/powerflex_monitoring/redis_health_check.py` & `powerflex-monitoring-1.6.0/src/powerflex_monitoring/redis_health_check.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import socket
 import time
 from collections import defaultdict
 from typing import Any, DefaultDict, Dict, NoReturn, Optional, TypeVar, Union, cast
 
 from pydantic import BaseSettings, Field
 from redis import Redis
+from redis.asyncio import Redis as AsyncRedis
 
 from powerflex_monitoring.format_exception import format_exception
 from powerflex_monitoring.monitoring import MonitoringServer
 
 logger = logging.getLogger(__name__)
 HOSTNAME_TEMPLATE_VAR = "{hostname}"
 
@@ -43,15 +44,17 @@
         description="Redis master set name.",
         default="mymaster",
     )
 
 
 class RedisHealthChecker:
     def __init__(
-        self, redis_conn: Redis[_StrType], monitoring_server: MonitoringServer
+        self,
+        redis_conn: Union[Redis[_StrType], AsyncRedis[_StrType]],
+        monitoring_server: MonitoringServer,
     ):
         self.config = RedisHealthCheckerConfig(
             # type:ignore
         )
 
         logger.info(
             "Configuration for Redis health check", extra={"config": self.config.dict()}
@@ -59,15 +62,14 @@
 
         self.redis_health_check_key = (
             self.config.REDIS_HEALTH_CHECK_KEY_TEMPLATE.replace(
                 HOSTNAME_TEMPLATE_VAR,
                 socket.gethostname(),
             )
         )
-
         self.redis_conn = redis_conn
         self.monitoring_server = monitoring_server
         self.time_since_redis_unhealthy: DefaultDict[
             str, Optional[float]
         ] = defaultdict(lambda: None)
 
     def on_unhealthy(self, health_check_name: str, cause: str) -> None:
@@ -122,23 +124,30 @@
         if not self.monitoring_server.ready_check.is_ready and all_health_checks_pass:
             self.monitoring_server.ready_check.set_ready(
                 ready=True,
                 cause="Redis is healthy again",
                 readiness_identifier="redis-identifier",
             )
 
-    def check_write_read_redis_service(self) -> None:
+    async def check_write_read_redis_service(  # pylint: disable=too-many-branches
+        self,
+    ) -> None:
         """Make a Redis write-read operation with a unique key to check Redis health."""
         health_check_name = self.check_write_read_redis_service.__name__
         test_value = str(time.time())
         result: Optional[bool] = False
         redis_value: Optional[str] = None
 
         try:
-            result = self.redis_conn.set(self.redis_health_check_key, test_value)
+            if isinstance(self.redis_conn, AsyncRedis):
+                result = await self.redis_conn.set(
+                    self.redis_health_check_key, test_value
+                )
+            else:
+                result = self.redis_conn.set(self.redis_health_check_key, test_value)
 
         except ConnectionError as exc:
             self.on_unhealthy(
                 health_check_name=health_check_name,
                 cause="Redis set to test writing a document failed. Exception: "
                 + format_exception(exc),
             )
@@ -149,15 +158,20 @@
                 cause="Unexpected exception when testing Redis SET operation. Exception: "
                 + format_exception(exc),
             )
             return
 
         if result:
             try:
-                _redis_value = self.redis_conn.get(self.redis_health_check_key)
+                if isinstance(self.redis_conn, AsyncRedis):
+                    _redis_value = await self.redis_conn.get(
+                        self.redis_health_check_key
+                    )
+                else:
+                    _redis_value = self.redis_conn.get(self.redis_health_check_key)
                 if _redis_value is not None:
                     if isinstance(_redis_value, bytes):
                         redis_value = _redis_value.decode("utf-8")
                     else:
                         redis_value = str(_redis_value)
             except ConnectionError as exc:
                 self.on_unhealthy(
@@ -180,21 +194,24 @@
             else:
                 self.on_unhealthy(
                     health_check_name=health_check_name,
                     cause="Redis GET operation returned an unexpected value."
                     f"Expected: {test_value}. Actual: {redis_value}",
                 )
 
-    def check_redis_service_health(self) -> None:
+    async def check_redis_service_health(self) -> None:
         """Check the Redis service's health to determine if it is healthy using the ping command."""
         health_check_name = self.check_redis_service_health.__name__
         try:
-            is_connected = self.redis_conn.ping()
+            if isinstance(self.redis_conn, AsyncRedis):
+                is_connected = await self.redis_conn.ping()
+            else:
+                is_connected = self.redis_conn.ping()
         except ConnectionError as exc:
-            connection_kwargs = cast(Dict[str, Any], self.redis_conn.get_connection_kwargs())  # type: ignore[no-untyped-call]
+            connection_kwargs = cast(Dict[str, Any], self.redis_conn.get_connection_kwargs())  # type: ignore[union-attr]
             self.on_unhealthy(
                 health_check_name=health_check_name,
                 cause="Could not connect to Redis service health check. "
                 + f"Host: {connection_kwargs.get('host', 'unknown')}, "
                 + f"Port: {connection_kwargs.get('port', 'unknown')}. Exception: "
                 + format_exception(exc),
             )
@@ -227,12 +244,11 @@
         REDIS_HEALTH_CHECK_UNHEALTHY_TIMEOUT_SEC,
         then mark the service as unhealth.
 
         If any health check fails at all, mark the service as not ready.
 
         Mark the service as ready if all health checks pass.
         """
-
         while True:
-            self.check_write_read_redis_service()
-            self.check_redis_service_health()
+            await self.check_write_read_redis_service()
+            await self.check_redis_service_health()
             await asyncio.sleep(self.config.REDIS_HEALTH_CHECK_REQUEST_PERIOD_SEC)
```

### Comparing `powerflex-monitoring-1.5.3/src/powerflex_monitoring/server_base.py` & `powerflex-monitoring-1.6.0/src/powerflex_monitoring/server_base.py`

 * *Files identical despite different names*

### Comparing `powerflex-monitoring-1.5.3/src/powerflex_monitoring/wait_for_service_ready.py` & `powerflex-monitoring-1.6.0/src/powerflex_monitoring/wait_for_service_ready.py`

 * *Files identical despite different names*

### Comparing `powerflex-monitoring-1.5.3/src/powerflex_monitoring.egg-info/PKG-INFO` & `powerflex-monitoring-1.6.0/src/powerflex_monitoring.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: powerflex-monitoring
-Version: 1.5.3
+Version: 1.6.0
 Summary:  Tools to assist in monitoring a Python service.
 Home-page: https://github.com/edf-re/powerflex_python_monitoring
 Project-URL: Issue Tracker, https://github.com/edf-re/powerflex_python_monitoring/issues
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: Unix
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python
```

### Comparing `powerflex-monitoring-1.5.3/src/powerflex_monitoring.egg-info/SOURCES.txt` & `powerflex-monitoring-1.6.0/src/powerflex_monitoring.egg-info/SOURCES.txt`

 * *Files identical despite different names*

