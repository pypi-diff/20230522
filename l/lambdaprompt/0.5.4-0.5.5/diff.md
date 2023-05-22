# Comparing `tmp/lambdaprompt-0.5.4.tar.gz` & `tmp/lambdaprompt-0.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/lambdaprompt/lambdaprompt/dist/.tmp-502lzvwh/lambdaprompt-0.5.4.tar", last modified: Fri May 19 21:34:18 2023, max compression
+gzip compressed data, was "/home/runner/work/lambdaprompt/lambdaprompt/dist/.tmp-293fkjkl/lambdaprompt-0.5.5.tar", last modified: Mon May 22 19:43:12 2023, max compression
```

## Comparing `lambdaprompt-0.5.4.tar` & `lambdaprompt-0.5.5.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 21:34:18.000000 lambdaprompt-0.5.4/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 21:34:18.000000 lambdaprompt-0.5.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 21:34:18.000000 lambdaprompt-0.5.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-05-19 21:34:05.000000 lambdaprompt-0.5.4/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3132 2023-05-19 21:34:05.000000 lambdaprompt-0.5.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-19 21:34:05.000000 lambdaprompt-0.5.4/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-05-19 21:34:05.000000 lambdaprompt-0.5.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6088 2023-05-19 21:34:18.000000 lambdaprompt-0.5.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5614 2023-05-19 21:34:05.000000 lambdaprompt-0.5.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-19 21:34:05.000000 lambdaprompt-0.5.4/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 21:34:18.000000 lambdaprompt-0.5.4/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-05-19 21:34:05.000000 lambdaprompt-0.5.4/examples/one.py
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-05-19 21:34:05.000000 lambdaprompt-0.5.4/examples/two.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 21:34:18.000000 lambdaprompt-0.5.4/lambdaprompt/
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-05-19 21:34:05.000000 lambdaprompt-0.5.4/lambdaprompt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10958 2023-05-19 21:34:05.000000 lambdaprompt-0.5.4/lambdaprompt/backends.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 21:34:18.000000 lambdaprompt-0.5.4/lambdaprompt/examples/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 21:34:05.000000 lambdaprompt-0.5.4/lambdaprompt/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-05-19 21:34:05.000000 lambdaprompt-0.5.4/lambdaprompt/examples/server.py
--rw-r--r--   0 runner    (1001) docker     (123)      676 2023-05-19 21:34:05.000000 lambdaprompt-0.5.4/lambdaprompt/gpt3.py
--rw-r--r--   0 runner    (1001) docker     (123)     9570 2023-05-19 21:34:05.000000 lambdaprompt-0.5.4/lambdaprompt/prompt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 21:34:18.000000 lambdaprompt-0.5.4/lambdaprompt/server/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 21:34:05.000000 lambdaprompt-0.5.4/lambdaprompt/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-05-19 21:34:05.000000 lambdaprompt-0.5.4/lambdaprompt/server/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     5197 2023-05-19 21:34:05.000000 lambdaprompt-0.5.4/lambdaprompt/server/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 21:34:18.000000 lambdaprompt-0.5.4/lambdaprompt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6088 2023-05-19 21:34:18.000000 lambdaprompt-0.5.4/lambdaprompt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-05-19 21:34:18.000000 lambdaprompt-0.5.4/lambdaprompt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 21:34:18.000000 lambdaprompt-0.5.4/lambdaprompt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-19 21:34:18.000000 lambdaprompt-0.5.4/lambdaprompt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-19 21:34:18.000000 lambdaprompt-0.5.4/lambdaprompt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-05-19 21:34:05.000000 lambdaprompt-0.5.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 21:34:18.000000 lambdaprompt-0.5.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 21:34:05.000000 lambdaprompt-0.5.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 21:34:18.000000 lambdaprompt-0.5.4/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 21:34:18.000000 lambdaprompt-0.5.4/tests/library/
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-19 21:34:05.000000 lambdaprompt-0.5.4/tests/library/serverexamples.py
--rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-05-19 21:34:05.000000 lambdaprompt-0.5.4/tests/test_gpt3.py
--rw-r--r--   0 runner    (1001) docker     (123)     2947 2023-05-19 21:34:05.000000 lambdaprompt-0.5.4/tests/test_prompt.py
--rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-05-19 21:34:05.000000 lambdaprompt-0.5.4/tests/test_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:43:12.000000 lambdaprompt-0.5.5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:43:12.000000 lambdaprompt-0.5.5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:43:12.000000 lambdaprompt-0.5.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-05-22 19:42:58.000000 lambdaprompt-0.5.5/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3132 2023-05-22 19:42:58.000000 lambdaprompt-0.5.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-22 19:42:58.000000 lambdaprompt-0.5.5/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-05-22 19:42:58.000000 lambdaprompt-0.5.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6088 2023-05-22 19:43:12.000000 lambdaprompt-0.5.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5614 2023-05-22 19:42:58.000000 lambdaprompt-0.5.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-22 19:42:58.000000 lambdaprompt-0.5.5/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:43:12.000000 lambdaprompt-0.5.5/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-05-22 19:42:58.000000 lambdaprompt-0.5.5/examples/one.py
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-05-22 19:42:58.000000 lambdaprompt-0.5.5/examples/two.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:43:12.000000 lambdaprompt-0.5.5/lambdaprompt/
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-05-22 19:42:58.000000 lambdaprompt-0.5.5/lambdaprompt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11213 2023-05-22 19:42:58.000000 lambdaprompt-0.5.5/lambdaprompt/backends.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:43:12.000000 lambdaprompt-0.5.5/lambdaprompt/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 19:42:58.000000 lambdaprompt-0.5.5/lambdaprompt/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-05-22 19:42:58.000000 lambdaprompt-0.5.5/lambdaprompt/examples/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-05-22 19:42:58.000000 lambdaprompt-0.5.5/lambdaprompt/gpt3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9570 2023-05-22 19:42:58.000000 lambdaprompt-0.5.5/lambdaprompt/prompt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:43:12.000000 lambdaprompt-0.5.5/lambdaprompt/server/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 19:42:58.000000 lambdaprompt-0.5.5/lambdaprompt/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-05-22 19:42:58.000000 lambdaprompt-0.5.5/lambdaprompt/server/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5197 2023-05-22 19:42:58.000000 lambdaprompt-0.5.5/lambdaprompt/server/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:43:12.000000 lambdaprompt-0.5.5/lambdaprompt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6088 2023-05-22 19:43:12.000000 lambdaprompt-0.5.5/lambdaprompt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-05-22 19:43:12.000000 lambdaprompt-0.5.5/lambdaprompt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 19:43:12.000000 lambdaprompt-0.5.5/lambdaprompt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-22 19:43:12.000000 lambdaprompt-0.5.5/lambdaprompt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-22 19:43:12.000000 lambdaprompt-0.5.5/lambdaprompt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-05-22 19:42:58.000000 lambdaprompt-0.5.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 19:43:12.000000 lambdaprompt-0.5.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 19:42:58.000000 lambdaprompt-0.5.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:43:12.000000 lambdaprompt-0.5.5/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:43:12.000000 lambdaprompt-0.5.5/tests/library/
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-22 19:42:58.000000 lambdaprompt-0.5.5/tests/library/serverexamples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-05-22 19:42:58.000000 lambdaprompt-0.5.5/tests/test_gpt3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2947 2023-05-22 19:42:58.000000 lambdaprompt-0.5.5/tests/test_prompt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-05-22 19:42:58.000000 lambdaprompt-0.5.5/tests/test_server.py
```

### Comparing `lambdaprompt-0.5.4/.github/workflows/publish-to-pypi.yml` & `lambdaprompt-0.5.5/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `lambdaprompt-0.5.4/.gitignore` & `lambdaprompt-0.5.5/.gitignore`

 * *Files identical despite different names*

### Comparing `lambdaprompt-0.5.4/LICENSE` & `lambdaprompt-0.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `lambdaprompt-0.5.4/PKG-INFO` & `lambdaprompt-0.5.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lambdaprompt
-Version: 0.5.4
+Version: 0.5.5
 Summary: A functional programming interface for building AI systems
 License: MIT
 Project-URL: homepage, https://github.com/approximatelabs/lambdaprompt
 Keywords: nlp,ai,functional,composition,prompt,apply,chain,machine
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `lambdaprompt-0.5.4/README.md` & `lambdaprompt-0.5.5/README.md`

 * *Files identical despite different names*

### Comparing `lambdaprompt-0.5.4/lambdaprompt/__init__.py` & `lambdaprompt-0.5.5/lambdaprompt/__init__.py`

 * *Files identical despite different names*

### Comparing `lambdaprompt-0.5.4/lambdaprompt/backends.py` & `lambdaprompt-0.5.5/lambdaprompt/backends.py`

 * *Files 6% similar despite different names*

```diff
@@ -215,36 +215,40 @@
         use_cache: bool = True
         do_sample: bool = True
         top_p: float = 0.92
         top_k: int = 0
         repetition_penalty: float = 1.1
         stop: Optional[Union[str, List[str]]]
 
-    def __init__(self, model_name, torch_dtype=None, trust_remote_code=True, use_auth_token=None, **param_override):
+    def __init__(self, model_name, torch_dtype=None, trust_remote_code=True, use_auth_token=None, use_device_map=True, load_config=True, **param_override):
         import torch
         from transformers import AutoConfig, AutoModelForCausalLM, AutoTokenizer
         torch_dtype = torch_dtype or torch.bfloat16
         super().__init__(**param_override)
-        config = AutoConfig.from_pretrained(
-            model_name,
-            trust_remote_code=True
-        )
+        init_kwargs = {
+            "torch_dtype": torch_dtype,
+            "trust_remote_code": trust_remote_code,
+            "use_auth_token": use_auth_token,
+        }
+        if load_config:
+            init_kwargs['config'] = AutoConfig.from_pretrained(
+                model_name,
+                trust_remote_code=True
+            )
+        if use_device_map:
+            init_kwargs['device_map'] = "auto"
         self.model = AutoModelForCausalLM.from_pretrained(
             model_name,
-            torch_dtype=torch_dtype,
-            trust_remote_code=trust_remote_code,
-            use_auth_token=use_auth_token,
-            config=config,
-            device_map="auto"
+            **init_kwargs
         )
         tokenizer = AutoTokenizer.from_pretrained(
             model_name,
             trust_remote_code=trust_remote_code,
             use_auth_token=use_auth_token,
-            device_map="auto"
+            **({"device_map":"auto"} if use_device_map else {})
         )
         if tokenizer.pad_token_id is None:
             tokenizer.pad_token = tokenizer.eos_token
         tokenizer.padding_side = "left"
         self.tokenizer = tokenizer
         self.model.eval()
 
@@ -286,16 +290,16 @@
                 new_tokens = new_tokens[:-end_id.shape[0]]
         output_text = self.tokenizer.decode(new_tokens, skip_special_tokens=True)
         return output_text
 
 
 class MPT7BInstructCompletion(HuggingFaceBackend):
     def __init__(self, **kwargs):
-        super().__init__("mosaicml/mpt-7b-instruct", **kwargs)
+        super().__init__("mosaicml/mpt-7b-instruct", use_device_map=False, **kwargs)
 
 
 class StarCoderCompletion(HuggingFaceBackend):
     def __init__(self, hf_access_token=None, **kwargs):
         hf_access_token = hf_access_token or os.environ.get("HF_ACCESS_TOKEN")
         if not hf_access_token:
             raise Exception("No HuggingFace access token found (envvar HF_ACCESS_TOKEN))")
-        super().__init__("bigcode/starcoder", use_auth_token=hf_access_token, **kwargs)
+        super().__init__("bigcode/starcoder", use_auth_token=hf_access_token, load_config=False, **kwargs)
```

### Comparing `lambdaprompt-0.5.4/lambdaprompt/gpt3.py` & `lambdaprompt-0.5.5/lambdaprompt/gpt3.py`

 * *Files identical despite different names*

### Comparing `lambdaprompt-0.5.4/lambdaprompt/prompt.py` & `lambdaprompt-0.5.5/lambdaprompt/prompt.py`

 * *Files identical despite different names*

### Comparing `lambdaprompt-0.5.4/lambdaprompt/server/data.py` & `lambdaprompt-0.5.5/lambdaprompt/server/data.py`

 * *Files identical despite different names*

### Comparing `lambdaprompt-0.5.4/lambdaprompt/server/main.py` & `lambdaprompt-0.5.5/lambdaprompt/server/main.py`

 * *Files identical despite different names*

### Comparing `lambdaprompt-0.5.4/lambdaprompt.egg-info/PKG-INFO` & `lambdaprompt-0.5.5/lambdaprompt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lambdaprompt
-Version: 0.5.4
+Version: 0.5.5
 Summary: A functional programming interface for building AI systems
 License: MIT
 Project-URL: homepage, https://github.com/approximatelabs/lambdaprompt
 Keywords: nlp,ai,functional,composition,prompt,apply,chain,machine
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `lambdaprompt-0.5.4/lambdaprompt.egg-info/SOURCES.txt` & `lambdaprompt-0.5.5/lambdaprompt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lambdaprompt-0.5.4/pyproject.toml` & `lambdaprompt-0.5.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `lambdaprompt-0.5.4/tests/test_gpt3.py` & `lambdaprompt-0.5.5/tests/test_gpt3.py`

 * *Files identical despite different names*

### Comparing `lambdaprompt-0.5.4/tests/test_prompt.py` & `lambdaprompt-0.5.5/tests/test_prompt.py`

 * *Files identical despite different names*

### Comparing `lambdaprompt-0.5.4/tests/test_server.py` & `lambdaprompt-0.5.5/tests/test_server.py`

 * *Files identical despite different names*

