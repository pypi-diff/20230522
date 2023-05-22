# Comparing `tmp/gptw-0.4.0.tar.gz` & `tmp/gptw-0.4.1.tar.gz`

## Comparing `gptw-0.4.0.tar` & `gptw-0.4.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 gptw-0.4.0/gptw/__init__.py
--rw-r--r--   0        0        0     6202 2020-02-02 00:00:00.000000 gptw-0.4.0/gptw/gptw.py
--rw-r--r--   0        0        0     2720 2020-02-02 00:00:00.000000 gptw-0.4.0/gptw/prompts.json
--rw-r--r--   0        0        0     1822 2020-02-02 00:00:00.000000 gptw-0.4.0/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 gptw-0.4.0/LICENSE
--rw-r--r--   0        0        0     3536 2020-02-02 00:00:00.000000 gptw-0.4.0/README.md
--rw-r--r--   0        0        0     1355 2020-02-02 00:00:00.000000 gptw-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     4608 2020-02-02 00:00:00.000000 gptw-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 gptw-0.4.1/gptw/__init__.py
+-rw-r--r--   0        0        0     6305 2020-02-02 00:00:00.000000 gptw-0.4.1/gptw/gptw.py
+-rw-r--r--   0        0        0     2720 2020-02-02 00:00:00.000000 gptw-0.4.1/gptw/prompts.json
+-rw-r--r--   0        0        0     1822 2020-02-02 00:00:00.000000 gptw-0.4.1/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 gptw-0.4.1/LICENSE
+-rw-r--r--   0        0        0     3536 2020-02-02 00:00:00.000000 gptw-0.4.1/README.md
+-rw-r--r--   0        0        0     1355 2020-02-02 00:00:00.000000 gptw-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0     4608 2020-02-02 00:00:00.000000 gptw-0.4.1/PKG-INFO
```

### Comparing `gptw-0.4.0/gptw/gptw.py` & `gptw-0.4.1/gptw/gptw.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,14 @@
 import argparse
 import json
 import logging
 import os
 import sys
 from os.path import expanduser
 
-import openai
-import poe
-
 import gptw
 
 
 def args_init():
     parser = argparse.ArgumentParser(
         description="\n".join(
             [
@@ -97,40 +94,49 @@
 
     cfg[key] = value
 
     with open(config_file, "w") as f:
         json.dump(cfg, f)
 
 
+CONFIG = None
+
+
 def get_config(key):
-    try:
+    if not CONFIG:
         with open(config_file) as f:
-            return json.load(f)[key]
+            CFG = json.load(f)
+    try:
+        return CFG[key]
     except Exception:
         print("config not found, run `ww --config` to set it")
         sys.exit(1)
 
 
 def get_prompts():
     with open(prompts_file) as f:
         return json.load(f)["cmds"]
 
 
 def ask_gpt(token, model, text):
+    import openai
+
     logging.debug(f"!!!ask:{text}")
     openai.api_key = token
     completion = openai.ChatCompletion.create(
         model=model,
         messages=[{"role": "user", "content": text}],
-        temperature=0.2,
+        temperature=0.5,
     )
     return str(completion.choices[0].message.content).strip()
 
 
 def ask_poe(token, bot_name, text):
+    import poe
+
     poe.logger.setLevel(logging.WARNING)
     client = poe.Client(token)
 
     for chunk in client.send_message(bot_name, text, with_chat_break=True):
         pass
     # delete the 3 latest messages, including the chat break
     client.purge_conversation(bot_name, count=3)
@@ -154,23 +160,25 @@
     response = ""
     for data in chatbot.ask(text):
         response = data["message"]
     return response
 
 
 def ask_azure(token, endpoint, depname, text):
+    import openai
+
     logging.debug(f"!!!ask:{text}")
     openai.api_key = token
     openai.api_base = endpoint
     openai.api_type = "azure"
     openai.api_version = "2023-05-15"
     completion = openai.ChatCompletion.create(
         engine=depname,
         messages=[{"role": "user", "content": text}],
-        temperature=0.2,
+        temperature=0.5,
     )
     return str(completion.choices[0].message.content).strip()
 
 
 def list_commands(prompts):
     print(f'{"cmd":<{3}} | {"meaning":<{30}} | {"example"}')
     for pmt in prompts:
@@ -207,15 +215,15 @@
 
     if not args.cmd or args.cmd not in prompts:
         print("need a command")
         exit(0)
 
     logging.debug(f"cmd:{args.cmd},text:{text}")
 
-    msg = f'{prompts[args.cmd]["prompt"]}\n\n{text}'
+    msg = f'{prompts[args.cmd]["prompt"]}\n```{text.replace("```","")}```'
 
     if get_config("provider") == "openai":
         logging.debug("use openai")
         model = get_config("openai-model")
         token = get_config("openai-token")
         print(ask_gpt(token, model, msg))
     if get_config("provider") == "poe":
```

### Comparing `gptw-0.4.0/gptw/prompts.json` & `gptw-0.4.1/gptw/prompts.json`

 * *Files identical despite different names*

### Comparing `gptw-0.4.0/.gitignore` & `gptw-0.4.1/.gitignore`

 * *Files identical despite different names*

### Comparing `gptw-0.4.0/LICENSE` & `gptw-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gptw-0.4.0/README.md` & `gptw-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `gptw-0.4.0/pyproject.toml` & `gptw-0.4.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `gptw-0.4.0/PKG-INFO` & `gptw-0.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gptw
-Version: 0.4.0
+Version: 0.4.1
 Summary: The ChatGPT command-line wrapper simplifies the execution of predetermined tasks through ChatGPT.
 Author: Xin Yang
 Author-email: xinydev@gmail.com
 License-Expression: Apache-2.0
 License-File: LICENSE
 Keywords: ChatGPT,Command Line,English Polishing,English Translation
 Classifier: Development Status :: 3 - Alpha
```

