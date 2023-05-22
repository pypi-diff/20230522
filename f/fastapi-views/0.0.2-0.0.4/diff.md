# Comparing `tmp/fastapi_views-0.0.2.tar.gz` & `tmp/fastapi_views-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi_views-0.0.2.tar", max compression
+gzip compressed data, was "fastapi_views-0.0.4.tar", max compression
```

## Comparing `fastapi_views-0.0.2.tar` & `fastapi_views-0.0.4.tar`

### file list

```diff
@@ -1,27 +1,29 @@
--rw-r--r--   0        0        0    11357 2023-04-06 09:52:57.767655 fastapi_views-0.0.2/LICENSE
--rw-r--r--   0        0        0     1983 2023-04-06 09:52:57.767655 fastapi_views-0.0.2/README.md
--rw-r--r--   0        0        0      593 2023-04-06 09:52:57.767655 fastapi_views-0.0.2/fastapi_views/__init__.py
--rw-r--r--   0        0        0       22 2023-04-06 09:52:57.767655 fastapi_views-0.0.2/fastapi_views/_version.py
--rw-r--r--   0        0        0     1792 2023-04-06 09:52:57.767655 fastapi_views-0.0.2/fastapi_views/config.py
--rw-r--r--   0        0        0      479 2023-04-06 09:52:57.767655 fastapi_views-0.0.2/fastapi_views/errors/__init__.py
--rw-r--r--   0        0        0      449 2023-04-06 09:52:57.767655 fastapi_views-0.0.2/fastapi_views/errors/exceptions.py
--rw-r--r--   0        0        0     1253 2023-04-06 09:52:57.767655 fastapi_views-0.0.2/fastapi_views/errors/handlers.py
--rw-r--r--   0        0        0     1811 2023-04-06 09:52:57.767655 fastapi_views-0.0.2/fastapi_views/errors/models.py
--rw-r--r--   0        0        0      986 2023-04-06 09:52:57.767655 fastapi_views-0.0.2/fastapi_views/errors/utils.py
--rw-r--r--   0        0        0     1634 2023-04-06 09:52:57.767655 fastapi_views-0.0.2/fastapi_views/healthcheck.py
--rw-r--r--   0        0        0      331 2023-04-06 09:52:57.767655 fastapi_views-0.0.2/fastapi_views/openapi.py
--rw-r--r--   0        0        0      655 2023-04-06 09:52:57.767655 fastapi_views-0.0.2/fastapi_views/prometheus.py
--rw-r--r--   0        0        0        0 2023-04-06 09:52:57.767655 fastapi_views-0.0.2/fastapi_views/py.typed
--rw-r--r--   0        0        0      413 2023-04-06 09:52:57.767655 fastapi_views-0.0.2/fastapi_views/response.py
--rw-r--r--   0        0        0      293 2023-04-06 09:52:57.767655 fastapi_views-0.0.2/fastapi_views/routers.py
--rw-r--r--   0        0        0      741 2023-04-06 09:52:57.767655 fastapi_views-0.0.2/fastapi_views/serializer.py
--rw-r--r--   0        0        0     2063 2023-04-06 09:52:57.767655 fastapi_views-0.0.2/fastapi_views/settings.py
--rw-r--r--   0        0        0      745 2023-04-06 09:52:57.767655 fastapi_views-0.0.2/fastapi_views/types.py
--rw-r--r--   0        0        0        0 2023-04-06 09:52:57.767655 fastapi_views-0.0.2/fastapi_views/views/__init__.py
--rw-r--r--   0        0        0    11545 2023-04-06 09:52:57.767655 fastapi_views-0.0.2/fastapi_views/views/api.py
--rw-r--r--   0        0        0     1406 2023-04-06 09:52:57.767655 fastapi_views-0.0.2/fastapi_views/views/functools.py
--rw-r--r--   0        0        0     6888 2023-04-06 09:52:57.767655 fastapi_views-0.0.2/fastapi_views/views/generics.py
--rw-r--r--   0        0        0     1367 2023-04-06 09:52:57.767655 fastapi_views-0.0.2/fastapi_views/views/mixins.py
--rw-r--r--   0        0        0     1631 2023-04-06 09:52:57.767655 fastapi_views-0.0.2/fastapi_views/views/viewsets.py
--rw-r--r--   0        0        0     1561 2023-04-06 09:52:57.771655 fastapi_views-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     2604 1970-01-01 00:00:00.000000 fastapi_views-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-22 09:02:02.788504 fastapi_views-0.0.4/LICENSE
+-rw-r--r--   0        0        0     2159 2023-05-22 09:02:02.788504 fastapi_views-0.0.4/README.md
+-rw-r--r--   0        0        0      760 2023-05-22 09:02:02.796504 fastapi_views-0.0.4/fastapi_views/__init__.py
+-rw-r--r--   0        0        0       22 2023-05-22 09:02:02.796504 fastapi_views-0.0.4/fastapi_views/_version.py
+-rw-r--r--   0        0        0     1320 2023-05-22 09:02:02.796504 fastapi_views-0.0.4/fastapi_views/config.py
+-rw-r--r--   0        0        0     1421 2023-05-22 09:02:02.796504 fastapi_views-0.0.4/fastapi_views/enum.py
+-rw-r--r--   0        0        0      479 2023-05-22 09:02:02.796504 fastapi_views-0.0.4/fastapi_views/errors/__init__.py
+-rw-r--r--   0        0        0      449 2023-05-22 09:02:02.796504 fastapi_views-0.0.4/fastapi_views/errors/exceptions.py
+-rw-r--r--   0        0        0     1238 2023-05-22 09:02:02.796504 fastapi_views-0.0.4/fastapi_views/errors/handlers.py
+-rw-r--r--   0        0        0     1811 2023-05-22 09:02:02.796504 fastapi_views-0.0.4/fastapi_views/errors/models.py
+-rw-r--r--   0        0        0      986 2023-05-22 09:02:02.796504 fastapi_views-0.0.4/fastapi_views/errors/utils.py
+-rw-r--r--   0        0        0     2001 2023-05-22 09:02:02.796504 fastapi_views-0.0.4/fastapi_views/healthcheck.py
+-rw-r--r--   0        0        0     1795 2023-05-22 09:02:02.796504 fastapi_views-0.0.4/fastapi_views/models.py
+-rw-r--r--   0        0        0      331 2023-05-22 09:02:02.796504 fastapi_views-0.0.4/fastapi_views/openapi.py
+-rw-r--r--   0        0        0      663 2023-05-22 09:02:02.796504 fastapi_views-0.0.4/fastapi_views/prometheus.py
+-rw-r--r--   0        0        0        0 2023-05-22 09:02:02.796504 fastapi_views-0.0.4/fastapi_views/py.typed
+-rw-r--r--   0        0        0      413 2023-05-22 09:02:02.796504 fastapi_views-0.0.4/fastapi_views/response.py
+-rw-r--r--   0        0        0     1338 2023-05-22 09:02:02.796504 fastapi_views-0.0.4/fastapi_views/routers.py
+-rw-r--r--   0        0        0     2051 2023-05-22 09:02:02.796504 fastapi_views-0.0.4/fastapi_views/settings.py
+-rw-r--r--   0        0        0     1121 2023-05-22 09:02:02.796504 fastapi_views-0.0.4/fastapi_views/types.py
+-rw-r--r--   0        0        0      881 2023-05-22 09:02:02.796504 fastapi_views-0.0.4/fastapi_views/utils.py
+-rw-r--r--   0        0        0      263 2023-05-22 09:02:02.796504 fastapi_views-0.0.4/fastapi_views/views/__init__.py
+-rw-r--r--   0        0        0    18045 2023-05-22 09:02:02.796504 fastapi_views-0.0.4/fastapi_views/views/api.py
+-rw-r--r--   0        0        0     2126 2023-05-22 09:02:02.796504 fastapi_views-0.0.4/fastapi_views/views/functools.py
+-rw-r--r--   0        0        0    13755 2023-05-22 09:02:02.796504 fastapi_views-0.0.4/fastapi_views/views/generics.py
+-rw-r--r--   0        0        0     1837 2023-05-22 09:02:02.796504 fastapi_views-0.0.4/fastapi_views/views/mixins.py
+-rw-r--r--   0        0        0     4355 2023-05-22 09:02:02.796504 fastapi_views-0.0.4/fastapi_views/views/viewsets.py
+-rw-r--r--   0        0        0     1629 2023-05-22 09:02:02.796504 fastapi_views-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     2816 1970-01-01 00:00:00.000000 fastapi_views-0.0.4/PKG-INFO
```

### Comparing `fastapi_views-0.0.2/LICENSE` & `fastapi_views-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `fastapi_views-0.0.2/README.md` & `fastapi_views-0.0.4/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 ![Mypy](https://img.shields.io/badge/mypy-checked-blue)
 ![Code Style](https://img.shields.io/badge/code%20style-black-000000.svg)
 [![security: bandit](https://img.shields.io/badge/security-bandit-yellow.svg)](https://github.com/PyCQA/bandit)
 
 *FastAPI Class Views and utilities*
 
 ---
-Version: 0.0.2
+Version: 0.0.4
 
 Documentation: https://performancemedia.github.io/fastapi-views/
 
 Repository: https://github.com/performancemedia/fastapi-views
 
 ---
 
@@ -29,32 +29,32 @@
 
 ## Usage
 
 ```python
 from typing import Optional
 from uuid import UUID
 
-from fastapi_views import Serializer
-from fastapi_views.views.api import L
-from fastapi_views.views.viewsets import APIViewSet
+from fastapi_views import Serializer, ViewRouter
+from fastapi_views.views.viewsets import AsyncAPIViewSet
 
 
 class ItemSchema(Serializer):
     id: UUID
     name: str
     price: int
 
 
 items = {}
 
 
-class MyView(APIViewSet):
+class MyViewSet(AsyncAPIViewSet):
+    api_component_name = "Item"
     serializer = ItemSchema
-
-    async def list(self, *args, **kwargs) -> L:
+    
+    async def list(self):
         return list(items.values())
 
     async def create(self, item: ItemSchema) -> ItemSchema:
         items[item.id] = item
         return item
 
     async def retrieve(self, id: UUID) -> Optional[ItemSchema]:
@@ -62,20 +62,27 @@
 
     async def update(self, item: ItemSchema):
         items[item.id] = item
 
     async def destroy(self, id: UUID) -> None:
         items.pop(id, None)
 
+router = ViewRouter(prefix="/items")
+router.register_view(MyViewSet)
+# in app.py
+# app.include_router(router)
+
 ```
 
 ## Features
 
 - Class Based Views
   - APIViews
   - GenericViews
   - ViewSets
+- Both async and sync function support
+- No dependencies on ORM
 - Openapi id simplification
 - 'Smart' and fast serialization using orjson
 - Http Problem Details implementation
 - Automatic prometheus metrics exporter
 - Pluggable healthcheck helper
```

### Comparing `fastapi_views-0.0.2/fastapi_views/config.py` & `fastapi_views-0.0.4/fastapi_views/config.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,53 +1,37 @@
 from __future__ import annotations
 
-import asyncio
-from typing import Sequence
-
 from fastapi import FastAPI
 
 from .errors import ServiceUnavailableAPIError, add_error_handlers
 from .healthcheck import HealthCheck
 from .openapi import simplify_operation_ids
 from .prometheus import add_prometheus_middleware
 from .settings import APISettings
-from .types import SideService
-
-
-def add_side_services(app: FastAPI, services: Sequence[SideService]) -> None:
-    @app.on_event("startup")
-    async def start_side_services():
-        await asyncio.gather(*[s.start() for s in services])
-
-    @app.on_event("shutdown")
-    async def stop_side_services():
-        await asyncio.gather(*[s.stop() for s in services])
 
 
 def configure_app(
     app: FastAPI,
     enable_error_handlers: bool = True,
     healthcheck: HealthCheck | None = None,
     enable_prometheus_middleware: bool = True,
-    side_services: Sequence[SideService] | None = None,
     simplify_openapi_ids: bool = True,
 ):
     if enable_error_handlers:
         add_error_handlers(app)
     if healthcheck:
         app.add_api_route(
             methods=["GET"],
             path=healthcheck.endpoint,
             endpoint=healthcheck.get_endpoint,
+            include_in_schema=healthcheck.include_in_schema,
             responses={503: {"model": ServiceUnavailableAPIError}},
         )
     if enable_prometheus_middleware:
         add_prometheus_middleware(app)
-    if side_services:
-        add_side_services(app, side_services)
     if simplify_openapi_ids:
         simplify_operation_ids(app)
 
 
 def create_fastapi_app(settings: APISettings, **kwargs) -> FastAPI:
     app = FastAPI(**settings.fastapi_kwargs, **kwargs)
     configure_app(app, **settings.config_kwargs)
```

### Comparing `fastapi_views-0.0.2/fastapi_views/errors/handlers.py` & `fastapi_views-0.0.4/fastapi_views/errors/handlers.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from fastapi import Request
-from fastapi.responses import ORJSONResponse
 from starlette.status import HTTP_500_INTERNAL_SERVER_ERROR
 
+from ..response import JsonResponse
 from .exceptions import APIError
 from .models import ErrorDetails, InternalServerAPIError
 from .utils import find_model_for_exc
 
 
 def api_error_handler(request: Request, exc: APIError):
-    return ORJSONResponse(
+    return JsonResponse(
         status_code=exc.status,
         content=ErrorDetails(
             detail=exc.detail,
             title=exc.title,
             status=exc.status,
             instance=exc.instance or request.url.path,
         ).dict(),
@@ -20,16 +20,16 @@
 
 
 def exception_handler(request, exc: Exception):
     model_cls = find_model_for_exc(type(exc).__name__)
     detail = getattr(exc, "detail", str(exc))
     if model_cls:
         model = model_cls(detail=detail, instance=request.url.path)
-        return ORJSONResponse(status_code=model.status, content=model.dict())
-    return ORJSONResponse(
+        return JsonResponse(status_code=model.status, content=model.dict())
+    return JsonResponse(
         status_code=HTTP_500_INTERNAL_SERVER_ERROR,
         content=InternalServerAPIError(
             detail=detail,
             instance=request.url.path,
         ).dict(),
     )
```

### Comparing `fastapi_views-0.0.2/fastapi_views/errors/models.py` & `fastapi_views-0.0.4/fastapi_views/errors/models.py`

 * *Files identical despite different names*

### Comparing `fastapi_views-0.0.2/fastapi_views/errors/utils.py` & `fastapi_views-0.0.4/fastapi_views/errors/utils.py`

 * *Files identical despite different names*

### Comparing `fastapi_views-0.0.2/fastapi_views/healthcheck.py` & `fastapi_views-0.0.4/fastapi_views/healthcheck.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,32 +1,40 @@
 from __future__ import annotations
 
 import asyncio
+import logging
 from typing import Any, Callable
 
 from starlette.status import HTTP_200_OK, HTTP_503_SERVICE_UNAVAILABLE
 
 from .errors import ServiceUnavailableAPIError
 from .response import JsonResponse
 
 
+async def _simple_healthcheck() -> bool:
+    return True
+
+
 class HealthCheck:
     """
     Group of functions that perform basic health checks of the application
     """
 
     def __init__(
         self,
         endpoint: str = "/healthz",
         checks: list[Callable[[], Any]] | None = None,
         response_class=JsonResponse,
+        include_in_schema: bool = False,
     ):
         self.endpoint = endpoint
         self.response_class = response_class
-        self.checks = checks or []
+        self.checks = checks or [_simple_healthcheck]
+        self.include_in_schema = include_in_schema
+        self.logger = logging.getLogger(type(self).__name__)
 
     def add_check(self, func):
         self.checks.append(func)
 
     def register(self):
         def wrapper(func):
             self.add_check(func)
@@ -35,22 +43,25 @@
         return wrapper
 
     async def get_endpoint(self):
         failed = False
         task = asyncio.gather(*[t() for t in self.checks], return_exceptions=True)
         try:
             results = await asyncio.wait_for(task, timeout=10)
-            if any(isinstance(r, Exception) for r in results):
-                failed = True
+            for r in results:
+                if isinstance(r, Exception):
+                    self.logger.warning(f"Healthcheck failed with exc: {r}")
+                    failed = True
+                    break
         except asyncio.TimeoutError:
             failed = True
         finally:
             if failed:
                 return self.response_class(
                     content=ServiceUnavailableAPIError(
-                        detail="Service health check failed"
+                        detail="Service liveness probe failed"
                     ).dict(),
                     status_code=HTTP_503_SERVICE_UNAVAILABLE,
                 )
             return self.response_class(
                 content={"status": "ok"}, status_code=HTTP_200_OK
             )
```

### Comparing `fastapi_views-0.0.2/fastapi_views/prometheus.py` & `fastapi_views-0.0.4/fastapi_views/prometheus.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-import os
+import socket
 from typing import Any
 
 from fastapi import FastAPI
 
 
 def add_prometheus_middleware(
     app: FastAPI, endpoint: str = "/metrics", **kwargs: Any
 ) -> None:
     from starlette_exporter import PrometheusMiddleware, handle_metrics
 
-    kwargs.setdefault("app", app.title.lower().replace(" ", "_"))
+    kwargs.setdefault("app_name", app.title.lower().replace(" ", "_"))
     kwargs.setdefault("skip_paths", ["/healthz", "/docs", "/openapi.json", "/metrics"])
     kwargs.setdefault("group_paths", True)
-    kwargs.setdefault("labels", {"server": os.getenv("HOSTNAME")})
+    kwargs.setdefault("labels", {"server": socket.gethostname()})
     kwargs.setdefault("always_use_int_status", True)
     app.add_middleware(PrometheusMiddleware, **kwargs)
     app.add_route(endpoint, handle_metrics)
```

### Comparing `fastapi_views-0.0.2/fastapi_views/settings.py` & `fastapi_views-0.0.4/fastapi_views/settings.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Any, Dict, List, Optional
+from typing import Any, Optional
 
 from pydantic import BaseSettings, Field, PyObject
 
 
 class APISettings(BaseSettings):
 
     # fastapi.applications.FastAPI initializer kwargs
@@ -16,19 +16,19 @@
 
     # Custom settings
     disable_docs: bool = Field(False, env="DISABLE_DOCS")
 
     enable_error_handlers: bool = Field(True, env="ERROR_HANDLERS_ENABLE")
     enable_prometheus_middleware: bool = Field(True, env="PROMETHEUS_MIDDLEWARE_ENABLE")
     healthcheck: Optional[PyObject] = None
-    side_services: List[PyObject] = []
+    side_services: list[PyObject] = []
     simplify_openapi_ids: bool = True
 
     @property
-    def fastapi_kwargs(self) -> Dict[str, Any]:
+    def fastapi_kwargs(self) -> dict[str, Any]:
         """
         This returns a dictionary of the most commonly used keyword arguments when initializing a FastAPI instance
         If `self.disable_docs` is True, the various docs-related arguments are disabled, preventing your spec from being
         published.
         """
         fastapi_kwargs = {
             "debug": self.debug,
@@ -42,15 +42,15 @@
         if self.disable_docs:
             fastapi_kwargs.update(
                 {"docs_url": None, "openapi_url": None, "redoc_url": None}
             )
         return fastapi_kwargs
 
     @property
-    def config_kwargs(self) -> Dict[str, Any]:
+    def config_kwargs(self) -> dict[str, Any]:
         return {
             "enable_error_handlers": self.enable_error_handlers,
             "healthcheck": self.healthcheck,
             "enable_prometheus_middleware": self.enable_prometheus_middleware,
             "side_services": self.side_services,
             "simplify_openapi_ids": self.simplify_openapi_ids,
         }
```

### Comparing `fastapi_views-0.0.2/fastapi_views/views/functools.py` & `fastapi_views-0.0.4/fastapi_views/views/functools.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,54 +1,76 @@
+from __future__ import annotations
+
+import asyncio
 import functools
-from typing import Any, Callable, Tuple, Type, Union
+from typing import TYPE_CHECKING, Any, Callable
 
-from fastapi_views.views.mixins import ErrorHandlerMixin
+if TYPE_CHECKING:
+    from fastapi_views.views.mixins import ErrorHandlerMixin
 
 VIEWSET_ROUTE_FLAG = "_is_viewset_route"
 
 
 def override(**kwargs):
     def wrapper(func):
         setattr(func, "kwargs", kwargs)
         return func
 
     return wrapper
 
 
-def route(**kwargs: Any) -> Callable:
+def route(path: str, **kwargs: Any) -> Callable:
     def wrapper(func: Callable):
         setattr(func, VIEWSET_ROUTE_FLAG, True)
-        return override(**kwargs)(func)
+        return override(path=path, **kwargs)(func)
 
     return wrapper
 
 
-def catch(exc_type: Union[Type[Exception], Tuple[Type[Exception]]], **kw: Any):
+def catch(exc_type: type[Exception] | tuple[type[Exception]], **kw: Any):
     def wrapper(func):
         @functools.wraps(func)
-        async def wrapped(self, *args, **kwargs):
+        async def wrapped_async(self, *args, **kwargs):
             try:
                 return await func(self, *args, **kwargs)
             except exc_type as e:
                 self.handle_error(exc_type, e, **kw)
 
-        return wrapped
+        @functools.wraps(func)
+        def wrapped_sync(self, *args, **kwargs):
+            try:
+                return func(self, *args, **kwargs)
+            except exc_type as e:
+                self.handle_error(exc_type, e, **kw)
+
+        if asyncio.iscoroutinefunction(func):
+            return wrapped_async
+        return wrapped_sync
 
     return wrapper
 
 
 def catch_defined(func):
     @functools.wraps(func)
-    async def wrapped(self: ErrorHandlerMixin, *args, **kwargs):
+    async def wrapped_async(self: ErrorHandlerMixin, *args, **kwargs):
         try:
             return await func(self, *args, **kwargs)
         except self.catches as e:
             self.handle_error(type(e), e)
 
-    return wrapped
+    @functools.wraps(func)
+    def wrapped_sync(self: ErrorHandlerMixin, *args, **kwargs):
+        try:
+            return func(self, *args, **kwargs)
+        except self.catches as e:
+            self.handle_error(type(e), e)
+
+    if asyncio.iscoroutinefunction(func):
+        return wrapped_async
+    return wrapped_sync
 
 
 get = functools.partial(route, methods=["GET"])
 post = functools.partial(route, methods=["POST"])
 put = functools.partial(route, methods=["PUT"])
 patch = functools.partial(route, methods=["PATCH"])
 delete = functools.partial(route, methods=["DELETE"])
```

### Comparing `fastapi_views-0.0.2/fastapi_views/views/mixins.py` & `fastapi_views-0.0.4/fastapi_views/views/mixins.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,20 @@
 from __future__ import annotations
 
-from typing import Any, Callable
+from typing import Any, Callable, Generic, TypeVar, Union
+from uuid import UUID
 
 from fastapi import Request
+from pydantic import BaseModel
 from starlette.status import HTTP_400_BAD_REQUEST, HTTP_404_NOT_FOUND
 
 from ..errors import APIError
+from ..types import AsyncRepository, Repository
+
+R = TypeVar("R", bound=Union[AsyncRepository, Repository])
 
 
 class DetailViewMixin:
     detail_route: str = "/{id}"
     raise_on_none: bool = True
     request: Request
     get_name: Callable[..., str]
@@ -24,27 +29,42 @@
 
 class _Sentinel(Exception):
     pass
 
 
 class ErrorHandlerMixin:
     request: Request
-    default_error_message = {
-        "detail": "Something went wrong",
-        "status": HTTP_400_BAD_REQUEST,
-    }
 
     catch: dict[type[Exception], dict[str, Any]] = {}
 
     def get_error_message(self, key: type[Exception]):
-        return self.catch.get(key) or self.default_error_message
+        return self.catch.get(
+            key, {"detail": "Something went wrong", "status": HTTP_400_BAD_REQUEST}
+        )
 
     def handle_error(self, exc_type: type[Exception], exc: Exception, **kwargs):
         kwargs.update(**self.get_error_message(exc_type))
         kwargs.setdefault("instance", self.request.url.path)
         kwargs.setdefault("title", exc_type.__name__)
         kwargs.setdefault("detail", str(exc))
         raise APIError(**kwargs)
 
     @property
     def catches(self):
         return tuple(self.catch.keys()) or _Sentinel
+
+
+class IdModel(BaseModel):
+    id: UUID
+
+
+class GenericViewMixin(ErrorHandlerMixin, Generic[R]):
+    repository: R
+    params: type[BaseModel] = BaseModel
+
+    @classmethod
+    def get_params(cls, action: str):
+        return cls.params
+
+
+class GenericDetailViewMixin(GenericViewMixin[R], DetailViewMixin):
+    pk: type[BaseModel] = IdModel
```

### Comparing `fastapi_views-0.0.2/pyproject.toml` & `fastapi_views-0.0.4/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,35 +1,39 @@
 [tool.poetry]
 name = "fastapi-views"
-version = "0.0.2"
+version = "0.0.4"
 description = "FastAPI Class Views and utilities"
 authors = ["Radzim Kowalow <radzim.kowalow@performance-media.pl>"]
 readme = "README.md"
 packages = [{include = "fastapi_views"}]
 
 [tool.poetry.dependencies]
-python = ">=3.8.1,<4.0"
+python = ">=3.9,<4.0"
 fastapi = "^0.95.0"
-orjson = "^3.8.9"
-uvicorn = "^0.21.1"
-starlette-exporter = "^0.15.1"
+orjson = ">=3.2.1,<=3.8.9"
+uvicorn = "^0.22.0"
+uvloop = "^0.17.0"
+starlette-exporter = "^0.16"
+
 
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2.1"
 pytest-asyncio = "^0.20.2"
 pytest-cov = "^4.0.0"
-mypy = "^0.961"
 black = "^22.3.0"
 flake8 = "^6.0.0"
 isort = "^5.10.1"
 tox = "^3.25.0"
 bandit = "^1.7.4"
 python-semantic-release = "^7.33.2"
 flake8-cognitive-complexity = "^0.1.0"
+httpx = "^0.24.0"
+asgi-lifespan = "^2.1.0"
+mypy = "^1.2.0"
 
 [tool.poetry.group.docs.dependencies]
 mkdocs = "^1.4.2"
 mkdocs-material = "^8.2.1"
 mkdocs-autorefs = "^0.4.1"
 mkdocs-gen-files = "^0.4.0"
 mkdocstrings-python = "^0.8.2"
```

### Comparing `fastapi_views-0.0.2/PKG-INFO` & `fastapi_views-0.0.4/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: fastapi-views
-Version: 0.0.2
+Version: 0.0.4
 Summary: FastAPI Class Views and utilities
 Author: Radzim Kowalow
 Author-email: radzim.kowalow@performance-media.pl
-Requires-Python: >=3.8.1,<4.0
+Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: fastapi (>=0.95.0,<0.96.0)
-Requires-Dist: orjson (>=3.8.9,<4.0.0)
-Requires-Dist: starlette-exporter (>=0.15.1,<0.16.0)
-Requires-Dist: uvicorn (>=0.21.1,<0.22.0)
+Requires-Dist: orjson (>=3.2.1,<=3.8.9)
+Requires-Dist: starlette-exporter (>=0.16,<0.17)
+Requires-Dist: uvicorn (>=0.22.0,<0.23.0)
+Requires-Dist: uvloop (>=0.17.0,<0.18.0)
 Description-Content-Type: text/markdown
 
 # fastapi-views
 
 ![CI](https://github.com/performancemedia/fastapi-views/workflows/CI/badge.svg)
 ![Build](https://github.com/performancemedia/fastapi-views/workflows/Publish/badge.svg)
 ![License](https://img.shields.io/github/license/performancemedia/fastapi-views)
@@ -26,15 +27,15 @@
 ![Mypy](https://img.shields.io/badge/mypy-checked-blue)
 ![Code Style](https://img.shields.io/badge/code%20style-black-000000.svg)
 [![security: bandit](https://img.shields.io/badge/security-bandit-yellow.svg)](https://github.com/PyCQA/bandit)
 
 *FastAPI Class Views and utilities*
 
 ---
-Version: 0.0.2
+Version: 0.0.4
 
 Documentation: https://performancemedia.github.io/fastapi-views/
 
 Repository: https://github.com/performancemedia/fastapi-views
 
 ---
 
@@ -46,32 +47,32 @@
 
 ## Usage
 
 ```python
 from typing import Optional
 from uuid import UUID
 
-from fastapi_views import Serializer
-from fastapi_views.views.api import L
-from fastapi_views.views.viewsets import APIViewSet
+from fastapi_views import Serializer, ViewRouter
+from fastapi_views.views.viewsets import AsyncAPIViewSet
 
 
 class ItemSchema(Serializer):
     id: UUID
     name: str
     price: int
 
 
 items = {}
 
 
-class MyView(APIViewSet):
+class MyViewSet(AsyncAPIViewSet):
+    api_component_name = "Item"
     serializer = ItemSchema
-
-    async def list(self, *args, **kwargs) -> L:
+    
+    async def list(self):
         return list(items.values())
 
     async def create(self, item: ItemSchema) -> ItemSchema:
         items[item.id] = item
         return item
 
     async def retrieve(self, id: UUID) -> Optional[ItemSchema]:
@@ -79,21 +80,28 @@
 
     async def update(self, item: ItemSchema):
         items[item.id] = item
 
     async def destroy(self, id: UUID) -> None:
         items.pop(id, None)
 
+router = ViewRouter(prefix="/items")
+router.register_view(MyViewSet)
+# in app.py
+# app.include_router(router)
+
 ```
 
 ## Features
 
 - Class Based Views
   - APIViews
   - GenericViews
   - ViewSets
+- Both async and sync function support
+- No dependencies on ORM
 - Openapi id simplification
 - 'Smart' and fast serialization using orjson
 - Http Problem Details implementation
 - Automatic prometheus metrics exporter
 - Pluggable healthcheck helper
```

