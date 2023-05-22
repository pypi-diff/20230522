# Comparing `tmp/tldrwl-0.0.7.tar.gz` & `tmp/tldrwl-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tldrwl-0.0.7.tar", last modified: Mon May 22 08:10:35 2023, max compression
+gzip compressed data, was "tldrwl-0.0.8.tar", last modified: Mon May 22 08:58:07 2023, max compression
```

## Comparing `tldrwl-0.0.7.tar` & `tldrwl-0.0.8.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 jrodal    (1000) jrodal    (1000)        0 2023-05-22 08:10:35.239869 tldrwl-0.0.7/
--rw-r--r--   0 jrodal    (1000) jrodal    (1000)       25 2023-05-22 01:33:23.000000 tldrwl-0.0.7/MANIFEST.in
--rw-r--r--   0 jrodal    (1000) jrodal    (1000)    16598 2023-05-22 08:10:35.239869 tldrwl-0.0.7/PKG-INFO
--rw-r--r--   0 jrodal    (1000) jrodal    (1000)    16308 2023-05-22 08:10:00.000000 tldrwl-0.0.7/README.md
--rw-r--r--   0 jrodal    (1000) jrodal    (1000)      100 2023-05-22 06:20:03.000000 tldrwl-0.0.7/requirements.txt
--rw-r--r--   0 jrodal    (1000) jrodal    (1000)       38 2023-05-22 08:10:35.239869 tldrwl-0.0.7/setup.cfg
--rw-r--r--   0 jrodal    (1000) jrodal    (1000)      614 2023-05-22 08:10:20.000000 tldrwl-0.0.7/setup.py
-drwxr-xr-x   0 jrodal    (1000) jrodal    (1000)        0 2023-05-22 08:10:35.239869 tldrwl-0.0.7/tldrwl/
--rw-r--r--   0 jrodal    (1000) jrodal    (1000)        0 2023-05-22 00:53:22.000000 tldrwl-0.0.7/tldrwl/__init__.py
--rw-r--r--   0 jrodal    (1000) jrodal    (1000)      907 2023-05-22 06:42:51.000000 tldrwl-0.0.7/tldrwl/ai_interface.py
--rw-r--r--   0 jrodal    (1000) jrodal    (1000)     1177 2023-05-22 05:37:32.000000 tldrwl-0.0.7/tldrwl/exception.py
--rw-r--r--   0 jrodal    (1000) jrodal    (1000)      679 2023-05-22 02:16:47.000000 tldrwl-0.0.7/tldrwl/register.py
--rw-r--r--   0 jrodal    (1000) jrodal    (1000)     1146 2023-05-22 06:59:34.000000 tldrwl-0.0.7/tldrwl/summarize.py
--rw-r--r--   0 jrodal    (1000) jrodal    (1000)     5288 2023-05-22 08:01:24.000000 tldrwl-0.0.7/tldrwl/summarize_text.py
--rw-r--r--   0 jrodal    (1000) jrodal    (1000)     2147 2023-05-22 06:55:40.000000 tldrwl-0.0.7/tldrwl/summarize_webpage.py
--rw-r--r--   0 jrodal    (1000) jrodal    (1000)     1770 2023-05-22 06:43:53.000000 tldrwl-0.0.7/tldrwl/summarize_youtube.py
-drwxr-xr-x   0 jrodal    (1000) jrodal    (1000)        0 2023-05-22 08:10:35.239869 tldrwl-0.0.7/tldrwl.egg-info/
--rw-r--r--   0 jrodal    (1000) jrodal    (1000)    16598 2023-05-22 08:10:35.000000 tldrwl-0.0.7/tldrwl.egg-info/PKG-INFO
--rw-r--r--   0 jrodal    (1000) jrodal    (1000)      378 2023-05-22 08:10:35.000000 tldrwl-0.0.7/tldrwl.egg-info/SOURCES.txt
--rw-r--r--   0 jrodal    (1000) jrodal    (1000)        1 2023-05-22 08:10:35.000000 tldrwl-0.0.7/tldrwl.egg-info/dependency_links.txt
--rw-r--r--   0 jrodal    (1000) jrodal    (1000)      100 2023-05-22 08:10:35.000000 tldrwl-0.0.7/tldrwl.egg-info/requires.txt
--rw-r--r--   0 jrodal    (1000) jrodal    (1000)        7 2023-05-22 08:10:35.000000 tldrwl-0.0.7/tldrwl.egg-info/top_level.txt
+drwxr-xr-x   0 jrodal    (1000) jrodal    (1000)        0 2023-05-22 08:58:07.389024 tldrwl-0.0.8/
+-rw-r--r--   0 jrodal    (1000) jrodal    (1000)       25 2023-05-22 01:33:23.000000 tldrwl-0.0.8/MANIFEST.in
+-rw-r--r--   0 jrodal    (1000) jrodal    (1000)    16607 2023-05-22 08:58:07.389024 tldrwl-0.0.8/PKG-INFO
+-rw-r--r--   0 jrodal    (1000) jrodal    (1000)    16317 2023-05-22 08:13:51.000000 tldrwl-0.0.8/README.md
+-rw-r--r--   0 jrodal    (1000) jrodal    (1000)      100 2023-05-22 06:20:03.000000 tldrwl-0.0.8/requirements.txt
+-rw-r--r--   0 jrodal    (1000) jrodal    (1000)       38 2023-05-22 08:58:07.389024 tldrwl-0.0.8/setup.cfg
+-rw-r--r--   0 jrodal    (1000) jrodal    (1000)      614 2023-05-22 08:57:57.000000 tldrwl-0.0.8/setup.py
+drwxr-xr-x   0 jrodal    (1000) jrodal    (1000)        0 2023-05-22 08:58:07.389024 tldrwl-0.0.8/tldrwl/
+-rw-r--r--   0 jrodal    (1000) jrodal    (1000)        0 2023-05-22 00:53:22.000000 tldrwl-0.0.8/tldrwl/__init__.py
+-rw-r--r--   0 jrodal    (1000) jrodal    (1000)     1519 2023-05-22 08:55:18.000000 tldrwl-0.0.8/tldrwl/ai_interface.py
+-rw-r--r--   0 jrodal    (1000) jrodal    (1000)     1177 2023-05-22 05:37:32.000000 tldrwl-0.0.8/tldrwl/exception.py
+-rw-r--r--   0 jrodal    (1000) jrodal    (1000)      679 2023-05-22 02:16:47.000000 tldrwl-0.0.8/tldrwl/register.py
+-rw-r--r--   0 jrodal    (1000) jrodal    (1000)     1148 2023-05-22 08:54:03.000000 tldrwl-0.0.8/tldrwl/summarize.py
+-rw-r--r--   0 jrodal    (1000) jrodal    (1000)     5290 2023-05-22 08:54:27.000000 tldrwl-0.0.8/tldrwl/summarize_text.py
+-rw-r--r--   0 jrodal    (1000) jrodal    (1000)     2149 2023-05-22 08:54:42.000000 tldrwl-0.0.8/tldrwl/summarize_webpage.py
+-rw-r--r--   0 jrodal    (1000) jrodal    (1000)     1772 2023-05-22 08:55:00.000000 tldrwl-0.0.8/tldrwl/summarize_youtube.py
+drwxr-xr-x   0 jrodal    (1000) jrodal    (1000)        0 2023-05-22 08:58:07.389024 tldrwl-0.0.8/tldrwl.egg-info/
+-rw-r--r--   0 jrodal    (1000) jrodal    (1000)    16607 2023-05-22 08:58:07.000000 tldrwl-0.0.8/tldrwl.egg-info/PKG-INFO
+-rw-r--r--   0 jrodal    (1000) jrodal    (1000)      378 2023-05-22 08:58:07.000000 tldrwl-0.0.8/tldrwl.egg-info/SOURCES.txt
+-rw-r--r--   0 jrodal    (1000) jrodal    (1000)        1 2023-05-22 08:58:07.000000 tldrwl-0.0.8/tldrwl.egg-info/dependency_links.txt
+-rw-r--r--   0 jrodal    (1000) jrodal    (1000)      100 2023-05-22 08:58:07.000000 tldrwl-0.0.8/tldrwl.egg-info/requires.txt
+-rw-r--r--   0 jrodal    (1000) jrodal    (1000)        7 2023-05-22 08:58:07.000000 tldrwl-0.0.8/tldrwl.egg-info/top_level.txt
```

### Comparing `tldrwl-0.0.7/PKG-INFO` & `tldrwl-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tldrwl
-Version: 0.0.7
+Version: 0.0.8
 Summary: Too long, didn't read/watch/listen
 Home-page: https://github.com/jrodal98/tldrwl
 Author: Jacob Rodal
 Author-email: dev@jrodal.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.8
@@ -22,15 +22,14 @@
 
 Summarize webpages, Youtube videos, and texts with a single api call:
 
 ```
 from tldrwl.summarize import Summarizer
 Summarizer().summarize_sync("<webpage url | youtube url | text>")
 await Summarizer().summarize_async("<webpage url | youtube url | text>")
-
 ```
 
 Example:
 
 ```
 >>> from tldrwl.summarize import Summarizer
 >>> summary = Summarizer().summarize_sync("https://www.youtube.com/watch?v=--khbXchTeE")
@@ -45,14 +44,15 @@
 - [x] Summarize text with a single API call
 - [x] Summarize webpages with a single API call
 - [x] Summarize Youtube videos with a single API call
 - [x] Report number of tokens + cost per request
 - [x] Sync APIs
 - [x] Async APIs - **much faster than the sync api!**
 - [ ] Summarize audio with a single API call
+- [ ] CLI
 
 ## Caveats
 
 - Requires an OpenAI API key
   - Export to env: `export OPENAI_API_KEY="<your api key here>"`
 - Slow
   - Small articles take ~20 seconds, longer articles and videos take a few minutes. **Prefer the async API, as that is much faster**. There is probably some more optimization to be had.
```

### Comparing `tldrwl-0.0.7/README.md` & `tldrwl-0.0.8/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 
 Summarize webpages, Youtube videos, and texts with a single api call:
 
 ```
 from tldrwl.summarize import Summarizer
 Summarizer().summarize_sync("<webpage url | youtube url | text>")
 await Summarizer().summarize_async("<webpage url | youtube url | text>")
-
 ```
 
 Example:
 
 ```
 >>> from tldrwl.summarize import Summarizer
 >>> summary = Summarizer().summarize_sync("https://www.youtube.com/watch?v=--khbXchTeE")
@@ -33,14 +32,15 @@
 - [x] Summarize text with a single API call
 - [x] Summarize webpages with a single API call
 - [x] Summarize Youtube videos with a single API call
 - [x] Report number of tokens + cost per request
 - [x] Sync APIs
 - [x] Async APIs - **much faster than the sync api!**
 - [ ] Summarize audio with a single API call
+- [ ] CLI
 
 ## Caveats
 
 - Requires an OpenAI API key
   - Export to env: `export OPENAI_API_KEY="<your api key here>"`
 - Slow
   - Small articles take ~20 seconds, longer articles and videos take a few minutes. **Prefer the async API, as that is much faster**. There is probably some more optimization to be had.
```

### Comparing `tldrwl-0.0.7/setup.py` & `tldrwl-0.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = f.read()
 
 with open("requirements.txt") as f:
     install_requires = f.read().splitlines()
 
 setuptools.setup(
     name="tldrwl",
-    version="0.0.7",
+    version="0.0.8",
     author="Jacob Rodal",
     author_email="dev@jrodal.com",
     description="Too long, didn't read/watch/listen",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/jrodal98/tldrwl",
     packages=setuptools.find_packages(),
```

### Comparing `tldrwl-0.0.7/tldrwl/exception.py` & `tldrwl-0.0.8/tldrwl/exception.py`

 * *Files identical despite different names*

### Comparing `tldrwl-0.0.7/tldrwl/register.py` & `tldrwl-0.0.8/tldrwl/register.py`

 * *Files identical despite different names*

### Comparing `tldrwl-0.0.7/tldrwl/summarize.py` & `tldrwl-0.0.8/tldrwl/summarize.py`

 * *Files 7% similar despite different names*

```diff
@@ -21,14 +21,14 @@
         elif WebpageSummarizer.is_url(text):
             self._logger.debug("Using WebpageSummarizer")
             return WebpageSummarizer()
         else:
             self._logger.debug("Using TextSummarizer")
             return TextSummarizer()
 
-    async def summarize_async(self, text: str) -> Summary:
+    async def _summarize_async(self, text: str) -> Summary:
         summarizer = self.get_summarizer(text)
         return await summarizer.summarize_async(text)
 
-    def summarize_sync(self, text: str) -> Summary:
+    def _summarize_sync(self, text: str) -> Summary:
         summarizer = self.get_summarizer(text)
         return summarizer.summarize_sync(text)
```

### Comparing `tldrwl-0.0.7/tldrwl/summarize_text.py` & `tldrwl-0.0.8/tldrwl/summarize_text.py`

 * *Files 2% similar despite different names*

```diff
@@ -89,15 +89,15 @@
 
         chunks = textwrap.wrap(text, self._chunk_size)[: self._max_num_chunks]
         num_chunks = len(chunks)
         self._logger.debug(f"{num_chunks=}")
 
         return chunks
 
-    async def summarize_async(self, text: str) -> Summary:
+    async def _summarize_async(self, text: str) -> Summary:
         chunks = self._get_chunks(text)
         summaries = await asyncio.gather(
             *[self._summarize_chunk_async(chunk, max_tokens=250) for chunk in chunks]
         )
         if len(summaries) == 0:
             return Summary(text="", num_tokens=0, model=self._model)
         elif len(summaries) == 1:
@@ -113,15 +113,15 @@
             return Summary(
                 text=final_summary.text,
                 num_tokens=final_summary.num_tokens
                 + sum(s.num_tokens for s in summaries),
                 model=self._model,
             )
 
-    def summarize_sync(self, text: str) -> Summary:
+    def _summarize_sync(self, text: str) -> Summary:
         chunks = self._get_chunks(text)
 
         summaries = [self._summarize_chunk(chunk, max_tokens=250) for chunk in chunks]
         if len(summaries) == 0:
             return Summary(text="", num_tokens=0, model=self._model)
         elif len(summaries) == 1:
             return summaries[0]
```

### Comparing `tldrwl-0.0.7/tldrwl/summarize_webpage.py` & `tldrwl-0.0.8/tldrwl/summarize_webpage.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,14 +47,14 @@
             async with session.get(url) as response:
                 response.raise_for_status()
                 soup = bs4.BeautifulSoup(await response.text(), "html.parser")
                 page_text = soup.get_text()
                 self._logger.debug(f"Done getting page text for {url}")
                 return page_text
 
-    async def summarize_async(self, text: str) -> Summary:
+    async def _summarize_async(self, text: str) -> Summary:
         page_text = await self._get_page_text_async(text)
         return await self._text_summarizer.summarize_async(page_text)
 
-    def summarize_sync(self, text: str) -> Summary:
+    def _summarize_sync(self, text: str) -> Summary:
         page_text = self._get_page_text(text)
         return self._text_summarizer.summarize_sync(page_text)
```

### Comparing `tldrwl-0.0.7/tldrwl/summarize_youtube.py` & `tldrwl-0.0.8/tldrwl/summarize_youtube.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,14 +35,14 @@
         if not video_id:
             raise TldrwlVideoUrlParsingException.make_error(video_url=url)
         self._logger.debug(f"Getting transcript for {video_id}")
         transcript = YouTubeTranscriptApi.get_transcript(video_id)  # type: ignore
         self._logger.debug(f"Done getting transcript for {video_id}")
         return TextFormatter().format_transcript(transcript)  # type: ignore
 
-    async def summarize_async(self, text: str) -> Summary:
+    async def _summarize_async(self, text: str) -> Summary:
         transcript = self._get_video_transcript(text)
         return await self._text_summarizer.summarize_async(transcript)
 
-    def summarize_sync(self, text: str) -> Summary:
+    def _summarize_sync(self, text: str) -> Summary:
         transcript = self._get_video_transcript(text)
         return self._text_summarizer.summarize_sync(transcript)
```

### Comparing `tldrwl-0.0.7/tldrwl.egg-info/PKG-INFO` & `tldrwl-0.0.8/tldrwl.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tldrwl
-Version: 0.0.7
+Version: 0.0.8
 Summary: Too long, didn't read/watch/listen
 Home-page: https://github.com/jrodal98/tldrwl
 Author: Jacob Rodal
 Author-email: dev@jrodal.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.8
@@ -22,15 +22,14 @@
 
 Summarize webpages, Youtube videos, and texts with a single api call:
 
 ```
 from tldrwl.summarize import Summarizer
 Summarizer().summarize_sync("<webpage url | youtube url | text>")
 await Summarizer().summarize_async("<webpage url | youtube url | text>")
-
 ```
 
 Example:
 
 ```
 >>> from tldrwl.summarize import Summarizer
 >>> summary = Summarizer().summarize_sync("https://www.youtube.com/watch?v=--khbXchTeE")
@@ -45,14 +44,15 @@
 - [x] Summarize text with a single API call
 - [x] Summarize webpages with a single API call
 - [x] Summarize Youtube videos with a single API call
 - [x] Report number of tokens + cost per request
 - [x] Sync APIs
 - [x] Async APIs - **much faster than the sync api!**
 - [ ] Summarize audio with a single API call
+- [ ] CLI
 
 ## Caveats
 
 - Requires an OpenAI API key
   - Export to env: `export OPENAI_API_KEY="<your api key here>"`
 - Slow
   - Small articles take ~20 seconds, longer articles and videos take a few minutes. **Prefer the async API, as that is much faster**. There is probably some more optimization to be had.
```

