# Comparing `tmp/flake8_django-1.2.tar.gz` & `tmp/flake8_django-1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flake8_django-1.2.tar", max compression
+gzip compressed data, was "flake8_django-1.3.tar", max compression
```

## Comparing `flake8_django-1.2.tar` & `flake8_django-1.3.tar`

### file list

```diff
@@ -1,16 +1,17 @@
--rw-r--r--   0        0        0     3393 2022-08-10 20:12:15.744827 flake8_django-1.2/README.md
--rw-r--r--   0        0        0       67 2022-08-10 20:12:15.744919 flake8_django-1.2/flake8_django/__init__.py
--rw-r--r--   0        0        0     2020 2022-08-10 20:12:15.744991 flake8_django-1.2/flake8_django/checker.py
--rw-r--r--   0        0        0      501 2022-08-10 20:12:15.745093 flake8_django-1.2/flake8_django/checkers/__init__.py
--rw-r--r--   0        0        0     1680 2022-08-10 20:12:15.745168 flake8_django-1.2/flake8_django/checkers/base_model_checker.py
--rw-r--r--   0        0        0      528 2022-08-10 20:12:15.745233 flake8_django-1.2/flake8_django/checkers/checker.py
--rw-r--r--   0        0        0      828 2022-08-10 20:12:15.745299 flake8_django-1.2/flake8_django/checkers/decorator.py
--rw-r--r--   0        0        0      504 2022-08-10 20:12:15.745364 flake8_django-1.2/flake8_django/checkers/issue.py
--rw-r--r--   0        0        0     3888 2022-08-10 20:12:15.745445 flake8_django-1.2/flake8_django/checkers/model_content_order.py
--rw-r--r--   0        0        0     1023 2022-08-10 20:12:15.745514 flake8_django-1.2/flake8_django/checkers/model_dunder_str.py
--rw-r--r--   0        0        0     1438 2022-08-10 20:12:15.745587 flake8_django-1.2/flake8_django/checkers/model_fields.py
--rw-r--r--   0        0        0     2134 2022-08-10 20:12:15.745661 flake8_django-1.2/flake8_django/checkers/model_form.py
--rw-r--r--   0        0        0     2378 2022-08-10 20:12:15.745725 flake8_django-1.2/flake8_django/checkers/model_meta.py
--rw-r--r--   0        0        0      731 2022-08-10 20:12:15.745787 flake8_django-1.2/flake8_django/checkers/render.py
--rw-r--r--   0        0        0      941 2023-04-15 10:01:06.825521 flake8_django-1.2/pyproject.toml
--rw-r--r--   0        0        0     4419 1970-01-01 00:00:00.000000 flake8_django-1.2/PKG-INFO
+-rw-r--r--   0        0        0     3393 2022-08-10 20:12:15.744827 flake8_django-1.3/README.md
+-rw-r--r--   0        0        0       67 2022-08-10 20:12:15.744919 flake8_django-1.3/flake8_django/__init__.py
+-rw-r--r--   0        0        0     3361 2023-05-22 09:49:06.622640 flake8_django-1.3/flake8_django/checker.py
+-rw-r--r--   0        0        0      501 2022-08-10 20:12:15.745093 flake8_django-1.3/flake8_django/checkers/__init__.py
+-rw-r--r--   0        0        0     1235 2023-05-22 09:49:06.622822 flake8_django-1.3/flake8_django/checkers/base_model_checker.py
+-rw-r--r--   0        0        0      708 2023-05-22 09:49:06.622980 flake8_django-1.3/flake8_django/checkers/checker.py
+-rw-r--r--   0        0        0      828 2022-08-10 20:12:15.745299 flake8_django-1.3/flake8_django/checkers/decorator.py
+-rw-r--r--   0        0        0      504 2022-08-10 20:12:15.745364 flake8_django-1.3/flake8_django/checkers/issue.py
+-rw-r--r--   0        0        0     3973 2023-05-22 09:49:06.623142 flake8_django-1.3/flake8_django/checkers/model_content_order.py
+-rw-r--r--   0        0        0      906 2023-05-22 09:49:06.623288 flake8_django-1.3/flake8_django/checkers/model_dunder_str.py
+-rw-r--r--   0        0        0     1438 2022-08-10 20:12:15.745587 flake8_django-1.3/flake8_django/checkers/model_fields.py
+-rw-r--r--   0        0        0     2182 2023-05-22 09:49:06.623441 flake8_django-1.3/flake8_django/checkers/model_form.py
+-rw-r--r--   0        0        0     2047 2023-05-22 09:49:06.623597 flake8_django-1.3/flake8_django/checkers/model_meta.py
+-rw-r--r--   0        0        0      731 2022-08-10 20:12:15.745787 flake8_django-1.3/flake8_django/checkers/render.py
+-rw-r--r--   0        0        0      680 2023-05-22 09:49:06.623716 flake8_django-1.3/flake8_django/checkers/utils.py
+-rw-r--r--   0        0        0      979 2023-05-22 09:52:23.605895 flake8_django-1.3/pyproject.toml
+-rw-r--r--   0        0        0     4414 1970-01-01 00:00:00.000000 flake8_django-1.3/PKG-INFO
```

### Comparing `flake8_django-1.2/README.md` & `flake8_django-1.3/README.md`

 * *Files identical despite different names*

### Comparing `flake8_django-1.2/flake8_django/checker.py` & `flake8_django-1.3/flake8_django/checker.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 import ast
+import os
+import sys
 
-from flake8_django.checkers import (
-    DecoratorChecker,
-    ModelContentOrderChecker,
-    ModelDunderStrMissingChecker,
-    ModelFieldChecker,
-    ModelFormChecker,
-    ModelMetaChecker,
-    RenderChecker,
-)
+import astroid
+
+from flake8_django.checkers import (DecoratorChecker, ModelContentOrderChecker,
+                                    ModelDunderStrMissingChecker,
+                                    ModelFieldChecker, ModelFormChecker,
+                                    ModelMetaChecker, RenderChecker)
 
 __version__ = '1.1.5'
 
 
 CHECKS_DISABLED_BY_DEFAULT = ['DJ10', 'DJ11']
 
 
@@ -21,20 +20,14 @@
     Visit the node, and return issues.
     """
     checkers = {
         'Call': [
             ModelFieldChecker(),
             RenderChecker(),
         ],
-        'ClassDef': [
-            ModelFormChecker(),
-            ModelDunderStrMissingChecker(),
-            ModelMetaChecker(),
-            ModelContentOrderChecker(),
-        ],
         'FunctionDef': [
             DecoratorChecker(),
         ]
     }
 
     def __init__(self, *args, **kwargs):
         super(DjangoStyleFinder, self).__init__(*args, **kwargs)
@@ -46,36 +39,84 @@
             if issues:
                 self.issues.extend(issues)
         self.generic_visit(node)
 
     def visit_Call(self, node):
         self.capture_issues_visitor('Call', node)
 
-    def visit_ClassDef(self, node):
-        self.capture_issues_visitor('ClassDef', node)
-
     def visit_FunctionDef(self, node):
         self.capture_issues_visitor('FunctionDef', node)
 
 
+class AstroidTreeVisitor:
+    """
+    Go through astroid tree and return issues by specified checkers.
+    """
+    checkers = {
+        "ClassDef": (
+            ModelMetaChecker(),
+            ModelFormChecker(),
+            ModelDunderStrMissingChecker(),
+            ModelContentOrderChecker(),
+        )
+    }
+
+    def __init__(self):
+        self.issues = []
+
+    def visit(self, tree):
+        for node in tree.body:
+            self.issues.extend(
+                self.run_checkers(
+                    node=node,
+                    checker_type=node.__class__.__name__,
+                ),
+            )
+
+    def run_checkers(self, node, checker_type):
+        issues = []
+        for checker in self.checkers.get(checker_type, []):
+            checker_issues = checker.run(node)
+            if checker_issues:
+                issues.extend(checker_issues)
+        return issues
+
+
 class DjangoStyleChecker(object):
     """
     Check common Django Style errors
     """
     name = 'flake8-django'
     version = __version__
+    astroid_manager = astroid.MANAGER
 
-    def __init__(self, tree, filename):
+    def __init__(self, tree, filename, lines=[]):
         self.tree = tree
         self.filename = filename
+        self.source_code = ''.join(lines)
+        self.build_astroid_tree()
+
+    def build_astroid_tree(self):
+        sys.path.append(os.getcwd())
+        if not self.filename:
+            self.astroid_tree = self.astroid_manager.ast_from_string(
+                self.source_code,
+            )
+        else:
+            self.astroid_tree = self.astroid_manager.ast_from_file(  # pragma: no cover
+                self.filename,
+            )
 
     @staticmethod
     def add_options(optmanager):
         """Informs flake8 to ignore checks by default."""
         optmanager.extend_default_ignore(CHECKS_DISABLED_BY_DEFAULT)
 
     def run(self):
         parser = DjangoStyleFinder()
         parser.visit(self.tree)
 
-        for issue in parser.issues:
+        astroid_parser = AstroidTreeVisitor()
+        astroid_parser.visit(self.astroid_tree)
+
+        for issue in parser.issues + astroid_parser.issues:
             yield issue.lineno, issue.col, issue.message, DjangoStyleChecker
```

### Comparing `flake8_django-1.2/flake8_django/checkers/decorator.py` & `flake8_django-1.3/flake8_django/checkers/decorator.py`

 * *Files identical despite different names*

### Comparing `flake8_django-1.2/flake8_django/checkers/model_content_order.py` & `flake8_django-1.3/flake8_django/checkers/model_content_order.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,13 @@
-from ast import Assign, ClassDef, FunctionDef
+import astroid
 from functools import partial
 
 from .base_model_checker import BaseModelChecker
 from .issue import Issue
+from .utils import node_is_subclass
 
 
 class DJ12(Issue):
     code = 'DJ12'
     description = (
         "The order of the model's inner classes, methods, and fields does not follow the "
         "Django Style Guide: {elem_type} should come before {before}"
@@ -18,39 +19,47 @@
             elem_type=elem_type,
             before=before,
         )
 
 
 def is_field_declaration(node):
     """
-    Verifies that the code is of the form: `field = models.CharField()`, matching by the `models` string.
+    Verify that node has Field value.
     """
     try:
-        return node.value.func.value.id == 'models'
+        for inferred_value in node.value.func.inferred():
+            if node_is_subclass(
+                inferred_value,
+                [".Field", "django.db.models.fields.Field"],
+            ):
+                return True
+        return False
     except AttributeError:
         return False
 
 
 def is_manager_declaration(node):
-    return isinstance(node, Assign) and getattr(node.targets[0], 'id', None) == 'objects'
+    return (
+        isinstance(node, astroid.Assign)
+        and getattr(node.targets[0], 'name', None) == 'objects'
+    )
 
 
 def is_meta_declaration(node):
-    return isinstance(node, ClassDef) and node.name == 'Meta'
+    return isinstance(node, astroid.ClassDef) and node.name == 'Meta'
 
 
 def is_method(node, method_name=None):
     if method_name is None:
-        return isinstance(node, FunctionDef)
-    return isinstance(node, FunctionDef) and node.name == method_name
+        return isinstance(node, astroid.FunctionDef)
+    return isinstance(node, astroid.FunctionDef) and node.name == method_name
 
 
 class ModelContentOrderChecker(BaseModelChecker):
-    model_name_lookup = 'Model'
-
+    model_name_lookups = ['.Model', 'django.db.models.base.Model']
     FIELD_DECLARATION = 'field declaration'
     MANAGER_DECLARATION = 'manager declaration'
     META_CLASS = 'Meta class'
     STR_METHOD = '__str__ method'
     SAVE_METHOD = 'save method'
     GET_ABSOLUTE_URL_METHOD = 'get_absolute_url method'
     CUSTOM_METHOD = 'custom method'
@@ -71,18 +80,15 @@
         (partial(is_method, method_name='__str__'), STR_METHOD),
         (partial(is_method, method_name='save'), SAVE_METHOD),
         (partial(is_method, method_name='get_absolute_url'), GET_ABSOLUTE_URL_METHOD),
         (is_method, CUSTOM_METHOD),
     ]
 
     def checker_applies(self, node):
-        for base in node.bases:
-            if self.is_model_name_lookup(base) or self.is_models_name_lookup_attribute(base):
-                return True
-        return False
+        return self.is_model(node)
 
     def run(self, node):
         if not self.checker_applies(node):
             return
 
         return self.get_issues(node)
```

### Comparing `flake8_django-1.2/flake8_django/checkers/model_dunder_str.py` & `flake8_django-1.3/flake8_django/checkers/model_dunder_str.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,31 +1,27 @@
-import ast
+import astroid
 
 from .base_model_checker import BaseModelChecker
 from .issue import Issue
 
 
 class DJ08(Issue):
     code = 'DJ08'
     description = 'Model does not define __str__ method'
 
 
 class ModelDunderStrMissingChecker(BaseModelChecker):
-    model_name_lookup = 'Model'
+    model_name_lookups = ['.Model', 'django.db.models.base.Model']
 
     def checker_applies(self, node):
-        for base in node.bases:
-            if self.is_model_name_lookup(base) or self.is_models_name_lookup_attribute(base):
-                if not self.is_abstract_model(node):
-                    return True
-        return False
+        return self.is_model(node) and not self.is_abstract_model(node)
 
     def is_dunder_str_method(self, element):
         return (
-            isinstance(element, ast.FunctionDef) and
+            isinstance(element, astroid.FunctionDef) and
             element.name == '__str__'
         )
 
     def run(self, node):
         if not self.checker_applies(node):
             return
```

### Comparing `flake8_django-1.2/flake8_django/checkers/model_fields.py` & `flake8_django-1.3/flake8_django/checkers/model_fields.py`

 * *Files identical despite different names*

### Comparing `flake8_django-1.2/flake8_django/checkers/model_form.py` & `flake8_django-1.3/flake8_django/checkers/model_form.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import ast
+import astroid
 
 from .base_model_checker import BaseModelChecker
 from .issue import Issue
 
 
 class DJ06(Issue):
     code = 'DJ06'
@@ -11,58 +11,57 @@
 
 class DJ07(Issue):
     code = 'DJ07'
     description = "Do not use __all__ with ModelForm, use fields instead"
 
 
 class ModelFormChecker(BaseModelChecker):
-    model_name_lookup = 'ModelForm'
+    model_name_lookups = ['.ModelForm', 'django.forms.models.ModelForm']
 
     def checker_applies(self, node):
-        for base in node.bases:
-            is_model_form = self.is_model_name_lookup(base) or self.is_models_name_lookup_attribute(base)
-            if is_model_form:
-                return True
-        return False
+        return self.is_model(node)
 
     def is_string_dunder_all(self, element):
         """
-        Return True if element is ast.Str or ast.Bytes and equals "__all__"
+        Return True if element is astroid.Const, astroid.List or astroid.Tuple  and equals "__all__"
         """
-        if not isinstance(element.value, (ast.Str, ast.Bytes)):
-            return False
-
-        node_value = element.value.s
-        if isinstance(node_value, bytes):
-            node_value = node_value.decode()
-        return node_value == '__all__'
+        if isinstance(element.value, (astroid.List, astroid.Tuple)):
+            return any(
+                iter_item.value == '__all__'
+                for iter_item in element.value.itered()
+            )
+        else:
+            node_value = element.value.value
+            if isinstance(node_value, bytes):
+                node_value = node_value.decode()
+            return node_value == '__all__'
 
     def run(self, node):
         """
         Captures the use of exclude in ModelForm Meta
         """
         if not self.checker_applies(node):
             return
 
         issues = []
         for body in node.body:
-            if not isinstance(body, ast.ClassDef):
+            if not isinstance(body, astroid.ClassDef):
                 continue
             for element in body.body:
-                if not isinstance(element, ast.Assign):
+                if not isinstance(element, astroid.Assign):
                     continue
                 for target in element.targets:
-                    if target.id == 'fields' and self.is_string_dunder_all(element):
+                    if target.name == 'fields' and self.is_string_dunder_all(element):
                         issues.append(
                             DJ07(
                                 lineno=node.lineno,
                                 col=node.col_offset,
                             )
                         )
-                    elif target.id == 'exclude':
+                    elif target.name == 'exclude':
                         issues.append(
                             DJ06(
                                 lineno=node.lineno,
                                 col=node.col_offset,
                             )
                         )
         return issues
```

### Comparing `flake8_django-1.2/flake8_django/checkers/model_meta.py` & `flake8_django-1.3/flake8_django/checkers/model_meta.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import ast
+import astroid
 
 from flake8_django.checkers.base_model_checker import BaseModelChecker
 from flake8_django.checkers.issue import Issue
 
 
 class DJ10(Issue):
     code = 'DJ10'
@@ -11,59 +11,46 @@
 
 class DJ11(Issue):
     code = 'DJ11'
     description = 'Model should define verbose_name_plural in its Meta inner class'
 
 
 class ModelMetaChecker(BaseModelChecker):
-    model_name_lookup = 'Model'
+    model_name_lookups = ['.Model', 'django.db.models.base.Model']
 
     def checker_applies(self, node):
-        for base in node.bases:
-            if self.is_model_name_lookup(base) or self.is_models_name_lookup_attribute(base):
-                if not self.is_abstract_model(node):
-                    return True
-        return False
+        return self.is_model(node) and not self.is_abstract_model(node)
 
-    @staticmethod
-    def has_meta_class(element):
-        # for node in element.body[0].body:  # type: ignore
-        for node in element.body:  # type: ignore
-            if isinstance(node, ast.ClassDef):
-                if node.name == 'Meta':
-                    return node
+    def get_meta_class(self, node):
+        for child_node in node.body:
+            if isinstance(child_node, astroid.ClassDef):
+                if child_node.name == 'Meta':
+                    return child_node
         return
 
+    def _has_element(self, node, target_name: str):
+        for child_node in node.body:
+            if not isinstance(child_node, astroid.Assign):
+                continue
+            attr = child_node.targets[0].name
+            if attr == target_name:
+                return True
+        return False
+
     def has_verbose_name(self, meta_class_node):
         return self._has_element(meta_class_node, 'verbose_name')
 
     def has_verbose_name_plural(self, meta_class_node):
         return self._has_element(meta_class_node, 'verbose_name_plural')
 
-    @staticmethod
-    def _has_element(element, target_name):
-        for node in ast.iter_child_nodes(element):
-            if not isinstance(node, ast.Assign):
-                continue
-            if not isinstance(node.targets[0], ast.Name):
-                continue
-            attr = node.targets[0].id
-            if attr == target_name:
-                return True
-        return False
-
     def run(self, node):
-        """
-        Check a single model.
-        """
         if not self.checker_applies(node):
             return
 
-        meta_class_node = self.has_meta_class(node)
-
+        meta_class_node = self.get_meta_class(node)
         issues = []
         if not meta_class_node or not self.has_verbose_name(meta_class_node):
             issues.append(
                 DJ10(
                     lineno=node.lineno,
                     col=node.col_offset,
                 )
```

### Comparing `flake8_django-1.2/flake8_django/checkers/render.py` & `flake8_django-1.3/flake8_django/checkers/render.py`

 * *Files identical despite different names*

### Comparing `flake8_django-1.2/pyproject.toml` & `flake8_django-1.3/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "flake8-django"
-version = "1.2"
+version = "1.3"
 license = "GPL-3.0-or-later"
 description = "Plugin to catch bad style specific to Django Projects."
 authors = ["Rocio Aramberri Schegel <rocio.aramberri@schegel.net>"]
 readme = "README.md"
 keywords = ["flake8", "django", "lint"]
 repository = "https://github.com/rocioar/flake8-django"
 classifiers=[
@@ -12,21 +12,23 @@
     "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Topic :: Software Development :: Quality Assurance",
 ]
 
 [tool.poetry.plugins]
 [tool.poetry.plugins."flake8.extension"]
-DJ0 = "flake8_django:DjangoStyleChecker"
+DJ = "flake8_django:DjangoStyleChecker"
 
 [build-system]
 requires = ["poetry_core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.dependencies]
-python = "^3.7"
+astroid = "^2.15.2"
+python = "^3.7.2"
 flake8 = ">=3.8.4,<7"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.1.2"
 pytest-cov = "^3.0.0"
 twine = "^4.0.1"
+django = ">=3.2"
```

### Comparing `flake8_django-1.2/PKG-INFO` & `flake8_django-1.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: flake8-django
-Version: 1.2
+Version: 1.3
 Summary: Plugin to catch bad style specific to Django Projects.
 Home-page: https://github.com/rocioar/flake8-django
 License: GPL-3.0-or-later
 Keywords: flake8,django,lint
 Author: Rocio Aramberri Schegel
 Author-email: rocio.aramberri@schegel.net
-Requires-Python: >=3.7,<4.0
+Requires-Python: >=3.7.2,<4.0.0
 Classifier: Framework :: Flake8
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Quality Assurance
+Requires-Dist: astroid (>=2.15.2,<3.0.0)
 Requires-Dist: flake8 (>=3.8.4,<7)
 Project-URL: Repository, https://github.com/rocioar/flake8-django
 Description-Content-Type: text/markdown
 
 # flake8-django
 
 [![pypi](https://img.shields.io/pypi/v/flake8-django.svg)](https://pypi.python.org/pypi/flake8-django/)
```

