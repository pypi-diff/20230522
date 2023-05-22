# Comparing `tmp/netteikei-0.2.0-py3-none-any.whl.zip` & `tmp/netteikei-0.2.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 6607 bytes, number of entries: 12
--rw-------  2.0 unx      131 b- defN 23-May-16 19:25 netteikei/__init__.py
+Zip file size: 6623 bytes, number of entries: 12
+-rw-------  2.0 unx      131 b- defN 23-May-22 02:58 netteikei/__init__.py
 -rw-------  2.0 unx     2679 b- defN 23-May-14 16:14 netteikei/core.py
 -rw-------  2.0 unx        0 b- defN 23-May-07 09:41 netteikei/py.typed
 -rw-------  2.0 unx     1297 b- defN 23-May-14 16:14 netteikei/typedefs.py
 -rw-------  2.0 unx        0 b- defN 23-May-07 13:53 netteikei/contrib/__init__.py
--rw-------  2.0 unx     2435 b- defN 23-May-14 16:48 netteikei/contrib/download.py
--rw-------  2.0 unx     1158 b- defN 23-May-14 17:10 netteikei/contrib/utils.py
--rw-------  2.0 unx     1068 b- defN 23-May-16 19:27 netteikei-0.2.0.dist-info/LICENSE
--rw-------  2.0 unx     1325 b- defN 23-May-16 19:27 netteikei-0.2.0.dist-info/METADATA
--rw-------  2.0 unx       92 b- defN 23-May-16 19:27 netteikei-0.2.0.dist-info/WHEEL
--rw-------  2.0 unx       10 b- defN 23-May-16 19:27 netteikei-0.2.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      949 b- defN 23-May-16 19:27 netteikei-0.2.0.dist-info/RECORD
-12 files, 11144 bytes uncompressed, 5013 bytes compressed:  55.0%
+-rw-------  2.0 unx     2429 b- defN 23-May-20 16:10 netteikei/contrib/download.py
+-rw-------  2.0 unx     1157 b- defN 23-May-20 16:09 netteikei/contrib/utils.py
+-rw-------  2.0 unx     1068 b- defN 23-May-22 03:01 netteikei-0.2.1.dist-info/LICENSE
+-rw-------  2.0 unx     1371 b- defN 23-May-22 03:01 netteikei-0.2.1.dist-info/METADATA
+-rw-------  2.0 unx       92 b- defN 23-May-22 03:01 netteikei-0.2.1.dist-info/WHEEL
+-rw-------  2.0 unx       10 b- defN 23-May-22 03:01 netteikei-0.2.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      949 b- defN 23-May-22 03:01 netteikei-0.2.1.dist-info/RECORD
+12 files, 11183 bytes uncompressed, 5029 bytes compressed:  55.0%
```

## zipnote {}

```diff
@@ -15,23 +15,23 @@
 
 Filename: netteikei/contrib/download.py
 Comment: 
 
 Filename: netteikei/contrib/utils.py
 Comment: 
 
-Filename: netteikei-0.2.0.dist-info/LICENSE
+Filename: netteikei-0.2.1.dist-info/LICENSE
 Comment: 
 
-Filename: netteikei-0.2.0.dist-info/METADATA
+Filename: netteikei-0.2.1.dist-info/METADATA
 Comment: 
 
-Filename: netteikei-0.2.0.dist-info/WHEEL
+Filename: netteikei-0.2.1.dist-info/WHEEL
 Comment: 
 
-Filename: netteikei-0.2.0.dist-info/top_level.txt
+Filename: netteikei-0.2.1.dist-info/top_level.txt
 Comment: 
 
-Filename: netteikei-0.2.0.dist-info/RECORD
+Filename: netteikei-0.2.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## netteikei/__init__.py

```diff
@@ -1,6 +1,6 @@
 from .core import Client, Handler
 from .typedefs import Request
 
 
-__version__ = "0.2.0"
+__version__ = "0.2.1"
 __all__ = ["Client", "Handler", "Request"]
```

## netteikei/contrib/download.py

```diff
@@ -3,16 +3,16 @@
 from pathlib import Path
 from typing import NamedTuple, Self, Unpack
 
 import aiofiles
 from aiohttp import ClientResponse, ClientSession
 import tqdm
 
-from .. import Client, Handler
-from ..typedefs import Request, SessionOpts, StrOrURL
+from .. import Client, Handler, Request
+from ..typedefs import SessionOpts, StrOrURL
 from .utils import isfile, parse_name, parse_length, get_start_byte
 
 
 _DIR: ContextVar[Path] = ContextVar("dir")
 
 
 class DownloadAlreadyExists(Exception):
@@ -20,66 +20,64 @@
     def __init__(self, path: Path) -> None:
         self.path = path
 
     def __str__(self) -> str:
         return f"'{self.path}' alredy exists"
 
 
-class Download(NamedTuple):
+class DownloadInfo(NamedTuple):
     url: StrOrURL
     path: Path
     length: int | None
     start: int
 
     @classmethod
-    async def new(cls, session: ClientSession, url: StrOrURL, /) -> Self:
-        async with session.head(url) as resp:
+    async def find(cls, session: ClientSession, url: StrOrURL, /) -> Self:
+        async with session.head(url, allow_redirects=True) as resp:
             name = parse_name(resp, "untitled")
             length = parse_length(resp.headers)
             path = _DIR.get() / name
             start = await get_start_byte(resp.headers, path)
             if await isfile(path) and start == length:
                 raise DownloadAlreadyExists(path)
             return cls(url, path, length, start)
 
 
-class Downloader(Handler[Download, None]):
+class DownloadHandler(Handler[DownloadInfo, None]):
 
     async def create_request(self) -> Request:
-        dl = self.ctx.get()
+        info = self.ctx.get()
         return Request.new(
-            url=dl.url,
-            headers={"Range": f"bytes={dl.start}-"}
+            url=info.url,
+            headers={"Range": f"bytes={info.start}-"}
         )
 
     async def process_response(self, resp: ClientResponse) -> None:
-        dl = self.ctx.get()
-        async with resp, aiofiles.open(dl.path, "wb") as f:
+        info = self.ctx.get()
+        async with resp, aiofiles.open(info.path, "ab") as fp:
             with tqdm.tqdm(
-                total=dl.length,
-                initial=dl.start,
+                total=info.length,
+                initial=info.start,
                 unit="B",
                 unit_scale=True,
                 unit_divisor=1024
-            ) as pbar:
-                if dl.start != 0:
-                    await f.seek(dl.start)
+            ) as bar:
                 async for chunk in resp.content.iter_any():
-                    await f.write(chunk)
-                    pbar.update(len(chunk))
+                    progress = await fp.write(chunk)
+                    bar.update(progress)
 
 
 async def download(
     dir: Path,
     /,
     *urls: StrOrURL,
     limit: int = 3,
     **kwargs: Unpack[SessionOpts]
 ) -> None:
     token = _DIR.set(dir)
     async with ClientSession(**kwargs) as session:
-        dls = await asyncio.gather(
-            *(Download.new(session, url) for url in urls)
+        info = await asyncio.gather(
+            *(DownloadInfo.find(session, url) for url in urls)
         )
-        client = Client(session, Downloader(), max_workers=limit)
-        await client.gather(*dls)
+        client = Client(session, DownloadHandler(), max_workers=limit)
+        await client.gather(*info)
     _DIR.reset(token)
```

## netteikei/contrib/utils.py

```diff
@@ -35,12 +35,11 @@
         return name
 
 
 def parse_length(headers: Headers) -> int | None:
     if (s := headers.get("Content-Length")) is not None:
         return int(s)
 
-
 async def get_start_byte(headers: Headers, file: Path) -> int:
     if headers.get("Accept-Ranges") == "bytes" and await isfile(file):
         return await getsize(file)
     return 0
```

## Comparing `netteikei-0.2.0.dist-info/LICENSE` & `netteikei-0.2.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `netteikei-0.2.0.dist-info/METADATA` & `netteikei-0.2.1.dist-info/METADATA`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: netteikei
-Version: 0.2.0
-Summary: Utility library for making concurrent HTTP requests using aiohttp
+Version: 0.2.1
+Summary: Utility for making concurrent HTTP requests with aiohttp
 Home-page: https://github.com/fernofsigma/netteikei
 Author: FernOfSigma
 Author-email: fernofsigma@tuta.io
 License: MIT
 Project-URL: GitHub: issues, https://github.com/fernofsigma/netteikei/issues
 Project-URL: GitHub: repo, https://github.com/fernofsigma/netteikei
 Classifier: Development Status :: 3 - Alpha
@@ -16,14 +16,15 @@
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Internet :: WWW/HTTP
+Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
 Requires-Python: >=3.11
 License-File: LICENSE
 Requires-Dist: aiohttp (<4.0.0,>=3.8.4)
 Provides-Extra: download
 Requires-Dist: aiofiles ; extra == 'download'
```

## Comparing `netteikei-0.2.0.dist-info/RECORD` & `netteikei-0.2.1.dist-info/RECORD`

 * *Files 21% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-netteikei/__init__.py,sha256=4OoJPt3pWzJhk4t7p68Lh81uzeBbt_-ZehOm210C_vU,131
+netteikei/__init__.py,sha256=G2R6WDGvsl5Afw8lvRywKP6WdlHC6LJo0BEeWaNCkn8,131
 netteikei/core.py,sha256=_iwcs1T3j8ZjN46x02f8rP0SlClnpeD-Q8Codq3Oz4Q,2679
 netteikei/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 netteikei/typedefs.py,sha256=WG1_PMtZVnXJTfOTTOUY9nSQ5TDID1URux9GwGJWVNA,1297
 netteikei/contrib/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-netteikei/contrib/download.py,sha256=gCRn4cVUPiVziPRK2ioJmcX_9eGIs3c13c6jttdDT8k,2435
-netteikei/contrib/utils.py,sha256=tWW73FXdlUGyhZKJoLU1lSb7u_OciKpcZPBXWFkwfyE,1158
-netteikei-0.2.0.dist-info/LICENSE,sha256=37AgUwjy1RqDbLVahc_zXbHKIRzTEKjlDpKfzB6a-6g,1068
-netteikei-0.2.0.dist-info/METADATA,sha256=Gntz48i9k8sdbgMQU5zxRv-IBzNCQ5GRFV2624ie-RI,1325
-netteikei-0.2.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-netteikei-0.2.0.dist-info/top_level.txt,sha256=1TkkZh-n9Ys0kU95kW0keVBeiiY87lC-pR-FF7FFGB0,10
-netteikei-0.2.0.dist-info/RECORD,,
+netteikei/contrib/download.py,sha256=asuoCP7GYoJnJW1RgbOCo7QGcmCHYJuOWQe_7h9_Vxk,2429
+netteikei/contrib/utils.py,sha256=SDpD4JTvAs0sT4U6HRuNgoqDwXFMNVFi3iSSYcXzctQ,1157
+netteikei-0.2.1.dist-info/LICENSE,sha256=37AgUwjy1RqDbLVahc_zXbHKIRzTEKjlDpKfzB6a-6g,1068
+netteikei-0.2.1.dist-info/METADATA,sha256=nGBOLCuLWatfhdZgFBR9t-VpWLBrfJyza6kOdP8nlp8,1371
+netteikei-0.2.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+netteikei-0.2.1.dist-info/top_level.txt,sha256=1TkkZh-n9Ys0kU95kW0keVBeiiY87lC-pR-FF7FFGB0,10
+netteikei-0.2.1.dist-info/RECORD,,
```

