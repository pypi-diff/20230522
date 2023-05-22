# Comparing `tmp/djangoviz-0.1.0.tar.gz` & `tmp/djangoviz-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "djangoviz-0.1.0.tar", last modified: Wed May 17 13:29:26 2023, max compression
+gzip compressed data, was "djangoviz-0.1.1.tar", last modified: Mon May 22 07:57:43 2023, max compression
```

## Comparing `djangoviz-0.1.0.tar` & `djangoviz-0.1.1.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:29:26.040793 djangoviz-0.1.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:29:26.032793 djangoviz-0.1.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:29:26.036793 djangoviz-0.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-05-17 13:29:02.000000 djangoviz-0.1.0/.github/workflows/cd-pypi.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-05-17 13:29:02.000000 djangoviz-0.1.0/.github/workflows/ci.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-17 13:29:02.000000 djangoviz-0.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-17 13:29:02.000000 djangoviz-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-05-17 13:29:26.040793 djangoviz-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-05-17 13:29:02.000000 djangoviz-0.1.0/Pipfile
--rw-r--r--   0 runner    (1001) docker     (123)     9468 2023-05-17 13:29:02.000000 djangoviz-0.1.0/Pipfile.lock
--rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-05-17 13:29:02.000000 djangoviz-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:29:26.036793 djangoviz-0.1.0/djangoviz/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 13:29:02.000000 djangoviz-0.1.0/djangoviz/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-17 13:29:02.000000 djangoviz-0.1.0/djangoviz/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:29:26.036793 djangoviz-0.1.0/djangoviz/management/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 13:29:02.000000 djangoviz-0.1.0/djangoviz/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:29:26.036793 djangoviz-0.1.0/djangoviz/management/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 13:29:02.000000 djangoviz-0.1.0/djangoviz/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5971 2023-05-17 13:29:02.000000 djangoviz-0.1.0/djangoviz/management/commands/djangoviz.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:29:26.036793 djangoviz-0.1.0/djangoviz.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-05-17 13:29:26.000000 djangoviz-0.1.0/djangoviz.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-05-17 13:29:26.000000 djangoviz-0.1.0/djangoviz.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 13:29:26.000000 djangoviz-0.1.0/djangoviz.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-17 13:29:26.000000 djangoviz-0.1.0/djangoviz.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-17 13:29:26.000000 djangoviz-0.1.0/djangoviz.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-05-17 13:29:02.000000 djangoviz-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-05-17 13:29:02.000000 djangoviz-0.1.0/run_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-05-17 13:29:02.000000 djangoviz-0.1.0/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 13:29:26.040793 djangoviz-0.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:29:26.040793 djangoviz-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 13:29:02.000000 djangoviz-0.1.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:29:26.040793 djangoviz-0.1.0/tests/app1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 13:29:02.000000 djangoviz-0.1.0/tests/app1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-05-17 13:29:02.000000 djangoviz-0.1.0/tests/app1/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:29:26.040793 djangoviz-0.1.0/tests/app1/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-05-17 13:29:02.000000 djangoviz-0.1.0/tests/app1/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 13:29:02.000000 djangoviz-0.1.0/tests/app1/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-05-17 13:29:02.000000 djangoviz-0.1.0/tests/app1/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:29:26.040793 djangoviz-0.1.0/tests/app2/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 13:29:02.000000 djangoviz-0.1.0/tests/app2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-05-17 13:29:02.000000 djangoviz-0.1.0/tests/app2/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:29:26.040793 djangoviz-0.1.0/tests/app2/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-05-17 13:29:02.000000 djangoviz-0.1.0/tests/app2/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 13:29:02.000000 djangoviz-0.1.0/tests/app2/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-05-17 13:29:02.000000 djangoviz-0.1.0/tests/app2/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     2908 2023-05-17 13:29:02.000000 djangoviz-0.1.0/tests/tests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 07:57:43.829117 djangoviz-0.1.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 07:57:43.825117 djangoviz-0.1.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 07:57:43.829117 djangoviz-0.1.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-05-22 07:57:23.000000 djangoviz-0.1.1/.github/workflows/cd-pypi.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-05-22 07:57:23.000000 djangoviz-0.1.1/.github/workflows/ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-22 07:57:23.000000 djangoviz-0.1.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-22 07:57:23.000000 djangoviz-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-05-22 07:57:43.829117 djangoviz-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-05-22 07:57:23.000000 djangoviz-0.1.1/Pipfile
+-rw-r--r--   0 runner    (1001) docker     (123)     9468 2023-05-22 07:57:23.000000 djangoviz-0.1.1/Pipfile.lock
+-rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-05-22 07:57:23.000000 djangoviz-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 07:57:43.829117 djangoviz-0.1.1/djangoviz/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 07:57:23.000000 djangoviz-0.1.1/djangoviz/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-22 07:57:23.000000 djangoviz-0.1.1/djangoviz/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 07:57:43.829117 djangoviz-0.1.1/djangoviz/management/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 07:57:23.000000 djangoviz-0.1.1/djangoviz/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 07:57:43.829117 djangoviz-0.1.1/djangoviz/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 07:57:23.000000 djangoviz-0.1.1/djangoviz/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5988 2023-05-22 07:57:23.000000 djangoviz-0.1.1/djangoviz/management/commands/djangoviz.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 07:57:43.829117 djangoviz-0.1.1/djangoviz.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-05-22 07:57:43.000000 djangoviz-0.1.1/djangoviz.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-05-22 07:57:43.000000 djangoviz-0.1.1/djangoviz.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 07:57:43.000000 djangoviz-0.1.1/djangoviz.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-22 07:57:43.000000 djangoviz-0.1.1/djangoviz.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-22 07:57:43.000000 djangoviz-0.1.1/djangoviz.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-05-22 07:57:23.000000 djangoviz-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-05-22 07:57:23.000000 djangoviz-0.1.1/run_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-05-22 07:57:23.000000 djangoviz-0.1.1/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 07:57:43.829117 djangoviz-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 07:57:43.829117 djangoviz-0.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 07:57:23.000000 djangoviz-0.1.1/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 07:57:43.829117 djangoviz-0.1.1/tests/app1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 07:57:23.000000 djangoviz-0.1.1/tests/app1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-05-22 07:57:23.000000 djangoviz-0.1.1/tests/app1/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 07:57:43.829117 djangoviz-0.1.1/tests/app1/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-05-22 07:57:23.000000 djangoviz-0.1.1/tests/app1/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 07:57:23.000000 djangoviz-0.1.1/tests/app1/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-05-22 07:57:23.000000 djangoviz-0.1.1/tests/app1/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 07:57:43.829117 djangoviz-0.1.1/tests/app2/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 07:57:23.000000 djangoviz-0.1.1/tests/app2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-05-22 07:57:23.000000 djangoviz-0.1.1/tests/app2/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 07:57:43.829117 djangoviz-0.1.1/tests/app2/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-05-22 07:57:23.000000 djangoviz-0.1.1/tests/app2/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 07:57:23.000000 djangoviz-0.1.1/tests/app2/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-05-22 07:57:23.000000 djangoviz-0.1.1/tests/app2/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2908 2023-05-22 07:57:23.000000 djangoviz-0.1.1/tests/tests.py
```

### Comparing `djangoviz-0.1.0/.github/workflows/cd-pypi.yaml` & `djangoviz-0.1.1/.github/workflows/cd-pypi.yaml`

 * *Files identical despite different names*

### Comparing `djangoviz-0.1.0/.github/workflows/ci.yaml` & `djangoviz-0.1.1/.github/workflows/ci.yaml`

 * *Files identical despite different names*

### Comparing `djangoviz-0.1.0/LICENSE` & `djangoviz-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `djangoviz-0.1.0/PKG-INFO` & `djangoviz-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djangoviz
-Version: 0.1.0
+Version: 0.1.1
 Summary: A visualization tool.
 Author-email: Yoni Davidson <y@ariga.io>
 Project-URL: Homepage, https://github.com/ariga/djangoviz
 Keywords: django,erd,visualization
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
```

### Comparing `djangoviz-0.1.0/Pipfile.lock` & `djangoviz-0.1.1/Pipfile.lock`

 * *Files identical despite different names*

### Comparing `djangoviz-0.1.0/README.md` & `djangoviz-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `djangoviz-0.1.0/djangoviz/management/commands/djangoviz.py` & `djangoviz-0.1.1/djangoviz/management/commands/djangoviz.py`

 * *Files 3% similar despite different names*

```diff
@@ -114,15 +114,15 @@
     def handle(self, *args, **options):
         db_driver = _get_db_driver()
         migrations = self._get_migrations()
         if not migrations:
             self.stderr.write(self.style.ERROR("no migrations found"))
             return
         client = GraphQLClient(endpoint=API_ENDPOINT)
-        client.inject_token("user-agent", f"djangoviz/{__version__}")
+        client.inject_token(token=f"djangoviz/{__version__}", headername="user-agent")
         try:
             atlas_schema = _get_atlas_schema(client, migrations, db_driver)
             if atlas_schema is None:
                 self.stdout.write(self.style.ERROR("atlas schema was not created"))
                 return
         except Exception as e:
             self.stdout.write(self.style.ERROR("failed to compute atlas schema"))
```

### Comparing `djangoviz-0.1.0/djangoviz.egg-info/PKG-INFO` & `djangoviz-0.1.1/djangoviz.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djangoviz
-Version: 0.1.0
+Version: 0.1.1
 Summary: A visualization tool.
 Author-email: Yoni Davidson <y@ariga.io>
 Project-URL: Homepage, https://github.com/ariga/djangoviz
 Keywords: django,erd,visualization
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
```

### Comparing `djangoviz-0.1.0/djangoviz.egg-info/SOURCES.txt` & `djangoviz-0.1.1/djangoviz.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `djangoviz-0.1.0/pyproject.toml` & `djangoviz-0.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `djangoviz-0.1.0/tests/app1/migrations/0001_initial.py` & `djangoviz-0.1.1/tests/app1/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangoviz-0.1.0/tests/app2/migrations/0001_initial.py` & `djangoviz-0.1.1/tests/app2/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangoviz-0.1.0/tests/tests.py` & `djangoviz-0.1.1/tests/tests.py`

 * *Files identical despite different names*

