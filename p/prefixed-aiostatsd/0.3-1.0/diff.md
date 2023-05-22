# Comparing `tmp/prefixed_aiostatsd-0.3-py3-none-any.whl.zip` & `tmp/prefixed_aiostatsd-1.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 2925 bytes, number of entries: 6
--rw-r--r--  2.0 unx     2787 b- defN 22-Apr-16 19:26 prefixed_aiostatsd/__init__.py
--rw-r--r--  2.0 unx     1067 b- defN 22-Apr-16 19:28 prefixed_aiostatsd-0.3.dist-info/LICENSE
--rw-r--r--  2.0 unx      447 b- defN 22-Apr-16 19:28 prefixed_aiostatsd-0.3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 22-Apr-16 19:28 prefixed_aiostatsd-0.3.dist-info/WHEEL
--rw-r--r--  2.0 unx       19 b- defN 22-Apr-16 19:28 prefixed_aiostatsd-0.3.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      517 b- defN 22-Apr-16 19:28 prefixed_aiostatsd-0.3.dist-info/RECORD
-6 files, 4929 bytes uncompressed, 1979 bytes compressed:  59.8%
+Zip file size: 3156 bytes, number of entries: 6
+-rw-r--r--  2.0 unx     3375 b- defN 23-May-22 18:13 prefixed_aiostatsd/__init__.py
+-rw-r--r--  2.0 unx     1067 b- defN 23-May-22 18:19 prefixed_aiostatsd-1.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx      677 b- defN 23-May-22 18:19 prefixed_aiostatsd-1.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-22 18:19 prefixed_aiostatsd-1.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       19 b- defN 23-May-22 18:19 prefixed_aiostatsd-1.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      517 b- defN 23-May-22 18:19 prefixed_aiostatsd-1.0.dist-info/RECORD
+6 files, 5747 bytes uncompressed, 2210 bytes compressed:  61.5%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: prefixed_aiostatsd/__init__.py
 Comment: 
 
-Filename: prefixed_aiostatsd-0.3.dist-info/LICENSE
+Filename: prefixed_aiostatsd-1.0.dist-info/LICENSE
 Comment: 
 
-Filename: prefixed_aiostatsd-0.3.dist-info/METADATA
+Filename: prefixed_aiostatsd-1.0.dist-info/METADATA
 Comment: 
 
-Filename: prefixed_aiostatsd-0.3.dist-info/WHEEL
+Filename: prefixed_aiostatsd-1.0.dist-info/WHEEL
 Comment: 
 
-Filename: prefixed_aiostatsd-0.3.dist-info/top_level.txt
+Filename: prefixed_aiostatsd-1.0.dist-info/top_level.txt
 Comment: 
 
-Filename: prefixed_aiostatsd-0.3.dist-info/RECORD
+Filename: prefixed_aiostatsd-1.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## prefixed_aiostatsd/__init__.py

```diff
@@ -1,17 +1,29 @@
+import abc
 import contextlib
 import time
-from typing import Any, Iterator
+from collections.abc import Iterator
+from typing import Any
 
 from aiostatsd.client import StatsdClient as StatsdClientBase
 
 
-class StatsdClient:
-    """This class is needed in order to add the param :prefix: to the
-    statsd client since is not supported in aiostatsd."""
+class IStatsdClient(StatsdClientBase, metaclass=abc.ABCMeta):
+    def __init__(self) -> None:
+        pass  # Override parent initializer. We don't want implementation inheritance.
+
+    @abc.abstractmethod
+    def with_suffix(self, suffix: str) -> "IStatsdClient":
+        """Returns an IStatsdClient with and additional prefix."""
+
+
+class StatsdClient(IStatsdClient):
+    """This class is needed to add the param :prefix: to the
+    statsd client since is not supported in aiostatsd.
+    """
 
     @staticmethod
     def from_host(
         prefix: str,
         host: str,
         port: int,
         packet_size: int = 512,
@@ -22,32 +34,35 @@
 
     def __init__(self, prefix: str, client: StatsdClientBase) -> None:
         assert prefix is not None
 
         self._client = client
         self._prefix = prefix
 
+    def with_suffix(self, suffix: str) -> IStatsdClient:
+        return StatsdClient(prefix=f"{self._prefix}.{suffix}", client=self._client)
+
     def send_counter(self, name: str, *args: Any, **kwargs: Any) -> None:
-        name = "%s.%s" % (self._prefix, name)
+        name = f"{self._prefix}.{name}"
         self._client.send_counter(name, *args, **kwargs)
 
     def send_timer(self, name: str, *args: Any, **kwargs: Any) -> None:
-        name = "%s.%s" % (self._prefix, name)
+        name = f"{self._prefix}.{name}"
         self._client.send_timer(name, *args, **kwargs)
 
     def send_gauge(self, name: str, *args: Any, **kwargs: Any) -> None:
-        name = "%s.%s" % (self._prefix, name)
+        name = f"{self._prefix}.{name}"
         self._client.send_gauge(name, *args, **kwargs)
 
     def incr(self, name: str, *args: Any, **kwargs: Any) -> None:
-        name = "%s.%s" % (self._prefix, name)
+        name = f"{self._prefix}.{name}"
         self._client.incr(name, *args, **kwargs)
 
     def decr(self, name: str, *args: Any, **kwargs: Any) -> None:
-        name = "%s.%s" % (self._prefix, name)
+        name = f"{self._prefix}.{name}"
         self._client.decr(name, *args, **kwargs)
 
     @contextlib.contextmanager
     def timer(self, name: str, rate: float = 1.0) -> Iterator[None]:
         start = time.time()
         try:
             yield
@@ -59,17 +74,20 @@
     async def run(self) -> None:
         await self._client.run()
 
     async def stop(self) -> None:
         await self._client.stop()
 
 
-class EmptyStatsdClient:
+class EmptyStatsdClient(IStatsdClient):
     """Null implementation of StatsdClient."""
 
+    def with_suffix(self, suffix: str) -> IStatsdClient:
+        return self
+
     def send_counter(self, name: str, *args: Any, **kwargs: Any) -> None:
         pass
 
     def send_timer(self, name: str, *args: Any, **kwargs: Any) -> None:
         pass
 
     def send_gauge(self, name: str, *args: Any, **kwargs: Any) -> None:
```

## Comparing `prefixed_aiostatsd-0.3.dist-info/LICENSE` & `prefixed_aiostatsd-1.0.dist-info/LICENSE`

 * *Files identical despite different names*

