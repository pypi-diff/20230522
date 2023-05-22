# Comparing `tmp/Shimarin-0.0.8.tar.gz` & `tmp/Shimarin-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Shimarin-0.0.8.tar", last modified: Sun May 21 19:04:46 2023, max compression
+gzip compressed data, was "Shimarin-0.0.9.tar", last modified: Mon May 22 12:23:19 2023, max compression
```

## Comparing `Shimarin-0.0.8.tar` & `Shimarin-0.0.9.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 19:04:46.386985 Shimarin-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-05-21 19:04:46.386985 Shimarin-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-05-21 19:04:37.000000 Shimarin-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 19:04:46.382984 Shimarin-0.0.8/Shimarin/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 19:04:37.000000 Shimarin-0.0.8/Shimarin/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 19:04:46.386985 Shimarin-0.0.8/Shimarin/client/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 19:04:37.000000 Shimarin-0.0.8/Shimarin/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-05-21 19:04:37.000000 Shimarin-0.0.8/Shimarin/client/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4724 2023-05-21 19:04:37.000000 Shimarin-0.0.8/Shimarin/client/events.py
--rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-05-21 19:04:37.000000 Shimarin-0.0.8/Shimarin/client/networking.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 19:04:46.386985 Shimarin-0.0.8/Shimarin/server/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 19:04:37.000000 Shimarin-0.0.8/Shimarin/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2600 2023-05-21 19:04:37.000000 Shimarin-0.0.8/Shimarin/server/events.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 19:04:46.386985 Shimarin-0.0.8/Shimarin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-05-21 19:04:46.000000 Shimarin-0.0.8/Shimarin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-05-21 19:04:46.000000 Shimarin-0.0.8/Shimarin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 19:04:46.000000 Shimarin-0.0.8/Shimarin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 19:04:46.000000 Shimarin-0.0.8/Shimarin.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-21 19:04:46.000000 Shimarin-0.0.8/Shimarin.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-21 19:04:46.000000 Shimarin-0.0.8/Shimarin.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-21 19:04:37.000000 Shimarin-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-05-21 19:04:46.390985 Shimarin-0.0.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 12:23:19.198397 Shimarin-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-05-22 12:23:19.198397 Shimarin-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-05-22 12:23:07.000000 Shimarin-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 12:23:19.194397 Shimarin-0.0.9/Shimarin/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 12:23:07.000000 Shimarin-0.0.9/Shimarin/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 12:23:19.198397 Shimarin-0.0.9/Shimarin/client/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 12:23:07.000000 Shimarin-0.0.9/Shimarin/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-05-22 12:23:07.000000 Shimarin-0.0.9/Shimarin/client/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5453 2023-05-22 12:23:07.000000 Shimarin-0.0.9/Shimarin/client/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-05-22 12:23:07.000000 Shimarin-0.0.9/Shimarin/client/networking.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 12:23:19.198397 Shimarin-0.0.9/Shimarin/server/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 12:23:07.000000 Shimarin-0.0.9/Shimarin/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3502 2023-05-22 12:23:07.000000 Shimarin-0.0.9/Shimarin/server/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-05-22 12:23:07.000000 Shimarin-0.0.9/Shimarin/server/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 12:23:19.194397 Shimarin-0.0.9/Shimarin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-05-22 12:23:19.000000 Shimarin-0.0.9/Shimarin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-05-22 12:23:19.000000 Shimarin-0.0.9/Shimarin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 12:23:19.000000 Shimarin-0.0.9/Shimarin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 12:23:19.000000 Shimarin-0.0.9/Shimarin.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-22 12:23:19.000000 Shimarin-0.0.9/Shimarin.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-22 12:23:19.000000 Shimarin-0.0.9/Shimarin.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-22 12:23:07.000000 Shimarin-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-05-22 12:23:19.198397 Shimarin-0.0.9/setup.cfg
```

### Comparing `Shimarin-0.0.8/PKG-INFO` & `Shimarin-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Shimarin
-Version: 0.0.8
+Version: 0.0.9
 Summary: asynchronous event-based communication between client and server
 Home-page: 
 Author: Kamuri Amorim
 Author-email: myk.gata14@gmail.com
 License: MIT
 Keywords: python events client server asynchronous
 Description-Content-Type: text/markdown
```

### Comparing `Shimarin-0.0.8/Shimarin/client/events.py` & `Shimarin-0.0.9/Shimarin/client/events.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,76 +9,100 @@
 from .networking import send_get_request, Response
 
 
 logger = logging.getLogger("Shimarin")
 
 
 class Event:
-    def __init__(self, event_type: str, identifier: str, payload: str | None, session: aiohttp.ClientSession, server_endpoint: str = config.SERVER_ENDPOINT) -> None:
+    def __init__(
+        self,
+        event_type: str,
+        identifier: str,
+        payload: str | None,
+        session: aiohttp.ClientSession,
+        server_endpoint: str = config.SERVER_ENDPOINT,
+        custom_headers: dict = {},
+    ) -> None:
         self.event_type = event_type
         self.payload = payload
         self.identifier = identifier
         self.__session = session
         self.server_endpoint = server_endpoint
+        self.custom_headers = custom_headers
 
     @staticmethod
-    def new(event_data: dict[str, str], session: aiohttp.ClientSession | None, server_endpoint: str = config.SERVER_ENDPOINT) -> 'Event':
-        return Event(event_data['event_type'], event_data['identifier'], event_data['payload'], session, server_endpoint)
-    
+    def new(
+        event_data: dict[str, str],
+        session: aiohttp.ClientSession | None,
+        server_endpoint: str = config.SERVER_ENDPOINT,
+        custom_headers: dict = {},
+    ) -> "Event":
+        return Event(
+            event_data["event_type"],
+            event_data["identifier"],
+            event_data["payload"],
+            session,
+            server_endpoint,
+            custom_headers,
+        )
+
     async def reply(self, payload: Any):
-        data = {
-            "identifier": str(self.identifier),
-            "payload": json.dumps(payload)
-        }
-        await send_get_request(self.__session, f"{self.server_endpoint}/callback", json=data)
-    
+        data = {"identifier": str(self.identifier), "payload": json.dumps(payload)}
+        await send_get_request(
+            self.__session,
+            f"{self.server_endpoint}/callback",
+            json=data,
+            headers=self.custom_headers,
+        )
+
     def __str__(self) -> str:
         return f"Event: {self.event_type}, Identifier: {self.identifier}, Payload: {self.payload}"
-    
+
     def __repr__(self) -> str:
         return self.__str__()
 
 
 class EventHandler:
     def __init__(self, event_type: str, callback: Callable[[Any, Any], Any]) -> None:
         self.event_type = event_type
         self.callback = callback
 
     async def trigger(self, *args, **kwargs) -> None:
         await self.callback(*args, **kwargs)
 
     def __str__(self) -> str:
         return f"Event: {self.event_type}, Callback: {self.callback}"
-    
+
     def __repr__(self) -> str:
         return self.__str__()
 
 
 class EventsHandlers:
     def __init__(self):
         self.handlers: list[EventHandler] = []
-    
+
     def register(self, handler: EventHandler) -> None:
         self.handlers.append(handler)
 
     def new(self, event_name: str):
         def wrapper(func: Callable):
             event_handler = EventHandler(event_name, func)
             self.register(event_handler)
             return func
+
         return wrapper
 
     async def handle(self, event: Event) -> None:
         for handle in self.handlers:
             if handle.event_type == event.event_type:
                 asyncio.gather(handle.trigger(event))
-    
+
     def __str__(self) -> str:
         return f"Handlers: {self.handlers}"
-    
+
     def __repr__(self) -> str:
         return self.__str__()
 
 
 class EventPolling:
     def __init__(self, events_handlers: EventsHandlers) -> None:
         self.session = aiohttp.ClientSession()
@@ -90,30 +114,52 @@
         await self.session.__aenter__()
         return self
 
     async def __aexit__(self, exc_type, exc_val, tb):
         if self.session:
             await self.session.__aexit__(exc_type, exc_val, tb)
 
-    async def start(self, polling_interval: int = 1, fetch: int = 10, custom_headers: dict = {}, server_endpoint: str = config.SERVER_ENDPOINT, retries: int = 5):
+    async def start(
+        self,
+        polling_interval: int = 1,
+        fetch: int = 10,
+        custom_headers: dict = {},
+        server_endpoint: str = config.SERVER_ENDPOINT,
+        retries: int = 5,
+    ):
         self.is_polling = True
         while self.is_polling:
             for _ in range(retries):
                 try:
-                    events: Response = await send_get_request(self.session, f"{server_endpoint}/events?fetch={fetch}", headers=custom_headers)
+                    events: Response = await send_get_request(
+                        self.session,
+                        f"{server_endpoint}/events?fetch={fetch}",
+                        headers=custom_headers,
+                    )
+
                     if events.status == 200:
                         event_json = await events.json()
                         for event in event_json:
                             if event_json:
-                                event = Event.new(event, self.session, server_endpoint)
+                                event = Event.new(
+                                    event, self.session, server_endpoint, custom_headers
+                                )
                                 await self.__task_manager(event)
                         break
                     raise aiohttp.ServerConnectionError
-                except (aiohttp.ClientError, aiohttp.ServerTimeoutError, aiohttp.ServerDisconnectedError, aiohttp.ServerConnectionError, aiohttp.ClientConnectionError):
-                    logger.warning(f"Error connecting to {server_endpoint}! Retrying...")
+                except (
+                    aiohttp.ClientError,
+                    aiohttp.ServerTimeoutError,
+                    aiohttp.ServerDisconnectedError,
+                    aiohttp.ServerConnectionError,
+                    aiohttp.ClientConnectionError,
+                ):
+                    logger.warning(
+                        f"Error connecting to {server_endpoint}! Retrying..."
+                    )
                     await asyncio.sleep(1)
             await asyncio.sleep(polling_interval)
 
     async def __task_manager(self, event: Event):
         task = asyncio.create_task(self.events_handlers.handle(event))
         self.running_tasks.add(task)
         task.add_done_callback(lambda t: self.running_tasks.remove(t))
```

### Comparing `Shimarin-0.0.8/Shimarin/client/networking.py` & `Shimarin-0.0.9/Shimarin/client/networking.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,15 +21,17 @@
     """
     response: typing.Union[Response, None] = None
     async with session.request("GET", *args, **kwargs) as resp:
         response = Response(resp.status, await resp.read())
     return response
 
 
-async def send_post_request(session: aiohttp.ClientSession, *args, **kwargs) -> Response:
+async def send_post_request(
+    session: aiohttp.ClientSession, *args, **kwargs
+) -> Response:
     """
     Function to send a rest request and return the Response
     :session A client session object from aiohttp
     :param *args and *kwargs to be used on the request
     :return a Response object with the content of the endpoint
     """
     response: typing.Union[Response, None] = None
```

### Comparing `Shimarin-0.0.8/Shimarin/server/events.py` & `Shimarin-0.0.9/Shimarin/server/events.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,88 +1,108 @@
 import asyncio
 import inspect
 import uuid
 from datetime import datetime
 from typing import Callable, Any
 
+from .exceptions import EventAnswerTimeoutError
+
 
 class Event:
-    def __init__(self, event_type: str, payload: str = None, callback: Callable |  None = None):
+    def __init__(
+        self, event_type: str, payload: str = None, callback: Callable | None = None
+    ):
         self.event_type = event_type
         self.payload = payload
         self.callback = callback
         self.identifier = str(uuid.uuid1())
         self.answered = True if callback is None else False
         self.__answer = ""
         self.__creation_date = datetime.now()
         self.done = False
         self.delete = False  # this config will be used later when callbacks are merged into emitter
 
     @staticmethod
-    def new(event_type: str, payload: str = None, callback: Callable |  None = None) -> 'Event':
+    def new(
+        event_type: str, payload: str = None, callback: Callable | None = None
+    ) -> "Event":
         return Event(event_type, payload, callback)
-    
+
     @property
     def age(self):
-        return datetime.now() - self.__creation_date
-    
+        return (datetime.now() - self.__creation_date).total_seconds()
+
     @property
     def answer(self):
         self.done = True
         return self.__answer
-    
-    async def get_answer(self):
+
+    async def get_answer(self, timeout: float = 0):
+        start = datetime.now()
         while self.answered is False:
             await asyncio.sleep(0)
+            if (datetime.now() - start).total_seconds() >= timeout:
+                raise EventAnswerTimeoutError
         return self.answer
 
     def json(self) -> dict:
         return {
             "event_type": self.event_type,
             "payload": self.payload,
-            "identifier": self.identifier
+            "identifier": self.identifier,
         }
-    
+
     def __repr__(self):
         return self.json().__str__()
-    
+
     async def trigger(self, payload: Any):
         self.answered = True
         if inspect.iscoroutinefunction(self.callback):
             self.__answer = await self.callback(payload)
         else:
             self.__answer = self.callback(payload)
         return self.__answer
 
 
-class EventEmitter:
+class CallbacksHandlers:
     def __init__(self):
         self.events: list[Event] = []
 
-    async def fetch_event(self, last: bool = True) -> Event:
-        try:
-            return self.events.pop(0 if not last else -1)
-        except IndexError:
-            return Event(None, None, None)
-        
-    async def send(self, event: Event) -> None:
+    async def register(self, event: Event):
         self.events.append(event)
 
+    async def handle(self, unique_identifier: str, payload: Any):
+        for event in self.events:
+            if event.identifier == unique_identifier:
+                return await event.trigger(payload)
+
 
-class CallbacksHandlers:
-    def __init__(self):
+class EventEmitter:
+    def __init__(self, max_age_seconds: float = 0):
         self.events: list[Event] = []
+        self.handlers = CallbacksHandlers()
+        self.max_age_seconds = max_age_seconds
 
-    async def clear_done(self):
+    async def clean_old_items(self):
         for event in self.events.copy():
-            if event.done:
+            if event.done or ((event.age >= self.max_age_seconds) if (self.max_age_seconds > 0) else False):
                 self.events.remove(event)
+        for event in self.handlers.events.copy():
+            if event.done or ((event.age >= self.max_age_seconds) if (self.max_age_seconds > 0) else False):
+                self.handlers.events.remove(event)
 
-    async def register(self, event: Event):
-        await self.clear_done()
+    async def fetch_event(self, last: bool = True) -> Event:
+        await self.clean_old_items()
+        try:
+            item = self.events.pop(0 if not last else -1)
+            await self.handlers.register(item)
+            return item
+        except IndexError:
+            return Event(None, None, None)
+
+    async def send(self, event: Event) -> None:
+        await self.clean_old_items()
         self.events.append(event)
 
     async def handle(self, unique_identifier: str, payload: Any):
-        await self.clear_done()
-        for event in self.events:
-            if event.identifier == unique_identifier:
-                return await event.trigger(payload)
+        await self.clean_old_items()
+        return await self.handlers.handle(unique_identifier, payload)
```

### Comparing `Shimarin-0.0.8/Shimarin.egg-info/PKG-INFO` & `Shimarin-0.0.9/Shimarin.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Shimarin
-Version: 0.0.8
+Version: 0.0.9
 Summary: asynchronous event-based communication between client and server
 Home-page: 
 Author: Kamuri Amorim
 Author-email: myk.gata14@gmail.com
 License: MIT
 Keywords: python events client server asynchronous
 Description-Content-Type: text/markdown
```

