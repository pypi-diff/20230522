# Comparing `tmp/devchat-0.1.7.tar.gz` & `tmp/devchat-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "devchat-0.1.7.tar", last modified: Sun May 21 11:37:41 2023, max compression
+gzip compressed data, was "devchat-0.1.8.tar", last modified: Mon May 22 14:40:52 2023, max compression
```

## Comparing `devchat-0.1.7.tar` & `devchat-0.1.8.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 basicthinker   (501) staff       (20)        0 2023-05-21 11:37:41.706506 devchat-0.1.7/
--rw-r--r--   0 basicthinker   (501) staff       (20)    11357 2023-05-05 13:17:54.000000 devchat-0.1.7/LICENSE
--rw-r--r--   0 basicthinker   (501) staff       (20)     5174 2023-05-21 11:37:41.706358 devchat-0.1.7/PKG-INFO
--rw-r--r--   0 basicthinker   (501) staff       (20)     4718 2023-05-21 11:37:13.000000 devchat-0.1.7/README.md
-drwxr-xr-x   0 basicthinker   (501) staff       (20)        0 2023-05-21 11:37:41.702882 devchat-0.1.7/devchat/
--rw-r--r--   0 basicthinker   (501) staff       (20)        0 2023-05-05 13:17:54.000000 devchat-0.1.7/devchat/__init__.py
--rw-r--r--   0 basicthinker   (501) staff       (20)     5660 2023-05-18 09:46:55.000000 devchat-0.1.7/devchat/_cli.py
--rw-r--r--   0 basicthinker   (501) staff       (20)     4552 2023-05-12 00:41:47.000000 devchat-0.1.7/devchat/assistant.py
--rw-r--r--   0 basicthinker   (501) staff       (20)     1464 2023-05-05 13:17:54.000000 devchat-0.1.7/devchat/chat.py
--rw-r--r--   0 basicthinker   (501) staff       (20)      614 2023-05-07 23:44:52.000000 devchat-0.1.7/devchat/message.py
-drwxr-xr-x   0 basicthinker   (501) staff       (20)        0 2023-05-21 11:37:41.704681 devchat-0.1.7/devchat/openai/
--rw-r--r--   0 basicthinker   (501) staff       (20)      248 2023-05-05 13:17:54.000000 devchat-0.1.7/devchat/openai/__init__.py
--rw-r--r--   0 basicthinker   (501) staff       (20)     3399 2023-05-18 09:47:11.000000 devchat-0.1.7/devchat/openai/openai_chat.py
--rw-r--r--   0 basicthinker   (501) staff       (20)     1561 2023-05-07 23:44:52.000000 devchat-0.1.7/devchat/openai/openai_message.py
--rw-r--r--   0 basicthinker   (501) staff       (20)     6017 2023-05-18 05:09:41.000000 devchat-0.1.7/devchat/openai/openai_prompt.py
--rw-r--r--   0 basicthinker   (501) staff       (20)     6447 2023-05-12 00:56:54.000000 devchat-0.1.7/devchat/prompt.py
--rw-r--r--   0 basicthinker   (501) staff       (20)     3704 2023-05-19 17:29:57.000000 devchat-0.1.7/devchat/store.py
--rw-r--r--   0 basicthinker   (501) staff       (20)     4981 2023-05-12 00:21:13.000000 devchat-0.1.7/devchat/utils.py
-drwxr-xr-x   0 basicthinker   (501) staff       (20)        0 2023-05-21 11:37:41.703837 devchat-0.1.7/devchat.egg-info/
--rw-r--r--   0 basicthinker   (501) staff       (20)     5174 2023-05-21 11:37:41.000000 devchat-0.1.7/devchat.egg-info/PKG-INFO
--rw-r--r--   0 basicthinker   (501) staff       (20)      628 2023-05-21 11:37:41.000000 devchat-0.1.7/devchat.egg-info/SOURCES.txt
--rw-r--r--   0 basicthinker   (501) staff       (20)        1 2023-05-21 11:37:41.000000 devchat-0.1.7/devchat.egg-info/dependency_links.txt
--rw-r--r--   0 basicthinker   (501) staff       (20)       46 2023-05-21 11:37:41.000000 devchat-0.1.7/devchat.egg-info/entry_points.txt
--rw-r--r--   0 basicthinker   (501) staff       (20)      116 2023-05-21 11:37:41.000000 devchat-0.1.7/devchat.egg-info/requires.txt
--rw-r--r--   0 basicthinker   (501) staff       (20)       14 2023-05-21 11:37:41.000000 devchat-0.1.7/devchat.egg-info/top_level.txt
--rw-r--r--   0 basicthinker   (501) staff       (20)      102 2023-05-05 13:17:54.000000 devchat-0.1.7/pyproject.toml
--rw-r--r--   0 basicthinker   (501) staff       (20)       38 2023-05-21 11:37:41.706543 devchat-0.1.7/setup.cfg
--rw-r--r--   0 basicthinker   (501) staff       (20)     1112 2023-05-21 11:37:27.000000 devchat-0.1.7/setup.py
-drwxr-xr-x   0 basicthinker   (501) staff       (20)        0 2023-05-21 11:37:41.706060 devchat-0.1.7/tests/
--rw-r--r--   0 basicthinker   (501) staff       (20)        0 2023-05-05 13:17:54.000000 devchat-0.1.7/tests/__init__.py
--rw-r--r--   0 basicthinker   (501) staff       (20)     5996 2023-05-12 00:42:14.000000 devchat-0.1.7/tests/test_cli.py
--rw-r--r--   0 basicthinker   (501) staff       (20)     1809 2023-05-07 23:44:52.000000 devchat-0.1.7/tests/test_openai_message.py
--rw-r--r--   0 basicthinker   (501) staff       (20)     5908 2023-05-12 00:53:18.000000 devchat-0.1.7/tests/test_openai_prompt.py
--rw-r--r--   0 basicthinker   (501) staff       (20)     2303 2023-05-05 15:34:17.000000 devchat-0.1.7/tests/test_store.py
--rw-r--r--   0 basicthinker   (501) staff       (20)     1225 2023-05-07 23:44:52.000000 devchat-0.1.7/tests/test_utils.py
+drwxr-xr-x   0 basicthinker   (501) staff       (20)        0 2023-05-22 14:40:52.733330 devchat-0.1.8/
+-rw-r--r--   0 basicthinker   (501) staff       (20)    11357 2023-05-05 13:17:54.000000 devchat-0.1.8/LICENSE
+-rw-r--r--   0 basicthinker   (501) staff       (20)     5174 2023-05-22 14:40:52.733133 devchat-0.1.8/PKG-INFO
+-rw-r--r--   0 basicthinker   (501) staff       (20)     4718 2023-05-21 11:37:13.000000 devchat-0.1.8/README.md
+drwxr-xr-x   0 basicthinker   (501) staff       (20)        0 2023-05-22 14:40:52.729619 devchat-0.1.8/devchat/
+-rw-r--r--   0 basicthinker   (501) staff       (20)        0 2023-05-05 13:17:54.000000 devchat-0.1.8/devchat/__init__.py
+-rw-r--r--   0 basicthinker   (501) staff       (20)     6136 2023-05-22 13:34:59.000000 devchat-0.1.8/devchat/_cli.py
+-rw-r--r--   0 basicthinker   (501) staff       (20)     4794 2023-05-22 13:47:32.000000 devchat-0.1.8/devchat/assistant.py
+-rw-r--r--   0 basicthinker   (501) staff       (20)     1682 2023-05-21 14:33:17.000000 devchat-0.1.8/devchat/chat.py
+-rw-r--r--   0 basicthinker   (501) staff       (20)      566 2023-05-22 04:56:01.000000 devchat-0.1.8/devchat/message.py
+drwxr-xr-x   0 basicthinker   (501) staff       (20)        0 2023-05-22 14:40:52.731572 devchat-0.1.8/devchat/openai/
+-rw-r--r--   0 basicthinker   (501) staff       (20)      248 2023-05-05 13:17:54.000000 devchat-0.1.8/devchat/openai/__init__.py
+-rw-r--r--   0 basicthinker   (501) staff       (20)     3030 2023-05-22 14:29:50.000000 devchat-0.1.8/devchat/openai/openai_chat.py
+-rw-r--r--   0 basicthinker   (501) staff       (20)     1561 2023-05-07 23:44:52.000000 devchat-0.1.8/devchat/openai/openai_message.py
+-rw-r--r--   0 basicthinker   (501) staff       (20)     6031 2023-05-22 11:27:42.000000 devchat-0.1.8/devchat/openai/openai_prompt.py
+-rw-r--r--   0 basicthinker   (501) staff       (20)     6604 2023-05-22 13:52:58.000000 devchat-0.1.8/devchat/prompt.py
+-rw-r--r--   0 basicthinker   (501) staff       (20)     4299 2023-05-22 12:34:46.000000 devchat-0.1.8/devchat/store.py
+-rw-r--r--   0 basicthinker   (501) staff       (20)     5306 2023-05-22 09:23:48.000000 devchat-0.1.8/devchat/utils.py
+drwxr-xr-x   0 basicthinker   (501) staff       (20)        0 2023-05-22 14:40:52.730661 devchat-0.1.8/devchat.egg-info/
+-rw-r--r--   0 basicthinker   (501) staff       (20)     5174 2023-05-22 14:40:52.000000 devchat-0.1.8/devchat.egg-info/PKG-INFO
+-rw-r--r--   0 basicthinker   (501) staff       (20)      628 2023-05-22 14:40:52.000000 devchat-0.1.8/devchat.egg-info/SOURCES.txt
+-rw-r--r--   0 basicthinker   (501) staff       (20)        1 2023-05-22 14:40:52.000000 devchat-0.1.8/devchat.egg-info/dependency_links.txt
+-rw-r--r--   0 basicthinker   (501) staff       (20)       46 2023-05-22 14:40:52.000000 devchat-0.1.8/devchat.egg-info/entry_points.txt
+-rw-r--r--   0 basicthinker   (501) staff       (20)      130 2023-05-22 14:40:52.000000 devchat-0.1.8/devchat.egg-info/requires.txt
+-rw-r--r--   0 basicthinker   (501) staff       (20)       14 2023-05-22 14:40:52.000000 devchat-0.1.8/devchat.egg-info/top_level.txt
+-rw-r--r--   0 basicthinker   (501) staff       (20)      102 2023-05-05 13:17:54.000000 devchat-0.1.8/pyproject.toml
+-rw-r--r--   0 basicthinker   (501) staff       (20)       38 2023-05-22 14:40:52.733371 devchat-0.1.8/setup.cfg
+-rw-r--r--   0 basicthinker   (501) staff       (20)     1112 2023-05-22 06:04:12.000000 devchat-0.1.8/setup.py
+drwxr-xr-x   0 basicthinker   (501) staff       (20)        0 2023-05-22 14:40:52.732741 devchat-0.1.8/tests/
+-rw-r--r--   0 basicthinker   (501) staff       (20)        0 2023-05-05 13:17:54.000000 devchat-0.1.8/tests/__init__.py
+-rw-r--r--   0 basicthinker   (501) staff       (20)     5996 2023-05-22 06:00:29.000000 devchat-0.1.8/tests/test_cli.py
+-rw-r--r--   0 basicthinker   (501) staff       (20)     1809 2023-05-07 23:44:52.000000 devchat-0.1.8/tests/test_openai_message.py
+-rw-r--r--   0 basicthinker   (501) staff       (20)     5887 2023-05-22 11:37:12.000000 devchat-0.1.8/tests/test_openai_prompt.py
+-rw-r--r--   0 basicthinker   (501) staff       (20)     2221 2023-05-21 23:12:05.000000 devchat-0.1.8/tests/test_store.py
+-rw-r--r--   0 basicthinker   (501) staff       (20)     1225 2023-05-07 23:44:52.000000 devchat-0.1.8/tests/test_utils.py
```

### Comparing `devchat-0.1.7/LICENSE` & `devchat-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `devchat-0.1.7/PKG-INFO` & `devchat-0.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: devchat
-Version: 0.1.7
+Version: 0.1.8
 Summary: DevChat is an open-source tool that helps developers write prompts to generate code and documentation.
 Home-page: https://github.com/covespace/devchat
 License: Apache License 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
```

### Comparing `devchat-0.1.7/README.md` & `devchat-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `devchat-0.1.7/devchat/_cli.py` & `devchat-0.1.8/devchat/_cli.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,58 +6,61 @@
 import os
 import sys
 from typing import List, Optional, Tuple
 import rich_click as click
 from devchat.store import Store
 from devchat.openai import OpenAIChatConfig, OpenAIChat
 from devchat.assistant import Assistant
-from devchat.utils import find_git_root, git_ignore, parse_files
+from devchat.utils import find_git_root, git_ignore, parse_files, setup_logger
 
 
 click.rich_click.USE_MARKDOWN = True
 
+logger = setup_logger(__name__)
+
 
 @click.group()
 def main():
     """DevChat CLI: A command-line interface for the DevChat chatbot."""
 
 
 @contextmanager
 def handle_errors():
     """Handle errors in the CLI."""
     try:
         yield
     except Exception as error:
-        click.echo(f"Error: {error}", err=True)
+        logger.exception(error)
+        click.echo(f"Error: {error}")
         sys.exit(os.EX_SOFTWARE)
 
 
-def init_dir() -> Tuple[dict, Store]:
+def init_dir() -> Tuple[dict, str]:
     git_root = find_git_root()
     chat_dir = os.path.join(git_root, ".chat")
     if not os.path.exists(chat_dir):
         os.makedirs(chat_dir)
 
     default_config_data = {
-        'model': 'gpt-3.5-turbo',
+        'model': 'gpt-4',
         'provider': 'OpenAI',
         'OpenAI': {
-            'temperature': 0
+            'temperature': 0,
+            'stream': True
         }
     }
 
     try:
         with open(os.path.join(chat_dir, 'config.json'), 'r', encoding='utf-8') as file:
             config_data = json.load(file)
     except FileNotFoundError:
         config_data = default_config_data
 
-    store = Store(chat_dir)
     git_ignore(git_root, chat_dir)
-    return config_data, store
+    return config_data, chat_dir
 
 
 @main.command()
 @click.argument('content', required=False)
 @click.option('-p', '--parent', help='Input the parent prompt hash to continue the conversation.')
 @click.option('-r', '--reference', multiple=True,
               help='Input one or more specific previous prompts to include in the current prompt.')
@@ -129,15 +132,15 @@
     Run the following command line with your API key:
 
     ```bash
     export OPENAI_API_KEY="sk-..."
     ```
 
     """
-    config, store = init_dir()
+    config, chat_dir = init_dir()
 
     with handle_errors():
         if content is None:
             content = click.get_text_stream('stdin').read()
 
         if content == '':
             return
@@ -148,39 +151,48 @@
         provider = config.get('provider')
         if provider == 'OpenAI':
             if model is None:
                 model = config['model']
             openai_config = OpenAIChatConfig(model=model, **config['OpenAI'])
 
             chat = OpenAIChat(openai_config)
+            store = Store(chat_dir, chat)
 
             assistant = Assistant(chat, store)
             if 'tokens-per-prompt' in config:
                 assistant.token_limit = config['tokens-per-prompt']
 
             assistant.make_prompt(content, instruct_contents, context_contents,
                                   parent, reference)
 
             for response in assistant.iterate_response():
                 click.echo(response, nl=False)
         else:
-            click.echo(f"Error: Invalid LLM in configuration '{provider}'", err=True)
+            click.echo(f"Error: Invalid LLM in configuration '{provider}'")
             sys.exit(os.EX_DATAERR)
 
 
 @main.command()
 @click.option('--skip', default=0, help='Skip number prompts before showing the prompt history.')
 @click.option('--max-count', default=100, help='Limit the number of commits to output.')
 def log(skip, max_count):
     """
     Show the prompt history.
     """
-    _, store = init_dir()
-
-    recent_prompts = store.select_recent(skip, skip + max_count)
+    config, chat_dir = init_dir()
+    provider = config.get('provider')
+    recent_prompts = []
+    if provider == 'OpenAI':
+        openai_config = OpenAIChatConfig(model=config['model'], **config['OpenAI'])
+        chat = OpenAIChat(openai_config)
+        store = Store(chat_dir, chat)
+        recent_prompts = store.select_recent(skip, skip + max_count)
+    else:
+        click.echo(f"Error: Invalid LLM in configuration '{provider}'")
+        sys.exit(os.EX_DATAERR)
 
     logs = []
     for record in recent_prompts:
         try:
             logs.append(record.shortlog())
         except Exception:
             continue
```

### Comparing `devchat-0.1.7/devchat/assistant.py` & `devchat-0.1.8/devchat/assistant.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 from typing import Optional, List, Iterator
-from devchat.utils import validate_hashes
-from devchat.message import MessageType
+from devchat.utils import setup_logger
+from devchat.message import Message
 from devchat.chat import Chat
 from devchat.prompt import Prompt
 from devchat.store import Store
 
 
+logger = setup_logger(__name__)
+
+
 class Assistant:
     def __init__(self, chat: Chat, store: Store):
         """
         Initializes an Assistant object.
 
         Args:
             chat (Chat): A Chat object used to communicate with chat APIs.
@@ -42,34 +45,40 @@
             references (Optional[List[str]]): The reference prompt hashes.
         """
         self._prompt = self._chat.init_prompt(request)
         self._check_limit()
         # Add instructions to the prompt
         if instruct_contents:
             combined_instruct = ''.join(instruct_contents)
-            self._prompt.append_new(MessageType.INSTRUCT, combined_instruct)
+            self._prompt.append_new(Message.INSTRUCT, combined_instruct)
             self._check_limit()
         # Add context to the prompt
         if context_contents:
             for context_content in context_contents:
-                self._prompt.append_new(MessageType.CONTEXT, context_content)
+                self._prompt.append_new(Message.CONTEXT, context_content)
                 self._check_limit()
 
         # Add history to the prompt
-        self._prompt.references = validate_hashes(references)
-        for reference_hash in self._prompt.references:
-            if not self._append_prompt(self._store.get_prompt(reference_hash)):
-                return
+        for reference_hash in references:
+            prompt = self._store.get_prompt(reference_hash)
+            if not prompt:
+                logger.error("Reference prompt not found: %s", reference_hash)
+                continue
+            self._prompt.references.append(reference_hash)
+            self._append_prompt(prompt)
         if parent:
-            self._prompt.parent = validate_hashes([parent])[0]
+            self._prompt.parent = parent
             parent_hash = parent
             while parent_hash:
                 parent_prompt = self._store.get_prompt(parent_hash)
+                if not parent_prompt:
+                    logger.error("Parent prompt not found: %s", parent_hash)
+                    break
                 if not self._append_prompt(parent_prompt):
-                    return
+                    break
                 parent_hash = parent_prompt.parent
 
     def iterate_response(self) -> Iterator[str]:
         """Get an iterator of response strings from the chat API.
 
         Returns:
             Iterator[str]: An iterator over response strings from the chat API.
@@ -82,25 +91,25 @@
             yield f'\n\nprompt {self._prompt.hash}\n'
             for index in range(1, len(self._prompt.response)):
                 yield self._prompt.formatted_response(index) + '\n'
         else:
             response_str = str(self._chat.complete_response(self._prompt))
             self._prompt.set_response(response_str)
             self._store.store_prompt(self._prompt)
-            for index in self._prompt.response.keys():
+            for index in range(len(self._prompt.response)):
                 yield self._prompt.formatted_response(index) + '\n'
 
     def _append_prompt(self, prompt: Prompt) -> bool:
         # Append the first response and the request of the appended prompt
-        if not self._prompt.append_history(MessageType.CHAT, prompt.response[0],
+        if not self._prompt.append_history(Message.CHAT, prompt.response[0],
                                            self.available_tokens):
             return False
-        if not self._prompt.append_history(MessageType.CHAT, prompt.request,
+        if not self._prompt.append_history(Message.CHAT, prompt.request,
                                            self.available_tokens):
             return False
 
         # Append the context messages of the appended prompt
         for context_message in prompt.new_context:
-            if not self._prompt.append_history(MessageType.CONTEXT, context_message,
+            if not self._prompt.append_history(Message.CONTEXT, context_message,
                                                self.available_tokens):
                 return False
         return True
```

### Comparing `devchat-0.1.7/devchat/chat.py` & `devchat-0.1.8/devchat/chat.py`

 * *Files 18% similar despite different names*

```diff
@@ -19,14 +19,23 @@
 
         Args:
             request (str): The basic request of the prompt.
                            The returned prompt can be combined with more instructions and context.
         """
 
     @abstractmethod
+    def load_prompt(self, data: dict) -> Prompt:
+        """
+        Load a prompt from a dictionary.
+
+        Args:
+            data (dict): The dictionary containing the prompt data.
+        """
+
+    @abstractmethod
     def complete_response(self, prompt: Prompt) -> str:
         """
         Retrieve a complete response JSON string from the chat system.
 
         Args:
             prompt (Prompt): A prompt of messages representing the conversation.
         Returns:
```

### Comparing `devchat-0.1.7/devchat/message.py` & `devchat-0.1.8/devchat/message.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,25 +1,22 @@
 from abc import ABC, abstractmethod
-from enum import Enum
 from dataclasses import dataclass
 
 
-class MessageType(Enum):
-    INSTRUCT = "instruct"
-    CONTEXT = "context"
-    CHAT = "chat"
-
-
 @dataclass
 class Message(ABC):
     """
     The basic unit of information in a prompt.
     """
     content: str = ""
 
+    INSTRUCT = "instruct"
+    CONTEXT = "context"
+    CHAT = "chat"
+
     @abstractmethod
     def to_dict(self) -> dict:
         """
         Convert the message to a dictionary.
         """
 
     @abstractmethod
```

### Comparing `devchat-0.1.7/devchat/openai/openai_chat.py` & `devchat-0.1.8/devchat/openai/openai_chat.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from typing import Optional, Union, List, Dict, Iterator
 from pydantic import BaseModel, Field, Extra
 import openai
 from devchat.chat import Chat
 from devchat.utils import get_git_user_info
+from .openai_message import OpenAIMessage
 from .openai_prompt import OpenAIPrompt
 
 
 class OpenAIChatConfig(BaseModel):
     """
     Configuration object for the OpenAIChat class.
     """
@@ -39,57 +40,43 @@
 
         Args:
             config (OpenAIChatConfig): Configuration object with parameters for the OpenAI Chat API.
         """
         self.config = config
 
     def init_prompt(self, request: str) -> OpenAIPrompt:
-        """
-        Initialize a prompt for the chat system.
-
-        Args:
-            request (str): The basic request of the prompt.
-                           The returned prompt can be combined with more instructions and context.
-        """
         user, email = get_git_user_info()
         prompt = OpenAIPrompt(self.config.model, user, email)
         prompt.set_request(request)
         return prompt
 
-    def complete_response(self, prompt: OpenAIPrompt) -> str:
-        """
-        Retrieve a complete response JSON string from the chat system.
+    def load_prompt(self, data: dict) -> OpenAIPrompt:
+        data['_new_messages'] = {
+            k: [OpenAIMessage(**m) for m in v] if isinstance(v, list) else OpenAIMessage(**v)
+            for k, v in data['_new_messages'].items()
+        }
+        data['_history_messages'] = {k: [OpenAIMessage(**m) for m in v]
+                                     for k, v in data['_history_messages'].items()}
+        return OpenAIPrompt(**data)
 
-        Args:
-            prompt (Prompt): A prompt of messages representing the conversation.
-        Returns:
-            str: A JSON string representing the complete response.
-        """
+    def complete_response(self, prompt: OpenAIPrompt) -> str:
         # Filter the config parameters with non-None values
         config_params = {
             key: value
             for key, value in self.config.dict().items() if value is not None
         }
         config_params['stream'] = False
 
         response = openai.ChatCompletion.create(
             messages=prompt.messages,
             **config_params
         )
         return response
 
     def stream_response(self, prompt: OpenAIPrompt) -> Iterator[str]:
-        """
-        Retrieve a streaming response as an iterator of JSON strings from the chat system.
-
-        Args:
-            prompt (Prompt): A prompt of messages representing the conversation.
-        Returns:
-            Iterator[str]: An iterator over JSON strings representing the streaming response events.
-        """
         # Filter the config parameters with non-None values
         config_params = {
             key: value
             for key, value in self.config.dict().items() if value is not None
         }
         config_params['stream'] = True
```

### Comparing `devchat-0.1.7/devchat/openai/openai_message.py` & `devchat-0.1.8/devchat/openai/openai_message.py`

 * *Files identical despite different names*

### Comparing `devchat-0.1.7/devchat/openai/openai_prompt.py` & `devchat-0.1.8/devchat/openai/openai_prompt.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,73 +1,69 @@
+from dataclasses import dataclass
 import json
 import math
 from typing import List
 from devchat.prompt import Prompt
-from devchat.message import MessageType, Message
+from devchat.message import Message
 from devchat.utils import update_dict, message_tokens
 from .openai_message import OpenAIMessage
 
 
+@dataclass
 class OpenAIPrompt(Prompt):
     """
     A class to represent a prompt and its corresponding responses from OpenAI APIs.
     """
 
-    def __init__(self, model: str, user_name: str, user_email: str):
-        super().__init__(model, user_name, user_email)
-        self._id: str = None
-
-    @property
-    def model(self) -> str:
-        return self._model
+    _id: str = None
 
     @property
     def id(self) -> str:
         return self._id
 
     @property
     def messages(self) -> List[dict]:
         combined = []
         # Instruction
-        if self._new_messages[MessageType.INSTRUCT]:
-            combined += [msg.to_dict() for msg in self._new_messages[MessageType.INSTRUCT]]
+        if self._new_messages[Message.INSTRUCT]:
+            combined += [msg.to_dict() for msg in self._new_messages[Message.INSTRUCT]]
         # History context
-        if self._history_messages[MessageType.CONTEXT]:
+        if self._history_messages[Message.CONTEXT]:
             combined += [update_dict(msg.to_dict(), 'content',
                                      f"<context>\n{msg.content}\n</context>")
                          for msg in self.new_context]
         # History chat
-        if self._history_messages[MessageType.CHAT]:
+        if self._history_messages[Message.CHAT]:
             combined += [msg.to_dict() for msg
-                         in reversed(self._history_messages[MessageType.CHAT])]
+                         in reversed(self._history_messages[Message.CHAT])]
         # Request
         if self.request:
             combined += [self.request.to_dict()]
         # New context
         if self.new_context:
             combined += [update_dict(msg.to_dict(), 'content',
                                      f"<context>\n{msg.content}\n</context>")
                          for msg in self.new_context]
         return combined
 
-    def append_new(self, message_type: MessageType, content: str,
+    def append_new(self, message_type: str, content: str,
                    available_tokens: int = math.inf) -> bool:
-        if message_type not in (MessageType.INSTRUCT, MessageType.CONTEXT):
+        if message_type not in (Message.INSTRUCT, Message.CONTEXT):
             raise ValueError(f"Current messages cannot be of type {message_type}.")
         message = OpenAIMessage(content, 'system')
         num_tokens = message_tokens(message.to_dict(), self.model)
         if num_tokens > available_tokens:
             return False
         self._new_messages[message_type].append(message)
         self._request_tokens += num_tokens
         return True
 
-    def append_history(self, message_type: MessageType, message: Message,
+    def append_history(self, message_type: str, message: Message,
                        available_tokens: int = math.inf) -> bool:
-        if message_type == MessageType.INSTRUCT:
+        if message_type == Message.INSTRUCT:
             raise ValueError("History messages cannot be of type INSTRUCT.")
         num_tokens = message_tokens(message.to_dict(), self.model)
         if num_tokens > available_tokens:
             return False
         self._history_messages[message_type].append(message)
         self._request_tokens += num_tokens
         return True
@@ -90,18 +86,19 @@
         self._validate_model(response_data)
         self._timestamp_from_dict(response_data)
         self._id_from_dict(response_data)
 
         self._request_tokens = response_data['usage']['prompt_tokens']
         self._response_tokens = response_data['usage']['completion_tokens']
 
-        self._new_messages['response'] = {
-            choice['index']: OpenAIMessage(**choice['message'])
-            for choice in response_data['choices']
-        }
+        for choice in response_data['choices']:
+            index = choice['index']
+            if index >= len(self.response):
+                self.response.extend([None] * (index - len(self.response) + 1))
+            self.response[index] = OpenAIMessage(**choice['message'])
         self.set_hash()
 
     def append_response(self, delta_str: str) -> str:
         """
         Append the content of a streaming response to the existing messages.
 
         Args:
@@ -116,15 +113,18 @@
         self._id_from_dict(response_data)
 
         delta_content = ''
         for choice in response_data['choices']:
             delta = choice['delta']
             index = choice['index']
 
-            if index not in self.response:
+            if index >= len(self.response):
+                self.response.extend([None] * (index - len(self.response) + 1))
+
+            if not self.response[index]:
                 self.response[index] = OpenAIMessage(**delta)
                 if index == 0:
                     delta_content = self.formatted_header()
                     delta_content += self.response[0].content
             else:
                 if index == 0:
                     delta_content = self.response[0].stream_from_dict(delta)
```

### Comparing `devchat-0.1.7/devchat/prompt.py` & `devchat-0.1.8/devchat/prompt.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,79 +1,79 @@
 from abc import ABC, abstractmethod
+from dataclasses import dataclass, field, asdict
 import hashlib
 import math
 from typing import Dict, List
-from devchat.message import MessageType, Message
-from devchat.utils import unix_to_local_datetime
+from devchat.message import Message
+from devchat.utils import unix_to_local_datetime, setup_logger
 
 
+logger = setup_logger(__name__)
+
+
+@dataclass
 class Prompt(ABC):
     """
     A class to represent a prompt and its corresponding responses from the chat API.
 
     Attributes:
-        _model (str): The name of the language model.
-        _user_name (str): The name of the user.
-        _user_email (str): The email address of the user.
+        model (str): The name of the language model.
+        user_name (str): The name of the user.
+        user_email (str): The email address of the user.
         _new_messages (dict): The messages for the current round of conversation.
         _history_messages (dict): The messages for the history of conversation.
         parent (str): The parent prompt hash.
         references (List[str]): The hashes of the referenced prompts.
         _timestamp (int): The timestamp when the response was created.
         _request_tokens (int): The number of tokens used in the request.
         _response_tokens (int): The number of tokens used in the response.
         _hash (str): The hash of the prompt.
     """
 
-    def __init__(self, model: str, user_name: str, user_email: str):
-        self._model: str = model
-        self._user_name: str = user_name
-        self._user_email: str = user_email
-        self._new_messages = {
-            MessageType.INSTRUCT: [],
-            'request': None,
-            MessageType.CONTEXT: [],
-            'response': {}
-        }
-        self._history_messages: Dict[str, Message] = {
-            MessageType.CONTEXT: [],
-            MessageType.CHAT: []
-        }
-        self.parent: str = None
-        self.references: List[str] = []
-        self._timestamp: int = None
-        self._request_tokens: int = 0
-        self._response_tokens: int = 0
-        self._hash: str = None
+    model: str
+    user_name: str
+    user_email: str
+    _new_messages: Dict = field(default_factory=lambda: {
+        Message.INSTRUCT: [],
+        'request': None,
+        Message.CONTEXT: [],
+        'response': []
+    })
+    _history_messages: Dict[str, Message] = field(default_factory=lambda: {
+        Message.CONTEXT: [],
+        Message.CHAT: []
+    })
+    parent: str = None
+    references: List[str] = field(default_factory=list)
+    _timestamp: int = None
+    _request_tokens: int = 0
+    _response_tokens: int = 0
+    _hash: str = None
 
     @property
     def timestamp(self) -> int:
         return self._timestamp
 
     @property
     @abstractmethod
     def messages(self) -> List[dict]:
         """
         List of messages in the prompt to be sent to the chat API.
         """
 
     @property
-    def new_messages(self) -> dict:
-        return self._new_messages
-
-    @property
     def new_context(self) -> List[Message]:
-        return self._new_messages[MessageType.CONTEXT]
+        return self._new_messages[Message.CONTEXT]
 
     @property
     def request(self) -> Message:
         return self._new_messages['request']
 
     @property
-    def response(self) -> Dict[int, Message]:
+    def response(self) -> List[Message]:
         return self._new_messages['response']
 
     @property
     def request_tokens(self) -> int:
         return self._request_tokens
 
     @property
@@ -81,36 +81,36 @@
         return self._response_tokens
 
     @property
     def hash(self) -> str:
         return self._hash
 
     @abstractmethod
-    def append_new(self, message_type: MessageType, content: str,
+    def append_new(self, message_type: str, content: str,
                    available_tokens: int = math.inf) -> bool:
         """
         Append a new message provided by the user to the prompt.
 
         Args:
-            message_type (MessageType): The type of the message.
+            message_type (str): The type of the message.
             content (str): The content of the message.
             available_tokens (int): The number of tokens available for the message.
 
         Returns:
             bool: Whether the message is appended.
         """
 
     @abstractmethod
-    def append_history(self, message_type: MessageType, message: Message,
+    def append_history(self, message_type: str, message: Message,
                        available_tokens: int = math.inf) -> bool:
         """
         Add to the history messages of the prompt.
 
         Args:
-            message_type (MessageType): The type of the message.
+            message_type (str): The type of the message.
             message (Message): The message to add.
             available_tokens (int): The number of tokens available for the message.
 
         Returns:
             bool: Whether the message is appended.
         """
 
@@ -140,54 +140,68 @@
         Args:
             delta_str (str): The JSON-formatted delta string from the chat API.
 
         Returns:
             str: The delta content with index 0. None when the response is over.
         """
 
-    def set_hash(self):
-        """Set the hash of the prompt."""
+    def set_hash(self) -> str:
+        """
+        Calculate and set the hash of the prompt.
+
+        Returns:
+            str: The hash of the prompt. None if the prompt is incomplete.
+        """
         if not self.request or not self.response:
-            raise ValueError("Prompt is incomplete for hash.")
-        hash_str = self.request.content
-        for response in self.response.values():
-            hash_str += response.content
-        self._hash = hashlib.sha1(hash_str.encode()).hexdigest()
+            logger.error("Prompt is incomplete for hash.")
+            return None
+        data = asdict(self)
+        assert data.pop('_hash') is None
+        string = str(tuple(sorted(data.items())))
+        self._hash = hashlib.sha256(string.encode('utf-8')).hexdigest()
         return self._hash
 
     def formatted_header(self) -> str:
         """Formatted string header of the prompt."""
-        formatted_str = f"User: {self._user_name} <{self._user_email}>\n"
+        formatted_str = f"User: {self.user_name} <{self.user_email}>\n"
 
         local_time = unix_to_local_datetime(self._timestamp)
         formatted_str += f"Date: {local_time.strftime('%a %b %d %H:%M:%S %Y %z')}\n\n"
 
         return formatted_str
 
     def formatted_response(self, index: int) -> str:
-        """Formatted response of the prompt."""
+        """
+        Formatted response of the prompt.
+
+        Args:
+            index (int): The index of the response to format.
+
+        Returns:
+            str: The formatted response string. None if the response is incomplete.
+        """
         formatted_str = self.formatted_header()
 
-        response = self.response.get(index, None)
-        if response is None or response.content is None:
-            raise ValueError(f"Response {index} is incomplete.")
+        if index >= len(self.response) or not self.response[index]:
+            logger.error("Response %d is incomplete for formatted response.", index)
+            return None
 
-        formatted_str += response.content.strip() + "\n\n"
+        formatted_str += self.response[index].content.strip() + "\n\n"
         formatted_str += f"prompt {self.hash}"
 
         return formatted_str
 
     def shortlog(self) -> List[dict]:
         """Generate a shortlog of the prompt."""
         if not self.request or not self.response:
             raise ValueError("Prompt is incomplete for shortlog.")
         logs = []
-        for message in self.response.values():
+        for message in self.response:
             shortlog_data = {
-                "user": f"{self._user_name} <{self._user_email}>",
+                "user": f"{self.user_name} <{self.user_email}>",
                 "date": self._timestamp,
                 "context": [msg.to_dict() for msg in self.new_context],
                 "request": self.request.content,
                 "response": message.content,
                 "hash": self.hash,
                 "parent": self.parent
             }
```

### Comparing `devchat-0.1.7/devchat/store.py` & `devchat-0.1.8/devchat/store.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,44 +1,46 @@
+from dataclasses import asdict
 import os
-import shelve
 from typing import List
 from xml.etree.ElementTree import ParseError
 import networkx as nx
+from tinydb import TinyDB, where
+from devchat.chat import Chat
 from devchat.prompt import Prompt
+from devchat.utils import setup_logger
+
+
+logger = setup_logger(__name__)
 
 
 class Store:
-    def __init__(self, store_dir: str):
+    def __init__(self, store_dir: str, chat: Chat):
         """
         Initializes a Store instance.
 
         Args:
             path (str): The folder to store the files containing the store.
         """
         store_dir = os.path.expanduser(store_dir)
         if not os.path.isdir(store_dir):
             os.makedirs(store_dir)
+
         self._graph_path = os.path.join(store_dir, 'prompts.graphml')
-        self._db_path = os.path.join(store_dir, 'prompts')
+        self._db_path = os.path.join(store_dir, 'prompts.json')
+        self._chat = chat
 
         if os.path.isfile(self._graph_path):
             try:
                 self._graph = nx.read_graphml(self._graph_path)
             except ParseError as error:
                 raise ValueError(f"Invalid file format for graph: {self._graph_path}") from error
         else:
             self._graph = nx.DiGraph()
 
-        self._db = shelve.open(self._db_path)
-
-    def __del__(self):
-        """
-        Close the shelve file when the Store object is destroyed.
-        """
-        self._db.close()
+        self._db = TinyDB(self._db_path)
 
     @property
     def graph_path(self) -> str:
         """
         The path to the graph store file.
         """
         return self._graph_path
@@ -56,46 +58,53 @@
 
         Args:
             prompt (Prompt): The prompt to store.
         """
         if not prompt.hash:
             prompt.set_hash()
 
-        # Store the prompt object in the shelve database
-        self._db[prompt.hash] = prompt
-        self._db.sync()
+        # Store the prompt object in TinyDB
+        self._db.insert(asdict(prompt))
 
         # Add the prompt to the graph
         self._graph.add_node(prompt.hash, timestamp=prompt.timestamp)
 
         # Add edges for parents and references
         if prompt.parent:
             if prompt.parent not in self._graph:
-                raise ValueError(f'Parent {prompt.parent} not found in the store.')
-            self._graph.add_edge(prompt.hash, prompt.parent)
+                logger.warning("Parent %s not found in the store.", prompt.parent)
+            else:
+                self._graph.add_edge(prompt.hash, prompt.parent)
         for reference_hash in prompt.references:
             if reference_hash not in self._graph:
-                raise ValueError(f'Reference {reference_hash} not found in the store.')
-            self._graph.add_edge(prompt.hash, reference_hash)
+                logger.warning("Reference %s not found in the store.", reference_hash)
+            else:
+                self._graph.add_edge(prompt.hash, reference_hash)
         nx.write_graphml(self._graph, self._graph_path)
 
     def get_prompt(self, prompt_hash: str) -> Prompt:
         """
         Retrieve a prompt from the store.
 
         Args:
             prompt_hash (str): The hash of the prompt to retrieve.
         Returns:
-            Prompt: The retrieved prompt.
+            Prompt: The retrieved prompt. None if the prompt is not found.
         """
         if prompt_hash not in self._graph:
-            raise ValueError(f'Prompt {prompt_hash} not found in the store.')
+            logger.warning("Prompt %s not found in the graph store.", prompt_hash)
+            return None
 
-        # Retrieve the prompt object from the shelve database
-        return self._db[prompt_hash]
+        # Retrieve the prompt object from TinyDB
+        prompt_data = self._db.search(where('_hash') == prompt_hash)
+        if not prompt_data:
+            logger.warning("Prompt %s not found in the object store.", prompt_hash)
+            return None
+        assert len(prompt_data) == 1
+        return self._chat.load_prompt(prompt_data[0])
 
     def select_recent(self, start: int, end: int) -> List[Prompt]:
         """
         Select recent prompts.
 
         Args:
             start (int): The start index.
@@ -106,8 +115,15 @@
                           the list will contain prompts from start to the end of the list.
         """
         sorted_nodes = sorted(self._graph.nodes(data=True),
                               key=lambda x: x[1]['timestamp'],
                               reverse=True)
         if end > len(sorted_nodes):
             end = len(sorted_nodes)
-        return [self.get_prompt(note[0]) for note in sorted_nodes[start:end]]
+        prompts = []
+        for node in sorted_nodes[start:end]:
+            prompt = self.get_prompt(node[0])
+            if not prompt:
+                logger.error("Selected prompt %s not found in the store.", node[0])
+                continue
+            prompts.append(prompt)
+        return prompts
```

### Comparing `devchat-0.1.7/devchat/utils.py` & `devchat-0.1.8/devchat/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,40 @@
 """
 utils.py - Utility functions for DevChat.
 """
+import logging
 import os
 import re
+import sys
 import getpass
 import socket
 import subprocess
 from typing import List, Tuple
 import datetime
 import pytz
 from dateutil import tz
 import tiktoken
 
 
+def setup_logger(name, level=logging.WARNING):
+    """Utility function to set up a logger with the specified name and level."""
+    formatter = logging.Formatter('%(asctime)s - %(name)s - %(levelname)s - %(message)s')
+
+    # Create a file handler for logging
+    console_handler = logging.StreamHandler(sys.stderr)
+    console_handler.setFormatter(formatter)
+
+    # Create a logger with the given name
+    logger = logging.getLogger(name)
+    logger.setLevel(level)
+    logger.addHandler(console_handler)
+
+    return logger
+
+
 def find_git_root():
     try:
         root = subprocess.check_output(["git", "rev-parse", "--show-toplevel"])
         return root.decode("utf-8").strip()
     except subprocess.CalledProcessError as error:
         raise RuntimeError("Not inside a Git repository") from error
 
@@ -91,30 +109,22 @@
             content = file.read()
             if not content:
                 raise ValueError(f"File {file_path} is empty.")
             contents.append(content)
     return contents
 
 
-def is_valid_hash(hash_str):
+def valid_hash(hash_str):
     """Check if a string is a valid hash value."""
     # Hash values are usually alphanumeric with a fixed length
     # depending on the algorithm used to generate them
-    pattern = re.compile(r'^[a-fA-F0-9]{40}$')  # Example pattern for SHA-1 hash
+    pattern = re.compile(r'^[a-f0-9]{64}$')  # Example pattern for SHA-256 hash
     return bool(pattern.match(hash_str))
 
 
-def validate_hashes(hashes: List[str]) -> List[str]:
-    if hashes:
-        for value in hashes:
-            if not is_valid_hash(value):
-                raise ValueError(f"Invalid hash value {value}.")
-    return hashes
-
-
 def update_dict(dict_to_update, key, value) -> dict:
     """
     Update a dictionary with a key-value pair and return the dictionary.
     """
     dict_to_update[key] = value
     return dict_to_update
```

### Comparing `devchat-0.1.7/devchat.egg-info/PKG-INFO` & `devchat-0.1.8/devchat.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: devchat
-Version: 0.1.7
+Version: 0.1.8
 Summary: DevChat is an open-source tool that helps developers write prompts to generate code and documentation.
 Home-page: https://github.com/covespace/devchat
 License: Apache License 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
```

### Comparing `devchat-0.1.7/devchat.egg-info/SOURCES.txt` & `devchat-0.1.8/devchat.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `devchat-0.1.7/setup.py` & `devchat-0.1.8/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 
 # Read the contents of the README.md file
 long_description = read_file("README.md")
 
 setup(
     name="devchat",
-    version="0.1.7",
+    version="0.1.8",
     packages=find_packages(),
     install_requires=requirements,
     entry_points={
         "console_scripts": [
             "devchat = devchat._cli:main",
         ],
     },
```

### Comparing `devchat-0.1.7/tests/test_cli.py` & `devchat-0.1.8/tests/test_cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,21 +39,21 @@
 
 def test_main_no_args(git_repo):  # pylint: disable=W0613
     result = runner.invoke(main, ['prompt'])
     assert result.exit_code == 0
 
 
 def _check_output_format(output) -> bool:
-    pattern = r"(User: .+ <.+@.+>\nDate: .+\n\n(?:.*\n)*\n(?:prompt [a-f0-9]{40}\n\n?)+)"
+    pattern = r"(User: .+ <.+@.+>\nDate: .+\n\n(?:.*\n)*\n(?:prompt [a-f0-9]{64}\n\n?)+)"
     return bool(re.fullmatch(pattern, output))
 
 
 def _get_core_content(output) -> str:
     header_pattern = r"User: .+ <.+@.+>\nDate: .+\n\n"
-    footer_pattern = r"\n(?:prompt [a-f0-9]{40}\n\n?)+"
+    footer_pattern = r"\n(?:prompt [a-f0-9]{64}\n\n?)+"
 
     core_content = re.sub(header_pattern, "", output)
     core_content = re.sub(footer_pattern, "", core_content)
 
     return core_content
```

### Comparing `devchat-0.1.7/tests/test_openai_message.py` & `devchat-0.1.8/tests/test_openai_message.py`

 * *Files identical despite different names*

### Comparing `devchat-0.1.7/tests/test_openai_prompt.py` & `devchat-0.1.8/tests/test_openai_prompt.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import json
 import os
 import pytest
-from devchat.message import MessageType
+from devchat.message import Message
 from devchat.openai import OpenAIMessage
 from devchat.openai import OpenAIPrompt
 from devchat.utils import get_git_user_info
 
 
 def test_prompt_init_and_set_response():
     name, email = get_git_user_info()
@@ -99,44 +99,44 @@
 
     expected_messages = [
         OpenAIMessage(role='assistant', content='Tomorrow.'),
         OpenAIMessage(role='assistant', content='Tomorrow!')
     ]
 
     assert len(prompt.response) == len(expected_messages)
-    for index, message in prompt.response.items():
+    for index, message in enumerate(prompt.response):
         assert message.role == expected_messages[index].role
         assert message.content == expected_messages[index].content
 
 
 def test_messages_empty():
     prompt = OpenAIPrompt("davinci-codex", "John Doe", "john.doe@example.com")
     assert prompt.messages == []
 
 
 def test_messages_instruct():
     prompt = OpenAIPrompt("davinci-codex", "John Doe", "john.doe@example.com")
     instruct_message = OpenAIMessage('Instructions', 'system')
-    prompt.append_new(MessageType.INSTRUCT, 'Instructions')
+    prompt.append_new(Message.INSTRUCT, 'Instructions')
     assert prompt.messages == [instruct_message.to_dict()]
 
 
 def test_messages_context():
     prompt = OpenAIPrompt("davinci-codex", "John Doe", "john.doe@example.com")
     context_message = OpenAIMessage('Context', 'system')
-    prompt.append_new(MessageType.CONTEXT, 'Context')
+    prompt.append_new(Message.CONTEXT, 'Context')
     expected_message = context_message.to_dict()
     expected_message["content"] = "<context>\n" + context_message.content + "\n</context>"
     assert prompt.messages == [expected_message]
 
 
 def test_messages_record():
     prompt = OpenAIPrompt("davinci-codex", "John Doe", "john.doe@example.com")
     with pytest.raises(ValueError):
-        prompt.append_new(MessageType.CHAT, 'Record')
+        prompt.append_new(Message.CHAT, 'Record')
 
 
 def test_messages_request():
     prompt = OpenAIPrompt("davinci-codex", "John Doe", "john.doe@example.com")
     request_message = OpenAIMessage('Request', 'user')
     prompt.set_request('Request')
     expected_message = request_message.to_dict()
@@ -145,16 +145,16 @@
 
 def test_messages_combined():
     prompt = OpenAIPrompt("davinci-codex", "John Doe", "john.doe@example.com")
     instruct_message = OpenAIMessage('Instructions', 'system')
     context_message = OpenAIMessage('Context', 'system')
     request_message = OpenAIMessage('Request', 'user')
 
-    prompt.append_new(MessageType.INSTRUCT, 'Instructions')
-    prompt.append_new(MessageType.CONTEXT, 'Context')
+    prompt.append_new(Message.INSTRUCT, 'Instructions')
+    prompt.append_new(Message.CONTEXT, 'Context')
     prompt.set_request('Request')
 
     expected_context_message = context_message.to_dict()
     expected_context_message["content"] = "<context>\n" + context_message.content + "\n</context>"
 
     expected_request_message = request_message.to_dict()
     expected_request_message["content"] = request_message.content
```

### Comparing `devchat-0.1.7/tests/test_store.py` & `devchat-0.1.8/tests/test_store.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,17 +1,16 @@
-from devchat.openai import OpenAIPrompt
+from devchat.openai import OpenAIChatConfig, OpenAIChat
 from devchat.store import Store
-from devchat.utils import get_git_user_info
 
 
 def test_get_prompt(tmp_path):
-    store = Store(tmp_path / "store.graphml")
-    name, email = get_git_user_info()
-    prompt = OpenAIPrompt(model="gpt-3.5-turbo", user_name=name, user_email=email)
-    prompt.set_request("Where was the 2020 World Series played?")
+    config = OpenAIChatConfig(model="gpt-3.5-turbo")
+    chat = OpenAIChat(config)
+    store = Store(tmp_path / "store.graphml", chat)
+    prompt = chat.init_prompt("Where was the 2020 World Series played?")
     response_str = '''
     {
       "id": "chatcmpl-6p9XYPYSTTRi0xEviKjjilqrWU2Ve",
       "object": "chat.completion",
       "created": 1577649420,
       "model": "gpt-3.5-turbo-0301",
       "usage": {"prompt_tokens": 56, "completion_tokens": 31, "total_tokens": 87},
@@ -30,22 +29,22 @@
     prompt.set_response(response_str)
     store.store_prompt(prompt)
 
     assert store.get_prompt(prompt.hash).timestamp == prompt.timestamp
 
 
 def test_select_recent(tmp_path):
-    store = Store(tmp_path / "store.graphml")
-    name, email = get_git_user_info()
+    config = OpenAIChatConfig(model="gpt-3.5-turbo")
+    chat = OpenAIChat(config)
+    store = Store(tmp_path / "store.graphml", chat)
 
     # Create and store 5 prompts
     hashes = []
     for index in range(5):
-        prompt = OpenAIPrompt(model="gpt-3.5-turbo", user_name=name, user_email=email)
-        prompt.set_request(f"Question {index}")
+        prompt = chat.init_prompt(f"Question {index}")
         response_str = f'''
         {{
           "id": "chatcmpl-6p9XYPYSTTRi0xEviKjjilqrWU2Ve",
           "object": "chat.completion",
           "created": 167764942{index},
           "model": "gpt-3.5-turbo-0301",
           "usage": {{"prompt_tokens": 56, "completion_tokens": 31, "total_tokens": 87}},
```

### Comparing `devchat-0.1.7/tests/test_utils.py` & `devchat-0.1.8/tests/test_utils.py`

 * *Files identical despite different names*

