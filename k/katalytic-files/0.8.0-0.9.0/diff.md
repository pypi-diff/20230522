# Comparing `tmp/katalytic-files-0.8.0.tar.gz` & `tmp/katalytic_files-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "katalytic-files-0.8.0.tar", last modified: Fri Apr 28 12:23:53 2023, max compression
+gzip compressed data, was "katalytic_files-0.9.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `katalytic-files-0.8.0.tar` & `katalytic_files-0.9.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0       87 2023-04-13 15:48:09.439894 katalytic-files-0.8.0/.coveragerc
--rw-r--r--   0        0        0      641 2023-04-05 07:07:35.618314 katalytic-files-0.8.0/.gitignore
--rw-r--r--   0        0        0     3109 2023-04-27 17:14:43.739675 katalytic-files-0.8.0/.gitlab-ci.yml
--rw-r--r--   0        0        0     1893 2023-04-28 12:23:36.854794 katalytic-files-0.8.0/CHANGELOG.md
--rw-r--r--   0        0        0     1066 2023-04-10 04:00:05.979612 katalytic-files-0.8.0/LICENSE.txt
--rw-r--r--   0        0        0     2031 2023-04-14 19:03:52.346854 katalytic-files-0.8.0/README.md
--rw-r--r--   0        0        0     1552 2023-04-28 12:23:36.854794 katalytic-files-0.8.0/pyproject.toml
--rw-r--r--   0        0        0    15909 2023-04-28 12:20:22.710268 katalytic-files-0.8.0/src/katalytic/files.py
--rw-r--r--   0        0        0    44993 2023-04-28 11:43:36.576283 katalytic-files-0.8.0/tests/test_files.py
--rw-r--r--   0        0        0     3209 1970-01-01 00:00:00.000000 katalytic-files-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0       87 2023-04-13 15:48:09.439894 katalytic_files-0.9.0/.coveragerc
+-rw-r--r--   0        0        0      651 2023-05-01 06:38:08.285250 katalytic_files-0.9.0/.gitignore
+-rw-r--r--   0        0        0     3242 2023-05-05 03:59:34.970335 katalytic_files-0.9.0/.gitlab-ci.yml
+-rw-r--r--   0        0        0     2614 2023-05-22 16:52:04.391944 katalytic_files-0.9.0/CHANGELOG.md
+-rw-r--r--   0        0        0     1066 2023-04-10 04:00:05.979612 katalytic_files-0.9.0/LICENSE.txt
+-rw-r--r--   0        0        0     1900 2023-05-14 08:37:32.778688 katalytic_files-0.9.0/README.md
+-rw-r--r--   0        0        0     1378 2023-05-22 16:52:04.367944 katalytic_files-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0    35693 2023-05-22 16:47:01.078578 katalytic_files-0.9.0/src/katalytic/files.py
+-rw-r--r--   0        0        0    45211 2023-05-20 16:40:59.258168 katalytic_files-0.9.0/tests/test_files.py
+-rw-r--r--   0        0        0     3183 1970-01-01 00:00:00.000000 katalytic_files-0.9.0/PKG-INFO
```

### Comparing `katalytic-files-0.8.0/.gitignore` & `katalytic_files-0.9.0/.gitignore`

 * *Files 12% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 __pycache__/*
 .cache/*
 .*.swp
 */.ipynb_checkpoints/*
 .DS_Store
 data/
 logs/
+sandbox.*
 
 # Project files
 .ropeproject
 .project
 .pydevproject
 .settings
 .idea
```

### Comparing `katalytic-files-0.8.0/.gitlab-ci.yml` & `katalytic_files-0.9.0/.gitlab-ci.yml`

 * *Files 6% similar despite different names*

```diff
@@ -1,35 +1,39 @@
 include:
 - template: Security/SAST.gitlab-ci.yml
 
-image: python:3.9
+image: python:3.6
 
 stages:
   - coverage
-  - security
   - test
+  - security
   - release
 
 variables:
-  TOX_ENV: py39
   PIP_DISABLE_PIP_VERSION_CHECK: "1"
   PIP_NO_CACHE_DIR: "off"
 
-test_cov:
+coverage:
   image: python:3.6
   stage: coverage
   script:
     - pip install --upgrade pip
-    - pip install pytest pytest-cov pytest-randomly
-    - pip install -e .
-    - python -m pytest --cov-fail-under=100 --cov=src --cov-report term-missing || { echo "Tests failed. Exiting ..." && exit 1; }
+    - pip install -e .[dev]
+    - python -m pytest --cov-fail-under=100 --cov=src --cov-report=xml --cov-report=term-missing || { echo "Tests failed. Exiting ..." && exit 1; }
   rules:
     - if: '$CI_COMMIT_MESSAGE =~ /(feat|fix|refactor|perf|test|chore|style)/i'
       when: always
     - when: never
+  coverage: /(?i)total.*? (100(?:\.0+)?\%|[1-9]?\d(?:\.\d+)?\%)$/
+  artifacts:
+    reports:
+      coverage_report:
+        coverage_format: cobertura
+        path: "coverage.xml"
   allow_failure: false
 
 
 # test_py36:
 #   image: python:3.6
 #   stage: test
 #   script:
```

### Comparing `katalytic-files-0.8.0/CHANGELOG.md` & `katalytic_files-0.9.0/CHANGELOG.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,16 @@
+## 0.9.0 (2023-05-22)
+### feat
+- [[`e339626`](https://gitlab.com/katalytic/katalytic-files/commit/e33962652287c979406ecc533da7a55e9cb58e50)] add ujson as optional dependency and try using it instead of the stdlib json for faster load/save
+### refactor
+- [[`00d80e2`](https://gitlab.com/katalytic/katalytic-files/commit/00d80e2b4b273e595a6f174750a0e69f29540387)] remove unused private function
+- [[`69bd62b`](https://gitlab.com/katalytic/katalytic-files/commit/69bd62be521ca9cf2628eb36b79d327995b5509f)] replace private functions with the ones from katalytic.data
+- [[`7ecef41`](https://gitlab.com/katalytic/katalytic-files/commit/7ecef418d0cd93f92da959c0c16d2ecdfd6c2218)] use is_none_of, is_any_of from katalytic-data
+
+
 ## 0.8.0 (2023-04-28)
 ### feat
 - [[`43ef293`](https://gitlab.com/katalytic/katalytic-files/commit/43ef293431fafae20d13dbc2798cb78958fea4c4)] remove the encoding arg from load/save and the **kwargs from non-universal funcs
 
 
 ## 0.7.0 (2023-04-28)
 ### feat
```

### Comparing `katalytic-files-0.8.0/LICENSE.txt` & `katalytic_files-0.9.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `katalytic-files-0.8.0/README.md` & `katalytic_files-0.9.0/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,16 +1,17 @@
+# Not fit for public use yet
+
 ## Description
 TODO: Let people know what your project can do specifically. Provide context and add a link to any reference visitors might be unfamiliar with. A list of Features or a Background subsection can also be added here. If there are alternatives to your project, this is a good place to list differentiating factors.
 
 [![version](https://img.shields.io/pypi/v/katalytic-files)](https://pypi.org/project/katalytic-files/)
-[![Build Status](https://app.travis-ci.com/katalytic/katalytic-files.svg?branch=main)](https://app.travis-ci.com/gitlab/katalytic/katalytic-files)
-[![Test Results](https://img.shields.io/travis/com/katalytic/katalytic-files?label=tests)](https://app.travis-ci.com/gitlab/katalytic/katalytic-files)
-[![Coverage Status](https://coveralls.io/repos/gitlab/katalytic/katalytic-files/badge.svg?branch=main)](https://coveralls.io/gitlab/katalytic/katalytic-files?branch=main)
-[![Docs Coverage](https://img.shields.io/readthedocs/katalytic-files.svg)](https://katalytic-files.readthedocs.io/en/latest/)
-[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
+[![tests](https://gitlab.com/katalytic/katalytic-files/badges/main/pipeline.svg?key_text=tests&key_width=38)](https://gitlab.com/katalytic/katalytic-files/-/commits/main)
+[![coverage](https://gitlab.com/katalytic/katalytic-files/badges/main/coverage.svg)](https://gitlab.com/katalytic/katalytic-files/-/commits/main)
+[![docs](https://img.shields.io/readthedocs/katalytic-files.svg)](https://katalytic-files.readthedocs.io/en/latest/)
+[![license: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 
 ## Installation
 By itself
 ```bash
 pip install katalytic-files
 ```
```

### Comparing `katalytic-files-0.8.0/pyproject.toml` & `katalytic_files-0.9.0/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "katalytic-files"
-version = "0.8.0"
+version = "0.9.0"
 description = "This plugin adds utilities for working with files to the katalytic namespace"
 license = {file = "LICENSE.txt"}
 readme = "README.md"
 
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
@@ -26,40 +26,32 @@
     "automation",
     "filesystem"
 ]
 authors = [{name="Valentin Neagu", email="vali19th@protonmail.com"}]
 
 requires-python = ">=3.6"
 dependencies = [
-    "katalytic-data>=0.4.0",
+    "katalytic-data>=0.9.1",
     "katalytic-pkg>=0.2.0",
 ]
 
 [project.optional-dependencies]
+all = [
+	"ujson",
+]
+
 dev = [
     "pytest",
     "pytest-cov",
+    "pytest-clarity",
     "pytest-randomly",
 ]
 
 [project.urls]
 homepage = "https://gitlab.com/katalytic/katalytic-files.git"
 repository = "https://gitlab.com/katalytic/katalytic-files.git"
 
 [tool.pytest.ini_options]
 addopts = ["--import-mode=importlib"]
 
-[tool.tox]
-legacy_tox_ini = """
-[tox]
-env_list = py36, py37, py38, py39
-isolated_build = True
-
-[testenv]
-extras = dev
-deps = -e .
-
-commands = pytest --cov-fail-under=100 --cov=katalytic --cov-report term-missing
-"""
-
 [tool.flit.module]
 name = "katalytic.files"
```

### Comparing `katalytic-files-0.8.0/tests/test_files.py` & `katalytic_files-0.9.0/tests/test_files.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,43 +1,32 @@
-import collections
 import copy
 import shutil
 import tempfile
 from pathlib import Path
 
 import pytest
 
+from katalytic.data import all_types_besides, as_dict_of_lists, as_list_of_lists, is_iterable, is_iterator
 from katalytic.files import _get_all, clear_dir, copy_dir, copy_file, delete_dir, delete_file, get_dirs, get_files, get_unique_path, is_dir_empty, get_all, load, load_csv, load_json, load_text, make_dir, move_dir, move_file, save, save_csv, save_json, save_text
 
 
-def _create_seq_of_seq():
-    return [
-        ['a', 'b', 'c', 'd', 'e'],
-        [1, 'x', True, -1.5, True],
-        [2, None, False, 0.0, 'z'],
-        [None, 'y', '', None, 'w'],
-    ]
-
-
 def _create_seq_of_dicts():
     return [
         {'a': 1, 'b': 'x', 'c': True, 'd': -1.5, 'e': True},
         {'a': 2, 'b': None, 'c': False, 'd': 0.0, 'e': 'z'},
         {'a': None, 'b': 'y', 'c': '', 'd': None, 'e': 'w'},
     ]
 
 
+def _create_seq_of_seq():
+    return as_list_of_lists(_create_seq_of_dicts())
+
+
 def _create_dict_of_seq():
-    return {
-        'a': [1, 2, None],
-        'b': ['x', None, 'y'],
-        'c': [True, False, ''],
-        'd': [-1.5, 0.0, None],
-        'e': [True, 'z', 'w'],
-    }
+    return as_dict_of_lists(_create_seq_of_dicts())
 
 
 class TestGroup_save_and_load:
     class Test_json:
         def test_indent_0(self):
             data = self.create_json_data()
             path = _setup_path()
@@ -59,15 +48,15 @@
         def test_indent_as_float(self):
             data = self.create_json_data()
             path = _setup_path()
 
             save_json(data, path, indent=1.0)
             assert load_json(path) == data
 
-        @pytest.mark.parametrize('mistake', ['1', 1.1, True, False, None, [], {}, (), object()])
+        @pytest.mark.parametrize('mistake', all_types_besides('int'))
         def test_indent_of_wrong_type(self, mistake):
             data = self.create_json_data()
             path = _setup_path()
             with pytest.raises(TypeError):
                 save_json(data, path, indent=mistake)
 
         def test_save_sort_keys(self):
@@ -84,15 +73,15 @@
 
         def are_keys_sorted_recursive(self, data):
             if isinstance(data, dict):
                 if list(data.keys()) != sorted(data.keys()):
                     return False
 
                 return all(self.are_keys_sorted_recursive(v) for v in data.values())
-            elif isinstance(data, collections.Iterable) and not isinstance(data, str):
+            elif is_iterable(data) and not isinstance(data, str):
                 return all(self.are_keys_sorted_recursive(item) for item in data)
             else:
                 return True
 
         def create_json_data(self):
             """The keys are not sorted on purpose."""
             return {'e': 0, 'a': 1, 'b': 2.0, 'c': 3.5, 'd': [{'y': None, 'f': True, 'g': {'x': 'i', 'j': [False]}}]}
@@ -150,18 +139,15 @@
                 '"","y","","","w"',
             ])
 
             assert load(path) == expected_csv
             assert load_text(path).strip() == expected_text
 
         def test_json(self):
-            data = {
-                'a': 1,
-                'b': [2, True, None, {}],
-            }
+            data = {'a': 1, 'b': [2, True, None, {}]}
             path = _setup_path('{}.json')
             save(data, path)
 
             expected_text = '\n'.join([
                 '{',
                 '    "a": 1,',
                 '    "b": [',
@@ -293,36 +279,36 @@
                 copy_dir(src, dest)
 
         def test_src_is_missing(self):
             with pytest.raises(FileNotFoundError):
                 src = get_unique_path()
                 copy_dir(src, f'{src}_copy')
 
-        @pytest.mark.parametrize('mistake', [0, None, {}, True])
+        @pytest.mark.parametrize('mistake', all_types_besides(['str', 'path']))
         def test_precondition_dest(self, mistake):
             with pytest.raises(TypeError):
                 copy_dir('src', mistake)
 
         @pytest.mark.parametrize('mistake', [0, None, {}, True, 'hello'])
         def test_precondition_dir_exists(self, mistake):
             with pytest.raises(ValueError):
                 copy_dir('src', 'dest', dir_exists=mistake)
 
         @pytest.mark.parametrize('mistake', [0, None, {}, 'hello'])
         def test_precondition_file_exists(self, mistake):
             with pytest.raises(ValueError):
                 copy_dir('src', 'dest', file_exists=mistake)
 
-        @pytest.mark.parametrize('mistake', [0, None, {}, ''])
+        @pytest.mark.parametrize('mistake', all_types_besides('booleans'))
         def test_precondition_make_dirs(self, mistake):
             with pytest.raises(TypeError):
                 src, dest = _setup_dir(n=2)
                 copy_dir(src, dest, make_dirs=mistake)
 
-        @pytest.mark.parametrize('mistake', [0, None, {}, True])
+        @pytest.mark.parametrize('mistake', all_types_besides(['str', 'path']))
         def test_precondition_src(self, mistake):
             with pytest.raises(TypeError):
                 copy_dir(mistake, 'dest')
 
     class Test_copy_file:
         def test_dir(self):
             with pytest.raises(IsADirectoryError):
@@ -376,20 +362,20 @@
             assert Path(dest).read_text() == src
 
         def test_same_path(self):
             with pytest.raises(ValueError):
                 src = _setup_file()
                 copy_file(src, src)
 
-        @pytest.mark.parametrize('mistake', [0, None, {}, True])
+        @pytest.mark.parametrize('mistake', all_types_besides(['str', 'path']))
         def test_precondition_src(self, mistake):
             with pytest.raises(TypeError):
                 copy_file(mistake, 'a')
 
-        @pytest.mark.parametrize('mistake', [0, None, {}, True])
+        @pytest.mark.parametrize('mistake', all_types_besides(['str', 'path']))
         def test_precondition_dest(self, mistake):
             with pytest.raises(TypeError):
                 copy_file('a', mistake)
 
         @pytest.mark.parametrize('mistake', [0, None, {}, 'hello'])
         def test_precondition_make_dirs(self, mistake):
             with pytest.raises(ValueError):
@@ -436,30 +422,30 @@
                 delete_dir(path, non_empty_dir='error')
 
         def test_non_empty_dir_true(self):
             path, _ = _setup_dir_and_file()
             delete_dir(path, non_empty_dir=True)
             assert not Path(path).exists()
 
-        @pytest.mark.parametrize('mistake', [0, None, {}, ''])
+        @pytest.mark.parametrize('mistake', all_types_besides('booleans'))
         def test_precondition_missing_ok(self, mistake):
             with pytest.raises(TypeError):
                 delete_dir(get_unique_path(), missing_ok=mistake)
 
-        @pytest.mark.parametrize('mistake', [0, None, {}, ''])
+        @pytest.mark.parametrize('mistake', all_types_besides('booleans'))
         def test_precondition_non_empty_dir(self, mistake):
             with pytest.raises(ValueError):
                 delete_dir(get_unique_path(), non_empty_dir=mistake)
 
         @pytest.mark.parametrize('mistake', [None, '', '.'])
         def test_precondition_path_current_dir(self, mistake):
             with pytest.raises(ValueError):
                 delete_dir(mistake)
 
-        @pytest.mark.parametrize('mistake', [0, {}, True])
+        @pytest.mark.parametrize('mistake', all_types_besides(['none', 'str', 'path']))
         def test_precondition_path_type(self, mistake):
             with pytest.raises(TypeError):
                 delete_dir(mistake)
 
     class Test_delete_file:
         def test_dir(self):
             with pytest.raises(IsADirectoryError):
@@ -477,20 +463,20 @@
                 delete_file(path, missing_ok=False)
 
         def test_missing_ok_true(self):
             path = get_unique_path()
             delete_file(path, missing_ok=True)
             assert not Path(path).exists()
 
-        @pytest.mark.parametrize('mistake', [0, None, {}, True])
+        @pytest.mark.parametrize('mistake', all_types_besides(['str', 'path']))
         def test_precondition_path(self, mistake):
             with pytest.raises(TypeError):
                 delete_file(mistake)
 
-        @pytest.mark.parametrize('mistake', [0, None, {}, ''])
+        @pytest.mark.parametrize('mistake', all_types_besides('booleans'))
         def test_precondition_missing_ok(self, mistake):
             with pytest.raises(TypeError):
                 delete_file(get_unique_path(), missing_ok=mistake)
 
 
 class TestGroup_get:
     class Test_get_all:
@@ -519,15 +505,15 @@
 
         def test_path_is_missing(self):
             with pytest.raises(FileNotFoundError):
                 get_all(get_unique_path())
 
         def test_iter(self):
             r = get_all('', iter_=True)
-            assert isinstance(r, collections.Iterator)
+            assert is_iterator(r)
 
         def test_glob(self):
             path = _setup_tree_2()
             assert get_all(f'{path}/*/a/*') == [f'{path}/a/a/6.py', f'{path}/b/a/5.py']
 
         def test_glob_recursive(self):
             path = _setup_tree_2()
@@ -547,45 +533,45 @@
             path = _setup_tree()
             assert _get_all(path, only_files=True, prefix=False) == ['1.txt']
 
         def test_only_conflict(self):
             with pytest.raises(ValueError):
                 _get_all('', only_files=True, only_dirs=True)
 
-        @pytest.mark.parametrize('mistake', [0, None, {}, ''])
+        @pytest.mark.parametrize('mistake', all_types_besides('booleans'))
         def test_precondition_glob(self, mistake):
             with pytest.raises(TypeError):
                 get_all('', glob=mistake)
 
-        @pytest.mark.parametrize('mistake', [0, None, {}, ''])
+        @pytest.mark.parametrize('mistake', all_types_besides('booleans'))
         def test_precondition_iter_(self, mistake):
             with pytest.raises(TypeError):
                 get_all('', iter_=mistake)
 
-        @pytest.mark.parametrize('mistake', [0, None, {}, ''])
+        @pytest.mark.parametrize('mistake', all_types_besides('booleans'))
         def test_precondition_only_dirs(self, mistake):
             with pytest.raises(TypeError):
                 _get_all('', only_dirs=mistake)
 
-        @pytest.mark.parametrize('mistake', [0, None, {}, ''])
+        @pytest.mark.parametrize('mistake', all_types_besides('booleans'))
         def test_precondition_only_files(self, mistake):
             with pytest.raises(TypeError):
                 _get_all('', only_files=mistake)
 
         @pytest.mark.parametrize('mistake', [0, None, {}, True])
         def test_precondition_path(self, mistake):
             with pytest.raises(TypeError):
                 get_all(mistake)
 
-        @pytest.mark.parametrize('mistake', [0, None, {}, ''])
+        @pytest.mark.parametrize('mistake', all_types_besides('booleans'))
         def test_precondition_prefix(self, mistake):
             with pytest.raises(TypeError):
                 get_all('', prefix=mistake)
 
-        @pytest.mark.parametrize('mistake', [0, None, {}, ''])
+        @pytest.mark.parametrize('mistake', all_types_besides('booleans'))
         def test_precondition_recursive(self, mistake):
             with pytest.raises(TypeError):
                 get_all('', recursive=mistake)
 
         def test_recursive(self):
             path = _setup_tree()
             assert set(get_all(path, recursive=True)) == {
@@ -636,47 +622,47 @@
 
         def test_path_is_missing(self):
             with pytest.raises(FileNotFoundError):
                 get_dirs(get_unique_path())
 
         def test_iter(self):
             r = get_dirs('', iter_=True)
-            assert isinstance(r, collections.Iterator)
+            assert is_iterator(r)
 
         def test_glob(self):
             path = _setup_tree_2()
             assert get_dirs(f'{path}/*/a') == [f'{path}/a/a', f'{path}/b/a']
 
         def test_glob_recursive(self):
             path = _setup_tree_2()
             expected = [f'{path}/a', f'{path}/a/a', f'{path}/b/a', f'{path}/b/c/a']
             assert get_dirs(f'{path}/**/a') == expected
             assert get_dirs(f'{path}/*/a', recursive=True) == expected
 
-        @pytest.mark.parametrize('mistake', [0, None, {}, ''])
+        @pytest.mark.parametrize('mistake', all_types_besides('booleans'))
         def test_precondition_prefix(self, mistake):
             with pytest.raises(TypeError):
                 get_dirs('', prefix=mistake)
 
-        @pytest.mark.parametrize('mistake', [0, None, {}, ''])
+        @pytest.mark.parametrize('mistake', all_types_besides('booleans'))
         def test_precondition_glob(self, mistake):
             with pytest.raises(TypeError):
                 get_dirs('', glob=mistake)
 
-        @pytest.mark.parametrize('mistake', [0, None, {}, ''])
+        @pytest.mark.parametrize('mistake', all_types_besides('booleans'))
         def test_precondition_iter_(self, mistake):
             with pytest.raises(TypeError):
                 get_dirs('', iter_=mistake)
 
-        @pytest.mark.parametrize('mistake', [0, None, {}, True])
+        @pytest.mark.parametrize('mistake', all_types_besides(['str', 'path']))
         def test_precondition_path(self, mistake):
             with pytest.raises(TypeError):
                 get_dirs(mistake)
 
-        @pytest.mark.parametrize('mistake', [0, None, {}, ''])
+        @pytest.mark.parametrize('mistake', all_types_besides('booleans'))
         def test_precondition_recursive(self, mistake):
             with pytest.raises(TypeError):
                 get_dirs('', recursive=mistake)
 
         def test_recursive(self):
             path = _setup_tree()
             assert set(get_dirs(path, recursive=True)) == {
@@ -721,50 +707,50 @@
 
         def test_path_is_missing(self):
             with pytest.raises(FileNotFoundError):
                 get_files(get_unique_path())
 
         def test_iter(self):
             r = get_files('', iter_=True)
-            assert isinstance(r, collections.Iterator)
+            assert is_iterator(r)
 
         def test_glob(self):
             path = _setup_tree_2()
             assert get_files(f'{path}/*.py') == [f'{path}/1.py']
 
         def test_glob_recursive(self):
             path = _setup_tree_2()
             expected = [f'{path}/1.py', f'{path}/a/2.py', f'{path}/a/a/6.py', f'{path}/b/a/5.py']
             assert get_files(f'{path}/**/*.py') == expected
 
         def test_only_conflict(self):
             with pytest.raises(ValueError):
                 _get_all('', only_files=True, only_dirs=True)
 
-        @pytest.mark.parametrize('mistake', [0, None, {}, ''])
+        @pytest.mark.parametrize('mistake', all_types_besides('booleans'))
         def test_precondition_prefix(self, mistake):
             with pytest.raises(TypeError):
                 get_files('', prefix=mistake)
 
-        @pytest.mark.parametrize('mistake', [0, None, {}, ''])
+        @pytest.mark.parametrize('mistake', all_types_besides('booleans'))
         def test_precondition_glob(self, mistake):
             with pytest.raises(TypeError):
                 get_files('', glob=mistake)
 
-        @pytest.mark.parametrize('mistake', [0, None, {}, ''])
+        @pytest.mark.parametrize('mistake', all_types_besides('booleans'))
         def test_precondition_iter_(self, mistake):
             with pytest.raises(TypeError):
                 get_files('', iter_=mistake)
 
-        @pytest.mark.parametrize('mistake', [0, None, {}, True])
+        @pytest.mark.parametrize('mistake', all_types_besides(['str', 'path']))
         def test_precondition_path(self, mistake):
             with pytest.raises(TypeError):
                 get_files(mistake)
 
-        @pytest.mark.parametrize('mistake', [0, None, {}, ''])
+        @pytest.mark.parametrize('mistake', all_types_besides('booleans'))
         def test_precondition_recursive(self, mistake):
             with pytest.raises(TypeError):
                 get_files('', recursive=mistake)
 
         def test_recursive(self):
             path = _setup_tree()
             assert set(get_files(path, recursive=True)) == {
@@ -813,21 +799,21 @@
             assert is_dir_empty(path)
 
         def test_is_file(self):
             with pytest.raises(NotADirectoryError):
                 file = _setup_file()
                 clear_dir(file)
 
-        @pytest.mark.parametrize('mistake', [0, None, {}, ''])
+        @pytest.mark.parametrize('mistake', all_types_besides('booleans'))
         def test_precondition_create_missing(self, mistake):
             path = get_unique_path()
             with pytest.raises(TypeError):
                 clear_dir(path, create_missing=mistake)
 
-        @pytest.mark.parametrize('mistake', [0, None, {}, True])
+        @pytest.mark.parametrize('mistake', all_types_besides(['str', 'path']))
         def test_precondition_path(self, mistake):
             with pytest.raises(TypeError):
                 clear_dir(mistake)
 
     class Test_is_dir_empty:
         def test_empty(self):
             path = _setup_dir()
@@ -856,15 +842,15 @@
 
         @pytest.mark.parametrize('mistake', [[], '', 0, None])
         def test_precondition_missing(self, mistake):
             with pytest.raises(ValueError):
                 path = get_unique_path()
                 is_dir_empty(path, missing=mistake)
 
-        @pytest.mark.parametrize('mistake', [0, None, {}, True])
+        @pytest.mark.parametrize('mistake', all_types_besides(['str', 'path']))
         def test_precondition_path(self, mistake):
             with pytest.raises(TypeError):
                 is_dir_empty(mistake)
 
     class Test_mkdir:
         def test_create(self):
             path = _setup_dir()
@@ -894,25 +880,25 @@
                 make_dir(path)
 
         def test_no_parents(self):
             with pytest.raises(FileNotFoundError):
                 d = get_unique_path('parent/{}/child')
                 make_dir(d, create_parents=False)
 
-        @pytest.mark.parametrize('mistake', [0, None, {}, ''])
+        @pytest.mark.parametrize('mistake', all_types_besides('booleans'))
         def test_precondition_create_parents(self, mistake):
             with pytest.raises(TypeError):
                 make_dir(get_unique_path(), create_parents=mistake)
 
-        @pytest.mark.parametrize('mistake', [0, None, {}, ''])
+        @pytest.mark.parametrize('mistake', all_types_besides('booleans'))
         def test_precondition_exists_ok(self, mistake):
             with pytest.raises(TypeError):
                 make_dir(get_unique_path(), exists_ok=mistake)
 
-        @pytest.mark.parametrize('mistake', [0, None, {}, True])
+        @pytest.mark.parametrize('mistake', all_types_besides(['str', 'path']))
         def test_precondition_path(self, mistake):
             with pytest.raises(TypeError):
                 make_dir(mistake)
 
 
 class TestGroup_move:
     class Test_move_dir:
@@ -1049,36 +1035,36 @@
                 move_dir(src, dest)
 
         def test_src_is_missing(self):
             with pytest.raises(FileNotFoundError):
                 src = get_unique_path()
                 move_dir(src, f'{src}_copy')
 
-        @pytest.mark.parametrize('mistake', [0, None, {}, True])
+        @pytest.mark.parametrize('mistake', all_types_besides(['str', 'path']))
         def test_precondition_dest(self, mistake):
             with pytest.raises(TypeError):
                 move_dir('src', mistake)
 
         @pytest.mark.parametrize('mistake', [0, None, {}, True, 'hello'])
         def test_precondition_dir_exists(self, mistake):
             with pytest.raises(ValueError):
                 move_dir('src', 'dest', dir_exists=mistake)
 
         @pytest.mark.parametrize('mistake', [0, None, {}, 'hello'])
         def test_precondition_file_exists(self, mistake):
             with pytest.raises(ValueError):
                 move_dir('src', 'dest', file_exists=mistake)
 
-        @pytest.mark.parametrize('mistake', [0, None, {}, ''])
+        @pytest.mark.parametrize('mistake', all_types_besides('booleans'))
         def test_precondition_make_dirs(self, mistake):
             with pytest.raises(TypeError):
                 src, dest = _setup_dir(n=2)
                 move_dir(src, dest, make_dirs=mistake)
 
-        @pytest.mark.parametrize('mistake', [0, None, {}, True])
+        @pytest.mark.parametrize('mistake', all_types_besides(['str', 'path']))
         def test_precondition_src(self, mistake):
             with pytest.raises(TypeError):
                 move_dir(mistake, 'dest')
 
     class Test_move_file:
         def test_dir(self):
             with pytest.raises(IsADirectoryError):
@@ -1124,20 +1110,20 @@
             assert not Path(src).exists()
 
         def test_same_path(self):
             with pytest.raises(ValueError):
                 src = _setup_file()
                 move_file(src, src)
 
-        @pytest.mark.parametrize('mistake', [0, None, {}, True])
+        @pytest.mark.parametrize('mistake', all_types_besides(['str', 'path']))
         def test_precondition_src(self, mistake):
             with pytest.raises(TypeError):
                 move_file(mistake, 'a')
 
-        @pytest.mark.parametrize('mistake', [0, None, {}, True])
+        @pytest.mark.parametrize('mistake', all_types_besides(['str', 'path']))
         def test_precondition_dest(self, mistake):
             with pytest.raises(TypeError):
                 move_file('a', mistake)
 
         @pytest.mark.parametrize('mistake', [0, None, {}, 'hello'])
         def test_precondition_make_dirs(self, mistake):
             with pytest.raises(ValueError):
@@ -1156,15 +1142,15 @@
         def test_consecutive_values(self):
             root = Path(_setup_dir())
             for i in range(1, 11):
                 file = get_unique_path(root/'{}')
                 assert file == f'{root}/{i}'
                 Path(file).touch()
 
-        @pytest.mark.parametrize('mistake', [[], 1, True, None])
+        @pytest.mark.parametrize('mistake', all_types_besides(['str', 'path']))
         def test_invalid_pattern_type(self, mistake):
             with pytest.raises(TypeError):
                 get_unique_path(mistake)
 
         @pytest.mark.parametrize('mistake', ['', '{0}', '{a}', '{:f}'])
         def test_invalid_placeholder(self, mistake):
             with pytest.raises(ValueError):
```

### Comparing `katalytic-files-0.8.0/PKG-INFO` & `katalytic_files-0.9.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: katalytic-files
-Version: 0.8.0
+Version: 0.9.0
 Summary: This plugin adds utilities for working with files to the katalytic namespace
 Keywords: automation,filesystem
 Author-email: Valentin Neagu <vali19th@protonmail.com>
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -13,32 +13,36 @@
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: System :: Filesystems
 Classifier: Topic :: System :: Systems Administration
 Classifier: Topic :: Utilities
-Requires-Dist: katalytic-data>=0.4.0
+Requires-Dist: katalytic-data>=0.9.1
 Requires-Dist: katalytic-pkg>=0.2.0
+Requires-Dist: ujson ; extra == "all"
 Requires-Dist: pytest ; extra == "dev"
 Requires-Dist: pytest-cov ; extra == "dev"
+Requires-Dist: pytest-clarity ; extra == "dev"
 Requires-Dist: pytest-randomly ; extra == "dev"
 Project-URL: homepage, https://gitlab.com/katalytic/katalytic-files.git
 Project-URL: repository, https://gitlab.com/katalytic/katalytic-files.git
+Provides-Extra: all
 Provides-Extra: dev
 
+# Not fit for public use yet
+
 ## Description
 TODO: Let people know what your project can do specifically. Provide context and add a link to any reference visitors might be unfamiliar with. A list of Features or a Background subsection can also be added here. If there are alternatives to your project, this is a good place to list differentiating factors.
 
 [![version](https://img.shields.io/pypi/v/katalytic-files)](https://pypi.org/project/katalytic-files/)
-[![Build Status](https://app.travis-ci.com/katalytic/katalytic-files.svg?branch=main)](https://app.travis-ci.com/gitlab/katalytic/katalytic-files)
-[![Test Results](https://img.shields.io/travis/com/katalytic/katalytic-files?label=tests)](https://app.travis-ci.com/gitlab/katalytic/katalytic-files)
-[![Coverage Status](https://coveralls.io/repos/gitlab/katalytic/katalytic-files/badge.svg?branch=main)](https://coveralls.io/gitlab/katalytic/katalytic-files?branch=main)
-[![Docs Coverage](https://img.shields.io/readthedocs/katalytic-files.svg)](https://katalytic-files.readthedocs.io/en/latest/)
-[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
+[![tests](https://gitlab.com/katalytic/katalytic-files/badges/main/pipeline.svg?key_text=tests&key_width=38)](https://gitlab.com/katalytic/katalytic-files/-/commits/main)
+[![coverage](https://gitlab.com/katalytic/katalytic-files/badges/main/coverage.svg)](https://gitlab.com/katalytic/katalytic-files/-/commits/main)
+[![docs](https://img.shields.io/readthedocs/katalytic-files.svg)](https://katalytic-files.readthedocs.io/en/latest/)
+[![license: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 
 ## Installation
 By itself
 ```bash
 pip install katalytic-files
 ```
```

