# Comparing `tmp/kedro-graphql-0.1.4.tar.gz` & `tmp/kedro-graphql-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kedro-graphql-0.1.4.tar", last modified: Fri May 19 18:26:22 2023, max compression
+gzip compressed data, was "kedro-graphql-0.2.0.tar", last modified: Mon May 22 20:49:53 2023, max compression
```

## Comparing `kedro-graphql-0.1.4.tar` & `kedro-graphql-0.2.0.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:26:22.748717 kedro-graphql-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-19 18:26:11.000000 kedro-graphql-0.1.4/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)    10675 2023-05-19 18:26:22.748717 kedro-graphql-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10120 2023-05-19 18:26:11.000000 kedro-graphql-0.1.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-05-19 18:26:11.000000 kedro-graphql-0.1.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-19 18:26:22.752717 kedro-graphql-0.1.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:26:22.744717 kedro-graphql-0.1.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:26:22.748717 kedro-graphql-0.1.4/src/kedro_graphql/
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-19 18:26:11.000000 kedro-graphql-0.1.4/src/kedro_graphql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-05-19 18:26:11.000000 kedro-graphql-0.1.4/src/kedro_graphql/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      676 2023-05-19 18:26:11.000000 kedro-graphql-0.1.4/src/kedro_graphql/asgi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:26:22.748717 kedro-graphql-0.1.4/src/kedro_graphql/backends/
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-05-19 18:26:11.000000 kedro-graphql-0.1.4/src/kedro_graphql/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      815 2023-05-19 18:26:11.000000 kedro-graphql-0.1.4/src/kedro_graphql/backends/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-05-19 18:26:11.000000 kedro-graphql-0.1.4/src/kedro_graphql/backends/mongodb.py
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-05-19 18:26:11.000000 kedro-graphql-0.1.4/src/kedro_graphql/celeryapp.py
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-05-19 18:26:11.000000 kedro-graphql-0.1.4/src/kedro_graphql/celeryconfig.py
--rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-05-19 18:26:11.000000 kedro-graphql-0.1.4/src/kedro_graphql/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-05-19 18:26:11.000000 kedro-graphql-0.1.4/src/kedro_graphql/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-05-19 18:26:11.000000 kedro-graphql-0.1.4/src/kedro_graphql/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     4791 2023-05-19 18:26:11.000000 kedro-graphql-0.1.4/src/kedro_graphql/events.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:26:22.748717 kedro-graphql-0.1.4/src/kedro_graphql/example/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 18:26:11.000000 kedro-graphql-0.1.4/src/kedro_graphql/example/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-05-19 18:26:11.000000 kedro-graphql-0.1.4/src/kedro_graphql/example/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     7055 2023-05-19 18:26:11.000000 kedro-graphql-0.1.4/src/kedro_graphql/models.py
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-05-19 18:26:11.000000 kedro-graphql-0.1.4/src/kedro_graphql/pipeline_registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:26:22.748717 kedro-graphql-0.1.4/src/kedro_graphql/pipelines/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 18:26:11.000000 kedro-graphql-0.1.4/src/kedro_graphql/pipelines/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:26:22.748717 kedro-graphql-0.1.4/src/kedro_graphql/pipelines/example00/
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-05-19 18:26:11.000000 kedro-graphql-0.1.4/src/kedro_graphql/pipelines/example00/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-05-19 18:26:11.000000 kedro-graphql-0.1.4/src/kedro_graphql/pipelines/example00/nodes.py
--rw-r--r--   0 runner    (1001) docker     (123)      402 2023-05-19 18:26:11.000000 kedro-graphql-0.1.4/src/kedro_graphql/pipelines/example00/pipeline.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:26:22.748717 kedro-graphql-0.1.4/src/kedro_graphql/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 18:26:11.000000 kedro-graphql-0.1.4/src/kedro_graphql/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-05-19 18:26:11.000000 kedro-graphql-0.1.4/src/kedro_graphql/plugins/plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)     3059 2023-05-19 18:26:11.000000 kedro-graphql-0.1.4/src/kedro_graphql/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-05-19 18:26:11.000000 kedro-graphql-0.1.4/src/kedro_graphql/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     4196 2023-05-19 18:26:11.000000 kedro-graphql-0.1.4/src/kedro_graphql/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:26:22.748717 kedro-graphql-0.1.4/src/kedro_graphql.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10675 2023-05-19 18:26:22.000000 kedro-graphql-0.1.4/src/kedro_graphql.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-05-19 18:26:22.000000 kedro-graphql-0.1.4/src/kedro_graphql.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 18:26:22.000000 kedro-graphql-0.1.4/src/kedro_graphql.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-19 18:26:22.000000 kedro-graphql-0.1.4/src/kedro_graphql.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-19 18:26:22.000000 kedro-graphql-0.1.4/src/kedro_graphql.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-19 18:26:22.000000 kedro-graphql-0.1.4/src/kedro_graphql.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-05-19 18:26:11.000000 kedro-graphql-0.1.4/src/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-05-19 18:26:11.000000 kedro-graphql-0.1.4/src/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:26:22.748717 kedro-graphql-0.1.4/src/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 18:26:11.000000 kedro-graphql-0.1.4/src/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3383 2023-05-19 18:26:11.000000 kedro-graphql-0.1.4/src/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:26:22.748717 kedro-graphql-0.1.4/src/tests/pipelines/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 18:26:11.000000 kedro-graphql-0.1.4/src/tests/pipelines/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:26:22.748717 kedro-graphql-0.1.4/src/tests/pipelines/example00/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 18:26:11.000000 kedro-graphql-0.1.4/src/tests/pipelines/example00/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-05-19 18:26:11.000000 kedro-graphql-0.1.4/src/tests/pipelines/example00/test_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     3040 2023-05-19 18:26:11.000000 kedro-graphql-0.1.4/src/tests/test_events.py
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-05-19 18:26:11.000000 kedro-graphql-0.1.4/src/tests/test_run.py
--rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-05-19 18:26:11.000000 kedro-graphql-0.1.4/src/tests/test_schema_mutation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-05-19 18:26:11.000000 kedro-graphql-0.1.4/src/tests/test_schema_query.py
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-05-19 18:26:11.000000 kedro-graphql-0.1.4/src/tests/test_schema_subscription.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:49:53.104714 kedro-graphql-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-22 20:49:41.000000 kedro-graphql-0.2.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    10675 2023-05-22 20:49:53.104714 kedro-graphql-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10120 2023-05-22 20:49:41.000000 kedro-graphql-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-05-22 20:49:41.000000 kedro-graphql-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-22 20:49:53.108714 kedro-graphql-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:49:53.100714 kedro-graphql-0.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:49:53.104714 kedro-graphql-0.2.0/src/kedro_graphql/
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-22 20:49:41.000000 kedro-graphql-0.2.0/src/kedro_graphql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-05-22 20:49:41.000000 kedro-graphql-0.2.0/src/kedro_graphql/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-05-22 20:49:41.000000 kedro-graphql-0.2.0/src/kedro_graphql/asgi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:49:53.104714 kedro-graphql-0.2.0/src/kedro_graphql/backends/
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-05-22 20:49:41.000000 kedro-graphql-0.2.0/src/kedro_graphql/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-05-22 20:49:41.000000 kedro-graphql-0.2.0/src/kedro_graphql/backends/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-05-22 20:49:41.000000 kedro-graphql-0.2.0/src/kedro_graphql/backends/mongodb.py
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-05-22 20:49:41.000000 kedro-graphql-0.2.0/src/kedro_graphql/celeryapp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-05-22 20:49:41.000000 kedro-graphql-0.2.0/src/kedro_graphql/celeryconfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-05-22 20:49:41.000000 kedro-graphql-0.2.0/src/kedro_graphql/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-05-22 20:49:41.000000 kedro-graphql-0.2.0/src/kedro_graphql/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-05-22 20:49:41.000000 kedro-graphql-0.2.0/src/kedro_graphql/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4791 2023-05-22 20:49:41.000000 kedro-graphql-0.2.0/src/kedro_graphql/events.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:49:53.104714 kedro-graphql-0.2.0/src/kedro_graphql/example/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 20:49:41.000000 kedro-graphql-0.2.0/src/kedro_graphql/example/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-05-22 20:49:41.000000 kedro-graphql-0.2.0/src/kedro_graphql/example/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7401 2023-05-22 20:49:41.000000 kedro-graphql-0.2.0/src/kedro_graphql/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-05-22 20:49:41.000000 kedro-graphql-0.2.0/src/kedro_graphql/pipeline_registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:49:53.104714 kedro-graphql-0.2.0/src/kedro_graphql/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 20:49:41.000000 kedro-graphql-0.2.0/src/kedro_graphql/pipelines/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:49:53.104714 kedro-graphql-0.2.0/src/kedro_graphql/pipelines/example00/
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-05-22 20:49:41.000000 kedro-graphql-0.2.0/src/kedro_graphql/pipelines/example00/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-05-22 20:49:41.000000 kedro-graphql-0.2.0/src/kedro_graphql/pipelines/example00/nodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-05-22 20:49:41.000000 kedro-graphql-0.2.0/src/kedro_graphql/pipelines/example00/pipeline.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:49:53.104714 kedro-graphql-0.2.0/src/kedro_graphql/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 20:49:41.000000 kedro-graphql-0.2.0/src/kedro_graphql/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-05-22 20:49:41.000000 kedro-graphql-0.2.0/src/kedro_graphql/plugins/plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3223 2023-05-22 20:49:41.000000 kedro-graphql-0.2.0/src/kedro_graphql/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-05-22 20:49:41.000000 kedro-graphql-0.2.0/src/kedro_graphql/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4196 2023-05-22 20:49:41.000000 kedro-graphql-0.2.0/src/kedro_graphql/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:49:53.104714 kedro-graphql-0.2.0/src/kedro_graphql.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10675 2023-05-22 20:49:53.000000 kedro-graphql-0.2.0/src/kedro_graphql.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-05-22 20:49:53.000000 kedro-graphql-0.2.0/src/kedro_graphql.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 20:49:53.000000 kedro-graphql-0.2.0/src/kedro_graphql.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-22 20:49:53.000000 kedro-graphql-0.2.0/src/kedro_graphql.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-22 20:49:53.000000 kedro-graphql-0.2.0/src/kedro_graphql.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-22 20:49:53.000000 kedro-graphql-0.2.0/src/kedro_graphql.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-05-22 20:49:41.000000 kedro-graphql-0.2.0/src/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-05-22 20:49:41.000000 kedro-graphql-0.2.0/src/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:49:53.104714 kedro-graphql-0.2.0/src/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 20:49:41.000000 kedro-graphql-0.2.0/src/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3524 2023-05-22 20:49:41.000000 kedro-graphql-0.2.0/src/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:49:53.104714 kedro-graphql-0.2.0/src/tests/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 20:49:41.000000 kedro-graphql-0.2.0/src/tests/pipelines/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:49:53.104714 kedro-graphql-0.2.0/src/tests/pipelines/example00/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 20:49:41.000000 kedro-graphql-0.2.0/src/tests/pipelines/example00/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-05-22 20:49:41.000000 kedro-graphql-0.2.0/src/tests/pipelines/example00/test_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3040 2023-05-22 20:49:41.000000 kedro-graphql-0.2.0/src/tests/test_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-05-22 20:49:41.000000 kedro-graphql-0.2.0/src/tests/test_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-05-22 20:49:41.000000 kedro-graphql-0.2.0/src/tests/test_schema_mutation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-05-22 20:49:41.000000 kedro-graphql-0.2.0/src/tests/test_schema_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-05-22 20:49:41.000000 kedro-graphql-0.2.0/src/tests/test_schema_subscription.py
```

### Comparing `kedro-graphql-0.1.4/LICENSE.txt` & `kedro-graphql-0.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `kedro-graphql-0.1.4/PKG-INFO` & `kedro-graphql-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kedro-graphql
-Version: 0.1.4
+Version: 0.2.0
 Summary: Kedro helps you build production-ready data and analytics pipelines
 Author: opensean
 License: Apache Software License (Apache 2.0)
 Project-URL: Homepage, https://github.com/opensean/kedro-graphql
 Project-URL: Source, https://github.com/opensean/kedro-graphql
 Keywords: pipelines,machine learning,data pipelines,data science,data engineering
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `kedro-graphql-0.1.4/README.md` & `kedro-graphql-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `kedro-graphql-0.1.4/pyproject.toml` & `kedro-graphql-0.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `kedro-graphql-0.1.4/src/kedro_graphql/__main__.py` & `kedro-graphql-0.2.0/src/kedro_graphql/__main__.py`

 * *Files identical despite different names*

### Comparing `kedro-graphql-0.1.4/src/kedro_graphql/asgi.py` & `kedro-graphql-0.2.0/src/kedro_graphql/asgi.py`

 * *Files identical despite different names*

### Comparing `kedro-graphql-0.1.4/src/kedro_graphql/backends/base.py` & `kedro-graphql-0.2.0/src/kedro_graphql/backends/base.py`

 * *Files identical despite different names*

### Comparing `kedro-graphql-0.1.4/src/kedro_graphql/backends/mongodb.py` & `kedro-graphql-0.2.0/src/kedro_graphql/backends/mongodb.py`

 * *Files identical despite different names*

### Comparing `kedro-graphql-0.1.4/src/kedro_graphql/commands.py` & `kedro-graphql-0.2.0/src/kedro_graphql/commands.py`

 * *Files identical despite different names*

### Comparing `kedro-graphql-0.1.4/src/kedro_graphql/config.py` & `kedro-graphql-0.2.0/src/kedro_graphql/config.py`

 * *Files identical despite different names*

### Comparing `kedro-graphql-0.1.4/src/kedro_graphql/decorators.py` & `kedro-graphql-0.2.0/src/kedro_graphql/decorators.py`

 * *Files identical despite different names*

### Comparing `kedro-graphql-0.1.4/src/kedro_graphql/events.py` & `kedro-graphql-0.2.0/src/kedro_graphql/events.py`

 * *Files identical despite different names*

### Comparing `kedro-graphql-0.1.4/src/kedro_graphql/example/app.py` & `kedro-graphql-0.2.0/src/kedro_graphql/example/app.py`

 * *Files identical despite different names*

### Comparing `kedro-graphql-0.1.4/src/kedro_graphql/models.py` & `kedro-graphql-0.2.0/src/kedro_graphql/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,23 @@
 import strawberry
 from typing import List, Optional
 import uuid
 from .config import conf_catalog, conf_parameters, PIPELINES
 
 @strawberry.type
+class Tag:
+    key: str
+    value: str
+
+@strawberry.input
+class TagInput:
+    key: str
+    value: str
+
+@strawberry.type
 class Parameter:
     name: str
     value: str
 
     def serialize(self) -> dict:
         """
         Returns serializable dict in format compatible with kedro.
@@ -143,23 +153,25 @@
 
 @strawberry.input(description = "PipelineInput")
 class PipelineInput:
     name: str
     parameters: List[ParameterInput]
     inputs: List[DataSetInput]
     outputs: List[DataSetInput]
+    tags: Optional[List[TagInput]] = None
 
 @strawberry.type
 class Pipeline:
     id: Optional[uuid.UUID] = None
     inputs: List[DataSet]
     name: str
     outputs: List[DataSet]
     parameters: List[Parameter]
     status: Optional[str] = None
+    tags: Optional[List[Tag]] = None
     task_id: Optional[str] = None
     task_name: Optional[str] = None
     task_args: Optional[str] = None
     task_kwargs: Optional[str] = None
     task_request: Optional[str] = None
     task_exception: Optional[str] = None
     task_traceback: Optional[str] = None
@@ -200,21 +212,27 @@
             "inputs": inputs,
             "outputs": outputs,
             "parameters": parameters,
         }
 
     @staticmethod
     def from_dict(payload):
+        if payload["tags"]:
+            tags = [Tag(**t) for t in payload["tags"]]
+        else:
+            tags = None
+
         return Pipeline(
             id = payload.get("id", None),
             name = payload["name"],
             inputs = [DataSet.from_dict(i) for i in payload["inputs"]],
             outputs = [DataSet.from_dict(o) for o in payload["outputs"]],
             parameters = [Parameter(**p) for p in payload["parameters"]],
             status = payload.get("status", None),
+            tags = tags,
             task_id = payload.get("task_id", None),
             task_name = payload.get("task_name", None),
             task_args = payload.get("task_args", None),
             task_kwargs = payload.get("task_kwargs", None),
             task_request = payload.get("task_request", None),
             task_exception = payload.get("task_exception", None),
             task_traceback = payload.get("task_traceback", None),
```

### Comparing `kedro-graphql-0.1.4/src/kedro_graphql/plugins/plugins.py` & `kedro-graphql-0.2.0/src/kedro_graphql/plugins/plugins.py`

 * *Files identical despite different names*

### Comparing `kedro-graphql-0.1.4/src/kedro_graphql/schema.py` & `kedro-graphql-0.2.0/src/kedro_graphql/schema.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from .events import PipelineEventMonitor
 import strawberry
 from strawberry.tools import merge_types
 from strawberry.types import Info
 from typing import AsyncGenerator, List
 from .celeryapp import app as APP_CELERY
 from .tasks import run_pipeline
-from .models import Parameter, ParameterInput, DataSet, DataSetInput, Pipeline, PipelineInput, PipelineEvent, PipelineTemplate
+from .models import Parameter, ParameterInput, DataSet, DataSetInput, Pipeline, PipelineInput, PipelineEvent, PipelineTemplate, Tag, TagInput
 
 @strawberry.type
 class Query:
     @strawberry.field
     def pipeline_templates(self) -> List[PipelineTemplate]:
         pipes = []
         for k,v in PIPELINES.items():
@@ -26,19 +26,25 @@
 class Mutation:
     @strawberry.mutation
     def pipeline(self, pipeline: PipelineInput, info: Info) -> Pipeline:
         """
         - fill in missing values from default catalog?
         - is validation against template needed, e.g. check DataSet type?
         """
+        if pipeline.tags:
+            tags = [Tag(**vars(t)) for t in pipeline.tags]
+        else:
+            tags = None
+
         p = Pipeline(
             name = pipeline.name,
             inputs = [DataSet(**vars(i)) for i in pipeline.inputs],
             outputs = [DataSet(**vars(o)) for o in pipeline.outputs],
             parameters = [Parameter(**vars(p)) for p in pipeline.parameters],
+            tags = tags,
             task_name = str(run_pipeline),
         )
 
         serial = p.serialize()
 
         result = run_pipeline.delay(
             name = serial["name"],
```

### Comparing `kedro-graphql-0.1.4/src/kedro_graphql/settings.py` & `kedro-graphql-0.2.0/src/kedro_graphql/settings.py`

 * *Files identical despite different names*

### Comparing `kedro-graphql-0.1.4/src/kedro_graphql/tasks.py` & `kedro-graphql-0.2.0/src/kedro_graphql/tasks.py`

 * *Files identical despite different names*

### Comparing `kedro-graphql-0.1.4/src/kedro_graphql.egg-info/PKG-INFO` & `kedro-graphql-0.2.0/src/kedro_graphql.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kedro-graphql
-Version: 0.1.4
+Version: 0.2.0
 Summary: Kedro helps you build production-ready data and analytics pipelines
 Author: opensean
 License: Apache Software License (Apache 2.0)
 Project-URL: Homepage, https://github.com/opensean/kedro-graphql
 Project-URL: Source, https://github.com/opensean/kedro-graphql
 Keywords: pipelines,machine learning,data pipelines,data science,data engineering
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `kedro-graphql-0.1.4/src/kedro_graphql.egg-info/SOURCES.txt` & `kedro-graphql-0.2.0/src/kedro_graphql.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kedro-graphql-0.1.4/src/setup.py` & `kedro-graphql-0.2.0/src/setup.py`

 * *Files identical despite different names*

### Comparing `kedro-graphql-0.1.4/src/tests/conftest.py` & `kedro-graphql-0.2.0/src/tests/conftest.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 from kedro.framework.project import settings
 from kedro.config import ConfigLoader
 from kedro.framework.context import KedroContext
 from kedro.framework.hooks import _create_hook_manager
 from kedro_graphql.backends import init_backend
 from kedro_graphql.tasks import run_pipeline
-from kedro_graphql.models import Pipeline, DataSet, Parameter
+from kedro_graphql.models import Pipeline, DataSet, Parameter, Tag
 from unittest.mock import patch
 
 
 
 @pytest.fixture(scope="session")
 def config_loader():
     return ConfigLoader(conf_source=str(Path.cwd() / settings.CONF_SOURCE))
@@ -78,20 +78,22 @@
 
 @pytest.fixture
 def mock_pipeline(mock_backend, tmp_path, mock_text_in, mock_text_out):
 
     inputs = [{"name": "text_in", "type": "text.TextDataSet", "filepath": str(mock_text_in)}]
     outputs = [{"name":"text_out", "type": "text.TextDataSet", "filepath": str(mock_text_out)}]
     parameters = [{"name":"example", "value":"hello"}]
+    tags = [{"key": "author", "value": "opensean"},{"key":"package", "value":"kedro-graphql"}]
 
     p = Pipeline(
         name = "example00",
         inputs = [DataSet(**i) for i in inputs],
         outputs = [DataSet(**o) for o in outputs],
         parameters = [Parameter(**p) for p in parameters],
+        tags = [Tag(**p) for p in tags],
         task_name = str(run_pipeline),
     )
 
     serial = p.serialize()
 
     result = run_pipeline.apply_async(kwargs = {"name": "example00", 
                                                  "inputs": serial["inputs"],
```

### Comparing `kedro-graphql-0.1.4/src/tests/test_events.py` & `kedro-graphql-0.2.0/src/tests/test_events.py`

 * *Files identical despite different names*

### Comparing `kedro-graphql-0.1.4/src/tests/test_run.py` & `kedro-graphql-0.2.0/src/tests/test_run.py`

 * *Files identical despite different names*

### Comparing `kedro-graphql-0.1.4/src/tests/test_schema_mutation.py` & `kedro-graphql-0.2.0/src/tests/test_schema_mutation.py`

 * *Files 9% similar despite different names*

```diff
@@ -36,14 +36,18 @@
               type
             }
             parameters {
               name
               value
             }
             status
+            tags {
+              key
+              value
+            }
             taskId
             taskName
             taskArgs
             taskKwargs
             taskRequest
             taskException
             taskTraceback
@@ -54,11 +58,12 @@
         """
 
         resp = await schema.execute(mutation, 
                                     variable_values = {"pipeline": {
                                       "name": "example00",
                                       "inputs": [{"name": "text_in", "type": "text.TextDataSet", "filepath": str(mock_text_in)}],
                                       "outputs": [{"name": "text_out", "type": "text.TextDataSet", "filepath": str(mock_text_out)}],
-                                      "parameters": [{"name":"example", "value":"hello"}] 
+                                      "parameters": [{"name":"example", "value":"hello"}],
+                                      "tags": [{"key": "author", "value": "opensean"},{"key":"package", "value":"kedro-graphql"}]
                                     }})
         
         assert resp.errors is None
```

### Comparing `kedro-graphql-0.1.4/src/tests/test_schema_query.py` & `kedro-graphql-0.2.0/src/tests/test_schema_query.py`

 * *Files identical despite different names*

### Comparing `kedro-graphql-0.1.4/src/tests/test_schema_subscription.py` & `kedro-graphql-0.2.0/src/tests/test_schema_subscription.py`

 * *Files identical despite different names*

