# Comparing `tmp/tldrwl-0.0.3.tar.gz` & `tmp/tldrwl-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tldrwl-0.0.3.tar", last modified: Mon May 22 04:39:18 2023, max compression
+gzip compressed data, was "tldrwl-0.0.4.tar", last modified: Mon May 22 06:00:44 2023, max compression
```

## Comparing `tldrwl-0.0.3.tar` & `tldrwl-0.0.4.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxr-xr-x   0 jrodal    (1000) jrodal    (1000)        0 2023-05-22 04:39:18.983630 tldrwl-0.0.3/
--rw-r--r--   0 jrodal    (1000) jrodal    (1000)       25 2023-05-22 01:33:23.000000 tldrwl-0.0.3/MANIFEST.in
--rw-r--r--   0 jrodal    (1000) jrodal    (1000)     1161 2023-05-22 04:39:18.983630 tldrwl-0.0.3/PKG-INFO
--rw-r--r--   0 jrodal    (1000) jrodal    (1000)      871 2023-05-22 04:38:38.000000 tldrwl-0.0.3/README.md
--rw-r--r--   0 jrodal    (1000) jrodal    (1000)       23 2023-05-22 04:16:37.000000 tldrwl-0.0.3/requirements.txt
--rw-r--r--   0 jrodal    (1000) jrodal    (1000)       38 2023-05-22 04:39:18.983630 tldrwl-0.0.3/setup.cfg
--rw-r--r--   0 jrodal    (1000) jrodal    (1000)      614 2023-05-22 04:35:17.000000 tldrwl-0.0.3/setup.py
-drwxr-xr-x   0 jrodal    (1000) jrodal    (1000)        0 2023-05-22 04:39:18.983630 tldrwl-0.0.3/tldrwl/
--rw-r--r--   0 jrodal    (1000) jrodal    (1000)        0 2023-05-22 00:53:22.000000 tldrwl-0.0.3/tldrwl/__init__.py
--rw-r--r--   0 jrodal    (1000) jrodal    (1000)      207 2023-05-22 01:55:37.000000 tldrwl-0.0.3/tldrwl/ai_interface.py
--rw-r--r--   0 jrodal    (1000) jrodal    (1000)      772 2023-05-22 02:09:19.000000 tldrwl-0.0.3/tldrwl/exception.py
--rw-r--r--   0 jrodal    (1000) jrodal    (1000)      679 2023-05-22 02:16:47.000000 tldrwl-0.0.3/tldrwl/register.py
--rw-r--r--   0 jrodal    (1000) jrodal    (1000)     4432 2023-05-22 04:26:05.000000 tldrwl-0.0.3/tldrwl/summarize_text.py
-drwxr-xr-x   0 jrodal    (1000) jrodal    (1000)        0 2023-05-22 04:39:18.983630 tldrwl-0.0.3/tldrwl.egg-info/
--rw-r--r--   0 jrodal    (1000) jrodal    (1000)     1161 2023-05-22 04:39:18.000000 tldrwl-0.0.3/tldrwl.egg-info/PKG-INFO
--rw-r--r--   0 jrodal    (1000) jrodal    (1000)      302 2023-05-22 04:39:18.000000 tldrwl-0.0.3/tldrwl.egg-info/SOURCES.txt
--rw-r--r--   0 jrodal    (1000) jrodal    (1000)        1 2023-05-22 04:39:18.000000 tldrwl-0.0.3/tldrwl.egg-info/dependency_links.txt
--rw-r--r--   0 jrodal    (1000) jrodal    (1000)       23 2023-05-22 04:39:18.000000 tldrwl-0.0.3/tldrwl.egg-info/requires.txt
--rw-r--r--   0 jrodal    (1000) jrodal    (1000)        7 2023-05-22 04:39:18.000000 tldrwl-0.0.3/tldrwl.egg-info/top_level.txt
+drwxr-xr-x   0 jrodal    (1000) jrodal    (1000)        0 2023-05-22 06:00:44.052178 tldrwl-0.0.4/
+-rw-r--r--   0 jrodal    (1000) jrodal    (1000)       25 2023-05-22 01:33:23.000000 tldrwl-0.0.4/MANIFEST.in
+-rw-r--r--   0 jrodal    (1000) jrodal    (1000)     2359 2023-05-22 06:00:44.052178 tldrwl-0.0.4/PKG-INFO
+-rw-r--r--   0 jrodal    (1000) jrodal    (1000)     2069 2023-05-22 05:59:40.000000 tldrwl-0.0.4/README.md
+-rw-r--r--   0 jrodal    (1000) jrodal    (1000)       60 2023-05-22 05:09:45.000000 tldrwl-0.0.4/requirements.txt
+-rw-r--r--   0 jrodal    (1000) jrodal    (1000)       38 2023-05-22 06:00:44.052178 tldrwl-0.0.4/setup.cfg
+-rw-r--r--   0 jrodal    (1000) jrodal    (1000)      614 2023-05-22 06:00:39.000000 tldrwl-0.0.4/setup.py
+drwxr-xr-x   0 jrodal    (1000) jrodal    (1000)        0 2023-05-22 06:00:44.052178 tldrwl-0.0.4/tldrwl/
+-rw-r--r--   0 jrodal    (1000) jrodal    (1000)        0 2023-05-22 00:53:22.000000 tldrwl-0.0.4/tldrwl/__init__.py
+-rw-r--r--   0 jrodal    (1000) jrodal    (1000)      207 2023-05-22 01:55:37.000000 tldrwl-0.0.4/tldrwl/ai_interface.py
+-rw-r--r--   0 jrodal    (1000) jrodal    (1000)     1177 2023-05-22 05:37:32.000000 tldrwl-0.0.4/tldrwl/exception.py
+-rw-r--r--   0 jrodal    (1000) jrodal    (1000)      679 2023-05-22 02:16:47.000000 tldrwl-0.0.4/tldrwl/register.py
+-rw-r--r--   0 jrodal    (1000) jrodal    (1000)     5369 2023-05-22 05:23:41.000000 tldrwl-0.0.4/tldrwl/summarize_text.py
+-rw-r--r--   0 jrodal    (1000) jrodal    (1000)     1847 2023-05-22 05:49:45.000000 tldrwl-0.0.4/tldrwl/summarize_youtube.py
+drwxr-xr-x   0 jrodal    (1000) jrodal    (1000)        0 2023-05-22 06:00:44.052178 tldrwl-0.0.4/tldrwl.egg-info/
+-rw-r--r--   0 jrodal    (1000) jrodal    (1000)     2359 2023-05-22 06:00:44.000000 tldrwl-0.0.4/tldrwl.egg-info/PKG-INFO
+-rw-r--r--   0 jrodal    (1000) jrodal    (1000)      330 2023-05-22 06:00:44.000000 tldrwl-0.0.4/tldrwl.egg-info/SOURCES.txt
+-rw-r--r--   0 jrodal    (1000) jrodal    (1000)        1 2023-05-22 06:00:44.000000 tldrwl-0.0.4/tldrwl.egg-info/dependency_links.txt
+-rw-r--r--   0 jrodal    (1000) jrodal    (1000)       60 2023-05-22 06:00:44.000000 tldrwl-0.0.4/tldrwl.egg-info/requires.txt
+-rw-r--r--   0 jrodal    (1000) jrodal    (1000)        7 2023-05-22 06:00:44.000000 tldrwl-0.0.4/tldrwl.egg-info/top_level.txt
```

### Comparing `tldrwl-0.0.3/PKG-INFO` & `tldrwl-0.0.4/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,46 +1,103 @@
 Metadata-Version: 2.1
 Name: tldrwl
-Version: 0.0.3
+Version: 0.0.4
 Summary: Too long, didn't read/watch/listen
 Home-page: https://github.com/jrodal98/tldrwl
 Author: Jacob Rodal
 Author-email: dev@jrodal.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # tldrwl (too long, didn't read/watch/listen)
 
 ## About
 
 - [x] Summarize text with a single API call
-- [ ] Summarize video with a single API call
+- [x] Summarize Youtube video with a single API call
 - [ ] Summarize audio with a single API call
 - [x] Sync APIs
 - [x] Async APIs
 
+OpenAI has a limit on maximum number of tokens per requests, so the following strategy is employed to generate the summaries:
+
+Split message into chunks
+Gather summaries for each chunk
+Summarize the summaries
+
 ## Install
 
 ```
 pip install tldrwl
 ```
 
 ## Examples
 
+### Youtube
+
+```python3
+#!/usr/bin/env python3
+# www.jrodal.com
+
+import asyncio
+import time
+from tldrwl.summarize_youtube import YoutubeSummarizer
+
+import logging
+
+logging.basicConfig(level=logging.DEBUG)
+
+yt_video = "https://www.youtube.com/watch?v=6E3-MRnh8TQ"
+
+
+def main_sync() -> None:
+    summary = YoutubeSummarizer().summarize_video(yt_video)
+
+    print(summary)
+    print(f"{summary.estimated_cost_usd=}")
+
+
+async def main_async() -> None:
+    summary = await YoutubeSummarizer().summarize_video_async(yt_video)
+
+    print(summary)
+    print(f"{summary.estimated_cost_usd=}")
+
+
+async def main() -> None:
+    start = time.time()
+    print("Running async")
+    await main_async()
+    end = time.time()
+    print(f"Finished async in {end - start}s")
+
+    start = time.time()
+    print("Running sync")
+    main_sync()
+    end = time.time()
+    print(f"Finished sync in {end - start}s")
+
+
+if __name__ == "__main__":
+    asyncio.run(main())
+```
+
 ### Text
 
 ```python3
 #!/usr/bin/env python3
 # my_script.py
 
 import asyncio
 from tldrwl.summarize_text import TextSummarizer
 
+text = "<my really long text>"
+
 def main_sync() -> None:
     summary = TextSummarizer().summarize_text(text)
 
     print(summary)
     print(summary.estimated_cost_usd)
 
 async def main_async() -> None:
```

### Comparing `tldrwl-0.0.3/setup.py` & `tldrwl-0.0.4/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = f.read()
 
 with open("requirements.txt") as f:
     install_requires = f.read().splitlines()
 
 setuptools.setup(
     name="tldrwl",
-    version="0.0.3",
+    version="0.0.4",
     author="Jacob Rodal",
     author_email="dev@jrodal.com",
     description="Too long, didn't read/watch/listen",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/jrodal98/tldrwl",
     packages=setuptools.find_packages(),
```

### Comparing `tldrwl-0.0.3/tldrwl/register.py` & `tldrwl-0.0.4/tldrwl/register.py`

 * *Files identical despite different names*

### Comparing `tldrwl-0.0.3/tldrwl/summarize_text.py` & `tldrwl-0.0.4/tldrwl/summarize_text.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 #!/usr/bin/env python3
 # www.jrodal.com
 
 import asyncio
+import time
 from dataclasses import dataclass
 from enum import Enum
 import logging
 import re
 import textwrap
 
 import openai
@@ -41,14 +42,15 @@
         self,
         *,
         model: Model = Model.GPT35TURBO,
         prompt_string: str = "Write a detailed summary of the following:\n\n{}\n",
         chunk_size: int = 8000,
         max_num_chunks: int = 15,
     ) -> None:
+        super().__init__()
         self._model = model
         self._prompt_string = prompt_string
         self._chunk_size = chunk_size
         self._max_num_chunks = max_num_chunks
         self._logger = logging.getLogger(__name__)
 
     def _response_to_text_summary(self, response: Dict[str, Any]) -> TextSummary:
@@ -62,31 +64,50 @@
             num_tokens=num_tokens,  # type: ignore
             model=self._model,
         )
 
     async def _summarize_chunk_async(self, chunk: str, max_tokens: int) -> TextSummary:
         prompt = self._prompt_string.format(chunk)
 
-        response = await openai.ChatCompletion.acreate(  # type: ignore
-            model=self._model.value,
-            messages=[{"role": "user", "content": prompt}],
-            max_tokens=max_tokens,
-        )
+        for _ in range(0, 3):
+            try:
+                response = await openai.ChatCompletion.acreate(  # type: ignore
+                    model=self._model.value,
+                    messages=[{"role": "user", "content": prompt}],
+                    max_tokens=max_tokens,
+                )
+                return self._response_to_text_summary(response)  # type: ignore
+            except openai.error.RateLimitError:  # pyright: ignore
+                retry_interval = 3
+                self._logger.debug(
+                    f"Rate limited by openai - resting for {retry_interval}s"
+                )
+                await asyncio.sleep(retry_interval)
 
-        return self._response_to_text_summary(response)  # type: ignore
+        return TextSummary(summary="", num_tokens=0, model=self._model)
 
     def _summarize_chunk(self, chunk: str, max_tokens: int) -> TextSummary:
         prompt = self._prompt_string.format(chunk)
 
-        response = openai.ChatCompletion.create(  # type: ignore
-            model=self._model.value,
-            messages=[{"role": "user", "content": prompt}],
-            max_tokens=max_tokens,
-        )
-        return self._response_to_text_summary(response)  # type: ignore
+        for _ in range(0, 3):
+            try:
+                response = openai.ChatCompletion.create(  # type: ignore
+                    model=self._model.value,
+                    messages=[{"role": "user", "content": prompt}],
+                    max_tokens=max_tokens,
+                )
+                return self._response_to_text_summary(response)  # type: ignore
+            except openai.error.RateLimitError:  # pyright: ignore
+                retry_interval = 3
+                self._logger.debug(
+                    f"Rate limited by openai - resting for {retry_interval}s"
+                )
+                time.sleep(retry_interval)
+
+        return TextSummary(summary="", num_tokens=0, model=self._model)
 
     def _get_chunks(self, text: str) -> List[str]:
         text_length = len(text)
         self._logger.debug(f"{text_length=}")
 
         chunks = textwrap.wrap(text, self._chunk_size)[: self._max_num_chunks]
         num_chunks = len(chunks)
```

### Comparing `tldrwl-0.0.3/tldrwl.egg-info/PKG-INFO` & `tldrwl-0.0.4/tldrwl.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,46 +1,103 @@
 Metadata-Version: 2.1
 Name: tldrwl
-Version: 0.0.3
+Version: 0.0.4
 Summary: Too long, didn't read/watch/listen
 Home-page: https://github.com/jrodal98/tldrwl
 Author: Jacob Rodal
 Author-email: dev@jrodal.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # tldrwl (too long, didn't read/watch/listen)
 
 ## About
 
 - [x] Summarize text with a single API call
-- [ ] Summarize video with a single API call
+- [x] Summarize Youtube video with a single API call
 - [ ] Summarize audio with a single API call
 - [x] Sync APIs
 - [x] Async APIs
 
+OpenAI has a limit on maximum number of tokens per requests, so the following strategy is employed to generate the summaries:
+
+Split message into chunks
+Gather summaries for each chunk
+Summarize the summaries
+
 ## Install
 
 ```
 pip install tldrwl
 ```
 
 ## Examples
 
+### Youtube
+
+```python3
+#!/usr/bin/env python3
+# www.jrodal.com
+
+import asyncio
+import time
+from tldrwl.summarize_youtube import YoutubeSummarizer
+
+import logging
+
+logging.basicConfig(level=logging.DEBUG)
+
+yt_video = "https://www.youtube.com/watch?v=6E3-MRnh8TQ"
+
+
+def main_sync() -> None:
+    summary = YoutubeSummarizer().summarize_video(yt_video)
+
+    print(summary)
+    print(f"{summary.estimated_cost_usd=}")
+
+
+async def main_async() -> None:
+    summary = await YoutubeSummarizer().summarize_video_async(yt_video)
+
+    print(summary)
+    print(f"{summary.estimated_cost_usd=}")
+
+
+async def main() -> None:
+    start = time.time()
+    print("Running async")
+    await main_async()
+    end = time.time()
+    print(f"Finished async in {end - start}s")
+
+    start = time.time()
+    print("Running sync")
+    main_sync()
+    end = time.time()
+    print(f"Finished sync in {end - start}s")
+
+
+if __name__ == "__main__":
+    asyncio.run(main())
+```
+
 ### Text
 
 ```python3
 #!/usr/bin/env python3
 # my_script.py
 
 import asyncio
 from tldrwl.summarize_text import TextSummarizer
 
+text = "<my really long text>"
+
 def main_sync() -> None:
     summary = TextSummarizer().summarize_text(text)
 
     print(summary)
     print(summary.estimated_cost_usd)
 
 async def main_async() -> None:
```

