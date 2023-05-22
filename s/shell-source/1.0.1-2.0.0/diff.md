# Comparing `tmp/shell-source-1.0.1.tar.gz` & `tmp/shell_source-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shell-source-1.0.1.tar", max compression
+gzip compressed data, was "shell_source-2.0.0.tar", max compression
```

## Comparing `shell-source-1.0.1.tar` & `shell_source-2.0.0.tar`

### file list

```diff
@@ -1,8 +1,7 @@
--rw-r--r--   0        0        0     1073 2022-07-13 21:37:09.120671 shell-source-1.0.1/LICENSE
--rw-r--r--   0        0        0     2805 2022-07-13 21:37:09.120671 shell-source-1.0.1/README.md
--rw-r--r--   0        0        0      719 2022-07-13 21:37:09.120671 shell-source-1.0.1/pyproject.toml
--rw-r--r--   0        0        0      513 2022-07-13 21:37:09.120671 shell-source-1.0.1/shell_source/__init__.py
--rw-r--r--   0        0        0     1128 2022-07-13 21:37:09.120671 shell-source-1.0.1/shell_source/shell_config.py
--rw-r--r--   0        0        0     4115 2022-07-13 21:37:09.120671 shell-source-1.0.1/shell_source/source.py
--rw-r--r--   0        0        0     3620 2022-07-13 21:37:17.401450 shell-source-1.0.1/setup.py
--rw-r--r--   0        0        0     3744 2022-07-13 21:37:17.401790 shell-source-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-05-22 12:08:20.496727 shell_source-2.0.0/LICENSE
+-rw-r--r--   0        0        0     2929 2023-05-22 12:08:20.500727 shell_source-2.0.0/README.md
+-rw-r--r--   0        0        0      741 2023-05-22 12:08:20.500727 shell_source-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0      513 2023-05-22 12:08:20.500727 shell_source-2.0.0/shell_source/__init__.py
+-rw-r--r--   0        0        0     1129 2023-05-22 12:08:20.500727 shell_source-2.0.0/shell_source/shell_config.py
+-rw-r--r--   0        0        0     4372 2023-05-22 12:08:20.500727 shell_source-2.0.0/shell_source/source.py
+-rw-r--r--   0        0        0     3919 1970-01-01 00:00:00.000000 shell_source-2.0.0/PKG-INFO
```

### Comparing `shell-source-1.0.1/LICENSE` & `shell_source-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `shell-source-1.0.1/README.md` & `shell_source-2.0.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,28 @@
 # python-shell-source
 A python module for sourcing variables from shell scripts.
 
 ## Installation
+
+You can install this package with pip or conda.
 ```sh
 $ pip install shell-source
 ```
+```sh
+$ conda install -c abrahammurciano shell-source
+```
 
 ## Documentation
 
 The full documentation is available [here](https://abrahammurciano.github.io/python-shell-source/shell_source)
 
 ## Usage
 This module provides a function `source` which attempts to mimic the shell's source command.
 
-The purpose of this function is to allow you to run a shell script which sets either environment variables or local variables, and then give you access to those variables. Normally this is not a straght-forward task, but this function achieves it by running the script in its intended shell then injecting commands to the shell to print its local variables and its environment variables. Finally it collects the shell's stdout and parses it to return to you with exactly the data you asked for.
+The purpose of this function is to allow you to run a shell script which sets either environment variables or local variables, and then give you access to those variables. Normally this is not a straght-forward task, but this function achieves it by running the script in its intended shell then injecting commands to the shell to write its local variables and its environment variables to a temporary file. Finally it reads the temporary file and parses it to return to you with exactly the data you asked for.
 
 ### Basic Usage
 
 If you just pass a script and an interpreter you'll get back all the environment variables and local variables visible to and set by the script.
 
 ```py
 >>> from shell_source import source
```

### Comparing `shell-source-1.0.1/pyproject.toml` & `shell_source-2.0.0/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 [tool.poetry]
 name = "shell-source"
-version = "1.0.1"
+version = "2.0.0"
 description = "A python module for sourcing variables from shell scripts"
 authors = ["Abraham Murciano <abrahammurciano@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/abrahammurciano/python-shell-source"
 documentation = "https://abrahammurciano.github.io/python-shell-source/shell_source/"
 keywords = ["shell", "source", "environment"]
 
 [tool.poetry.dependencies]
 python = "^3.7"
 importlib-metadata = "^4.11.4"
 toml = "^0.10.2"
 
-[tool.poetry.dev-dependencies]
+[tool.poetry.group.dev.dependencies]
+mypy = "^1.3.0"
 pytest = "^7.1.2"
 black = "^22.3.0"
 types-toml = "^0.10.7"
 pdoc3 = "^0.10.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
```

### Comparing `shell-source-1.0.1/shell_source/__init__.py` & `shell_source-2.0.0/shell_source/__init__.py`

 * *Files identical despite different names*

### Comparing `shell-source-1.0.1/shell_source/shell_config.py` & `shell_source-2.0.0/shell_source/shell_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,12 +16,12 @@
         get_var: How to get the value of a variable named {var}.
         get_all_locals: How to print all local variables.
         prev_exit_code: How to get the exit code of the previous command.
     """
 
     source_cmd: str = "source {script}"
     exit_cmd: str = "exit {code}"
-    redirect_stdout: str = "{cmd} > {file}"
+    redirect_stdout: str = "{cmd} >> {file}"
     boolean_or: str = "{cmd1} || {cmd2}"
     get_var: str = "${var}"
     get_all_locals: str = "set"
     prev_exit_code: str = "$?"
```

### Comparing `shell-source-1.0.1/setup.py` & `shell_source-2.0.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,30 +1,86 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: shell-source
+Version: 2.0.0
+Summary: A python module for sourcing variables from shell scripts
+Home-page: https://github.com/abrahammurciano/python-shell-source
+License: MIT
+Keywords: shell,source,environment
+Author: Abraham Murciano
+Author-email: abrahammurciano@gmail.com
+Requires-Python: >=3.7,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: importlib-metadata (>=4.11.4,<5.0.0)
+Requires-Dist: toml (>=0.10.2,<0.11.0)
+Project-URL: Documentation, https://abrahammurciano.github.io/python-shell-source/shell_source/
+Project-URL: Repository, https://github.com/abrahammurciano/python-shell-source
+Description-Content-Type: text/markdown
+
+# python-shell-source
+A python module for sourcing variables from shell scripts.
+
+## Installation
+
+You can install this package with pip or conda.
+```sh
+$ pip install shell-source
+```
+```sh
+$ conda install -c abrahammurciano shell-source
+```
+
+## Documentation
+
+The full documentation is available [here](https://abrahammurciano.github.io/python-shell-source/shell_source)
+
+## Usage
+This module provides a function `source` which attempts to mimic the shell's source command.
+
+The purpose of this function is to allow you to run a shell script which sets either environment variables or local variables, and then give you access to those variables. Normally this is not a straght-forward task, but this function achieves it by running the script in its intended shell then injecting commands to the shell to write its local variables and its environment variables to a temporary file. Finally it reads the temporary file and parses it to return to you with exactly the data you asked for.
+
+### Basic Usage
+
+If you just pass a script and an interpreter you'll get back all the environment variables and local variables visible to and set by the script.
+
+```py
+>>> from shell_source import source
+>>> variables = source("path/to/script.sh", "bash")
+>>> # It returns a dictionary of local and environment variables known by the script.
+>>> variables
+{"USER": "abraham", "PATH": "/bin:/usr/bin", ..., "foo": "bar"}
+```
+
+### Requesting Specific Variables
+
+If you specify the argument `variables`, then only those variables you passed will be present as keys in the returned dictionary.
+
+```py
+>>> source("path/to/script.sh", "csh", variables=("foo", "bar", "biz"))
+{"foo": ..., "bar": ..., "biz", ...}
+```
+
+### Ignoring Local Variables
+
+If you don't want to obtain any local variables set by the script, but only want the environment variables, you can pass `ignore_locals=True`.
+
+### Supporting Different Shells
+
+This module has been tested to work with `bash`, `zsh`, `tcsh`, and `ksh`. You can use any other shell that's somewhat posix compliant and supports the keyword "source", but it it doesn't work, you may use the `ShellConfig` class to indicate to `source` how to interact with your shell.
+
+The class `ShellConfig` contains several string templates which are used to run the necessary commands with the shell. If the shell you want to use doesn't support any of the commands set by default in that class, you can pass an instance of `ShellConfig` to `source` to override the default templates.
+
+For example, `csh` and `fish` are not supported by default, (specifically because they don't have the variable `$?` to get the exit status of the last command,) but we can source a script for one of these shells anyways by passing a `ShellConfig` instance which will declare how to get the exit code of the previous command.
+
+```py
+source(
+	"path/to/script.csh",
+	"csh",
+	shell_config=ShellConfig(prev_exit_code="$status")
+)
+```
 
-packages = \
-['shell_source']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['importlib-metadata>=4.11.4,<5.0.0', 'toml>=0.10.2,<0.11.0']
-
-setup_kwargs = {
-    'name': 'shell-source',
-    'version': '1.0.1',
-    'description': 'A python module for sourcing variables from shell scripts',
-    'long_description': '# python-shell-source\nA python module for sourcing variables from shell scripts.\n\n## Installation\n```sh\n$ pip install shell-source\n```\n\n## Documentation\n\nThe full documentation is available [here](https://abrahammurciano.github.io/python-shell-source/shell_source)\n\n## Usage\nThis module provides a function `source` which attempts to mimic the shell\'s source command.\n\nThe purpose of this function is to allow you to run a shell script which sets either environment variables or local variables, and then give you access to those variables. Normally this is not a straght-forward task, but this function achieves it by running the script in its intended shell then injecting commands to the shell to print its local variables and its environment variables. Finally it collects the shell\'s stdout and parses it to return to you with exactly the data you asked for.\n\n### Basic Usage\n\nIf you just pass a script and an interpreter you\'ll get back all the environment variables and local variables visible to and set by the script.\n\n```py\n>>> from shell_source import source\n>>> variables = source("path/to/script.sh", "bash")\n>>> # It returns a dictionary of local and environment variables known by the script.\n>>> variables\n{"USER": "abraham", "PATH": "/bin:/usr/bin", ..., "foo": "bar"}\n```\n\n### Requesting Specific Variables\n\nIf you specify the argument `variables`, then only those variables you passed will be present as keys in the returned dictionary.\n\n```py\n>>> source("path/to/script.sh", "csh", variables=("foo", "bar", "biz"))\n{"foo": ..., "bar": ..., "biz", ...}\n```\n\n### Ignoring Local Variables\n\nIf you don\'t want to obtain any local variables set by the script, but only want the environment variables, you can pass `ignore_locals=True`.\n\n### Supporting Different Shells\n\nThis module has been tested to work with `bash`, `zsh`, `tcsh`, and `ksh`. You can use any other shell that\'s somewhat posix compliant and supports the keyword "source", but it it doesn\'t work, you may use the `ShellConfig` class to indicate to `source` how to interact with your shell.\n\nThe class `ShellConfig` contains several string templates which are used to run the necessary commands with the shell. If the shell you want to use doesn\'t support any of the commands set by default in that class, you can pass an instance of `ShellConfig` to `source` to override the default templates.\n\nFor example, `csh` and `fish` are not supported by default, (specifically because they don\'t have the variable `$?` to get the exit status of the last command,) but we can source a script for one of these shells anyways by passing a `ShellConfig` instance which will declare how to get the exit code of the previous command.\n\n```py\nsource(\n\t"path/to/script.csh",\n\t"csh",\n\tshell_config=ShellConfig(prev_exit_code="$status")\n)\n```\n',
-    'author': 'Abraham Murciano',
-    'author_email': 'abrahammurciano@gmail.com',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'https://github.com/abrahammurciano/python-shell-source',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.7,<4.0',
-}
-
-
-setup(**setup_kwargs)
```

