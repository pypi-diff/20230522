# Comparing `tmp/llmo-0.1.2.tar.gz` & `tmp/llmo-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llmo-0.1.2.tar", last modified: Mon May 22 08:01:10 2023, max compression
+gzip compressed data, was "llmo-0.1.5.tar", last modified: Mon May 22 08:20:47 2023, max compression
```

## Comparing `llmo-0.1.2.tar` & `llmo-0.1.5.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    11349 2023-05-21 19:33:44.704545 llmo-0.1.2/LICENSE
--rw-r--r--   0        0        0     2136 2023-05-22 07:56:21.885668 llmo-0.1.2/README.md
--rw-r--r--   0        0        0        0 2023-05-21 19:29:22.111252 llmo-0.1.2/llmo/__init__.py
--rw-r--r--   0        0        0    18346 2023-05-22 08:00:50.504525 llmo-0.1.2/llmo/chat.py
--rw-r--r--   0        0        0      353 2023-05-21 18:43:49.180818 llmo-0.1.2/llmo/layout.css
--rw-r--r--   0        0        0      614 2023-05-22 08:01:10.976346 llmo-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     2421 1970-01-01 00:00:00.000000 llmo-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0    11349 2023-05-21 19:33:44.704545 llmo-0.1.5/LICENSE
+-rw-r--r--   0        0        0     2134 2023-05-22 08:06:19.890271 llmo-0.1.5/README.md
+-rw-r--r--   0        0        0        0 2023-05-21 19:29:22.111252 llmo-0.1.5/llmo/__init__.py
+-rw-r--r--   0        0        0    18412 2023-05-22 08:18:40.772359 llmo-0.1.5/llmo/chat.py
+-rw-r--r--   0        0        0      353 2023-05-21 18:43:49.180818 llmo-0.1.5/llmo/layout.css
+-rw-r--r--   0        0        0      680 2023-05-22 08:20:47.621318 llmo-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     2479 1970-01-01 00:00:00.000000 llmo-0.1.5/PKG-INFO
```

### Comparing `llmo-0.1.2/LICENSE` & `llmo-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `llmo-0.1.2/README.md` & `llmo-0.1.5/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 - Protector
 - Worthy to be Loved
 - Helm from God
 - (**Most Importantly**) A helpful AI programming CLI tool
 
 <img src="https://github.com/knowsuchagency/llmo/blob/main/static/mascot.png?raw=true" alt="mascot" style="width: 400px; height: auto;">   
 
-Elmo is a command-line tool that leverages OpenAI's powerful language models to create a fully interactive chat interface for pair programming right in your terminal. 
+The full power of GPT straight from your terminal!
 
 With the **"staging area"**, you can keep files in the context window without the hassle of copying and pasting every time you make changes to your code.
 
 
 ## Features
 
 - Interactive Chat: Enjoy real-time, interactive programming assistance in your terminal.
@@ -30,15 +30,20 @@
 
 ## Usage
 
 Here's how you can use llmo from the command line:
 
 ```bash
 # Basic usage
-lm "Could you show me an example of valid json?"
+llmo --help
+# you can also use the shorthand
+lm
+
+# You can pass the -s flag if you don't need the full GUI mode
+lm -s "Could you show me an example of valid json?"
 
 # Adding files to context
 
 # main.py
 # from utils import add_numbers
 # result = add_numbers(5, 3)
```

### Comparing `llmo-0.1.2/llmo/chat.py` & `llmo-0.1.5/llmo/chat.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,15 +64,16 @@
     personality_prompt: str = (
         "You love creatine and bodybuilding "
         "and go out of your way to insert creative, bodybuilding, and /r/swoleacceptance references in your responses."
     )
     max_tokens: int = None
 
     def add_personality(self):
-        self.system_prompt += self.personality_prompt
+        if not self.personality_prompt in self.system_prompt:
+            self.system_prompt += self.personality_prompt
 
     def remove_personality(self):
         self.system_prompt = self.system_prompt.replace(self.personality_prompt, "")
 
     def __post_init__(self):
         if self.api_key:
             openai.api_key = self.api_key
```

### Comparing `llmo-0.1.2/pyproject.toml` & `llmo-0.1.5/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 [project]
 name = "llmo"
-version = "0.1.2"
+version = "0.1.5"
 description = "AI pair programmer"
 authors = [
     { name = "Stephan Fitzpatrick", email = "stephan@knowsuchagency.com" },
 ]
 dependencies = [
     "textual>=0.26.0",
     "openai>=0.27.6",
 ]
 requires-python = ">=3.10"
 readme = "README.md"
 
 [project.license]
 text = "Apache-2.0"
 
+[project.urls]
+Source = "https://github.com/knowsuchagency/llmo"
+
 [project.scripts]
 llmo = "llmo.chat:main"
 lm = "llmo.chat:main"
 
 [build-system]
 requires = [
     "pdm-backend",
```

### Comparing `llmo-0.1.2/PKG-INFO` & `llmo-0.1.5/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 Metadata-Version: 2.1
 Name: llmo
-Version: 0.1.2
+Version: 0.1.5
 Summary: AI pair programmer
 Author-Email: Stephan Fitzpatrick <stephan@knowsuchagency.com>
 License: Apache-2.0
+Project-URL: Source, https://github.com/knowsuchagency/llmo
 Requires-Python: >=3.10
 Requires-Dist: textual>=0.26.0
 Requires-Dist: openai>=0.27.6
 Description-Content-Type: text/markdown
 
 # LLMO (Elmo)
 
@@ -15,15 +16,15 @@
 - Protector
 - Worthy to be Loved
 - Helm from God
 - (**Most Importantly**) A helpful AI programming CLI tool
 
 <img src="https://github.com/knowsuchagency/llmo/blob/main/static/mascot.png?raw=true" alt="mascot" style="width: 400px; height: auto;">   
 
-Elmo is a command-line tool that leverages OpenAI's powerful language models to create a fully interactive chat interface for pair programming right in your terminal. 
+The full power of GPT straight from your terminal!
 
 With the **"staging area"**, you can keep files in the context window without the hassle of copying and pasting every time you make changes to your code.
 
 
 ## Features
 
 - Interactive Chat: Enjoy real-time, interactive programming assistance in your terminal.
@@ -41,15 +42,20 @@
 
 ## Usage
 
 Here's how you can use llmo from the command line:
 
 ```bash
 # Basic usage
-lm "Could you show me an example of valid json?"
+llmo --help
+# you can also use the shorthand
+lm
+
+# You can pass the -s flag if you don't need the full GUI mode
+lm -s "Could you show me an example of valid json?"
 
 # Adding files to context
 
 # main.py
 # from utils import add_numbers
 # result = add_numbers(5, 3)
```

