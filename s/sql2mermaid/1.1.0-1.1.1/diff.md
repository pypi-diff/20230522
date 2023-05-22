# Comparing `tmp/sql2mermaid-1.1.0.tar.gz` & `tmp/sql2mermaid-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sql2mermaid-1.1.0.tar", max compression
+gzip compressed data, was "sql2mermaid-1.1.1.tar", max compression
```

## Comparing `sql2mermaid-1.1.0.tar` & `sql2mermaid-1.1.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1060 2023-04-04 11:16:22.644988 sql2mermaid-1.1.0/LICENSE.md
--rw-r--r--   0        0        0     1537 2023-04-07 18:27:39.373474 sql2mermaid-1.1.0/README.md
--rw-r--r--   0        0        0     1184 2023-04-11 08:40:45.495251 sql2mermaid-1.1.0/pyproject.toml
--rw-r--r--   0        0        0       71 2023-04-11 08:40:45.495766 sql2mermaid-1.1.0/sql2mermaid/__init__.py
--rw-r--r--   0        0        0      496 2023-04-06 13:15:37.128373 sql2mermaid-1.1.0/sql2mermaid/dependencies.py
--rw-r--r--   0        0        0     3277 2023-04-11 08:36:09.297910 sql2mermaid-1.1.0/sql2mermaid/main.py
--rw-r--r--   0        0        0      597 2023-04-06 13:37:41.942630 sql2mermaid-1.1.0/sql2mermaid/tables.py
--rw-r--r--   0        0        0      352 2023-04-11 08:36:09.298385 sql2mermaid-1.1.0/sql2mermaid/utils.py
--rw-r--r--   0        0        0     2184 1970-01-01 00:00:00.000000 sql2mermaid-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1060 2023-04-04 11:16:22.644988 sql2mermaid-1.1.1/LICENSE.md
+-rw-r--r--   0        0        0     1670 2023-05-22 15:24:21.992050 sql2mermaid-1.1.1/README.md
+-rw-r--r--   0        0        0      914 2023-05-22 15:26:43.823022 sql2mermaid-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0       71 2023-05-22 15:26:32.441919 sql2mermaid-1.1.1/sql2mermaid/__init__.py
+-rw-r--r--   0        0        0      496 2023-05-22 15:07:55.807416 sql2mermaid-1.1.1/sql2mermaid/dependencies.py
+-rw-r--r--   0        0        0     3204 2023-05-22 15:07:24.945900 sql2mermaid-1.1.1/sql2mermaid/main.py
+-rw-r--r--   0        0        0      597 2023-04-06 13:37:41.942630 sql2mermaid-1.1.1/sql2mermaid/tables.py
+-rw-r--r--   0        0        0      283 2023-05-22 15:07:24.946480 sql2mermaid-1.1.1/sql2mermaid/utils.py
+-rw-r--r--   0        0        0     2317 1970-01-01 00:00:00.000000 sql2mermaid-1.1.1/PKG-INFO
```

### Comparing `sql2mermaid-1.1.0/LICENSE.md` & `sql2mermaid-1.1.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `sql2mermaid-1.1.0/README.md` & `sql2mermaid-1.1.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -55,14 +55,22 @@
 
 ## Options
 
 You can change the name of the root and whether the FROM, JOIN clause is displayed.
 
 <img src="https://raw.githubusercontent.com/nkato/sql2mermaid/main/img/option-example.png" width="1200px">
 
+## How to Develop
+
+If you've installed Poetry on your machine, you can test it by doing the following:
+
+```shell
+poetry run tox
+```
+
 ## Author
 
 - [nkato](https://github.com/nkato)
 
 ## License
 
 This project is licensed under the MIT License - see the [LICENSE.md](https://github.com/nkato/sql2mermaid/blob/main/LICENSE.md) for details
```

### Comparing `sql2mermaid-1.1.0/sql2mermaid/main.py` & `sql2mermaid-1.1.1/sql2mermaid/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,18 +6,15 @@
 from .tables import Tables
 from .utils import is_pre_tables_mark, remove_quotes
 
 
 def is_ignorable(x: sqlparse.sql.Token) -> bool:
     if x.ttype in (sqlparse.tokens.Newline, sqlparse.tokens.Whitespace, sqlparse.tokens.Comment):
         return True
-    elif isinstance(x, sqlparse.sql.Comment) or "Comment" in str(x.ttype):
-        return True
-    else:
-        return False
+    return isinstance(x, sqlparse.sql.Comment) or "Comment" in str(x.ttype)
 
 
 def analyze_query(query: str, root_name: str) -> Tuple[Tables, Dependencies]:
     tables = Tables()
     tables.add(root_name)
     dependencies = Dependencies()
 
@@ -37,15 +34,15 @@
             current_indent_level -= 1
         elif token.ttype is sqlparse.tokens.Name and current_indent_level == 0 and is_in_with:  # Sub table
             table_name = remove_quotes(token.value)
             tables.add(table_name)
             current_table = table_name
         elif token.ttype is sqlparse.tokens.Keyword and is_pre_tables_mark(token.value, parsed[i - 3].value):  # FROM or JOIN
             table_name = remove_quotes(parsed[i + 1].value)
-            if not table_name == "(":
+            if table_name != "(":
                 tables.add(table_name)
                 dep = Dependency(current_table, token.value, table_name)
                 if dep not in dependencies:
                     dependencies.add(dep)
         elif token.ttype is sqlparse.tokens.Keyword.DML and token.value.upper() == "SELECT" and current_indent_level == 0:
             is_in_with = False
             current_table = root_name
@@ -60,15 +57,18 @@
         if dep.start in leafs:
             leafs.remove(dep.start)
             internals.add(dep.start)
     return internals, leafs
 
 
 def generate_mermaid(
-    internals: Tables, leafs: Tables, dependencies: Dependencies, display_join: Literal["none", "upper", "lower"]
+    internals: Tables,
+    leafs: Tables,
+    dependencies: Dependencies,
+    display_join: Literal["none", "upper", "lower"],
 ) -> str:
     res = "graph LR\n\n"
     for table in internals:
         res += f"{table}([{table}])\n"
 
     res += "\n"
     for table in leafs:
@@ -85,9 +85,8 @@
 
     return res
 
 
 def convert(query: str, *, root_name: str = "root", display_join: Literal["none", "upper", "lower"] = "none") -> str:
     tables, dependencies = analyze_query(query, root_name)
     internals, leafs = extract_leafs(tables, dependencies)
-    mermaid_text = generate_mermaid(internals, leafs, dependencies, display_join)
-    return mermaid_text
+    return generate_mermaid(internals, leafs, dependencies, display_join)
```

### Comparing `sql2mermaid-1.1.0/sql2mermaid/tables.py` & `sql2mermaid-1.1.1/sql2mermaid/tables.py`

 * *Files identical despite different names*

### Comparing `sql2mermaid-1.1.0/PKG-INFO` & `sql2mermaid-1.1.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sql2mermaid
-Version: 1.1.0
+Version: 1.1.1
 Summary: Convert SQL table dependencies to mermaid.js
 Home-page: https://github.com/nkato/sql2mermaid
 License: MIT
 Author: nkato
 Author-email: naokato.aq@gmail.com
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
@@ -73,14 +73,22 @@
 
 ## Options
 
 You can change the name of the root and whether the FROM, JOIN clause is displayed.
 
 <img src="https://raw.githubusercontent.com/nkato/sql2mermaid/main/img/option-example.png" width="1200px">
 
+## How to Develop
+
+If you've installed Poetry on your machine, you can test it by doing the following:
+
+```shell
+poetry run tox
+```
+
 ## Author
 
 - [nkato](https://github.com/nkato)
 
 ## License
 
 This project is licensed under the MIT License - see the [LICENSE.md](https://github.com/nkato/sql2mermaid/blob/main/LICENSE.md) for details
```

