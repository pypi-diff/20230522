# Comparing `tmp/easyinstruct-0.0.4.tar.gz` & `tmp/easyinstruct-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easyinstruct-0.0.4.tar", last modified: Mon May 15 15:44:50 2023, max compression
+gzip compressed data, was "easyinstruct-0.0.5.tar", last modified: Mon May 22 16:24:02 2023, max compression
```

## Comparing `easyinstruct-0.0.4.tar` & `easyinstruct-0.0.5.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 maoshengyu   (501) staff       (20)        0 2023-05-15 15:44:50.419206 easyinstruct-0.0.4/
--rw-r--r--   0 maoshengyu   (501) staff       (20)     1063 2023-05-15 15:24:51.000000 easyinstruct-0.0.4/LICENSE
--rw-r--r--   0 maoshengyu   (501) staff       (20)    13323 2023-05-15 15:44:50.419006 easyinstruct-0.0.4/PKG-INFO
--rw-r--r--   0 maoshengyu   (501) staff       (20)    12662 2023-05-15 15:24:51.000000 easyinstruct-0.0.4/README.md
-drwxr-xr-x   0 maoshengyu   (501) staff       (20)        0 2023-05-15 15:44:50.415398 easyinstruct-0.0.4/easyinstruct/
--rw-r--r--   0 maoshengyu   (501) staff       (20)       67 2023-05-15 15:25:40.000000 easyinstruct-0.0.4/easyinstruct/__init__.py
-drwxr-xr-x   0 maoshengyu   (501) staff       (20)        0 2023-05-15 15:44:50.416733 easyinstruct-0.0.4/easyinstruct/engines/
--rw-r--r--   0 maoshengyu   (501) staff       (20)       74 2023-05-15 15:24:51.000000 easyinstruct-0.0.4/easyinstruct/engines/__init__.py
--rw-r--r--   0 maoshengyu   (501) staff       (20)      446 2023-05-15 15:24:51.000000 easyinstruct-0.0.4/easyinstruct/engines/base_engine.py
--rw-r--r--   0 maoshengyu   (501) staff       (20)     4075 2023-05-15 15:24:51.000000 easyinstruct-0.0.4/easyinstruct/engines/llama_engine.py
-drwxr-xr-x   0 maoshengyu   (501) staff       (20)        0 2023-05-15 15:44:50.418081 easyinstruct-0.0.4/easyinstruct/prompts/
--rw-r--r--   0 maoshengyu   (501) staff       (20)      269 2023-05-15 15:24:51.000000 easyinstruct-0.0.4/easyinstruct/prompts/__init__.py
--rw-r--r--   0 maoshengyu   (501) staff       (20)     4572 2023-05-15 15:24:51.000000 easyinstruct-0.0.4/easyinstruct/prompts/base_prompt.py
--rw-r--r--   0 maoshengyu   (501) staff       (20)     2732 2023-05-15 15:24:51.000000 easyinstruct-0.0.4/easyinstruct/prompts/batch_prompt.py
--rw-r--r--   0 maoshengyu   (501) staff       (20)      493 2023-05-15 15:24:51.000000 easyinstruct-0.0.4/easyinstruct/prompts/cot_prompt.py
--rw-r--r--   0 maoshengyu   (501) staff       (20)     1007 2023-05-15 15:24:51.000000 easyinstruct-0.0.4/easyinstruct/prompts/icl_prompt.py
--rw-r--r--   0 maoshengyu   (501) staff       (20)    18141 2023-05-15 15:24:51.000000 easyinstruct-0.0.4/easyinstruct/prompts/ie_prompt.py
--rw-r--r--   0 maoshengyu   (501) staff       (20)     3592 2023-05-15 15:24:51.000000 easyinstruct-0.0.4/easyinstruct/prompts/index_prompt.py
--rw-r--r--   0 maoshengyu   (501) staff       (20)     4815 2023-05-15 15:24:51.000000 easyinstruct-0.0.4/easyinstruct/prompts/mm_prompt.py
-drwxr-xr-x   0 maoshengyu   (501) staff       (20)        0 2023-05-15 15:44:50.418762 easyinstruct-0.0.4/easyinstruct/utils/
--rw-r--r--   0 maoshengyu   (501) staff       (20)       58 2023-05-15 15:44:37.000000 easyinstruct-0.0.4/easyinstruct/utils/__init__.py
--rw-r--r--   0 maoshengyu   (501) staff       (20)      726 2023-05-15 15:24:51.000000 easyinstruct-0.0.4/easyinstruct/utils/api.py
--rw-r--r--   0 maoshengyu   (501) staff       (20)      913 2023-05-15 15:24:51.000000 easyinstruct-0.0.4/easyinstruct/utils/file.py
--rw-r--r--   0 maoshengyu   (501) staff       (20)     1700 2023-05-15 15:24:51.000000 easyinstruct-0.0.4/easyinstruct/utils/log.py
-drwxr-xr-x   0 maoshengyu   (501) staff       (20)        0 2023-05-15 15:44:50.416050 easyinstruct-0.0.4/easyinstruct.egg-info/
--rw-r--r--   0 maoshengyu   (501) staff       (20)    13323 2023-05-15 15:44:50.000000 easyinstruct-0.0.4/easyinstruct.egg-info/PKG-INFO
--rw-r--r--   0 maoshengyu   (501) staff       (20)      727 2023-05-15 15:44:50.000000 easyinstruct-0.0.4/easyinstruct.egg-info/SOURCES.txt
--rw-r--r--   0 maoshengyu   (501) staff       (20)        1 2023-05-15 15:44:50.000000 easyinstruct-0.0.4/easyinstruct.egg-info/dependency_links.txt
--rw-r--r--   0 maoshengyu   (501) staff       (20)      176 2023-05-15 15:44:50.000000 easyinstruct-0.0.4/easyinstruct.egg-info/requires.txt
--rw-r--r--   0 maoshengyu   (501) staff       (20)       13 2023-05-15 15:44:50.000000 easyinstruct-0.0.4/easyinstruct.egg-info/top_level.txt
--rw-r--r--   0 maoshengyu   (501) staff       (20)       38 2023-05-15 15:44:50.419254 easyinstruct-0.0.4/setup.cfg
--rw-r--r--   0 maoshengyu   (501) staff       (20)     1564 2023-05-15 15:27:48.000000 easyinstruct-0.0.4/setup.py
+drwxrwxr-x   0 oeheart   (1020) oeheart   (1020)        0 2023-05-22 16:24:02.407927 easyinstruct-0.0.5/
+-rw-rw-r--   0 oeheart   (1020) oeheart   (1020)     1063 2023-05-02 08:36:56.000000 easyinstruct-0.0.5/LICENSE
+-rw-rw-r--   0 oeheart   (1020) oeheart   (1020)    14313 2023-05-22 16:24:02.407927 easyinstruct-0.0.5/PKG-INFO
+-rw-rw-r--   0 oeheart   (1020) oeheart   (1020)    13652 2023-05-22 16:16:58.000000 easyinstruct-0.0.5/README.md
+drwxrwxr-x   0 oeheart   (1020) oeheart   (1020)        0 2023-05-22 16:24:02.403926 easyinstruct-0.0.5/easyinstruct/
+-rw-rw-r--   0 oeheart   (1020) oeheart   (1020)       67 2023-05-22 16:11:58.000000 easyinstruct-0.0.5/easyinstruct/__init__.py
+drwxrwxr-x   0 oeheart   (1020) oeheart   (1020)        0 2023-05-22 16:24:02.407927 easyinstruct-0.0.5/easyinstruct/engines/
+-rw-rw-r--   0 oeheart   (1020) oeheart   (1020)       74 2023-05-02 08:36:56.000000 easyinstruct-0.0.5/easyinstruct/engines/__init__.py
+-rw-rw-r--   0 oeheart   (1020) oeheart   (1020)      446 2023-05-02 08:52:57.000000 easyinstruct-0.0.5/easyinstruct/engines/base_engine.py
+-rw-rw-r--   0 oeheart   (1020) oeheart   (1020)     3231 2023-05-22 16:11:58.000000 easyinstruct-0.0.5/easyinstruct/engines/llama_engine.py
+drwxrwxr-x   0 oeheart   (1020) oeheart   (1020)        0 2023-05-22 16:24:02.407927 easyinstruct-0.0.5/easyinstruct/prompts/
+-rw-rw-r--   0 oeheart   (1020) oeheart   (1020)      269 2023-05-02 08:36:56.000000 easyinstruct-0.0.5/easyinstruct/prompts/__init__.py
+-rw-rw-r--   0 oeheart   (1020) oeheart   (1020)     4572 2023-05-04 05:06:08.000000 easyinstruct-0.0.5/easyinstruct/prompts/base_prompt.py
+-rw-rw-r--   0 oeheart   (1020) oeheart   (1020)     2732 2023-05-02 09:01:03.000000 easyinstruct-0.0.5/easyinstruct/prompts/batch_prompt.py
+-rw-rw-r--   0 oeheart   (1020) oeheart   (1020)      493 2023-05-02 08:36:56.000000 easyinstruct-0.0.5/easyinstruct/prompts/cot_prompt.py
+-rw-rw-r--   0 oeheart   (1020) oeheart   (1020)     1007 2023-05-02 08:36:56.000000 easyinstruct-0.0.5/easyinstruct/prompts/icl_prompt.py
+-rw-rw-r--   0 oeheart   (1020) oeheart   (1020)    18141 2023-05-02 08:36:56.000000 easyinstruct-0.0.5/easyinstruct/prompts/ie_prompt.py
+-rw-rw-r--   0 oeheart   (1020) oeheart   (1020)     3592 2023-05-02 08:36:56.000000 easyinstruct-0.0.5/easyinstruct/prompts/index_prompt.py
+-rw-rw-r--   0 oeheart   (1020) oeheart   (1020)     4815 2023-05-02 08:36:56.000000 easyinstruct-0.0.5/easyinstruct/prompts/mm_prompt.py
+drwxrwxr-x   0 oeheart   (1020) oeheart   (1020)        0 2023-05-22 16:24:02.407927 easyinstruct-0.0.5/easyinstruct/utils/
+-rw-rw-r--   0 oeheart   (1020) oeheart   (1020)       58 2023-05-22 16:11:58.000000 easyinstruct-0.0.5/easyinstruct/utils/__init__.py
+-rw-rw-r--   0 oeheart   (1020) oeheart   (1020)      726 2023-05-02 08:36:56.000000 easyinstruct-0.0.5/easyinstruct/utils/api.py
+-rw-rw-r--   0 oeheart   (1020) oeheart   (1020)      913 2023-05-02 08:36:56.000000 easyinstruct-0.0.5/easyinstruct/utils/file.py
+-rw-rw-r--   0 oeheart   (1020) oeheart   (1020)     1700 2023-05-02 08:36:56.000000 easyinstruct-0.0.5/easyinstruct/utils/log.py
+drwxrwxr-x   0 oeheart   (1020) oeheart   (1020)        0 2023-05-22 16:24:02.403926 easyinstruct-0.0.5/easyinstruct.egg-info/
+-rw-rw-r--   0 oeheart   (1020) oeheart   (1020)    14313 2023-05-22 16:24:02.000000 easyinstruct-0.0.5/easyinstruct.egg-info/PKG-INFO
+-rw-rw-r--   0 oeheart   (1020) oeheart   (1020)      727 2023-05-22 16:24:02.000000 easyinstruct-0.0.5/easyinstruct.egg-info/SOURCES.txt
+-rw-rw-r--   0 oeheart   (1020) oeheart   (1020)        1 2023-05-22 16:24:02.000000 easyinstruct-0.0.5/easyinstruct.egg-info/dependency_links.txt
+-rw-rw-r--   0 oeheart   (1020) oeheart   (1020)      151 2023-05-22 16:24:02.000000 easyinstruct-0.0.5/easyinstruct.egg-info/requires.txt
+-rw-rw-r--   0 oeheart   (1020) oeheart   (1020)       13 2023-05-22 16:24:02.000000 easyinstruct-0.0.5/easyinstruct.egg-info/top_level.txt
+-rw-rw-r--   0 oeheart   (1020) oeheart   (1020)       38 2023-05-22 16:24:02.407927 easyinstruct-0.0.5/setup.cfg
+-rw-rw-r--   0 oeheart   (1020) oeheart   (1020)     1539 2023-05-22 16:12:51.000000 easyinstruct-0.0.5/setup.py
```

### Comparing `easyinstruct-0.0.4/LICENSE` & `easyinstruct-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `easyinstruct-0.0.4/PKG-INFO` & `easyinstruct-0.0.5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easyinstruct
-Version: 0.0.4
+Version: 0.0.5
 Summary: A easy-to-use framework to instruct large language models.
 Home-page: https://github.com/zjunlp/EasyInstruct
 Author: Yixin Ou
 Keywords: AI,NLP,instruction,language model
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -29,24 +29,26 @@
   <a href="#installation">Installation</a> •
   <a href="#use-easyinstruct">How To Use</a> •
   <a href="https://zjunlp.gitbook.io/easyinstruct/">Docs</a> •
   <a href="#citation">Citation</a> •
   <a href="#contributors">Contributors</a>
 </p>
 
-![](https://img.shields.io/badge/version-v0.0.3-blue)
+![](https://img.shields.io/badge/version-v0.0.5-blue)
 [![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](https://opensource.org/licenses/MIT)
 ![](https://img.shields.io/github/last-commit/zjunlp/EasyInstruct?color=green) 
 ![](https://img.shields.io/badge/PRs-Welcome-red) 
 
 </div>
 
 
 ## 🔔News
 
+- **2023-5-23 We release version 0.0.5, removing requirement of llama-cpp-python.**
+- **2023-5-16 We release version 0.0.4, fixing some problems.**
 - **2023-4-21 We release version 0.0.3. Check out our [documentations](https://zjunlp.gitbook.io/easyinstruct/documentations) for more details!**
 - **2023-3-25 We release version 0.0.2, suporting IndexPrompt, MMPrompt, IEPrompt and more LLMs**
 - **2023-3-13 We release version 0.0.1, supporting in-context learning, chain-of-thought with ChatGPT.**
 
 ---
 
 
@@ -56,15 +58,15 @@
 
 ---
 
 ## 🔧Installation
 
 **Installation using PyPI:**
 ```
-pip install easyinstruct==0.0.3 -i https://pypi.org/simple
+pip install easyinstruct==0.0.5 -i https://pypi.org/simple
 ```
 
 **Installation for local development:**
 ```
 git clone https://github.com/zjunlp/EasyInstruct
 cd EasyInstruct
 pip install -e .
@@ -364,16 +366,37 @@
 # Step5: Get the result from LLM API service
 batch_prompt.get_openai_result(engine = "gpt-3.5-turbo")
 
 # Step6: Parse the response
 batch_prompt.parse_response()
 ```
 
----
+### llamaEngine
+> `llamaEngine` is the class for local Llama models. It's an alternative to the openAI engine which supports local deployment.It support both hf mode and llama.cpp mode.
+
+**Example**
+```python
+from easyinstruct import llamaEngine
+from transformers import GenerationConfig
+# Step1: Initialize according to the your model path and the weight format
+# Load the model in hf format
+lengine=llamaEngine(base_path=YOUR_BASE_PATH,adapter_path=YOUR_ADAPTER_PATH,gpu=True,multi_gpu=True) 
+# Load the model in cpp format
+# lengine=llamaEngine(base_path=YOUR_BASE_PATH,gpu=False)
+
+# Step2: do inference
+generation_config = GenerationConfig(
+                    temperature=0.6,
+                    top_p=0.95,
+                    repetition_penalty=1.15,
+                )
+print(lengine('介绍一下浙江大学',generation_config))
+```
 
+---
 ### 🚩Citation
 
 Please cite our repository if you use EasyInstruct in your work.
 
 ```
 @misc{easyinstruct,
   author = {Yixin Ou and Shengyu Mao and Lei Li and Ziwen Xu and Xiaolong Weng and Shuofei Qiao and Yuqi Zhu and Yinuo Jiang and Zhen Bi and Jing Chen and Huajun Chen and Ningyu Zhang},
```

#### html2text {}

```diff
@@ -1,32 +1,34 @@
-Metadata-Version: 2.1 Name: easyinstruct Version: 0.0.4 Summary: A easy-to-use
+Metadata-Version: 2.1 Name: easyinstruct Version: 0.0.5 Summary: A easy-to-use
 framework to instruct large language models. Home-page: https://github.com/
 zjunlp/EasyInstruct Author: Yixin Ou Keywords: AI,NLP,instruction,language
 model Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Intended
 Audience :: Developers Classifier: Intended Audience :: Education Classifier:
 Intended Audience :: Science/Research Requires-Python: >=3.7.0 Description-
 Content-Type: text/markdown License-File: LICENSE
  [figs/EasyInstruct.png] **An Easy-to-use Framework to Instruct Large Language
                                  Models.** ---
 Overview â¢ Installation â¢ How_To_Use â¢ Docs â¢ Citation â¢ Contributors
-![](https://img.shields.io/badge/version-v0.0.3-blue) [![License: MIT](https://
+![](https://img.shields.io/badge/version-v0.0.5-blue) [![License: MIT](https://
  img.shields.io/badge/License-MIT-green.svg)](https://opensource.org/licenses/
           MIT) ![](https://img.shields.io/github/last-commit/zjunlp/
   EasyInstruct?color=green) ![](https://img.shields.io/badge/PRs-Welcome-red)
-## ðNews - **2023-4-21 We release version 0.0.3. Check out our
+## ðNews - **2023-5-23 We release version 0.0.5, removing requirement of
+llama-cpp-python.** - **2023-5-16 We release version 0.0.4, fixing some
+problems.** - **2023-4-21 We release version 0.0.3. Check out our
 [documentations](https://zjunlp.gitbook.io/easyinstruct/documentations) for
 more details!** - **2023-3-25 We release version 0.0.2, suporting IndexPrompt,
 MMPrompt, IEPrompt and more LLMs** - **2023-3-13 We release version 0.0.1,
 supporting in-context learning, chain-of-thought with ChatGPT.** --- ##
 ðOverview EasyInstruct is a Python package for instructing Large Language
 Models(LLM) like GPT-3 in your research experiments. It is designed to be easy
 to use and easy to extend. --- ## ð§Installation **Installation using PyPI:**
-``` pip install easyinstruct==0.0.3 -i https://pypi.org/simple ```
+``` pip install easyinstruct==0.0.5 -i https://pypi.org/simple ```
 **Installation for local development:** ``` git clone https://github.com/
 zjunlp/EasyInstruct cd EasyInstruct pip install -e . ``` --- ## ðUse
 EasyInstruct Please refer to our [documentations](https://zjunlp.gitbook.io/
 easyinstruct/documentations) for more details. ### BasePrompt > `BasePrompt` is
 the base class for all prompts.Currently we support building prompts to
 instruct LLM by calling LLM API service of OpenAI (GPT-3, ChatGPT) and
 Anthropic (Claude). We will support more available LLM products such as Llama
@@ -151,16 +153,26 @@
 zeroshot_prompts.build_prompt(question) fewshot_prompts = FewshotCoTPrompt()
 fewshot_prompts.build_prompt(question, in_context_examples =
 in_context_examples, n_shots = 1) # Step3: Declare a batch prompt class
 batch_prompt = BatchPrompt() # Step4: Build all prompts in a batch
 batch_prompt.build_prompt([prompts, ieprompts, zeroshot_prompts,
 fewshot_prompts]) # Step5: Get the result from LLM API service
 batch_prompt.get_openai_result(engine = "gpt-3.5-turbo") # Step6: Parse the
-response batch_prompt.parse_response() ``` --- ### ð©Citation Please cite our
-repository if you use EasyInstruct in your work. ``` @misc{easyinstruct, author
-= {Yixin Ou and Shengyu Mao and Lei Li and Ziwen Xu and Xiaolong Weng and
-Shuofei Qiao and Yuqi Zhu and Yinuo Jiang and Zhen Bi and Jing Chen and Huajun
-Chen and Ningyu Zhang}, title = {EasyInstruct: An Easy-to-use Framework to
-Instruct Large Language Models}, year = {2023}, publisher = {GitHub}, journal =
-{GitHub repository}, howpublished = {\url{https://github.com/zjunlp/
-EasyInstruct}}, } ``` --- ## ðContributors [https://contrib.rocks/
-image?repo=zjunlp/EasyInstruct]
+response batch_prompt.parse_response() ``` ### llamaEngine > `llamaEngine` is
+the class for local Llama models. It's an alternative to the openAI engine
+which supports local deployment.It support both hf mode and llama.cpp mode.
+**Example** ```python from easyinstruct import llamaEngine from transformers
+import GenerationConfig # Step1: Initialize according to the your model path
+and the weight format # Load the model in hf format lengine=llamaEngine
+(base_path=YOUR_BASE_PATH,adapter_path=YOUR_ADAPTER_PATH,gpu=True,multi_gpu=True)
+# Load the model in cpp format # lengine=llamaEngine
+(base_path=YOUR_BASE_PATH,gpu=False) # Step2: do inference generation_config =
+GenerationConfig( temperature=0.6, top_p=0.95, repetition_penalty=1.15, ) print
+(lengine('ä»ç»ä¸ä¸æµæ±å¤§å­¦',generation_config)) ``` --- ###
+ð©Citation Please cite our repository if you use EasyInstruct in your work.
+``` @misc{easyinstruct, author = {Yixin Ou and Shengyu Mao and Lei Li and Ziwen
+Xu and Xiaolong Weng and Shuofei Qiao and Yuqi Zhu and Yinuo Jiang and Zhen Bi
+and Jing Chen and Huajun Chen and Ningyu Zhang}, title = {EasyInstruct: An
+Easy-to-use Framework to Instruct Large Language Models}, year = {2023},
+publisher = {GitHub}, journal = {GitHub repository}, howpublished = {\url
+{https://github.com/zjunlp/EasyInstruct}}, } ``` --- ## ðContributors
+[https://contrib.rocks/image?repo=zjunlp/EasyInstruct]
```

### Comparing `easyinstruct-0.0.4/README.md` & `easyinstruct-0.0.5/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -11,24 +11,26 @@
   <a href="#installation">Installation</a> •
   <a href="#use-easyinstruct">How To Use</a> •
   <a href="https://zjunlp.gitbook.io/easyinstruct/">Docs</a> •
   <a href="#citation">Citation</a> •
   <a href="#contributors">Contributors</a>
 </p>
 
-![](https://img.shields.io/badge/version-v0.0.3-blue)
+![](https://img.shields.io/badge/version-v0.0.5-blue)
 [![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](https://opensource.org/licenses/MIT)
 ![](https://img.shields.io/github/last-commit/zjunlp/EasyInstruct?color=green) 
 ![](https://img.shields.io/badge/PRs-Welcome-red) 
 
 </div>
 
 
 ## 🔔News
 
+- **2023-5-23 We release version 0.0.5, removing requirement of llama-cpp-python.**
+- **2023-5-16 We release version 0.0.4, fixing some problems.**
 - **2023-4-21 We release version 0.0.3. Check out our [documentations](https://zjunlp.gitbook.io/easyinstruct/documentations) for more details!**
 - **2023-3-25 We release version 0.0.2, suporting IndexPrompt, MMPrompt, IEPrompt and more LLMs**
 - **2023-3-13 We release version 0.0.1, supporting in-context learning, chain-of-thought with ChatGPT.**
 
 ---
 
 
@@ -38,15 +40,15 @@
 
 ---
 
 ## 🔧Installation
 
 **Installation using PyPI:**
 ```
-pip install easyinstruct==0.0.3 -i https://pypi.org/simple
+pip install easyinstruct==0.0.5 -i https://pypi.org/simple
 ```
 
 **Installation for local development:**
 ```
 git clone https://github.com/zjunlp/EasyInstruct
 cd EasyInstruct
 pip install -e .
@@ -346,16 +348,37 @@
 # Step5: Get the result from LLM API service
 batch_prompt.get_openai_result(engine = "gpt-3.5-turbo")
 
 # Step6: Parse the response
 batch_prompt.parse_response()
 ```
 
----
+### llamaEngine
+> `llamaEngine` is the class for local Llama models. It's an alternative to the openAI engine which supports local deployment.It support both hf mode and llama.cpp mode.
+
+**Example**
+```python
+from easyinstruct import llamaEngine
+from transformers import GenerationConfig
+# Step1: Initialize according to the your model path and the weight format
+# Load the model in hf format
+lengine=llamaEngine(base_path=YOUR_BASE_PATH,adapter_path=YOUR_ADAPTER_PATH,gpu=True,multi_gpu=True) 
+# Load the model in cpp format
+# lengine=llamaEngine(base_path=YOUR_BASE_PATH,gpu=False)
+
+# Step2: do inference
+generation_config = GenerationConfig(
+                    temperature=0.6,
+                    top_p=0.95,
+                    repetition_penalty=1.15,
+                )
+print(lengine('介绍一下浙江大学',generation_config))
+```
 
+---
 ### 🚩Citation
 
 Please cite our repository if you use EasyInstruct in your work.
 
 ```
 @misc{easyinstruct,
   author = {Yixin Ou and Shengyu Mao and Lei Li and Ziwen Xu and Xiaolong Weng and Shuofei Qiao and Yuqi Zhu and Yinuo Jiang and Zhen Bi and Jing Chen and Huajun Chen and Ningyu Zhang},
```

### Comparing `easyinstruct-0.0.4/easyinstruct/engines/llama_engine.py` & `easyinstruct-0.0.5/easyinstruct/engines/llama_engine.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,79 +1,51 @@
 import torch
 from transformers import LlamaTokenizer, LlamaForCausalLM, GenerationConfig
 from peft import PeftModel, get_peft_model, set_peft_model_state_dict, LoraConfig
-from llama_cpp import Llama
 from typing import Optional
+from transformers import GenerationConfig
 
-from .base_engine import BaseEngine
-
-
-class llamaEngine(BaseEngine):
-    r"""
-        llama Engine wrapper according to choosing use gpu or not
-    """
-
-    def __init__(self,base_path:str,gpu:bool=True,adapter_path:Optional[str]=None,multi_gpu:Optional[bool]=False):
-        if gpu:
-            self.engine=llama_gpu_Engine(base_path=base_path,adapter_path=adapter_path,multi_gpu=multi_gpu)
-        else:
-            self.engine=llama_cpp_Engine(base_path=base_path)
-    def _call(self, prompt, stop=None,**kwargs):
-        return self.engine(prompt,stop=stop,**kwargs)
-
-
-class llama_gpu_Engine(BaseEngine):
+class llamaEngine():
     r"""
         llama Engine for inference.
         Example:
-        >>>lengine=llamaEngine(base_path=YOUR_BASE_PATH,adapter_path=YOUR_ADAPTER_PATH)
+        >>>lengine=llamaEngine(base_path=YOUR_BASE_PATH,device_map="auto",adapter_path=YOUR_ADAPTER_PATH)
         >>>print(lengine('介绍一下浙江大学'))
     """
-
-    def __init__(self,base_path:str,adapter_path:Optional[str]=None,multi_gpu:Optional[bool]=False):
+    def __init__(self,base_path:str,device_map:str,adapter_path:Optional[str]=None,):
         
         self.tokenizer = LlamaTokenizer.from_pretrained(base_path)
         self.tokenizer.pad_token_id = 0
         self.tokenizer.padding_side = "left"
         """init model"""
-        if not multi_gpu:
-            self.model = LlamaForCausalLM.from_pretrained(
-            base_path,
-            load_in_8bit=True,
-            device_map={'':'cuda:1'},
-            )
-            if adapter_path is not None:
-                """apply lora"""
-                config = LoraConfig(
-                    r=8,
-                    lora_alpha=16,
-                    target_modules=["q_proj", "v_proj"],
-                    lora_dropout=0.05,
-                    bias="none",
-                    task_type="CAUSAL_LM"
-                )
-                self.model = get_peft_model(self.model, config) 
-                adapters_weights = torch.load(adapter_path, map_location="cuda:1")
-                self.model = set_peft_model_state_dict(self.model, adapters_weights)
-        else:
-            """multi GPU enable float16"""
-            self.model = LlamaForCausalLM.from_pretrained(
-                base_path,
-                torch_dtype=torch.float16,
-                device_map="auto",
+        self.model = LlamaForCausalLM.from_pretrained(
+        base_path,
+        load_in_8bit=True,
+        device_map=device_map,
+        )
+        if adapter_path is not None:
+            """apply lora"""
+            # config = LoraConfig(
+            #     r=8,
+            #     lora_alpha=16,
+            #     target_modules=["q_proj", "v_proj"],
+            #     lora_dropout=0.05,
+            #     bias="none",
+            #     task_type="CAUSAL_LM"
+            # )
+            # self.model = get_peft_model(self.model, config) 
+            # adapters_weights = torch.load(adapter_path)
+            # self.model = set_peft_model_state_dict(self.model, adapters_weights)
+            self.model = PeftModel.from_pretrained(
+                self.model, 
+                adapter_path,
+                torch_dtype=torch.float16
             )
-            if adapter_path is not None:
-                """apply lora"""
-                self.model = PeftModel.from_pretrained(
-                    self.model, 
-                    adapter_path,
-                    torch_dtype=torch.float16
-                )
 
-    def _call(self, prompt, stop=None,**kwargs):
+    def __call__(self, prompt, stop=None,**kwargs):
         inputs = self.tokenizer(prompt, return_tensors="pt")
         input_ids = inputs["input_ids"].cuda()      
         #set default values
         temperature=kwargs.pop('temperature',0.6)
         top_p=kwargs.pop('top_p',0.95)
         repetition_penalty=kwargs.pop('repetition_penalty',1.15)
         max_new_tokens=kwargs.pop('max_new_tokens',256)
@@ -92,17 +64,20 @@
             )
         s = generation_output.sequences[0]
         output = self.tokenizer.decode(s,skip_special_tokens=True)
         del input_ids, generation_output,s
         torch.cuda.empty_cache()
         return output
 
-class llama_cpp_Engine(BaseEngine):
-    def __init__(self,base_path:str):
-        self.model= Llama(model_path=base_path)
-
-    def _call(self, prompt, stop=None,**kwargs):
-        if stop is None:
-            stop=["\n"]
-        max_tokens=kwargs.pop('max_new_tokens',256),
-        output=self.model(prompt,stop=stop,max_tokens=max_tokens)
-        return output
+if __name__ == "__main__":
+   
+    # Step1: Initialize according to the your model path and the weight format
+    # Load the model in hf format
+    lengine=llamaEngine(base_path='/mnt/ceph-user/jyn/model/llama_hf_7B',device_map="auto")
+
+    # Step2: do inference
+    generation_config = GenerationConfig(
+                        temperature=0.6,
+                        top_p=0.95,
+                        repetition_penalty=1.15,
+                    )
+    print(lengine('介绍一下浙江大学',generation_config))
```

### Comparing `easyinstruct-0.0.4/easyinstruct/prompts/base_prompt.py` & `easyinstruct-0.0.5/easyinstruct/prompts/base_prompt.py`

 * *Files identical despite different names*

### Comparing `easyinstruct-0.0.4/easyinstruct/prompts/batch_prompt.py` & `easyinstruct-0.0.5/easyinstruct/prompts/batch_prompt.py`

 * *Files identical despite different names*

### Comparing `easyinstruct-0.0.4/easyinstruct/prompts/icl_prompt.py` & `easyinstruct-0.0.5/easyinstruct/prompts/icl_prompt.py`

 * *Files identical despite different names*

### Comparing `easyinstruct-0.0.4/easyinstruct/prompts/ie_prompt.py` & `easyinstruct-0.0.5/easyinstruct/prompts/ie_prompt.py`

 * *Files identical despite different names*

### Comparing `easyinstruct-0.0.4/easyinstruct/prompts/index_prompt.py` & `easyinstruct-0.0.5/easyinstruct/prompts/index_prompt.py`

 * *Files identical despite different names*

### Comparing `easyinstruct-0.0.4/easyinstruct/prompts/mm_prompt.py` & `easyinstruct-0.0.5/easyinstruct/prompts/mm_prompt.py`

 * *Files identical despite different names*

### Comparing `easyinstruct-0.0.4/easyinstruct/utils/api.py` & `easyinstruct-0.0.5/easyinstruct/utils/api.py`

 * *Files identical despite different names*

### Comparing `easyinstruct-0.0.4/easyinstruct/utils/file.py` & `easyinstruct-0.0.5/easyinstruct/utils/file.py`

 * *Files identical despite different names*

### Comparing `easyinstruct-0.0.4/easyinstruct/utils/log.py` & `easyinstruct-0.0.5/easyinstruct/utils/log.py`

 * *Files identical despite different names*

### Comparing `easyinstruct-0.0.4/easyinstruct.egg-info/PKG-INFO` & `easyinstruct-0.0.5/easyinstruct.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easyinstruct
-Version: 0.0.4
+Version: 0.0.5
 Summary: A easy-to-use framework to instruct large language models.
 Home-page: https://github.com/zjunlp/EasyInstruct
 Author: Yixin Ou
 Keywords: AI,NLP,instruction,language model
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -29,24 +29,26 @@
   <a href="#installation">Installation</a> •
   <a href="#use-easyinstruct">How To Use</a> •
   <a href="https://zjunlp.gitbook.io/easyinstruct/">Docs</a> •
   <a href="#citation">Citation</a> •
   <a href="#contributors">Contributors</a>
 </p>
 
-![](https://img.shields.io/badge/version-v0.0.3-blue)
+![](https://img.shields.io/badge/version-v0.0.5-blue)
 [![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](https://opensource.org/licenses/MIT)
 ![](https://img.shields.io/github/last-commit/zjunlp/EasyInstruct?color=green) 
 ![](https://img.shields.io/badge/PRs-Welcome-red) 
 
 </div>
 
 
 ## 🔔News
 
+- **2023-5-23 We release version 0.0.5, removing requirement of llama-cpp-python.**
+- **2023-5-16 We release version 0.0.4, fixing some problems.**
 - **2023-4-21 We release version 0.0.3. Check out our [documentations](https://zjunlp.gitbook.io/easyinstruct/documentations) for more details!**
 - **2023-3-25 We release version 0.0.2, suporting IndexPrompt, MMPrompt, IEPrompt and more LLMs**
 - **2023-3-13 We release version 0.0.1, supporting in-context learning, chain-of-thought with ChatGPT.**
 
 ---
 
 
@@ -56,15 +58,15 @@
 
 ---
 
 ## 🔧Installation
 
 **Installation using PyPI:**
 ```
-pip install easyinstruct==0.0.3 -i https://pypi.org/simple
+pip install easyinstruct==0.0.5 -i https://pypi.org/simple
 ```
 
 **Installation for local development:**
 ```
 git clone https://github.com/zjunlp/EasyInstruct
 cd EasyInstruct
 pip install -e .
@@ -364,16 +366,37 @@
 # Step5: Get the result from LLM API service
 batch_prompt.get_openai_result(engine = "gpt-3.5-turbo")
 
 # Step6: Parse the response
 batch_prompt.parse_response()
 ```
 
----
+### llamaEngine
+> `llamaEngine` is the class for local Llama models. It's an alternative to the openAI engine which supports local deployment.It support both hf mode and llama.cpp mode.
+
+**Example**
+```python
+from easyinstruct import llamaEngine
+from transformers import GenerationConfig
+# Step1: Initialize according to the your model path and the weight format
+# Load the model in hf format
+lengine=llamaEngine(base_path=YOUR_BASE_PATH,adapter_path=YOUR_ADAPTER_PATH,gpu=True,multi_gpu=True) 
+# Load the model in cpp format
+# lengine=llamaEngine(base_path=YOUR_BASE_PATH,gpu=False)
+
+# Step2: do inference
+generation_config = GenerationConfig(
+                    temperature=0.6,
+                    top_p=0.95,
+                    repetition_penalty=1.15,
+                )
+print(lengine('介绍一下浙江大学',generation_config))
+```
 
+---
 ### 🚩Citation
 
 Please cite our repository if you use EasyInstruct in your work.
 
 ```
 @misc{easyinstruct,
   author = {Yixin Ou and Shengyu Mao and Lei Li and Ziwen Xu and Xiaolong Weng and Shuofei Qiao and Yuqi Zhu and Yinuo Jiang and Zhen Bi and Jing Chen and Huajun Chen and Ningyu Zhang},
```

#### html2text {}

```diff
@@ -1,32 +1,34 @@
-Metadata-Version: 2.1 Name: easyinstruct Version: 0.0.4 Summary: A easy-to-use
+Metadata-Version: 2.1 Name: easyinstruct Version: 0.0.5 Summary: A easy-to-use
 framework to instruct large language models. Home-page: https://github.com/
 zjunlp/EasyInstruct Author: Yixin Ou Keywords: AI,NLP,instruction,language
 model Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Intended
 Audience :: Developers Classifier: Intended Audience :: Education Classifier:
 Intended Audience :: Science/Research Requires-Python: >=3.7.0 Description-
 Content-Type: text/markdown License-File: LICENSE
  [figs/EasyInstruct.png] **An Easy-to-use Framework to Instruct Large Language
                                  Models.** ---
 Overview â¢ Installation â¢ How_To_Use â¢ Docs â¢ Citation â¢ Contributors
-![](https://img.shields.io/badge/version-v0.0.3-blue) [![License: MIT](https://
+![](https://img.shields.io/badge/version-v0.0.5-blue) [![License: MIT](https://
  img.shields.io/badge/License-MIT-green.svg)](https://opensource.org/licenses/
           MIT) ![](https://img.shields.io/github/last-commit/zjunlp/
   EasyInstruct?color=green) ![](https://img.shields.io/badge/PRs-Welcome-red)
-## ðNews - **2023-4-21 We release version 0.0.3. Check out our
+## ðNews - **2023-5-23 We release version 0.0.5, removing requirement of
+llama-cpp-python.** - **2023-5-16 We release version 0.0.4, fixing some
+problems.** - **2023-4-21 We release version 0.0.3. Check out our
 [documentations](https://zjunlp.gitbook.io/easyinstruct/documentations) for
 more details!** - **2023-3-25 We release version 0.0.2, suporting IndexPrompt,
 MMPrompt, IEPrompt and more LLMs** - **2023-3-13 We release version 0.0.1,
 supporting in-context learning, chain-of-thought with ChatGPT.** --- ##
 ðOverview EasyInstruct is a Python package for instructing Large Language
 Models(LLM) like GPT-3 in your research experiments. It is designed to be easy
 to use and easy to extend. --- ## ð§Installation **Installation using PyPI:**
-``` pip install easyinstruct==0.0.3 -i https://pypi.org/simple ```
+``` pip install easyinstruct==0.0.5 -i https://pypi.org/simple ```
 **Installation for local development:** ``` git clone https://github.com/
 zjunlp/EasyInstruct cd EasyInstruct pip install -e . ``` --- ## ðUse
 EasyInstruct Please refer to our [documentations](https://zjunlp.gitbook.io/
 easyinstruct/documentations) for more details. ### BasePrompt > `BasePrompt` is
 the base class for all prompts.Currently we support building prompts to
 instruct LLM by calling LLM API service of OpenAI (GPT-3, ChatGPT) and
 Anthropic (Claude). We will support more available LLM products such as Llama
@@ -151,16 +153,26 @@
 zeroshot_prompts.build_prompt(question) fewshot_prompts = FewshotCoTPrompt()
 fewshot_prompts.build_prompt(question, in_context_examples =
 in_context_examples, n_shots = 1) # Step3: Declare a batch prompt class
 batch_prompt = BatchPrompt() # Step4: Build all prompts in a batch
 batch_prompt.build_prompt([prompts, ieprompts, zeroshot_prompts,
 fewshot_prompts]) # Step5: Get the result from LLM API service
 batch_prompt.get_openai_result(engine = "gpt-3.5-turbo") # Step6: Parse the
-response batch_prompt.parse_response() ``` --- ### ð©Citation Please cite our
-repository if you use EasyInstruct in your work. ``` @misc{easyinstruct, author
-= {Yixin Ou and Shengyu Mao and Lei Li and Ziwen Xu and Xiaolong Weng and
-Shuofei Qiao and Yuqi Zhu and Yinuo Jiang and Zhen Bi and Jing Chen and Huajun
-Chen and Ningyu Zhang}, title = {EasyInstruct: An Easy-to-use Framework to
-Instruct Large Language Models}, year = {2023}, publisher = {GitHub}, journal =
-{GitHub repository}, howpublished = {\url{https://github.com/zjunlp/
-EasyInstruct}}, } ``` --- ## ðContributors [https://contrib.rocks/
-image?repo=zjunlp/EasyInstruct]
+response batch_prompt.parse_response() ``` ### llamaEngine > `llamaEngine` is
+the class for local Llama models. It's an alternative to the openAI engine
+which supports local deployment.It support both hf mode and llama.cpp mode.
+**Example** ```python from easyinstruct import llamaEngine from transformers
+import GenerationConfig # Step1: Initialize according to the your model path
+and the weight format # Load the model in hf format lengine=llamaEngine
+(base_path=YOUR_BASE_PATH,adapter_path=YOUR_ADAPTER_PATH,gpu=True,multi_gpu=True)
+# Load the model in cpp format # lengine=llamaEngine
+(base_path=YOUR_BASE_PATH,gpu=False) # Step2: do inference generation_config =
+GenerationConfig( temperature=0.6, top_p=0.95, repetition_penalty=1.15, ) print
+(lengine('ä»ç»ä¸ä¸æµæ±å¤§å­¦',generation_config)) ``` --- ###
+ð©Citation Please cite our repository if you use EasyInstruct in your work.
+``` @misc{easyinstruct, author = {Yixin Ou and Shengyu Mao and Lei Li and Ziwen
+Xu and Xiaolong Weng and Shuofei Qiao and Yuqi Zhu and Yinuo Jiang and Zhen Bi
+and Jing Chen and Huajun Chen and Ningyu Zhang}, title = {EasyInstruct: An
+Easy-to-use Framework to Instruct Large Language Models}, year = {2023},
+publisher = {GitHub}, journal = {GitHub repository}, howpublished = {\url
+{https://github.com/zjunlp/EasyInstruct}}, } ``` --- ## ðContributors
+[https://contrib.rocks/image?repo=zjunlp/EasyInstruct]
```

### Comparing `easyinstruct-0.0.4/easyinstruct.egg-info/SOURCES.txt` & `easyinstruct-0.0.5/easyinstruct.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `easyinstruct-0.0.4/setup.py` & `easyinstruct-0.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 REQUIRES = """
 torch>=1.13.0
 transformers>=4.28.0
 peft==0.2.0
 accelerate==0.17.1
 openai==0.27.0
 anthropic==0.2.7
-llama-cpp-python==0.1.41
 llama-index==0.4.29
 langchain==0.0.116
 tiktoken
 nltk
 """
 
 def get_install_requires():
@@ -24,15 +23,15 @@
 with open("README.md") as f:
     readme = f.read()
 
 
 def do_setup():
     setup(
         name="easyinstruct",
-        version = '0.0.4',
+        version = '0.0.5',
         description = "A easy-to-use framework to instruct large language models.",
         url="https://github.com/zjunlp/EasyInstruct",
         author = 'Yixin Ou',
         long_description=readme,
         long_description_content_type="text/markdown",
         install_requires=get_install_requires(),
         python_requires=">=3.7.0",
```

