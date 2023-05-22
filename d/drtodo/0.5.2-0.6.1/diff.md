# Comparing `tmp/drtodo-0.5.2.tar.gz` & `tmp/drtodo-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drtodo-0.5.2.tar", max compression
+gzip compressed data, was "drtodo-0.6.1.tar", max compression
```

## Comparing `drtodo-0.5.2.tar` & `drtodo-0.6.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1064 2023-04-02 19:49:28.749709 drtodo-0.5.2/LICENSE
--rw-r--r--   0        0        0     9429 2023-05-16 21:07:43.881069 drtodo-0.5.2/drtodo/README.md
--rw-r--r--   0        0        0      224 2023-05-16 17:06:02.545312 drtodo-0.5.2/drtodo/__init__.py
--rw-r--r--   0        0        0       44 2023-05-13 23:41:09.525609 drtodo-0.5.2/drtodo/__main__.py
--rw-r--r--   0        0        0    11815 2023-05-17 20:03:17.579930 drtodo-0.5.2/drtodo/main.py
--rw-r--r--   0        0        0     4681 2023-05-17 21:29:11.605170 drtodo-0.5.2/drtodo/man_command.py
--rw-r--r--   0        0        0     4718 2023-05-17 21:29:59.622815 drtodo-0.5.2/drtodo/mdparser.py
--rw-r--r--   0        0        0     1406 2023-05-16 16:38:13.234806 drtodo-0.5.2/drtodo/mistuneplugin.py
--rw-r--r--   0        0        0      618 2023-05-16 16:11:27.772546 drtodo-0.5.2/drtodo/rich_display.py
--rw-r--r--   0        0        0     7088 2023-05-17 22:53:38.670275 drtodo-0.5.2/drtodo/settings.py
--rw-r--r--   0        0        0       11 2023-04-02 19:49:28.755456 drtodo-0.5.2/drtodo/util.py
--rw-r--r--   0        0        0      709 2023-05-17 21:30:39.963042 drtodo-0.5.2/pyproject.toml
--rw-r--r--   0        0        0    10177 1970-01-01 00:00:00.000000 drtodo-0.5.2/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-05-22 16:06:20.808229 drtodo-0.6.1/LICENSE
+-rw-r--r--   0        0        0     9777 2023-05-22 16:06:20.808229 drtodo-0.6.1/drtodo/README.md
+-rw-r--r--   0        0        0      224 2023-05-22 16:06:20.808229 drtodo-0.6.1/drtodo/__init__.py
+-rw-r--r--   0        0        0       44 2023-05-22 16:06:20.808229 drtodo-0.6.1/drtodo/__main__.py
+-rw-r--r--   0        0        0    11816 2023-05-22 16:06:20.808229 drtodo-0.6.1/drtodo/main.py
+-rw-r--r--   0        0        0     4681 2023-05-22 16:06:20.808229 drtodo-0.6.1/drtodo/man_command.py
+-rw-r--r--   0        0        0     4718 2023-05-22 16:06:20.808229 drtodo-0.6.1/drtodo/mdparser.py
+-rw-r--r--   0        0        0     1406 2023-05-22 16:06:20.808229 drtodo-0.6.1/drtodo/mistuneplugin.py
+-rw-r--r--   0        0        0      618 2023-05-22 16:06:20.808229 drtodo-0.6.1/drtodo/rich_display.py
+-rw-r--r--   0        0        0     7052 2023-05-22 16:06:20.808229 drtodo-0.6.1/drtodo/settings.py
+-rw-r--r--   0        0        0       11 2023-05-22 16:06:20.808229 drtodo-0.6.1/drtodo/util.py
+-rw-r--r--   0        0        0      807 2023-05-22 16:06:34.996262 drtodo-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0    10671 1970-01-01 00:00:00.000000 drtodo-0.6.1/PKG-INFO
```

### Comparing `drtodo-0.5.2/LICENSE` & `drtodo-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `drtodo-0.5.2/drtodo/README.md` & `drtodo-0.6.1/drtodo/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,16 @@
 # DrTodo
 
 **DrToDo, MD**: *a straightforward todo list manager for markdown files in git repos.*
 
+TODO items are listed in markdown (*MD*) files using standard markdown syntax understood by most
+environments including Github. You can add and modify these items easily from the command line.
+Markdown files are then just committed to git as you'd normally do and shared with others or as
+part of projects, or just kept locally in your computer.
+
 ## Quick Start
 
 ### installation
 
 ```console
 $ pip install drtodo
 ```
@@ -125,15 +130,15 @@
 
 ```console
 $ DrTodo [OPTIONS] COMMAND [ARGS]...
 ```
 
 **Options**:
 
-* `-s, --settings PATH`: Settings file to use  [default: /Users/bcs/.drtodo]
+* `-s, --settings PATH`: Settings file to use  [default: /Users/USER/.drtodo]
 * `-v, --verbose`: Verbose output
 * `--mdfile PATH`: Markdown file to use for todo list  [default: TEST.md]
 * `-V, --version`: Show version and exit
 * `--install-completion`: Install completion for the current shell.
 * `--show-completion`: Show completion for the current shell, to copy it or customize the installation.
 * `--help`: Show this message and exit.
```

### Comparing `drtodo-0.5.2/drtodo/main.py` & `drtodo-0.6.1/drtodo/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,20 @@
-from typing import Optional
+import re
 from pathlib import Path
+from typing import Optional
+
+import rich.markdown
 import typer
-from rich import print
 from git import Repo
-import rich.markdown
-import re
-from .settings import constants, settings, globals
-from .mdparser import TodoListParser, TaskListTraverser
+from rich import print
+
 from .man_command import manapp
+from .mdparser import TaskListTraverser, TodoListParser
 from .rich_display import console
-
+from .settings import constants, globals, settings
 
 app = typer.Typer(
     no_args_is_help=True,
     rich_markup_mode="markdown",
     help="**{constants.appname}, MD**: *a straightforward todo list manager for markdown files in git repos.*",
     epilog=f"DrTodo can manage items in a global todo list ({globals.global_todofile_pretty})"
     f" and in a local todo list ({globals.local_todofile_pretty or 'if the current folder is under a git repo'})."
```

### Comparing `drtodo-0.5.2/drtodo/man_command.py` & `drtodo-0.6.1/drtodo/man_command.py`

 * *Files identical despite different names*

### Comparing `drtodo-0.5.2/drtodo/mdparser.py` & `drtodo-0.6.1/drtodo/mdparser.py`

 * *Files identical despite different names*

### Comparing `drtodo-0.5.2/drtodo/mistuneplugin.py` & `drtodo-0.6.1/drtodo/mistuneplugin.py`

 * *Files identical despite different names*

### Comparing `drtodo-0.5.2/drtodo/rich_display.py` & `drtodo-0.6.1/drtodo/rich_display.py`

 * *Files identical despite different names*

### Comparing `drtodo-0.5.2/drtodo/settings.py` & `drtodo-0.6.1/drtodo/settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-from __future__ import annotations
-
 import getpass
 from dataclasses import dataclass
 from pathlib import Path
 from typing import Optional, Any, Union
 
 import typer
 from pydantic import BaseModel, BaseSettings, Field
```

### Comparing `drtodo-0.5.2/PKG-INFO` & `drtodo-0.6.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 Metadata-Version: 2.1
 Name: drtodo
-Version: 0.5.2
+Version: 0.6.1
 Summary: DrTodo, MD: todo list manager using markdown files and git
+Home-page: https://github.com/exilium-com/DrTodo
 License: MIT
+Keywords: utilities,todo,markdown
 Author: exilium
 Author-email: info@exilium.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -14,20 +16,26 @@
 Requires-Dist: gitpython
 Requires-Dist: mistune (==3.0.0rc5)
 Requires-Dist: pydantic
 Requires-Dist: rich
 Requires-Dist: tomli ; python_version < "3.11"
 Requires-Dist: typer
 Requires-Dist: typing-extensions (>=4.5.0,<5.0.0) ; python_version < "3.11"
+Project-URL: Repository, https://github.com/exilium-com/DrTodo
 Description-Content-Type: text/markdown
 
 # DrTodo
 
 **DrToDo, MD**: *a straightforward todo list manager for markdown files in git repos.*
 
+TODO items are listed in markdown (*MD*) files using standard markdown syntax understood by most
+environments including Github. You can add and modify these items easily from the command line.
+Markdown files are then just committed to git as you'd normally do and shared with others or as
+part of projects, or just kept locally in your computer.
+
 ## Quick Start
 
 ### installation
 
 ```console
 $ pip install drtodo
 ```
@@ -147,15 +155,15 @@
 
 ```console
 $ DrTodo [OPTIONS] COMMAND [ARGS]...
 ```
 
 **Options**:
 
-* `-s, --settings PATH`: Settings file to use  [default: /Users/bcs/.drtodo]
+* `-s, --settings PATH`: Settings file to use  [default: /Users/USER/.drtodo]
 * `-v, --verbose`: Verbose output
 * `--mdfile PATH`: Markdown file to use for todo list  [default: TEST.md]
 * `-V, --version`: Show version and exit
 * `--install-completion`: Install completion for the current shell.
 * `--show-completion`: Show completion for the current shell, to copy it or customize the installation.
 * `--help`: Show this message and exit.
```

