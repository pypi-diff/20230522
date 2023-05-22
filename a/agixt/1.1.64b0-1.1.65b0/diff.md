# Comparing `tmp/agixt-1.1.64b0.tar.gz` & `tmp/agixt-1.1.65b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agixt-1.1.64b0.tar", last modified: Mon May 22 00:58:50 2023, max compression
+gzip compressed data, was "agixt-1.1.65b0.tar", last modified: Mon May 22 01:44:49 2023, max compression
```

## Comparing `agixt-1.1.64b0.tar` & `agixt-1.1.65b0.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 00:58:50.185376 agixt-1.1.64b0/
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-05-22 00:58:37.000000 agixt-1.1.64b0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-22 00:58:37.000000 agixt-1.1.64b0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    13861 2023-05-22 00:58:50.185376 agixt-1.1.64b0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 00:58:50.181376 agixt-1.1.64b0/agixt/
--rw-r--r--   0 runner    (1001) docker     (123)    15962 2023-05-22 00:58:37.000000 agixt-1.1.64b0/agixt/AGiXT.py
--rw-r--r--   0 runner    (1001) docker     (123)    12848 2023-05-22 00:58:37.000000 agixt-1.1.64b0/agixt/Agent.py
--rw-r--r--   0 runner    (1001) docker     (123)     6997 2023-05-22 00:58:37.000000 agixt-1.1.64b0/agixt/Chain.py
--rw-r--r--   0 runner    (1001) docker     (123)     6153 2023-05-22 00:58:37.000000 agixt-1.1.64b0/agixt/Commands.py
--rw-r--r--   0 runner    (1001) docker     (123)      960 2023-05-22 00:58:37.000000 agixt-1.1.64b0/agixt/Config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-05-22 00:58:37.000000 agixt-1.1.64b0/agixt/CustomPrompt.py
--rw-r--r--   0 runner    (1001) docker     (123)     6337 2023-05-22 00:58:37.000000 agixt-1.1.64b0/agixt/Embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-05-22 00:58:37.000000 agixt-1.1.64b0/agixt/Main.py
--rw-r--r--   0 runner    (1001) docker     (123)     8367 2023-05-22 00:58:37.000000 agixt-1.1.64b0/agixt/Memories.py
--rw-r--r--   0 runner    (1001) docker     (123)     8476 2023-05-22 00:58:37.000000 agixt-1.1.64b0/agixt/Tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-05-22 00:58:37.000000 agixt-1.1.64b0/agixt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12961 2023-05-22 00:58:37.000000 agixt-1.1.64b0/agixt/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 00:58:50.185376 agixt-1.1.64b0/agixt/provider/
--rw-r--r--   0 runner    (1001) docker     (123)     2157 2023-05-22 00:58:37.000000 agixt-1.1.64b0/agixt/provider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-05-22 00:58:37.000000 agixt-1.1.64b0/agixt/provider/azure.py
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-05-22 00:58:37.000000 agixt-1.1.64b0/agixt/provider/bard.py
--rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-05-22 00:58:37.000000 agixt-1.1.64b0/agixt/provider/bing.py
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-05-22 00:58:37.000000 agixt-1.1.64b0/agixt/provider/chatgpt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-05-22 00:58:37.000000 agixt-1.1.64b0/agixt/provider/claude.py
--rw-r--r--   0 runner    (1001) docker     (123)      757 2023-05-22 00:58:37.000000 agixt-1.1.64b0/agixt/provider/fastchat.py
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-05-22 00:58:37.000000 agixt-1.1.64b0/agixt/provider/gpt4all.py
--rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-05-22 00:58:37.000000 agixt-1.1.64b0/agixt/provider/gpt4free.py
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-22 00:58:37.000000 agixt-1.1.64b0/agixt/provider/gpugpt4all.py
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-05-22 00:58:37.000000 agixt-1.1.64b0/agixt/provider/huggingchat.py
--rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-05-22 00:58:37.000000 agixt-1.1.64b0/agixt/provider/kobold.py
--rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-05-22 00:58:37.000000 agixt-1.1.64b0/agixt/provider/llamacpp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-05-22 00:58:37.000000 agixt-1.1.64b0/agixt/provider/oobabooga.py
--rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-05-22 00:58:37.000000 agixt-1.1.64b0/agixt/provider/openai.py
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-05-22 00:58:37.000000 agixt-1.1.64b0/agixt/provider/palm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2772 2023-05-22 00:58:37.000000 agixt-1.1.64b0/agixt/provider/transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)      881 2023-05-22 00:58:37.000000 agixt-1.1.64b0/agixt/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-22 00:58:37.000000 agixt-1.1.64b0/agixt/version
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 00:58:50.181376 agixt-1.1.64b0/agixt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13861 2023-05-22 00:58:50.000000 agixt-1.1.64b0/agixt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-05-22 00:58:50.000000 agixt-1.1.64b0/agixt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 00:58:50.000000 agixt-1.1.64b0/agixt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-05-22 00:58:50.000000 agixt-1.1.64b0/agixt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-22 00:58:50.000000 agixt-1.1.64b0/agixt.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 00:58:50.185376 agixt-1.1.64b0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)    13404 2023-05-22 00:58:37.000000 agixt-1.1.64b0/docs/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-22 00:58:37.000000 agixt-1.1.64b0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 00:58:50.185376 agixt-1.1.64b0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-05-22 00:58:37.000000 agixt-1.1.64b0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 01:44:49.345782 agixt-1.1.65b0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-05-22 01:44:37.000000 agixt-1.1.65b0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-22 01:44:37.000000 agixt-1.1.65b0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    13677 2023-05-22 01:44:49.345782 agixt-1.1.65b0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 01:44:49.345782 agixt-1.1.65b0/agixt/
+-rw-r--r--   0 runner    (1001) docker     (123)    15962 2023-05-22 01:44:37.000000 agixt-1.1.65b0/agixt/AGiXT.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12848 2023-05-22 01:44:37.000000 agixt-1.1.65b0/agixt/Agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6997 2023-05-22 01:44:37.000000 agixt-1.1.65b0/agixt/Chain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6153 2023-05-22 01:44:37.000000 agixt-1.1.65b0/agixt/Commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)      960 2023-05-22 01:44:37.000000 agixt-1.1.65b0/agixt/Config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-05-22 01:44:37.000000 agixt-1.1.65b0/agixt/CustomPrompt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6337 2023-05-22 01:44:37.000000 agixt-1.1.65b0/agixt/Embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-05-22 01:44:37.000000 agixt-1.1.65b0/agixt/Main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8367 2023-05-22 01:44:37.000000 agixt-1.1.65b0/agixt/Memories.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8476 2023-05-22 01:44:37.000000 agixt-1.1.65b0/agixt/Tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-05-22 01:44:37.000000 agixt-1.1.65b0/agixt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12961 2023-05-22 01:44:37.000000 agixt-1.1.65b0/agixt/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 01:44:49.345782 agixt-1.1.65b0/agixt/provider/
+-rw-r--r--   0 runner    (1001) docker     (123)     2157 2023-05-22 01:44:37.000000 agixt-1.1.65b0/agixt/provider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-05-22 01:44:37.000000 agixt-1.1.65b0/agixt/provider/azure.py
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-05-22 01:44:37.000000 agixt-1.1.65b0/agixt/provider/bard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-05-22 01:44:37.000000 agixt-1.1.65b0/agixt/provider/bing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-05-22 01:44:37.000000 agixt-1.1.65b0/agixt/provider/chatgpt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-05-22 01:44:37.000000 agixt-1.1.65b0/agixt/provider/claude.py
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-05-22 01:44:37.000000 agixt-1.1.65b0/agixt/provider/fastchat.py
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-05-22 01:44:37.000000 agixt-1.1.65b0/agixt/provider/gpt4all.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-05-22 01:44:37.000000 agixt-1.1.65b0/agixt/provider/gpt4free.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-22 01:44:37.000000 agixt-1.1.65b0/agixt/provider/gpugpt4all.py
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-05-22 01:44:37.000000 agixt-1.1.65b0/agixt/provider/huggingchat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-05-22 01:44:37.000000 agixt-1.1.65b0/agixt/provider/kobold.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-05-22 01:44:37.000000 agixt-1.1.65b0/agixt/provider/llamacpp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-05-22 01:44:37.000000 agixt-1.1.65b0/agixt/provider/oobabooga.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-05-22 01:44:37.000000 agixt-1.1.65b0/agixt/provider/openai.py
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-05-22 01:44:37.000000 agixt-1.1.65b0/agixt/provider/palm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2772 2023-05-22 01:44:37.000000 agixt-1.1.65b0/agixt/provider/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      881 2023-05-22 01:44:37.000000 agixt-1.1.65b0/agixt/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-22 01:44:37.000000 agixt-1.1.65b0/agixt/version
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 01:44:49.345782 agixt-1.1.65b0/agixt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13677 2023-05-22 01:44:49.000000 agixt-1.1.65b0/agixt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-05-22 01:44:49.000000 agixt-1.1.65b0/agixt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 01:44:49.000000 agixt-1.1.65b0/agixt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-05-22 01:44:49.000000 agixt-1.1.65b0/agixt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-22 01:44:49.000000 agixt-1.1.65b0/agixt.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 01:44:49.345782 agixt-1.1.65b0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)    13220 2023-05-22 01:44:37.000000 agixt-1.1.65b0/docs/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-22 01:44:37.000000 agixt-1.1.65b0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 01:44:49.345782 agixt-1.1.65b0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-05-22 01:44:37.000000 agixt-1.1.65b0/setup.py
```

### Comparing `agixt-1.1.64b0/LICENSE` & `agixt-1.1.65b0/LICENSE`

 * *Files identical despite different names*

### Comparing `agixt-1.1.64b0/PKG-INFO` & `agixt-1.1.65b0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agixt
-Version: 1.1.64b0
+Version: 1.1.65b0
 Summary: An Artificial Intelligence Automation Platform. AI Instruction management from various providers, has an adaptive memory, and a versatile plugin system with many commands including web browsing. Supports many AI providers and models and growing support every day.
 Author: Josh XT
 Author-email: josh@devxt.com
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -71,17 +71,17 @@
 - **Audio-to-Text & Text-to-Speech Options**: Integration with Hugging Face for seamless audio-to-text transcription, and multiple TTS choices, featuring Brian TTS, Mac OS TTS, and ElevenLabs.
 - **Platform Interoperability & AI Agent Management**: Streamlined creation, renaming, deletion, and updating of AI agent settings along with easy interaction with popular platforms like Twitter, GitHub, Google, DALL-E, and more.
 - **Custom Prompts & Command Control**: Granular control over agent abilities through enabling or disabling specific commands, and easy creation, editing, and deletion of custom prompts to standardize user inputs.
 - **RESTful API**: FastAPI-powered RESTful API for seamless integration with external applications and services.
 - **Expanding AI Support**: Continually updated to include new AI providers and services, ensuring the software stays at the forefront of AI technology.
 
 ## Quickstart with Docker
-Download the `docker-compose` file and run the AGiXT Streamlit Web App.
+Clone the repository and run the AGiXT Streamlit Web App.
 ```
-wget https://raw.githubusercontent.com/Josh-XT/AGiXT/main/docker/docker-compose.yml
+git clone https://github.com/Josh-XT/AGiXT
 docker compose --profile streamlit up
 ```
 
 - Web Interface http://localhost:8501
 ### Windows Docker Desktop (streamlit only example)
 - Container Name: AGiXT
 - Host Port: 8501:8501/tcp
@@ -91,16 +91,15 @@
 Run all available services, this includes the FastAPI back end (Port 7437) and NextJS front end (Port 3000).
 ```
 docker compose --profile all up
 ```
 
 ### Development using docker
 ```
-wget https://raw.githubusercontent.com/Josh-XT/AGiXT/main/docker/docker-compose.yml
-wget https://raw.githubusercontent.com/Josh-XT/AGiXT/main/docker/docker-compose.dev.yml
+git clone https://github.com/Josh-XT/AGiXT
 docker compose --profile all -f docker-compose.yml -f docker-compose.dev.yaml up
 ```
 
 ## Local Development
 
 Clone the repository for the AGiXT back end and start it.
```

### Comparing `agixt-1.1.64b0/agixt/AGiXT.py` & `agixt-1.1.65b0/agixt/AGiXT.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.64b0/agixt/Agent.py` & `agixt-1.1.65b0/agixt/Agent.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.64b0/agixt/Chain.py` & `agixt-1.1.65b0/agixt/Chain.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.64b0/agixt/Commands.py` & `agixt-1.1.65b0/agixt/Commands.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.64b0/agixt/Config.py` & `agixt-1.1.65b0/agixt/Config.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.64b0/agixt/CustomPrompt.py` & `agixt-1.1.65b0/agixt/CustomPrompt.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.64b0/agixt/Embedding.py` & `agixt-1.1.65b0/agixt/Embedding.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.64b0/agixt/Main.py` & `agixt-1.1.65b0/agixt/Main.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.64b0/agixt/Memories.py` & `agixt-1.1.65b0/agixt/Memories.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.64b0/agixt/Tasks.py` & `agixt-1.1.65b0/agixt/Tasks.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.64b0/agixt/app.py` & `agixt-1.1.65b0/agixt/app.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.64b0/agixt/provider/__init__.py` & `agixt-1.1.65b0/agixt/provider/__init__.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.64b0/agixt/provider/azure.py` & `agixt-1.1.65b0/agixt/provider/azure.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.64b0/agixt/provider/bing.py` & `agixt-1.1.65b0/agixt/provider/bing.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.64b0/agixt/provider/chatgpt.py` & `agixt-1.1.65b0/agixt/provider/chatgpt.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.64b0/agixt/provider/claude.py` & `agixt-1.1.65b0/agixt/provider/claude.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.64b0/agixt/provider/fastchat.py` & `agixt-1.1.65b0/agixt/provider/fastchat.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.64b0/agixt/provider/gpt4all.py` & `agixt-1.1.65b0/agixt/provider/gpt4all.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.64b0/agixt/provider/gpt4free.py` & `agixt-1.1.65b0/agixt/provider/gpt4free.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.64b0/agixt/provider/gpugpt4all.py` & `agixt-1.1.65b0/agixt/provider/gpugpt4all.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.64b0/agixt/provider/huggingchat.py` & `agixt-1.1.65b0/agixt/provider/huggingchat.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.64b0/agixt/provider/kobold.py` & `agixt-1.1.65b0/agixt/provider/kobold.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.64b0/agixt/provider/llamacpp.py` & `agixt-1.1.65b0/agixt/provider/llamacpp.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.64b0/agixt/provider/oobabooga.py` & `agixt-1.1.65b0/agixt/provider/oobabooga.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.64b0/agixt/provider/openai.py` & `agixt-1.1.65b0/agixt/provider/openai.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.64b0/agixt/provider/palm.py` & `agixt-1.1.65b0/agixt/provider/palm.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.64b0/agixt/provider/transformer.py` & `agixt-1.1.65b0/agixt/provider/transformer.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.64b0/agixt/requirements.txt` & `agixt-1.1.65b0/agixt/requirements.txt`

 * *Files identical despite different names*

### Comparing `agixt-1.1.64b0/agixt.egg-info/PKG-INFO` & `agixt-1.1.65b0/agixt.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agixt
-Version: 1.1.64b0
+Version: 1.1.65b0
 Summary: An Artificial Intelligence Automation Platform. AI Instruction management from various providers, has an adaptive memory, and a versatile plugin system with many commands including web browsing. Supports many AI providers and models and growing support every day.
 Author: Josh XT
 Author-email: josh@devxt.com
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -71,17 +71,17 @@
 - **Audio-to-Text & Text-to-Speech Options**: Integration with Hugging Face for seamless audio-to-text transcription, and multiple TTS choices, featuring Brian TTS, Mac OS TTS, and ElevenLabs.
 - **Platform Interoperability & AI Agent Management**: Streamlined creation, renaming, deletion, and updating of AI agent settings along with easy interaction with popular platforms like Twitter, GitHub, Google, DALL-E, and more.
 - **Custom Prompts & Command Control**: Granular control over agent abilities through enabling or disabling specific commands, and easy creation, editing, and deletion of custom prompts to standardize user inputs.
 - **RESTful API**: FastAPI-powered RESTful API for seamless integration with external applications and services.
 - **Expanding AI Support**: Continually updated to include new AI providers and services, ensuring the software stays at the forefront of AI technology.
 
 ## Quickstart with Docker
-Download the `docker-compose` file and run the AGiXT Streamlit Web App.
+Clone the repository and run the AGiXT Streamlit Web App.
 ```
-wget https://raw.githubusercontent.com/Josh-XT/AGiXT/main/docker/docker-compose.yml
+git clone https://github.com/Josh-XT/AGiXT
 docker compose --profile streamlit up
 ```
 
 - Web Interface http://localhost:8501
 ### Windows Docker Desktop (streamlit only example)
 - Container Name: AGiXT
 - Host Port: 8501:8501/tcp
@@ -91,16 +91,15 @@
 Run all available services, this includes the FastAPI back end (Port 7437) and NextJS front end (Port 3000).
 ```
 docker compose --profile all up
 ```
 
 ### Development using docker
 ```
-wget https://raw.githubusercontent.com/Josh-XT/AGiXT/main/docker/docker-compose.yml
-wget https://raw.githubusercontent.com/Josh-XT/AGiXT/main/docker/docker-compose.dev.yml
+git clone https://github.com/Josh-XT/AGiXT
 docker compose --profile all -f docker-compose.yml -f docker-compose.dev.yaml up
 ```
 
 ## Local Development
 
 Clone the repository for the AGiXT back end and start it.
```

### Comparing `agixt-1.1.64b0/agixt.egg-info/SOURCES.txt` & `agixt-1.1.65b0/agixt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `agixt-1.1.64b0/agixt.egg-info/requires.txt` & `agixt-1.1.65b0/agixt.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `agixt-1.1.64b0/docs/README.md` & `agixt-1.1.65b0/docs/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -61,17 +61,17 @@
 - **Audio-to-Text & Text-to-Speech Options**: Integration with Hugging Face for seamless audio-to-text transcription, and multiple TTS choices, featuring Brian TTS, Mac OS TTS, and ElevenLabs.
 - **Platform Interoperability & AI Agent Management**: Streamlined creation, renaming, deletion, and updating of AI agent settings along with easy interaction with popular platforms like Twitter, GitHub, Google, DALL-E, and more.
 - **Custom Prompts & Command Control**: Granular control over agent abilities through enabling or disabling specific commands, and easy creation, editing, and deletion of custom prompts to standardize user inputs.
 - **RESTful API**: FastAPI-powered RESTful API for seamless integration with external applications and services.
 - **Expanding AI Support**: Continually updated to include new AI providers and services, ensuring the software stays at the forefront of AI technology.
 
 ## Quickstart with Docker
-Download the `docker-compose` file and run the AGiXT Streamlit Web App.
+Clone the repository and run the AGiXT Streamlit Web App.
 ```
-wget https://raw.githubusercontent.com/Josh-XT/AGiXT/main/docker/docker-compose.yml
+git clone https://github.com/Josh-XT/AGiXT
 docker compose --profile streamlit up
 ```
 
 - Web Interface http://localhost:8501
 ### Windows Docker Desktop (streamlit only example)
 - Container Name: AGiXT
 - Host Port: 8501:8501/tcp
@@ -81,16 +81,15 @@
 Run all available services, this includes the FastAPI back end (Port 7437) and NextJS front end (Port 3000).
 ```
 docker compose --profile all up
 ```
 
 ### Development using docker
 ```
-wget https://raw.githubusercontent.com/Josh-XT/AGiXT/main/docker/docker-compose.yml
-wget https://raw.githubusercontent.com/Josh-XT/AGiXT/main/docker/docker-compose.dev.yml
+git clone https://github.com/Josh-XT/AGiXT
 docker compose --profile all -f docker-compose.yml -f docker-compose.dev.yaml up
 ```
 
 ## Local Development
 
 Clone the repository for the AGiXT back end and start it.
```

### Comparing `agixt-1.1.64b0/setup.py` & `agixt-1.1.65b0/setup.py`

 * *Files identical despite different names*

