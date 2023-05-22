# Comparing `tmp/ramqp-8.3.1.tar.gz` & `tmp/ramqp-8.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ramqp-8.3.1.tar", max compression
+gzip compressed data, was "ramqp-8.4.0.tar", max compression
```

## Comparing `ramqp-8.3.1.tar` & `ramqp-8.4.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0        0        0        0 2023-05-17 13:06:54.569245 ramqp-8.3.1/LICENSES/
--rw-r--r--   0        0        0    15177 2023-05-17 13:06:54.569245 ramqp-8.3.1/LICENSES/MPL-2.0.txt
--rw-r--r--   0        0        0     7466 2023-05-17 13:06:54.569245 ramqp-8.3.1/README.md
--rw-r--r--   0        0        0     1460 2023-05-17 13:07:10.359384 ramqp-8.3.1/pyproject.toml
--rw-r--r--   0        0        0      321 2023-05-17 13:06:54.571245 ramqp-8.3.1/ramqp/__init__.py
--rw-r--r--   0        0        0    13047 2023-05-17 13:06:54.571245 ramqp-8.3.1/ramqp/abstract.py
--rw-r--r--   0        0        0      668 2023-05-17 13:06:54.571245 ramqp-8.3.1/ramqp/amqp.py
--rw-r--r--   0        0        0     2729 2023-05-17 13:06:54.571245 ramqp-8.3.1/ramqp/config.py
--rw-r--r--   0        0        0    10021 2023-05-17 13:06:54.571245 ramqp-8.3.1/ramqp/depends.py
--rw-r--r--   0        0        0     7010 2023-05-17 13:06:54.572245 ramqp-8.3.1/ramqp/metrics.py
--rw-r--r--   0        0        0     8652 2023-05-17 13:06:54.572245 ramqp-8.3.1/ramqp/mo.py
--rw-r--r--   0        0        0        0 2023-05-17 13:06:54.696254 ramqp-8.3.1/ramqp/py.typed
--rw-r--r--   0        0        0     1367 2023-05-17 13:06:54.572245 ramqp-8.3.1/ramqp/utils.py
--rw-r--r--   0        0        0     8361 1970-01-01 00:00:00.000000 ramqp-8.3.1/PKG-INFO
+drwxr-xr-x   0        0        0        0 2023-05-22 14:48:16.191417 ramqp-8.4.0/LICENSES/
+-rw-r--r--   0        0        0    15177 2023-05-22 14:48:16.191417 ramqp-8.4.0/LICENSES/MPL-2.0.txt
+-rw-r--r--   0        0        0     7466 2023-05-22 14:48:16.192417 ramqp-8.4.0/README.md
+-rw-r--r--   0        0        0     1460 2023-05-22 14:48:28.848330 ramqp-8.4.0/pyproject.toml
+-rw-r--r--   0        0        0      321 2023-05-22 14:48:16.194417 ramqp-8.4.0/ramqp/__init__.py
+-rw-r--r--   0        0        0    16392 2023-05-22 14:48:16.194417 ramqp-8.4.0/ramqp/abstract.py
+-rw-r--r--   0        0        0      668 2023-05-22 14:48:16.194417 ramqp-8.4.0/ramqp/amqp.py
+-rw-r--r--   0        0        0     2729 2023-05-22 14:48:16.194417 ramqp-8.4.0/ramqp/config.py
+-rw-r--r--   0        0        0    10021 2023-05-22 14:48:16.195417 ramqp-8.4.0/ramqp/depends.py
+-rw-r--r--   0        0        0     7010 2023-05-22 14:48:16.195417 ramqp-8.4.0/ramqp/metrics.py
+-rw-r--r--   0        0        0     8652 2023-05-22 14:48:16.195417 ramqp-8.4.0/ramqp/mo.py
+-rw-r--r--   0        0        0        0 2023-05-22 14:48:16.253421 ramqp-8.4.0/ramqp/py.typed
+-rw-r--r--   0        0        0     1367 2023-05-22 14:48:16.196417 ramqp-8.4.0/ramqp/utils.py
+-rw-r--r--   0        0        0     8361 1970-01-01 00:00:00.000000 ramqp-8.4.0/PKG-INFO
```

### Comparing `ramqp-8.3.1/LICENSES/MPL-2.0.txt` & `ramqp-8.4.0/LICENSES/MPL-2.0.txt`

 * *Files identical despite different names*

### Comparing `ramqp-8.3.1/README.md` & `ramqp-8.4.0/README.md`

 * *Files identical despite different names*

### Comparing `ramqp-8.3.1/pyproject.toml` & `ramqp-8.4.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ramqp"
-version = "8.3.1"
+version = "8.4.0"
 description = "Rammearkitektur AMQP library (aio_pika wrapper)"
 authors = ["Magenta ApS <info@magenta.dk>"]
 license = "MPL-2.0"
 readme = "README.md"
 homepage = "https://magenta.dk/"
 repository = "https://git.magenta.dk/rammearkitektur/ramqp"
 keywords = ["os2mo", "amqp"]
```

### Comparing `ramqp-8.3.1/ramqp/abstract.py` & `ramqp-8.4.0/ramqp/abstract.py`

 * *Files 14% similar despite different names*

```diff
@@ -22,15 +22,17 @@
 from aio_pika import ExchangeType
 from aio_pika import IncomingMessage
 from aio_pika import Message
 from aio_pika.abc import AbstractExchange
 from aio_pika.abc import AbstractQueue
 from aio_pika.abc import AbstractRobustChannel
 from aio_pika.abc import AbstractRobustConnection
+from aiormq import ChannelPreconditionFailed
 from more_itertools import all_unique
+from more_itertools import one
 
 from .config import AMQPConnectionSettings
 from .depends import dependency_injected
 from .metrics import _handle_publish_metrics
 from .metrics import _handle_receive_metrics
 from .metrics import _setup_channel_metrics
 from .metrics import _setup_connection_metrics
@@ -38,15 +40,14 @@
 from .metrics import callbacks_registered
 from .metrics import routes_bound
 from .utils import CallbackType
 from .utils import function_to_name
 from .utils import RejectMessage
 from .utils import RequeueMessage
 
-
 logger = structlog.get_logger()
 
 
 class AbstractRouter:
     """Abstract base-class for Routers.
 
     Shared code used by both Router and MORouter.
@@ -251,20 +252,82 @@
             settings.exchange, ExchangeType.TOPIC, durable=True
         )
 
         # TODO: Create queues and binds in parallel?
         self._queues = {}
         for callback, routing_keys in self.router.registry.items():
             function_name = function_to_name(callback)
-            log = logger.bind(function=function_name)
-
             queue_name = f"{settings.queue_prefix}_{function_name}"
-            log.info("Declaring unique message queue", queue_name=queue_name)
-            # Make our queues durable so they survive broker restarts
-            queue = await self._channel.declare_queue(queue_name, durable=True)
+            log = logger.bind(queue=queue_name)
+
+            log.info("Declaring unique message queue")
+            # Make our queue quorum, so it survives broker restarts, and so that
+            # messages that are rejected or nacked will be returned to the _back_ of
+            # the queue. This allows us to consume as many messages as possible,
+            # instead of blocking on the first unprocessable one.
+            # NOTE: If a delivery-limit is set, the queue will use the original
+            # behaviour of returning the message near the head of the queue.
+            # https://www.rabbitmq.com/quorum-queues.html#repeated-requeues
+
+            # TODO: BEGIN quorum migration
+            async def ensure_quorum() -> bool:
+                """Attempt to allow migration to a quorum queue.
+
+                Returns: True, if the queue is already, or can be, migrated to
+                         (declared as) a quorum queue. False otherwise.
+                """
+                # pylint: disable=cell-var-from-loop
+                assert self._connection is not None
+                try:
+                    # Try to declare the queue as quorum. The call uses a temporary
+                    # channel since it will be closed on ChannelPreconditionFailed.
+                    async with self._connection.channel() as temporary_channel:
+                        await temporary_channel.declare_queue(
+                            queue_name,
+                            durable=True,
+                            arguments={
+                                "x-queue-type": "quorum",
+                            },
+                        )
+                    # If that worked, the queue is already migrated
+                    return True
+                except ChannelPreconditionFailed as error:
+                    # If we cannot declare the queue as quorum, it's probably because
+                    # it already exists as a non-quorum classical queue.
+                    assert "inequivalent arg 'x-queue-type'" in one(error.args)
+                    # If so -- and it's empty -- try to delete it
+                    try:
+                        log.warning("Quorum migration: Deleting existing classic queue")
+                        async with self._connection.channel() as temporary_channel:
+                            q = await temporary_channel.get_queue(
+                                queue_name, ensure=True
+                            )
+                            await q.delete(if_empty=True)
+                            # If that worked, the queue can be declared as quorum
+                            return True
+                    except ChannelPreconditionFailed:
+                        # If we are unable to delete the existing queue, there's nothing
+                        # we can do. Let the caller know they should use a classic queue
+                        # for now.
+                        log.warning("Unable to delete queue (probably non-empty)")
+                        return False
+
+            if not await ensure_quorum():
+                queue = await self._channel.declare_queue(queue_name, durable=True)
+            else:
+                # TODO: END quorum migration
+                # This is the code that would remain after the migration period
+                queue = await self._channel.declare_queue(
+                    queue_name,
+                    durable=True,
+                    arguments={
+                        "x-queue-type": "quorum",
+                    },
+                )
+
             self._queues[function_name] = queue
 
             log.info("Starting message listener")
             await queue.consume(partial(self._on_message, callback))
 
             log.info("Binding routing keys")
             for routing_key in routing_keys:
```

### Comparing `ramqp-8.3.1/ramqp/amqp.py` & `ramqp-8.4.0/ramqp/amqp.py`

 * *Files identical despite different names*

### Comparing `ramqp-8.3.1/ramqp/config.py` & `ramqp-8.4.0/ramqp/config.py`

 * *Files identical despite different names*

### Comparing `ramqp-8.3.1/ramqp/depends.py` & `ramqp-8.4.0/ramqp/depends.py`

 * *Files identical despite different names*

### Comparing `ramqp-8.3.1/ramqp/metrics.py` & `ramqp-8.4.0/ramqp/metrics.py`

 * *Files identical despite different names*

### Comparing `ramqp-8.3.1/ramqp/mo.py` & `ramqp-8.4.0/ramqp/mo.py`

 * *Files identical despite different names*

### Comparing `ramqp-8.3.1/ramqp/utils.py` & `ramqp-8.4.0/ramqp/utils.py`

 * *Files identical despite different names*

### Comparing `ramqp-8.3.1/PKG-INFO` & `ramqp-8.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ramqp
-Version: 8.3.1
+Version: 8.4.0
 Summary: Rammearkitektur AMQP library (aio_pika wrapper)
 Home-page: https://magenta.dk/
 License: MPL-2.0
 Keywords: os2mo,amqp
 Author: Magenta ApS
 Author-email: info@magenta.dk
 Requires-Python: >=3.10,<4.0
```

