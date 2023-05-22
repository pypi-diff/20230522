# Comparing `tmp/rabbie-0.0.8.tar.gz` & `tmp/rabbie-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rabbie-0.0.8.tar", last modified: Thu May 18 08:08:04 2023, max compression
+gzip compressed data, was "rabbie-0.0.9.tar", last modified: Mon May 22 16:23:39 2023, max compression
```

## Comparing `rabbie-0.0.8.tar` & `rabbie-0.0.9.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxrwxrwx   0        0        0        0 2023-05-18 08:08:04.255935 rabbie-0.0.8/
--rw-rw-rw-   0        0        0     1077 2023-04-24 20:01:12.000000 rabbie-0.0.8/LICENSE
--rw-rw-rw-   0        0        0     9287 2023-05-18 08:08:04.254938 rabbie-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     8813 2023-05-18 08:05:34.000000 rabbie-0.0.8/README.md
--rw-rw-rw-   0        0        0       63 2023-04-02 21:06:34.000000 rabbie-0.0.8/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-05-18 08:08:04.196422 rabbie-0.0.8/rabbie/
--rw-rw-rw-   0        0        0      265 2023-05-18 08:05:34.000000 rabbie-0.0.8/rabbie/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-18 08:08:04.212937 rabbie-0.0.8/rabbie/broker_types/
--rw-rw-rw-   0        0        0       60 2023-05-11 11:17:49.000000 rabbie-0.0.8/rabbie/broker_types/__init__.py
--rw-rw-rw-   0        0        0     4898 2023-05-11 11:34:26.000000 rabbie-0.0.8/rabbie/broker_types/channel.py
--rw-rw-rw-   0        0        0      182 2023-05-11 11:17:49.000000 rabbie-0.0.8/rabbie/broker_types/relayed_types.py
-drwxrwxrwx   0        0        0        0 2023-05-18 08:08:04.214933 rabbie-0.0.8/rabbie/connection/
--rw-rw-rw-   0        0        0       44 2023-05-11 11:17:49.000000 rabbie-0.0.8/rabbie/connection/__init__.py
--rw-rw-rw-   0        0        0      294 2023-05-11 11:17:49.000000 rabbie-0.0.8/rabbie/connection/details.py
-drwxrwxrwx   0        0        0        0 2023-05-18 08:08:04.217934 rabbie-0.0.8/rabbie/consumer/
--rw-rw-rw-   0        0        0      175 2023-05-11 11:17:49.000000 rabbie-0.0.8/rabbie/consumer/__init__.py
--rw-rw-rw-   0        0        0     9107 2023-05-18 08:05:34.000000 rabbie-0.0.8/rabbie/consumer/consumer.py
-drwxrwxrwx   0        0        0        0 2023-05-18 08:08:04.221933 rabbie-0.0.8/rabbie/consumer/listener/
--rw-rw-rw-   0        0        0      116 2023-05-18 08:05:34.000000 rabbie-0.0.8/rabbie/consumer/listener/__init__.py
--rw-rw-rw-   0        0        0     7620 2023-05-18 08:05:34.000000 rabbie-0.0.8/rabbie/consumer/listener/listener.py
--rw-rw-rw-   0        0        0      725 2023-05-18 08:05:34.000000 rabbie-0.0.8/rabbie/consumer/listener/listener_details.py
--rw-rw-rw-   0        0        0      124 2023-05-18 08:05:34.000000 rabbie-0.0.8/rabbie/consumer/listener/listener_status.py
--rw-rw-rw-   0        0        0     4150 2023-05-18 08:05:34.000000 rabbie-0.0.8/rabbie/consumer/microconsumer.py
-drwxrwxrwx   0        0        0        0 2023-05-18 08:08:04.223935 rabbie-0.0.8/rabbie/decoder/
--rw-rw-rw-   0        0        0       78 2023-05-11 11:17:49.000000 rabbie-0.0.8/rabbie/decoder/__init__.py
--rw-rw-rw-   0        0        0      132 2023-04-24 20:01:12.000000 rabbie-0.0.8/rabbie/decoder/decoder.py
-drwxrwxrwx   0        0        0        0 2023-05-18 08:08:04.226933 rabbie-0.0.8/rabbie/decoder/decoders/
--rw-rw-rw-   0        0        0       78 2023-05-11 11:17:49.000000 rabbie-0.0.8/rabbie/decoder/decoders/__init__.py
--rw-rw-rw-   0        0        0      219 2023-05-11 11:17:49.000000 rabbie-0.0.8/rabbie/decoder/decoders/auto_decoder.py
--rw-rw-rw-   0        0        0      148 2023-04-24 20:01:12.000000 rabbie-0.0.8/rabbie/decoder/decoders/json_decoder.py
-drwxrwxrwx   0        0        0        0 2023-05-18 08:08:04.229934 rabbie-0.0.8/rabbie/decoder/exceptions/
--rw-rw-rw-   0        0        0       94 2023-03-29 12:21:12.000000 rabbie-0.0.8/rabbie/decoder/exceptions/__init__.py
--rw-rw-rw-   0        0        0       44 2023-03-29 12:19:53.000000 rabbie-0.0.8/rabbie/decoder/exceptions/decode_exception.py
-drwxrwxrwx   0        0        0        0 2023-05-18 08:08:04.231935 rabbie-0.0.8/rabbie/encoder/
--rw-rw-rw-   0        0        0       78 2023-05-11 11:17:49.000000 rabbie-0.0.8/rabbie/encoder/__init__.py
--rw-rw-rw-   0        0        0      197 2023-05-11 11:17:49.000000 rabbie-0.0.8/rabbie/encoder/encoder.py
-drwxrwxrwx   0        0        0        0 2023-05-18 08:08:04.234936 rabbie-0.0.8/rabbie/encoder/encoders/
--rw-rw-rw-   0        0        0       78 2023-05-11 11:17:49.000000 rabbie-0.0.8/rabbie/encoder/encoders/__init__.py
--rw-rw-rw-   0        0        0      461 2023-05-11 11:17:49.000000 rabbie-0.0.8/rabbie/encoder/encoders/auto_encoder.py
--rw-rw-rw-   0        0        0      215 2023-05-11 11:17:49.000000 rabbie-0.0.8/rabbie/encoder/encoders/json_encoder.py
-drwxrwxrwx   0        0        0        0 2023-05-18 08:08:04.237934 rabbie-0.0.8/rabbie/events/
--rw-rw-rw-   0        0        0       53 2023-05-18 08:05:34.000000 rabbie-0.0.8/rabbie/events/__init__.py
--rw-rw-rw-   0        0        0     1274 2023-05-18 08:05:34.000000 rabbie-0.0.8/rabbie/events/event.py
-drwxrwxrwx   0        0        0        0 2023-05-18 08:08:04.239933 rabbie-0.0.8/rabbie/logger/
--rw-rw-rw-   0        0        0      631 2023-05-18 08:05:34.000000 rabbie-0.0.8/rabbie/logger/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-18 08:08:04.241933 rabbie-0.0.8/rabbie/producer/
--rw-rw-rw-   0        0        0       46 2023-05-11 11:17:49.000000 rabbie-0.0.8/rabbie/producer/__init__.py
--rw-rw-rw-   0        0        0     4584 2023-05-11 11:17:49.000000 rabbie-0.0.8/rabbie/producer/producer.py
-drwxrwxrwx   0        0        0        0 2023-05-18 08:08:04.244935 rabbie-0.0.8/rabbie/producer/publisher/
--rw-rw-rw-   0        0        0       34 2023-05-11 11:17:49.000000 rabbie-0.0.8/rabbie/producer/publisher/__init__.py
--rw-rw-rw-   0        0        0     3176 2023-05-11 11:17:49.000000 rabbie-0.0.8/rabbie/producer/publisher/publisher.py
-drwxrwxrwx   0        0        0        0 2023-05-18 08:08:04.247934 rabbie-0.0.8/rabbie/supervisor/
--rw-rw-rw-   0        0        0       50 2023-04-24 20:01:12.000000 rabbie-0.0.8/rabbie/supervisor/__init__.py
--rw-rw-rw-   0        0        0     4560 2023-04-24 20:01:12.000000 rabbie-0.0.8/rabbie/supervisor/supervisor.py
-drwxrwxrwx   0        0        0        0 2023-05-18 08:08:04.209933 rabbie-0.0.8/rabbie.egg-info/
--rw-rw-rw-   0        0        0     9287 2023-05-18 08:08:04.000000 rabbie-0.0.8/rabbie.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1431 2023-05-18 08:08:04.000000 rabbie-0.0.8/rabbie.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-18 08:08:04.000000 rabbie-0.0.8/rabbie.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2023-05-18 08:08:04.000000 rabbie-0.0.8/rabbie.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-18 08:08:04.000000 rabbie-0.0.8/rabbie.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-18 08:08:04.255935 rabbie-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0      854 2023-05-18 08:05:34.000000 rabbie-0.0.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-18 08:08:04.253935 rabbie-0.0.8/tests/
--rw-rw-rw-   0        0        0     4962 2023-05-18 08:05:34.000000 rabbie-0.0.8/tests/test_consumer.py
--rw-rw-rw-   0        0        0        0 2023-04-24 20:01:12.000000 rabbie-0.0.8/tests/test_decoder.py
--rw-rw-rw-   0        0        0        0 2023-04-24 20:01:12.000000 rabbie-0.0.8/tests/test_listener.py
--rw-rw-rw-   0        0        0        0 2023-04-24 20:01:12.000000 rabbie-0.0.8/tests/test_microconsumer.py
--rw-rw-rw-   0        0        0        0 2023-05-11 11:17:49.000000 rabbie-0.0.8/tests/test_producer.py
+drwxrwxrwx   0        0        0        0 2023-05-22 16:23:39.337698 rabbie-0.0.9/
+-rw-rw-rw-   0        0        0     1077 2023-04-24 20:01:12.000000 rabbie-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0     9287 2023-05-22 16:23:39.337698 rabbie-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     8813 2023-05-18 08:05:34.000000 rabbie-0.0.9/README.md
+-rw-rw-rw-   0        0        0       63 2023-04-02 21:06:34.000000 rabbie-0.0.9/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-05-22 16:23:39.215991 rabbie-0.0.9/rabbie/
+-rw-rw-rw-   0        0        0      265 2023-05-18 08:05:34.000000 rabbie-0.0.9/rabbie/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-22 16:23:39.239011 rabbie-0.0.9/rabbie/broker_types/
+-rw-rw-rw-   0        0        0       60 2023-05-11 11:17:49.000000 rabbie-0.0.9/rabbie/broker_types/__init__.py
+-rw-rw-rw-   0        0        0     4898 2023-05-11 11:34:26.000000 rabbie-0.0.9/rabbie/broker_types/channel.py
+-rw-rw-rw-   0        0        0      182 2023-05-11 11:17:49.000000 rabbie-0.0.9/rabbie/broker_types/relayed_types.py
+drwxrwxrwx   0        0        0        0 2023-05-22 16:23:39.241011 rabbie-0.0.9/rabbie/connection/
+-rw-rw-rw-   0        0        0       44 2023-05-11 11:17:49.000000 rabbie-0.0.9/rabbie/connection/__init__.py
+-rw-rw-rw-   0        0        0      294 2023-05-11 11:17:49.000000 rabbie-0.0.9/rabbie/connection/details.py
+drwxrwxrwx   0        0        0        0 2023-05-22 16:23:39.245522 rabbie-0.0.9/rabbie/consumer/
+-rw-rw-rw-   0        0        0      175 2023-05-11 11:17:49.000000 rabbie-0.0.9/rabbie/consumer/__init__.py
+-rw-rw-rw-   0        0        0     9107 2023-05-18 08:05:34.000000 rabbie-0.0.9/rabbie/consumer/consumer.py
+drwxrwxrwx   0        0        0        0 2023-05-22 16:23:39.249522 rabbie-0.0.9/rabbie/consumer/listener/
+-rw-rw-rw-   0        0        0      116 2023-05-18 08:05:34.000000 rabbie-0.0.9/rabbie/consumer/listener/__init__.py
+-rw-rw-rw-   0        0        0     7726 2023-05-22 16:23:07.000000 rabbie-0.0.9/rabbie/consumer/listener/listener.py
+-rw-rw-rw-   0        0        0      725 2023-05-18 08:05:34.000000 rabbie-0.0.9/rabbie/consumer/listener/listener_details.py
+-rw-rw-rw-   0        0        0      124 2023-05-18 08:05:34.000000 rabbie-0.0.9/rabbie/consumer/listener/listener_status.py
+-rw-rw-rw-   0        0        0     4150 2023-05-18 08:05:34.000000 rabbie-0.0.9/rabbie/consumer/microconsumer.py
+drwxrwxrwx   0        0        0        0 2023-05-22 16:23:39.251521 rabbie-0.0.9/rabbie/decoder/
+-rw-rw-rw-   0        0        0       78 2023-05-11 11:17:49.000000 rabbie-0.0.9/rabbie/decoder/__init__.py
+-rw-rw-rw-   0        0        0      132 2023-04-24 20:01:12.000000 rabbie-0.0.9/rabbie/decoder/decoder.py
+drwxrwxrwx   0        0        0        0 2023-05-22 16:23:39.255036 rabbie-0.0.9/rabbie/decoder/decoders/
+-rw-rw-rw-   0        0        0       78 2023-05-11 11:17:49.000000 rabbie-0.0.9/rabbie/decoder/decoders/__init__.py
+-rw-rw-rw-   0        0        0      235 2023-05-22 16:23:07.000000 rabbie-0.0.9/rabbie/decoder/decoders/auto_decoder.py
+-rw-rw-rw-   0        0        0      148 2023-04-24 20:01:12.000000 rabbie-0.0.9/rabbie/decoder/decoders/json_decoder.py
+drwxrwxrwx   0        0        0        0 2023-05-22 16:23:39.258036 rabbie-0.0.9/rabbie/decoder/exceptions/
+-rw-rw-rw-   0        0        0       94 2023-03-29 12:21:12.000000 rabbie-0.0.9/rabbie/decoder/exceptions/__init__.py
+-rw-rw-rw-   0        0        0       44 2023-03-29 12:19:53.000000 rabbie-0.0.9/rabbie/decoder/exceptions/decode_exception.py
+drwxrwxrwx   0        0        0        0 2023-05-22 16:23:39.260036 rabbie-0.0.9/rabbie/encoder/
+-rw-rw-rw-   0        0        0       78 2023-05-11 11:17:49.000000 rabbie-0.0.9/rabbie/encoder/__init__.py
+-rw-rw-rw-   0        0        0      197 2023-05-11 11:17:49.000000 rabbie-0.0.9/rabbie/encoder/encoder.py
+drwxrwxrwx   0        0        0        0 2023-05-22 16:23:39.320132 rabbie-0.0.9/rabbie/encoder/encoders/
+-rw-rw-rw-   0        0        0       78 2023-05-11 11:17:49.000000 rabbie-0.0.9/rabbie/encoder/encoders/__init__.py
+-rw-rw-rw-   0        0        0      461 2023-05-11 11:17:49.000000 rabbie-0.0.9/rabbie/encoder/encoders/auto_encoder.py
+-rw-rw-rw-   0        0        0      215 2023-05-11 11:17:49.000000 rabbie-0.0.9/rabbie/encoder/encoders/json_encoder.py
+drwxrwxrwx   0        0        0        0 2023-05-22 16:23:39.322132 rabbie-0.0.9/rabbie/events/
+-rw-rw-rw-   0        0        0       53 2023-05-18 08:05:34.000000 rabbie-0.0.9/rabbie/events/__init__.py
+-rw-rw-rw-   0        0        0     1274 2023-05-18 08:05:34.000000 rabbie-0.0.9/rabbie/events/event.py
+drwxrwxrwx   0        0        0        0 2023-05-22 16:23:39.323131 rabbie-0.0.9/rabbie/logger/
+-rw-rw-rw-   0        0        0      631 2023-05-18 08:05:34.000000 rabbie-0.0.9/rabbie/logger/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-22 16:23:39.325131 rabbie-0.0.9/rabbie/producer/
+-rw-rw-rw-   0        0        0       46 2023-05-11 11:17:49.000000 rabbie-0.0.9/rabbie/producer/__init__.py
+-rw-rw-rw-   0        0        0     4898 2023-05-22 16:23:07.000000 rabbie-0.0.9/rabbie/producer/producer.py
+drwxrwxrwx   0        0        0        0 2023-05-22 16:23:39.328192 rabbie-0.0.9/rabbie/producer/publisher/
+-rw-rw-rw-   0        0        0       34 2023-05-11 11:17:49.000000 rabbie-0.0.9/rabbie/producer/publisher/__init__.py
+-rw-rw-rw-   0        0        0     3209 2023-05-22 16:23:07.000000 rabbie-0.0.9/rabbie/producer/publisher/publisher.py
+drwxrwxrwx   0        0        0        0 2023-05-22 16:23:39.330192 rabbie-0.0.9/rabbie/supervisor/
+-rw-rw-rw-   0        0        0       50 2023-04-24 20:01:12.000000 rabbie-0.0.9/rabbie/supervisor/__init__.py
+-rw-rw-rw-   0        0        0     4560 2023-04-24 20:01:12.000000 rabbie-0.0.9/rabbie/supervisor/supervisor.py
+drwxrwxrwx   0        0        0        0 2023-05-22 16:23:39.236009 rabbie-0.0.9/rabbie.egg-info/
+-rw-rw-rw-   0        0        0     9287 2023-05-22 16:23:39.000000 rabbie-0.0.9/rabbie.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1431 2023-05-22 16:23:39.000000 rabbie-0.0.9/rabbie.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-22 16:23:39.000000 rabbie-0.0.9/rabbie.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2023-05-22 16:23:39.000000 rabbie-0.0.9/rabbie.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-22 16:23:39.000000 rabbie-0.0.9/rabbie.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-22 16:23:39.338706 rabbie-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      854 2023-05-22 16:23:07.000000 rabbie-0.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-22 16:23:39.336192 rabbie-0.0.9/tests/
+-rw-rw-rw-   0        0        0     4962 2023-05-18 08:05:34.000000 rabbie-0.0.9/tests/test_consumer.py
+-rw-rw-rw-   0        0        0        0 2023-04-24 20:01:12.000000 rabbie-0.0.9/tests/test_decoder.py
+-rw-rw-rw-   0        0        0        0 2023-04-24 20:01:12.000000 rabbie-0.0.9/tests/test_listener.py
+-rw-rw-rw-   0        0        0        0 2023-04-24 20:01:12.000000 rabbie-0.0.9/tests/test_microconsumer.py
+-rw-rw-rw-   0        0        0        0 2023-05-11 11:17:49.000000 rabbie-0.0.9/tests/test_producer.py
```

### Comparing `rabbie-0.0.8/LICENSE` & `rabbie-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `rabbie-0.0.8/PKG-INFO` & `rabbie-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rabbie
-Version: 0.0.8
+Version: 0.0.9
 Summary: A simple, decorator interface for AMQP based message brokers
 Home-page: https://github.com/scuffi/rabbie
 Author: Archie Ferguson
 Author-email: iamarchieferguson@gmail.com
 License: MIT license
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `rabbie-0.0.8/README.md` & `rabbie-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `rabbie-0.0.8/rabbie/broker_types/channel.py` & `rabbie-0.0.9/rabbie/broker_types/channel.py`

 * *Files identical despite different names*

### Comparing `rabbie-0.0.8/rabbie/consumer/consumer.py` & `rabbie-0.0.9/rabbie/consumer/consumer.py`

 * *Files identical despite different names*

### Comparing `rabbie-0.0.8/rabbie/consumer/listener/listener.py` & `rabbie-0.0.9/rabbie/consumer/listener/listener.py`

 * *Files 4% similar despite different names*

```diff
@@ -81,35 +81,37 @@
             else body
             for arg in sig.parameters.keys()
         }
 
         # Run the callback function safely, so if it errors, the listener won't stop
         self._run_safely(self.details, Channel(channel), **arguments)
 
-    def _run_safely(self, details: ListenerDetails, channel: Channel, *args, **kwargs):
+    def _run_safely(
+        self, _details: ListenerDetails, _channel: Channel, *args, **kwargs
+    ):
         """
         This function runs a callback function safely, whilst still printing any tracebacks.
         """
         try:
             # Call the function, and keep it's output incase it requires repushing to the channel
-            output = details.callback(*args, **kwargs)
+            output = _details.callback(*args, **kwargs)
 
             # If there was data returned, we want to send this data back to the message broker
             if output is not None:
                 # Use specified encoder and send back to same queue
-                channel.publish(
+                _channel.publish(
                     body=output,
                     queue=self.details.return_queue or self.details.queue_name,
                     encoder=self.details.encoder,
                 )
         except Exception:
             traceback.print_exc()
 
     def _start_worker(self, index: int, registry: DictProxy):
-        # TODO: Change this function, it's ugly
+        # TODO: Change this function, it's ugly, (change to worker.py Worker class, encapsulate all Worker requirements in there)
         try:
             # Create a BlockingConnection into the queue
             connection = pika.BlockingConnection(self.connection_parameters)
 
             # Open a channel to receive messages through
             channel = connection.channel()
 
@@ -133,18 +135,14 @@
                 auto_ack=self.details.auto_ack,
             )
 
             # Allow for manipulation of channel before we start consuming incase we missed anything to do with configuration
             if self.details.configuration_callback:
                 self.details.configuration_callback(channel)
 
-            # TODO: Use this instead for more control of what variables to pass?
-            # for method, properties, body in channel.consume(self.queue_name):
-            #         self._callback(channel, method, properties, body)
-
             # Create a signal handler to close the connection when we receive a SIGINT
             def handle_sigterm(sig, frame):
                 log.debug("Gracefully closing connection...")
                 channel.close()
                 connection.close()
                 sys.exit(0)
 
@@ -158,14 +156,18 @@
             # We can assume now that we've connected successfully.
             self._change_status(registry, Status.CONNECTED)
 
             log.info(
                 f"[{os.getpid()}] [green]Listening to [bold cyan]{self.details.queue_name}[/bold cyan]"
             )
 
+            # TODO: Use this instead for more control of what variables to pass?
+            # for method, properties, body in channel.consume(self.details.queue_name):
+            #     self._callback(channel, method, properties, body)
+
             channel.start_consuming()
 
         except AMQPError:
             if self.details.restart:
                 if registry[os.getpid()] != Status.DISCONNECTED:
                     log.error(
                         f"[{os.getpid()}] [red]Connection to broker failed. Worker will reconnect when possible."
```

### Comparing `rabbie-0.0.8/rabbie/consumer/listener/listener_details.py` & `rabbie-0.0.9/rabbie/consumer/listener/listener_details.py`

 * *Files identical despite different names*

### Comparing `rabbie-0.0.8/rabbie/consumer/microconsumer.py` & `rabbie-0.0.9/rabbie/consumer/microconsumer.py`

 * *Files identical despite different names*

### Comparing `rabbie-0.0.8/rabbie/events/event.py` & `rabbie-0.0.9/rabbie/events/event.py`

 * *Files identical despite different names*

### Comparing `rabbie-0.0.8/rabbie/logger/__init__.py` & `rabbie-0.0.9/rabbie/logger/__init__.py`

 * *Files identical despite different names*

### Comparing `rabbie-0.0.8/rabbie/producer/producer.py` & `rabbie-0.0.9/rabbie/producer/producer.py`

 * *Files 3% similar despite different names*

```diff
@@ -61,15 +61,22 @@
         self.connection_parameters = pika.ConnectionParameters(
             port=self._port,
             host=self._host,
             credentials=credentials,
             **kwargs,
         )
 
-        self.connection = connection_type(self.connection_parameters)
+        self.connection_type = connection_type
+
+        # Assume that when connection is None we are not connected
+        self.connection: pika.BlockingConnection = None
+
+    def _is_connected(self):
+        if self.connection is None or self.connection.is_closed:
+            self.connection = self.connection_type(self.connection_parameters)
 
     def connect(self, queue: str = None, exchange: str = None, encoder: Encoder = None):
         """
         Connect to a message broker. This does NOT open a connection, unless you are using a context manager.
 
         You should always use this function like: `with producer.connect() as channel:`
 
@@ -84,13 +91,15 @@
         format to be used for the messages being published. It is an instance of the Encoder class, which is
         responsible for serializing the message data into a format that can be transmitted over the network.
         If no encoder is specified, the default encoder for
 
         Returns:
           A Publisher object is being returned.
         """
+        self._is_connected()
+
         return Publisher(
             connection=self.connection,
             default_queue=queue,
             default_exchange=exchange,
             default_encoder=encoder,
         )
```

### Comparing `rabbie-0.0.8/rabbie/producer/publisher/publisher.py` & `rabbie-0.0.9/rabbie/producer/publisher/publisher.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 
     def close(self):
         """
         This function closes the channel.
         """
         self.channel.close()
         self.channel = None
+        self.connection.close()
 
     def publish(
         self,
         body: str,
         queue: str = None,
         properties: Properties = None,
         encoder: Encoder = None,
```

### Comparing `rabbie-0.0.8/rabbie/supervisor/supervisor.py` & `rabbie-0.0.9/rabbie/supervisor/supervisor.py`

 * *Files identical despite different names*

### Comparing `rabbie-0.0.8/rabbie.egg-info/PKG-INFO` & `rabbie-0.0.9/rabbie.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rabbie
-Version: 0.0.8
+Version: 0.0.9
 Summary: A simple, decorator interface for AMQP based message brokers
 Home-page: https://github.com/scuffi/rabbie
 Author: Archie Ferguson
 Author-email: iamarchieferguson@gmail.com
 License: MIT license
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `rabbie-0.0.8/rabbie.egg-info/SOURCES.txt` & `rabbie-0.0.9/rabbie.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rabbie-0.0.8/setup.py` & `rabbie-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
-version = "0.0.8"
+version = "0.0.9"
 requirements = ["pika", "multiprocess", "rich", "watchdog"]
 
 setup(
     name="rabbie",
     version=version,
     author="Archie Ferguson",
     author_email="iamarchieferguson@gmail.com",
```

### Comparing `rabbie-0.0.8/tests/test_consumer.py` & `rabbie-0.0.9/tests/test_consumer.py`

 * *Files identical despite different names*

