# Comparing `tmp/ipywidgets_jsonschema-0.9.0.tar.gz` & `tmp/ipywidgets_jsonschema-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ipywidgets_jsonschema-0.9.0.tar", last modified: Fri Sep  9 11:46:53 2022, max compression
+gzip compressed data, was "ipywidgets_jsonschema-1.0.0.tar", last modified: Mon May 22 13:14:19 2023, max compression
```

## Comparing `ipywidgets_jsonschema-0.9.0.tar` & `ipywidgets_jsonschema-1.0.0.tar`

### file list

```diff
@@ -1,16 +1,64 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 11:46:53.422709 ipywidgets_jsonschema-0.9.0/
--rw-r--r--   0 runner    (1001) docker     (121)     1105 2022-09-09 11:46:49.000000 ipywidgets_jsonschema-0.9.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (121)     2413 2022-09-09 11:46:53.422709 ipywidgets_jsonschema-0.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2019 2022-09-09 11:46:49.000000 ipywidgets_jsonschema-0.9.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 11:46:53.422709 ipywidgets_jsonschema-0.9.0/ipywidgets_jsonschema/
--rw-r--r--   0 runner    (1001) docker     (121)       67 2022-09-09 11:46:49.000000 ipywidgets_jsonschema-0.9.0/ipywidgets_jsonschema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    25026 2022-09-09 11:46:49.000000 ipywidgets_jsonschema-0.9.0/ipywidgets_jsonschema/form.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 11:46:53.422709 ipywidgets_jsonschema-0.9.0/ipywidgets_jsonschema.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2413 2022-09-09 11:46:53.000000 ipywidgets_jsonschema-0.9.0/ipywidgets_jsonschema.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      342 2022-09-09 11:46:53.000000 ipywidgets_jsonschema-0.9.0/ipywidgets_jsonschema.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-09 11:46:53.000000 ipywidgets_jsonschema-0.9.0/ipywidgets_jsonschema.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       52 2022-09-09 11:46:53.000000 ipywidgets_jsonschema-0.9.0/ipywidgets_jsonschema.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       22 2022-09-09 11:46:53.000000 ipywidgets_jsonschema-0.9.0/ipywidgets_jsonschema.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      164 2022-09-09 11:46:49.000000 ipywidgets_jsonschema-0.9.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      594 2022-09-09 11:46:53.426709 ipywidgets_jsonschema-0.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)       39 2022-09-09 11:46:49.000000 ipywidgets_jsonschema-0.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 13:14:19.549289 ipywidgets_jsonschema-1.0.0/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 13:14:19.545289 ipywidgets_jsonschema-1.0.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (122)      120 2023-05-22 13:14:10.000000 ipywidgets_jsonschema-1.0.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 13:14:19.545289 ipywidgets_jsonschema-1.0.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (122)     1217 2023-05-22 13:14:10.000000 ipywidgets_jsonschema-1.0.0/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      601 2023-05-22 13:14:10.000000 ipywidgets_jsonschema-1.0.0/.github/workflows/pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     2837 2023-05-22 13:14:10.000000 ipywidgets_jsonschema-1.0.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (122)      989 2023-05-22 13:14:10.000000 ipywidgets_jsonschema-1.0.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     1105 2023-05-22 13:14:10.000000 ipywidgets_jsonschema-1.0.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (122)     2662 2023-05-22 13:14:19.549289 ipywidgets_jsonschema-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2263 2023-05-22 13:14:10.000000 ipywidgets_jsonschema-1.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 13:14:19.545289 ipywidgets_jsonschema-1.0.0/demo/
+-rw-r--r--   0 runner    (1001) docker     (122)     3235 2023-05-22 13:14:10.000000 ipywidgets_jsonschema-1.0.0/demo/demo.ipynb
+-rw-r--r--   0 runner    (1001) docker     (122)  2180597 2023-05-22 13:14:10.000000 ipywidgets_jsonschema-1.0.0/ipywidgets-jsonschema.gif
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 13:14:19.545289 ipywidgets_jsonschema-1.0.0/ipywidgets_jsonschema/
+-rw-r--r--   0 runner    (1001) docker     (122)      175 2023-05-22 13:14:10.000000 ipywidgets_jsonschema-1.0.0/ipywidgets_jsonschema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      160 2023-05-22 13:14:19.000000 ipywidgets_jsonschema-1.0.0/ipywidgets_jsonschema/_version.py
+-rw-r--r--   0 runner    (1001) docker     (122)    28372 2023-05-22 13:14:10.000000 ipywidgets_jsonschema-1.0.0/ipywidgets_jsonschema/form.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 13:14:19.545289 ipywidgets_jsonschema-1.0.0/ipywidgets_jsonschema.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     2662 2023-05-22 13:14:19.000000 ipywidgets_jsonschema-1.0.0/ipywidgets_jsonschema.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1688 2023-05-22 13:14:19.000000 ipywidgets_jsonschema-1.0.0/ipywidgets_jsonschema.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-22 13:14:19.000000 ipywidgets_jsonschema-1.0.0/ipywidgets_jsonschema.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       52 2023-05-22 13:14:19.000000 ipywidgets_jsonschema-1.0.0/ipywidgets_jsonschema.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       22 2023-05-22 13:14:19.000000 ipywidgets_jsonschema-1.0.0/ipywidgets_jsonschema.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     1085 2023-05-22 13:14:10.000000 ipywidgets_jsonschema-1.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)       35 2023-05-22 13:14:10.000000 ipywidgets_jsonschema-1.0.0/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-22 13:14:19.549289 ipywidgets_jsonschema-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)       39 2023-05-22 13:14:10.000000 ipywidgets_jsonschema-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 13:14:19.545289 ipywidgets_jsonschema-1.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)      499 2023-05-22 13:14:10.000000 ipywidgets_jsonschema-1.0.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 13:14:19.549289 ipywidgets_jsonschema-1.0.0/tests/schemas/
+-rw-r--r--   0 runner    (1001) docker     (122)    11590 2023-05-22 13:14:10.000000 ipywidgets_jsonschema-1.0.0/tests/schemas/adaptivefiltering-application.json
+-rw-r--r--   0 runner    (1001) docker     (122)      218 2023-05-22 13:14:10.000000 ipywidgets_jsonschema-1.0.0/tests/schemas/anyof-simple.json
+-rw-r--r--   0 runner    (1001) docker     (122)      240 2023-05-22 13:14:10.000000 ipywidgets_jsonschema-1.0.0/tests/schemas/anyof-title.json
+-rw-r--r--   0 runner    (1001) docker     (122)      177 2023-05-22 13:14:10.000000 ipywidgets_jsonschema-1.0.0/tests/schemas/array-defaults.json
+-rw-r--r--   0 runner    (1001) docker     (122)      215 2023-05-22 13:14:10.000000 ipywidgets_jsonschema-1.0.0/tests/schemas/array-fixed.json
+-rw-r--r--   0 runner    (1001) docker     (122)      228 2023-05-22 13:14:10.000000 ipywidgets_jsonschema-1.0.0/tests/schemas/array-minmax.json
+-rw-r--r--   0 runner    (1001) docker     (122)      215 2023-05-22 13:14:10.000000 ipywidgets_jsonschema-1.0.0/tests/schemas/array-simple.json
+-rw-r--r--   0 runner    (1001) docker     (122)      131 2023-05-22 13:14:10.000000 ipywidgets_jsonschema-1.0.0/tests/schemas/boolean-simple.json
+-rw-r--r--   0 runner    (1001) docker     (122)       83 2023-05-22 13:14:10.000000 ipywidgets_jsonschema-1.0.0/tests/schemas/const-simple.json
+-rw-r--r--   0 runner    (1001) docker     (122)      169 2023-05-22 13:14:10.000000 ipywidgets_jsonschema-1.0.0/tests/schemas/enum-simple.json
+-rw-r--r--   0 runner    (1001) docker     (122)       92 2023-05-22 13:14:10.000000 ipywidgets_jsonschema-1.0.0/tests/schemas/enum-single.json
+-rw-r--r--   0 runner    (1001) docker     (122)      801 2023-05-22 13:14:10.000000 ipywidgets_jsonschema-1.0.0/tests/schemas/if-then-complex.json
+-rw-r--r--   0 runner    (1001) docker     (122)      903 2023-05-22 13:14:10.000000 ipywidgets_jsonschema-1.0.0/tests/schemas/if-then-else.json
+-rw-r--r--   0 runner    (1001) docker     (122)      860 2023-05-22 13:14:10.000000 ipywidgets_jsonschema-1.0.0/tests/schemas/if-then-same.json
+-rw-r--r--   0 runner    (1001) docker     (122)      820 2023-05-22 13:14:10.000000 ipywidgets_jsonschema-1.0.0/tests/schemas/if-then.json
+-rw-r--r--   0 runner    (1001) docker     (122)      151 2023-05-22 13:14:10.000000 ipywidgets_jsonschema-1.0.0/tests/schemas/integer-minmax.json
+-rw-r--r--   0 runner    (1001) docker     (122)      132 2023-05-22 13:14:10.000000 ipywidgets_jsonschema-1.0.0/tests/schemas/integer-onesided-max.json
+-rw-r--r--   0 runner    (1001) docker     (122)      132 2023-05-22 13:14:10.000000 ipywidgets_jsonschema-1.0.0/tests/schemas/integer-onesided-min.json
+-rw-r--r--   0 runner    (1001) docker     (122)      119 2023-05-22 13:14:10.000000 ipywidgets_jsonschema-1.0.0/tests/schemas/integer-simple.json
+-rw-r--r--   0 runner    (1001) docker     (122)       60 2023-05-22 13:14:10.000000 ipywidgets_jsonschema-1.0.0/tests/schemas/null-simple.json
+-rw-r--r--   0 runner    (1001) docker     (122)      159 2023-05-22 13:14:10.000000 ipywidgets_jsonschema-1.0.0/tests/schemas/number-description.json
+-rw-r--r--   0 runner    (1001) docker     (122)      178 2023-05-22 13:14:10.000000 ipywidgets_jsonschema-1.0.0/tests/schemas/number-exlusiveminmax.json
+-rw-r--r--   0 runner    (1001) docker     (122)      150 2023-05-22 13:14:10.000000 ipywidgets_jsonschema-1.0.0/tests/schemas/number-minmax.json
+-rw-r--r--   0 runner    (1001) docker     (122)      131 2023-05-22 13:14:10.000000 ipywidgets_jsonschema-1.0.0/tests/schemas/number-onesided-maximum.json
+-rw-r--r--   0 runner    (1001) docker     (122)      131 2023-05-22 13:14:10.000000 ipywidgets_jsonschema-1.0.0/tests/schemas/number-onesided-min.json
+-rw-r--r--   0 runner    (1001) docker     (122)      139 2023-05-22 13:14:10.000000 ipywidgets_jsonschema-1.0.0/tests/schemas/number-simple.json
+-rw-r--r--   0 runner    (1001) docker     (122)      345 2023-05-22 13:14:10.000000 ipywidgets_jsonschema-1.0.0/tests/schemas/object-many.json
+-rw-r--r--   0 runner    (1001) docker     (122)      240 2023-05-22 13:14:10.000000 ipywidgets_jsonschema-1.0.0/tests/schemas/object-simple.json
+-rw-r--r--   0 runner    (1001) docker     (122)     8137 2023-05-22 13:14:10.000000 ipywidgets_jsonschema-1.0.0/tests/schemas/parafields-application.json
+-rw-r--r--   0 runner    (1001) docker     (122)      172 2023-05-22 13:14:10.000000 ipywidgets_jsonschema-1.0.0/tests/schemas/string-description.json
+-rw-r--r--   0 runner    (1001) docker     (122)      161 2023-05-22 13:14:10.000000 ipywidgets_jsonschema-1.0.0/tests/schemas/string-pattern.json
+-rw-r--r--   0 runner    (1001) docker     (122)      113 2023-05-22 13:14:10.000000 ipywidgets_jsonschema-1.0.0/tests/schemas/string-simple.json
+-rw-r--r--   0 runner    (1001) docker     (122)     1066 2023-05-22 13:14:10.000000 ipywidgets_jsonschema-1.0.0/tests/test_form.py
```

### Comparing `ipywidgets_jsonschema-0.9.0/LICENSE.md` & `ipywidgets_jsonschema-1.0.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `ipywidgets_jsonschema-0.9.0/PKG-INFO` & `ipywidgets_jsonschema-1.0.0/ipywidgets_jsonschema.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,33 +1,37 @@
 Metadata-Version: 2.1
-Name: ipywidgets_jsonschema
-Version: 0.9.0
+Name: ipywidgets-jsonschema
+Version: 1.0.0
 Summary: Widget Generator for JSON schema
-Author: Dominic Kempf
-Author-email: ssc@iwr.uni-heidelberg.de
-License: MIT
+Maintainer-email: Dominic Kempf <ssc@iwr.uni-heidelberg.de>
+License: LICENSE.md
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
 # ipywidgets-jsonschema - A widget generator for your Jupyter notebooks
 
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
-[![GitHub Workflow Status](https://img.shields.io/github/workflow/status/ssciwr/ipywidgets-jsonschema/CI)](https://github.com/ssciwr/ipywidgets-jsonschema/actions?query=workflow%3ACI)
+[![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/ssciwr/ipywidgets-jsonschema/ci.yml?branch=main)](https://github.com/ssciwr/ipywidgets-jsonschema/actions/workflows/ci.yml)
 [![PyPI version](https://badge.fury.io/py/ipywidgets-jsonschema.svg)](https://badge.fury.io/py/ipywidgets-jsonschema)
 [![Conda Version](https://img.shields.io/conda/vn/conda-forge/ipywidgets-jsonschema.svg)](https://anaconda.org/conda-forge/ipywidgets-jsonschema)
 [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/ssciwr/ipywidgets-jsonschema/main?labpath=demo%2Fdemo.ipynb)
 
+## Usage
+
+![Minimum usage exmaple](https://raw.githubusercontent.com/ssciwr/ipywidgets-jsonschema/main/ipywidgets-jsonschema.gif)
+
 This project allows you to generate Jupyter widgets from schemas
 that follow the [JSONSchema specification](https://json-schema.org). If you already have
 a schema available, creating a widget form for it is as simple
 as this:
 
+
 ```
 from ipywidgets_jsonschema import Form
 form = Form(schema)
 form.show()
 ```
 
 The data can then be retrieved from `form` by accessing `form.data`.
@@ -53,13 +57,13 @@
 conda install -c conda-forge ipywidgets-jsonschema
 ```
 
 ## Known limitations
 
 * Some aspects of the JSON Schema specification are hard to implement in
   a form generator and are therefore omitted e.g.
-  * The `allOf` and `not` rules for schema composition
+  * The `allOf` and `not` rules for schema composition are only partially or not at all supported.
   * Media types
-  * Conditional subschemas (might be added)
+  * There is only rudimentary support for conditional subschemas (like `if`-`then`-`else`)
 * Some annotations that are purely optional in the specification are required
   for the schema to be usable with `ipywidgets-jsonschema` e.g. a `title` field
   when the resulting widget would otherwise not be self-explanatory.
```

### Comparing `ipywidgets_jsonschema-0.9.0/README.md` & `ipywidgets_jsonschema-1.0.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,20 +1,37 @@
+Metadata-Version: 2.1
+Name: ipywidgets_jsonschema
+Version: 1.0.0
+Summary: Widget Generator for JSON schema
+Maintainer-email: Dominic Kempf <ssc@iwr.uni-heidelberg.de>
+License: LICENSE.md
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Description-Content-Type: text/markdown
+License-File: LICENSE.md
+
 # ipywidgets-jsonschema - A widget generator for your Jupyter notebooks
 
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
-[![GitHub Workflow Status](https://img.shields.io/github/workflow/status/ssciwr/ipywidgets-jsonschema/CI)](https://github.com/ssciwr/ipywidgets-jsonschema/actions?query=workflow%3ACI)
+[![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/ssciwr/ipywidgets-jsonschema/ci.yml?branch=main)](https://github.com/ssciwr/ipywidgets-jsonschema/actions/workflows/ci.yml)
 [![PyPI version](https://badge.fury.io/py/ipywidgets-jsonschema.svg)](https://badge.fury.io/py/ipywidgets-jsonschema)
 [![Conda Version](https://img.shields.io/conda/vn/conda-forge/ipywidgets-jsonschema.svg)](https://anaconda.org/conda-forge/ipywidgets-jsonschema)
 [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/ssciwr/ipywidgets-jsonschema/main?labpath=demo%2Fdemo.ipynb)
 
+## Usage
+
+![Minimum usage exmaple](https://raw.githubusercontent.com/ssciwr/ipywidgets-jsonschema/main/ipywidgets-jsonschema.gif)
+
 This project allows you to generate Jupyter widgets from schemas
 that follow the [JSONSchema specification](https://json-schema.org). If you already have
 a schema available, creating a widget form for it is as simple
 as this:
 
+
 ```
 from ipywidgets_jsonschema import Form
 form = Form(schema)
 form.show()
 ```
 
 The data can then be retrieved from `form` by accessing `form.data`.
@@ -40,13 +57,13 @@
 conda install -c conda-forge ipywidgets-jsonschema
 ```
 
 ## Known limitations
 
 * Some aspects of the JSON Schema specification are hard to implement in
   a form generator and are therefore omitted e.g.
-  * The `allOf` and `not` rules for schema composition
+  * The `allOf` and `not` rules for schema composition are only partially or not at all supported.
   * Media types
-  * Conditional subschemas (might be added)
+  * There is only rudimentary support for conditional subschemas (like `if`-`then`-`else`)
 * Some annotations that are purely optional in the specification are required
   for the schema to be usable with `ipywidgets-jsonschema` e.g. a `title` field
   when the resulting widget would otherwise not be self-explanatory.
```

### Comparing `ipywidgets_jsonschema-0.9.0/ipywidgets_jsonschema/form.py` & `ipywidgets_jsonschema-1.0.0/ipywidgets_jsonschema/form.py`

 * *Files 12% similar despite different names*

```diff
@@ -219,52 +219,131 @@
                 accordion.set_title(i, title)
 
         # This folds the accordion
         accordion.selected_index = None
         return [accordion]
 
     def _construct_object(self, schema, label=None, root=False):
-        # Construct form elements for all the fields
+        # Construct form elements for all the fields, including some that are
+        # added through 'if'-'then' rules. This maps key -> FormElement
         elements = {}
+
+        # Store the conditional information from the schema in the following form:
+        # [(schema, cprop, element), ..]
+        # with the following meaning:
+        #   schema: The schema that the data needs to match
+        #   cprop: The property that is maybe added
+        #   element: The subelement for the property
+        conditionals = []
         for prop, subschema in schema["properties"].items():
             elements[prop] = self._construct(subschema, label=prop)
 
+        # Add conditional elements
+        def add_conditional_elements(s):
+            # Check whether we have an if statement
+            cond = s.get("if", None)
+            if cond is None:
+                return
+
+            for cprop, csubschema in s.get("then", {}).get("properties", {}).items():
+                celem = self._construct(csubschema, label=cprop)
+                conditionals.append((cond, cprop, celem))
+                elements[cprop] = celem
+
+            if "else" in s:
+                add_conditional_elements(s["else"])
+
+        add_conditional_elements(schema)
+
         # Apply sorting to the keys
         keys = schema["properties"].keys()
         try:
             keys = self.sorter(keys)
         except TypeError:
             # If the keys cannot be compared, we stick to the original order
             pass
 
-        # If this is not the root document, we wrap this in an Accordion widget
+        # Collect the list of widgets: First the regular ones, then conditional ones
         widget_list = sum((elements[k].widgets for k in keys), [])
-        if not root:
-            widget_list = self._wrap_accordion(widget_list, schema, label=label)
+        widget_list.extend(
+            [
+                ipywidgets.HBox(layout=ipywidgets.Layout(width="100%"))
+                for _ in range(len(conditionals))
+            ]
+        )
 
-        def _setter(_d):
+        # Maybe wrap this in an Accordion widget
+        wrapped_widget_list = widget_list
+        if not root and len(schema["properties"]) > 1:
+            wrapped_widget_list = self._wrap_accordion(widget_list, schema, label=label)
+
+        def _getter():
+            # Get all regular properties
+            result = {}
             for k in schema["properties"].keys():
+                result[k] = elements[k].getter()
+
+            # Add conditional properties
+            for cschema, cprop, celem in conditionals:
+                try:
+                    jsonschema.validate(instance=result, schema=cschema)
+                    result[cprop] = celem.getter()
+                except jsonschema.ValidationError:
+                    pass
+
+            return result
+
+        def _setter(_d):
+            for k in elements.keys():
                 if k in _d:
                     elements[k].setter(_d[k])
                 else:
                     elements[k].resetter()
 
         def _register_observer(h, n, t):
             for e in elements.values():
                 e.register_observer(h, n, t)
 
         def _resetter():
             for e in elements.values():
                 e.resetter()
 
+        # Add the conditional information
+        for i, (cschema, cprop, celem) in enumerate(conditionals):
+
+            def create_observer(j, s, prop, e):
+                def _cond_observer(_):
+                    # Check whether our data matches the given schema
+                    try:
+                        jsonschema.validate(instance=_getter(), schema=s)
+                        elements[prop] = e
+                        widget_list[len(keys) + j].children = e.widgets
+                    except jsonschema.ValidationError:
+                        widget_list[len(keys) + j].children = []
+
+                # We need to call the observer once so that we get a correctly
+                # initialized widget, because otherwise it triggers only if it
+                # differs from the default.
+                _cond_observer({})
+
+                return _cond_observer
+
+            for k in cschema.get("properties", {}).keys():
+                elements[k].register_observer(
+                    create_observer(i, cschema, cprop, celem), "value", "change"
+                )
+
+        # Ensure that defaults are initialized
+        _resetter()
+
         return self.construct_element(
-            getter=lambda: {p: e.getter() for p, e in elements.items()},
+            getter=_getter,
             setter=_setter,
             resetter=_resetter,
-            widgets=widget_list,
+            widgets=wrapped_widget_list,
             subelements=elements,
             register_observer=_register_observer,
         )
 
     def _construct_simple(self, schema, widget, label=None, root=False):
         # Extract the best description that we have
         tooltip = schema.get("description", None)
@@ -281,30 +360,29 @@
 
             # Prepend a label to the widget
             box.insert(
                 0,
                 ipywidgets.Label(
                     title,
                     layout=ipywidgets.Layout(width="100%"),
-                    tooltip=tooltip,
                 ),
             )
 
         # Make sure that the widget shows the tooltip
         if tooltip is not None:
             widget.tooltip = tooltip
 
         # Apply potential constant values without generating a widget
         if "const" in schema:
             return self.construct_element(getter=lambda: schema["const"])
 
         # Apply regex pattern matching
         def pattern_checker(val):
             # This only makes sense for strings
-            if schema["type"] != "string":
+            if schema["type"] != "string" or val is None:
                 return True
 
             # Try matching the given data against the pattern
             pattern = schema.get("pattern", ".*")
             return re.fullmatch(pattern, val)
 
         # Describe how change handlers are registered
@@ -351,15 +429,15 @@
         if self.vertically_place_labels:
             box_type = ipywidgets.VBox
 
         return self.construct_element(
             getter=_getter,
             setter=_setter,
             resetter=_resetter,
-            widgets=[box_type(box)],
+            widgets=[box_type(box, layout=ipywidgets.Layout(width="100%"))],
             register_observer=_register_observer,
         )
 
     def _construct_string(self, schema, label=None, root=False):
         return self._construct_simple(schema, ipywidgets.Text(), label=label)
 
     def _construct_number(self, schema, label=None, root=False):
@@ -420,36 +498,40 @@
     def _construct_null(self, schema, label=None, root=False):
         return self.construct_element()
 
     def _construct_array(self, schema, label=None, root=False):
         if "items" not in schema:
             raise FormError("Expecting 'items' key for 'array' type")
 
+        # Determine whether this is a fixed length list
+        fixed_length = schema.get("minItems", -1) == schema.get("maxItems", -2)
+
         # Construct a widget that allows to add an array entry
         button = ipywidgets.Button(
             description="Add entry", icon="plus", layout=ipywidgets.Layout(width="100%")
         )
 
         # Construct the final widget that will be updated by handlers
-        vbox = ipywidgets.VBox([button])
+        vbox = ipywidgets.VBox([])
 
         # The subelements of this widget that are referenced in the
         # recursive implementation of this array element
         elements = []
 
         # We separately to store the size of the elements array. The reason
         # for this is that we do want to minimize the amount of element creations
         # as these are very costly for complex schemas
         element_size = 0
 
         # Trigger whenever the resulting widget needs update
         def update_widget():
-            vbox.children = sum((e.widgets for e in elements[:element_size]), []) + [
-                button
-            ]
+            subwidgets = sum((e.widgets for e in elements[:element_size]), [])
+            if not fixed_length:
+                subwidgets.append(button)
+            vbox.children = subwidgets
 
         def add_entry(_):
             nonlocal element_size
 
             # if we are at the specified maximum, add should be ignored
             if "maxItems" in schema:
                 if element_size == schema["maxItems"]:
@@ -470,15 +552,14 @@
                                 "type": "change",
                             }
                         )
 
             # A new element should only be generated if we do not have an excess
             # one stored in the elements list
             if element_size == len(elements):
-
                 # Create a new element by going into recursion
                 recelem = self._construct(schema["items"], label=None)
 
                 # Register existing observers
                 for h, n, t in self._observers:
                     recelem.register_observer(h, n, t)
 
@@ -537,22 +618,25 @@
                     return _move
 
                 # Register the handler for moving up and down
                 up.on_click(move(-1))
                 down.on_click(move(1))
 
                 # Construct the final widget including array controls
-                array_entry_widget = ipywidgets.VBox(
-                    [
-                        recelem.widgets[0].children[0],
+                children = [
+                    recelem.widgets[0].children[0],
+                ]
+                if not fixed_length:
+                    children.append(
                         ipywidgets.HBox(
                             [trash, up, down], layout=ipywidgets.Layout(width="100%")
-                        ),
-                    ]
-                )
+                        )
+                    )
+
+                array_entry_widget = ipywidgets.VBox(children)
 
                 # Modify recelem to our needs
                 elemdict = recelem._asdict()
                 elemdict["widgets"] = [array_entry_widget]
 
                 # Insert this into the elements list
                 elements.append(self.construct_element(**elemdict))
@@ -590,14 +674,16 @@
             element_size = 0
 
             # Update the widget potentially constructing new ones.
             for i, item in enumerate(_d):
                 add_entry(None)
                 elements[i].setter(item)
 
+            update_widget()
+
         def _register_observer(h, n, t):
             for e in elements:
                 e.register_observer(h, n, t)
 
         def _resetter():
             # If a default was specified, we now set it
             if "default" in schema:
@@ -622,18 +708,17 @@
 
         # Otherwise, we use a dropdown menu
         return self._construct_simple(
             schema, ipywidgets.Dropdown(options=schema["enum"]), label=label
         )
 
     def _construct_anyof(self, schema, label=None, key="anyOf"):
-        # Maybe create an explanatory widget
-        title = []
-        if "title" in schema:
-            title = [ipywidgets.Label(schema["title"])]
+        # If this is a trivial anyOf rule, we omit it:
+        if len(schema[key]) == 1:
+            return self._construct(schema[key][0], label=label, root=False)
 
         # The list of subelements and their descriptive names
         names = []
         elements = []
 
         # Iterate over the given subschema
         for s in schema[key]:
@@ -674,11 +759,11 @@
             for e in elements:
                 e.register_observer(h, n, t)
 
         return self.construct_element(
             getter=lambda: elements[names.index(selector.value)].getter(),
             setter=_setter,
             resetter=_resetter,
-            widgets=[ipywidgets.VBox(children=title + [widget])],
+            widgets=[ipywidgets.VBox(children=[widget])],
             subelements=elements,
             register_observer=_register_observer,
         )
```

### Comparing `ipywidgets_jsonschema-0.9.0/ipywidgets_jsonschema.egg-info/PKG-INFO` & `ipywidgets_jsonschema-1.0.0/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,33 +1,25 @@
-Metadata-Version: 2.1
-Name: ipywidgets-jsonschema
-Version: 0.9.0
-Summary: Widget Generator for JSON schema
-Author: Dominic Kempf
-Author-email: ssc@iwr.uni-heidelberg.de
-License: MIT
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Description-Content-Type: text/markdown
-License-File: LICENSE.md
-
 # ipywidgets-jsonschema - A widget generator for your Jupyter notebooks
 
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
-[![GitHub Workflow Status](https://img.shields.io/github/workflow/status/ssciwr/ipywidgets-jsonschema/CI)](https://github.com/ssciwr/ipywidgets-jsonschema/actions?query=workflow%3ACI)
+[![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/ssciwr/ipywidgets-jsonschema/ci.yml?branch=main)](https://github.com/ssciwr/ipywidgets-jsonschema/actions/workflows/ci.yml)
 [![PyPI version](https://badge.fury.io/py/ipywidgets-jsonschema.svg)](https://badge.fury.io/py/ipywidgets-jsonschema)
 [![Conda Version](https://img.shields.io/conda/vn/conda-forge/ipywidgets-jsonschema.svg)](https://anaconda.org/conda-forge/ipywidgets-jsonschema)
 [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/ssciwr/ipywidgets-jsonschema/main?labpath=demo%2Fdemo.ipynb)
 
+## Usage
+
+![Minimum usage exmaple](https://raw.githubusercontent.com/ssciwr/ipywidgets-jsonschema/main/ipywidgets-jsonschema.gif)
+
 This project allows you to generate Jupyter widgets from schemas
 that follow the [JSONSchema specification](https://json-schema.org). If you already have
 a schema available, creating a widget form for it is as simple
 as this:
 
+
 ```
 from ipywidgets_jsonschema import Form
 form = Form(schema)
 form.show()
 ```
 
 The data can then be retrieved from `form` by accessing `form.data`.
@@ -53,13 +45,13 @@
 conda install -c conda-forge ipywidgets-jsonschema
 ```
 
 ## Known limitations
 
 * Some aspects of the JSON Schema specification are hard to implement in
   a form generator and are therefore omitted e.g.
-  * The `allOf` and `not` rules for schema composition
+  * The `allOf` and `not` rules for schema composition are only partially or not at all supported.
   * Media types
-  * Conditional subschemas (might be added)
+  * There is only rudimentary support for conditional subschemas (like `if`-`then`-`else`)
 * Some annotations that are purely optional in the specification are required
   for the schema to be usable with `ipywidgets-jsonschema` e.g. a `title` field
   when the resulting widget would otherwise not be self-explanatory.
```

