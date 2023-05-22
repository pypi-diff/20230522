# Comparing `tmp/llm_code-0.3.tar.gz` & `tmp/llm_code-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llm_code-0.3.tar", max compression
+gzip compressed data, was "llm_code-0.4.tar", max compression
```

## Comparing `llm_code-0.3.tar` & `llm_code-0.4.tar`

### file list

```diff
@@ -1,10 +1,11 @@
--rw-r--r--   0        0        0     1070 2023-05-19 17:20:49.716226 llm_code-0.3/LICENSE
--rw-r--r--   0        0        0     2933 2023-05-21 02:48:12.815312 llm_code-0.3/README.md
--rw-r--r--   0        0        0       75 2023-05-21 03:18:50.955110 llm_code-0.3/llm_code/__init__.py
--rw-r--r--   0        0        0     2949 2023-05-21 03:25:05.157471 llm_code-0.3/llm_code/llm_code.py
--rw-r--r--   0        0        0     3293 2023-05-21 02:14:00.115437 llm_code-0.3/llm_code/templates.py
--rw-r--r--   0        0        0      161 2023-05-21 02:14:00.117237 llm_code-0.3/prompts/coding/system.toml
--rw-r--r--   0        0        0      613 2023-05-21 02:14:00.117511 llm_code-0.3/prompts/coding/user/input.toml
--rw-r--r--   0        0        0      396 2023-05-21 02:14:00.117693 llm_code-0.3/prompts/coding/user/simple.toml
--rw-r--r--   0        0        0     1132 2023-05-21 03:31:31.039632 llm_code-0.3/pyproject.toml
--rw-r--r--   0        0        0     3865 1970-01-01 00:00:00.000000 llm_code-0.3/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-05-19 17:43:32.824715 llm_code-0.4/LICENSE
+-rw-r--r--   0        0        0     2933 2023-05-21 18:28:27.298503 llm_code-0.4/README.md
+-rw-r--r--   0        0        0       75 2023-05-21 18:28:27.298792 llm_code-0.4/llm_code/__init__.py
+-rw-r--r--   0        0        0     1938 2023-05-22 20:59:37.527156 llm_code-0.4/llm_code/db.py
+-rw-r--r--   0        0        0     4382 2023-05-22 20:59:37.527939 llm_code-0.4/llm_code/llm_code.py
+-rw-r--r--   0        0        0     3293 2023-05-19 22:57:07.356159 llm_code-0.4/llm_code/templates.py
+-rw-r--r--   0        0        0      161 2023-05-19 18:26:22.445515 llm_code-0.4/prompts/coding/system.toml
+-rw-r--r--   0        0        0      613 2023-05-19 18:23:27.578834 llm_code-0.4/prompts/coding/user/input.toml
+-rw-r--r--   0        0        0      396 2023-05-19 18:19:43.905655 llm_code-0.4/prompts/coding/user/simple.toml
+-rw-r--r--   0        0        0     1155 2023-05-22 20:59:37.530387 llm_code-0.4/pyproject.toml
+-rw-r--r--   0        0        0     3909 1970-01-01 00:00:00.000000 llm_code-0.4/PKG-INFO
```

### Comparing `llm_code-0.3/LICENSE` & `llm_code-0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `llm_code-0.3/README.md` & `llm_code-0.4/README.md`

 * *Files identical despite different names*

### Comparing `llm_code-0.3/llm_code/llm_code.py` & `llm_code-0.4/llm_code/llm_code.py`

 * *Files 25% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import click
 import openai
 from pydantic import BaseSettings
 from rich.console import Console
 from rich.syntax import Syntax
 
-from llm_code import __version__
+from llm_code import __version__, db
 
 from .templates import Message, TemplateLibrary
 
 
 class Settings(BaseSettings):
     openai_api_key: str = ""
     model: str = "gpt-3.5-turbo"
@@ -29,32 +29,62 @@
     path = path / "prompts"
     if path.exists():
         return TemplateLibrary.from_file_or_directory(path)
     else:
         return None
 
 
+def init_db(config_dir: Path):
+    config_dir.mkdir(parents=True, exist_ok=True)
+    db_path = config_dir / "db.sqlite"
+    _ = db.Database.get(db_path)
+
+
+def get_cached_response(settings: Settings, messages: list[dict]) -> Optional[Message]:
+    record = db.get_last_inserted_row()
+    if not record:
+        return None
+    if (
+        record.model != settings.model
+        or record.temperature != settings.temperature
+        or record.max_tokens != settings.max_tokens
+        or record.system_message != messages[0]["content"]
+        or record.user_message != messages[1]["content"]
+    ):
+        return None
+
+    return Message(
+        role="assistant",
+        content=record.assistant_message,
+    )
+
+
 @click.command()
 @click.option("-i", "--inputs", default=None, help="Glob of input files.")
-@click.option("-ln", "--line-numbers", is_flag=True, help="Show line numbers.")
+@click.option("-nc", "--no-cache", is_flag=True, help="Don't use cache.")
+@click.option("-4", "--gpt-4", is_flag=True, help="Use GPT-4.")
 @click.option("--version", is_flag=True, help="Show version.")
 @click.argument("instructions", nargs=-1)
-def main(inputs, line_numbers, instructions, version):
+def main(inputs, instructions, version, no_cache, gpt_4):
     """Coding assistant using OpenAI's chat models.
 
     Requires OPENAI_API_KEY as an environment variable. Alternately, you can set it in
     ~/.llm_code/env.
     """
     console = Console()
 
     if version:
         console.print(f"[bold green]llm_code[/] version {__version__}")
         sys.exit(0)
 
     settings = Settings()
+    if gpt_4:
+        settings.model = "gpt-4"
+    init_db(settings.config_dir)
+
     if not settings.openai_api_key:
         raise click.UsageError("OPENAI_API_KEY must be set.")
 
     instructions = " ".join(instructions)
     if not instructions:
         raise click.UsageError("Please provide some instructions.")
 
@@ -70,29 +100,43 @@
     if input:
         message = library["coding/input"].message(code=input, instructions=instructions)
     else:
         message = library["coding/simple"].message(instructions=instructions)
 
     messages = [library["coding/system"].message(), message]
 
-    with console.status("[bold green]Asking OpenAI..."):
-        response = openai.ChatCompletion.create(
-            api_key=settings.openai_api_key,
+    cached_response = get_cached_response(settings, messages)
+    if no_cache or not cached_response:
+        with console.status("[bold green]Asking OpenAI..."):
+            response = openai.ChatCompletion.create(
+                api_key=settings.openai_api_key,
+                model=settings.model,
+                temperature=settings.temperature,
+                max_tokens=settings.max_tokens,
+                messages=messages,
+            )
+
+        message = Message.from_message(response.choices[0]["message"])  # type: ignore
+
+        db.write(
             model=settings.model,
             temperature=settings.temperature,
             max_tokens=settings.max_tokens,
-            messages=messages,
+            system_message=messages[0]["content"],
+            user_message=messages[1]["content"],
+            assistant_message=message.content,
+            input_tokens=response.usage["prompt_tokens"],  # type: ignore
+            output_tokens=response.usage["completion_tokens"],  # type: ignore
         )
+    else:
+        message = cached_response
 
-    message = Message.from_message(response.choices[0]["message"])  # type: ignore
     code = message.code()
     if code:
-        console.print(Syntax(code.code, code.lang, line_numbers=line_numbers))
+        console.print(Syntax(code.code, code.lang))
     else:
         console.print(f"No code found in message: \n\n{message.content}")
         sys.exit(1)
 
 
 if __name__ == "__main__":
     main()
-if __name__ == "__main__":
-    main()
```

### Comparing `llm_code-0.3/llm_code/templates.py` & `llm_code-0.4/llm_code/templates.py`

 * *Files identical despite different names*

### Comparing `llm_code-0.3/prompts/coding/user/input.toml` & `llm_code-0.4/prompts/coding/user/input.toml`

 * *Files identical despite different names*

### Comparing `llm_code-0.3/pyproject.toml` & `llm_code-0.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "llm-code"
-version = "0.3"
+version = "0.4"
 description = "An OpenAI LLM based CLI coding assistant."
 authors = ["Rushabh Doshi <radoshi+pypi@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "llm_code" }]
 homepage = "https://github.com/radoshi/llm-code"
 repository = "https://github.com/radoshi/llm-code"
@@ -23,14 +23,15 @@
 [tool.poetry.dependencies]
 python = "^3.11"
 pydantic = { extras = ["dotenv"], version = "^1.10.7" }
 openai = "^0.27.6"
 click = "^8.1.3"
 rich = "^13.3.5"
 tomli = "^2.0.1"
+sqlalchemy = "^2.0.15"
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.3.0"
 isort = "^5.12.0"
 ruff = "^0.0.269"
 pytest-cov = "^4.0.0"
 mypy = "^1.3.0"
```

### Comparing `llm_code-0.3/PKG-INFO` & `llm_code-0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llm-code
-Version: 0.3
+Version: 0.4
 Summary: An OpenAI LLM based CLI coding assistant.
 Home-page: https://github.com/radoshi/llm-code
 License: MIT
 Keywords: openai,llm,cli,coding,assistant
 Author: Rushabh Doshi
 Author-email: radoshi+pypi@gmail.com
 Requires-Python: >=3.11,<4.0
@@ -15,14 +15,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Code Generators
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: openai (>=0.27.6,<0.28.0)
 Requires-Dist: pydantic[dotenv] (>=1.10.7,<2.0.0)
 Requires-Dist: rich (>=13.3.5,<14.0.0)
+Requires-Dist: sqlalchemy (>=2.0.15,<3.0.0)
 Requires-Dist: tomli (>=2.0.1,<3.0.0)
 Project-URL: Repository, https://github.com/radoshi/llm-code
 Description-Content-Type: text/markdown
 
 # llm-code
 
 ![PyPi](https://img.shields.io/pypi/v/llm-code?color=green)
```

