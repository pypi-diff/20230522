# Comparing `tmp/qtgql-0.116.1.tar.gz` & `tmp/qtgql-0.117.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qtgql-0.116.1.tar", max compression
+gzip compressed data, was "qtgql-0.117.0.tar", max compression
```

## Comparing `qtgql-0.116.1.tar` & `qtgql-0.117.0.tar`

### file list

```diff
@@ -1,40 +1,26 @@
--rw-r--r--   0        0        0     1064 2023-04-04 14:21:32.337292 qtgql-0.116.1/LICENSE
--rw-r--r--   0        0        0     2243 2023-04-04 14:21:32.337292 qtgql-0.116.1/README.md
--rw-r--r--   0        0        0     4537 2023-04-04 14:21:50.997379 qtgql-0.116.1/pyproject.toml
--rw-r--r--   0        0        0      138 2023-04-04 14:21:32.349292 qtgql-0.116.1/qtgql/__init__.py
--rw-r--r--   0        0        0        0 2023-04-04 14:21:32.349292 qtgql-0.116.1/qtgql/codegen/__init__.py
--rw-r--r--   0        0        0     2176 2023-04-04 14:21:32.349292 qtgql-0.116.1/qtgql/codegen/cli.py
--rw-r--r--   0        0        0     3187 2023-04-04 14:21:32.349292 qtgql-0.116.1/qtgql/codegen/graphql_ref.py
--rw-r--r--   0        0        0    20033 2023-04-04 14:21:32.349292 qtgql-0.116.1/qtgql/codegen/introspection.py
--rw-r--r--   0        0        0        0 2023-04-04 14:21:32.349292 qtgql-0.116.1/qtgql/codegen/py/__init__.py
--rw-r--r--   0        0        0        0 2023-04-04 14:21:32.349292 qtgql-0.116.1/qtgql/codegen/py/compiler/__init__.py
--rw-r--r--   0        0        0     1057 2023-04-04 14:21:32.353292 qtgql-0.116.1/qtgql/codegen/py/compiler/builtin_scalars.py
--rw-r--r--   0        0        0     2382 2023-04-04 14:21:32.353292 qtgql-0.116.1/qtgql/codegen/py/compiler/config.py
--rw-r--r--   0        0        0     7900 2023-04-04 14:21:32.353292 qtgql-0.116.1/qtgql/codegen/py/compiler/operation.py
--rw-r--r--   0        0        0     2971 2023-04-04 14:21:32.353292 qtgql-0.116.1/qtgql/codegen/py/compiler/template.py
--rw-r--r--   0        0        0    10561 2023-04-04 14:21:32.353292 qtgql-0.116.1/qtgql/codegen/py/objecttype.py
--rw-r--r--   0        0        0        0 2023-04-04 14:21:32.353292 qtgql-0.116.1/qtgql/codegen/py/runtime/__init__.py
--rw-r--r--   0        0        0     7553 2023-04-04 14:21:32.353292 qtgql-0.116.1/qtgql/codegen/py/runtime/bases.py
--rw-r--r--   0        0        0     4152 2023-04-04 14:21:32.353292 qtgql-0.116.1/qtgql/codegen/py/runtime/custom_scalars.py
--rw-r--r--   0        0        0     1417 2023-04-04 14:21:32.353292 qtgql-0.116.1/qtgql/codegen/py/runtime/environment.py
--rw-r--r--   0        0        0     5642 2023-04-04 14:21:32.353292 qtgql-0.116.1/qtgql/codegen/py/runtime/queryhandler.py
--rw-r--r--   0        0        0      569 2023-04-04 14:21:32.353292 qtgql-0.116.1/qtgql/codegen/py/templates/config.jinja.py
--rw-r--r--   0        0        0     4819 2023-04-04 14:21:32.353292 qtgql-0.116.1/qtgql/codegen/py/templates/handlers.jinja.py
--rw-r--r--   0        0        0     7045 2023-04-04 14:21:32.353292 qtgql-0.116.1/qtgql/codegen/py/templates/macros.jinja.py
--rw-r--r--   0        0        0     6198 2023-04-04 14:21:32.353292 qtgql-0.116.1/qtgql/codegen/py/templates/schema.jinja.py
--rw-r--r--   0        0        0      607 2023-04-04 14:21:32.353292 qtgql-0.116.1/qtgql/codegen/utils.py
--rw-r--r--   0        0        0       41 2023-04-04 14:21:32.353292 qtgql-0.116.1/qtgql/exceptions.py
--rw-r--r--   0        0        0        0 2023-04-04 14:21:32.353292 qtgql-0.116.1/qtgql/ext/__init__.py
--rw-r--r--   0        0        0      306 2023-04-04 14:21:32.353292 qtgql-0.116.1/qtgql/ext/mypy_plugin.py
--rwxr-xr-x   0        0        0      126 2023-04-04 14:21:32.353292 qtgql-0.116.1/qtgql/gqltransport/__init__.py
--rw-r--r--   0        0        0     8894 2023-04-04 14:21:32.353292 qtgql-0.116.1/qtgql/gqltransport/client.py
--rw-r--r--   0        0        0     1116 2023-04-04 14:21:32.353292 qtgql-0.116.1/qtgql/gqltransport/core.py
--rw-r--r--   0        0        0        0 2023-04-04 14:21:32.353292 qtgql-0.116.1/qtgql/py.typed
--rw-r--r--   0        0        0      154 2023-04-04 14:21:32.353292 qtgql-0.116.1/qtgql/tools/__init__.py
--rw-r--r--   0        0        0     3439 2023-04-04 14:21:32.353292 qtgql-0.116.1/qtgql/tools/autoproperty.py
--rwxr-xr-x   0        0        0    10819 2023-04-04 14:21:32.353292 qtgql-0.116.1/qtgql/tools/itemsystem.py
--rw-r--r--   0        0        0     1898 2023-04-04 14:21:32.353292 qtgql-0.116.1/qtgql/tools/qproperty.py
--rw-r--r--   0        0        0     1549 2023-04-04 14:21:32.353292 qtgql-0.116.1/qtgql/tools/slot.py
--rw-r--r--   0        0        0        0 2023-04-04 14:21:32.353292 qtgql-0.116.1/qtgql/utils/__init__.py
--rw-r--r--   0        0        0      241 2023-04-04 14:21:32.353292 qtgql-0.116.1/qtgql/utils/graphql.py
--rw-r--r--   0        0        0     3339 1970-01-01 00:00:00.000000 qtgql-0.116.1/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-05-22 06:43:00.978167 qtgql-0.117.0/LICENSE
+-rw-r--r--   0        0        0     1901 2023-05-22 06:43:00.978167 qtgql-0.117.0/README.md
+-rw-r--r--   0        0        0     4342 2023-05-22 06:43:28.758674 qtgql-0.117.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-22 06:43:00.990167 qtgql-0.117.0/qtgqlcodegen/__init__.py
+-rw-r--r--   0        0        0     1866 2023-05-22 06:43:00.990167 qtgql-0.117.0/qtgqlcodegen/cli.py
+-rw-r--r--   0        0        0        0 2023-05-22 06:43:00.990167 qtgql-0.117.0/qtgqlcodegen/compiler/__init__.py
+-rw-r--r--   0        0        0     1587 2023-05-22 06:43:00.990167 qtgql-0.117.0/qtgqlcodegen/compiler/builtin_scalars.py
+-rw-r--r--   0        0        0    11556 2023-05-22 06:43:00.990167 qtgql-0.117.0/qtgqlcodegen/compiler/operation.py
+-rw-r--r--   0        0        0     3731 2023-05-22 06:43:00.990167 qtgql-0.117.0/qtgqlcodegen/compiler/template.py
+-rw-r--r--   0        0        0     2065 2023-05-22 06:43:00.990167 qtgql-0.117.0/qtgqlcodegen/config.py
+-rw-r--r--   0        0        0      413 2023-05-22 06:43:00.990167 qtgql-0.117.0/qtgqlcodegen/cppref.py
+-rw-r--r--   0        0        0       41 2023-05-22 06:43:00.990167 qtgql-0.117.0/qtgqlcodegen/exceptions.py
+-rw-r--r--   0        0        0     3187 2023-05-22 06:43:00.990167 qtgql-0.117.0/qtgqlcodegen/graphql_ref.py
+-rw-r--r--   0        0        0    17696 2023-05-22 06:43:00.990167 qtgql-0.117.0/qtgqlcodegen/introspection.py
+-rw-r--r--   0        0        0    10999 2023-05-22 06:43:00.990167 qtgql-0.117.0/qtgqlcodegen/objecttype.py
+-rw-r--r--   0        0        0        0 2023-05-22 06:43:00.990167 qtgql-0.117.0/qtgqlcodegen/py.typed
+-rw-r--r--   0        0        0        0 2023-05-22 06:43:00.990167 qtgql-0.117.0/qtgqlcodegen/runtime/__init__.py
+-rw-r--r--   0        0        0     4152 2023-05-22 06:43:00.990167 qtgql-0.117.0/qtgqlcodegen/runtime/custom_scalars.py
+-rw-r--r--   0        0        0     5662 2023-05-22 06:43:00.990167 qtgql-0.117.0/qtgqlcodegen/runtime/queryhandler.py
+-rw-r--r--   0        0        0      467 2023-05-22 06:43:00.990167 qtgql-0.117.0/qtgqlcodegen/templates/CMakeLists.jinja.cmake
+-rw-r--r--   0        0        0      541 2023-05-22 06:43:00.990167 qtgql-0.117.0/qtgqlcodegen/templates/config.jinja.hpp
+-rw-r--r--   0        0        0     2065 2023-05-22 06:43:00.990167 qtgql-0.117.0/qtgqlcodegen/templates/macros.jinja.hpp
+-rw-r--r--   0        0        0     2397 2023-05-22 06:43:00.990167 qtgql-0.117.0/qtgqlcodegen/templates/operation.jinja.hpp
+-rw-r--r--   0        0        0     2461 2023-05-22 06:43:00.990167 qtgql-0.117.0/qtgqlcodegen/templates/schema.jinja.hpp
+-rw-r--r--   0        0        0     1028 2023-05-22 06:43:00.994167 qtgql-0.117.0/qtgqlcodegen/utils.py
+-rw-r--r--   0        0        0     2896 1970-01-01 00:00:00.000000 qtgql-0.117.0/PKG-INFO
```

### Comparing `qtgql-0.116.1/LICENSE` & `qtgql-0.117.0/LICENSE`

 * *Files identical despite different names*

### Comparing `qtgql-0.116.1/README.md` & `qtgql-0.117.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -7,34 +7,25 @@
 [![Discord](https://img.shields.io/discord/1067870318301032558?label=discord&style=for-the-badge)](https://discord.gg/5vmRRJp9fu)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/qtgql?style=for-the-badge)
 
 ### Disclaimer
 This project is currently under development, and **it is not** production ready,
 You can play-around and tell us what is wrong / missing / awesome :smile:.
 
-[Visit the docs for more info](https://nrbnlulu.github.io/qtgql/)
+[Visit the docs for more info](https://nrbnlulu.github.io/qtgql/) (WIP)
 
 
 ### Features
-- [x] object types, for each field there is a corresponding `Property`
-- [x] enums
-- [x] custom scalars
-- [x] Unions
-- [x] interfaces
-- [x] Garbage collection
-- [x] Type-safe Mutation handlers
-- [x] Type-safe Query handlers: queries your server when a component uses this query (or imperatively fetched).
-- [x] Query updates: fetch the same query multiple times would not instantiate everything from scratch
+- [ ] object types, for each field there is a corresponding `Property`
+- [ ] enums
+- [ ] custom scalars
+- [ ] Unions
+- [ ] interfaces
+- [ ] Garbage collection
+- [ ] Type-safe Mutation handlers
+- [ ] Type-safe Query handlers: queries your server when a component uses this query (or imperatively fetched).
+- [ ] Query updates: fetch the same query multiple times would not instantiate everything from scratch
 it would compare the current data with data received and emit __only__ the signals that are needed.
 - [x] Native-Qt client implementation of "[graphql-transport-ws](https://github.com/enisdenjo/graphql-ws/blob/master/PROTOCOL.md)" protocol (supports subscriptions) - You can provide your own network layer though.
-- [x] Mutations.
-- [x] Subscriptions.
-- [x] Fully typed input variables.
-
-#### Helpers
-- [x] generic models that get created from dictionaries (with update, pop, insert implemented by default)
-- [x] `Property` classes that are accessible from QML, with dataclasses  syntax (using attrs)
-- [x] `@slot` - decorator to be replaced with `QtCore.Slot()` that get types from type hints.
-
-### TODO
-- Migrate to C++
-- Fragments?
+- [ ] Mutations.
+- [ ] Subscriptions.
+- [ ] Fully typed input variables.
```

### Comparing `qtgql-0.116.1/pyproject.toml` & `qtgql-0.117.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,66 +1,64 @@
 [tool.poetry]
 name = "qtgql"
-version = "0.116.1"
-packages = [{ include = "qtgql" }]
+version = "0.117.0"
+packages = [{ include = "qtgqlcodegen" }]
 description = "Qt framework for building graphql driven QML applications"
 authors = ["Nir <88795475+nrbnlulu@users.noreply.github.com>"]
 maintainers = ["Nir.J Benlulu <nrbnlulu@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.urls]
 "Homepage" = "https://github.com/nrbnlulu/qtgql"
 "Documentation" = "https://nrbnlulu.github.io/qtgql/"
 
 
 [tool.poetry.dependencies]
 python = ">=3.9,<3.12"
-PySide6 = "^6.4.2"
 attrs = "^22.2.0"
 # codegen
-graphql-core = {version = "<3.3.0", optional=true}
+graphql-core = "^3.2.3"
 jinja2 = {version = "^3.1.2", optional=true}
-typer = {extras = ["all"], version = "^0.7.0", optional=true}
-toml = {version = "^0.10.2", optional=true}
 typingref = "^0.100.0"
+typer = "^0.9.0"
+rich = "^13.3.5"
+frozendict = "^2.3.8"
 
 
 
 [tool.poetry.group.dev.dependencies]
-pytest-qt = "^4.2.0"
 pytest-cov = "^4.0.0"
 aiohttp = {extras = ["speedups"], version = "^3.8.3"}
-
 faker = ">=15.3.4,<19.0.0"
-types-toml = "^0.10.8.1"
-# doc deps
+mypy = "^1.0.1"
+strawberry-graphql = ">=0.158.2,<0.180.0"
+aqtinstall = "^3.1.6"
+conan = "^2.0.4"
+cmake = "3.25.0"
+
+[tool.poetry.group.docs.dependencies]
 mkdocs-material = "^9.0.5"
 mike = "^1.1.2"
 markdown-include = "^0.8.0"
-mkdocstrings = {extras = ["python"], version = ">=0.19.1,<0.21.0"}
+mkdocstrings = {extras = ["python"], version = ">=0.19.1,<0.22.0"}
 pygments = "^2.14.0"
-mktestdocs = "^0.2.0"
-mypy = "^1.0.1"
-strawberry-graphql = ">=0.158.2,<0.180.0"
 
 
-[tool.poetry.extras]
-codegen = ["graphql-core", "jinja2", "typer", "toml"]
+
 
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 
 
 [tool.mypy]
-plugins = ['qtgql/ext/mypy_plugin.py']
 ignore_missing_imports = "True"
 exclude = "(?x)^(.*\\.jinja.py|)$"
 warn_no_return = "False"
 
 [tool.black]
 line-length = 100
 target-version = ['py310']
@@ -244,8 +242,8 @@
 [tool.autopub]
 git-username = "QtGqlBot"
 git-email = "bot@no.reply"
 project-name = "qtgql"
 append-github-contributor = true
 
 [tool.poetry.scripts]
-qtgql = "qtgql.codegen.cli:entrypoint"
+qtgql = "qtgql.cli:entrypoint"
```

### Comparing `qtgql-0.116.1/qtgql/codegen/cli.py` & `qtgql-0.117.0/qtgqlcodegen/cli.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,78 +1,65 @@
 from __future__ import annotations
 
+import glob
 import importlib
+import os
+import sys
 from pathlib import Path
-from typing import Optional
 from typing import TYPE_CHECKING
 
 import rich
-import toml
 import typer
 
 if TYPE_CHECKING:
-    from qtgql.codegen.py.compiler.config import QtGqlConfig
+    from qtgqlcodegen.config import QtGqlConfig
 
 console = rich.console.Console()
-
-
-# these lines are covered coverage failed to catch them.
-def _get_pyproject(p: Path) -> Optional[Path]:
-    pproject = p / "pyproject.toml"
-    if pproject.exists():
-        return pproject
-
-
-def _find_pyproject(p: Path) -> Optional[Path]:
-    if pp := _get_pyproject(p):
-        return pp
-    for parent in p.parents:  # pragma: no cover
-        return _find_pyproject(parent)
-
-
-def _get_app_import_path(root: Path = Path.cwd()) -> str:
-    pyproject = _find_pyproject(root)
-    assert pyproject
-    pp = toml.load(pyproject)
-    try:
-        return pp["tool"][TOOL_NAME][QTGQL_CONFIG_KEY]
-    except KeyError as e:
-        raise KeyError(
-            f"Could not find 'tool.{TOOL_NAME}' in your pyproject.toml.",
-            f"or you haven't defined '{QTGQL_CONFIG_KEY}'",
-            "Make sure you have configured your project properly",
-        ) from e
-
-
 app = typer.Typer(pretty_exceptions_show_locals=False)
 
-TOOL_NAME = "qtgql"
-QTGQL_CONFIG_KEY = "config"
+QTGQL_CONFIG_FNAME = "qtgqlconfig.py"
 
 
 def _get_config() -> QtGqlConfig:
-    console.print("[bold blue]Running system checks")
-    mod, conf = _get_app_import_path().split(":")
-    return getattr(importlib.import_module(mod), conf)
+    console.print("[bold blue]Looking for you config file...")
+    res = glob.glob(f"{QTGQL_CONFIG_FNAME}")
+
+    if not len(res) > 1:
+        console.print(
+            f"[bold red]Found more than one config file. {len(res)}"
+            f" found: {os.linesep.join(res)}",
+        )
+        typer.Abort()
+    if len(res) == 0:
+        console.print("[bold red]Found more than one config file using the first one")
+        typer.Abort()
+    mod_path = Path(res[0]).resolve(True)
+    spec = importlib.util.spec_from_file_location(QTGQL_CONFIG_FNAME, mod_path)
+    assert spec
+    module = importlib.util.module_from_spec(spec)
+    sys.modules[QTGQL_CONFIG_FNAME] = module
+    assert spec.loader
+    spec.loader.exec_module(module)
+    return module.config
 
 
 @app.command()
 def gen():
     """Generates types based on your `QtGqlConfig` configuration object."""
     console.print("[bold blue]Generating...")
     with console.status("Still generating...") as s:
         config = _get_config()
         s.update("[green]Configuration file loaded")
         s.update("[bold blue]Just a second I need some coffee ☕")
         config.generate()
 
     console.print(
         "[bold green]Types were generated to"
-        f"[link={config.generated_types_dir.resolve()}]"
-        f"file://{config.generated_types_dir.resolve()}[/link] successfully!",
+        f"[link={config.generated_dir.resolve()}]"
+        f"file://{config.generated_dir.resolve()}[/link] successfully!",
     )
 
 
 @app.command()
 def hotreload():  # pragma: no cover
     raise NotImplementedError
```

### Comparing `qtgql-0.116.1/qtgql/codegen/graphql_ref.py` & `qtgql-0.117.0/qtgqlcodegen/graphql_ref.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.116.1/qtgql/codegen/introspection.py` & `qtgql-0.117.0/qtgqlcodegen/introspection.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,55 +1,59 @@
 from __future__ import annotations
 
+import subprocess
 import warnings
 from functools import cached_property
 from typing import List
 from typing import Optional
 from typing import TYPE_CHECKING
 from typing import TypedDict
 from typing import Union
 
 import graphql
 from graphql import language as gql_lang
 from graphql import OperationType
 from graphql.language import visitor
 from graphql.type import definition as gql_def
 
-from qtgql.codegen.graphql_ref import is_enum_definition
-from qtgql.codegen.graphql_ref import is_input_definition
-from qtgql.codegen.graphql_ref import is_interface_definition
-from qtgql.codegen.graphql_ref import is_list_definition
-from qtgql.codegen.graphql_ref import is_named_type_node
-from qtgql.codegen.graphql_ref import is_non_null_definition
-from qtgql.codegen.graphql_ref import is_nonnull_node
-from qtgql.codegen.graphql_ref import is_object_definition
-from qtgql.codegen.graphql_ref import is_operation_def_node
-from qtgql.codegen.graphql_ref import is_scalar_definition
-from qtgql.codegen.graphql_ref import is_union_definition
-from qtgql.codegen.py.compiler.builtin_scalars import BuiltinScalars
-from qtgql.codegen.py.compiler.operation import QtGqlOperationDefinition
-from qtgql.codegen.py.compiler.operation import QtGqlQueriedField
-from qtgql.codegen.py.compiler.template import handlers_template
-from qtgql.codegen.py.compiler.template import schema_types_template
-from qtgql.codegen.py.compiler.template import TemplateContext
-from qtgql.codegen.py.objecttype import EnumMap
-from qtgql.codegen.py.objecttype import EnumValue
-from qtgql.codegen.py.objecttype import GqlTypeHinter
-from qtgql.codegen.py.objecttype import QtGqlEnumDefinition
-from qtgql.codegen.py.objecttype import QtGqlFieldDefinition
-from qtgql.codegen.py.objecttype import QtGqlInputFieldDefinition
-from qtgql.codegen.py.objecttype import QtGqlInputObjectTypeDefinition
-from qtgql.codegen.py.objecttype import QtGqlInterfaceDefinition
-from qtgql.codegen.py.objecttype import QtGqlObjectTypeDefinition
-from qtgql.codegen.py.objecttype import QtGqlVariableDefinition
-from qtgql.codegen.utils import anti_forward_ref
-from qtgql.exceptions import QtGqlException
+from qtgqlcodegen.compiler.builtin_scalars import BuiltinScalars
+from qtgqlcodegen.compiler.operation import QtGqlOperationDefinition
+from qtgqlcodegen.compiler.template import cmake_template
+from qtgqlcodegen.compiler.template import CmakeTemplateContext
+from qtgqlcodegen.compiler.template import operation_template
+from qtgqlcodegen.compiler.template import OperationTemplateContext
+from qtgqlcodegen.compiler.template import schema_types_template
+from qtgqlcodegen.compiler.template import SchemaTemplateContext
+from qtgqlcodegen.exceptions import QtGqlException
+from qtgqlcodegen.graphql_ref import is_enum_definition
+from qtgqlcodegen.graphql_ref import is_input_definition
+from qtgqlcodegen.graphql_ref import is_interface_definition
+from qtgqlcodegen.graphql_ref import is_list_definition
+from qtgqlcodegen.graphql_ref import is_named_type_node
+from qtgqlcodegen.graphql_ref import is_non_null_definition
+from qtgqlcodegen.graphql_ref import is_nonnull_node
+from qtgqlcodegen.graphql_ref import is_object_definition
+from qtgqlcodegen.graphql_ref import is_operation_def_node
+from qtgqlcodegen.graphql_ref import is_scalar_definition
+from qtgqlcodegen.graphql_ref import is_union_definition
+from qtgqlcodegen.objecttype import EnumMap
+from qtgqlcodegen.objecttype import EnumValue
+from qtgqlcodegen.objecttype import GqlTypeHinter
+from qtgqlcodegen.objecttype import QtGqlEnumDefinition
+from qtgqlcodegen.objecttype import QtGqlFieldDefinition
+from qtgqlcodegen.objecttype import QtGqlInputFieldDefinition
+from qtgqlcodegen.objecttype import QtGqlInputObjectTypeDefinition
+from qtgqlcodegen.objecttype import QtGqlInterfaceDefinition
+from qtgqlcodegen.objecttype import QtGqlObjectTypeDefinition
+from qtgqlcodegen.objecttype import QtGqlVariableDefinition
+from qtgqlcodegen.utils import anti_forward_ref
+from qtgqlcodegen.utils import FileSpec
 
 if TYPE_CHECKING:  # pragma: no cover
-    from qtgql.codegen.py.compiler.config import QtGqlConfig
+    from qtgqlcodegen.config import QtGqlConfig
 
 introspection_query = graphql.get_introspection_query(descriptions=True)
 
 
 class GeneratedNamespace(TypedDict):
     handlers: str
     objecttypes: str
@@ -60,31 +64,17 @@
 
     Also injects id field to types that have id field but not explicitly
     queried it.
     """
 
     def __init__(self, evaluator: SchemaEvaluator):
         super().__init__()
-        self.query_handlers: dict[str, QtGqlOperationDefinition] = {}
-        self.mutation_handlers: dict[str, QtGqlOperationDefinition] = {}
-        self.subscription_handlers: dict[str, QtGqlOperationDefinition] = {}
+        self.operations: dict[str, QtGqlOperationDefinition] = {}
         self.evaluator = evaluator
 
-    def _get_root_type_field(
-        self,
-        root_type: QtGqlObjectTypeDefinition,
-        gql_field: gql_lang.FieldNode,
-    ) -> QtGqlQueriedField:
-        return QtGqlQueriedField.from_field(
-            root_type.fields_dict[gql_field.name.value],
-            gql_field.selection_set,
-            self.evaluator,
-            parent_interface_field=None,
-        )
-
     def _parse_variable_definition(
         self,
         var: gql_lang.VariableDefinitionNode,
     ) -> QtGqlVariableDefinition:
         return QtGqlVariableDefinition(
             name=var.variable.name.value,
             type=self.evaluator.get_type(var.type),
@@ -97,86 +87,40 @@
     def enter_operation_definition(self, node, key, parent, path, ancestors) -> None:
         if operation := is_operation_def_node(node):
             if operation.operation in (
                 OperationType.QUERY,
                 OperationType.MUTATION,
                 OperationType.SUBSCRIPTION,
             ):
-                root_field: gql_lang.FieldNode = operation.selection_set.selections[0]  # type: ignore
                 assert operation.name, "QtGql enforces operations to have names."
-                op_name = operation.name.value
                 operation_vars: list[QtGqlVariableDefinition] = []
+
+                # input variables
                 if variables_def := operation.variable_definitions:
                     for var in variables_def:
                         operation_vars.append(self._parse_variable_definition(var))
-                if operation.operation is OperationType.QUERY:
-                    assert self.evaluator._query_type
-                    root_qtgql_field = self._get_root_type_field(
-                        self.evaluator._query_type,
-                        root_field,
-                    )
-                    operation_definition = QtGqlOperationDefinition(
-                        query=graphql.print_ast(node),
-                        operation_type=self.evaluator._query_type,
-                        name=op_name,
-                        field=root_qtgql_field,
-                        directives=node.directives,
-                        variables=operation_vars,
-                    )
-                    self.query_handlers[op_name] = operation_definition
-                elif operation.operation is OperationType.MUTATION:
-                    assert (
-                        self.evaluator._mutation_type
-                    ), "You don't have any mutations on your schema"
-                    root_qtgql_field = self._get_root_type_field(
-                        self.evaluator._mutation_type,
-                        root_field,
-                    )
-                    operation_definition = QtGqlOperationDefinition(
-                        query=graphql.print_ast(node),
-                        operation_type=self.evaluator._mutation_type,
-                        name=op_name,
-                        field=root_qtgql_field,
-                        directives=node.directives,
-                        variables=operation_vars,
-                    )
-                    self.mutation_handlers[op_name] = operation_definition
 
-                elif operation.operation is OperationType.SUBSCRIPTION:
-                    assert (
-                        self.evaluator._subscription_type
-                    ), "You don't have a subscription type on your schema"
-                    root_qtgql_field = self._get_root_type_field(
-                        self.evaluator._subscription_type,
-                        root_field,
-                    )
-                    operation_definition = QtGqlOperationDefinition(
-                        query=graphql.print_ast(node),
-                        operation_type=self.evaluator._subscription_type,
-                        name=op_name,
-                        field=root_qtgql_field,
-                        directives=node.directives,
-                        variables=operation_vars,
-                    )
-                    self.subscription_handlers[op_name] = operation_definition
+                operation_definition = QtGqlOperationDefinition.from_definition(
+                    operation_def=operation,
+                    evaluator=self.evaluator,
+                    directives=node.directives,
+                    variables=operation_vars,
+                )
+                self.operations[operation_definition.name] = operation_definition
 
 
 class SchemaEvaluator:
     def __init__(self, config: QtGqlConfig):
         self.config = config
         self._objecttypes_def_map: dict[str, QtGqlObjectTypeDefinition] = {}
         self._enums_def_map: EnumMap = {}
         self._input_objects_def_map: dict[str, QtGqlInputObjectTypeDefinition] = {}
         self._interfaces_map: dict[str, QtGqlInterfaceDefinition] = {}
-        self._query_handlers: dict[str, QtGqlOperationDefinition] = {}
-        self._mutation_handlers: dict[str, QtGqlOperationDefinition] = {}
-        self._subscription_handlers: dict[str, QtGqlOperationDefinition] = {}
-        self._query_type: Optional[QtGqlObjectTypeDefinition] = None
-        self._mutation_type: Optional[QtGqlObjectTypeDefinition] = None
-        self._subscription_type: Optional[QtGqlObjectTypeDefinition] = None
+        self._operations: dict[str, QtGqlOperationDefinition] = {}
+        self.operation_types: dict[OperationType, QtGqlObjectTypeDefinition] = {}
 
     def get_interface_by_name(self, name: str) -> Optional[QtGqlInterfaceDefinition]:
         return self._interfaces_map.get(name, None)
 
     def get_objecttype_by_name(self, name: str) -> Optional[QtGqlObjectTypeDefinition]:
         return self._objecttypes_def_map.get(name, None)
 
@@ -192,25 +136,30 @@
             gql_concrete = self.schema_definition.get_type(named_type.name.value)
             assert gql_concrete
             return self._evaluate_field_type(gql_concrete)
         raise NotImplementedError(node, "Type is not supported as a variable ATM")
 
     @cached_property
     def schema_definition(self) -> graphql.GraphQLSchema:
-        with (self.config.graphql_dir / "schema.graphql").open() as f:
-            return graphql.build_schema(f.read())
+        return graphql.build_schema(
+            (self.config.graphql_dir / "schema.graphql").resolve(True).read_text(),
+        )
 
     @cached_property
     def root_types(self) -> List[Optional[gql_def.GraphQLObjectType]]:
         return [
             self.schema_definition.get_root_type(OperationType.QUERY),
             self.schema_definition.get_root_type(OperationType.MUTATION),
             self.schema_definition.get_root_type(OperationType.SUBSCRIPTION),
         ]
 
+    @cached_property
+    def root_types_names(self) -> str:
+        return " ".join([tp.name for tp in self.root_types if tp])
+
     def _evaluate_field_type(self, t: gql_def.GraphQLType) -> GqlTypeHinter:
         # even though every type in qtgql has a default constructor,
         # hence there is no "real" non-null values
         # we store it as optional for generating nullable checks only for what's required.
         ret = None
         is_optional = True
         if non_null := is_non_null_definition(t):
@@ -304,15 +253,15 @@
     def _evaluate_object_type(
         self,
         type_: gql_def.GraphQLObjectType,
     ) -> Optional[QtGqlObjectTypeDefinition]:
         t_name: str = type_.name
         if evaluated := self._objecttypes_def_map.get(t_name, None):
             return evaluated
-        if type_ not in self.root_types:
+        if type_.name not in self.root_types_names:
             try:
                 id_field = type_.fields["id"]
                 if nonull := is_non_null_definition(id_field.type):
                     id_scalar = graphql.type.scalars.GraphQLID
                     if nonull.of_type is not id_scalar:
                         raise QtGqlException(
                             f"id field type must be of the {id_scalar} scalar!"
@@ -337,15 +286,14 @@
             name=t_name,
             implements=implements,
             docstring=type_.description,
             fields_dict={
                 name: self._evaluate_field(name, field) for name, field in type_.fields.items()
             },
         )
-        assert ret not in self.root_types
         self._objecttypes_def_map[ret.name] = ret
         for interface in type_.interfaces:
             qtgql_interface = self._evaluate_interface_type(interface)
             qtgql_interface.implementations[type_.name] = ret
         return ret
 
     def _evaluate_input_type(
@@ -403,19 +351,19 @@
     def parse_schema_concretes(self) -> None:
         for name, type_ in self.schema_definition.type_map.items():
             if name.startswith("__"):
                 continue
             if object_definition := is_object_definition(type_):
                 if object_type := self._evaluate_object_type(object_definition):
                     if object_definition is self.schema_definition.query_type:
-                        self._query_type = object_type
+                        self.operation_types[OperationType.QUERY] = object_type
                     elif object_definition is self.schema_definition.mutation_type:
-                        self._mutation_type = object_type
+                        self.operation_types[OperationType.MUTATION] = object_type
                     elif object_definition is self.schema_definition.subscription_type:
-                        self._subscription_type = object_type
+                        self.operation_types[OperationType.SUBSCRIPTION] = object_type
 
             elif enum_def := is_enum_definition(type_):
                 if enum := self._evaluate_enum(enum_def):
                     self._enums_def_map[enum.name] = enum
 
     def parse_operations(self) -> None:
         with (self.config.graphql_dir / "operations.graphql").open() as f:
@@ -424,39 +372,60 @@
         # validate the operation against the static schema
         if errors := graphql.validate(self.schema_definition, operations):
             raise QtGqlException([error.formatted for error in errors])
 
         # get QtGql fields from the query AST and inject ID field.
         operation_miner = QtGqlVisitor(self)
         visitor.visit(operations, operation_miner)
-        self._query_handlers.update(operation_miner.query_handlers)
-        self._mutation_handlers.update(operation_miner.mutation_handlers)
-        self._subscription_handlers.update(operation_miner.subscription_handlers)
+        self._operations.update(operation_miner.operations)
 
-    def dumps(self) -> GeneratedNamespace:
-        """:return: The generated modules as a string."""
+    def generate(self) -> list[FileSpec]:
         self.parse_schema_concretes()
         self.parse_operations()
-        context = TemplateContext(
+        context = SchemaTemplateContext(
             enums=list(self._enums_def_map.values()),
             types=[
                 t
                 for name, t in self._objecttypes_def_map.items()
-                if name not in BuiltinScalars.keys()
+                if name not in BuiltinScalars.keys() and name not in self.root_types_names
             ],
-            queries=list(self._query_handlers.values()),
             interfaces=list(self._interfaces_map.values()),
-            mutations=list(self._mutation_handlers.values()),
-            subscriptions=list(self._subscription_handlers.values()),
             input_objects=list(self._input_objects_def_map.values()),
             config=self.config,
         )
-        return GeneratedNamespace(
-            handlers=handlers_template(context),
-            objecttypes=schema_types_template(context),
+
+        operations: list[FileSpec] = []
+        for op_name, op in self._operations.items():
+            operations.append(
+                FileSpec(
+                    content=operation_template(
+                        OperationTemplateContext(
+                            operation=op,
+                            config=self.config,
+                        ),
+                    ),
+                    path=self.config.generated_dir / f"{op_name}.hpp",
+                ),
+            )
+        schema = FileSpec(
+            content=schema_types_template(context),
+            path=self.config.generated_dir / "schema.hpp",
         )
 
+        return [schema, *operations]
+
     def dump(self):
         """:param file: Path to the directory the codegen would dump to."""
-        for fname, content in self.dumps().items():
-            with (self.config.graphql_dir / (fname + ".py")).open("w") as fh:
-                fh.write(content)
+        headers = self.generate()
+
+        args = ["clang-format"] + [
+            str(f.path) for f in headers if f.path.suffix in (".cpp", ".h", ".hpp")
+        ]
+        cmake = FileSpec(
+            content=cmake_template(CmakeTemplateContext(config=self.config, sources=headers)),
+            path=self.config.generated_dir / "CMakeLists.txt",
+        )
+        headers.append(cmake)
+        args.append("-i")
+        for f in headers:
+            f.dump()
+        subprocess.run(args)
```

### Comparing `qtgql-0.116.1/qtgql/codegen/py/compiler/config.py` & `qtgql-0.117.0/qtgqlcodegen/config.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,64 +1,58 @@
 from functools import cached_property
 from pathlib import Path
 from typing import Callable
 from typing import Type
 
 from attrs import define
 
-from qtgql.codegen.introspection import SchemaEvaluator
-from qtgql.codegen.py.compiler.template import schema_types_template
-from qtgql.codegen.py.compiler.template import TemplateContext
-from qtgql.codegen.py.runtime.bases import _BaseQGraphQLObject
-from qtgql.codegen.py.runtime.bases import BaseGraphQLObject
-from qtgql.codegen.py.runtime.custom_scalars import CUSTOM_SCALARS
-from qtgql.codegen.py.runtime.custom_scalars import CustomScalarMap
+from qtgqlcodegen.compiler.template import schema_types_template
+from qtgqlcodegen.compiler.template import SchemaTemplateContext
+from qtgqlcodegen.introspection import SchemaEvaluator
+from qtgqlcodegen.runtime.custom_scalars import CUSTOM_SCALARS
+from qtgqlcodegen.runtime.custom_scalars import CustomScalarMap
 
 
 @define(slots=False)
 class QtGqlConfig:
     """Encapsulates configurations for a qtgql-codegen application per GraphQL
     schema."""
 
     graphql_dir: Path
-    """A directory contains [schema.graphql, query.graphql, mutation.graphql,
-    subscription.graphql] generated types come from the schema.
+    """A directory contains.
 
-    and queries, mutations, subscription handlers would be generated
-    from the corresponding `.graphql` files.
+    - schema.graphql, represents the current schema definition at the server.
+    - operations.graphql, queries, mutations and subscription handlers would be generated based on the operations defined there.
     """
     env_name: str = "QGqlEnv"
     """The generated types would find the environment by this name.
 
     Also the generated QML imports would fall under this namespace.
     """
     evaluator: Type[SchemaEvaluator] = SchemaEvaluator
     """evaluates the schema and generates types."""
-    custom_scalars: CustomScalarMap = CUSTOM_SCALARS
+    custom_scalars: CustomScalarMap = {}
     """mapping of custom scalars, respected by the schema evaluator."""
-    template_class: Callable[[TemplateContext], str] = schema_types_template
+    template_class: Callable[[SchemaTemplateContext], str] = schema_types_template
     """jinja template."""
-    base_object: Type[_BaseQGraphQLObject] = BaseGraphQLObject
-    """base object to be extended by all generated types."""
 
-    @property
+    @cached_property
     def schema_path(self) -> Path:
         return self.graphql_dir / "schema.graphql"
 
-    @property
+    @cached_property
     def operations_dir(self) -> Path:
         return self.graphql_dir / "operations.graphql"
 
-    @property
-    def generated_types_dir(self) -> Path:
-        return self.graphql_dir / "objecttypes.py"
-
-    @property
-    def generated_handlers_dir(self) -> Path:
-        return self.graphql_dir / "handlers.py"
+    @cached_property
+    def generated_dir(self):
+        ret = self.graphql_dir / "__generated__"
+        if not ret.exists():
+            ret.mkdir()
+        return ret
 
     @cached_property
     def _evaluator(self) -> SchemaEvaluator:
         return self.evaluator(self)
 
     def generate(self) -> None:
         self._evaluator.dump()
```

### Comparing `qtgql-0.116.1/qtgql/codegen/py/compiler/template.py` & `qtgql-0.117.0/qtgqlcodegen/compiler/template.py`

 * *Files 21% similar despite different names*

```diff
@@ -6,67 +6,104 @@
 
 from attrs import define
 from jinja2 import Environment
 from jinja2 import PackageLoader
 from jinja2 import select_autoescape
 
 if TYPE_CHECKING:  # pragma: no cover
-    from qtgql.codegen.py.compiler.config import QtGqlConfig
-    from qtgql.codegen.py.compiler.query import QtGqlOperationDefinition, QtGqlQueriedField
-    from qtgql.codegen.py.objecttype import (
+    from qtgqlcodegen.config import QtGqlConfig
+    from qtgqlcodegen.compiler.operation import QtGqlOperationDefinition, QtGqlQueriedField
+    from qtgqlcodegen.utils import FileSpec
+    from qtgqlcodegen.objecttype import (
         QtGqlEnumDefinition,
         QtGqlInputObjectTypeDefinition,
         QtGqlInterfaceDefinition,
         QtGqlObjectTypeDefinition,
     )
 
-template_env = Environment(loader=PackageLoader("qtgql.codegen.py"), autoescape=select_autoescape())
 
-SCHEMA_TEMPLATE = template_env.get_template("schema.jinja.py")
-HANDLERS_TEMPLATE = template_env.get_template("handlers.jinja.py")
-CONFIG_TEMPLATE = template_env.get_template("config.jinja.py")
+template_env = Environment(
+    loader=PackageLoader("qtgqlcodegen"),
+    autoescape=select_autoescape(),
+    variable_start_string="👉",  # originally {{ variable }}, using 👉 variable 👈 because C++ uses curly brackets.
+    variable_end_string="👈",
+)
+
+
+def wrap_curly_filter(v: str, ignore: bool = False) -> str:
+    if ignore:
+        return v
+    return "{" + v + "}"
+
+
+template_env.filters["wrapcurly"] = wrap_curly_filter
+
+SCHEMA_TEMPLATE = template_env.get_template("schema.jinja.hpp")
+OPERATION_TEMPLATE = template_env.get_template("operation.jinja.hpp")
+CONFIG_TEMPLATE = template_env.get_template("config.jinja.hpp")
+CMAKE_TEMPLATE = template_env.get_template("CMakeLists.jinja.cmake")
 
 
 @define
-class TemplateContext:
+class SchemaTemplateContext:
     enums: list[QtGqlEnumDefinition]
     types: list[QtGqlObjectTypeDefinition]
     interfaces: list[QtGqlInterfaceDefinition]
-    queries: list[QtGqlOperationDefinition]
-    mutations: list[QtGqlOperationDefinition]
-    subscriptions: list[QtGqlOperationDefinition]
     input_objects: list[QtGqlInputObjectTypeDefinition]
     config: QtGqlConfig
 
     @property
     def dependencies(self) -> list[str]:
         def build_import_statement(t: type[Any]) -> str:
             mod = inspect.getmodule(t)
             assert mod
             return f"from {mod.__name__} import {t.__name__}"
 
         ret = [build_import_statement(scalar) for scalar in self.config.custom_scalars.values()]
-        ret.append(build_import_statement(self.config.base_object))
         return ret
 
     @property
     def custom_scalars(self) -> list[str]:
         return [scalar.__name__ for scalar in self.config.custom_scalars.values()]
 
+
+@define(slots=False)
+class OperationTemplateContext:
+    operation: QtGqlOperationDefinition
+    config: QtGqlConfig
+
     @property
-    def base_object_name(self) -> str:
-        return self.config.base_object.__name__
+    def ns(self) -> str:
+        return self.operation.name.lower()
+
+    @property
+    def schema_ns(self) -> str:
+        return self.config.env_name
 
 
-def schema_types_template(context: TemplateContext) -> str:
+def schema_types_template(context: SchemaTemplateContext) -> str:
     return SCHEMA_TEMPLATE.render(context=context)
 
 
-def handlers_template(context: TemplateContext) -> str:
-    return HANDLERS_TEMPLATE.render(context=context)
+def operation_template(context: OperationTemplateContext) -> str:
+    return OPERATION_TEMPLATE.render(context=context)
+
+
+@define(slots=False)
+class CmakeTemplateContext:
+    config: QtGqlConfig
+    sources: list[FileSpec]
+
+    @property
+    def target_name(self) -> str:
+        return self.config.env_name
+
+
+def cmake_template(context: SchemaTemplateContext) -> str:
+    return CMAKE_TEMPLATE.render(context=context)
 
 
 @define
 class ConfigContext:
     p_field: QtGqlQueriedField
 
     @property
@@ -81,15 +118,16 @@
         else:
             return {}
 
     @property
     def selections(self) -> dict[str, str]:
         if self.p_field.selections:
             return {
-                selection.name: selection.as_conf_string() for selection in self.p_field.selections
+                selection.name: selection.as_conf_string()
+                for selection in self.p_field.selections.values()
             }
         else:
             return {}
 
 
 def config_template(context: ConfigContext):
     return CONFIG_TEMPLATE.render(context=context)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `qtgql-0.116.1/qtgql/codegen/py/objecttype.py` & `qtgql-0.117.0/qtgqlcodegen/objecttype.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,19 +10,20 @@
 from typing import TypeVar
 
 import attrs
 from attrs import define
 from typingref import TypeHinter
 from typingref import UNSET
 
-from qtgql.codegen.py.compiler.builtin_scalars import BuiltinScalar
-from qtgql.codegen.py.runtime.bases import QGraphQListModel
-from qtgql.codegen.py.runtime.custom_scalars import BaseCustomScalar
-from qtgql.codegen.py.runtime.custom_scalars import CustomScalarMap
-from qtgql.codegen.utils import AntiForwardRef
+from qtgqlcodegen.compiler.builtin_scalars import BuiltinScalar
+from qtgqlcodegen.compiler.operation import QtGqlQueriedObjectType
+from qtgqlcodegen.cppref import QtGqlTypes
+from qtgqlcodegen.runtime.custom_scalars import BaseCustomScalar
+from qtgqlcodegen.runtime.custom_scalars import CustomScalarMap
+from qtgqlcodegen.utils import AntiForwardRef
 
 
 class Kinds(enum.Enum):
     SCALAR = "SCALAR"
     OBJECT = "OBJECT"
     ENUM = "ENUM"
     LIST = "LIST"
@@ -136,24 +137,28 @@
                 or self.type.is_object_type
                 or self.type.is_interface
                 or self.type.is_union
             )
             return "QObject"
 
     @cached_property
+    def getter_name(self) -> str:
+        return f"get_{self.name}"
+
+    @cached_property
     def setter_name(self) -> str:
-        return self.name + "_setter"
+        return f"{self.name}_setter"
 
     @cached_property
     def signal_name(self) -> str:
-        return self.name + "Changed"
+        return f"{self.name}Changed"
 
     @cached_property
     def private_name(self) -> str:
-        return "_" + self.name
+        return f"m_{self.name}"
 
     @property
     def fget(self) -> str:
         if self.type.is_custom_scalar:
             return f"return self.{self.private_name}.{BaseCustomScalar.to_qt.__name__}()"
         if self.type.is_enum:
             return f"return self.{self.private_name}.value"
@@ -259,14 +264,20 @@
         with contextlib.suppress(TypeError):
             if issubclass(t_self, AntiForwardRef):
                 ret = t_self.resolve()
                 if isinstance(ret, QtGqlObjectTypeDefinition):
                     return ret
 
     @cached_property
+    def is_queried_object_type(self) -> Optional[QtGqlQueriedObjectType]:
+        t_self = self.optional_maybe.type
+        if isinstance(t_self, QtGqlQueriedObjectType):
+            return t_self
+
+    @cached_property
     def is_input_object_type(self) -> Optional[QtGqlInputObjectTypeDefinition]:
         t_self = self.optional_maybe.type
         if isinstance(t_self, QtGqlInputObjectTypeDefinition):
             return t_self
 
     @cached_property
     def is_model(self) -> Optional[GqlTypeHinter]:
@@ -309,26 +320,28 @@
         this goes for init and the property setter. They are optional by default,
         (at the template) so unwrap optional first
         """
         t_self = self.optional_maybe
 
         # int, str, float etc...
         if builtin_scalar := t_self.is_builtin_scalar:
-            return builtin_scalar.tp.__name__
+            return builtin_scalar.tp
 
         if scalar := t_self.is_custom_scalar:
             return f"SCALARS.{scalar.__name__}"
         if gql_enum := t_self.is_enum:
             return gql_enum.name
         if model_of := t_self.is_model:
-            return f"{QGraphQListModel.__name__}[{model_of.annotation}]"
+            return f"{QtGqlTypes.QGraphQLList.name}[{model_of.annotation}]"
         if object_def := t_self.is_object_type or t_self.is_interface:
-            return f"Optional[{object_def.name}]"
+            return f"{object_def.name}"
+        if q_object_def := t_self.is_queried_object_type:
+            return f"{q_object_def.name}"
         if t_self.is_union:
-            return "Union[" + ", ".join(th.annotation for th in t_self.of_type) + "]"
+            return "std::variant<" + ", ".join(th.annotation for th in t_self.of_type) + ">"
         if input_obj := t_self.is_input_object_type:
             return input_obj.name
 
         raise NotImplementedError  # pragma no cover
 
     def as_annotation(self, object_map=None):  # pragma: no cover
         raise NotImplementedError("not safe to call on this type")
```

### Comparing `qtgql-0.116.1/qtgql/codegen/py/runtime/custom_scalars.py` & `qtgql-0.117.0/qtgqlcodegen/runtime/custom_scalars.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.116.1/qtgql/codegen/py/runtime/queryhandler.py` & `qtgql-0.117.0/qtgqlcodegen/runtime/queryhandler.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,20 +10,20 @@
 from typing import TYPE_CHECKING
 from typing import TypeVar
 
 from PySide6.QtCore import QObject
 from PySide6.QtCore import Signal
 from PySide6.QtQuick import QQuickItem
 
-from qtgql.codegen.py.runtime.environment import get_gql_env
-from qtgql.tools import qproperty
-from qtgql.tools import slot
+from qtgqlcodegen.py.runtime.environment import get_gql_env
+from qtgqlcodegen.tools import qproperty
+from qtgqlcodegen.tools import slot
 
 if TYPE_CHECKING:
-    from qtgql.gqltransport.client import GqlClientMessage
+    from qtgqlcodegen.gqltransport.client import GqlClientMessage
 
 T_QObject = TypeVar("T_QObject", bound=QObject)
 
 
 class SelectionConfig(NamedTuple):
     selections: Dict[str, Optional[SelectionConfig]] = {}
     choices: Dict[str, SelectionConfig] = {}
```

### Comparing `qtgql-0.116.1/qtgql/codegen/py/templates/config.jinja.py` & `qtgql-0.117.0/qtgqlcodegen/templates/config.jinja.hpp`

 * *Files 19% similar despite different names*

```diff
@@ -1,16 +1,15 @@
-{% if context.selections or context.choices %}SelectionConfig(
-    selections={
+{% if context.selections or context.choices %}
+    {
         {% for name, selection in context.selections.items() %}
-        "{{name}}": {%if selection %} {{selection}} {% else %} None {% endif %},{% endfor %}
+                {"👉name👈", {%if selection %} 👉selection👈 {% else %} {} {% endif %}},{% endfor %}
     },
 {% if context.choices %}
 choices={
 {% for choice_name, selections in context.choices.items() %}
-    "{{choice_name}}": SelectionConfig(selections={
-                       {% for field_name, inner_template in selections.items() %} "{{field_name}}": {{inner_template}}, {% endfor %}
-}),
+    "👉choice_name👈": {
+                       {% for field_name, inner_template in selections.items() %} {"👉field_name👈", 👉inner_template👈}, {% endfor %}
+}
 {% endfor %}
 }
 {% endif %}
-)
 {% endif %}
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `qtgql-0.116.1/PKG-INFO` & `qtgql-0.117.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 Metadata-Version: 2.1
 Name: qtgql
-Version: 0.116.1
+Version: 0.117.0
 Summary: Qt framework for building graphql driven QML applications
 License: MIT
 Author: Nir
 Author-email: 88795475+nrbnlulu@users.noreply.github.com
 Maintainer: Nir.J Benlulu
 Maintainer-email: nrbnlulu@gmail.com
 Requires-Python: >=3.9,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Provides-Extra: codegen
-Requires-Dist: PySide6 (>=6.4.2,<7.0.0)
 Requires-Dist: attrs (>=22.2.0,<23.0.0)
-Requires-Dist: graphql-core (<3.3.0) ; extra == "codegen"
-Requires-Dist: jinja2 (>=3.1.2,<4.0.0) ; extra == "codegen"
-Requires-Dist: toml (>=0.10.2,<0.11.0) ; extra == "codegen"
-Requires-Dist: typer[all] (>=0.7.0,<0.8.0) ; extra == "codegen"
+Requires-Dist: frozendict (>=2.3.8,<3.0.0)
+Requires-Dist: graphql-core (>=3.2.3,<4.0.0)
+Requires-Dist: jinja2 (>=3.1.2,<4.0.0)
+Requires-Dist: rich (>=13.3.5,<14.0.0)
+Requires-Dist: typer (>=0.9.0,<0.10.0)
 Requires-Dist: typingref (>=0.100.0,<0.101.0)
 Project-URL: Documentation, https://nrbnlulu.github.io/qtgql/
 Project-URL: Homepage, https://github.com/nrbnlulu/qtgql
 Description-Content-Type: text/markdown
 
 ###  Qt framework for building graphql driven QML applications
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/qtgql?style=for-the-badge)](https://pypi.org/project/qtgql/)
@@ -34,35 +33,26 @@
 [![Discord](https://img.shields.io/discord/1067870318301032558?label=discord&style=for-the-badge)](https://discord.gg/5vmRRJp9fu)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/qtgql?style=for-the-badge)
 
 ### Disclaimer
 This project is currently under development, and **it is not** production ready,
 You can play-around and tell us what is wrong / missing / awesome :smile:.
 
-[Visit the docs for more info](https://nrbnlulu.github.io/qtgql/)
+[Visit the docs for more info](https://nrbnlulu.github.io/qtgql/) (WIP)
 
 
 ### Features
-- [x] object types, for each field there is a corresponding `Property`
-- [x] enums
-- [x] custom scalars
-- [x] Unions
-- [x] interfaces
-- [x] Garbage collection
-- [x] Type-safe Mutation handlers
-- [x] Type-safe Query handlers: queries your server when a component uses this query (or imperatively fetched).
-- [x] Query updates: fetch the same query multiple times would not instantiate everything from scratch
+- [ ] object types, for each field there is a corresponding `Property`
+- [ ] enums
+- [ ] custom scalars
+- [ ] Unions
+- [ ] interfaces
+- [ ] Garbage collection
+- [ ] Type-safe Mutation handlers
+- [ ] Type-safe Query handlers: queries your server when a component uses this query (or imperatively fetched).
+- [ ] Query updates: fetch the same query multiple times would not instantiate everything from scratch
 it would compare the current data with data received and emit __only__ the signals that are needed.
 - [x] Native-Qt client implementation of "[graphql-transport-ws](https://github.com/enisdenjo/graphql-ws/blob/master/PROTOCOL.md)" protocol (supports subscriptions) - You can provide your own network layer though.
-- [x] Mutations.
-- [x] Subscriptions.
-- [x] Fully typed input variables.
-
-#### Helpers
-- [x] generic models that get created from dictionaries (with update, pop, insert implemented by default)
-- [x] `Property` classes that are accessible from QML, with dataclasses  syntax (using attrs)
-- [x] `@slot` - decorator to be replaced with `QtCore.Slot()` that get types from type hints.
-
-### TODO
-- Migrate to C++
-- Fragments?
+- [ ] Mutations.
+- [ ] Subscriptions.
+- [ ] Fully typed input variables.
```

