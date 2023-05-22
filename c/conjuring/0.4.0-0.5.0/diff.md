# Comparing `tmp/conjuring-0.4.0.tar.gz` & `tmp/conjuring-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "conjuring-0.4.0.tar", max compression
+gzip compressed data, was "conjuring-0.5.0.tar", max compression
```

## Comparing `conjuring-0.4.0.tar` & `conjuring-0.5.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0     1410 2023-05-21 11:47:31.040329 conjuring-0.4.0/docs/README.md
--rw-r--r--   0        0        0     9163 2023-05-21 11:47:31.040329 conjuring-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     1900 2023-05-21 11:47:31.044329 conjuring-0.4.0/src/conjuring/__init__.py
--rw-r--r--   0        0        0      541 2023-05-21 11:47:31.044329 conjuring-0.4.0/src/conjuring/colors.py
--rw-r--r--   0        0        0      313 2023-05-21 11:47:31.044329 conjuring-0.4.0/src/conjuring/constants.py
--rw-r--r--   0        0        0    10397 2023-05-21 11:47:31.044329 conjuring-0.4.0/src/conjuring/grimoire.py
--rw-r--r--   0        0        0        0 2023-05-21 11:47:31.044329 conjuring-0.4.0/src/conjuring/spells/__init__.py
--rw-r--r--   0        0        0     2191 2023-05-21 11:47:31.044329 conjuring-0.4.0/src/conjuring/spells/aws.py
--rw-r--r--   0        0        0     3018 2023-05-21 11:47:31.044329 conjuring-0.4.0/src/conjuring/spells/blanket.py
--rw-r--r--   0        0        0     1438 2023-05-21 11:47:31.044329 conjuring-0.4.0/src/conjuring/spells/conjuring.py
--rw-r--r--   0        0        0     1240 2023-05-21 11:47:31.044329 conjuring-0.4.0/src/conjuring/spells/docker.py
--rw-r--r--   0        0        0     1725 2023-05-21 11:47:31.044329 conjuring-0.4.0/src/conjuring/spells/duplicity.py
--rw-r--r--   0        0        0     1018 2023-05-21 11:47:31.044329 conjuring-0.4.0/src/conjuring/spells/fork.py
--rw-r--r--   0        0        0    14779 2023-05-21 11:47:31.044329 conjuring-0.4.0/src/conjuring/spells/git.py
--rw-r--r--   0        0        0     1008 2023-05-21 11:47:31.044329 conjuring-0.4.0/src/conjuring/spells/jrnl.py
--rw-r--r--   0        0        0     2967 2023-05-21 11:47:31.044329 conjuring-0.4.0/src/conjuring/spells/k8s.py
--rw-r--r--   0        0        0     7050 2023-05-21 11:47:31.044329 conjuring-0.4.0/src/conjuring/spells/media.py
--rw-r--r--   0        0        0      777 2023-05-21 11:47:31.044329 conjuring-0.4.0/src/conjuring/spells/mkdocs.py
--rw-r--r--   0        0        0     2647 2023-05-21 11:47:31.044329 conjuring-0.4.0/src/conjuring/spells/mr.py
--rw-r--r--   0        0        0      824 2023-05-21 11:47:31.044329 conjuring-0.4.0/src/conjuring/spells/onedrive.py
--rw-r--r--   0        0        0    11612 2023-05-21 11:47:31.044329 conjuring-0.4.0/src/conjuring/spells/paperless.py
--rw-r--r--   0        0        0     2724 2023-05-21 11:47:31.044329 conjuring-0.4.0/src/conjuring/spells/pre_commit.py
--rw-r--r--   0        0        0     9159 2023-05-21 11:47:31.044329 conjuring-0.4.0/src/conjuring/spells/py.py
--rw-r--r--   0        0        0     1081 2023-05-21 11:47:31.044329 conjuring-0.4.0/src/conjuring/spells/shell.py
--rw-r--r--   0        0        0     1928 2023-05-21 11:47:31.044329 conjuring-0.4.0/src/conjuring/visibility.py
--rw-r--r--   0        0        0     2528 1970-01-01 00:00:00.000000 conjuring-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1455 2023-05-22 01:07:03.669380 conjuring-0.5.0/docs/README.md
+-rw-r--r--   0        0        0     9175 2023-05-22 01:07:03.669380 conjuring-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     4393 2023-05-22 01:07:03.669380 conjuring-0.5.0/src/conjuring/__init__.py
+-rw-r--r--   0        0        0      541 2023-05-22 01:07:03.669380 conjuring-0.5.0/src/conjuring/colors.py
+-rw-r--r--   0        0        0      398 2023-05-22 01:07:03.669380 conjuring-0.5.0/src/conjuring/constants.py
+-rw-r--r--   0        0        0    10397 2023-05-22 01:07:03.669380 conjuring-0.5.0/src/conjuring/grimoire.py
+-rw-r--r--   0        0        0        0 2023-05-22 01:07:03.669380 conjuring-0.5.0/src/conjuring/spells/__init__.py
+-rw-r--r--   0        0        0     2191 2023-05-22 01:07:03.669380 conjuring-0.5.0/src/conjuring/spells/aws.py
+-rw-r--r--   0        0        0     3018 2023-05-22 01:07:03.669380 conjuring-0.5.0/src/conjuring/spells/blanket.py
+-rw-r--r--   0        0        0     2058 2023-05-22 01:07:03.669380 conjuring-0.5.0/src/conjuring/spells/conjuring.py
+-rw-r--r--   0        0        0     1240 2023-05-22 01:07:03.669380 conjuring-0.5.0/src/conjuring/spells/docker.py
+-rw-r--r--   0        0        0     1725 2023-05-22 01:07:03.669380 conjuring-0.5.0/src/conjuring/spells/duplicity.py
+-rw-r--r--   0        0        0     1018 2023-05-22 01:07:03.669380 conjuring-0.5.0/src/conjuring/spells/fork.py
+-rw-r--r--   0        0        0    14779 2023-05-22 01:07:03.669380 conjuring-0.5.0/src/conjuring/spells/git.py
+-rw-r--r--   0        0        0     1008 2023-05-22 01:07:03.669380 conjuring-0.5.0/src/conjuring/spells/jrnl.py
+-rw-r--r--   0        0        0     2967 2023-05-22 01:07:03.669380 conjuring-0.5.0/src/conjuring/spells/k8s.py
+-rw-r--r--   0        0        0     7050 2023-05-22 01:07:03.669380 conjuring-0.5.0/src/conjuring/spells/media.py
+-rw-r--r--   0        0        0      777 2023-05-22 01:07:03.669380 conjuring-0.5.0/src/conjuring/spells/mkdocs.py
+-rw-r--r--   0        0        0     2647 2023-05-22 01:07:03.669380 conjuring-0.5.0/src/conjuring/spells/mr.py
+-rw-r--r--   0        0        0      824 2023-05-22 01:07:03.669380 conjuring-0.5.0/src/conjuring/spells/onedrive.py
+-rw-r--r--   0        0        0    11612 2023-05-22 01:07:03.669380 conjuring-0.5.0/src/conjuring/spells/paperless.py
+-rw-r--r--   0        0        0     2724 2023-05-22 01:07:03.669380 conjuring-0.5.0/src/conjuring/spells/pre_commit.py
+-rw-r--r--   0        0        0     9187 2023-05-22 01:07:03.669380 conjuring-0.5.0/src/conjuring/spells/py.py
+-rw-r--r--   0        0        0     1081 2023-05-22 01:07:03.669380 conjuring-0.5.0/src/conjuring/spells/shell.py
+-rw-r--r--   0        0        0     1928 2023-05-22 01:07:03.669380 conjuring-0.5.0/src/conjuring/visibility.py
+-rw-r--r--   0        0        0     2573 1970-01-01 00:00:00.000000 conjuring-0.5.0/PKG-INFO
```

### Comparing `conjuring-0.4.0/docs/README.md` & `conjuring-0.5.0/docs/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -5,44 +5,41 @@
 
 ## Features
 
 - Merge any local `tasks.py` file with global Conjuring tasks
 - Use all global Conjuring tasks provided by this package
 - Only include the global Conjuring tasks you want (opt-in mode)
 - Use all Conjuring tasks excluding some (opt-out mode)
+- Add your own custom tasks from Python modules or packages to global tasks
 - Display your custom task modules conditionally
 - Display your custom individual tasks conditionally
 - Merge your project tasks with the global reusable tasks
 - Prefix task names of your custom module
 
 More details on the [features documentation](https://andreoliwa.github.io/conjuring/features/).
 
 ## Tasks
 
 Each module under [the `conjuring/spells` directory](https://github.com/andreoliwa/conjuring/tree/master/src/conjuring/spells)
 is a collection of Invoke tasks.
 
 ## Quick setup
 
-1. Install invoke in an isolated virtualenv with [pipx](https://github.com/pypa/pipx):
+1. Install Conjuring in an isolated virtualenv with [pipx](https://github.com/pypa/pipx):
 
    ```shell
-   pipx install invoke
+   pipx install --include-deps conjuring
    ```
 
-2. Install Conjuring from GitHub, injecting it directly into the isolated virtualenv:
+   The `--include-deps` flag is needed to install Invoke's apps (`invoke` and `inv`).
 
-   ```shell
-   pipx inject invoke conjuring
-   ```
-
-3. Create a `tasks.py` file on your home dir:
+2. Create a `tasks.py` file on your home dir:
 
    ```shell
    echo -e "from conjuring import *\n\nnamespace = cast_all_spells()" > ~/tasks.py
    ```
 
-4. You should see the list of Conjuring tasks from any directory where you type this:
+3. You should see the list of Conjuring tasks from any directory where you type this:
 
    ```shell
    invoke --list
    ```
```

### Comparing `conjuring-0.4.0/pyproject.toml` & `conjuring-0.5.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "conjuring"
-version = "0.4.0"
+version = "0.5.0"
 description = "🐍🤖 Reusable global Invoke tasks that can be merged with local project tasks"
 authors = ["W. Augusto Andreoli <andreoliwa@gmail.com>"]
 license = "MIT"
 readme = "docs/README.md"
 repository = "https://github.com/andreoliwa/conjuring"
 documentation = "https://andreoliwa.github.io/conjuring/"
 keywords = ["invoke", "tasks", "automation", "cli", "python"]
@@ -24,15 +24,15 @@
 requests = "*"
 
 [tool.poetry.dev-dependencies]
 pytest = "*"
 
 [tool.commitizen]
 name = "cz_conventional_commits"
-version = "0.4.0"
+version = "0.5.0"
 
 # https://commitizen-tools.github.io/commitizen/bump/#configuration
 version_files = [
     "pyproject.toml:^version"
 ]
 tag_format = "v$version"
 update_changelog_on_bump = true
@@ -56,15 +56,19 @@
 select = ["ALL"]
 
 # https://beta.ruff.rs/docs/settings/#show-fixes
 show-fixes = true
 
 # https://beta.ruff.rs/docs/settings/#ignore
 ignore = [
+    "ANN101", # Missing type annotation for ? in method
     "ERA", # https://beta.ruff.rs/docs/rules/#eradicate-era
+    "D107", # Missing docstring in ? https://beta.ruff.rs/docs/rules/?q=D107
+    "D203", # 1 blank line required before class docstring
+    "D213", # Multi-line docstring summary should start at the second line
     "TD002", # Missing author https://beta.ruff.rs/docs/rules/#flake8-todos-td
     "TD003", # Missing issue link on the line following this
 ]
 
 # https://beta.ruff.rs/docs/settings/#line-length
 line-length = 120
 
@@ -95,27 +99,25 @@
 ]
 # TODO: Ignores to fix
 # A001 Variable ? is shadowing a Python builtin https://beta.ruff.rs/docs/rules/?q=A001
 # A002 Argument ? is shadowing a Python builtin https://beta.ruff.rs/docs/rules/?q=A002
 # ANN001 Missing type annotation for function argument ? https://beta.ruff.rs/docs/rules/?q=ANN001
 # ANN002 Missing type annotation for ? https://beta.ruff.rs/docs/rules/?q=ANN002
 # ANN003 Missing type annotation for ? https://beta.ruff.rs/docs/rules/?q=ANN003
-# ANN101 Missing type annotation for ? in method https://beta.ruff.rs/docs/rules/?q=ANN101
 # ANN201 Missing return type annotation for public function ? https://beta.ruff.rs/docs/rules/?q=ANN201
 # ANN202 Missing return type annotation for private function ? https://beta.ruff.rs/docs/rules/?q=ANN202
 # ANN204 Missing return type annotation for special method ? https://beta.ruff.rs/docs/rules/?q=ANN204
 # ARG001 Unused function argument: ? https://beta.ruff.rs/docs/rules/?q=ARG001
 # B904 Within an ? clause, raise exceptions with ? or ? to distinguish them from errors in exception handling https://beta.ruff.rs/docs/rules/?q=B904
 # D100 Missing docstring in public module https://beta.ruff.rs/docs/rules/?q=D100
 # D101 Missing docstring in public class https://beta.ruff.rs/docs/rules/?q=D101
 # D102 Missing docstring in public method https://beta.ruff.rs/docs/rules/?q=D102
 # D103 Missing docstring in public function https://beta.ruff.rs/docs/rules/?q=D103
 # D104 Missing docstring in public package https://beta.ruff.rs/docs/rules/?q=D104
 # D105 Missing docstring in magic method https://beta.ruff.rs/docs/rules/?q=D105
-# D107 Missing docstring in ? https://beta.ruff.rs/docs/rules/?q=D107
 # D401 First line of docstring should be in imperative mood: "Setup Conjuring on your home dir." https://beta.ruff.rs/docs/rules/?q=D401
 # DTZ011 The use of ? is not allowed, use ? instead https://beta.ruff.rs/docs/rules/?q=DTZ011
 # E402 Module level import not at top of file https://beta.ruff.rs/docs/rules/?q=E402
 # E501 Line too long (134 > 120 characters) https://beta.ruff.rs/docs/rules/?q=E501
 # FBT001 Boolean positional arg in function definition https://beta.ruff.rs/docs/rules/?q=FBT001
 # FBT002 Boolean default value in function definition https://beta.ruff.rs/docs/rules/?q=FBT002
 # FBT003 Boolean positional value in function call https://beta.ruff.rs/docs/rules/?q=FBT003
@@ -130,31 +132,31 @@
 # TCH003 Move standard library import ? into a type-checking block https://beta.ruff.rs/docs/rules/?q=TCH003
 # TRY300 Consider moving this statement to an ? block https://beta.ruff.rs/docs/rules/?q=TRY300
 "src/conjuring/colors.py" = ["D100"]
 "src/conjuring/constants.py" = ["D100"]
 "src/conjuring/grimoire.py" = ["ANN001", "ANN003", "ANN201", "B904", "D100", "D101", "D103", "PLR0913", "T201", "TCH003"]
 "src/conjuring/spells/__init__.py" = ["D104"]
 "src/conjuring/spells/aws.py" = ["ANN001", "ANN002", "ANN201", "D100", "D103", "T201"]
-"src/conjuring/spells/blanket.py" = ["ANN001", "ANN101", "ANN201", "ANN204", "D101", "D105", "FBT002", "ISC003", "PGH003", "PLR0913", "T201"]
+"src/conjuring/spells/blanket.py" = ["ANN001", "ANN201", "ANN204", "D101", "D105", "FBT002", "ISC003", "PGH003", "PLR0913", "T201"]
 "src/conjuring/spells/conjuring.py" = ["ANN001", "ANN201", "D100", "D401", "FBT002", "PLR5501", "T201"]
 "src/conjuring/spells/docker.py" = ["ANN001", "ANN201", "D100", "FBT002"]
 "src/conjuring/spells/duplicity.py" = ["ANN001", "ANN201", "D100", "D103", "T201"]
 "src/conjuring/spells/fork.py" = ["ANN001", "ANN201", "D100"]
-"src/conjuring/spells/git.py" = ["ANN001", "ANN101", "ANN201", "D100", "D101", "D102", "D107", "E501", "FBT002", "T201", "TRY300"]
+"src/conjuring/spells/git.py" = ["ANN001", "ANN201", "D100", "D101", "D102", "E501", "FBT002", "T201", "TRY300"]
 "src/conjuring/spells/jrnl.py" = ["A001", "ANN001", "ANN201", "D100", "FBT002", "PLR0913"]
-"src/conjuring/spells/k8s.py" = ["ANN001", "ANN101", "ANN201", "FBT002"]
+"src/conjuring/spells/k8s.py" = ["ANN001", "ANN201", "FBT002"]
 "src/conjuring/spells/media.py" = ["ANN001", "ANN201", "D100", "DTZ011", "FBT002", "RET508", "T201"]
 "src/conjuring/spells/mkdocs.py" = ["ANN001", "ANN201"]
-"src/conjuring/spells/mr.py" = ["ANN001", "ANN101", "ANN201", "D101", "FBT002", "T201"]
+"src/conjuring/spells/mr.py" = ["ANN001", "ANN201", "D101", "FBT002", "T201"]
 "src/conjuring/spells/onedrive.py" = ["ANN001", "ANN201", "D100", "T201"]
-"src/conjuring/spells/paperless.py" = ["ANN001", "ANN101", "ANN201", "ANN202", "ANN204", "D101", "D103", "D105", "FBT001", "FBT002", "FBT003", "PLR0913", "PLR2004", "T201", "TCH003"]
+"src/conjuring/spells/paperless.py" = ["ANN001", "ANN201", "ANN202", "ANN204", "D101", "D103", "D105", "FBT001", "FBT002", "FBT003", "PLR0913", "PLR2004", "T201", "TCH003"]
 "src/conjuring/spells/pre_commit.py" = ["ANN001", "ANN201", "ANN202", "D100", "FBT001", "FBT002"]
-"src/conjuring/spells/py.py" = ["ANN001", "ANN101", "ANN201", "ANN202", "D100", "D101", "D102", "D107", "FBT001", "FBT002", "FBT003", "PLR0913", "RET504", "T201"]
+"src/conjuring/spells/py.py" = ["ANN001", "ANN201", "ANN202", "D100", "D101", "D102", "FBT001", "FBT002", "FBT003", "PLR0913", "RET504", "T201"]
 "src/conjuring/spells/shell.py" = ["ANN001", "ANN201"]
-"src/conjuring/visibility.py" = ["A002", "ANN001", "ANN101", "ANN201", "D100", "D101", "D103", "D107", "FBT001", "FBT002", "PLR0913"]
+"src/conjuring/visibility.py" = ["A002", "ANN001", "ANN201", "D100", "D101", "D103", "FBT001", "FBT002", "PLR0913"]
 "tests/__init__.py" = ["D104"]
 "tests/fixtures/__init__.py" = ["D104"]
 "tests/fixtures/conditional.py" = ["ANN001", "ANN201", "ARG001"]
 "tests/fixtures/magic.py" = ["ANN001", "ANN201", "ARG001"]
 "tests/fixtures/not_prefixed.py" = ["ANN001", "ANN201", "ARG001"]
 "tests/fixtures/prefixed.py" = ["ANN001", "ANN201", "ARG001"]
 "tests/fixtures/root.py" = ["ANN001", "ANN201", "ARG001"]
```

### Comparing `conjuring-0.4.0/src/conjuring/colors.py` & `conjuring-0.5.0/src/conjuring/colors.py`

 * *Files identical despite different names*

### Comparing `conjuring-0.4.0/src/conjuring/grimoire.py` & `conjuring-0.5.0/src/conjuring/grimoire.py`

 * *Files identical despite different names*

### Comparing `conjuring-0.4.0/src/conjuring/spells/aws.py` & `conjuring-0.5.0/src/conjuring/spells/aws.py`

 * *Files identical despite different names*

### Comparing `conjuring-0.4.0/src/conjuring/spells/blanket.py` & `conjuring-0.5.0/src/conjuring/spells/blanket.py`

 * *Files identical despite different names*

### Comparing `conjuring-0.4.0/src/conjuring/spells/conjuring.py` & `conjuring-0.5.0/src/conjuring/spells/conjuring.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,41 +1,52 @@
 from pathlib import Path
 
 from invoke import task
 
-from conjuring.grimoire import run_command
-from conjuring.visibility import ShouldDisplayTasks, is_home_dir
+from conjuring.constants import CONJURING_INIT, INVOKE_YAML
+from conjuring.grimoire import print_success, print_warning, run_command, run_stdout
 
 SHOULD_PREFIX = True
-should_display_tasks: ShouldDisplayTasks = is_home_dir
 
 
 @task(
     help={
         "edit": "Open the config file with $EDITOR",
         "revert": "Revert the changes and go back to using tasks.py as the default tasks file",
     },
 )
-def setup(c, edit=False, revert=False):
-    """Setup Conjuring on your home dir."""
-    config_file = Path("~/.invoke.yaml").expanduser()
-    json_config = """'{"tasks":{"collection_name":"conjuring_summon"}}'"""
+def init(c, edit=False, revert=False):
+    """Init Conjuring on your home dir to merge any local `tasks.py` file with global Conjuring tasks."""
+    config_file = INVOKE_YAML
+
+    json_config = f"""'{{"tasks":{{"collection_name":"{CONJURING_INIT}"}}'"""
     if config_file.exists():
-        message = "Remove this from" if revert else "Add this to"
-        print(f"The {config_file} configuration file already exists! {message} the file:")
-        run_command(c, "yq eval -n", json_config)
-        if edit:
-            run_command(c, "$EDITOR", str(config_file))
+        current_collection_name = run_stdout(c, f"yq e '.tasks.collection_name' {config_file}")
+        if current_collection_name == CONJURING_INIT:
+            print_success(f"Configuration file is already set to {CONJURING_INIT!r}")
+            run_command(c, f"cat {config_file}")
+        else:
+            message = "Remove this from" if revert else "Add this to"
+            print(f"The {config_file} configuration file already exists! {message} the file:")
+            run_command(c, "yq eval -n", json_config)
+            if edit:
+                run_command(c, "$EDITOR", str(config_file))
     else:
         if not revert:
             c.run(f"touch {config_file}")
             run_command(c, "yq eval -i", json_config, str(config_file))
             c.run(f"cat {config_file}")
 
     default_tasks = Path("~/tasks.py").expanduser()
-    conjuring_tasks = Path("~/conjuring_summon.py").expanduser()
+    conjuring_init = Path(f"~/{CONJURING_INIT}.py").expanduser()
     if revert:
-        if conjuring_tasks.exists():
-            conjuring_tasks.rename(default_tasks)
+        if conjuring_init.exists():
+            conjuring_init.rename(default_tasks)
     else:
         if default_tasks.exists():
-            default_tasks.rename(conjuring_tasks)
+            default_tasks.rename(conjuring_init)
+        else:
+            if conjuring_init.exists():
+                print_success("Global tasks file already exists.")
+                run_command(c, f"cat {conjuring_init}")
+            else:
+                print_warning(f"Nothing to do: file {default_tasks} does not exist!")
```

### Comparing `conjuring-0.4.0/src/conjuring/spells/docker.py` & `conjuring-0.5.0/src/conjuring/spells/docker.py`

 * *Files identical despite different names*

### Comparing `conjuring-0.4.0/src/conjuring/spells/duplicity.py` & `conjuring-0.5.0/src/conjuring/spells/duplicity.py`

 * *Files identical despite different names*

### Comparing `conjuring-0.4.0/src/conjuring/spells/fork.py` & `conjuring-0.5.0/src/conjuring/spells/fork.py`

 * *Files identical despite different names*

### Comparing `conjuring-0.4.0/src/conjuring/spells/git.py` & `conjuring-0.5.0/src/conjuring/spells/git.py`

 * *Files identical despite different names*

### Comparing `conjuring-0.4.0/src/conjuring/spells/jrnl.py` & `conjuring-0.5.0/src/conjuring/spells/jrnl.py`

 * *Files identical despite different names*

### Comparing `conjuring-0.4.0/src/conjuring/spells/k8s.py` & `conjuring-0.5.0/src/conjuring/spells/k8s.py`

 * *Files identical despite different names*

### Comparing `conjuring-0.4.0/src/conjuring/spells/media.py` & `conjuring-0.5.0/src/conjuring/spells/media.py`

 * *Files identical despite different names*

### Comparing `conjuring-0.4.0/src/conjuring/spells/mkdocs.py` & `conjuring-0.5.0/src/conjuring/spells/mkdocs.py`

 * *Files identical despite different names*

### Comparing `conjuring-0.4.0/src/conjuring/spells/mr.py` & `conjuring-0.5.0/src/conjuring/spells/mr.py`

 * *Files identical despite different names*

### Comparing `conjuring-0.4.0/src/conjuring/spells/onedrive.py` & `conjuring-0.5.0/src/conjuring/spells/onedrive.py`

 * *Files identical despite different names*

### Comparing `conjuring-0.4.0/src/conjuring/spells/paperless.py` & `conjuring-0.5.0/src/conjuring/spells/paperless.py`

 * *Files identical despite different names*

### Comparing `conjuring-0.4.0/src/conjuring/spells/pre_commit.py` & `conjuring-0.5.0/src/conjuring/spells/pre_commit.py`

 * *Files identical despite different names*

### Comparing `conjuring-0.4.0/src/conjuring/spells/py.py` & `conjuring-0.5.0/src/conjuring/spells/py.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from pathlib import Path
 from textwrap import dedent
 from typing import Optional
 
 from invoke import Context, task
 
 from conjuring.grimoire import print_error, run_command, run_lines, run_with_fzf
-from conjuring.visibility import ShouldDisplayTasks, is_poetry_project
+from conjuring.visibility import MagicTask, ShouldDisplayTasks, is_poetry_project
 
 SHOULD_PREFIX = True
 should_display_tasks: ShouldDisplayTasks = is_poetry_project
 
 PYPROJECT_TOML = "pyproject.toml"
 REGEX_RUFF_LINE = re.compile(r"^(?P<filename>.*?):\d+:\d+: (?P<code>.*?)(?P<message> .*)$")
 REGEX_RUFF_MESSAGE = re.compile(r"`[^`]+`")
@@ -190,15 +190,15 @@
         "pudb" if pudb or all_ else "",
         "icecream" if icecream or all_ else "",
         "devtools[pygments]" if devtools or all_ else "",
     ]
     run_command(c, "poetry run pip install --upgrade", *tools)
 
 
-@task
+@task(klass=MagicTask)
 def ruff_config(c):
     """Generate ruff configuration from existing warnings."""
     # TODO: feat: check if the global ruff is installed and use it if it is
     ignore: dict[str, set[str]] = defaultdict(set)
     per_file_ignores: dict[str, set[str]] = defaultdict(set)
     for line in run_lines(c, "pre-commit run --all-files ruff", warn=True):
         if line.startswith("warning:"):
```

### Comparing `conjuring-0.4.0/src/conjuring/spells/shell.py` & `conjuring-0.5.0/src/conjuring/spells/shell.py`

 * *Files identical despite different names*

### Comparing `conjuring-0.4.0/src/conjuring/visibility.py` & `conjuring-0.5.0/src/conjuring/visibility.py`

 * *Files identical despite different names*

### Comparing `conjuring-0.4.0/PKG-INFO` & `conjuring-0.5.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: conjuring
-Version: 0.4.0
+Version: 0.5.0
 Summary: 🐍🤖 Reusable global Invoke tasks that can be merged with local project tasks
 Home-page: https://github.com/andreoliwa/conjuring
 License: MIT
 Keywords: invoke,tasks,automation,cli,python
 Author: W. Augusto Andreoli
 Author-email: andreoliwa@gmail.com
 Requires-Python: >=3.9,<4.0
@@ -33,45 +33,42 @@
 
 ## Features
 
 - Merge any local `tasks.py` file with global Conjuring tasks
 - Use all global Conjuring tasks provided by this package
 - Only include the global Conjuring tasks you want (opt-in mode)
 - Use all Conjuring tasks excluding some (opt-out mode)
+- Add your own custom tasks from Python modules or packages to global tasks
 - Display your custom task modules conditionally
 - Display your custom individual tasks conditionally
 - Merge your project tasks with the global reusable tasks
 - Prefix task names of your custom module
 
 More details on the [features documentation](https://andreoliwa.github.io/conjuring/features/).
 
 ## Tasks
 
 Each module under [the `conjuring/spells` directory](https://github.com/andreoliwa/conjuring/tree/master/src/conjuring/spells)
 is a collection of Invoke tasks.
 
 ## Quick setup
 
-1. Install invoke in an isolated virtualenv with [pipx](https://github.com/pypa/pipx):
+1. Install Conjuring in an isolated virtualenv with [pipx](https://github.com/pypa/pipx):
 
    ```shell
-   pipx install invoke
+   pipx install --include-deps conjuring
    ```
 
-2. Install Conjuring from GitHub, injecting it directly into the isolated virtualenv:
+   The `--include-deps` flag is needed to install Invoke's apps (`invoke` and `inv`).
 
-   ```shell
-   pipx inject invoke conjuring
-   ```
-
-3. Create a `tasks.py` file on your home dir:
+2. Create a `tasks.py` file on your home dir:
 
    ```shell
    echo -e "from conjuring import *\n\nnamespace = cast_all_spells()" > ~/tasks.py
    ```
 
-4. You should see the list of Conjuring tasks from any directory where you type this:
+3. You should see the list of Conjuring tasks from any directory where you type this:
 
    ```shell
    invoke --list
    ```
```

