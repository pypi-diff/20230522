# Comparing `tmp/AkvoResponseGrouper-1.3.1a0.tar.gz` & `tmp/AkvoResponseGrouper-1.3.2a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AkvoResponseGrouper-1.3.1a0.tar", last modified: Tue May  9 06:05:26 2023, max compression
+gzip compressed data, was "AkvoResponseGrouper-1.3.2a0.tar", last modified: Mon May 22 13:39:30 2023, max compression
```

## Comparing `AkvoResponseGrouper-1.3.1a0.tar` & `AkvoResponseGrouper-1.3.2a0.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 06:05:26.497058 AkvoResponseGrouper-1.3.1a0/
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-05-09 06:05:17.000000 AkvoResponseGrouper-1.3.1a0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-05-09 06:05:17.000000 AkvoResponseGrouper-1.3.1a0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4944 2023-05-09 06:05:26.497058 AkvoResponseGrouper-1.3.1a0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3759 2023-05-09 06:05:17.000000 AkvoResponseGrouper-1.3.1a0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-09 06:05:17.000000 AkvoResponseGrouper-1.3.1a0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-05-09 06:05:26.497058 AkvoResponseGrouper-1.3.1a0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-05-09 06:05:17.000000 AkvoResponseGrouper-1.3.1a0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 06:05:26.493058 AkvoResponseGrouper-1.3.1a0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 06:05:26.493058 AkvoResponseGrouper-1.3.1a0/src/AkvoResponseGrouper/
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-09 06:05:17.000000 AkvoResponseGrouper-1.3.1a0/src/AkvoResponseGrouper/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 06:05:26.497058 AkvoResponseGrouper-1.3.1a0/src/AkvoResponseGrouper/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 06:05:17.000000 AkvoResponseGrouper-1.3.1a0/src/AkvoResponseGrouper/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5394 2023-05-09 06:05:17.000000 AkvoResponseGrouper-1.3.1a0/src/AkvoResponseGrouper/cli/checker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-05-09 06:05:17.000000 AkvoResponseGrouper-1.3.1a0/src/AkvoResponseGrouper/cli/checker_db.py
--rw-r--r--   0 runner    (1001) docker     (123)     3050 2023-05-09 06:05:17.000000 AkvoResponseGrouper-1.3.1a0/src/AkvoResponseGrouper/cli/generate_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     3667 2023-05-09 06:05:17.000000 AkvoResponseGrouper-1.3.1a0/src/AkvoResponseGrouper/cli/migrate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1867 2023-05-09 06:05:17.000000 AkvoResponseGrouper-1.3.1a0/src/AkvoResponseGrouper/db.py
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-05-09 06:05:17.000000 AkvoResponseGrouper-1.3.1a0/src/AkvoResponseGrouper/models.py
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-05-09 06:05:17.000000 AkvoResponseGrouper-1.3.1a0/src/AkvoResponseGrouper/response_grouper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-05-09 06:05:17.000000 AkvoResponseGrouper-1.3.1a0/src/AkvoResponseGrouper/routes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 06:05:26.497058 AkvoResponseGrouper-1.3.1a0/src/AkvoResponseGrouper/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 06:05:17.000000 AkvoResponseGrouper-1.3.1a0/src/AkvoResponseGrouper/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-05-09 06:05:17.000000 AkvoResponseGrouper-1.3.1a0/src/AkvoResponseGrouper/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-05-09 06:05:17.000000 AkvoResponseGrouper-1.3.1a0/src/AkvoResponseGrouper/tests/test_lib_01_route.py
--rw-r--r--   0 runner    (1001) docker     (123)     3922 2023-05-09 06:05:17.000000 AkvoResponseGrouper-1.3.1a0/src/AkvoResponseGrouper/tests/test_lib_02_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4847 2023-05-09 06:05:17.000000 AkvoResponseGrouper-1.3.1a0/src/AkvoResponseGrouper/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-05-09 06:05:17.000000 AkvoResponseGrouper-1.3.1a0/src/AkvoResponseGrouper/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 06:05:26.497058 AkvoResponseGrouper-1.3.1a0/src/AkvoResponseGrouper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4944 2023-05-09 06:05:26.000000 AkvoResponseGrouper-1.3.1a0/src/AkvoResponseGrouper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-09 06:05:26.000000 AkvoResponseGrouper-1.3.1a0/src/AkvoResponseGrouper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 06:05:26.000000 AkvoResponseGrouper-1.3.1a0/src/AkvoResponseGrouper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-09 06:05:26.000000 AkvoResponseGrouper-1.3.1a0/src/AkvoResponseGrouper.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-09 06:05:26.000000 AkvoResponseGrouper-1.3.1a0/src/AkvoResponseGrouper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-09 06:05:26.000000 AkvoResponseGrouper-1.3.1a0/src/AkvoResponseGrouper.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 06:05:26.497058 AkvoResponseGrouper-1.3.1a0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4968 2023-05-09 06:05:17.000000 AkvoResponseGrouper-1.3.1a0/tests/test_category_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-05-09 06:05:17.000000 AkvoResponseGrouper-1.3.1a0/tests/test_category_data_frame.py
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-05-09 06:05:17.000000 AkvoResponseGrouper-1.3.1a0/tests/test_example.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:39:30.062710 AkvoResponseGrouper-1.3.2a0/
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-05-22 13:39:14.000000 AkvoResponseGrouper-1.3.2a0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-05-22 13:39:14.000000 AkvoResponseGrouper-1.3.2a0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4944 2023-05-22 13:39:30.062710 AkvoResponseGrouper-1.3.2a0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3759 2023-05-22 13:39:14.000000 AkvoResponseGrouper-1.3.2a0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-22 13:39:14.000000 AkvoResponseGrouper-1.3.2a0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-05-22 13:39:30.062710 AkvoResponseGrouper-1.3.2a0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-05-22 13:39:14.000000 AkvoResponseGrouper-1.3.2a0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:39:30.058710 AkvoResponseGrouper-1.3.2a0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:39:30.062710 AkvoResponseGrouper-1.3.2a0/src/AkvoResponseGrouper/
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-22 13:39:14.000000 AkvoResponseGrouper-1.3.2a0/src/AkvoResponseGrouper/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:39:30.062710 AkvoResponseGrouper-1.3.2a0/src/AkvoResponseGrouper/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 13:39:14.000000 AkvoResponseGrouper-1.3.2a0/src/AkvoResponseGrouper/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5394 2023-05-22 13:39:14.000000 AkvoResponseGrouper-1.3.2a0/src/AkvoResponseGrouper/cli/checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-05-22 13:39:14.000000 AkvoResponseGrouper-1.3.2a0/src/AkvoResponseGrouper/cli/checker_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3050 2023-05-22 13:39:14.000000 AkvoResponseGrouper-1.3.2a0/src/AkvoResponseGrouper/cli/generate_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3667 2023-05-22 13:39:14.000000 AkvoResponseGrouper-1.3.2a0/src/AkvoResponseGrouper/cli/migrate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1867 2023-05-22 13:39:14.000000 AkvoResponseGrouper-1.3.2a0/src/AkvoResponseGrouper/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-05-22 13:39:14.000000 AkvoResponseGrouper-1.3.2a0/src/AkvoResponseGrouper/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-05-22 13:39:14.000000 AkvoResponseGrouper-1.3.2a0/src/AkvoResponseGrouper/response_grouper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1967 2023-05-22 13:39:14.000000 AkvoResponseGrouper-1.3.2a0/src/AkvoResponseGrouper/routes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:39:30.062710 AkvoResponseGrouper-1.3.2a0/src/AkvoResponseGrouper/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 13:39:14.000000 AkvoResponseGrouper-1.3.2a0/src/AkvoResponseGrouper/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-05-22 13:39:14.000000 AkvoResponseGrouper-1.3.2a0/src/AkvoResponseGrouper/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-05-22 13:39:14.000000 AkvoResponseGrouper-1.3.2a0/src/AkvoResponseGrouper/tests/test_lib_01_route.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3922 2023-05-22 13:39:14.000000 AkvoResponseGrouper-1.3.2a0/src/AkvoResponseGrouper/tests/test_lib_02_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4847 2023-05-22 13:39:14.000000 AkvoResponseGrouper-1.3.2a0/src/AkvoResponseGrouper/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-05-22 13:39:14.000000 AkvoResponseGrouper-1.3.2a0/src/AkvoResponseGrouper/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:39:30.062710 AkvoResponseGrouper-1.3.2a0/src/AkvoResponseGrouper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4944 2023-05-22 13:39:29.000000 AkvoResponseGrouper-1.3.2a0/src/AkvoResponseGrouper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-22 13:39:30.000000 AkvoResponseGrouper-1.3.2a0/src/AkvoResponseGrouper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 13:39:29.000000 AkvoResponseGrouper-1.3.2a0/src/AkvoResponseGrouper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-22 13:39:29.000000 AkvoResponseGrouper-1.3.2a0/src/AkvoResponseGrouper.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-22 13:39:29.000000 AkvoResponseGrouper-1.3.2a0/src/AkvoResponseGrouper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-22 13:39:29.000000 AkvoResponseGrouper-1.3.2a0/src/AkvoResponseGrouper.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:39:30.062710 AkvoResponseGrouper-1.3.2a0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4968 2023-05-22 13:39:14.000000 AkvoResponseGrouper-1.3.2a0/tests/test_category_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-05-22 13:39:14.000000 AkvoResponseGrouper-1.3.2a0/tests/test_category_data_frame.py
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-05-22 13:39:14.000000 AkvoResponseGrouper-1.3.2a0/tests/test_example.py
```

### Comparing `AkvoResponseGrouper-1.3.1a0/LICENSE` & `AkvoResponseGrouper-1.3.2a0/LICENSE`

 * *Files identical despite different names*

### Comparing `AkvoResponseGrouper-1.3.1a0/PKG-INFO` & `AkvoResponseGrouper-1.3.2a0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AkvoResponseGrouper
-Version: 1.3.1a0
+Version: 1.3.2a0
 Summary: Fast-API Response catalog for pre-computed query
 Home-page: https://github.com/akvo/Akvo-ResponseGrouper
 Author: Akvo
 Author-email: tech.consultancy@akvo.org
 Project-URL: Documentation, https://github.com/akvo/Akvo-ResponseGrouper
 Project-URL: Bug Reports, https://github.com/akvo/Akvo-ResponseGrouper/issues
 Project-URL: Source Code, https://github.com/akvo/Akvo-ResponseGrouper
```

### Comparing `AkvoResponseGrouper-1.3.1a0/README.md` & `AkvoResponseGrouper-1.3.2a0/README.md`

 * *Files identical despite different names*

### Comparing `AkvoResponseGrouper-1.3.1a0/setup.py` & `AkvoResponseGrouper-1.3.2a0/setup.py`

 * *Files identical despite different names*

### Comparing `AkvoResponseGrouper-1.3.1a0/src/AkvoResponseGrouper/cli/checker.py` & `AkvoResponseGrouper-1.3.2a0/src/AkvoResponseGrouper/cli/checker.py`

 * *Files identical despite different names*

### Comparing `AkvoResponseGrouper-1.3.1a0/src/AkvoResponseGrouper/cli/checker_db.py` & `AkvoResponseGrouper-1.3.2a0/src/AkvoResponseGrouper/cli/checker_db.py`

 * *Files identical despite different names*

### Comparing `AkvoResponseGrouper-1.3.1a0/src/AkvoResponseGrouper/cli/generate_schema.py` & `AkvoResponseGrouper-1.3.2a0/src/AkvoResponseGrouper/cli/generate_schema.py`

 * *Files identical despite different names*

### Comparing `AkvoResponseGrouper-1.3.1a0/src/AkvoResponseGrouper/cli/migrate.py` & `AkvoResponseGrouper-1.3.2a0/src/AkvoResponseGrouper/cli/migrate.py`

 * *Files identical despite different names*

### Comparing `AkvoResponseGrouper-1.3.1a0/src/AkvoResponseGrouper/db.py` & `AkvoResponseGrouper-1.3.2a0/src/AkvoResponseGrouper/db.py`

 * *Files identical despite different names*

### Comparing `AkvoResponseGrouper-1.3.1a0/src/AkvoResponseGrouper/models.py` & `AkvoResponseGrouper-1.3.2a0/src/AkvoResponseGrouper/models.py`

 * *Files identical despite different names*

### Comparing `AkvoResponseGrouper-1.3.1a0/src/AkvoResponseGrouper/routes.py` & `AkvoResponseGrouper-1.3.2a0/src/AkvoResponseGrouper/routes.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 async def get_index_category(
     form: Optional[int] = Query(default=None),
     name: Optional[str] = Query(default=None),
     category: Optional[str] = Query(default=None),
     data: Optional[str] = Query(default=None),
     session: Session = Depends(get_session),
 ):
+    data = data.split(",") if data else None
     res = get_categories(
         form=form, name=name, category=category, data=data, session=session
     )
     return res
 
 
 @collection_route.get(
```

### Comparing `AkvoResponseGrouper-1.3.1a0/src/AkvoResponseGrouper/tests/conftest.py` & `AkvoResponseGrouper-1.3.2a0/src/AkvoResponseGrouper/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `AkvoResponseGrouper-1.3.1a0/src/AkvoResponseGrouper/tests/test_lib_01_route.py` & `AkvoResponseGrouper-1.3.2a0/src/AkvoResponseGrouper/tests/test_lib_01_route.py`

 * *Files identical despite different names*

### Comparing `AkvoResponseGrouper-1.3.1a0/src/AkvoResponseGrouper/tests/test_lib_02_utils.py` & `AkvoResponseGrouper-1.3.2a0/src/AkvoResponseGrouper/tests/test_lib_02_utils.py`

 * *Files identical despite different names*

### Comparing `AkvoResponseGrouper-1.3.1a0/src/AkvoResponseGrouper/utils.py` & `AkvoResponseGrouper-1.3.2a0/src/AkvoResponseGrouper/utils.py`

 * *Files identical despite different names*

### Comparing `AkvoResponseGrouper-1.3.1a0/src/AkvoResponseGrouper/views.py` & `AkvoResponseGrouper-1.3.2a0/src/AkvoResponseGrouper/views.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,46 +1,51 @@
 from typing import List, Optional
+from sqlalchemy import func
 from sqlalchemy.orm import Session
 from .models import Category, CategoryDict
 from .utils import transform_categories_to_df, get_counted_category
 
 
-def get_data_categories(session: Session):
-    categories = session.query(Category).all()
+def get_data_categories(
+    session: Session,
+    form: Optional[int] = None,
+    name: Optional[str] = None,
+    data: Optional[List[int]] = None,
+):
+    queries = []
+    if form:
+        queries.append(Category.form == form)
+    if name:
+        queries.append(func.lower(Category.name) == name.lower())
+    if data:
+        queries.append(Category.data == data)
+    categories = session.query(Category).filter(*queries).all()
     categories = [c.serialize for c in categories]
     return categories
 
 
 def get_results(session: Session):
     categories = get_data_categories(session=session)
     return transform_categories_to_df(categories=categories)
 
 
 def get_categories(
     session: Session,
     form: Optional[int] = None,
     name: Optional[str] = None,
     category: Optional[str] = None,
-    data: Optional[str] = None,
+    data: Optional[List[int]] = None,
 ) -> List[CategoryDict]:
-    res = get_results(session=session)
-    queries = []
-    if form:
-        queries.append(f"form == {form}")
-    if name:
-        queries.append(f"name.str.lower() == '{name.lower()}'")
+    categories = get_data_categories(
+        session=session, form=form, name=name, data=data
+    )
+    df = transform_categories_to_df(categories=categories)
     if category:
-        queries.append(f"category.str.lower() == '{category.lower()}'")
-    if data:
-        data = [int(d) for d in data.split(",")]
-        queries.append("data.isin(@data).values")
-    if len(queries):
-        queries = " & ".join(queries)
-        res = res.query(queries)
-    return res.to_dict("records")
+        df = df.query(f"category.str.lower() == '{category.lower()}'")
+    return df.to_dict("records")
 
 
 def get_group_by_category(
     session: Session,
     category: Optional[str] = None,
     form: Optional[int] = None,
 ):
```

### Comparing `AkvoResponseGrouper-1.3.1a0/src/AkvoResponseGrouper.egg-info/PKG-INFO` & `AkvoResponseGrouper-1.3.2a0/src/AkvoResponseGrouper.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AkvoResponseGrouper
-Version: 1.3.1a0
+Version: 1.3.2a0
 Summary: Fast-API Response catalog for pre-computed query
 Home-page: https://github.com/akvo/Akvo-ResponseGrouper
 Author: Akvo
 Author-email: tech.consultancy@akvo.org
 Project-URL: Documentation, https://github.com/akvo/Akvo-ResponseGrouper
 Project-URL: Bug Reports, https://github.com/akvo/Akvo-ResponseGrouper/issues
 Project-URL: Source Code, https://github.com/akvo/Akvo-ResponseGrouper
```

### Comparing `AkvoResponseGrouper-1.3.1a0/src/AkvoResponseGrouper.egg-info/SOURCES.txt` & `AkvoResponseGrouper-1.3.2a0/src/AkvoResponseGrouper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `AkvoResponseGrouper-1.3.1a0/tests/test_category_checker.py` & `AkvoResponseGrouper-1.3.2a0/tests/test_category_checker.py`

 * *Files identical despite different names*

### Comparing `AkvoResponseGrouper-1.3.1a0/tests/test_category_data_frame.py` & `AkvoResponseGrouper-1.3.2a0/tests/test_category_data_frame.py`

 * *Files identical despite different names*

