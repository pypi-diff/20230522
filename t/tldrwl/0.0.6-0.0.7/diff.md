# Comparing `tmp/tldrwl-0.0.6.tar.gz` & `tmp/tldrwl-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tldrwl-0.0.6.tar", last modified: Mon May 22 07:37:29 2023, max compression
+gzip compressed data, was "tldrwl-0.0.7.tar", last modified: Mon May 22 08:10:35 2023, max compression
```

## Comparing `tldrwl-0.0.6.tar` & `tldrwl-0.0.7.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 jrodal    (1000) jrodal    (1000)        0 2023-05-22 07:37:29.810449 tldrwl-0.0.6/
--rw-r--r--   0 jrodal    (1000) jrodal    (1000)       25 2023-05-22 01:33:23.000000 tldrwl-0.0.6/MANIFEST.in
--rw-r--r--   0 jrodal    (1000) jrodal    (1000)    12006 2023-05-22 07:37:29.810449 tldrwl-0.0.6/PKG-INFO
--rw-r--r--   0 jrodal    (1000) jrodal    (1000)    11716 2023-05-22 07:29:21.000000 tldrwl-0.0.6/README.md
--rw-r--r--   0 jrodal    (1000) jrodal    (1000)      100 2023-05-22 06:20:03.000000 tldrwl-0.0.6/requirements.txt
--rw-r--r--   0 jrodal    (1000) jrodal    (1000)       38 2023-05-22 07:37:29.810449 tldrwl-0.0.6/setup.cfg
--rw-r--r--   0 jrodal    (1000) jrodal    (1000)      614 2023-05-22 07:37:15.000000 tldrwl-0.0.6/setup.py
-drwxr-xr-x   0 jrodal    (1000) jrodal    (1000)        0 2023-05-22 07:37:29.810449 tldrwl-0.0.6/tldrwl/
--rw-r--r--   0 jrodal    (1000) jrodal    (1000)        0 2023-05-22 00:53:22.000000 tldrwl-0.0.6/tldrwl/__init__.py
--rw-r--r--   0 jrodal    (1000) jrodal    (1000)      907 2023-05-22 06:42:51.000000 tldrwl-0.0.6/tldrwl/ai_interface.py
--rw-r--r--   0 jrodal    (1000) jrodal    (1000)     1177 2023-05-22 05:37:32.000000 tldrwl-0.0.6/tldrwl/exception.py
--rw-r--r--   0 jrodal    (1000) jrodal    (1000)      679 2023-05-22 02:16:47.000000 tldrwl-0.0.6/tldrwl/register.py
--rw-r--r--   0 jrodal    (1000) jrodal    (1000)     1146 2023-05-22 06:59:34.000000 tldrwl-0.0.6/tldrwl/summarize.py
--rw-r--r--   0 jrodal    (1000) jrodal    (1000)     4811 2023-05-22 07:36:42.000000 tldrwl-0.0.6/tldrwl/summarize_text.py
--rw-r--r--   0 jrodal    (1000) jrodal    (1000)     2147 2023-05-22 06:55:40.000000 tldrwl-0.0.6/tldrwl/summarize_webpage.py
--rw-r--r--   0 jrodal    (1000) jrodal    (1000)     1770 2023-05-22 06:43:53.000000 tldrwl-0.0.6/tldrwl/summarize_youtube.py
-drwxr-xr-x   0 jrodal    (1000) jrodal    (1000)        0 2023-05-22 07:37:29.810449 tldrwl-0.0.6/tldrwl.egg-info/
--rw-r--r--   0 jrodal    (1000) jrodal    (1000)    12006 2023-05-22 07:37:29.000000 tldrwl-0.0.6/tldrwl.egg-info/PKG-INFO
--rw-r--r--   0 jrodal    (1000) jrodal    (1000)      378 2023-05-22 07:37:29.000000 tldrwl-0.0.6/tldrwl.egg-info/SOURCES.txt
--rw-r--r--   0 jrodal    (1000) jrodal    (1000)        1 2023-05-22 07:37:29.000000 tldrwl-0.0.6/tldrwl.egg-info/dependency_links.txt
--rw-r--r--   0 jrodal    (1000) jrodal    (1000)      100 2023-05-22 07:37:29.000000 tldrwl-0.0.6/tldrwl.egg-info/requires.txt
--rw-r--r--   0 jrodal    (1000) jrodal    (1000)        7 2023-05-22 07:37:29.000000 tldrwl-0.0.6/tldrwl.egg-info/top_level.txt
+drwxr-xr-x   0 jrodal    (1000) jrodal    (1000)        0 2023-05-22 08:10:35.239869 tldrwl-0.0.7/
+-rw-r--r--   0 jrodal    (1000) jrodal    (1000)       25 2023-05-22 01:33:23.000000 tldrwl-0.0.7/MANIFEST.in
+-rw-r--r--   0 jrodal    (1000) jrodal    (1000)    16598 2023-05-22 08:10:35.239869 tldrwl-0.0.7/PKG-INFO
+-rw-r--r--   0 jrodal    (1000) jrodal    (1000)    16308 2023-05-22 08:10:00.000000 tldrwl-0.0.7/README.md
+-rw-r--r--   0 jrodal    (1000) jrodal    (1000)      100 2023-05-22 06:20:03.000000 tldrwl-0.0.7/requirements.txt
+-rw-r--r--   0 jrodal    (1000) jrodal    (1000)       38 2023-05-22 08:10:35.239869 tldrwl-0.0.7/setup.cfg
+-rw-r--r--   0 jrodal    (1000) jrodal    (1000)      614 2023-05-22 08:10:20.000000 tldrwl-0.0.7/setup.py
+drwxr-xr-x   0 jrodal    (1000) jrodal    (1000)        0 2023-05-22 08:10:35.239869 tldrwl-0.0.7/tldrwl/
+-rw-r--r--   0 jrodal    (1000) jrodal    (1000)        0 2023-05-22 00:53:22.000000 tldrwl-0.0.7/tldrwl/__init__.py
+-rw-r--r--   0 jrodal    (1000) jrodal    (1000)      907 2023-05-22 06:42:51.000000 tldrwl-0.0.7/tldrwl/ai_interface.py
+-rw-r--r--   0 jrodal    (1000) jrodal    (1000)     1177 2023-05-22 05:37:32.000000 tldrwl-0.0.7/tldrwl/exception.py
+-rw-r--r--   0 jrodal    (1000) jrodal    (1000)      679 2023-05-22 02:16:47.000000 tldrwl-0.0.7/tldrwl/register.py
+-rw-r--r--   0 jrodal    (1000) jrodal    (1000)     1146 2023-05-22 06:59:34.000000 tldrwl-0.0.7/tldrwl/summarize.py
+-rw-r--r--   0 jrodal    (1000) jrodal    (1000)     5288 2023-05-22 08:01:24.000000 tldrwl-0.0.7/tldrwl/summarize_text.py
+-rw-r--r--   0 jrodal    (1000) jrodal    (1000)     2147 2023-05-22 06:55:40.000000 tldrwl-0.0.7/tldrwl/summarize_webpage.py
+-rw-r--r--   0 jrodal    (1000) jrodal    (1000)     1770 2023-05-22 06:43:53.000000 tldrwl-0.0.7/tldrwl/summarize_youtube.py
+drwxr-xr-x   0 jrodal    (1000) jrodal    (1000)        0 2023-05-22 08:10:35.239869 tldrwl-0.0.7/tldrwl.egg-info/
+-rw-r--r--   0 jrodal    (1000) jrodal    (1000)    16598 2023-05-22 08:10:35.000000 tldrwl-0.0.7/tldrwl.egg-info/PKG-INFO
+-rw-r--r--   0 jrodal    (1000) jrodal    (1000)      378 2023-05-22 08:10:35.000000 tldrwl-0.0.7/tldrwl.egg-info/SOURCES.txt
+-rw-r--r--   0 jrodal    (1000) jrodal    (1000)        1 2023-05-22 08:10:35.000000 tldrwl-0.0.7/tldrwl.egg-info/dependency_links.txt
+-rw-r--r--   0 jrodal    (1000) jrodal    (1000)      100 2023-05-22 08:10:35.000000 tldrwl-0.0.7/tldrwl.egg-info/requires.txt
+-rw-r--r--   0 jrodal    (1000) jrodal    (1000)        7 2023-05-22 08:10:35.000000 tldrwl-0.0.7/tldrwl.egg-info/top_level.txt
```

### Comparing `tldrwl-0.0.6/PKG-INFO` & `tldrwl-0.0.7/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,32 +1,29 @@
-Metadata-Version: 2.1
-Name: tldrwl
-Version: 0.0.6
-Summary: Too long, didn't read/watch/listen
-Home-page: https://github.com/jrodal98/tldrwl
-Author: Jacob Rodal
-Author-email: dev@jrodal.com
-License: UNKNOWN
-Platform: UNKNOWN
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-
 # tldrwl (too long, didn't read/watch/listen)
 
 ## Install
 
 ```
 pip install tldrwl
 ```
 
 ## About
 
 Summarize webpages, Youtube videos, and texts with a single api call:
 
 ```
+from tldrwl.summarize import Summarizer
+Summarizer().summarize_sync("<webpage url | youtube url | text>")
+await Summarizer().summarize_async("<webpage url | youtube url | text>")
+
+```
+
+Example:
+
+```
 >>> from tldrwl.summarize import Summarizer
 >>> summary = Summarizer().summarize_sync("https://www.youtube.com/watch?v=--khbXchTeE")
 >>> print(summary)
 Summary(text="OpenAI's GPT-4 is an advanced AI system that can generate up to 25,000 words of text and understand images to express logical ideas about them. Despite its imperfections, it has great potential to add value to everyday life, especially in the field of education, where it can act as a personal math tutor or teach a wide range of subjects. OpenAI and Microsoft are partnering to shape this technology so that it's beneficial to society. The AI's development is an accumulation of all past technological advancements and opens up possibilities for successors with more capabilities. OpenAI recognizes the importance of making the technology useful to everyone, not just early adopters, and thus encourages participation to learn how it can be helpful. The team has put in place internal guardrails for safety and privacy concerns and will continue to learn and improve.", num_tokens=793, model=<Model.GPT35TURBO: 'gpt-3.5-turbo'>)
 >>> print(f"{summary.estimated_cost_usd=}")
 summary.estimated_cost_usd=0.0015860000000000002
 ```
@@ -34,23 +31,39 @@
 ## Features
 
 - [x] Summarize text with a single API call
 - [x] Summarize webpages with a single API call
 - [x] Summarize Youtube videos with a single API call
 - [x] Report number of tokens + cost per request
 - [x] Sync APIs
-- [x] Async APIs
+- [x] Async APIs - **much faster than the sync api!**
 - [ ] Summarize audio with a single API call
 
 ## Caveats
 
 - Requires an OpenAI API key
   - Export to env: `export OPENAI_API_KEY="<your api key here>"`
 - Slow
-  - Small articles take ~20 seconds, longer articles and videos take minutes. There is probably some optimization to be had.
+  - Small articles take ~20 seconds, longer articles and videos take a few minutes. **Prefer the async API, as that is much faster**. There is probably some more optimization to be had.
+- Cost
+  - Can be expensive - by default, this uses the "gpt-3.5-turbo" model, which costs $0.002 / 1000 tokens. In the future, I may make the model customizable to allow for cheaper models.
+  - To minimize cost, the library currently limits the number of input characters to 120,000. This limits the cost of a request to a maximum of ~$0.062. In the future, I may add a flag to modify or remove this limit.
+
+To illustrate speed and cost: [This wikipedia page](https://en.wikipedia.org/wiki/List_of_common_misconceptions) hits the maximum limit:
+
+```
+Running async
+Summary(text='The Wikipedia page "List of common misconceptions" provides a comprehensive list of popular misconceptions and myths in various fields, including arts and culture, business, food and cooking, history, science and mathematics, and film and television. The page corrects commonly held false beliefs that arise from old wives\' tales, superstitions, pseudoscience, and fallacies, among others. The page is divided into sections that relate to different areas of knowledge with listed misconceptions and concise corrections. The page is dynamic and can be regularly updated by readers with reliable sources, and encourages people to be critical of information presented to distinguish fact from fiction. The article debunks several popular myths across fields, including the belief that Santa Claus\'s current image was created by The Coca-Cola Company, the association of the term "zombie" with beings from the film Dawn of the Dead, and the myth that Eskimos have a disproportionate number of words for snow. It also clarifies that sign languages are not universal, and each country has its own native sign language, and police officers are allowed to lie during undercover work. The page corrects misconceptions related to religion and history, such as Mary\'s immaculate conception, the paternity of Paul the Apostle, and the belief that the First Council of Nicaea established the books of the Bible. Additionally, the page debunks common historical myths, such as the belief that Christopher Columbus believed in a flat Earth and that the Plymouth Colony settlers wore Puritan attire. The page covers several misconceptions related to biology, evolution and paleontology, including the myth that cockroaches are radiation-resistant and that honey bees are essential to human food production. It also clarifies common misconceptions related to healthcare and nutrition, such as the belief that exercise-induced muscle soreness is caused by lactic acid build-up and that covering the head prevents heat loss more effectively than other body parts. The page concludes by emphasizing the importance of distinguishing fact from fiction and being critical of information presented.', num_tokens=30749, model=<Model.GPT35TURBO: 'gpt-3.5-turbo'>)
+summary.estimated_cost_usd=0.061498000000000004
+Finished async in 108.65759706497192s
+Running sync
+Summary(text='The Wikipedia page on common misconceptions offers a comprehensive list of erroneous beliefs that people commonly hold in various fields such as arts and culture, business, food and cooking, science, mathematics, history, and more. The entries on the list are written as corrections of the misconceptions rather than statements of the myths themselves, and the page provides concise summaries with links to relevant articles for more elaboration. The page covers a plethora of topics from the history of Santa Claus to the spicy part of chili peppers, from legal tender laws to the tryptophan content of turkey. The page also debunks numerous myths related to film and television, language, and law, among other things. Other articles discussed on the Wikipedia page cover particular topics, such as debunking common misconceptions surrounding notable figures in history and religion, as well as science and evolution. Additional articles cover misconceptions in areas such as computing and the internet, geography, and health and nutrition. Overall, the Wikipedia page on common misconceptions serves as a valuable resource for people interested in exploring and dispelling common untruths across a wide range of fields.', num_tokens=30203, model=<Model.GPT35TURBO: 'gpt-3.5-turbo'>)
+summary.estimated_cost_usd=0.060406
+Finished sync in 316.76091599464417s
+```
 
 ## General Approach
 
 OpenAI has a limit on maximum number of tokens per requests, so the following strategy is employed to generate the summaries:
 
 1. Split message into chunks
 2. Gather summaries for each chunk
@@ -114,9 +127,7 @@
 
 ## Contributing
 
 1. Setup a virtual env `python3 -m venv .venv`
 2. Activate venv `source .venv/bin/activate`
 3. Install requirements to venv `pip install -r requirements.txt`
 4. Setup local import path resolution `make develop`
-
-
```

### Comparing `tldrwl-0.0.6/setup.py` & `tldrwl-0.0.7/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = f.read()
 
 with open("requirements.txt") as f:
     install_requires = f.read().splitlines()
 
 setuptools.setup(
     name="tldrwl",
-    version="0.0.6",
+    version="0.0.7",
     author="Jacob Rodal",
     author_email="dev@jrodal.com",
     description="Too long, didn't read/watch/listen",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/jrodal98/tldrwl",
     packages=setuptools.find_packages(),
```

### Comparing `tldrwl-0.0.6/tldrwl/ai_interface.py` & `tldrwl-0.0.7/tldrwl/ai_interface.py`

 * *Files identical despite different names*

### Comparing `tldrwl-0.0.6/tldrwl/exception.py` & `tldrwl-0.0.7/tldrwl/exception.py`

 * *Files identical despite different names*

### Comparing `tldrwl-0.0.6/tldrwl/register.py` & `tldrwl-0.0.7/tldrwl/register.py`

 * *Files identical despite different names*

### Comparing `tldrwl-0.0.6/tldrwl/summarize.py` & `tldrwl-0.0.7/tldrwl/summarize.py`

 * *Files identical despite different names*

### Comparing `tldrwl-0.0.6/tldrwl/summarize_text.py` & `tldrwl-0.0.7/tldrwl/summarize_text.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,23 +8,25 @@
 import textwrap
 
 import openai
 from typing import List, Dict, Any
 
 from .ai_interface import AiInterface, Model, Summary
 
+MAX_TOKEN_RESPONSE = 1500
+
 
 class TextSummarizer(AiInterface):
     def __init__(
         self,
         *,
         model: Model = Model.GPT35TURBO,
         prompt_string: str = "Write a detailed summary of the following:\n\n{}\n",
-        chunk_size: int = 8000,
-        max_num_chunks: int = 15,
+        chunk_size: int = 12000,
+        max_num_chunks: int = 10,
     ) -> None:
         super().__init__()
         self._model = model
         self._prompt_string = prompt_string
         self._chunk_size = chunk_size
         self._max_num_chunks = max_num_chunks
         self._logger = logging.getLogger(__name__)
@@ -98,16 +100,19 @@
         )
         if len(summaries) == 0:
             return Summary(text="", num_tokens=0, model=self._model)
         elif len(summaries) == 1:
             return summaries[0]
         else:
             final_input = " ".join(s.text for s in summaries)
+            # TODO: recursively summarize if it is still too big instead
+            # of hoping that this will work - maybe catch this exception?
+            # noqa openai.error.InvalidRequestError: This model's maximum context length is 4097 tokens. However, you requested 4612 tokens (3112 in the messages, 1500 in the completion). Please reduce the length of the messages or completion.
             final_summary = await self._summarize_chunk_async(
-                final_input, max_tokens=1500
+                final_input, max_tokens=MAX_TOKEN_RESPONSE
             )
             return Summary(
                 text=final_summary.text,
                 num_tokens=final_summary.num_tokens
                 + sum(s.num_tokens for s in summaries),
                 model=self._model,
             )
@@ -118,14 +123,16 @@
         summaries = [self._summarize_chunk(chunk, max_tokens=250) for chunk in chunks]
         if len(summaries) == 0:
             return Summary(text="", num_tokens=0, model=self._model)
         elif len(summaries) == 1:
             return summaries[0]
         else:
             final_input = " ".join(s.text for s in summaries)
-            final_summary = self._summarize_chunk(final_input, max_tokens=2000)
+            final_summary = self._summarize_chunk(
+                final_input, max_tokens=MAX_TOKEN_RESPONSE
+            )
             return Summary(
                 text=final_summary.text,
                 num_tokens=final_summary.num_tokens
                 + sum(s.num_tokens for s in summaries),
                 model=self._model,
             )
```

### Comparing `tldrwl-0.0.6/tldrwl/summarize_webpage.py` & `tldrwl-0.0.7/tldrwl/summarize_webpage.py`

 * *Files identical despite different names*

### Comparing `tldrwl-0.0.6/tldrwl/summarize_youtube.py` & `tldrwl-0.0.7/tldrwl/summarize_youtube.py`

 * *Files identical despite different names*

### Comparing `tldrwl-0.0.6/tldrwl.egg-info/PKG-INFO` & `tldrwl-0.0.7/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tldrwl
-Version: 0.0.6
+Version: 0.0.7
 Summary: Too long, didn't read/watch/listen
 Home-page: https://github.com/jrodal98/tldrwl
 Author: Jacob Rodal
 Author-email: dev@jrodal.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.8
@@ -19,14 +19,23 @@
 ```
 
 ## About
 
 Summarize webpages, Youtube videos, and texts with a single api call:
 
 ```
+from tldrwl.summarize import Summarizer
+Summarizer().summarize_sync("<webpage url | youtube url | text>")
+await Summarizer().summarize_async("<webpage url | youtube url | text>")
+
+```
+
+Example:
+
+```
 >>> from tldrwl.summarize import Summarizer
 >>> summary = Summarizer().summarize_sync("https://www.youtube.com/watch?v=--khbXchTeE")
 >>> print(summary)
 Summary(text="OpenAI's GPT-4 is an advanced AI system that can generate up to 25,000 words of text and understand images to express logical ideas about them. Despite its imperfections, it has great potential to add value to everyday life, especially in the field of education, where it can act as a personal math tutor or teach a wide range of subjects. OpenAI and Microsoft are partnering to shape this technology so that it's beneficial to society. The AI's development is an accumulation of all past technological advancements and opens up possibilities for successors with more capabilities. OpenAI recognizes the importance of making the technology useful to everyone, not just early adopters, and thus encourages participation to learn how it can be helpful. The team has put in place internal guardrails for safety and privacy concerns and will continue to learn and improve.", num_tokens=793, model=<Model.GPT35TURBO: 'gpt-3.5-turbo'>)
 >>> print(f"{summary.estimated_cost_usd=}")
 summary.estimated_cost_usd=0.0015860000000000002
 ```
@@ -34,23 +43,39 @@
 ## Features
 
 - [x] Summarize text with a single API call
 - [x] Summarize webpages with a single API call
 - [x] Summarize Youtube videos with a single API call
 - [x] Report number of tokens + cost per request
 - [x] Sync APIs
-- [x] Async APIs
+- [x] Async APIs - **much faster than the sync api!**
 - [ ] Summarize audio with a single API call
 
 ## Caveats
 
 - Requires an OpenAI API key
   - Export to env: `export OPENAI_API_KEY="<your api key here>"`
 - Slow
-  - Small articles take ~20 seconds, longer articles and videos take minutes. There is probably some optimization to be had.
+  - Small articles take ~20 seconds, longer articles and videos take a few minutes. **Prefer the async API, as that is much faster**. There is probably some more optimization to be had.
+- Cost
+  - Can be expensive - by default, this uses the "gpt-3.5-turbo" model, which costs $0.002 / 1000 tokens. In the future, I may make the model customizable to allow for cheaper models.
+  - To minimize cost, the library currently limits the number of input characters to 120,000. This limits the cost of a request to a maximum of ~$0.062. In the future, I may add a flag to modify or remove this limit.
+
+To illustrate speed and cost: [This wikipedia page](https://en.wikipedia.org/wiki/List_of_common_misconceptions) hits the maximum limit:
+
+```
+Running async
+Summary(text='The Wikipedia page "List of common misconceptions" provides a comprehensive list of popular misconceptions and myths in various fields, including arts and culture, business, food and cooking, history, science and mathematics, and film and television. The page corrects commonly held false beliefs that arise from old wives\' tales, superstitions, pseudoscience, and fallacies, among others. The page is divided into sections that relate to different areas of knowledge with listed misconceptions and concise corrections. The page is dynamic and can be regularly updated by readers with reliable sources, and encourages people to be critical of information presented to distinguish fact from fiction. The article debunks several popular myths across fields, including the belief that Santa Claus\'s current image was created by The Coca-Cola Company, the association of the term "zombie" with beings from the film Dawn of the Dead, and the myth that Eskimos have a disproportionate number of words for snow. It also clarifies that sign languages are not universal, and each country has its own native sign language, and police officers are allowed to lie during undercover work. The page corrects misconceptions related to religion and history, such as Mary\'s immaculate conception, the paternity of Paul the Apostle, and the belief that the First Council of Nicaea established the books of the Bible. Additionally, the page debunks common historical myths, such as the belief that Christopher Columbus believed in a flat Earth and that the Plymouth Colony settlers wore Puritan attire. The page covers several misconceptions related to biology, evolution and paleontology, including the myth that cockroaches are radiation-resistant and that honey bees are essential to human food production. It also clarifies common misconceptions related to healthcare and nutrition, such as the belief that exercise-induced muscle soreness is caused by lactic acid build-up and that covering the head prevents heat loss more effectively than other body parts. The page concludes by emphasizing the importance of distinguishing fact from fiction and being critical of information presented.', num_tokens=30749, model=<Model.GPT35TURBO: 'gpt-3.5-turbo'>)
+summary.estimated_cost_usd=0.061498000000000004
+Finished async in 108.65759706497192s
+Running sync
+Summary(text='The Wikipedia page on common misconceptions offers a comprehensive list of erroneous beliefs that people commonly hold in various fields such as arts and culture, business, food and cooking, science, mathematics, history, and more. The entries on the list are written as corrections of the misconceptions rather than statements of the myths themselves, and the page provides concise summaries with links to relevant articles for more elaboration. The page covers a plethora of topics from the history of Santa Claus to the spicy part of chili peppers, from legal tender laws to the tryptophan content of turkey. The page also debunks numerous myths related to film and television, language, and law, among other things. Other articles discussed on the Wikipedia page cover particular topics, such as debunking common misconceptions surrounding notable figures in history and religion, as well as science and evolution. Additional articles cover misconceptions in areas such as computing and the internet, geography, and health and nutrition. Overall, the Wikipedia page on common misconceptions serves as a valuable resource for people interested in exploring and dispelling common untruths across a wide range of fields.', num_tokens=30203, model=<Model.GPT35TURBO: 'gpt-3.5-turbo'>)
+summary.estimated_cost_usd=0.060406
+Finished sync in 316.76091599464417s
+```
 
 ## General Approach
 
 OpenAI has a limit on maximum number of tokens per requests, so the following strategy is employed to generate the summaries:
 
 1. Split message into chunks
 2. Gather summaries for each chunk
```

