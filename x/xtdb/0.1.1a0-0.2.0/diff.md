# Comparing `tmp/xtdb-0.1.1a0.tar.gz` & `tmp/xtdb-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xtdb-0.1.1a0.tar", max compression
+gzip compressed data, was "xtdb-0.2.0.tar", max compression
```

## Comparing `xtdb-0.1.1a0.tar` & `xtdb-0.2.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0    13827 2023-05-19 16:06:23.580008 xtdb-0.1.1a0/LICENSE
--rw-r--r--   0        0        0     2708 2023-05-19 16:06:23.580008 xtdb-0.1.1a0/README.md
--rw-r--r--   0        0        0     1582 2023-05-19 16:06:23.580008 xtdb-0.1.1a0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-19 16:06:23.580008 xtdb-0.1.1a0/xtdb/__init__.py
--rw-r--r--   0        0        0      240 2023-05-19 16:06:23.580008 xtdb-0.1.1a0/xtdb/__main__.py
--rw-r--r--   0        0        0      165 2023-05-19 16:06:23.580008 xtdb-0.1.1a0/xtdb/exceptions.py
--rw-r--r--   0        0        0     1857 2023-05-19 16:06:23.580008 xtdb-0.1.1a0/xtdb/orm.py
--rw-r--r--   0        0        0     5620 2023-05-19 16:06:23.580008 xtdb-0.1.1a0/xtdb/query.py
--rw-r--r--   0        0        0     7140 2023-05-19 16:06:23.580008 xtdb-0.1.1a0/xtdb/session.py
--rw-r--r--   0        0        0     3404 1970-01-01 00:00:00.000000 xtdb-0.1.1a0/PKG-INFO
+-rw-r--r--   0        0        0    13827 2023-05-22 07:17:23.468748 xtdb-0.2.0/LICENSE
+-rw-r--r--   0        0        0     2749 2023-05-22 07:17:23.468748 xtdb-0.2.0/README.md
+-rw-r--r--   0        0        0     1581 2023-05-22 07:17:23.468748 xtdb-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-22 07:17:23.468748 xtdb-0.2.0/xtdb/__init__.py
+-rw-r--r--   0        0        0      232 2023-05-22 07:17:23.468748 xtdb-0.2.0/xtdb/__main__.py
+-rw-r--r--   0        0        0      165 2023-05-22 07:17:23.468748 xtdb-0.2.0/xtdb/exceptions.py
+-rw-r--r--   0        0        0     1857 2023-05-22 07:17:23.468748 xtdb-0.2.0/xtdb/orm.py
+-rw-r--r--   0        0        0     8079 2023-05-22 07:17:23.472748 xtdb-0.2.0/xtdb/query.py
+-rw-r--r--   0        0        0    11754 2023-05-22 07:17:23.472748 xtdb-0.2.0/xtdb/session.py
+-rw-r--r--   0        0        0     3443 1970-01-01 00:00:00.000000 xtdb-0.2.0/PKG-INFO
```

### Comparing `xtdb-0.1.1a0/LICENSE` & `xtdb-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `xtdb-0.1.1a0/README.md` & `xtdb-0.2.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 # XTDB Python
 
 A Python connector and ORM for XTDB.
 
+
 [![Code Integration](https://github.com/Donnype/xtdb-py/actions/workflows/tests.yml/badge.svg)](https://github.com/Donnype/xtdb-py/actions/workflows/tests.yml)
-[![Pypi release](https://github.com/Donnype/xtdb-py/actions/workflows/release.yml/badge.svg)](https://github.com/Donnype/xtdb-py/actions/workflows/release.yml)
+[![Stable Version](https://img.shields.io/pypi/v/xtdb?label=stable)](https://pypi.org/project/xtdb/#history)
+[![Python Versions](https://img.shields.io/pypi/pyversions/xtdb)](https://pypi.org/project/xtdb/)
+
 
 ## Installation
 
 ```bash
 pip install xtdb
 ```
 
@@ -55,17 +58,17 @@
 ```
 
 ### Using only the client
 
 ```python3
 import os
 
-from xtdb.session import XTDBHTTPClient, Operation
+from xtdb.session import XTDBClient, Operation
 
-client = XTDBHTTPClient(os.environ["XTDB_URI"])
+client = XTDBClient(os.environ["XTDB_URI"])
 client.submit_transaction([Operation.put({"xt/id": "123", "name": "fred"})])
 
 client.query('{:query {:find [(pull ?e [*])] :where [[ ?e :name "fred" ]]}}')
 client.get_entity("123")
 ```
 
 ### Using the CLI tool for querying
```

### Comparing `xtdb-0.1.1a0/pyproject.toml` & `xtdb-0.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "xtdb"
-version = "0.1.1a"
+version = "0.2.0"
 packages = [{ include = "xtdb" }]
 include  = ["xtdb/**"]
 exclude = [
     "**/.idea",
     "**/.git*",
     "**/.*ignore",
     "**/.flake8",
```

### Comparing `xtdb-0.1.1a0/xtdb/orm.py` & `xtdb-0.2.0/xtdb/orm.py`

 * *Files identical despite different names*

### Comparing `xtdb-0.1.1a0/xtdb/query.py` & `xtdb-0.2.0/xtdb/query.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,14 +2,19 @@
 from typing import List, Optional, Type, Union
 
 from xtdb.exceptions import InvalidField
 from xtdb.orm import TYPE_FIELD, Base
 
 
 @dataclass
+class Var:
+    val: str
+
+
+@dataclass
 class Query:
     """Object representing an XTDB query.
 
         result_type: Object being queried: executing the query should yield only this Object.
 
     Example usage:
 
@@ -26,48 +31,127 @@
 
     result_type: Type[Base]
 
     _where_clauses: List[str] = field(default_factory=list)
     _find_clauses: List[str] = field(default_factory=list)
     _limit: Optional[int] = None
     _offset: Optional[int] = None
+    _preserved_return_type: bool = True
 
     def where(self, object_type: Type[Base], **kwargs) -> "Query":
         for field_name, value in kwargs.items():
             self._where_field_is(object_type, field_name, value)
 
         return self
 
     def format(self) -> str:
         return self._compile(separator="\n    ")
 
-    def count(self, object_type: Type[Base]) -> "Query":
-        self._find_clauses.append(f"(count {object_type.alias()})")
+    def count(self, var: Union[Type[Base], Var]) -> "Query":
+        self._preserved_return_type = False
+
+        if isinstance(var, Var):
+            self._find_clauses.append(f"(count ?{var.val})")
+            return self
+
+        self._find_clauses.append(f"(count {var.alias()})")
+        return self
+
+    def avg(self, var: Var) -> "Query":
+        self._preserved_return_type = False
+        self._find_clauses.append(f"(avg ?{var.val})")
+
+        return self
+
+    def max(self, var: Var) -> "Query":
+        self._preserved_return_type = False
+        self._find_clauses.append(f"(max ?{var.val})")
+
+        return self
+
+    def min(self, var: Var) -> "Query":
+        self._preserved_return_type = False
+        self._find_clauses.append(f"(min ?{var.val})")
+
+        return self
+
+    def count_distinct(self, var: Var) -> "Query":
+        self._preserved_return_type = False
+        self._find_clauses.append(f"(count-distinct ?{var.val})")
+
+        return self
+
+    def sum(self, var: Var) -> "Query":
+        self._preserved_return_type = False
+        self._find_clauses.append(f"(sum ?{var.val})")
+
+        return self
+
+    def median(self, var: Var) -> "Query":
+        self._preserved_return_type = False
+        self._find_clauses.append(f"(median ?{var.val})")
+
+        return self
+
+    def variance(self, var: Var) -> "Query":
+        self._preserved_return_type = False
+        self._find_clauses.append(f"(variance ?{var.val})")
+
+        return self
+
+    def stddev(self, var: Var) -> "Query":
+        self._preserved_return_type = False
+        self._find_clauses.append(f"(stddev ?{var.val})")
+
+        return self
+
+    def distinct(self, var: Var) -> "Query":
+        self._preserved_return_type = False
+        self._find_clauses.append(f"(distinct ?{var.val})")
+
+        return self
+
+    def rand(self, var: Var, N: int) -> "Query":
+        self._preserved_return_type = False
+        self._find_clauses.append(f"(rand {N} ?{var.val})")
+
+        return self
+
+    def sample(self, var: Var, N: int) -> "Query":
+        self._preserved_return_type = False
+        self._find_clauses.append(f"(sample {N} ?{var.val})")
 
         return self
 
     def group_by(self, object_type: Type[Base]) -> "Query":
+        self._preserved_return_type = False
         self._find_clauses.append(f"{object_type.alias()}")
 
         return self
 
     def limit(self, limit: int) -> "Query":
         self._limit = limit
 
         return self
 
     def offset(self, offset: int) -> "Query":
         self._offset = offset
 
         return self
 
-    def _where_field_is(self, object_type: Type[Base], field_name: str, value: Union[Type[Base], str, None]) -> None:
+    def _where_field_is(
+        self, object_type: Type[Base], field_name: str, value: Union[Type[Base], Var, str, None]
+    ) -> None:
         if field_name not in object_type.fields():
             raise InvalidField(f'"{field_name}" is not a field of {object_type.alias()}')
 
+        if isinstance(value, Var):
+            self._add_where_statement(object_type, field_name, f"?{value.val}")
+            return
+
         if isinstance(value, str):
             value = value.replace('"', r"\"")
             self._add_where_statement(object_type, field_name, f'"{value}"')
             return
 
         if type(value) in [int, float, bool]:
             self._add_where_statement(object_type, field_name, f"{value}")
@@ -123,31 +207,33 @@
             return self._to_type_statement(object_type, object_type)
 
         return f"(or {' '.join([self._to_type_statement(object_type, x) for x in object_type.__subclasses__()])} )"
 
     def _to_type_statement(self, object_type: Type[Base], other_type: Type[Base]) -> str:
         return f'[ {object_type.alias()} :{TYPE_FIELD} "{other_type.alias()}" ]'
 
-    def _compile_where_clauses(self, *, separator=" ") -> str:
+    def _compile_where_clauses(self, where_clauses: List[str], *, separator=" ") -> str:
         """Sorted and deduplicated where clauses, since they are both idempotent and commutative"""
 
-        return separator + separator.join(sorted(set(self._where_clauses)))
+        return separator + separator.join(sorted(set(where_clauses)))
 
-    def _compile_find_clauses(self) -> str:
-        return " ".join(self._find_clauses)
+    def _compile_find_clauses(self, find_clauses: List[str]) -> str:
+        return " ".join(find_clauses)
 
     def _compile(self, *, separator=" ") -> str:
-        self._where_clauses.append(self._assert_type(self.result_type))
-        where_clauses = self._compile_where_clauses(separator=separator)
+        where_clauses = self._where_clauses
+        where_clauses.append(self._assert_type(self.result_type))
 
         if not self._find_clauses:
-            self._find_clauses = [f"(pull {self.result_type.alias()} [*])"]
+            find_clauses = self._compile_find_clauses([f"(pull {self.result_type.alias()} [*])"])
+        else:
+            find_clauses = self._compile_find_clauses(self._find_clauses)
 
-        find_clauses = self._compile_find_clauses()
-        compiled = f"{{:query {{:find [{find_clauses}] :where [{where_clauses}]"
+        compiled_where_clauses = self._compile_where_clauses(where_clauses, separator=separator)
+        compiled = f"{{:query {{:find [{find_clauses}] :where [{compiled_where_clauses}]"
 
         if self._limit is not None:
             compiled += f" :limit {self._limit}"
 
         if self._offset is not None:
             compiled += f" :offset {self._offset}"
```

### Comparing `xtdb-0.1.1a0/PKG-INFO` & `xtdb-0.2.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xtdb
-Version: 0.1.1a0
+Version: 0.2.0
 Summary: A Python connector and ORM for XTDB.
 Home-page: https://github.com/Donnype/xtdb-py
 Author: Donny Peeters
 Author-email: donny.peeters@hotmail.com
 Maintainer: Donny Peeters
 Maintainer-email: donny.peeters@hotmail.com
 Requires-Python: >=3.8,<4.0
@@ -17,16 +17,19 @@
 Project-URL: Repository, https://github.com/Donnype/xtdb-py
 Description-Content-Type: text/markdown
 
 # XTDB Python
 
 A Python connector and ORM for XTDB.
 
+
 [![Code Integration](https://github.com/Donnype/xtdb-py/actions/workflows/tests.yml/badge.svg)](https://github.com/Donnype/xtdb-py/actions/workflows/tests.yml)
-[![Pypi release](https://github.com/Donnype/xtdb-py/actions/workflows/release.yml/badge.svg)](https://github.com/Donnype/xtdb-py/actions/workflows/release.yml)
+[![Stable Version](https://img.shields.io/pypi/v/xtdb?label=stable)](https://pypi.org/project/xtdb/#history)
+[![Python Versions](https://img.shields.io/pypi/pyversions/xtdb)](https://pypi.org/project/xtdb/)
+
 
 ## Installation
 
 ```bash
 pip install xtdb
 ```
 
@@ -74,17 +77,17 @@
 ```
 
 ### Using only the client
 
 ```python3
 import os
 
-from xtdb.session import XTDBHTTPClient, Operation
+from xtdb.session import XTDBClient, Operation
 
-client = XTDBHTTPClient(os.environ["XTDB_URI"])
+client = XTDBClient(os.environ["XTDB_URI"])
 client.submit_transaction([Operation.put({"xt/id": "123", "name": "fred"})])
 
 client.query('{:query {:find [(pull ?e [*])] :where [[ ?e :name "fred" ]]}}')
 client.get_entity("123")
 ```
 
 ### Using the CLI tool for querying
```

