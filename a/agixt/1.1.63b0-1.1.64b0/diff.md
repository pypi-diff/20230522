# Comparing `tmp/agixt-1.1.63b0.tar.gz` & `tmp/agixt-1.1.64b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agixt-1.1.63b0.tar", last modified: Mon May 22 00:28:31 2023, max compression
+gzip compressed data, was "agixt-1.1.64b0.tar", last modified: Mon May 22 00:58:50 2023, max compression
```

## Comparing `agixt-1.1.63b0.tar` & `agixt-1.1.64b0.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 00:28:31.418599 agixt-1.1.63b0/
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-05-22 00:28:19.000000 agixt-1.1.63b0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-22 00:28:19.000000 agixt-1.1.63b0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    13861 2023-05-22 00:28:31.414599 agixt-1.1.63b0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 00:28:31.410599 agixt-1.1.63b0/agixt/
--rw-r--r--   0 runner    (1001) docker     (123)    16067 2023-05-22 00:28:19.000000 agixt-1.1.63b0/agixt/AGiXT.py
--rw-r--r--   0 runner    (1001) docker     (123)    12848 2023-05-22 00:28:19.000000 agixt-1.1.63b0/agixt/Agent.py
--rw-r--r--   0 runner    (1001) docker     (123)     5075 2023-05-22 00:28:19.000000 agixt-1.1.63b0/agixt/Chain.py
--rw-r--r--   0 runner    (1001) docker     (123)     6153 2023-05-22 00:28:19.000000 agixt-1.1.63b0/agixt/Commands.py
--rw-r--r--   0 runner    (1001) docker     (123)      960 2023-05-22 00:28:19.000000 agixt-1.1.63b0/agixt/Config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-05-22 00:28:19.000000 agixt-1.1.63b0/agixt/CustomPrompt.py
--rw-r--r--   0 runner    (1001) docker     (123)     6337 2023-05-22 00:28:19.000000 agixt-1.1.63b0/agixt/Embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-05-22 00:28:19.000000 agixt-1.1.63b0/agixt/Main.py
--rw-r--r--   0 runner    (1001) docker     (123)     8367 2023-05-22 00:28:19.000000 agixt-1.1.63b0/agixt/Memories.py
--rw-r--r--   0 runner    (1001) docker     (123)     8476 2023-05-22 00:28:19.000000 agixt-1.1.63b0/agixt/Tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-05-22 00:28:19.000000 agixt-1.1.63b0/agixt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12961 2023-05-22 00:28:19.000000 agixt-1.1.63b0/agixt/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 00:28:31.414599 agixt-1.1.63b0/agixt/provider/
--rw-r--r--   0 runner    (1001) docker     (123)     2157 2023-05-22 00:28:19.000000 agixt-1.1.63b0/agixt/provider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-05-22 00:28:19.000000 agixt-1.1.63b0/agixt/provider/azure.py
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-05-22 00:28:19.000000 agixt-1.1.63b0/agixt/provider/bard.py
--rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-05-22 00:28:19.000000 agixt-1.1.63b0/agixt/provider/bing.py
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-05-22 00:28:19.000000 agixt-1.1.63b0/agixt/provider/chatgpt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-05-22 00:28:19.000000 agixt-1.1.63b0/agixt/provider/claude.py
--rw-r--r--   0 runner    (1001) docker     (123)      757 2023-05-22 00:28:19.000000 agixt-1.1.63b0/agixt/provider/fastchat.py
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-05-22 00:28:19.000000 agixt-1.1.63b0/agixt/provider/gpt4all.py
--rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-05-22 00:28:19.000000 agixt-1.1.63b0/agixt/provider/gpt4free.py
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-22 00:28:19.000000 agixt-1.1.63b0/agixt/provider/gpugpt4all.py
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-05-22 00:28:19.000000 agixt-1.1.63b0/agixt/provider/huggingchat.py
--rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-05-22 00:28:19.000000 agixt-1.1.63b0/agixt/provider/kobold.py
--rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-05-22 00:28:19.000000 agixt-1.1.63b0/agixt/provider/llamacpp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-05-22 00:28:19.000000 agixt-1.1.63b0/agixt/provider/oobabooga.py
--rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-05-22 00:28:19.000000 agixt-1.1.63b0/agixt/provider/openai.py
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-05-22 00:28:19.000000 agixt-1.1.63b0/agixt/provider/palm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2772 2023-05-22 00:28:19.000000 agixt-1.1.63b0/agixt/provider/transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)      881 2023-05-22 00:28:19.000000 agixt-1.1.63b0/agixt/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-22 00:28:19.000000 agixt-1.1.63b0/agixt/version
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 00:28:31.414599 agixt-1.1.63b0/agixt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13861 2023-05-22 00:28:31.000000 agixt-1.1.63b0/agixt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-05-22 00:28:31.000000 agixt-1.1.63b0/agixt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 00:28:31.000000 agixt-1.1.63b0/agixt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-05-22 00:28:31.000000 agixt-1.1.63b0/agixt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-22 00:28:31.000000 agixt-1.1.63b0/agixt.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 00:28:31.414599 agixt-1.1.63b0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)    13404 2023-05-22 00:28:19.000000 agixt-1.1.63b0/docs/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-22 00:28:19.000000 agixt-1.1.63b0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 00:28:31.418599 agixt-1.1.63b0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-05-22 00:28:19.000000 agixt-1.1.63b0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 00:58:50.185376 agixt-1.1.64b0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-05-22 00:58:37.000000 agixt-1.1.64b0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-22 00:58:37.000000 agixt-1.1.64b0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    13861 2023-05-22 00:58:50.185376 agixt-1.1.64b0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 00:58:50.181376 agixt-1.1.64b0/agixt/
+-rw-r--r--   0 runner    (1001) docker     (123)    15962 2023-05-22 00:58:37.000000 agixt-1.1.64b0/agixt/AGiXT.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12848 2023-05-22 00:58:37.000000 agixt-1.1.64b0/agixt/Agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6997 2023-05-22 00:58:37.000000 agixt-1.1.64b0/agixt/Chain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6153 2023-05-22 00:58:37.000000 agixt-1.1.64b0/agixt/Commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)      960 2023-05-22 00:58:37.000000 agixt-1.1.64b0/agixt/Config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-05-22 00:58:37.000000 agixt-1.1.64b0/agixt/CustomPrompt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6337 2023-05-22 00:58:37.000000 agixt-1.1.64b0/agixt/Embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-05-22 00:58:37.000000 agixt-1.1.64b0/agixt/Main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8367 2023-05-22 00:58:37.000000 agixt-1.1.64b0/agixt/Memories.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8476 2023-05-22 00:58:37.000000 agixt-1.1.64b0/agixt/Tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-05-22 00:58:37.000000 agixt-1.1.64b0/agixt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12961 2023-05-22 00:58:37.000000 agixt-1.1.64b0/agixt/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 00:58:50.185376 agixt-1.1.64b0/agixt/provider/
+-rw-r--r--   0 runner    (1001) docker     (123)     2157 2023-05-22 00:58:37.000000 agixt-1.1.64b0/agixt/provider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-05-22 00:58:37.000000 agixt-1.1.64b0/agixt/provider/azure.py
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-05-22 00:58:37.000000 agixt-1.1.64b0/agixt/provider/bard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-05-22 00:58:37.000000 agixt-1.1.64b0/agixt/provider/bing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-05-22 00:58:37.000000 agixt-1.1.64b0/agixt/provider/chatgpt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-05-22 00:58:37.000000 agixt-1.1.64b0/agixt/provider/claude.py
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-05-22 00:58:37.000000 agixt-1.1.64b0/agixt/provider/fastchat.py
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-05-22 00:58:37.000000 agixt-1.1.64b0/agixt/provider/gpt4all.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-05-22 00:58:37.000000 agixt-1.1.64b0/agixt/provider/gpt4free.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-22 00:58:37.000000 agixt-1.1.64b0/agixt/provider/gpugpt4all.py
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-05-22 00:58:37.000000 agixt-1.1.64b0/agixt/provider/huggingchat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-05-22 00:58:37.000000 agixt-1.1.64b0/agixt/provider/kobold.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-05-22 00:58:37.000000 agixt-1.1.64b0/agixt/provider/llamacpp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-05-22 00:58:37.000000 agixt-1.1.64b0/agixt/provider/oobabooga.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-05-22 00:58:37.000000 agixt-1.1.64b0/agixt/provider/openai.py
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-05-22 00:58:37.000000 agixt-1.1.64b0/agixt/provider/palm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2772 2023-05-22 00:58:37.000000 agixt-1.1.64b0/agixt/provider/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      881 2023-05-22 00:58:37.000000 agixt-1.1.64b0/agixt/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-22 00:58:37.000000 agixt-1.1.64b0/agixt/version
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 00:58:50.181376 agixt-1.1.64b0/agixt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13861 2023-05-22 00:58:50.000000 agixt-1.1.64b0/agixt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-05-22 00:58:50.000000 agixt-1.1.64b0/agixt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 00:58:50.000000 agixt-1.1.64b0/agixt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-05-22 00:58:50.000000 agixt-1.1.64b0/agixt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-22 00:58:50.000000 agixt-1.1.64b0/agixt.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 00:58:50.185376 agixt-1.1.64b0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)    13404 2023-05-22 00:58:37.000000 agixt-1.1.64b0/docs/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-22 00:58:37.000000 agixt-1.1.64b0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 00:58:50.185376 agixt-1.1.64b0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-05-22 00:58:37.000000 agixt-1.1.64b0/setup.py
```

### Comparing `agixt-1.1.63b0/LICENSE` & `agixt-1.1.64b0/LICENSE`

 * *Files identical despite different names*

### Comparing `agixt-1.1.63b0/PKG-INFO` & `agixt-1.1.64b0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agixt
-Version: 1.1.63b0
+Version: 1.1.64b0
 Summary: An Artificial Intelligence Automation Platform. AI Instruction management from various providers, has an adaptive memory, and a versatile plugin system with many commands including web browsing. Supports many AI providers and models and growing support every day.
 Author: Josh XT
 Author-email: josh@devxt.com
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `agixt-1.1.63b0/agixt/AGiXT.py` & `agixt-1.1.64b0/agixt/AGiXT.py`

 * *Files 1% similar despite different names*

```diff
@@ -95,29 +95,29 @@
                 loop = asyncio.new_event_loop()
                 asyncio.set_event_loop(loop)
                 loop.run_until_complete(
                     self.websearch_agent(task=task, depth=websearch_depth)
                 )
             else:
                 self.websearch_agent(task=task, depth=websearch_depth)
-        if int(tokens) > int(self.agent.MAX_TOKENS):
+        try:
+            self.response = self.agent.instruct(formatted_prompt, tokens=tokens)
+        except:
             if context_results > 0:
                 context_results = context_results - 1
             if context_results == 0:
                 print("Warning: No context injected due to max tokens.")
             return self.run(
                 task=task,
                 prompt=prompt,
                 context_results=context_results,
-                websearch=websearch,
-                websearch_depth=websearch_depth,
                 async_exec=async_exec,
                 **kwargs,
             )
-        self.response = self.agent.instruct(formatted_prompt, tokens=tokens)
+
         # Handle commands if the prompt contains the {COMMANDS} placeholder
         # We handle command injection that DOESN'T allow command execution by using {command_list} in the prompt
         if "{COMMANDS}" in unformatted_prompt:
             execution_response = self.execution_agent(
                 execution_response=self.response,
                 task=task,
                 context_results=context_results,
```

### Comparing `agixt-1.1.63b0/agixt/Agent.py` & `agixt-1.1.64b0/agixt/Agent.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.63b0/agixt/Commands.py` & `agixt-1.1.64b0/agixt/Commands.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.63b0/agixt/Config.py` & `agixt-1.1.64b0/agixt/Config.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.63b0/agixt/CustomPrompt.py` & `agixt-1.1.64b0/agixt/CustomPrompt.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.63b0/agixt/Embedding.py` & `agixt-1.1.64b0/agixt/Embedding.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.63b0/agixt/Main.py` & `agixt-1.1.64b0/agixt/Main.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.63b0/agixt/Memories.py` & `agixt-1.1.64b0/agixt/Memories.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.63b0/agixt/Tasks.py` & `agixt-1.1.64b0/agixt/Tasks.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.63b0/agixt/app.py` & `agixt-1.1.64b0/agixt/app.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.63b0/agixt/provider/__init__.py` & `agixt-1.1.64b0/agixt/provider/__init__.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.63b0/agixt/provider/azure.py` & `agixt-1.1.64b0/agixt/provider/azure.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.63b0/agixt/provider/bing.py` & `agixt-1.1.64b0/agixt/provider/bing.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.63b0/agixt/provider/chatgpt.py` & `agixt-1.1.64b0/agixt/provider/chatgpt.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.63b0/agixt/provider/claude.py` & `agixt-1.1.64b0/agixt/provider/claude.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.63b0/agixt/provider/fastchat.py` & `agixt-1.1.64b0/agixt/provider/fastchat.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.63b0/agixt/provider/gpt4all.py` & `agixt-1.1.64b0/agixt/provider/gpt4all.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.63b0/agixt/provider/gpt4free.py` & `agixt-1.1.64b0/agixt/provider/gpt4free.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.63b0/agixt/provider/gpugpt4all.py` & `agixt-1.1.64b0/agixt/provider/gpugpt4all.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.63b0/agixt/provider/huggingchat.py` & `agixt-1.1.64b0/agixt/provider/huggingchat.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.63b0/agixt/provider/kobold.py` & `agixt-1.1.64b0/agixt/provider/kobold.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.63b0/agixt/provider/llamacpp.py` & `agixt-1.1.64b0/agixt/provider/llamacpp.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.63b0/agixt/provider/oobabooga.py` & `agixt-1.1.64b0/agixt/provider/oobabooga.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.63b0/agixt/provider/openai.py` & `agixt-1.1.64b0/agixt/provider/openai.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.63b0/agixt/provider/palm.py` & `agixt-1.1.64b0/agixt/provider/palm.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.63b0/agixt/provider/transformer.py` & `agixt-1.1.64b0/agixt/provider/transformer.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.63b0/agixt/requirements.txt` & `agixt-1.1.64b0/agixt/requirements.txt`

 * *Files identical despite different names*

### Comparing `agixt-1.1.63b0/agixt.egg-info/PKG-INFO` & `agixt-1.1.64b0/agixt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agixt
-Version: 1.1.63b0
+Version: 1.1.64b0
 Summary: An Artificial Intelligence Automation Platform. AI Instruction management from various providers, has an adaptive memory, and a versatile plugin system with many commands including web browsing. Supports many AI providers and models and growing support every day.
 Author: Josh XT
 Author-email: josh@devxt.com
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `agixt-1.1.63b0/agixt.egg-info/SOURCES.txt` & `agixt-1.1.64b0/agixt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `agixt-1.1.63b0/agixt.egg-info/requires.txt` & `agixt-1.1.64b0/agixt.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `agixt-1.1.63b0/docs/README.md` & `agixt-1.1.64b0/docs/README.md`

 * *Files identical despite different names*

### Comparing `agixt-1.1.63b0/setup.py` & `agixt-1.1.64b0/setup.py`

 * *Files identical despite different names*

