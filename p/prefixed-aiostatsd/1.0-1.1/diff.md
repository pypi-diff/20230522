# Comparing `tmp/prefixed_aiostatsd-1.0-py3-none-any.whl.zip` & `tmp/prefixed_aiostatsd-1.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 3156 bytes, number of entries: 6
--rw-r--r--  2.0 unx     3375 b- defN 23-May-22 18:13 prefixed_aiostatsd/__init__.py
--rw-r--r--  2.0 unx     1067 b- defN 23-May-22 18:19 prefixed_aiostatsd-1.0.dist-info/LICENSE
--rw-r--r--  2.0 unx      677 b- defN 23-May-22 18:19 prefixed_aiostatsd-1.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-22 18:19 prefixed_aiostatsd-1.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       19 b- defN 23-May-22 18:19 prefixed_aiostatsd-1.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      517 b- defN 23-May-22 18:19 prefixed_aiostatsd-1.0.dist-info/RECORD
-6 files, 5747 bytes uncompressed, 2210 bytes compressed:  61.5%
+Zip file size: 3164 bytes, number of entries: 6
+-rw-r--r--  2.0 unx     3276 b- defN 23-May-22 19:03 prefixed_aiostatsd/__init__.py
+-rw-r--r--  2.0 unx     1067 b- defN 23-May-22 19:05 prefixed_aiostatsd-1.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx      677 b- defN 23-May-22 19:05 prefixed_aiostatsd-1.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-22 19:05 prefixed_aiostatsd-1.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       19 b- defN 23-May-22 19:05 prefixed_aiostatsd-1.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      517 b- defN 23-May-22 19:05 prefixed_aiostatsd-1.1.dist-info/RECORD
+6 files, 5648 bytes uncompressed, 2218 bytes compressed:  60.7%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: prefixed_aiostatsd/__init__.py
 Comment: 
 
-Filename: prefixed_aiostatsd-1.0.dist-info/LICENSE
+Filename: prefixed_aiostatsd-1.1.dist-info/LICENSE
 Comment: 
 
-Filename: prefixed_aiostatsd-1.0.dist-info/METADATA
+Filename: prefixed_aiostatsd-1.1.dist-info/METADATA
 Comment: 
 
-Filename: prefixed_aiostatsd-1.0.dist-info/WHEEL
+Filename: prefixed_aiostatsd-1.1.dist-info/WHEEL
 Comment: 
 
-Filename: prefixed_aiostatsd-1.0.dist-info/top_level.txt
+Filename: prefixed_aiostatsd-1.1.dist-info/top_level.txt
 Comment: 
 
-Filename: prefixed_aiostatsd-1.0.dist-info/RECORD
+Filename: prefixed_aiostatsd-1.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## prefixed_aiostatsd/__init__.py

```diff
@@ -29,49 +29,44 @@
         packet_size: int = 512,
         flush_interval: float = 5.0,
     ) -> "StatsdClient":
         client = StatsdClientBase(host, port, packet_size, flush_interval)
         return StatsdClient(prefix, client)
 
     def __init__(self, prefix: str, client: StatsdClientBase) -> None:
-        assert prefix is not None
+        assert prefix, "Prefix must be defined."
 
         self._client = client
-        self._prefix = prefix
+        self._prefix = prefix + "."
 
     def with_suffix(self, suffix: str) -> IStatsdClient:
-        return StatsdClient(prefix=f"{self._prefix}.{suffix}", client=self._client)
+        return StatsdClient(prefix=self._prefix + suffix, client=self._client)
 
     def send_counter(self, name: str, *args: Any, **kwargs: Any) -> None:
-        name = f"{self._prefix}.{name}"
-        self._client.send_counter(name, *args, **kwargs)
+        self._client.send_counter(self._prefix + name, *args, **kwargs)
 
     def send_timer(self, name: str, *args: Any, **kwargs: Any) -> None:
-        name = f"{self._prefix}.{name}"
-        self._client.send_timer(name, *args, **kwargs)
+        self._client.send_timer(self._prefix + name, *args, **kwargs)
 
     def send_gauge(self, name: str, *args: Any, **kwargs: Any) -> None:
-        name = f"{self._prefix}.{name}"
-        self._client.send_gauge(name, *args, **kwargs)
+        self._client.send_gauge(self._prefix + name, *args, **kwargs)
 
     def incr(self, name: str, *args: Any, **kwargs: Any) -> None:
-        name = f"{self._prefix}.{name}"
-        self._client.incr(name, *args, **kwargs)
+        self._client.incr(self._prefix + name, *args, **kwargs)
 
     def decr(self, name: str, *args: Any, **kwargs: Any) -> None:
-        name = f"{self._prefix}.{name}"
-        self._client.decr(name, *args, **kwargs)
+        self._client.decr(self._prefix + name, *args, **kwargs)
 
     @contextlib.contextmanager
     def timer(self, name: str, rate: float = 1.0) -> Iterator[None]:
-        start = time.time()
+        start = time.monotonic()
         try:
             yield
         finally:
-            duration_sec = time.time() - start
+            duration_sec = time.monotonic() - start
             duration_msec = int(round(duration_sec * 1000))
             self.send_timer(name, duration_msec, rate=rate)
 
     async def run(self) -> None:
         await self._client.run()
 
     async def stop(self) -> None:
```

## Comparing `prefixed_aiostatsd-1.0.dist-info/LICENSE` & `prefixed_aiostatsd-1.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `prefixed_aiostatsd-1.0.dist-info/METADATA` & `prefixed_aiostatsd-1.1.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prefixed-aiostatsd
-Version: 1.0
+Version: 1.1
 Summary: Prefixed AioStatsD
 Home-page: https://github.com/DomainsBot/prefixed-aiostatsd
 Author: Domainsbot
 Author-email: tech@domainsbot.com
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: POSIX :: Linux
```

