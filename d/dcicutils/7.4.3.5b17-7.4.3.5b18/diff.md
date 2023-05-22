# Comparing `tmp/dcicutils-7.4.3.5b17.tar.gz` & `tmp/dcicutils-7.4.3.5b18.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dcicutils-7.4.3.5b17.tar", max compression
+gzip compressed data, was "dcicutils-7.4.3.5b18.tar", max compression
```

## Comparing `dcicutils-7.4.3.5b17.tar` & `dcicutils-7.4.3.5b18.tar`

### file list

```diff
@@ -1,51 +1,51 @@
--rw-r--r--   0        0        0     1098 2023-05-22 01:31:48.665995 dcicutils-7.4.3.5b17/LICENSE.txt
--rw-r--r--   0        0        0     1166 2023-05-22 01:31:48.665995 dcicutils-7.4.3.5b17/README.rst
--rw-r--r--   0        0        0        0 2023-05-22 01:31:48.665995 dcicutils-7.4.3.5b17/dcicutils/__init__.py
--rw-r--r--   0        0        0     5115 2023-05-22 01:31:48.665995 dcicutils-7.4.3.5b17/dcicutils/base.py
--rwxr-xr-x   0        0        0    51434 2023-05-22 01:31:48.669995 dcicutils-7.4.3.5b17/dcicutils/beanstalk_utils.py
--rw-r--r--   0        0        0    13786 2023-05-22 01:31:48.669995 dcicutils-7.4.3.5b17/dcicutils/cloudformation_utils.py
--rw-r--r--   0        0        0     1155 2023-05-22 01:31:48.669995 dcicutils-7.4.3.5b17/dcicutils/codebuild_utils.py
--rw-r--r--   0        0        0    15285 2023-05-22 01:31:48.669995 dcicutils-7.4.3.5b17/dcicutils/command_utils.py
--rw-r--r--   0        0        0     3723 2023-05-22 01:31:48.669995 dcicutils-7.4.3.5b17/dcicutils/common.py
--rw-r--r--   0        0        0    11032 2023-05-22 01:31:48.669995 dcicutils-7.4.3.5b17/dcicutils/creds_utils.py
--rw-r--r--   0        0        0     3098 2023-05-22 01:31:48.669995 dcicutils-7.4.3.5b17/dcicutils/data_utils.py
--rw-r--r--   0        0        0    68354 2023-05-22 01:31:48.669995 dcicutils-7.4.3.5b17/dcicutils/deployment_utils.py
--rw-r--r--   0        0        0     8118 2023-05-22 01:31:48.669995 dcicutils-7.4.3.5b17/dcicutils/diff_utils.py
--rw-r--r--   0        0        0     1747 2023-05-22 01:31:48.669995 dcicutils-7.4.3.5b17/dcicutils/docker_utils.py
--rw-r--r--   0        0        0    19474 2023-05-22 01:31:48.669995 dcicutils-7.4.3.5b17/dcicutils/ecr_scripts.py
--rw-r--r--   0        0        0    13079 2023-05-22 01:31:48.669995 dcicutils-7.4.3.5b17/dcicutils/ecr_utils.py
--rw-r--r--   0        0        0     3590 2023-05-22 01:31:48.669995 dcicutils-7.4.3.5b17/dcicutils/ecs_utils.py
--rw-r--r--   0        0        0     6356 2023-05-22 01:31:48.669995 dcicutils-7.4.3.5b17/dcicutils/env_base.py
--rw-r--r--   0        0        0     9444 2023-05-22 01:31:48.669995 dcicutils-7.4.3.5b17/dcicutils/env_manager.py
--rw-r--r--   0        0        0     3909 2023-05-22 01:31:48.669995 dcicutils-7.4.3.5b17/dcicutils/env_scripts.py
--rw-r--r--   0        0        0    46739 2023-05-22 01:31:48.669995 dcicutils-7.4.3.5b17/dcicutils/env_utils.py
--rw-r--r--   0        0        0    29032 2023-05-22 01:31:48.669995 dcicutils-7.4.3.5b17/dcicutils/env_utils_legacy.py
--rw-r--r--   0        0        0     7541 2023-05-22 01:31:48.669995 dcicutils-7.4.3.5b17/dcicutils/es_utils.py
--rw-r--r--   0        0        0     9931 2023-05-22 01:31:48.669995 dcicutils-7.4.3.5b17/dcicutils/exceptions.py
--rw-r--r--   0        0        0    36918 2023-05-22 01:31:48.669995 dcicutils-7.4.3.5b17/dcicutils/ff_mocks.py
--rw-r--r--   0        0        0    66453 2023-05-22 01:31:48.669995 dcicutils-7.4.3.5b17/dcicutils/ff_utils.py
--rw-r--r--   0        0        0    10026 2023-05-22 01:31:48.669995 dcicutils-7.4.3.5b17/dcicutils/function_cache_decorator.py
--rw-r--r--   0        0        0    33704 2023-05-22 01:31:48.669995 dcicutils-7.4.3.5b17/dcicutils/glacier_utils.py
--rw-r--r--   0        0        0    11502 2023-05-22 01:31:48.669995 dcicutils-7.4.3.5b17/dcicutils/jh_utils.py
--rw-r--r--   0        0        0    16225 2023-05-22 01:31:48.669995 dcicutils-7.4.3.5b17/dcicutils/kibana/dashboards.json
--rw-r--r--   0        0        0     2164 2023-05-22 01:31:48.669995 dcicutils-7.4.3.5b17/dcicutils/kibana/readme.md
--rw-r--r--   0        0        0    27302 2023-05-22 01:31:48.669995 dcicutils-7.4.3.5b17/dcicutils/lang_utils.py
--rw-r--r--   0        0        0    10883 2023-05-22 01:31:48.669995 dcicutils-7.4.3.5b17/dcicutils/log_utils.py
--rw-r--r--   0        0        0    90749 2023-05-22 01:31:48.669995 dcicutils-7.4.3.5b17/dcicutils/misc_utils.py
--rw-r--r--   0        0        0     5963 2023-05-22 01:31:48.669995 dcicutils-7.4.3.5b17/dcicutils/obfuscation_utils.py
--rw-r--r--   0        0        0     1017 2023-05-22 01:31:48.669995 dcicutils-7.4.3.5b17/dcicutils/opensearch_utils.py
--rw-r--r--   0        0        0    28244 2023-05-22 01:31:48.669995 dcicutils-7.4.3.5b17/dcicutils/project_utils.py
--rw-r--r--   0        0        0    20234 2023-05-22 01:31:48.669995 dcicutils-7.4.3.5b17/dcicutils/qa_checkers.py
--rw-r--r--   0        0        0   156269 2023-05-22 01:31:48.673995 dcicutils-7.4.3.5b17/dcicutils/qa_utils.py
--rw-r--r--   0        0        0     6509 2023-05-22 01:31:48.673995 dcicutils-7.4.3.5b17/dcicutils/redis_tools.py
--rw-r--r--   0        0        0     6462 2023-05-22 01:31:48.673995 dcicutils-7.4.3.5b17/dcicutils/redis_utils.py
--rw-r--r--   0        0        0    28852 2023-05-22 01:31:48.673995 dcicutils-7.4.3.5b17/dcicutils/s3_utils.py
--rw-r--r--   0        0        0    11044 2023-05-22 01:31:48.673995 dcicutils-7.4.3.5b17/dcicutils/scripts/publish_to_pypi.py
--rw-r--r--   0        0        0    19745 2023-05-22 01:31:48.673995 dcicutils-7.4.3.5b17/dcicutils/secrets_utils.py
--rw-r--r--   0        0        0    22961 2023-05-22 01:31:48.673995 dcicutils-7.4.3.5b17/dcicutils/snapshot_utils.py
--rw-r--r--   0        0        0     9707 2023-05-22 01:31:48.673995 dcicutils-7.4.3.5b17/dcicutils/ssl_certificate_utils.py
--rw-r--r--   0        0        0     8082 2023-05-22 01:31:48.673995 dcicutils-7.4.3.5b17/dcicutils/task_utils.py
--rw-r--r--   0        0        0     1769 2023-05-22 01:31:48.673995 dcicutils-7.4.3.5b17/dcicutils/trace_utils.py
--rw-r--r--   0        0        0     3968 2023-05-22 01:31:48.673995 dcicutils-7.4.3.5b17/pyproject.toml
--rw-r--r--   0        0        0     2665 1970-01-01 00:00:00.000000 dcicutils-7.4.3.5b17/setup.py
--rw-r--r--   0        0        0     3003 1970-01-01 00:00:00.000000 dcicutils-7.4.3.5b17/PKG-INFO
+-rw-r--r--   0        0        0     1098 2023-05-22 05:06:05.121567 dcicutils-7.4.3.5b18/LICENSE.txt
+-rw-r--r--   0        0        0     1166 2023-05-22 05:06:05.121567 dcicutils-7.4.3.5b18/README.rst
+-rw-r--r--   0        0        0        0 2023-05-22 05:06:05.121567 dcicutils-7.4.3.5b18/dcicutils/__init__.py
+-rw-r--r--   0        0        0     5115 2023-05-22 05:06:05.121567 dcicutils-7.4.3.5b18/dcicutils/base.py
+-rwxr-xr-x   0        0        0    51434 2023-05-22 05:06:05.121567 dcicutils-7.4.3.5b18/dcicutils/beanstalk_utils.py
+-rw-r--r--   0        0        0    13786 2023-05-22 05:06:05.121567 dcicutils-7.4.3.5b18/dcicutils/cloudformation_utils.py
+-rw-r--r--   0        0        0     1155 2023-05-22 05:06:05.121567 dcicutils-7.4.3.5b18/dcicutils/codebuild_utils.py
+-rw-r--r--   0        0        0    15285 2023-05-22 05:06:05.121567 dcicutils-7.4.3.5b18/dcicutils/command_utils.py
+-rw-r--r--   0        0        0     3723 2023-05-22 05:06:05.121567 dcicutils-7.4.3.5b18/dcicutils/common.py
+-rw-r--r--   0        0        0    11032 2023-05-22 05:06:05.125567 dcicutils-7.4.3.5b18/dcicutils/creds_utils.py
+-rw-r--r--   0        0        0     3098 2023-05-22 05:06:05.125567 dcicutils-7.4.3.5b18/dcicutils/data_utils.py
+-rw-r--r--   0        0        0    68354 2023-05-22 05:06:05.125567 dcicutils-7.4.3.5b18/dcicutils/deployment_utils.py
+-rw-r--r--   0        0        0     8118 2023-05-22 05:06:05.125567 dcicutils-7.4.3.5b18/dcicutils/diff_utils.py
+-rw-r--r--   0        0        0     1747 2023-05-22 05:06:05.125567 dcicutils-7.4.3.5b18/dcicutils/docker_utils.py
+-rw-r--r--   0        0        0    19474 2023-05-22 05:06:05.125567 dcicutils-7.4.3.5b18/dcicutils/ecr_scripts.py
+-rw-r--r--   0        0        0    13079 2023-05-22 05:06:05.125567 dcicutils-7.4.3.5b18/dcicutils/ecr_utils.py
+-rw-r--r--   0        0        0     3590 2023-05-22 05:06:05.125567 dcicutils-7.4.3.5b18/dcicutils/ecs_utils.py
+-rw-r--r--   0        0        0     6356 2023-05-22 05:06:05.125567 dcicutils-7.4.3.5b18/dcicutils/env_base.py
+-rw-r--r--   0        0        0     9444 2023-05-22 05:06:05.125567 dcicutils-7.4.3.5b18/dcicutils/env_manager.py
+-rw-r--r--   0        0        0     3909 2023-05-22 05:06:05.125567 dcicutils-7.4.3.5b18/dcicutils/env_scripts.py
+-rw-r--r--   0        0        0    46739 2023-05-22 05:06:05.125567 dcicutils-7.4.3.5b18/dcicutils/env_utils.py
+-rw-r--r--   0        0        0    29032 2023-05-22 05:06:05.125567 dcicutils-7.4.3.5b18/dcicutils/env_utils_legacy.py
+-rw-r--r--   0        0        0     7541 2023-05-22 05:06:05.125567 dcicutils-7.4.3.5b18/dcicutils/es_utils.py
+-rw-r--r--   0        0        0     9931 2023-05-22 05:06:05.125567 dcicutils-7.4.3.5b18/dcicutils/exceptions.py
+-rw-r--r--   0        0        0    36918 2023-05-22 05:06:05.125567 dcicutils-7.4.3.5b18/dcicutils/ff_mocks.py
+-rw-r--r--   0        0        0    66453 2023-05-22 05:06:05.125567 dcicutils-7.4.3.5b18/dcicutils/ff_utils.py
+-rw-r--r--   0        0        0    10026 2023-05-22 05:06:05.125567 dcicutils-7.4.3.5b18/dcicutils/function_cache_decorator.py
+-rw-r--r--   0        0        0    33704 2023-05-22 05:06:05.125567 dcicutils-7.4.3.5b18/dcicutils/glacier_utils.py
+-rw-r--r--   0        0        0    11502 2023-05-22 05:06:05.125567 dcicutils-7.4.3.5b18/dcicutils/jh_utils.py
+-rw-r--r--   0        0        0    16225 2023-05-22 05:06:05.125567 dcicutils-7.4.3.5b18/dcicutils/kibana/dashboards.json
+-rw-r--r--   0        0        0     2164 2023-05-22 05:06:05.125567 dcicutils-7.4.3.5b18/dcicutils/kibana/readme.md
+-rw-r--r--   0        0        0    27302 2023-05-22 05:06:05.125567 dcicutils-7.4.3.5b18/dcicutils/lang_utils.py
+-rw-r--r--   0        0        0    10883 2023-05-22 05:06:05.125567 dcicutils-7.4.3.5b18/dcicutils/log_utils.py
+-rw-r--r--   0        0        0    90749 2023-05-22 05:06:05.125567 dcicutils-7.4.3.5b18/dcicutils/misc_utils.py
+-rw-r--r--   0        0        0     5963 2023-05-22 05:06:05.125567 dcicutils-7.4.3.5b18/dcicutils/obfuscation_utils.py
+-rw-r--r--   0        0        0     1017 2023-05-22 05:06:05.125567 dcicutils-7.4.3.5b18/dcicutils/opensearch_utils.py
+-rw-r--r--   0        0        0    28276 2023-05-22 05:06:05.125567 dcicutils-7.4.3.5b18/dcicutils/project_utils.py
+-rw-r--r--   0        0        0    20234 2023-05-22 05:06:05.125567 dcicutils-7.4.3.5b18/dcicutils/qa_checkers.py
+-rw-r--r--   0        0        0   156269 2023-05-22 05:06:05.129567 dcicutils-7.4.3.5b18/dcicutils/qa_utils.py
+-rw-r--r--   0        0        0     6509 2023-05-22 05:06:05.129567 dcicutils-7.4.3.5b18/dcicutils/redis_tools.py
+-rw-r--r--   0        0        0     6462 2023-05-22 05:06:05.129567 dcicutils-7.4.3.5b18/dcicutils/redis_utils.py
+-rw-r--r--   0        0        0    28852 2023-05-22 05:06:05.129567 dcicutils-7.4.3.5b18/dcicutils/s3_utils.py
+-rw-r--r--   0        0        0    11044 2023-05-22 05:06:05.129567 dcicutils-7.4.3.5b18/dcicutils/scripts/publish_to_pypi.py
+-rw-r--r--   0        0        0    19745 2023-05-22 05:06:05.129567 dcicutils-7.4.3.5b18/dcicutils/secrets_utils.py
+-rw-r--r--   0        0        0    22961 2023-05-22 05:06:05.129567 dcicutils-7.4.3.5b18/dcicutils/snapshot_utils.py
+-rw-r--r--   0        0        0     9707 2023-05-22 05:06:05.129567 dcicutils-7.4.3.5b18/dcicutils/ssl_certificate_utils.py
+-rw-r--r--   0        0        0     8082 2023-05-22 05:06:05.129567 dcicutils-7.4.3.5b18/dcicutils/task_utils.py
+-rw-r--r--   0        0        0     1769 2023-05-22 05:06:05.129567 dcicutils-7.4.3.5b18/dcicutils/trace_utils.py
+-rw-r--r--   0        0        0     3968 2023-05-22 05:06:05.129567 dcicutils-7.4.3.5b18/pyproject.toml
+-rw-r--r--   0        0        0     2665 1970-01-01 00:00:00.000000 dcicutils-7.4.3.5b18/setup.py
+-rw-r--r--   0        0        0     3003 1970-01-01 00:00:00.000000 dcicutils-7.4.3.5b18/PKG-INFO
```

### Comparing `dcicutils-7.4.3.5b17/LICENSE.txt` & `dcicutils-7.4.3.5b18/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.3.5b17/README.rst` & `dcicutils-7.4.3.5b18/README.rst`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.3.5b17/dcicutils/base.py` & `dcicutils-7.4.3.5b18/dcicutils/base.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.3.5b17/dcicutils/beanstalk_utils.py` & `dcicutils-7.4.3.5b18/dcicutils/beanstalk_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.3.5b17/dcicutils/cloudformation_utils.py` & `dcicutils-7.4.3.5b18/dcicutils/cloudformation_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.3.5b17/dcicutils/codebuild_utils.py` & `dcicutils-7.4.3.5b18/dcicutils/codebuild_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.3.5b17/dcicutils/command_utils.py` & `dcicutils-7.4.3.5b18/dcicutils/command_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.3.5b17/dcicutils/common.py` & `dcicutils-7.4.3.5b18/dcicutils/common.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.3.5b17/dcicutils/creds_utils.py` & `dcicutils-7.4.3.5b18/dcicutils/creds_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.3.5b17/dcicutils/data_utils.py` & `dcicutils-7.4.3.5b18/dcicutils/data_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.3.5b17/dcicutils/deployment_utils.py` & `dcicutils-7.4.3.5b18/dcicutils/deployment_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.3.5b17/dcicutils/diff_utils.py` & `dcicutils-7.4.3.5b18/dcicutils/diff_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.3.5b17/dcicutils/docker_utils.py` & `dcicutils-7.4.3.5b18/dcicutils/docker_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.3.5b17/dcicutils/ecr_scripts.py` & `dcicutils-7.4.3.5b18/dcicutils/ecr_scripts.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.3.5b17/dcicutils/ecr_utils.py` & `dcicutils-7.4.3.5b18/dcicutils/ecr_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.3.5b17/dcicutils/ecs_utils.py` & `dcicutils-7.4.3.5b18/dcicutils/ecs_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.3.5b17/dcicutils/env_base.py` & `dcicutils-7.4.3.5b18/dcicutils/env_base.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.3.5b17/dcicutils/env_manager.py` & `dcicutils-7.4.3.5b18/dcicutils/env_manager.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.3.5b17/dcicutils/env_scripts.py` & `dcicutils-7.4.3.5b18/dcicutils/env_scripts.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.3.5b17/dcicutils/env_utils.py` & `dcicutils-7.4.3.5b18/dcicutils/env_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.3.5b17/dcicutils/env_utils_legacy.py` & `dcicutils-7.4.3.5b18/dcicutils/env_utils_legacy.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.3.5b17/dcicutils/es_utils.py` & `dcicutils-7.4.3.5b18/dcicutils/es_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.3.5b17/dcicutils/exceptions.py` & `dcicutils-7.4.3.5b18/dcicutils/exceptions.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.3.5b17/dcicutils/ff_mocks.py` & `dcicutils-7.4.3.5b18/dcicutils/ff_mocks.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.3.5b17/dcicutils/ff_utils.py` & `dcicutils-7.4.3.5b18/dcicutils/ff_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.3.5b17/dcicutils/function_cache_decorator.py` & `dcicutils-7.4.3.5b18/dcicutils/function_cache_decorator.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.3.5b17/dcicutils/glacier_utils.py` & `dcicutils-7.4.3.5b18/dcicutils/glacier_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.3.5b17/dcicutils/jh_utils.py` & `dcicutils-7.4.3.5b18/dcicutils/jh_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.3.5b17/dcicutils/kibana/dashboards.json` & `dcicutils-7.4.3.5b18/dcicutils/kibana/dashboards.json`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.3.5b17/dcicutils/kibana/readme.md` & `dcicutils-7.4.3.5b18/dcicutils/kibana/readme.md`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.3.5b17/dcicutils/lang_utils.py` & `dcicutils-7.4.3.5b18/dcicutils/lang_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.3.5b17/dcicutils/log_utils.py` & `dcicutils-7.4.3.5b18/dcicutils/log_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.3.5b17/dcicutils/misc_utils.py` & `dcicutils-7.4.3.5b18/dcicutils/misc_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.3.5b17/dcicutils/obfuscation_utils.py` & `dcicutils-7.4.3.5b18/dcicutils/obfuscation_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.3.5b17/dcicutils/opensearch_utils.py` & `dcicutils-7.4.3.5b18/dcicutils/opensearch_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.3.5b17/dcicutils/project_utils.py` & `dcicutils-7.4.3.5b18/dcicutils/project_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -337,18 +337,18 @@
 
 
 class ProjectRegistry:
 
     PROJECT_BASE_CLASS: Type[Project] = Project
 
     # If true, a herald will be shown; otherwise (if false), no herald will be shown
-    INITIALIZE_VERBOSE = environ_bool("PROJECT_INITIALIZE_VERBOSE", default=True)
+    PROJECT_INITIALIZE_VERBOSE = environ_bool("PROJECT_INITIALIZE_VERBOSE", default=True)
 
     # If true, any herald shown will have multi-line details; otherwise (if false), it'll be a single-line summary.
-    INITIALIZE_DETAILED = environ_bool("PROJECT_INITIALIZE_DETAILED", default=False)
+    PROJECT_INITIALIZE_DETAILED = environ_bool("PROJECT_INITIALIZE_DETAILED", default=False)
 
     REGISTERED_PROJECTS = {}
 
     # All of these might never be other than None so be careful when accessing them.
     APPLICATION_PROJECT_HOME = None
     PYPROJECT_TOML_FILE = None
     PYPROJECT_TOML = None
@@ -503,16 +503,16 @@
             raise ValueError(f"Registered pyproject {cls.PYPROJECT_NAME!r} ({project_class.__name__})"
                              f" is not a subclass of {cls.PROJECT_BASE_CLASS.__name__}.")
         project: Project = project_class()
         return project  # instantiate and return
 
     @classmethod
     def initialize(cls, force=False, verbose: Optional[bool] = None, detailed: Optional[bool] = None) -> Project:
-        show_herald = cls.INITIALIZE_VERBOSE if verbose is None else verbose
-        detailed = cls.INITIALIZE_DETAILED if detailed is None else detailed
+        show_herald = cls.PROJECT_INITIALIZE_VERBOSE if verbose is None else verbose
+        detailed = cls.PROJECT_INITIALIZE_DETAILED if detailed is None else detailed
         shared_app_project: Optional[Project] = _SHARED_APP_PROJECT_CELL.value
         if shared_app_project and not force:
             return shared_app_project
         _SHARED_APP_PROJECT_CELL.value = cls._make_project()
         app_project: Project = cls.app_project  # Now that it's initialized, make sure it comes from the right place
         if show_herald:
             app_project.show_herald(detailed=detailed)
```

### Comparing `dcicutils-7.4.3.5b17/dcicutils/qa_checkers.py` & `dcicutils-7.4.3.5b18/dcicutils/qa_checkers.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.3.5b17/dcicutils/qa_utils.py` & `dcicutils-7.4.3.5b18/dcicutils/qa_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.3.5b17/dcicutils/redis_tools.py` & `dcicutils-7.4.3.5b18/dcicutils/redis_tools.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.3.5b17/dcicutils/redis_utils.py` & `dcicutils-7.4.3.5b18/dcicutils/redis_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.3.5b17/dcicutils/s3_utils.py` & `dcicutils-7.4.3.5b18/dcicutils/s3_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.3.5b17/dcicutils/scripts/publish_to_pypi.py` & `dcicutils-7.4.3.5b18/dcicutils/scripts/publish_to_pypi.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.3.5b17/dcicutils/secrets_utils.py` & `dcicutils-7.4.3.5b18/dcicutils/secrets_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.3.5b17/dcicutils/snapshot_utils.py` & `dcicutils-7.4.3.5b18/dcicutils/snapshot_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.3.5b17/dcicutils/ssl_certificate_utils.py` & `dcicutils-7.4.3.5b18/dcicutils/ssl_certificate_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.3.5b17/dcicutils/task_utils.py` & `dcicutils-7.4.3.5b18/dcicutils/task_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.3.5b17/dcicutils/trace_utils.py` & `dcicutils-7.4.3.5b18/dcicutils/trace_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.3.5b17/pyproject.toml` & `dcicutils-7.4.3.5b18/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dcicutils"
-version = "7.4.3.5b17"  # to become 7.5.0
+version = "7.4.3.5b18"  # to become 7.5.0
 description = "Utility package for interacting with the 4DN Data Portal and other 4DN resources"
 authors = ["4DN-DCIC Team <support@4dnucleome.org>"]
 license = "MIT"
 readme = "README.rst"
 homepage = "https://github.com/4dn-dcic/utils"
 repository = "https://github.com/4dn-dcic/utils"
 packages = [
```

### Comparing `dcicutils-7.4.3.5b17/setup.py` & `dcicutils-7.4.3.5b18/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 
 entry_points = \
 {'console_scripts': ['publish-to-pypi = '
                      'dcicutils.scripts.publish_to_pypi:main']}
 
 setup_kwargs = {
     'name': 'dcicutils',
-    'version': '7.4.3.5b17',
+    'version': '7.4.3.5b18',
     'description': 'Utility package for interacting with the 4DN Data Portal and other 4DN resources',
     'long_description': '=====\nutils\n=====\n\nCheck out our full documentation `here <https://dcic-utils.readthedocs.io/en/latest/>`_\n\nThis repository contains various utility modules shared amongst several projects in the 4DN-DCIC. It is meant to be used internally by the DCIC team and externally as a Python API to `Fourfront <https://data.4dnucleome.org>`_\\ , the 4DN data portal.\n\npip installable as the ``dcicutils`` package with: ``pip install dcicutils``\n\nSee `this document <https://dcic-utils.readthedocs.io/en/latest/getting_started.html>`_ for tips on getting started. `Go here <https://dcic-utils.readthedocs.io/en/latest/examples.html>`_ for examples of some of the most useful functions.\n\n\n.. image:: https://travis-ci.org/4dn-dcic/utils.svg?branch=master\n   :target: https://travis-ci.org/4dn-dcic/utils\n   :alt: Build Status\n\n\n.. image:: https://coveralls.io/repos/github/4dn-dcic/utils/badge.svg?branch=master\n   :target: https://coveralls.io/github/4dn-dcic/utils?branch=master\n   :alt: Coverage\n\n.. image:: https://readthedocs.org/projects/dcic-utils/badge/?version=latest\n   :target: https://dcic-utils.readthedocs.io/en/latest/?badge=latest\n   :alt: Documentation Status\n',
     'author': '4DN-DCIC Team',
     'author_email': 'support@4dnucleome.org',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/4dn-dcic/utils',
```

### Comparing `dcicutils-7.4.3.5b17/PKG-INFO` & `dcicutils-7.4.3.5b18/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcicutils
-Version: 7.4.3.5b17
+Version: 7.4.3.5b18
 Summary: Utility package for interacting with the 4DN Data Portal and other 4DN resources
 Home-page: https://github.com/4dn-dcic/utils
 License: MIT
 Author: 4DN-DCIC Team
 Author-email: support@4dnucleome.org
 Requires-Python: >=3.7,<3.10
 Classifier: Development Status :: 4 - Beta
```

