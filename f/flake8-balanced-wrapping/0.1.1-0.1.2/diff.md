# Comparing `tmp/flake8-balanced-wrapping-0.1.1.tar.gz` & `tmp/flake8-balanced-wrapping-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flake8-balanced-wrapping-0.1.1.tar", last modified: Sun Feb 26 16:46:46 2023, max compression
+gzip compressed data, was "flake8-balanced-wrapping-0.1.2.tar", last modified: Mon May 22 21:37:46 2023, max compression
```

## Comparing `flake8-balanced-wrapping-0.1.1.tar` & `flake8-balanced-wrapping-0.1.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-02-26 16:46:46.850028 flake8-balanced-wrapping-0.1.1/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11339 2023-02-26 16:46:37.000000 flake8-balanced-wrapping-0.1.1/LICENSE
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2256 2023-02-26 16:46:46.850028 flake8-balanced-wrapping-0.1.1/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1242 2023-02-26 16:46:37.000000 flake8-balanced-wrapping-0.1.1/README.md
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-02-26 16:46:46.850028 flake8-balanced-wrapping-0.1.1/flake8_balanced_wrapping.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2256 2023-02-26 16:46:46.000000 flake8-balanced-wrapping-0.1.1/flake8_balanced_wrapping.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)      354 2023-02-26 16:46:46.000000 flake8-balanced-wrapping-0.1.1/flake8_balanced_wrapping.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-02-26 16:46:46.000000 flake8-balanced-wrapping-0.1.1/flake8_balanced_wrapping.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       79 2023-02-26 16:46:46.000000 flake8-balanced-wrapping-0.1.1/flake8_balanced_wrapping.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       35 2023-02-26 16:46:46.000000 flake8-balanced-wrapping-0.1.1/flake8_balanced_wrapping.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       25 2023-02-26 16:46:46.000000 flake8-balanced-wrapping-0.1.1/flake8_balanced_wrapping.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9402 2023-02-26 16:46:37.000000 flake8-balanced-wrapping-0.1.1/flake8_balanced_wrapping.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      956 2023-02-26 16:46:46.850028 flake8-balanced-wrapping-0.1.1/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1602 2023-02-26 16:46:37.000000 flake8-balanced-wrapping-0.1.1/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-22 21:37:46.653696 flake8-balanced-wrapping-0.1.2/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11339 2023-05-22 21:37:35.000000 flake8-balanced-wrapping-0.1.2/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2256 2023-05-22 21:37:46.657696 flake8-balanced-wrapping-0.1.2/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1242 2023-05-22 21:37:35.000000 flake8-balanced-wrapping-0.1.2/README.md
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-22 21:37:46.653696 flake8-balanced-wrapping-0.1.2/flake8_balanced_wrapping.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2256 2023-05-22 21:37:46.000000 flake8-balanced-wrapping-0.1.2/flake8_balanced_wrapping.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      354 2023-05-22 21:37:46.000000 flake8-balanced-wrapping-0.1.2/flake8_balanced_wrapping.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-05-22 21:37:46.000000 flake8-balanced-wrapping-0.1.2/flake8_balanced_wrapping.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       79 2023-05-22 21:37:46.000000 flake8-balanced-wrapping-0.1.2/flake8_balanced_wrapping.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       53 2023-05-22 21:37:46.000000 flake8-balanced-wrapping-0.1.2/flake8_balanced_wrapping.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       25 2023-05-22 21:37:46.000000 flake8-balanced-wrapping-0.1.2/flake8_balanced_wrapping.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11406 2023-05-22 21:37:35.000000 flake8-balanced-wrapping-0.1.2/flake8_balanced_wrapping.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1005 2023-05-22 21:37:46.657696 flake8-balanced-wrapping-0.1.2/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1631 2023-05-22 21:37:35.000000 flake8-balanced-wrapping-0.1.2/setup.py
```

### Comparing `flake8-balanced-wrapping-0.1.1/LICENSE` & `flake8-balanced-wrapping-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `flake8-balanced-wrapping-0.1.1/PKG-INFO` & `flake8-balanced-wrapping-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flake8-balanced-wrapping
-Version: 0.1.1
+Version: 0.1.2
 Summary: A flake8 plugin that helps you wrap code with visual balance.
 Home-page: https://github.com/PeterJCLaw/flake8-balanced-wrapping
 Author: Peter Law
 Author-email: PeterJCLaw@gmail.com
 License: Apache 2.0
 Project-URL: Issue tracker, https://github.com/PeterJCLaw/flake8-balanced-wrapping/issues
 Platform: UNKNOWN
```

### Comparing `flake8-balanced-wrapping-0.1.1/README.md` & `flake8-balanced-wrapping-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `flake8-balanced-wrapping-0.1.1/flake8_balanced_wrapping.egg-info/PKG-INFO` & `flake8-balanced-wrapping-0.1.2/flake8_balanced_wrapping.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flake8-balanced-wrapping
-Version: 0.1.1
+Version: 0.1.2
 Summary: A flake8 plugin that helps you wrap code with visual balance.
 Home-page: https://github.com/PeterJCLaw/flake8-balanced-wrapping
 Author: Peter Law
 Author-email: PeterJCLaw@gmail.com
 License: Apache 2.0
 Project-URL: Issue tracker, https://github.com/PeterJCLaw/flake8-balanced-wrapping/issues
 Platform: UNKNOWN
```

### Comparing `flake8-balanced-wrapping-0.1.1/flake8_balanced_wrapping.py` & `flake8-balanced-wrapping-0.1.2/flake8_balanced_wrapping.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,38 +1,66 @@
 from __future__ import annotations
 
 import ast
 import sys
 import token
 import tokenize
+import itertools
 import collections
 import dataclasses
 from typing import cast, Iterable, Iterator, Collection, NamedTuple
+from typing_extensions import Protocol
 
 from tuck.ast import Position, _last_token, _first_token
 from asttokens import ASTTokens
 from tuck.wrappers import expression_is_parenthesised
 
 
+class Error(Protocol):
+    @property
+    def position(self) -> Position:
+        ...
+
+    def __str__(self) -> str:
+        ...
+
+
 @dataclasses.dataclass(frozen=True)
-class Error:
+class UnderWrappedError:
     node: ast.AST
     conflicts: list[Position]
 
     @property
     def position(self) -> Position:
         return self.conflicts[0]
 
     def __str__(self) -> str:
         return (
             f"BWR001 {type(self.node).__name__} is wrapped badly - {len(self.conflicts)} "
             "elements on the same line"
         )
 
 
+@dataclasses.dataclass(frozen=True)
+class OverWrappedError:
+    node: ast.AST
+    positions: list[Position]
+
+    @property
+    def position(self) -> Position:
+        return self.positions[0]
+
+    def __str__(self) -> str:
+        lines = set(x.line for x in self.positions)
+        return (
+            f"BWR002 {type(self.node).__name__} is wrapped unexpectedly over "
+            f"{len(lines)} lines"
+        )
+
+
 class PositionsSummary(NamedTuple):
     is_single_line_or_column: bool
     most_common_line_number: int
 
 
 def get_start_position(node: ast.AST) -> Position:
     return Position.from_node_start(node)
@@ -51,15 +79,15 @@
     return positions
 
 
 class Visitor(ast.NodeVisitor):
     def __init__(self, asttokens: ASTTokens) -> None:
         super().__init__()
         self.asttokens = asttokens
-        self.bad_nodes: dict[ast.AST, list[Position]] = {}
+        self.errors: list[Error] = []
 
     def _get_nodes_by_line_number(
         self,
         node: ast.AST,
         reference: Position,
         nodes: Collection[ast.AST],
         include_node_end: bool,
@@ -93,21 +121,26 @@
         counts = {x: len(y) for x, y in nodes_by_line_number.items()}
         (line_num, max_nodes_per_line), = collections.Counter(counts).most_common(1)
         return PositionsSummary(
             len(counts) == 1 or max_nodes_per_line == 1,
             line_num,
         )
 
-    def _record_error(self, node: ast.AST, nodes: list[ast.AST]) -> None:
+    def _record_error(
+        self,
+        node: ast.AST,
+        nodes: list[ast.AST],
+        error_type: type[UnderWrappedError] | type[OverWrappedError] = UnderWrappedError,
+    ) -> None:
         maybe_positions = [get_start_position(x) for x in nodes]
         positions = [x for x in maybe_positions if x is not None]
         assert positions
-        self.bad_nodes[node] = positions
+        self.errors.append(error_type(node, positions))
 
-    def _check_nodes(
+    def _check_under_wrapping(
         self,
         node: ast.AST,
         reference: Position,
         nodes: Collection[ast.AST],
         include_node_end: bool,
         include_node_start: bool = True,
     ) -> None:
@@ -126,15 +159,15 @@
 
     def visit_ClassDef(self, node: ast.ClassDef) -> None:
         nodes = [*node.bases, *node.keywords]
 
         class_tok = self.asttokens.find_token(_first_token(node), token.NAME, 'class')
         open_paren = self.asttokens.find_token(class_tok, token.OP, '(')
 
-        self._check_nodes(
+        self._check_under_wrapping(
             node,
             Position(*open_paren.end),
             nodes,
             include_node_end=False,
         )
         self.generic_visit(node)
 
@@ -152,27 +185,27 @@
 
         if sys.version_info >= (3, 8):
             nodes = [*node.args.posonlyargs, *nodes]
 
         def_tok = self.asttokens.find_token(_first_token(node), token.NAME, 'def')
         open_paren = self.asttokens.find_token(def_tok, token.OP, '(')
 
-        self._check_nodes(
+        self._check_under_wrapping(
             node,
             Position(*open_paren.end),
             [x for x in nodes if x],
             include_node_end=False,
         )
         self.generic_visit(node)
 
     visit_AsyncFunctionDef = visit_FunctionDef
 
     def visit_Call(self, node: ast.Call) -> None:
         open_paren = self.asttokens.find_token(_last_token(node.func), token.OP, '(')
-        self._check_nodes(
+        self._check_under_wrapping(
             node,
             Position(*open_paren.end),
             [*node.args, *node.keywords],
             include_node_end=True,
         )
         self.generic_visit(node)
 
@@ -238,48 +271,87 @@
 
     def visit_JoinedStr(self, node: ast.JoinedStr) -> None:
         # Position information in f-strings is a mess, so ASTTokens doesn't have
         # useful information, so we don't try either.
         return
 
     def visit_List(self, node: ast.List) -> None:
-        self._check_nodes(
+        self._check_under_wrapping(
             node,
             Position.from_node_start(node),
             node.elts,
             include_node_end=True,
         )
         self.generic_visit(node)
 
     def visit_Tuple(self, node: ast.Tuple) -> None:
         is_parenthesised = (
             _first_token(node).string == '(' and
             _last_token(node).string == ')'
         )
 
-        self._check_nodes(
+        self._check_under_wrapping(
             node,
             Position.from_node_start(node),
             node.elts,
             include_node_end=is_parenthesised,
             include_node_start=is_parenthesised,
         )
 
         self.generic_visit(node)
 
+    def _check_over_wrapping(
+        self,
+        node: ast.AST,
+        reference: Position,
+        nodes: Collection[ast.AST],
+        include_node_end: bool,
+        include_node_start: bool = True,
+    ) -> None:
+        by_line_no = self._get_nodes_by_line_number(
+            node,
+            reference,
+            nodes,
+            include_node_end=include_node_end,
+            include_node_start=include_node_start,
+        )
+
+        if len(by_line_no) != 1:
+            self._record_error(
+                node,
+                list(itertools.chain.from_iterable(by_line_no.values())),
+                error_type=OverWrappedError,
+            )
+
+    def visit_comprehension(self, node: ast.comprehension) -> None:
+        self._check_over_wrapping(
+            node,
+            Position.from_node_start(node),
+            [node.target, node.iter],
+            include_node_end=False,
+            include_node_start=False,
+        )
+        self.generic_visit(node)
+
+    def visit_Compare(self, node: ast.Compare) -> None:
+        self._check_over_wrapping(
+            node,
+            Position.from_node_start(node.left),
+            [node.left, *node.comparators],
+            include_node_end=True,
+            include_node_start=True,
+        )
+        self.generic_visit(node)
+
 
 def check(asttokens: ASTTokens) -> list[Error]:
     visitor = Visitor(asttokens)
     assert asttokens.tree  # placate mypy
     visitor.visit(asttokens.tree)
-
-    return [
-        Error(node, conflicts)
-        for node, conflicts in visitor.bad_nodes.items()
-    ]
+    return visitor.errors
 
 
 def flake8_balanced_wrapping(
     tree: ast.AST,
     file_tokens: list[tokenize.TokenInfo],
     lines: list[str],
 ) -> Iterator[tuple[int, int, str, None]]:
```

### Comparing `flake8-balanced-wrapping-0.1.1/setup.cfg` & `flake8-balanced-wrapping-0.1.2/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -7,25 +7,27 @@
 	.git,
 	.pybuild,
 	__pycache__,
 	build,
 	debian,
 	script
 ignore = 
+	C401
 	W504
 max_line_length = 95
 
 [isort]
 atomic = True
 balanced_wrapping = True
 combine_as_imports = True
 include_trailing_comma = True
 length_sort = True
 multi_line_output = 3
 order_by_type = False
+extra_standard_library = typing_extensions
 default_section = THIRDPARTY
 sections = FUTURE,STDLIB,THIRDPARTY,FIRSTPARTY,LOCALFOLDER
 
 [mypy]
 disallow_any_explicit = True
 disallow_any_generics = True
 disallow_subclassing_any = True
```

### Comparing `flake8-balanced-wrapping-0.1.1/setup.py` & `flake8-balanced-wrapping-0.1.2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from setuptools import setup
 
 long_description = (Path(__file__).parent / 'README.md').read_text()
 
 setup(
     name='flake8-balanced-wrapping',
-    version='0.1.1',
+    version='0.1.2',
     url='https://github.com/PeterJCLaw/flake8-balanced-wrapping',
     project_urls={
         'Issue tracker': 'https://github.com/PeterJCLaw/flake8-balanced-wrapping/issues',
     },
     description="A flake8 plugin that helps you wrap code with visual balance.",
     long_description=long_description,
     long_description_content_type='text/markdown',
@@ -44,9 +44,10 @@
     },
 
     install_requires=(
         'asttokens >=2.1.0, <3',
         # Don't really want to depend on tuck long-term, but for now it's an
         # easy thing to use.
         'tuck >=0.2, <0.3',
+        'typing-extensions',
     ),
 )
```

