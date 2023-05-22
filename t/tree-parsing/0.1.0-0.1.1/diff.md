# Comparing `tmp/tree_parsing-0.1.0.tar.gz` & `tmp/tree_parsing-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tree_parsing-0.1.0.tar", max compression
+gzip compressed data, was "tree_parsing-0.1.1.tar", max compression
```

## Comparing `tree_parsing-0.1.0.tar` & `tree_parsing-0.1.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1090 2023-05-09 21:22:25.678206 tree_parsing-0.1.0/LICENSE
--rw-r--r--   0        0        0     1241 2023-05-20 15:11:23.870495 tree_parsing-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     4901 2023-05-20 15:11:37.953749 tree_parsing-0.1.0/README.md
--rw-r--r--   0        0        0       23 2023-05-20 13:37:44.796675 tree_parsing-0.1.0/tree_parsing/__init__.py
--rw-r--r--   0        0        0     3377 2023-05-20 13:35:55.043354 tree_parsing-0.1.0/tree_parsing/tree.py
--rw-r--r--   0        0        0     5664 1970-01-01 00:00:00.000000 tree_parsing-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1090 2023-05-09 21:22:25.678206 tree_parsing-0.1.1/LICENSE
+-rw-r--r--   0        0        0     1241 2023-05-22 01:47:09.855788 tree_parsing-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     4901 2023-05-20 15:11:37.953749 tree_parsing-0.1.1/README.md
+-rw-r--r--   0        0        0       23 2023-05-20 13:37:44.796675 tree_parsing-0.1.1/tree_parsing/__init__.py
+-rw-r--r--   0        0        0     3483 2023-05-22 01:48:28.959854 tree_parsing-0.1.1/tree_parsing/tree.py
+-rw-r--r--   0        0        0     5664 1970-01-01 00:00:00.000000 tree_parsing-0.1.1/PKG-INFO
```

### Comparing `tree_parsing-0.1.0/LICENSE` & `tree_parsing-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tree_parsing-0.1.0/pyproject.toml` & `tree_parsing-0.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tree-parsing"
-version = "0.1.0"
+version = "0.1.1"
 description = "library to work with tree and lists"
 license = "MIT"
 authors = ["Jorge Silva <jorgesilva.ti@hotmail.com>"]
 maintainers = ["Jorge Silva <jorgesilva.ti@hotmail.com>"]
 readme = "README.md"
 repository = "https://github.com/scjorge/tree-parsing"
 documentation = "https://tree-parsing.readthedocs.io/en/latest/"
```

### Comparing `tree_parsing-0.1.0/README.md` & `tree_parsing-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `tree_parsing-0.1.0/tree_parsing/tree.py` & `tree_parsing-0.1.1/tree_parsing/tree.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,14 +27,17 @@
     ) -> None:
         flow = f"{parent_number}-{child_number + 1}"
         node[self._flow_key] = flow
 
     def new_node(self, node: Dict) -> None:
         return
 
+    def new_node_list(self, node: Dict) -> None:
+        return
+
 
 class Tree(BaseTree, MixinTree):
     def __init__(
         self,
         id_key: str = "id",
         parent_key: str = "parent",
         parent_start: Any = "0",
@@ -69,14 +72,15 @@
         for tree in local_record_list:
             self._build_list(tree)
         return self._final_tree
 
     def _build_list(self, tree):
         tree_new = [tree]
         for node in tree_new:
+            self.new_node_list(node)
             item = deepcopy(node)
             item.pop(self._child_key, None)
             self._final_tree.append(item)
             if self._child_key in node and node[self._child_key]:
                 for child in node[self._child_key]:
                     self._build_list(child)
```

### Comparing `tree_parsing-0.1.0/PKG-INFO` & `tree_parsing-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tree-parsing
-Version: 0.1.0
+Version: 0.1.1
 Summary: library to work with tree and lists
 Home-page: https://github.com/scjorge/tree-parsing
 License: MIT
 Keywords: node,tree,json,json-schema,hints,parsin,parsing,workflow
 Author: Jorge Silva
 Author-email: jorgesilva.ti@hotmail.com
 Maintainer: Jorge Silva
```

