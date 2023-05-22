# Comparing `tmp/is_wire-1.2.0.tar.gz` & `tmp/is_wire-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/is_wire-1.2.0.tar", last modified: Fri May 24 21:22:01 2019, max compression
+gzip compressed data, was "is_wire-1.2.1.tar", last modified: Mon May 22 16:05:05 2023, max compression
```

## Comparing `is_wire-1.2.0.tar` & `is_wire-1.2.1.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-05-24 21:22:01.000000 is_wire-1.2.0/
--rw-rw-r--   0 travis    (2000) travis    (2000)     6120 2019-05-24 21:21:26.000000 is_wire-1.2.0/README.md
--rw-rw-r--   0 travis    (2000) travis    (2000)      486 2019-05-24 21:21:26.000000 is_wire-1.2.0/setup.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       38 2019-05-24 21:22:01.000000 is_wire-1.2.0/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)      208 2019-05-24 21:22:01.000000 is_wire-1.2.0/PKG-INFO
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-05-24 21:22:01.000000 is_wire-1.2.0/src/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-05-24 21:22:01.000000 is_wire-1.2.0/src/is_wire/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-05-24 21:21:26.000000 is_wire-1.2.0/src/is_wire/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-05-24 21:22:01.000000 is_wire-1.2.0/src/is_wire/core/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1958 2019-05-24 21:21:26.000000 is_wire-1.2.0/src/is_wire/core/subscription.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      631 2019-05-24 21:21:26.000000 is_wire-1.2.0/src/is_wire/core/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2662 2019-05-24 21:21:26.000000 is_wire-1.2.0/src/is_wire/core/channel.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1677 2019-05-24 21:21:26.000000 is_wire-1.2.0/src/is_wire/core/logger.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-05-24 21:22:01.000000 is_wire-1.2.0/src/is_wire/core/wire/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1278 2019-05-24 21:21:26.000000 is_wire-1.2.0/src/is_wire/core/wire/content_type.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-05-24 21:21:26.000000 is_wire-1.2.0/src/is_wire/core/wire/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1738 2019-05-24 21:21:26.000000 is_wire-1.2.0/src/is_wire/core/wire/status.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    10928 2019-05-24 21:21:26.000000 is_wire-1.2.0/src/is_wire/core/wire/wire_pb2.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3051 2019-05-24 21:21:26.000000 is_wire-1.2.0/src/is_wire/core/wire/conversion.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    12354 2019-05-24 21:21:26.000000 is_wire-1.2.0/src/is_wire/core/message.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      855 2019-05-24 21:21:26.000000 is_wire-1.2.0/src/is_wire/core/utils.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-05-24 21:22:01.000000 is_wire-1.2.0/src/is_wire/core/tracing/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1039 2019-05-24 21:21:26.000000 is_wire-1.2.0/src/is_wire/core/tracing/tracer.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-05-24 21:21:26.000000 is_wire-1.2.0/src/is_wire/core/tracing/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1605 2019-05-24 21:21:26.000000 is_wire-1.2.0/src/is_wire/core/tracing/propagation.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-05-24 21:22:01.000000 is_wire-1.2.0/src/is_wire/rpc/
--rw-rw-r--   0 travis    (2000) travis    (2000)     5176 2019-05-24 21:21:26.000000 is_wire-1.2.0/src/is_wire/rpc/service_provider.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      939 2019-05-24 21:21:26.000000 is_wire-1.2.0/src/is_wire/rpc/metrics_interceptor.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1372 2019-05-24 21:21:26.000000 is_wire-1.2.0/src/is_wire/rpc/tracing_interceptor.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      125 2019-05-24 21:21:26.000000 is_wire-1.2.0/src/is_wire/rpc/interceptor.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      416 2019-05-24 21:21:26.000000 is_wire-1.2.0/src/is_wire/rpc/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      783 2019-05-24 21:21:26.000000 is_wire-1.2.0/src/is_wire/rpc/log_interceptor.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      344 2019-05-24 21:21:26.000000 is_wire-1.2.0/src/is_wire/rpc/context.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-05-24 21:22:01.000000 is_wire-1.2.0/src/is_wire.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)        8 2019-05-24 21:22:01.000000 is_wire-1.2.0/src/is_wire.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2019-05-24 21:22:01.000000 is_wire-1.2.0/src/is_wire.egg-info/not-zip-safe
--rw-rw-r--   0 travis    (2000) travis    (2000)      101 2019-05-24 21:22:01.000000 is_wire-1.2.0/src/is_wire.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      208 2019-05-24 21:22:01.000000 is_wire-1.2.0/src/is_wire.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2019-05-24 21:22:01.000000 is_wire-1.2.0/src/is_wire.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      942 2019-05-24 21:22:01.000000 is_wire-1.2.0/src/is_wire.egg-info/SOURCES.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:05:05.188951 is_wire-1.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     8451 2023-05-22 16:05:05.188951 is_wire-1.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7833 2023-05-22 16:04:51.000000 is_wire-1.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-05-22 16:05:05.188951 is_wire-1.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-05-22 16:04:51.000000 is_wire-1.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:05:05.184950 is_wire-1.2.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:05:05.184950 is_wire-1.2.1/src/is_wire/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 16:04:51.000000 is_wire-1.2.1/src/is_wire/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:05:05.184950 is_wire-1.2.1/src/is_wire/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-05-22 16:04:51.000000 is_wire-1.2.1/src/is_wire/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-05-22 16:04:51.000000 is_wire-1.2.1/src/is_wire/core/channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-05-22 16:04:51.000000 is_wire-1.2.1/src/is_wire/core/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12479 2023-05-22 16:04:51.000000 is_wire-1.2.1/src/is_wire/core/message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-05-22 16:04:51.000000 is_wire-1.2.1/src/is_wire/core/subscription.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:05:05.184950 is_wire-1.2.1/src/is_wire/core/tracing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 16:04:51.000000 is_wire-1.2.1/src/is_wire/core/tracing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-05-22 16:04:51.000000 is_wire-1.2.1/src/is_wire/core/tracing/propagation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-05-22 16:04:51.000000 is_wire-1.2.1/src/is_wire/core/tracing/tracer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-05-22 16:04:51.000000 is_wire-1.2.1/src/is_wire/core/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:05:05.184950 is_wire-1.2.1/src/is_wire/core/wire/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 16:04:51.000000 is_wire-1.2.1/src/is_wire/core/wire/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-05-22 16:04:51.000000 is_wire-1.2.1/src/is_wire/core/wire/content_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3052 2023-05-22 16:04:51.000000 is_wire-1.2.1/src/is_wire/core/wire/conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1739 2023-05-22 16:04:51.000000 is_wire-1.2.1/src/is_wire/core/wire/status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2461 2023-05-22 16:04:51.000000 is_wire-1.2.1/src/is_wire/core/wire/wire_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:05:05.188951 is_wire-1.2.1/src/is_wire/rpc/
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-05-22 16:04:51.000000 is_wire-1.2.1/src/is_wire/rpc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-05-22 16:04:51.000000 is_wire-1.2.1/src/is_wire/rpc/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-22 16:04:51.000000 is_wire-1.2.1/src/is_wire/rpc/interceptor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-05-22 16:04:51.000000 is_wire-1.2.1/src/is_wire/rpc/log_interceptor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-05-22 16:04:51.000000 is_wire-1.2.1/src/is_wire/rpc/metrics_interceptor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5207 2023-05-22 16:04:51.000000 is_wire-1.2.1/src/is_wire/rpc/service_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-05-22 16:04:51.000000 is_wire-1.2.1/src/is_wire/rpc/tracing_interceptor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:05:05.184950 is_wire-1.2.1/src/is_wire.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8451 2023-05-22 16:05:05.000000 is_wire-1.2.1/src/is_wire.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-05-22 16:05:05.000000 is_wire-1.2.1/src/is_wire.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 16:05:05.000000 is_wire-1.2.1/src/is_wire.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 16:05:05.000000 is_wire-1.2.1/src/is_wire.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-22 16:05:05.000000 is_wire-1.2.1/src/is_wire.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-22 16:05:05.000000 is_wire-1.2.1/src/is_wire.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `is_wire-1.2.0/README.md` & `is_wire-1.2.1/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 
-# Wire
+# is-wire
 
-Pub/Sub middleware for the *is* architecture (python implementation)
+[![PyPI](https://img.shields.io/pypi/v/is-wire.svg?style=for-the-badge)](https://pypi.org/project/is-wire/)
+[![Build](https://img.shields.io/github/actions/workflow/status/labvisio/is-wire-py/main.yml?style=for-the-badge)](https://github.com/labvisio/is-wire-py/actions)
+[![Python suport](https://img.shields.io/pypi/pyversions/is-wire?style=for-the-badge)](https://pypi.org/project/is-wire)
+[![Downloads](https://img.shields.io/pypi/dm/is-wire?style=for-the-badge)](https://pypi.org/project/is-wire/)
 
-![PyPI](https://img.shields.io/pypi/v/is-wire.svg?label=is-wire&style=for-the-badge)
-![Travis](https://img.shields.io/travis/com/labviros/is-wire-py.svg?label=Linux&style=for-the-badge)
-![Appveyor](https://img.shields.io/appveyor/ci/felippe-mendonca/is-wire-py.svg?label=Windows&style=for-the-badge)
+Pub/Sub middleware for the *is* architecture (python implementation)
 
 ## Installation 
 
 Install the wire package using `pip` or `pipenv`:
 
 ```shell
   pip install --user is-wire
@@ -28,15 +29,14 @@
 ```
 
 ### Basic send/receive
 
 Create a channel to connect to a broker, create a subscription and subscribe to desired topics to receive messages:
 
 ```python
-from __future__ import print_function
 from is_wire.core import Channel, Subscription
 
 # Connect to the broker
 channel = Channel("amqp://guest:guest@localhost:5672")
 
 # Subscribe to the desired topic(s)
 subscription = Subscription(channel)
@@ -129,15 +129,14 @@
 
 provider.run() # Blocks forever processing requests
 ```
 
 Send a request to the RPC Server:
 
 ```python
-from __future__ import print_function
 from is_wire.core import Channel, Message, Subscription
 from google.protobuf.struct_pb2 import Struct
 import socket
 
 channel = Channel("amqp://guest:guest@localhost:5672")
 subscription = Subscription(channel)
 
@@ -153,14 +152,56 @@
     reply = channel.consume(timeout=1.0)
     struct = reply.unpack(Struct)
     print('RPC Status:', reply.status, '\nReply:', struct)
 except socket.timeout:
     print('No reply :(')
 ```
 
+Multiples requests can be done throughout same client. To distinguish which reply is related to each request, you can use the `correlation_id`. This attribute is always set when a `Message` is published containing `reply_to` parameter, which means that it was a RPC request. Example below shows how to deal with it.
+
+```python
+from is_wire.core import Channel, Message, Subscription
+from google.protobuf.struct_pb2 import Struct
+import socket
+
+channel = Channel("amqp://guest:guest@localhost:5672")
+subscription = Subscription(channel)
+
+# Prepare first request
+struct = Struct()
+struct.fields["value"].number_value = 1.0
+request_1 = Message(content=struct, reply_to=subscription)
+
+# Prepare second request
+struct = Struct()
+struct.fields["value"].number_value = 2.0
+request_2 = Message(content=struct, reply_to=subscription)
+
+# Make requests
+channel.publish(request_1, topic="MyService.Increment")
+channel.publish(request_2, topic="MyService.Increment")
+
+# Wait for replies with 1.0 seconds timeout
+n_replies = 0
+while n_replies < 2:
+    try:
+        reply = channel.consume(timeout=1.0)
+        struct = reply.unpack(Struct)
+        if reply.correlation_id == request_1.correlation_id:
+            n_replies += 1
+            print('First Request\nRPC Status:', reply.status, '\nReply:', struct)
+        elif reply.correlation_id == request_2.correlation_id:
+            n_replies += 1
+            print('Second Request\nRPC Status:', reply.status, '\nReply:', struct)
+        else:
+            print('Unexpected message')
+    except socket.timeout:
+        print('No reply :(')
+```
+
 ### Tracing messages
 
 This middleware uses [opencensus](https://github.com/census-instrumentation/opencensus-python) as instrumentation library. Latest versions of opencensus released separate packages to integrate with different frameworks and tracing collector tools. When interacting with services implemented with either the C++ or Python of is-wire, we recommend to use [Zipkin](https://zipkin.apache.org/) to collect the tracing data. To do so, use the latest version of [OpenCensus Zipkin Exporter](https://github.com/census-instrumentation/opencensus-python/tree/master/contrib/opencensus-ext-zipkin).
 
 Instantiate an Exporter to trace requests:
 
 ```python
```

### Comparing `is_wire-1.2.0/src/is_wire/core/subscription.py` & `is_wire-1.2.1/src/is_wire/core/subscription.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from .utils import consumer_id
 
 
 class Subscription(object):
+
     def __init__(self, channel, name=None):
         self._id = consumer_id()
         self._name = self._id if name is None else name
         self._topics = set()
 
         self._channel = channel._channel
         self._exchange = channel._exchange
```

### Comparing `is_wire-1.2.0/src/is_wire/core/__init__.py` & `is_wire-1.2.1/src/is_wire/core/__init__.py`

 * *Files identical despite different names*

### Comparing `is_wire-1.2.0/src/is_wire/core/channel.py` & `is_wire-1.2.1/src/is_wire/core/channel.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import amqp
 from six.moves import urllib
 from .wire.conversion import WireV1
 
 
 class Channel(object):
+
     def __init__(self, uri="amqp://guest:guest@localhost:5672", exchange="is"):
         url = urllib.parse.urlparse(uri)
 
         self.connection = amqp.Connection(
             host="{}:{}".format(url.hostname or "localhost", url.port or 5672),
             userid=url.username or "guest",
             password=url.password or "guest",
```

### Comparing `is_wire-1.2.0/src/is_wire/core/logger.py` & `is_wire-1.2.1/src/is_wire/core/logger.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,15 +25,16 @@
                 'DEBUG': 'cyan',
                 'INFO': 'white',
                 'WARNING': 'yellow',
                 'ERROR': 'red',
                 'CRITICAL': 'white,bg_red',
             },
             secondary_log_colors={},
-            style='%')
+            style='%',
+        )
 
         self.logger = getLogger(name)
         if len(self.logger.handlers) == 0 and name:
             handler = StreamHandler()
             handler.setFormatter(formatter)
             self.logger.addHandler(handler)
             self.set_level(level)
```

### Comparing `is_wire-1.2.0/src/is_wire/core/wire/content_type.py` & `is_wire-1.2.1/src/is_wire/core/wire/content_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,16 @@
 
 class ContentType(Enum):
     PROTOBUF = wire_pb2.ContentType.Value("PROTOBUF")
     JSON = wire_pb2.ContentType.Value("JSON")
 
 
 def content_type_to_wire(content_type):
-    """ Converts an object of type ContentType to the wire string representation.
+    """ Converts an object of type ContentType to the wire string
+    representation.
     Args:
         content_type (ContentType): enum value
     Returns:
         str: wire string representation
     """
     assert_type(content_type, ContentType, "content_type")
     if content_type == ContentType.PROTOBUF:
```

### Comparing `is_wire-1.2.0/src/is_wire/core/wire/status.py` & `is_wire-1.2.1/src/is_wire/core/wire/status.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,14 +17,15 @@
     FAILED_PRECONDITION = wire_pb2.StatusCode.Value('FAILED_PRECONDITION')
     OUT_OF_RANGE = wire_pb2.StatusCode.Value('OUT_OF_RANGE')
     UNIMPLEMENTED = wire_pb2.StatusCode.Value('UNIMPLEMENTED')
     INTERNAL_ERROR = wire_pb2.StatusCode.Value('INTERNAL_ERROR')
 
 
 class Status(object):
+
     def __init__(self, code=StatusCode.UNKNOWN, why=""):
         self._code = None
         self._why = None
         self.code = code
         self.why = why
 
     def __eq__(self, other):
```

### Comparing `is_wire-1.2.0/src/is_wire/core/wire/conversion.py` & `is_wire-1.2.1/src/is_wire/core/wire/conversion.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from .status import Status, StatusCode
 from . import wire_pb2
 from google.protobuf import json_format
 from six import binary_type
 
 
 class WireV1(object):
+
     @staticmethod
     def from_amqp_message(amqp_message):
         message = Message()
 
         if not isinstance(amqp_message.body, binary_type):
             message.body = amqp_message.body.encode('latin')
         else:
```

### Comparing `is_wire-1.2.0/src/is_wire/core/message.py` & `is_wire-1.2.1/src/is_wire/core/message.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from .subscription import Subscription
 from .wire.status import Status
 from .wire.content_type import ContentType
 from .tracing.propagation import TextFormatPropagator
 
 
 class Message(object):
+
     def __init__(self, content=None, reply_to=None, content_type=None):
         """ Creates a new message.
         Args:
             content (str or object): sets the message body with the
             given content. If an object is provided, it will be packed
             using the given content_type.
 
@@ -160,16 +161,16 @@
 
     @subscription_id.setter
     def subscription_id(self, value):
         assert_type(value, string_types, "subscription_id")
         self._subscription_id = value
 
     def has_subscription_id(self):
-        """ Returns: True if the property subscription_id of the message is set,
-         False otherwise """
+        """ Returns: True if the property subscription_id of the message is
+        set, False otherwise """
         return bool(self._subscription_id)
 
     # correlation_id
 
     @property
     def correlation_id(self):
         """ int: Unique ID used to correlate reply/response messages """
@@ -321,23 +322,27 @@
 
         if isDict:
             obj = pb.ParseDict(obj, Struct())
 
         if not self.has_content_type():
             # Default for dict object is to be serialized as json
             # Default for protobuf object is to be binary serialized
-            self.content_type = ContentType.JSON if isDict else ContentType.PROTOBUF
+            if isDict:
+                self.content_type = ContentType.JSON
+            else:
+                self.content_type = ContentType.PROTOBUF
 
         if self.content_type == ContentType.PROTOBUF:
             # SerializeToString returns py2: str, py3: bytes
             self.body = obj.SerializeToString()
         elif self.content_type == ContentType.JSON:
             # MessageToJson returns py2: str, py3: str
-            packed = pb.MessageToJson(
-                obj, indent=0, including_default_value_fields=True)
+            packed = pb.MessageToJson(obj,
+                                      indent=0,
+                                      including_default_value_fields=True)
             if not isinstance(packed, binary_type):
                 self.body = packed.encode('latin')
             else:
                 self.body = packed
         else:
             raise NotImplementedError(
                 "Serialization to '{}' type not implemented".format(
```

### Comparing `is_wire-1.2.0/src/is_wire/core/utils.py` & `is_wire-1.2.1/src/is_wire/core/utils.py`

 * *Files identical despite different names*

### Comparing `is_wire-1.2.0/src/is_wire/core/tracing/tracer.py` & `is_wire-1.2.1/src/is_wire/core/tracing/tracer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 from opencensus.trace import tracer
 from opencensus.trace.span_context import SpanContext
 
 # Patch opencensus to allow 64 bit trace ids.
 import opencensus.trace.span_context
 import re
+
 opencensus.trace.span_context.TRACE_ID_PATTERN = re.compile('[0-9a-f]{16}?')
 opencensus.trace.span_context._INVALID_TRACE_ID = '0' * 16
 # Function 'generate_trace_id' is overwritted with 'generate_span_id'
 # because this function generates a ID with 64 bits.
 opencensus.trace.span_context.generate_trace_id = \
     opencensus.trace.span_context.generate_span_id
 
 
 class Tracer(object):
+
     def __init__(self, exporter=None, span_context=None):
         if span_context is None:
             span_context = SpanContext()
 
         self.tracer = tracer.Tracer(
             exporter=exporter,
             span_context=span_context,
```

### Comparing `is_wire-1.2.0/src/is_wire/core/tracing/propagation.py` & `is_wire-1.2.1/src/is_wire/core/tracing/propagation.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from opencensus.trace.span_context import SpanContext
 from ..utils import assert_type
 
 # Patch opencensus to allow 64 bit trace ids
 import opencensus.trace.span_context
 import re
+
 opencensus.trace.span_context.TRACE_ID_PATTERN = re.compile('[0-9a-f]{16}?')
 opencensus.trace.span_context._INVALID_TRACE_ID = '0' * 16
 
 
 class TextFormatPropagator(object):
     trace_prefix = 'x-b3'
     trace_id_key = '{}-traceid'.format(trace_prefix)
```

### Comparing `is_wire-1.2.0/src/is_wire/rpc/service_provider.py` & `is_wire-1.2.1/src/is_wire/rpc/service_provider.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,14 +67,15 @@
     def run(self):
         """ Blocks the current thread listening for requests """
         self.log.info("Listening for requests")
         while True:
             self.serve(self._channel.consume())
 
     def wrap(self, function, request_type, reply_type):
+
         def safe_call(*args):
             try:
                 result = function(*args)
                 assert_type(result, (Status, reply_type), "function result")
                 return result
             except Exception:
                 return Status(
@@ -103,15 +104,16 @@
                     result = safe_call(arg, context)
                     if isinstance(result, Status):
                         reply.status = result
                     else:
                         reply.pack(result)
                         reply.status = Status(code=StatusCode.OK)
                 except ParseError:
-                    why = "Expected request type '{}' but received something else"\
+                    why = "Expected request type '{}' but received " \
+                        "something else" \
                         .format(request_type.DESCRIPTOR.full_name)
                     reply.status = Status(StatusCode.FAILED_PRECONDITION, why)
                 except Exception:
                     trace = traceback.format_exc()
                     self.log.error("Unexpected error\n{}", trace)
                     reply.status = Status(StatusCode.INTERNAL_ERROR, trace)
```

### Comparing `is_wire-1.2.0/src/is_wire/rpc/metrics_interceptor.py` & `is_wire-1.2.1/src/is_wire/rpc/metrics_interceptor.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from prometheus_client import start_http_server, Counter
 from ..rpc import Interceptor
 from ..core import Logger
 import time
 
 
 class MetricsInterceptor(Interceptor):
+
     def __init__(self):
         self.log = Logger(name='MetricsInterceptor')
         labels = ("service", "status_code")
         self.duration = Counter("rpc_duration_total",
                                 "How long requests took in seconds", labels)
         self.count = Counter("rpc_count_total",
                              "How many requests were processed", labels)
 
-
     def start_server(self, port=8000):
         start_http_server(port)
 
     def before_call(self, context):
         self.begin = time.time()
 
     def after_call(self, context):
```

### Comparing `is_wire-1.2.0/src/is_wire/rpc/tracing_interceptor.py` & `is_wire-1.2.1/src/is_wire/rpc/tracing_interceptor.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,30 +3,31 @@
 
 
 def service_name(context):
     return context.request.topic.split(".")[-1]
 
 
 class TracingInterceptor(Interceptor):
+
     def __init__(self, exporter, span_namer=service_name):
         """ Construct a TracingInterceptor to automatically trace requests
         of a ServiceProvider.
         Args:
             exporter (opencensus.Exporter): object responsible for exporting
             spans to a tracer.
             span_namer (function: Context -> str): function responsible
             for generating the name of the request span.
         """
         self.log = Logger(name='TracingInterceptor')
         self.exporter = exporter
         self.namer = span_namer
 
     def before_call(self, context):
-        self.tracer = Tracer(
-            self.exporter, span_context=context.request.extract_tracing())
+        self.tracer = Tracer(self.exporter,
+                             span_context=context.request.extract_tracing())
         context.addons["tracer"] = self.tracer
         self.span = self.tracer.start_span(name=self.namer(context))
 
     def after_call(self, context):
         status = context.reply.status
         if not status.ok():
             self.span.add_attribute("reply_to", context.request.reply_to)
```

### Comparing `is_wire-1.2.0/src/is_wire/rpc/log_interceptor.py` & `is_wire-1.2.1/src/is_wire/rpc/log_interceptor.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from ..core import Logger, now, StatusCode
 from ..rpc import Interceptor
 
 
 class LogInterceptor(Interceptor):
+
     def __init__(self):
         self.log = Logger(name='LogInterceptor')
 
     def before_call(self, context):
         self.begin = now()
 
     def after_call(self, context):
```

### Comparing `is_wire-1.2.0/src/is_wire.egg-info/SOURCES.txt` & `is_wire-1.2.1/src/is_wire.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 README.md
+setup.cfg
 setup.py
 src/is_wire/__init__.py
 src/is_wire.egg-info/PKG-INFO
 src/is_wire.egg-info/SOURCES.txt
 src/is_wire.egg-info/dependency_links.txt
 src/is_wire.egg-info/not-zip-safe
 src/is_wire.egg-info/requires.txt
```

