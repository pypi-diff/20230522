# Comparing `tmp/rstream-0.6.0.tar.gz` & `tmp/rstream-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rstream-0.6.0.tar", max compression
+gzip compressed data, was "rstream-0.7.0.tar", max compression
```

## Comparing `rstream-0.6.0.tar` & `rstream-0.7.0.tar`

### file list

```diff
@@ -1,15 +1,16 @@
--rw-r--r--   0        0        0     1074 2023-04-12 12:26:02.281874 rstream-0.6.0/LICENSE
--rw-r--r--   0        0        0     5442 2023-04-12 12:26:02.281874 rstream-0.6.0/README.md
--rw-r--r--   0        0        0      660 2023-04-12 12:26:02.281874 rstream-0.6.0/pyproject.toml
--rw-r--r--   0        0        0      721 2023-04-12 12:26:02.281874 rstream-0.6.0/rstream/__init__.py
--rw-r--r--   0        0        0      651 2023-04-12 12:26:02.281874 rstream-0.6.0/rstream/amqp.py
--rw-r--r--   0        0        0    17432 2023-04-12 12:26:02.281874 rstream-0.6.0/rstream/client.py
--rw-r--r--   0        0        0     2117 2023-04-12 12:26:02.285874 rstream-0.6.0/rstream/connection.py
--rw-r--r--   0        0        0      928 2023-04-12 12:26:02.285874 rstream-0.6.0/rstream/constants.py
--rw-r--r--   0        0        0     8080 2023-04-12 12:26:02.285874 rstream-0.6.0/rstream/consumer.py
--rw-r--r--   0        0        0     5638 2023-04-12 12:26:02.285874 rstream-0.6.0/rstream/encoding.py
--rw-r--r--   0        0        0     1364 2023-04-12 12:26:02.285874 rstream-0.6.0/rstream/exceptions.py
--rw-r--r--   0        0        0    12802 2023-04-12 12:26:02.285874 rstream-0.6.0/rstream/producer.py
--rw-r--r--   0        0        0    12768 2023-04-12 12:26:02.285874 rstream-0.6.0/rstream/schema.py
--rw-r--r--   0        0        0      705 2023-04-12 12:26:02.285874 rstream-0.6.0/rstream/utils.py
--rw-r--r--   0        0        0     6073 1970-01-01 00:00:00.000000 rstream-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-05-22 09:13:56.508781 rstream-0.7.0/LICENSE
+-rw-r--r--   0        0        0     6796 2023-05-22 09:13:56.508781 rstream-0.7.0/README.md
+-rw-r--r--   0        0        0      660 2023-05-22 09:13:56.508781 rstream-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0      799 2023-05-22 09:13:56.508781 rstream-0.7.0/rstream/__init__.py
+-rw-r--r--   0        0        0      651 2023-05-22 09:13:56.508781 rstream-0.7.0/rstream/amqp.py
+-rw-r--r--   0        0        0    17432 2023-05-22 09:13:56.508781 rstream-0.7.0/rstream/client.py
+-rw-r--r--   0        0        0     4883 2023-05-22 09:13:56.508781 rstream-0.7.0/rstream/compression.py
+-rw-r--r--   0        0        0     2117 2023-05-22 09:13:56.508781 rstream-0.7.0/rstream/connection.py
+-rw-r--r--   0        0        0      928 2023-05-22 09:13:56.508781 rstream-0.7.0/rstream/constants.py
+-rw-r--r--   0        0        0     8080 2023-05-22 09:13:56.508781 rstream-0.7.0/rstream/consumer.py
+-rw-r--r--   0        0        0     5638 2023-05-22 09:13:56.508781 rstream-0.7.0/rstream/encoding.py
+-rw-r--r--   0        0        0     1364 2023-05-22 09:13:56.508781 rstream-0.7.0/rstream/exceptions.py
+-rw-r--r--   0        0        0    15804 2023-05-22 09:13:56.508781 rstream-0.7.0/rstream/producer.py
+-rw-r--r--   0        0        0    15024 2023-05-22 09:13:56.508781 rstream-0.7.0/rstream/schema.py
+-rw-r--r--   0        0        0      950 2023-05-22 09:13:56.508781 rstream-0.7.0/rstream/utils.py
+-rw-r--r--   0        0        0     7427 1970-01-01 00:00:00.000000 rstream-0.7.0/PKG-INFO
```

### Comparing `rstream-0.6.0/LICENSE` & `rstream-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rstream-0.6.0/README.md` & `rstream-0.7.0/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -12,16 +12,17 @@
 ## Quick start
 
 ### Publishing messages: 
 
 You can publish messages with three different methods:
 
 * send: asynchronous, messages are automatically buffered internally and sent at once after a timeout expires.
-* batch_send: Synchronous, the user buffers the messages and sends them. This is the fastest publishing method.
-* send_wait: Synchronous, the caller wait till the message is confirmed. This is the slowest publishing method.
+* batch_send: synchronous, the user buffers the messages and sends them. This is the fastest publishing method.
+* send_wait: synchronous, the caller wait till the message is confirmed. This is the slowest publishing method.
+* send_sub_entry: asynchronous, allow batch in sub-entry mode. This mode increases throughput at the cost of increased latency and potential duplicated messages even when deduplication is enabled. It also allows using compression to reduce bandwidth and storage if messages are reasonably similar, at the cost of increasing CPU usage on the client side.
 
 Example Using send:
 
 ```python
 import asyncio
 from rstream import Producer, AMQPMessage
 
@@ -55,15 +56,15 @@
                 body='hello: {}'.format(i),
             )
             await producer.send_wait('mystream', amqp_message)
 
 asyncio.run(publish())
 ```
 
-Eventually using batch_send:
+or using batch_send:
 
 ```python
 import asyncio
 from rstream import Producer, AMQPMessage
 
 async def publish():
     async with Producer('localhost', username='guest', password='guest') as producer:
@@ -77,14 +78,44 @@
             list_messages.append(amqp_message)
 
         await producer.send_batch('mystream',  list_messages) 
 
 asyncio.run(publish())
 ```
 
+and eventually using sub_entry_batch:
+
+```python
+async def publish():
+    async with Producer('localhost', username='guest', password='guest') as producer:
+        await producer.delete_stream('mystream', missing_ok=True)
+        await producer.create_stream('mystream', exists_ok=True)
+
+        messages = []
+        for i in range(10):
+            amqp_message = AMQPMessage(
+                body='a:{}'.format(i),
+            )
+            messages.append(amqp_message_list)
+
+       
+        await producer.send_sub_entry('mixing', compression_type=CompressionType.Gzip,
+                                      sub_entry_messages=messages)
+        
+        
+        await producer.send_sub_entry('mixing', compression_type=CompressionType.No,
+                                      sub_entry_messages=messages)
+
+    await producer.close()
+  
+asyncio.run(publish())
+```
+
+You have the possibility to specify NoCompression (compression_type=CompressionType.No) or Gzip (compression_type=CompressionType.Gzip).
+
 ### Publishing with confirmation
 
 The Send method takes as parameter an handle function that will be called asynchronously when the message sent will be notified from the server to have been published.
 
 In this case the example will work like this:
```

### Comparing `rstream-0.6.0/pyproject.toml` & `rstream-0.7.0/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "rstream"
-version = "0.6.0"
+version = "0.7.0"
 description = "A python client for RabbitMQ Streams"
 authors = ["George Fortunatov <qweeeze@gmail.com>"]
 readme = "README.md"
 homepage = "https://github.com/qweeze/rstream"
 repository = "https://github.com/qweeze/rstream"
 license = "MIT"
```

### Comparing `rstream-0.6.0/rstream/__init__.py` & `rstream-0.7.0/rstream/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 except metadata.PackageNotFoundError:
     __version__ = "dev"
     __license__ = None
 
 del metadata
 
 from .amqp import AMQPMessage, amqp_decoder  # noqa: E402
+from .compression import CompressionType  # noqa: E402
 from .constants import OffsetType  # noqa: E402
 from .consumer import Consumer  # noqa: E402
 from .producer import (  # noqa: E402
     ConfirmationStatus,
     Producer,
     RawMessage,
 )
@@ -25,8 +26,9 @@
     "AMQPMessage",
     "amqp_decoder",
     "Consumer",
     "RawMessage",
     "Producer",
     "OffsetType",
     "ConfirmationStatus",
+    "CompressionType",
 ]
```

### Comparing `rstream-0.6.0/rstream/amqp.py` & `rstream-0.7.0/rstream/amqp.py`

 * *Files identical despite different names*

### Comparing `rstream-0.6.0/rstream/client.py` & `rstream-0.7.0/rstream/client.py`

 * *Files identical despite different names*

### Comparing `rstream-0.6.0/rstream/connection.py` & `rstream-0.7.0/rstream/connection.py`

 * *Files identical despite different names*

### Comparing `rstream-0.6.0/rstream/constants.py` & `rstream-0.7.0/rstream/constants.py`

 * *Files identical despite different names*

### Comparing `rstream-0.6.0/rstream/consumer.py` & `rstream-0.7.0/rstream/consumer.py`

 * *Files identical despite different names*

### Comparing `rstream-0.6.0/rstream/encoding.py` & `rstream-0.7.0/rstream/encoding.py`

 * *Files identical despite different names*

### Comparing `rstream-0.6.0/rstream/exceptions.py` & `rstream-0.7.0/rstream/exceptions.py`

 * *Files identical despite different names*

### Comparing `rstream-0.6.0/rstream/producer.py` & `rstream-0.7.0/rstream/producer.py`

 * *Files 19% similar despite different names*

```diff
@@ -19,14 +19,20 @@
     TypeVar,
     Union,
 )
 
 from . import exceptions, schema, utils
 from .amqp import _MessageProtocol
 from .client import Addr, Client, ClientPool
+from .compression import (
+    CompressionHelper,
+    CompressionType,
+    ICompressionCodec,
+)
+from .utils import RawMessage
 
 MessageT = TypeVar("MessageT", _MessageProtocol, bytes)
 MT = TypeVar("MT")
 CB = Annotated[Callable[[MT], Union[None, Awaitable[None]]], "Message callback type"]
 
 
 @dataclass
@@ -35,26 +41,18 @@
     reference: str
     stream: str
     sequence: utils.MonotonicSeq
     client: Client
 
 
 @dataclass
-class RawMessage(_MessageProtocol):
-    data: bytes
-    publishing_id: Optional[int] = None
-
-    def __bytes__(self) -> bytes:
-        return self.data
-
-
-@dataclass
 class _MessageNotification(Generic[MessageT]):
-    message: MessageT
+    entry: MessageT | ICompressionCodec
     callback: Optional[CB[ConfirmationStatus]] = None
+    publisher_name: Optional[str] = None
 
 
 @dataclass
 class ConfirmationStatus:
     message_id: int
     is_confirmed: bool = False
     response_code: int = 0
@@ -198,80 +196,124 @@
         batch: list[MessageT],
         publisher_name: Optional[str] = None,
         on_publish_confirm: Optional[CB[ConfirmationStatus]] = None,
     ) -> list[int]:
 
         wrapped_batch = []
         for item in batch:
-            wrapped_item = _MessageNotification(item, on_publish_confirm)
+            wrapped_item = _MessageNotification(
+                entry=item, callback=on_publish_confirm, publisher_name=publisher_name
+            )
             wrapped_batch.append(wrapped_item)
 
-        return await self._send_batch(stream, wrapped_batch, sync=False, publisher_name=publisher_name)
+        return await self._send_batch(stream, wrapped_batch, sync=False)
 
     async def _send_batch(
         self,
         stream: str,
         batch: list[_MessageNotification],
         sync: bool = True,
-        publisher_name: Optional[str] = None,
     ) -> list[int]:
         if len(batch) == 0:
             raise ValueError("Empty batch")
 
-        async with self._lock:
-            publisher = await self._get_or_create_publisher(stream, publisher_name=publisher_name)
-
         messages = []
+        publishing_ids = set()
+        publishing_ids_callback: dict[CB[ConfirmationStatus], set[int]] = defaultdict(set)
 
         for item in batch:
 
-            msg = RawMessage(item.message) if isinstance(item.message, bytes) else item.message
+            async with self._lock:
+                publisher = await self._get_or_create_publisher(stream, publisher_name=item.publisher_name)
+
+            if not isinstance(item.entry, ICompressionCodec):
+
+                msg = RawMessage(item.entry) if isinstance(item.entry, bytes) else item.entry
 
-            if msg.publishing_id is None:
-                msg.publishing_id = publisher.sequence.next()
+                if msg.publishing_id is None:
+                    msg.publishing_id = publisher.sequence.next()
 
-            messages.append(
-                schema.Message(
-                    publishing_id=msg.publishing_id,
-                    data=bytes(msg),
+                messages.append(
+                    schema.Message(
+                        publishing_id=msg.publishing_id,
+                        data=bytes(msg),
+                    )
                 )
-            )
 
-        await publisher.client.send_frame(
-            schema.Publish(
-                publisher_id=publisher.id,
-                messages=messages,
-            ),
-        )
+                if item.callback is not None:
+                    publishing_ids_callback[item.callback].update([msg.publishing_id])
+
+            else:
+                compression_codec = item.entry
+                if len(messages) > 0:
+                    await publisher.client.send_frame(
+                        schema.Publish(
+                            publisher_id=publisher.id,
+                            messages=messages,
+                        ),
+                    )
+                    # publishing_ids.update([m.publishing_id for m in messages])
+                    messages.clear()
+                for _ in range(item.entry.messages_count()):
+                    publishing_id = publisher.sequence.next()
+
+                await publisher.client.send_frame(
+                    schema.PublishSubBatching(
+                        publisher_id=publisher.id,
+                        number_of_root_messages=1,
+                        publishing_id=publishing_id,
+                        compress_type=0x80 | compression_codec.compression_type() << 4,
+                        subbatching_message_count=compression_codec.messages_count(),
+                        uncompressed_data_size=compression_codec.uncompressed_size(),
+                        compressed_data_size=compression_codec.compressed_size(),
+                        messages=compression_codec.data(),
+                    ),
+                )
+                publishing_ids.update([publishing_id])
+
+                if item.callback is not None:
+                    publishing_ids_callback[item.callback].update([publishing_id])
 
-        publishing_ids = [m.publishing_id for m in messages]
+        if len(messages) > 0:
 
-        if item.callback is not None:
-            self._waiting_for_confirm[publisher.reference][item.callback] = set(publishing_ids)
-        elif sync:
+            await publisher.client.send_frame(
+                schema.Publish(
+                    publisher_id=publisher.id,
+                    messages=messages,
+                ),
+            )
+            publishing_ids.update([m.publishing_id for m in messages])
+
+        for callback in publishing_ids_callback:
+            self._waiting_for_confirm[publisher.reference][callback] = publishing_ids_callback[
+                callback
+            ].copy()
+        # this is just called in case of send_wait
+        if sync:
             future: asyncio.Future[None] = asyncio.Future()
-            self._waiting_for_confirm[publisher.reference][future] = set(publishing_ids)
+            self._waiting_for_confirm[publisher.reference][future] = publishing_ids.copy()
             await future
 
-        return publishing_ids
+        return list(publishing_ids)
 
     async def send_wait(
         self,
         stream: str,
         message: MessageT,
         publisher_name: Optional[str] = None,
     ) -> int:
 
-        wrapped_message: _MessageNotification = _MessageNotification(message, None)
+        wrapped_message: _MessageNotification = _MessageNotification(
+            entry=message, callback=None, publisher_name=publisher_name
+        )
 
         publishing_ids = await self._send_batch(
             stream,
             [wrapped_message],
             sync=True,
-            publisher_name=publisher_name,
         )
         return publishing_ids[0]
 
     def _timer_completed(self, context):
 
         if not context.cancelled():
             if context.exception():
@@ -288,18 +330,44 @@
     ):
 
         # start the background thread to send buffered messages
         if self.task is None:
             self.task = asyncio.create_task(self._timer())
             self.task.add_done_callback(self._timer_completed)
 
-        async with self._lock:
-            await self._get_or_create_publisher(stream, publisher_name=publisher_name)
+        wrapped_message = _MessageNotification(
+            entry=message, callback=on_publish_confirm, publisher_name=publisher_name
+        )
+        async with self._buffered_messages_lock:
+            self._buffered_messages[stream].append(wrapped_message)
+
+        await asyncio.sleep(0)
+
+    async def send_sub_entry(
+        self,
+        stream: str,
+        sub_entry_messages: list[MessageT],
+        compression_type: CompressionType = CompressionType.No,
+        publisher_name: Optional[str] = None,
+        on_publish_confirm: Optional[CB[ConfirmationStatus]] = None,
+    ):
+
+        if len(sub_entry_messages) == 0:
+            raise ValueError("Empty batch")
+
+        # start the background thread to send buffered messages
+        if self.task is None:
+            self.task = asyncio.create_task(self._timer())
+            self.task.add_done_callback(self._timer_completed)
+
+        compression_codec = CompressionHelper.compress(sub_entry_messages, compression_type)
 
-        wrapped_message = _MessageNotification(message, on_publish_confirm)
+        wrapped_message = _MessageNotification(
+            entry=compression_codec, callback=on_publish_confirm, publisher_name=publisher_name
+        )
         async with self._buffered_messages_lock:
             self._buffered_messages[stream].append(wrapped_message)
 
         await asyncio.sleep(0)
 
     # After the timeout send the messages in _buffered_messages in batches
     async def _timer(self):
```

### Comparing `rstream-0.6.0/rstream/schema.py` & `rstream-0.7.0/rstream/schema.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # Copyright 2023 VMware, Inc. All Rights Reserved.
 # SPDX-License-Identifier: MIT
 
 import zlib
 from dataclasses import dataclass, field
 from typing import ClassVar, Optional, Type, cast
 
+from .compression import CompressionHelper, CompressionType
 from .constants import Key, OffsetType, T
 from .exceptions import ServerError
 
 registry: dict[tuple[bool, Key], Type["Frame"]] = {}
 
 
 @dataclass
@@ -179,14 +180,27 @@
 @dataclass
 class Message(Struct):
     publishing_id: int = field(metadata={"type": T.uint64})
     data: bytes = field(metadata={"type": T.bytes})
 
 
 @dataclass
+class PublishSubBatching(Frame):
+    key = Key.Publish
+    publisher_id: int = field(metadata={"type": T.uint8})
+    number_of_root_messages: int = field(metadata={"type": T.int32})
+    publishing_id: int = field(metadata={"type": T.uint64})
+    compress_type: int = field(metadata={"type": T.uint8})
+    subbatching_message_count: int = field(metadata={"type": T.uint16})
+    uncompressed_data_size: int = field(metadata={"type": T.int32})
+    compressed_data_size: int = field(metadata={"type": T.int32})
+    messages: bytes = field(metadata={"type": T.raw})
+
+
+@dataclass
 class Publish(Frame):
     key = Key.Publish
     publisher_id: int = field(metadata={"type": T.uint8})
     messages: list[Message]
 
 
 @dataclass
@@ -372,14 +386,47 @@
     key = Key.QueryOffset
     correlation_id: int = field(metadata={"type": T.uint32})
     response_code: int = field(metadata={"type": T.uint16})
     offset: int = field(metadata={"type": T.uint64})
 
 
 @dataclass
+class SubEntryChunk:
+    @classmethod
+    def read(self, data: bytes, entry_type: int, offset: int) -> tuple[list[bytes], int]:
+        # total bytes read
+        index = 0
+        num_records_in_batch = int.from_bytes(data[index + offset : index + offset + 2], byteorder="big")
+        index += 2
+        uncompressed_data_size = int.from_bytes(data[index + offset : index + offset + 4], byteorder="big")
+        index += 4
+        data_len = int.from_bytes(data[index + offset : index + offset + 4], byteorder="big")
+        index += 4
+
+        compression_type = CompressionType((entry_type & 0x70) >> 4)
+
+        current_pos = index + offset
+        data_compressed = data[current_pos : current_pos + data_len]
+        index += data_len
+
+        uncompressed_data = CompressionHelper.uncompress(
+            data_compressed, compression_type=compression_type, uncompressed_data_size=uncompressed_data_size
+        )
+        subbatch_entries = []
+        uncompressed_index = 0
+        for i in range(num_records_in_batch):
+            size = int.from_bytes(uncompressed_data[uncompressed_index : uncompressed_index + 4], "big")
+            uncompressed_index += 4
+            subbatch_entries.append(uncompressed_data[uncompressed_index : uncompressed_index + size])
+            uncompressed_index += size
+
+        return subbatch_entries, index
+
+
+@dataclass
 class Deliver(Frame):
     key = Key.Deliver
     subscription_id: int = field(metadata={"type": T.uint8})
     magic_version: int = field(metadata={"type": T.int8})
     chunk_type: int = field(metadata={"type": T.int8})
     num_entries: int = field(metadata={"type": T.uint16})
     num_records: int = field(metadata={"type": T.uint32})
@@ -401,22 +448,29 @@
 
         if zlib.crc32(self.data) != self.chunk_crc:
             raise ValueError("Invalid checksum")
 
     def get_messages(self) -> list[bytes]:
         messages = []
         pos = 0
+
         for _ in range(self.num_entries):
-            if (self.data[pos] & 0x80) == 0:
+            entry_type = self.data[pos]
+
+            if entry_type & 0x80 == 0:
                 size = int.from_bytes(self.data[pos : pos + 4], "big")
                 pos += 4
                 messages.append(self.data[pos : pos + size])
                 pos += size
+            # is a subentry-batch message
             else:
-                raise NotImplementedError
+                pos += 1
+                sub_batched_messages, total_bytes_read = SubEntryChunk.read(self.data, entry_type, pos)
+                messages.extend(sub_batched_messages)
+                pos += total_bytes_read
 
         return messages
 
 
 @dataclass
 class Credit(Frame):
     key = Key.Credit
```

### Comparing `rstream-0.6.0/PKG-INFO` & `rstream-0.7.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rstream
-Version: 0.6.0
+Version: 0.7.0
 Summary: A python client for RabbitMQ Streams
 Home-page: https://github.com/qweeze/rstream
 License: MIT
 Author: George Fortunatov
 Author-email: qweeeze@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -30,16 +30,17 @@
 ## Quick start
 
 ### Publishing messages: 
 
 You can publish messages with three different methods:
 
 * send: asynchronous, messages are automatically buffered internally and sent at once after a timeout expires.
-* batch_send: Synchronous, the user buffers the messages and sends them. This is the fastest publishing method.
-* send_wait: Synchronous, the caller wait till the message is confirmed. This is the slowest publishing method.
+* batch_send: synchronous, the user buffers the messages and sends them. This is the fastest publishing method.
+* send_wait: synchronous, the caller wait till the message is confirmed. This is the slowest publishing method.
+* send_sub_entry: asynchronous, allow batch in sub-entry mode. This mode increases throughput at the cost of increased latency and potential duplicated messages even when deduplication is enabled. It also allows using compression to reduce bandwidth and storage if messages are reasonably similar, at the cost of increasing CPU usage on the client side.
 
 Example Using send:
 
 ```python
 import asyncio
 from rstream import Producer, AMQPMessage
 
@@ -73,15 +74,15 @@
                 body='hello: {}'.format(i),
             )
             await producer.send_wait('mystream', amqp_message)
 
 asyncio.run(publish())
 ```
 
-Eventually using batch_send:
+or using batch_send:
 
 ```python
 import asyncio
 from rstream import Producer, AMQPMessage
 
 async def publish():
     async with Producer('localhost', username='guest', password='guest') as producer:
@@ -95,14 +96,44 @@
             list_messages.append(amqp_message)
 
         await producer.send_batch('mystream',  list_messages) 
 
 asyncio.run(publish())
 ```
 
+and eventually using sub_entry_batch:
+
+```python
+async def publish():
+    async with Producer('localhost', username='guest', password='guest') as producer:
+        await producer.delete_stream('mystream', missing_ok=True)
+        await producer.create_stream('mystream', exists_ok=True)
+
+        messages = []
+        for i in range(10):
+            amqp_message = AMQPMessage(
+                body='a:{}'.format(i),
+            )
+            messages.append(amqp_message_list)
+
+       
+        await producer.send_sub_entry('mixing', compression_type=CompressionType.Gzip,
+                                      sub_entry_messages=messages)
+        
+        
+        await producer.send_sub_entry('mixing', compression_type=CompressionType.No,
+                                      sub_entry_messages=messages)
+
+    await producer.close()
+  
+asyncio.run(publish())
+```
+
+You have the possibility to specify NoCompression (compression_type=CompressionType.No) or Gzip (compression_type=CompressionType.Gzip).
+
 ### Publishing with confirmation
 
 The Send method takes as parameter an handle function that will be called asynchronously when the message sent will be notified from the server to have been published.
 
 In this case the example will work like this:
```

