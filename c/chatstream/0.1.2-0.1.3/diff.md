# Comparing `tmp/chatstream-0.1.2.tar.gz` & `tmp/chatstream-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chatstream-0.1.2.tar", last modified: Mon May 22 02:39:00 2023, max compression
+gzip compressed data, was "chatstream-0.1.3.tar", last modified: Mon May 22 04:54:09 2023, max compression
```

## Comparing `chatstream-0.1.2.tar` & `chatstream-0.1.3.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-05-22 02:39:00.391983 chatstream-0.1.2/
-drwxrwxrwx   0        0        0        0 2023-05-22 02:39:00.376145 chatstream-0.1.2/ChatStream.egg-info/
--rw-rw-rw-   0        0        0     6926 2023-05-22 02:39:00.000000 chatstream-0.1.2/ChatStream.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      768 2023-05-22 02:39:00.000000 chatstream-0.1.2/ChatStream.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-22 02:39:00.000000 chatstream-0.1.2/ChatStream.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2023-05-22 02:39:00.000000 chatstream-0.1.2/ChatStream.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-05-22 02:39:00.000000 chatstream-0.1.2/ChatStream.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    11356 2023-05-21 23:57:09.000000 chatstream-0.1.2/LICENSE
--rw-rw-rw-   0        0        0     6926 2023-05-22 02:39:00.391983 chatstream-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     6103 2023-05-22 01:43:46.000000 chatstream-0.1.2/README.md
-drwxrwxrwx   0        0        0        0 2023-05-22 02:39:00.389978 chatstream-0.1.2/chatstream/
--rw-rw-rw-   0        0        0      168 2023-05-21 23:57:09.000000 chatstream-0.1.2/chatstream/__init__.py
--rw-rw-rw-   0        0        0     8430 2023-05-21 23:57:09.000000 chatstream-0.1.2/chatstream/chat_core.py
--rw-rw-rw-   0        0        0     8648 2023-05-21 23:57:09.000000 chatstream-0.1.2/chatstream/chat_process.py
--rw-rw-rw-   0        0        0     2644 2023-05-21 23:57:09.000000 chatstream-0.1.2/chatstream/chat_process_mock.py
--rw-rw-rw-   0        0        0     6416 2023-05-22 01:34:57.000000 chatstream-0.1.2/chatstream/chat_prompt.py
--rw-rw-rw-   0        0        0    20904 2023-05-22 00:16:49.000000 chatstream-0.1.2/chatstream/chat_stream.py
--rw-rw-rw-   0        0        0     3146 2023-05-21 23:57:09.000000 chatstream-0.1.2/chatstream/mock_response_example_text.py
-drwxrwxrwx   0        0        0        0 2023-05-22 02:39:00.390982 chatstream-0.1.2/chatstream/request_handler/
--rw-rw-rw-   0        0        0        0 2023-05-21 23:57:09.000000 chatstream-0.1.2/chatstream/request_handler/__init__.py
--rw-rw-rw-   0        0        0     4071 2023-05-21 23:57:09.000000 chatstream-0.1.2/chatstream/request_handler/request_handler.py
--rw-rw-rw-   0        0        0     4916 2023-05-21 23:57:09.000000 chatstream-0.1.2/chatstream/request_handler/simple_session_request_handler.py
--rw-rw-rw-   0        0        0     3356 2023-05-21 23:57:09.000000 chatstream-0.1.2/chatstream/sampling_utils.py
--rw-rw-rw-   0        0        0      803 2023-05-21 23:57:09.000000 chatstream-0.1.2/chatstream/util_request_id.py
--rw-rw-rw-   0        0        0       42 2023-05-22 02:39:00.391983 chatstream-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0     1001 2023-05-22 02:38:03.000000 chatstream-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-22 04:54:09.835131 chatstream-0.1.3/
+drwxrwxrwx   0        0        0        0 2023-05-22 04:54:09.769747 chatstream-0.1.3/ChatStream.egg-info/
+-rw-rw-rw-   0        0        0     7337 2023-05-22 04:54:09.000000 chatstream-0.1.3/ChatStream.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      768 2023-05-22 04:54:09.000000 chatstream-0.1.3/ChatStream.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-22 04:54:09.000000 chatstream-0.1.3/ChatStream.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       28 2023-05-22 04:54:09.000000 chatstream-0.1.3/ChatStream.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-05-22 04:54:09.000000 chatstream-0.1.3/ChatStream.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    11356 2023-05-21 23:57:09.000000 chatstream-0.1.3/LICENSE
+-rw-rw-rw-   0        0        0     7337 2023-05-22 04:54:09.835131 chatstream-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     6485 2023-05-22 04:52:49.000000 chatstream-0.1.3/README.md
+drwxrwxrwx   0        0        0        0 2023-05-22 04:54:09.828133 chatstream-0.1.3/chatstream/
+-rw-rw-rw-   0        0        0      168 2023-05-21 23:57:09.000000 chatstream-0.1.3/chatstream/__init__.py
+-rw-rw-rw-   0        0        0     8430 2023-05-21 23:57:09.000000 chatstream-0.1.3/chatstream/chat_core.py
+-rw-rw-rw-   0        0        0     8648 2023-05-21 23:57:09.000000 chatstream-0.1.3/chatstream/chat_process.py
+-rw-rw-rw-   0        0        0     2644 2023-05-21 23:57:09.000000 chatstream-0.1.3/chatstream/chat_process_mock.py
+-rw-rw-rw-   0        0        0     6416 2023-05-22 01:34:57.000000 chatstream-0.1.3/chatstream/chat_prompt.py
+-rw-rw-rw-   0        0        0    20904 2023-05-22 00:16:49.000000 chatstream-0.1.3/chatstream/chat_stream.py
+-rw-rw-rw-   0        0        0     3146 2023-05-21 23:57:09.000000 chatstream-0.1.3/chatstream/mock_response_example_text.py
+drwxrwxrwx   0        0        0        0 2023-05-22 04:54:09.834129 chatstream-0.1.3/chatstream/request_handler/
+-rw-rw-rw-   0        0        0        0 2023-05-21 23:57:09.000000 chatstream-0.1.3/chatstream/request_handler/__init__.py
+-rw-rw-rw-   0        0        0     4071 2023-05-21 23:57:09.000000 chatstream-0.1.3/chatstream/request_handler/request_handler.py
+-rw-rw-rw-   0        0        0     4916 2023-05-21 23:57:09.000000 chatstream-0.1.3/chatstream/request_handler/simple_session_request_handler.py
+-rw-rw-rw-   0        0        0     3356 2023-05-21 23:57:09.000000 chatstream-0.1.3/chatstream/sampling_utils.py
+-rw-rw-rw-   0        0        0      803 2023-05-21 23:57:09.000000 chatstream-0.1.3/chatstream/util_request_id.py
+-rw-rw-rw-   0        0        0       42 2023-05-22 04:54:09.835131 chatstream-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      985 2023-05-22 04:53:08.000000 chatstream-0.1.3/setup.py
```

### Comparing `chatstream-0.1.2/ChatStream.egg-info/PKG-INFO` & `chatstream-0.1.3/ChatStream.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatstream
-Version: 0.1.2
+Version: 0.1.3
 Summary: Streaming chat server building blocks for FastAPI/Starlette
 Home-page: https://github.com/riversun/ChatStream
 Author: Tom Misawa
 Author-email: riversun.org@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
@@ -21,49 +21,78 @@
 
 ## Installation
 
 ```
 pip install chatstream
 ```
 
-
 ## What can it do?
 
 ### 1. Simplifies the construction of streaming chats
 
 You can easily construct streaming chats with large pre-trained language models based on HuggingFace.
 
 **What is a Streaming Chat**
 
-When generating sentences with a large language model, there are methods that generate the next sentence entirely based on the inputted prompt (and the conversation history so far) before outputting it, and methods that sequentially output the next sentence one token at a time. The latter method is specifically referred to as 'streaming'. In this package, token generation is done one token at a time, and it is streamed as a response to the client. This contributes to a better user experience compared to waiting for the entire sentence to be generated.
+When generating sentences with a large language model, there are methods that generate the next sentence entirely based
+on the inputted prompt (and the conversation history so far) before outputting it, and methods that sequentially output
+the next sentence one token at a time. The latter method is specifically referred to as 'streaming'. In this package,
+token generation is done one token at a time, and it is streamed as a response to the client. This contributes to a
+better user experience compared to waiting for the entire sentence to be generated.
 
 ### 2. Automatically maintains conversation history and context
 
-By default, the HTTP session feature keeps the conversation history between the user and the language model in on-memory on the server-side. The session duration can be set, but it is basically while the browser is open. This makes it possible to have multi-round web chats with continued context.
+By default, the HTTP session feature keeps the conversation history between the user and the language model in on-memory
+on the server-side. The session duration can be set, but it is basically while the browser is open. This makes it
+possible to have multi-round web chats with continued context.
 
 ### 3. Control of concurrent access from multiple users
 
-It is designed with concurrent access from multiple clients in mind, and is controlled according to the following parameters specified in the constructor
+It is designed with concurrent access from multiple clients in mind, and is controlled according to the following
+parameters specified in the constructor
 
-`num_of_concurrent_executions` : int ... The number of concurrent sentence generation tasks to the pre-trained language model  
+`num_of_concurrent_executions` : int ... The number of concurrent sentence generation tasks to the pre-trained language
+model
 
-`max_queue_size: int` ... The size of the queue for sentence generation. When the number of concurrent sentence generation tasks falls below the limit
+`max_queue_size: int` ... The size of the queue for sentence generation. When the number of concurrent sentence
+generation tasks falls below the limit
 
 ![img](https://github.com/riversun/ChatStream/assets/11747460/f743ba6a-64ec-4f44-80aa-ba9a8d9c7875)
 
-
 # How to use
 
 The following is an example of streaming chat using `togethercomputer/RedPajama-INCITE-Chat-3B-v1` as a model
 
-Create a chat_prompt class (chat_prompt_for_redpajama_incite.py) that generates prompts for the model and a server.py that acts as a streaming server.
+Create a chat_prompt class (chat_prompt_for_redpajama_incite.py) that generates prompts for the model and a server.py
+that acts as a streaming server.
 
-**chat_prompt_for_redpajama_incite.py**
+## Required Packages for the Demo Code
+
+- Pytorch  
+  If you're using CUDA, please install the CUDA-compatible version of pytorch.
+
+```
+pip install torch torchvision torchaudio --index-url https://download.pytorch.org/whl/cu117
+```
+
+- HuggingFace Transformer Library
 
+```
+pip install transformers
+```
+
+- Web server
+
+uvicorn or gunicorn
 
+```
+pip install "uvicorn[standard]" gunicorn 
+```
+
+**chat_prompt_for_redpajama_incite.py**
 
 ```python
 from chatstream.chat_prompt import AbstractChatPrompt
 
 
 class ChatPromptRedpajamaIncite(AbstractChatPrompt):
```

### Comparing `chatstream-0.1.2/ChatStream.egg-info/SOURCES.txt` & `chatstream-0.1.3/ChatStream.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `chatstream-0.1.2/LICENSE` & `chatstream-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `chatstream-0.1.2/PKG-INFO` & `chatstream-0.1.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatstream
-Version: 0.1.2
+Version: 0.1.3
 Summary: Streaming chat server building blocks for FastAPI/Starlette
 Home-page: https://github.com/riversun/ChatStream
 Author: Tom Misawa
 Author-email: riversun.org@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
@@ -21,49 +21,78 @@
 
 ## Installation
 
 ```
 pip install chatstream
 ```
 
-
 ## What can it do?
 
 ### 1. Simplifies the construction of streaming chats
 
 You can easily construct streaming chats with large pre-trained language models based on HuggingFace.
 
 **What is a Streaming Chat**
 
-When generating sentences with a large language model, there are methods that generate the next sentence entirely based on the inputted prompt (and the conversation history so far) before outputting it, and methods that sequentially output the next sentence one token at a time. The latter method is specifically referred to as 'streaming'. In this package, token generation is done one token at a time, and it is streamed as a response to the client. This contributes to a better user experience compared to waiting for the entire sentence to be generated.
+When generating sentences with a large language model, there are methods that generate the next sentence entirely based
+on the inputted prompt (and the conversation history so far) before outputting it, and methods that sequentially output
+the next sentence one token at a time. The latter method is specifically referred to as 'streaming'. In this package,
+token generation is done one token at a time, and it is streamed as a response to the client. This contributes to a
+better user experience compared to waiting for the entire sentence to be generated.
 
 ### 2. Automatically maintains conversation history and context
 
-By default, the HTTP session feature keeps the conversation history between the user and the language model in on-memory on the server-side. The session duration can be set, but it is basically while the browser is open. This makes it possible to have multi-round web chats with continued context.
+By default, the HTTP session feature keeps the conversation history between the user and the language model in on-memory
+on the server-side. The session duration can be set, but it is basically while the browser is open. This makes it
+possible to have multi-round web chats with continued context.
 
 ### 3. Control of concurrent access from multiple users
 
-It is designed with concurrent access from multiple clients in mind, and is controlled according to the following parameters specified in the constructor
+It is designed with concurrent access from multiple clients in mind, and is controlled according to the following
+parameters specified in the constructor
 
-`num_of_concurrent_executions` : int ... The number of concurrent sentence generation tasks to the pre-trained language model  
+`num_of_concurrent_executions` : int ... The number of concurrent sentence generation tasks to the pre-trained language
+model
 
-`max_queue_size: int` ... The size of the queue for sentence generation. When the number of concurrent sentence generation tasks falls below the limit
+`max_queue_size: int` ... The size of the queue for sentence generation. When the number of concurrent sentence
+generation tasks falls below the limit
 
 ![img](https://github.com/riversun/ChatStream/assets/11747460/f743ba6a-64ec-4f44-80aa-ba9a8d9c7875)
 
-
 # How to use
 
 The following is an example of streaming chat using `togethercomputer/RedPajama-INCITE-Chat-3B-v1` as a model
 
-Create a chat_prompt class (chat_prompt_for_redpajama_incite.py) that generates prompts for the model and a server.py that acts as a streaming server.
+Create a chat_prompt class (chat_prompt_for_redpajama_incite.py) that generates prompts for the model and a server.py
+that acts as a streaming server.
 
-**chat_prompt_for_redpajama_incite.py**
+## Required Packages for the Demo Code
+
+- Pytorch  
+  If you're using CUDA, please install the CUDA-compatible version of pytorch.
+
+```
+pip install torch torchvision torchaudio --index-url https://download.pytorch.org/whl/cu117
+```
+
+- HuggingFace Transformer Library
 
+```
+pip install transformers
+```
+
+- Web server
+
+uvicorn or gunicorn
 
+```
+pip install "uvicorn[standard]" gunicorn 
+```
+
+**chat_prompt_for_redpajama_incite.py**
 
 ```python
 from chatstream.chat_prompt import AbstractChatPrompt
 
 
 class ChatPromptRedpajamaIncite(AbstractChatPrompt):
```

### Comparing `chatstream-0.1.2/README.md` & `chatstream-0.1.3/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -4,49 +4,78 @@
 
 ## Installation
 
 ```
 pip install chatstream
 ```
 
-
 ## What can it do?
 
 ### 1. Simplifies the construction of streaming chats
 
 You can easily construct streaming chats with large pre-trained language models based on HuggingFace.
 
 **What is a Streaming Chat**
 
-When generating sentences with a large language model, there are methods that generate the next sentence entirely based on the inputted prompt (and the conversation history so far) before outputting it, and methods that sequentially output the next sentence one token at a time. The latter method is specifically referred to as 'streaming'. In this package, token generation is done one token at a time, and it is streamed as a response to the client. This contributes to a better user experience compared to waiting for the entire sentence to be generated.
+When generating sentences with a large language model, there are methods that generate the next sentence entirely based
+on the inputted prompt (and the conversation history so far) before outputting it, and methods that sequentially output
+the next sentence one token at a time. The latter method is specifically referred to as 'streaming'. In this package,
+token generation is done one token at a time, and it is streamed as a response to the client. This contributes to a
+better user experience compared to waiting for the entire sentence to be generated.
 
 ### 2. Automatically maintains conversation history and context
 
-By default, the HTTP session feature keeps the conversation history between the user and the language model in on-memory on the server-side. The session duration can be set, but it is basically while the browser is open. This makes it possible to have multi-round web chats with continued context.
+By default, the HTTP session feature keeps the conversation history between the user and the language model in on-memory
+on the server-side. The session duration can be set, but it is basically while the browser is open. This makes it
+possible to have multi-round web chats with continued context.
 
 ### 3. Control of concurrent access from multiple users
 
-It is designed with concurrent access from multiple clients in mind, and is controlled according to the following parameters specified in the constructor
+It is designed with concurrent access from multiple clients in mind, and is controlled according to the following
+parameters specified in the constructor
 
-`num_of_concurrent_executions` : int ... The number of concurrent sentence generation tasks to the pre-trained language model  
+`num_of_concurrent_executions` : int ... The number of concurrent sentence generation tasks to the pre-trained language
+model
 
-`max_queue_size: int` ... The size of the queue for sentence generation. When the number of concurrent sentence generation tasks falls below the limit
+`max_queue_size: int` ... The size of the queue for sentence generation. When the number of concurrent sentence
+generation tasks falls below the limit
 
 ![img](https://github.com/riversun/ChatStream/assets/11747460/f743ba6a-64ec-4f44-80aa-ba9a8d9c7875)
 
-
 # How to use
 
 The following is an example of streaming chat using `togethercomputer/RedPajama-INCITE-Chat-3B-v1` as a model
 
-Create a chat_prompt class (chat_prompt_for_redpajama_incite.py) that generates prompts for the model and a server.py that acts as a streaming server.
+Create a chat_prompt class (chat_prompt_for_redpajama_incite.py) that generates prompts for the model and a server.py
+that acts as a streaming server.
 
-**chat_prompt_for_redpajama_incite.py**
+## Required Packages for the Demo Code
+
+- Pytorch  
+  If you're using CUDA, please install the CUDA-compatible version of pytorch.
+
+```
+pip install torch torchvision torchaudio --index-url https://download.pytorch.org/whl/cu117
+```
+
+- HuggingFace Transformer Library
 
+```
+pip install transformers
+```
+
+- Web server
+
+uvicorn or gunicorn
 
+```
+pip install "uvicorn[standard]" gunicorn 
+```
+
+**chat_prompt_for_redpajama_incite.py**
 
 ```python
 from chatstream.chat_prompt import AbstractChatPrompt
 
 
 class ChatPromptRedpajamaIncite(AbstractChatPrompt):
```

### Comparing `chatstream-0.1.2/chatstream/chat_core.py` & `chatstream-0.1.3/chatstream/chat_core.py`

 * *Files identical despite different names*

### Comparing `chatstream-0.1.2/chatstream/chat_process.py` & `chatstream-0.1.3/chatstream/chat_process.py`

 * *Files identical despite different names*

### Comparing `chatstream-0.1.2/chatstream/chat_process_mock.py` & `chatstream-0.1.3/chatstream/chat_process_mock.py`

 * *Files identical despite different names*

### Comparing `chatstream-0.1.2/chatstream/chat_prompt.py` & `chatstream-0.1.3/chatstream/chat_prompt.py`

 * *Files identical despite different names*

### Comparing `chatstream-0.1.2/chatstream/chat_stream.py` & `chatstream-0.1.3/chatstream/chat_stream.py`

 * *Files identical despite different names*

### Comparing `chatstream-0.1.2/chatstream/mock_response_example_text.py` & `chatstream-0.1.3/chatstream/mock_response_example_text.py`

 * *Files identical despite different names*

### Comparing `chatstream-0.1.2/chatstream/request_handler/request_handler.py` & `chatstream-0.1.3/chatstream/request_handler/request_handler.py`

 * *Files identical despite different names*

### Comparing `chatstream-0.1.2/chatstream/request_handler/simple_session_request_handler.py` & `chatstream-0.1.3/chatstream/request_handler/simple_session_request_handler.py`

 * *Files identical despite different names*

### Comparing `chatstream-0.1.2/chatstream/sampling_utils.py` & `chatstream-0.1.3/chatstream/sampling_utils.py`

 * *Files identical despite different names*

### Comparing `chatstream-0.1.2/chatstream/util_request_id.py` & `chatstream-0.1.3/chatstream/util_request_id.py`

 * *Files identical despite different names*

### Comparing `chatstream-0.1.2/setup.py` & `chatstream-0.1.3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,28 @@
 from setuptools import setup, find_packages
 
 setup(
     name="chatstream",
-    version="0.1.2",
+    version="0.1.3",
     author="Tom Misawa",
     author_email="riversun.org@gmail.com",
     description="Streaming chat server building blocks for FastAPI/Starlette",
     long_description=open("README.md", "r").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/riversun/ChatStream",
     packages=find_packages(exclude=["tests.*", "tests", "examples.*", "examples"]),
-    tests_require=["pytest", "httpx"],
+    tests_require=["pytest", "httpx", "transformers", "torch"],
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: Apache Software License",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
     ],
     python_requires=">=3.8",
     install_requires=[
-        "torch",
-        "transformers",
         "fastapi",
         "fastsession",
         "tokflow"
     ]
 )
```

