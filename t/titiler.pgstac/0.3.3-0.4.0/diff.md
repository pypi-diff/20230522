# Comparing `tmp/titiler.pgstac-0.3.3.tar.gz` & `tmp/titiler.pgstac-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "titiler.pgstac-0.3.3.tar", last modified: Thu Apr 27 22:41:45 2023, max compression
+gzip compressed data, was "titiler.pgstac-0.4.0.tar", last modified: Mon May 22 19:15:37 2023, max compression
```

## Comparing `titiler.pgstac-0.3.3.tar` & `titiler.pgstac-0.4.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1097 2023-04-27 22:41:06.687272 titiler.pgstac-0.3.3/LICENSE
--rw-r--r--   0        0        0     4451 2023-04-27 22:41:06.687272 titiler.pgstac-0.3.3/README.md
--rw-r--r--   0        0        0     2628 2023-04-27 22:41:06.795274 titiler.pgstac-0.3.3/pyproject.toml
--rw-r--r--   0        0        0       44 2023-04-27 22:41:06.799274 titiler.pgstac-0.3.3/titiler/pgstac/__init__.py
--rw-r--r--   0        0        0      874 2023-04-27 22:41:06.799274 titiler.pgstac-0.3.3/titiler/pgstac/db.py
--rw-r--r--   0        0        0     3936 2023-04-27 22:41:06.799274 titiler.pgstac-0.3.3/titiler/pgstac/dependencies.py
--rw-r--r--   0        0        0    39829 2023-04-27 22:41:06.799274 titiler.pgstac-0.3.3/titiler/pgstac/factory.py
--rw-r--r--   0        0        0       91 2023-04-27 22:41:06.799274 titiler.pgstac-0.3.3/titiler/pgstac/logger.py
--rw-r--r--   0        0        0     3860 2023-04-27 22:41:06.799274 titiler.pgstac-0.3.3/titiler/pgstac/main.py
--rw-r--r--   0        0        0     6797 2023-04-27 22:41:06.799274 titiler.pgstac-0.3.3/titiler/pgstac/model.py
--rw-r--r--   0        0        0    12681 2023-04-27 22:41:06.799274 titiler.pgstac-0.3.3/titiler/pgstac/mosaic.py
--rw-r--r--   0        0        0     2642 2023-04-27 22:41:06.799274 titiler.pgstac-0.3.3/titiler/pgstac/reader.py
--rw-r--r--   0        0        0     3518 2023-04-27 22:41:06.799274 titiler.pgstac-0.3.3/titiler/pgstac/settings.py
--rw-r--r--   0        0        0      834 2023-04-27 22:41:06.799274 titiler.pgstac-0.3.3/titiler/pgstac/utils.py
--rw-r--r--   0        0        0     5671 1970-01-01 00:00:00.000000 titiler.pgstac-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0     1097 2023-05-22 19:15:07.041101 titiler.pgstac-0.4.0/LICENSE
+-rw-r--r--   0        0        0     4451 2023-05-22 19:15:07.041101 titiler.pgstac-0.4.0/README.md
+-rw-r--r--   0        0        0     2618 2023-05-22 19:15:07.149102 titiler.pgstac-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0       44 2023-05-22 19:15:07.153102 titiler.pgstac-0.4.0/titiler/pgstac/__init__.py
+-rw-r--r--   0        0        0      874 2023-05-22 19:15:07.153102 titiler.pgstac-0.4.0/titiler/pgstac/db.py
+-rw-r--r--   0        0        0     3936 2023-05-22 19:15:07.153102 titiler.pgstac-0.4.0/titiler/pgstac/dependencies.py
+-rw-r--r--   0        0        0    37682 2023-05-22 19:15:07.153102 titiler.pgstac-0.4.0/titiler/pgstac/factory.py
+-rw-r--r--   0        0        0       91 2023-05-22 19:15:07.153102 titiler.pgstac-0.4.0/titiler/pgstac/logger.py
+-rw-r--r--   0        0        0     3860 2023-05-22 19:15:07.153102 titiler.pgstac-0.4.0/titiler/pgstac/main.py
+-rw-r--r--   0        0        0     6797 2023-05-22 19:15:07.153102 titiler.pgstac-0.4.0/titiler/pgstac/model.py
+-rw-r--r--   0        0        0    12695 2023-05-22 19:15:07.153102 titiler.pgstac-0.4.0/titiler/pgstac/mosaic.py
+-rw-r--r--   0        0        0     2642 2023-05-22 19:15:07.153102 titiler.pgstac-0.4.0/titiler/pgstac/reader.py
+-rw-r--r--   0        0        0     3518 2023-05-22 19:15:07.153102 titiler.pgstac-0.4.0/titiler/pgstac/settings.py
+-rw-r--r--   0        0        0      834 2023-05-22 19:15:07.153102 titiler.pgstac-0.4.0/titiler/pgstac/utils.py
+-rw-r--r--   0        0        0     5671 1970-01-01 00:00:00.000000 titiler.pgstac-0.4.0/PKG-INFO
```

### Comparing `titiler.pgstac-0.3.3/LICENSE` & `titiler.pgstac-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `titiler.pgstac-0.3.3/README.md` & `titiler.pgstac-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `titiler.pgstac-0.3.3/pyproject.toml` & `titiler.pgstac-0.4.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -22,23 +22,23 @@
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Topic :: Scientific/Engineering :: GIS",
 ]
 dependencies = [
-    "titiler.core>=0.10.2,<0.11",
-    "titiler.mosaic>=0.10.2,<0.11",
-    "geojson-pydantic>=0.4,<0.5",
+    "titiler.core>=0.11.6,<0.12",
+    "titiler.mosaic>=0.11.6,<0.12",
+    "geojson-pydantic",
     "stac-pydantic==2.0.*",
-    "fastapi>=0.87,<0.92",
+    "fastapi>=0.87,<0.95",
     "starlette>=0.21.0,<0.25",
 ]
 dynamic = []
-version = "0.3.3"
+version = "0.4.0"
 
 [project.license]
 file = "LICENSE"
 
 [project.optional-dependencies]
 psycopg = [
     "psycopg[pool]",
```

### Comparing `titiler.pgstac-0.3.3/titiler/pgstac/db.py` & `titiler.pgstac-0.4.0/titiler/pgstac/db.py`

 * *Files identical despite different names*

### Comparing `titiler.pgstac-0.3.3/titiler/pgstac/dependencies.py` & `titiler.pgstac-0.4.0/titiler/pgstac/dependencies.py`

 * *Files identical despite different names*

### Comparing `titiler.pgstac-0.3.3/titiler/pgstac/factory.py` & `titiler.pgstac-0.4.0/titiler/pgstac/factory.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 """Custom MosaicTiler Factory for PgSTAC Mosaic Backend."""
 
 import os
 import re
-import time
 from dataclasses import dataclass
 from typing import (
     Any,
     Callable,
     Dict,
     Generator,
     List,
@@ -17,33 +16,32 @@
     Union,
 )
 from urllib.parse import urlencode
 
 import rasterio
 from cogeo_mosaic.backends import BaseBackend
 from cogeo_mosaic.errors import MosaicNotFoundError
-from fastapi import Body, Depends, Path, Query
+from fastapi import Body, Depends, HTTPException, Path, Query
 from geojson_pydantic import Feature, FeatureCollection
 from psycopg import sql
 from psycopg.rows import class_row
 from rio_tiler.constants import MAX_THREADS
 from rio_tiler.models import BandStatistics
 from rio_tiler.utils import get_array_statistics
 from starlette.datastructures import QueryParams
 from starlette.requests import Request
 from starlette.responses import HTMLResponse, Response
 
 from titiler.core.dependencies import (
     AssetsBidxExprParams,
     DefaultDependency,
     HistogramParams,
-    RescalingParams,
     StatisticsParams,
 )
-from titiler.core.factory import BaseTilerFactory, img_endpoint_params, templates
+from titiler.core.factory import BaseTilerFactory, img_endpoint_params
 from titiler.core.models.mapbox import TileJSON
 from titiler.core.models.responses import MultiBaseStatisticsGeoJSON
 from titiler.core.resources.enums import ImageType, MediaType, OptionalHeader
 from titiler.core.resources.responses import GeoJSONResponse, XMLResponse
 from titiler.mosaic.resources.enums import PixelSelectionMethod
 from titiler.pgstac import model
 from titiler.pgstac.dependencies import (
@@ -56,41 +54,14 @@
 
 
 def _first_value(values: List[Any], default: Any = None):
     """Return the first not None value."""
     return next(filter(lambda x: x is not None, values), default)
 
 
-# This code is copied from marblecutter
-#  https://github.com/mojodna/marblecutter/blob/master/marblecutter/stats.py
-# License:
-# Original work Copyright 2016 Stamen Design
-# Modified work Copyright 2016-2017 Seth Fitzsimmons
-# Modified work Copyright 2016 American Red Cross
-# Modified work Copyright 2016-2017 Humanitarian OpenStreetMap Team
-# Modified work Copyright 2017 Mapzen
-class Timer(object):
-    """Time a code block."""
-
-    def __enter__(self):
-        """Starts timer."""
-        self.start = time.time()
-        return self
-
-    def __exit__(self, ty, val, tb):
-        """Stops timer."""
-        self.end = time.time()
-        self.elapsed = self.end - self.start
-
-    @property
-    def from_start(self):
-        """Return time elapsed from start."""
-        return time.time() - self.start
-
-
 @dataclass
 class MosaicTilerFactory(BaseTilerFactory):
     """Custom MosaicTiler for PgSTAC Mosaic Backend."""
 
     reader: Type[BaseBackend] = PGSTACBackend
     path_dependency: Callable[..., str] = PathParams
     layer_dependency: Type[DefaultDependency] = AssetsBidxExprParams
@@ -129,52 +100,14 @@
 
         if self.add_map_viewer:
             self._map_routes()
 
     def _tiles_routes(self) -> None:
         """register tiles routes."""
 
-        @self.router.get(
-            "/tiles/{searchid}/{z}/{x}/{y}", **img_endpoint_params, deprecated=True
-        )
-        @self.router.get(
-            "/tiles/{searchid}/{z}/{x}/{y}.{format}",
-            **img_endpoint_params,
-            deprecated=True,
-        )
-        @self.router.get(
-            "/tiles/{searchid}/{z}/{x}/{y}@{scale}x",
-            **img_endpoint_params,
-            deprecated=True,
-        )
-        @self.router.get(
-            "/tiles/{searchid}/{z}/{x}/{y}@{scale}x.{format}",
-            **img_endpoint_params,
-            deprecated=True,
-        )
-        @self.router.get(
-            "/tiles/{searchid}/{TileMatrixSetId}/{z}/{x}/{y}",
-            **img_endpoint_params,
-            deprecated=True,
-        )
-        @self.router.get(
-            "/tiles/{searchid}/{TileMatrixSetId}/{z}/{x}/{y}.{format}",
-            **img_endpoint_params,
-            deprecated=True,
-        )
-        @self.router.get(
-            "/tiles/{searchid}/{TileMatrixSetId}/{z}/{x}/{y}@{scale}x",
-            **img_endpoint_params,
-            deprecated=True,
-        )
-        @self.router.get(
-            "/tiles/{searchid}/{TileMatrixSetId}/{z}/{x}/{y}@{scale}x.{format}",
-            **img_endpoint_params,
-            deprecated=True,
-        )
         @self.router.get("/{searchid}/tiles/{z}/{x}/{y}", **img_endpoint_params)
         @self.router.get(
             "/{searchid}/tiles/{z}/{x}/{y}.{format}", **img_endpoint_params
         )
         @self.router.get(
             "/{searchid}/tiles/{z}/{x}/{y}@{scale}x", **img_endpoint_params
         )
@@ -220,86 +153,86 @@
                 None,
                 gt=0,
                 alias="buffer",
                 title="Tile buffer.",
                 description="Buffer on each side of the given tile. It must be a multiple of `0.5`. Output **tilesize** will be expanded to `tilesize + 2 * buffer` (e.g 0.5 = 257x257, 1.0 = 258x258).",
             ),
             post_process=Depends(self.process_dependency),
-            rescale: Optional[List[Tuple[float, ...]]] = Depends(RescalingParams),
+            rescale=Depends(self.rescale_dependency),
             color_formula: Optional[str] = Query(
                 None,
                 title="Color Formula",
                 description="rio-color formula (info: https://github.com/mapbox/rio-color)",
             ),
             colormap=Depends(self.colormap_dependency),
             render_params=Depends(self.render_dependency),
             pgstac_params: PgSTACParams = Depends(),
             backend_params=Depends(self.backend_dependency),
             reader_params=Depends(self.reader_dependency),
             env=Depends(self.environment_dependency),
         ):
             """Create map tile."""
-            timings = []
             headers: Dict[str, str] = {}
 
             tms = self.supported_tms.get(TileMatrixSetId)
 
             threads = int(os.getenv("MOSAIC_CONCURRENCY", MAX_THREADS))
-            with Timer() as t:
-                with rasterio.Env(**env):
-                    with self.reader(
-                        searchid,
-                        tms=tms,
-                        reader_options={**reader_params},
-                        **backend_params,
-                    ) as src_dst:
-                        mosaic_read = t.from_start
-                        timings.append(("mosaicread", round(mosaic_read * 1000, 2)))
-
-                        image, assets = src_dst.tile(
-                            x,
-                            y,
-                            z,
-                            pixel_selection=pixel_selection.method(),
-                            tilesize=scale * 256,
-                            threads=threads,
-                            buffer=buffer,
-                            **layer_params,
-                            **dataset_params,
-                            **pgstac_params,
+
+            strict_zoom = str(os.getenv("MOSAIC_STRICT_ZOOM", False)).lower() in [
+                "true",
+                "yes",
+            ]
+
+            with rasterio.Env(**env):
+                with self.reader(
+                    searchid,
+                    tms=tms,
+                    reader_options={**reader_params},
+                    **backend_params,
+                ) as src_dst:
+
+                    if strict_zoom and (z < src_dst.minzoom or z > src_dst.maxzoom):
+                        raise HTTPException(
+                            400,
+                            f"Invalid ZOOM level {z}. Should be between {src_dst.minzoom} and {src_dst.maxzoom}",
                         )
-            timings.append(("dataread", round((t.elapsed - mosaic_read) * 1000, 2)))
 
-            with Timer() as t:
-                if post_process:
-                    image = post_process(image)
-
-                if rescale:
-                    image.rescale(rescale)
-
-                if color_formula:
-                    image.apply_color_formula(color_formula)
-            timings.append(("postprocess", round(t.elapsed * 1000, 2)))
+                    image, assets = src_dst.tile(
+                        x,
+                        y,
+                        z,
+                        tilesize=scale * 256,
+                        buffer=buffer,
+                        pixel_selection=pixel_selection.method(),
+                        threads=threads,
+                        **layer_params,
+                        **dataset_params,
+                        **pgstac_params,
+                    )
+
+            if post_process:
+                image = post_process(image)
+
+            if rescale:
+                image.rescale(rescale)
+
+            if color_formula:
+                image.apply_color_formula(color_formula)
+
+            if colormap:
+                image = image.apply_colormap(colormap)
 
             if not format:
                 format = ImageType.jpeg if image.mask.all() else ImageType.png
 
-            with Timer() as t:
-                content = image.render(
-                    img_format=format.driver,
-                    colormap=colormap,
-                    **format.profile,
-                    **render_params,
-                )
-            timings.append(("format", round(t.elapsed * 1000, 2)))
-
-            if OptionalHeader.server_timing in self.optional_headers:
-                headers["Server-Timing"] = ", ".join(
-                    [f"{name};dur={time}" for (name, time) in timings]
-                )
+            content = image.render(
+                img_format=format.driver,
+                **format.profile,
+                **render_params,
+            )
 
             if OptionalHeader.x_assets in self.optional_headers:
                 ids = [x["id"] for x in assets]
                 headers["X-Assets"] = ",".join(ids)
 
             return Response(content, media_type=format.mediatype, headers=headers)
 
@@ -346,17 +279,15 @@
                 None,
                 gt=0,
                 alias="buffer",
                 title="Tile buffer.",
                 description="Buffer on each side of the given tile. It must be a multiple of `0.5`. Output **tilesize** will be expanded to `tilesize + 2 * buffer` (e.g 0.5 = 257x257, 1.0 = 258x258).",
             ),  # noqa
             post_process=Depends(self.process_dependency),  # noqa
-            rescale: Optional[List[Tuple[float, ...]]] = Depends(
-                RescalingParams
-            ),  # noqa
+            rescale=Depends(self.rescale_dependency),  # noqa
             color_formula: Optional[str] = Query(
                 None,
                 title="Color Formula",
                 description="rio-color formula (info: https://github.com/mapbox/rio-color)",
             ),  # noqa
             colormap=Depends(self.colormap_dependency),  # noqa
             render_params=Depends(self.render_dependency),  # noqa
@@ -381,14 +312,15 @@
                 "x": "{x}",
                 "y": "{y}",
                 "scale": tile_scale,
                 "TileMatrixSetId": TileMatrixSetId,
             }
             if tile_format:
                 route_params["format"] = tile_format.value
+
             tiles_url = self.url_for(request, "tile", **route_params)
 
             qs_key_to_remove = [
                 "tilematrixsetid",
                 "tile_format",
                 "tile_scale",
                 "minzoom",
@@ -423,18 +355,18 @@
         @self.router.get("/{searchid}/map", response_class=HTMLResponse)
         @self.router.get(
             "/{searchid}/{TileMatrixSetId}/map", response_class=HTMLResponse
         )
         def map_viewer(
             request: Request,
             searchid=Depends(self.path_dependency),
-            TileMatrixSetId: Literal["WebMercatorQuad"] = Query(
-                "WebMercatorQuad",
-                description="TileMatrixSet Name (default: 'WebMercatorQuad')",
-            ),  # noqa
+            TileMatrixSetId: Literal[tuple(self.supported_tms.list())] = Query(  # type: ignore
+                self.default_tms,
+                description=f"TileMatrixSet Name (default: '{self.default_tms}')",
+            ),
             tile_format: Optional[ImageType] = Query(
                 None, description="Output image type. Default is auto."
             ),  # noqa
             tile_scale: int = Query(
                 1, gt=0, lt=4, description="Tile size scale. 1=256x256, 2=512x512..."
             ),  # noqa
             minzoom: Optional[int] = Query(
@@ -452,17 +384,15 @@
                 None,
                 gt=0,
                 alias="buffer",
                 title="Tile buffer.",
                 description="Buffer on each side of the given tile. It must be a multiple of `0.5`. Output **tilesize** will be expanded to `tilesize + 2 * buffer` (e.g 0.5 = 257x257, 1.0 = 258x258).",
             ),  # noqa
             post_process=Depends(self.process_dependency),  # noqa
-            rescale: Optional[List[Tuple[float, ...]]] = Depends(
-                RescalingParams
-            ),  # noqa
+            rescale=Depends(self.rescale_dependency),  # noqa
             color_formula: Optional[str] = Query(
                 None,
                 title="Color Formula",
                 description="rio-color formula (info: https://github.com/mapbox/rio-color)",
             ),  # noqa
             colormap=Depends(self.colormap_dependency),  # noqa
             render_params=Depends(self.render_dependency),  # noqa
@@ -475,15 +405,15 @@
             tilejson_url = self.url_for(
                 request, "tilejson", searchid=searchid, TileMatrixSetId=TileMatrixSetId
             )
             if request.query_params._list:
                 tilejson_url += f"?{urlencode(request.query_params._list)}"
 
             tms = self.supported_tms.get(TileMatrixSetId)
-            return templates.TemplateResponse(
+            return self.templates.TemplateResponse(
                 name="index.html",
                 context={
                     "request": request,
                     "tilejson_endpoint": tilejson_url,
                     "tms": tms,
                     "resolutions": [tms._resolution(matrix) for matrix in tms],
                 },
@@ -527,17 +457,15 @@
                 None,
                 gt=0,
                 alias="buffer",
                 title="Tile buffer.",
                 description="Buffer on each side of the given tile. It must be a multiple of `0.5`. Output **tilesize** will be expanded to `tilesize + 2 * buffer` (e.g 0.5 = 257x257, 1.0 = 258x258).",
             ),  # noqa
             post_process=Depends(self.process_dependency),  # noqa
-            rescale: Optional[List[Tuple[float, ...]]] = Depends(
-                RescalingParams
-            ),  # noqa
+            rescale=Depends(self.rescale_dependency),  # noqa
             color_formula: Optional[str] = Query(
                 None,
                 title="Color Formula",
                 description="rio-color formula (info: https://github.com/mapbox/rio-color)",
             ),  # noqa
             colormap=Depends(self.colormap_dependency),  # noqa
             render_params=Depends(self.render_dependency),  # noqa
@@ -604,15 +532,15 @@
                             <TileWidth>{matrix.tileWidth}</TileWidth>
                             <TileHeight>{matrix.tileHeight}</TileHeight>
                             <MatrixWidth>{matrix.matrixWidth}</MatrixWidth>
                             <MatrixHeight>{matrix.matrixHeight}</MatrixHeight>
                         </TileMatrix>"""
                 tileMatrix.append(tm)
 
-            return templates.TemplateResponse(
+            return self.templates.TemplateResponse(
                 "wmts.xml",
                 {
                     "request": request,
                     "tiles_endpoint": tiles_url,
                     "bounds": bounds,
                     "tileMatrix": tileMatrix,
                     "tms": tms,
@@ -625,19 +553,30 @@
 
     def _assets_routes(self):
         """Register assets routes."""
 
         @self.router.get(
             "/{searchid}/{z}/{x}/{y}/assets",
             responses={200: {"description": "Return list of assets"}},
+            deprecated=True,
         )
         @self.router.get(
             "/{searchid}/{TileMatrixSetId}/{z}/{x}/{y}/assets",
             responses={200: {"description": "Return list of assets"}},
             response_model=List[Dict],
+            deprecated=True,
+        )
+        @self.router.get(
+            "/{searchid}/tiles/{z}/{x}/{y}/assets",
+            responses={200: {"description": "Return list of assets"}},
+        )
+        @self.router.get(
+            "/{searchid}/tiles/{TileMatrixSetId}/{z}/{x}/{y}/assets",
+            responses={200: {"description": "Return list of assets"}},
+            response_model=List[Dict],
         )
         def assets_for_tile(
             searchid=Depends(self.path_dependency),
             z: int = Path(..., ge=0, le=30, description="Tiles's zoom level"),
             x: int = Path(..., description="Tiles's column"),
             y: int = Path(..., description="Tiles's row"),
             TileMatrixSetId: Literal[tuple(self.supported_tms.list())] = Query(  # type: ignore
@@ -949,15 +888,15 @@
             backend_params=Depends(self.backend_dependency),
             reader_params=Depends(self.reader_dependency),
             env=Depends(self.environment_dependency),
         ):
             """Get Statistics from a geojson feature or featureCollection."""
             fc = geojson
             if isinstance(fc, Feature):
-                fc = FeatureCollection(features=[geojson])
+                fc = FeatureCollection(type="FeatureCollection", features=[geojson])
 
             threads = int(os.getenv("MOSAIC_CONCURRENCY", MAX_THREADS))
 
             with rasterio.Env(**env):
                 with self.reader(
                     searchid,
                     reader_options={**reader_params},
```

### Comparing `titiler.pgstac-0.3.3/titiler/pgstac/main.py` & `titiler.pgstac-0.4.0/titiler/pgstac/main.py`

 * *Files identical despite different names*

### Comparing `titiler.pgstac-0.3.3/titiler/pgstac/model.py` & `titiler.pgstac-0.4.0/titiler/pgstac/model.py`

 * *Files identical despite different names*

### Comparing `titiler.pgstac-0.3.3/titiler/pgstac/mosaic.py` & `titiler.pgstac-0.4.0/titiler/pgstac/mosaic.py`

 * *Files 0% similar despite different names*

```diff
@@ -172,15 +172,15 @@
     def assets_for_point(self, lng: float, lat: float, **kwargs: Any) -> List[Dict]:
         """Retrieve assets for point."""
         # Point search is currently broken within PgSTAC
         # in order to return the correct result we need to make sure exitwhenfull and skipcovered options
         # are set to `False`
         # ref: https://github.com/stac-utils/pgstac/pull/52
         kwargs.update(**{"exitwhenfull": False, "skipcovered": False})
-        return self.get_assets(Point(coordinates=(lng, lat)), **kwargs)
+        return self.get_assets(Point(type="Point", coordinates=(lng, lat)), **kwargs)
 
     def assets_for_bbox(
         self,
         xmin: float,
         ymin: float,
         xmax: float,
         ymax: float,
```

### Comparing `titiler.pgstac-0.3.3/titiler/pgstac/reader.py` & `titiler.pgstac-0.4.0/titiler/pgstac/reader.py`

 * *Files identical despite different names*

### Comparing `titiler.pgstac-0.3.3/titiler/pgstac/settings.py` & `titiler.pgstac-0.4.0/titiler/pgstac/settings.py`

 * *Files identical despite different names*

### Comparing `titiler.pgstac-0.3.3/titiler/pgstac/utils.py` & `titiler.pgstac-0.4.0/titiler/pgstac/utils.py`

 * *Files identical despite different names*

### Comparing `titiler.pgstac-0.3.3/PKG-INFO` & `titiler.pgstac-0.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: titiler.pgstac
-Version: 0.3.3
+Version: 0.4.0
 Summary: Connect PgSTAC and TiTiler.
 Keywords: COG,STAC,MosaicJSON,Fastapi,Dynamic tile server,pgSTAC
 Author-email: Vincent Sarago <vincent@developmentseed.com>,David Bitner <david@developmentseed.com>
 Requires-Python: >=3.8
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: titiler.pgstac Version: 0.3.3 Summary: Connect
+Metadata-Version: 2.1 Name: titiler.pgstac Version: 0.4.0 Summary: Connect
 PgSTAC and TiTiler. Keywords: COG,STAC,MosaicJSON,Fastapi,Dynamic tile
 server,pgSTAC Author-email: Vincent Sarago
 developmentseed.com>,David Bitner
 developmentseed.com> Requires-Python: >=3.8 Classifier: Intended Audience ::
 Information Technology Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
```

