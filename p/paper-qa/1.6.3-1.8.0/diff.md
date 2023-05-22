# Comparing `tmp/paper-qa-1.6.3.tar.gz` & `tmp/paper-qa-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "paper-qa-1.6.3.tar", last modified: Sat May 20 06:41:14 2023, max compression
+gzip compressed data, was "paper-qa-1.8.0.tar", last modified: Mon May 22 16:09:54 2023, max compression
```

## Comparing `paper-qa-1.6.3.tar` & `paper-qa-1.8.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 06:41:14.458464 paper-qa-1.6.3/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-20 06:40:38.000000 paper-qa-1.6.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    12585 2023-05-20 06:41:14.458464 paper-qa-1.6.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12150 2023-05-20 06:40:38.000000 paper-qa-1.6.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 06:41:14.454464 paper-qa-1.6.3/paper_qa.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12585 2023-05-20 06:41:14.000000 paper-qa-1.6.3/paper_qa.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-05-20 06:41:14.000000 paper-qa-1.6.3/paper_qa.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 06:41:14.000000 paper-qa-1.6.3/paper_qa.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-20 06:41:14.000000 paper-qa-1.6.3/paper_qa.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-20 06:41:14.000000 paper-qa-1.6.3/paper_qa.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 06:41:14.454464 paper-qa-1.6.3/paperqa/
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-20 06:40:38.000000 paper-qa-1.6.3/paperqa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5820 2023-05-20 06:40:38.000000 paper-qa-1.6.3/paperqa/agent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 06:41:14.454464 paper-qa-1.6.3/paperqa/contrib/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-20 06:40:38.000000 paper-qa-1.6.3/paperqa/contrib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11743 2023-05-20 06:40:38.000000 paper-qa-1.6.3/paperqa/contrib/zotero.py
--rw-r--r--   0 runner    (1001) docker     (123)    20314 2023-05-20 06:40:38.000000 paper-qa-1.6.3/paperqa/docs.py
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-20 06:40:38.000000 paper-qa-1.6.3/paperqa/paths.py
--rw-r--r--   0 runner    (1001) docker     (123)     4130 2023-05-20 06:40:38.000000 paper-qa-1.6.3/paperqa/qaprompts.py
--rw-r--r--   0 runner    (1001) docker     (123)     6773 2023-05-20 06:40:38.000000 paper-qa-1.6.3/paperqa/readers.py
--rw-r--r--   0 runner    (1001) docker     (123)      992 2023-05-20 06:40:38.000000 paper-qa-1.6.3/paperqa/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-05-20 06:40:38.000000 paper-qa-1.6.3/paperqa/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-20 06:40:38.000000 paper-qa-1.6.3/paperqa/version.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-20 06:41:14.458464 paper-qa-1.6.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      957 2023-05-20 06:40:38.000000 paper-qa-1.6.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 06:41:14.454464 paper-qa-1.6.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    12935 2023-05-20 06:40:38.000000 paper-qa-1.6.3/tests/test_paperqa.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:09:54.293750 paper-qa-1.8.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-22 16:09:10.000000 paper-qa-1.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12585 2023-05-22 16:09:54.293750 paper-qa-1.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12150 2023-05-22 16:09:10.000000 paper-qa-1.8.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:09:54.293750 paper-qa-1.8.0/paper_qa.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12585 2023-05-22 16:09:54.000000 paper-qa-1.8.0/paper_qa.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-05-22 16:09:54.000000 paper-qa-1.8.0/paper_qa.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 16:09:54.000000 paper-qa-1.8.0/paper_qa.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-22 16:09:54.000000 paper-qa-1.8.0/paper_qa.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-22 16:09:54.000000 paper-qa-1.8.0/paper_qa.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:09:54.293750 paper-qa-1.8.0/paperqa/
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-22 16:09:10.000000 paper-qa-1.8.0/paperqa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5855 2023-05-22 16:09:10.000000 paper-qa-1.8.0/paperqa/agent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:09:54.293750 paper-qa-1.8.0/paperqa/contrib/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-22 16:09:10.000000 paper-qa-1.8.0/paperqa/contrib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11743 2023-05-22 16:09:10.000000 paper-qa-1.8.0/paperqa/contrib/zotero.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20314 2023-05-22 16:09:10.000000 paper-qa-1.8.0/paperqa/docs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-22 16:09:10.000000 paper-qa-1.8.0/paperqa/paths.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4184 2023-05-22 16:09:10.000000 paper-qa-1.8.0/paperqa/qaprompts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6773 2023-05-22 16:09:10.000000 paper-qa-1.8.0/paperqa/readers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      992 2023-05-22 16:09:10.000000 paper-qa-1.8.0/paperqa/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-05-22 16:09:10.000000 paper-qa-1.8.0/paperqa/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-22 16:09:10.000000 paper-qa-1.8.0/paperqa/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 16:09:54.293750 paper-qa-1.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-05-22 16:09:10.000000 paper-qa-1.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:09:54.293750 paper-qa-1.8.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    12936 2023-05-22 16:09:10.000000 paper-qa-1.8.0/tests/test_paperqa.py
```

### Comparing `paper-qa-1.6.3/LICENSE` & `paper-qa-1.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `paper-qa-1.6.3/PKG-INFO` & `paper-qa-1.8.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paper-qa
-Version: 1.6.3
+Version: 1.8.0
 Summary: LLM Chain for answering questions from docs 
 Home-page: https://github.com/whitead/paper-qa
 Author: Andrew White
 Author-email: white.d.andrew@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `paper-qa-1.6.3/README.md` & `paper-qa-1.8.0/README.md`

 * *Files identical despite different names*

### Comparing `paper-qa-1.6.3/paper_qa.egg-info/PKG-INFO` & `paper-qa-1.8.0/paper_qa.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paper-qa
-Version: 1.6.3
+Version: 1.8.0
 Summary: LLM Chain for answering questions from docs 
 Home-page: https://github.com/whitead/paper-qa
 Author: Andrew White
 Author-email: white.d.andrew@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `paper-qa-1.6.3/paperqa/agent.py` & `paper-qa-1.8.0/paperqa/agent.py`

 * *Files 1% similar despite different names*

```diff
@@ -78,14 +78,15 @@
 
 
 class AnswerTool(BaseTool):
     name = "Propose Answer"
     description = "Ask a researcher to propose an answer using evidence from papers. The input is the question to be answered."
     docs: Docs = None
     answer: Answer = None
+    return_direct = True
 
     def __init__(self, docs, answer):
         # call the parent class constructor
         super(AnswerTool, self).__init__()
 
         self.docs = docs
         self.answer = answer
@@ -125,15 +126,15 @@
             import paperscraper
         except ImportError:
             raise ImportError(
                 "Please install paperscraper (github.com/blackadad/paper-scraper) to use agent"
             )
 
         papers = paperscraper.search_papers(
-            query, limit=20, verbose=False, pdir=self.docs.index_path
+            query, limit=5, _limit=20, verbose=False, pdir=self.docs.index_path
         )
         for path, data in papers.items():
             try:
                 self.docs.add(path, citation=data["citation"])
             except:
                 pass
         return status(self.answer, self.docs)
```

### Comparing `paper-qa-1.6.3/paperqa/contrib/zotero.py` & `paper-qa-1.8.0/paperqa/contrib/zotero.py`

 * *Files identical despite different names*

### Comparing `paper-qa-1.6.3/paperqa/docs.py` & `paper-qa-1.8.0/paperqa/docs.py`

 * *Files identical despite different names*

### Comparing `paper-qa-1.6.3/paperqa/qaprompts.py` & `paper-qa-1.8.0/paperqa/qaprompts.py`

 * *Files 4% similar despite different names*

```diff
@@ -44,14 +44,15 @@
 
 
 search_prompt = prompts.PromptTemplate(
     input_variables=["question"],
     template="We want to answer the following question: {question} \n"
     "Provide three keyword searches (one search per line) "
     "that will find papers to help answer the question. Do not use boolean operators. "
+    "Provide some broad and some specific searches. "
     "Recent years are 2021, 2022, 2023.\n\n"
     "1.",
 )
 
 
 select_paper_prompt = prompts.PromptTemplate(
     input_variables=["instructions", "papers"],
```

### Comparing `paper-qa-1.6.3/paperqa/readers.py` & `paper-qa-1.8.0/paperqa/readers.py`

 * *Files identical despite different names*

### Comparing `paper-qa-1.6.3/paperqa/types.py` & `paper-qa-1.8.0/paperqa/types.py`

 * *Files identical despite different names*

### Comparing `paper-qa-1.6.3/paperqa/utils.py` & `paper-qa-1.8.0/paperqa/utils.py`

 * *Files identical despite different names*

### Comparing `paper-qa-1.6.3/setup.py` & `paper-qa-1.8.0/setup.py`

 * *Files identical despite different names*

### Comparing `paper-qa-1.6.3/tests/test_paperqa.py` & `paper-qa-1.8.0/tests/test_paperqa.py`

 * *Files 0% similar despite different names*

```diff
@@ -68,15 +68,15 @@
         docs.add(doc_path, "WikiMedia Foundation, 2023, Accessed tomorrow")
         os.remove(doc_path)
         answer = await docs.aquery(
             "What is Frederick Bates's greatest accomplishment?",
             get_callbacks=lambda x: [TestHandler()],
         )
         assert answer.tokens > 100
-        assert answer.cost > 0.01
+        assert answer.cost > 0.001
 
 
 def test_evidence():
     doc_path = "example.txt"
     with open(doc_path, "w", encoding="utf-8") as f:
         # get wiki page about politician
         r = requests.get("https://en.wikipedia.org/wiki/Frederick_Bates_(politician)")
```

