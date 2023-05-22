# Comparing `tmp/embedbase-1.1.9.tar.gz` & `tmp/embedbase-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "embedbase-1.1.9.tar", max compression
+gzip compressed data, was "embedbase-1.2.0.tar", max compression
```

## Comparing `embedbase-1.1.9.tar` & `embedbase-1.2.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     1069 2023-05-20 09:06:52.366709 embedbase-1.1.9/LICENSE
--rw-r--r--   0        0        0     4905 2023-05-20 09:06:52.366709 embedbase-1.1.9/README.md
--rw-r--r--   0        0        0      121 2023-05-20 09:06:52.498710 embedbase-1.1.9/embedbase/__init__.py
--rw-r--r--   0        0        0     1716 2023-05-20 09:06:52.498710 embedbase-1.1.9/embedbase/__main__.py
--rw-r--r--   0        0        0      976 2023-05-20 09:06:52.498710 embedbase-1.1.9/embedbase/api.py
--rw-r--r--   0        0        0    17884 2023-05-20 09:06:52.498710 embedbase-1.1.9/embedbase/app.py
--rw-r--r--   0        0        0       88 2023-05-20 09:06:52.498710 embedbase-1.1.9/embedbase/database/__init__.py
--rw-r--r--   0        0        0     3406 2023-05-20 09:06:52.498710 embedbase-1.1.9/embedbase/database/base.py
--rw-r--r--   0        0        0     6220 2023-05-20 09:06:52.498710 embedbase-1.1.9/embedbase/database/memory_db.py
--rw-r--r--   0        0        0    10191 2023-05-20 09:06:52.498710 embedbase-1.1.9/embedbase/database/postgres_db.py
--rw-r--r--   0        0        0     7585 2023-05-20 09:06:52.498710 embedbase-1.1.9/embedbase/database/supabase_db.py
--rw-r--r--   0        0        0       77 2023-05-20 09:06:52.498710 embedbase-1.1.9/embedbase/embedding/__init__.py
--rw-r--r--   0        0        0      858 2023-05-20 09:06:52.502710 embedbase-1.1.9/embedbase/embedding/base.py
--rw-r--r--   0        0        0     1237 2023-05-20 09:06:52.502710 embedbase-1.1.9/embedbase/embedding/cohere.py
--rw-r--r--   0        0        0     2059 2023-05-20 09:06:52.502710 embedbase-1.1.9/embedbase/embedding/openai.py
--rw-r--r--   0        0        0     1551 2023-05-20 09:06:52.502710 embedbase-1.1.9/embedbase/firebase_auth.py
--rw-r--r--   0        0        0      690 2023-05-20 09:06:52.502710 embedbase-1.1.9/embedbase/logging_utils.py
--rw-r--r--   0        0        0      955 2023-05-20 09:06:52.502710 embedbase-1.1.9/embedbase/models.py
--rw-r--r--   0        0        0     1285 2023-05-20 09:06:52.502710 embedbase-1.1.9/embedbase/settings.py
--rw-r--r--   0        0        0     3208 2023-05-20 09:06:52.502710 embedbase-1.1.9/embedbase/strings.py
--rw-r--r--   0        0        0      301 2023-05-20 09:06:52.502710 embedbase-1.1.9/embedbase/supabase_auth.py
--rw-r--r--   0        0        0     3867 2023-05-20 09:06:52.502710 embedbase-1.1.9/embedbase/utils.py
--rw-r--r--   0        0        0     3666 2023-05-20 09:06:52.502710 embedbase-1.1.9/pyproject.toml
--rw-r--r--   0        0        0     6138 1970-01-01 00:00:00.000000 embedbase-1.1.9/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-05-22 12:12:22.291315 embedbase-1.2.0/LICENSE
+-rw-r--r--   0        0        0     4905 2023-05-22 12:12:22.291315 embedbase-1.2.0/README.md
+-rw-r--r--   0        0        0      121 2023-05-22 12:12:22.423314 embedbase-1.2.0/embedbase/__init__.py
+-rw-r--r--   0        0        0     1716 2023-05-22 12:12:22.423314 embedbase-1.2.0/embedbase/__main__.py
+-rw-r--r--   0        0        0      976 2023-05-22 12:12:22.423314 embedbase-1.2.0/embedbase/api.py
+-rw-r--r--   0        0        0    17884 2023-05-22 12:12:22.423314 embedbase-1.2.0/embedbase/app.py
+-rw-r--r--   0        0        0       88 2023-05-22 12:12:22.423314 embedbase-1.2.0/embedbase/database/__init__.py
+-rw-r--r--   0        0        0     3406 2023-05-22 12:12:22.423314 embedbase-1.2.0/embedbase/database/base.py
+-rw-r--r--   0        0        0     6220 2023-05-22 12:12:22.423314 embedbase-1.2.0/embedbase/database/memory_db.py
+-rw-r--r--   0        0        0    10191 2023-05-22 12:12:22.423314 embedbase-1.2.0/embedbase/database/postgres_db.py
+-rw-r--r--   0        0        0     7571 2023-05-22 12:12:22.423314 embedbase-1.2.0/embedbase/database/supabase_db.py
+-rw-r--r--   0        0        0       77 2023-05-22 12:12:22.423314 embedbase-1.2.0/embedbase/embedding/__init__.py
+-rw-r--r--   0        0        0      858 2023-05-22 12:12:22.423314 embedbase-1.2.0/embedbase/embedding/base.py
+-rw-r--r--   0        0        0     1237 2023-05-22 12:12:22.423314 embedbase-1.2.0/embedbase/embedding/cohere.py
+-rw-r--r--   0        0        0     2059 2023-05-22 12:12:22.423314 embedbase-1.2.0/embedbase/embedding/openai.py
+-rw-r--r--   0        0        0     1551 2023-05-22 12:12:22.423314 embedbase-1.2.0/embedbase/firebase_auth.py
+-rw-r--r--   0        0        0      690 2023-05-22 12:12:22.423314 embedbase-1.2.0/embedbase/logging_utils.py
+-rw-r--r--   0        0        0      955 2023-05-22 12:12:22.423314 embedbase-1.2.0/embedbase/models.py
+-rw-r--r--   0        0        0     1285 2023-05-22 12:12:22.423314 embedbase-1.2.0/embedbase/settings.py
+-rw-r--r--   0        0        0     3208 2023-05-22 12:12:22.423314 embedbase-1.2.0/embedbase/strings.py
+-rw-r--r--   0        0        0      301 2023-05-22 12:12:22.423314 embedbase-1.2.0/embedbase/supabase_auth.py
+-rw-r--r--   0        0        0     3867 2023-05-22 12:12:22.423314 embedbase-1.2.0/embedbase/utils.py
+-rw-r--r--   0        0        0     3730 2023-05-22 12:12:22.427314 embedbase-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     6337 1970-01-01 00:00:00.000000 embedbase-1.2.0/PKG-INFO
```

### Comparing `embedbase-1.1.9/LICENSE` & `embedbase-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `embedbase-1.1.9/README.md` & `embedbase-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `embedbase-1.1.9/embedbase/__main__.py` & `embedbase-1.2.0/embedbase/__main__.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.1.9/embedbase/api.py` & `embedbase-1.2.0/embedbase/api.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.1.9/embedbase/app.py` & `embedbase-1.2.0/embedbase/app.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.1.9/embedbase/database/base.py` & `embedbase-1.2.0/embedbase/database/base.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.1.9/embedbase/database/memory_db.py` & `embedbase-1.2.0/embedbase/database/memory_db.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.1.9/embedbase/database/postgres_db.py` & `embedbase-1.2.0/embedbase/database/postgres_db.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.1.9/embedbase/database/supabase_db.py` & `embedbase-1.2.0/embedbase/database/supabase_db.py`

 * *Files 0% similar despite different names*

```diff
@@ -209,15 +209,15 @@
         user_id: Optional[str] = None,
         offset: int = 0,
         limit: int = 100,
     ) -> List[Document]:
         req = self.supabase.table("documents").select("*").eq("dataset_id", dataset_id)
         if user_id:
             req = req.eq("user_id", user_id)
-        req = req.range(offset * limit, (offset + 1) * limit)
+        req = req.range(offset, offset + limit)
         data = req.execute().data
         return [
             Document(
                 id=row["id"],
                 data=row["data"],
                 embedding=ast.literal_eval(row["embedding"]),
                 hash=row["hash"],
```

### Comparing `embedbase-1.1.9/embedbase/embedding/base.py` & `embedbase-1.2.0/embedbase/embedding/base.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.1.9/embedbase/embedding/cohere.py` & `embedbase-1.2.0/embedbase/embedding/cohere.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.1.9/embedbase/embedding/openai.py` & `embedbase-1.2.0/embedbase/embedding/openai.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.1.9/embedbase/firebase_auth.py` & `embedbase-1.2.0/embedbase/firebase_auth.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.1.9/embedbase/logging_utils.py` & `embedbase-1.2.0/embedbase/logging_utils.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.1.9/embedbase/models.py` & `embedbase-1.2.0/embedbase/models.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.1.9/embedbase/settings.py` & `embedbase-1.2.0/embedbase/settings.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.1.9/embedbase/strings.py` & `embedbase-1.2.0/embedbase/strings.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.1.9/embedbase/utils.py` & `embedbase-1.2.0/embedbase/utils.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.1.9/pyproject.toml` & `embedbase-1.2.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 [build-system]
 requires = ["poetry_core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
+[virtualenvs]
+create = true
+in-project = true
+
 [tool.poetry]
 name = "embedbase"
-version = "1.1.9"
+version = "1.2.0"
 description = "Open-source API & SDK to integrate your data and easily hook them up to LLMs."
 readme = "README.md"
 authors = ["Different AI <louis@embedbase.xyz>"]
 license = "MIT"
 repository = "https://github.com/different-ai/embedbase"
 homepage = "https://github.com/different-ai/embedbase"
 keywords = ["embeddings", "machine learning", "artificial intelligence", "llm"]
@@ -28,15 +32,15 @@
 # Entry points for the package
 "embedbase" = "embedbase.__main__:run_app"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 
 fastapi = "^0.95.1"
-uvicorn = {extras = ["standard"], version = "^0.15.0"}
+uvicorn = {extras = ["standard"], version = "^0.22.0"}
 pandas = "^1.3.4"
 openai = "^0.27.0"
 tenacity = "^8.0.1"
 pydantic_yaml = {extras = ["pyyaml"], version = "^0.4.0"}
 tiktoken = "^0.3.3"
 
 [tool.poetry.dev-dependencies]
@@ -55,23 +59,25 @@
 coverage = "^6.1.2"
 coverage-badge = "^1.1.0"
 pytest-html = "^3.1.1"
 pytest-cov = "^4.0.0"
 httpx = "^0.23.0"
 pytest-asyncio = "^0.21.0"
 requests-mock = "^1.10.0"
+torch = "2.0.0"
 sentence-transformers = "^2.2.2"
 
 # TODO: following integrations might be moved outside this repo - loose coupling
 firebase-admin = "^6.1.0"
 sentry-sdk = {extras = ["fastapi"], version = "^1.21.1"}
 supabase = "^1.0.3"
 psycopg = {extras = ["binary", "pool"], version = "^3.1.8"}
 pgvector = "^0.1.6"
 
+
 [tool.black]
 target-version = ["py38"]
 line-length = 88
 color = true
 
 exclude = '''
 /(
```

### Comparing `embedbase-1.1.9/PKG-INFO` & `embedbase-1.2.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: embedbase
-Version: 1.1.9
+Version: 1.2.0
 Summary: Open-source API & SDK to integrate your data and easily hook them up to LLMs.
 Home-page: https://github.com/different-ai/embedbase
 License: MIT
 Keywords: embeddings,machine learning,artificial intelligence,llm
 Author: Different AI
 Author-email: louis@embedbase.xyz
 Requires-Python: >=3.8,<4.0
@@ -12,22 +12,26 @@
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Dist: fastapi (>=0.95.1,<0.96.0)
 Requires-Dist: openai (>=0.27.0,<0.28.0)
 Requires-Dist: pandas (>=1.3.4,<2.0.0)
 Requires-Dist: pydantic_yaml[pyyaml] (>=0.4.0,<0.5.0)
 Requires-Dist: tenacity (>=8.0.1,<9.0.0)
 Requires-Dist: tiktoken (>=0.3.3,<0.4.0)
-Requires-Dist: uvicorn[standard] (>=0.15.0,<0.16.0)
+Requires-Dist: uvicorn[standard] (>=0.22.0,<0.23.0)
 Project-URL: Repository, https://github.com/different-ai/embedbase
 Description-Content-Type: text/markdown
 
 <br />
 
 
 <p align="center">
```

