# Comparing `tmp/manifest-ml-0.1.7.tar.gz` & `tmp/manifest-ml-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "manifest-ml-0.1.7.tar", last modified: Wed May 17 23:44:42 2023, max compression
+gzip compressed data, was "manifest-ml-0.1.8.tar", last modified: Mon May 22 17:54:12 2023, max compression
```

## Comparing `manifest-ml-0.1.7.tar` & `manifest-ml-0.1.8.tar`

### file list

```diff
@@ -1,71 +1,75 @@
-drwxr-xr-x   0 laurelorr   (501) staff       (20)        0 2023-05-17 23:44:42.197950 manifest-ml-0.1.7/
--rw-r--r--   0 laurelorr   (501) staff       (20)    11357 2023-02-14 19:01:23.000000 manifest-ml-0.1.7/LICENSE
--rw-r--r--   0 laurelorr   (501) staff       (20)    10728 2023-05-17 23:44:42.197169 manifest-ml-0.1.7/PKG-INFO
--rw-r--r--   0 laurelorr   (501) staff       (20)    10040 2023-05-17 05:53:01.000000 manifest-ml-0.1.7/README.md
-drwxr-xr-x   0 laurelorr   (501) staff       (20)        0 2023-05-17 23:44:42.185554 manifest-ml-0.1.7/manifest/
--rw-r--r--   0 laurelorr   (501) staff       (20)      183 2023-03-12 04:05:54.000000 manifest-ml-0.1.7/manifest/__init__.py
-drwxr-xr-x   0 laurelorr   (501) staff       (20)        0 2023-05-17 23:44:42.186284 manifest-ml-0.1.7/manifest/api/
--rw-r--r--   0 laurelorr   (501) staff       (20)       16 2023-02-14 19:01:23.000000 manifest-ml-0.1.7/manifest/api/__init__.py
--rw-r--r--   0 laurelorr   (501) staff       (20)     8947 2023-04-16 20:56:11.000000 manifest-ml-0.1.7/manifest/api/app.py
-drwxr-xr-x   0 laurelorr   (501) staff       (20)        0 2023-05-17 23:44:42.187795 manifest-ml-0.1.7/manifest/api/models/
--rw-r--r--   0 laurelorr   (501) staff       (20)       19 2023-02-14 19:01:23.000000 manifest-ml-0.1.7/manifest/api/models/__init__.py
--rw-r--r--   0 laurelorr   (501) staff       (20)     4383 2023-04-09 06:56:02.000000 manifest-ml-0.1.7/manifest/api/models/diffuser.py
--rw-r--r--   0 laurelorr   (501) staff       (20)    23667 2023-05-17 05:53:01.000000 manifest-ml-0.1.7/manifest/api/models/huggingface.py
--rw-r--r--   0 laurelorr   (501) staff       (20)     2798 2023-04-09 06:56:02.000000 manifest-ml-0.1.7/manifest/api/models/model.py
--rw-r--r--   0 laurelorr   (501) staff       (20)     3880 2023-04-09 06:56:02.000000 manifest-ml-0.1.7/manifest/api/models/sentence_transformer.py
--rw-r--r--   0 laurelorr   (501) staff       (20)     1767 2023-04-17 05:07:52.000000 manifest-ml-0.1.7/manifest/api/response.py
-drwxr-xr-x   0 laurelorr   (501) staff       (20)        0 2023-05-17 23:44:42.189549 manifest-ml-0.1.7/manifest/caches/
--rw-r--r--   0 laurelorr   (501) staff       (20)       18 2023-02-14 19:01:23.000000 manifest-ml-0.1.7/manifest/caches/__init__.py
--rw-r--r--   0 laurelorr   (501) staff       (20)     3725 2023-02-14 19:01:23.000000 manifest-ml-0.1.7/manifest/caches/array_cache.py
--rw-r--r--   0 laurelorr   (501) staff       (20)     4386 2023-04-24 18:36:42.000000 manifest-ml-0.1.7/manifest/caches/cache.py
--rw-r--r--   0 laurelorr   (501) staff       (20)     1131 2023-02-14 19:01:23.000000 manifest-ml-0.1.7/manifest/caches/noop.py
--rw-r--r--   0 laurelorr   (501) staff       (20)     3944 2023-03-12 04:05:54.000000 manifest-ml-0.1.7/manifest/caches/postgres.py
--rw-r--r--   0 laurelorr   (501) staff       (20)     1716 2023-02-14 19:01:23.000000 manifest-ml-0.1.7/manifest/caches/redis.py
--rw-r--r--   0 laurelorr   (501) staff       (20)     5997 2023-04-24 18:36:42.000000 manifest-ml-0.1.7/manifest/caches/serializers.py
--rw-r--r--   0 laurelorr   (501) staff       (20)     1772 2023-02-14 19:01:23.000000 manifest-ml-0.1.7/manifest/caches/sqlite.py
-drwxr-xr-x   0 laurelorr   (501) staff       (20)        0 2023-05-17 23:44:42.192626 manifest-ml-0.1.7/manifest/clients/
--rw-r--r--   0 laurelorr   (501) staff       (20)       19 2023-02-14 19:01:23.000000 manifest-ml-0.1.7/manifest/clients/__init__.py
--rw-r--r--   0 laurelorr   (501) staff       (20)     3303 2023-04-24 18:36:42.000000 manifest-ml-0.1.7/manifest/clients/ai21.py
--rw-r--r--   0 laurelorr   (501) staff       (20)    14482 2023-05-17 23:04:40.000000 manifest-ml-0.1.7/manifest/clients/client.py
--rw-r--r--   0 laurelorr   (501) staff       (20)     3461 2023-04-24 18:36:42.000000 manifest-ml-0.1.7/manifest/clients/cohere.py
--rw-r--r--   0 laurelorr   (501) staff       (20)     2821 2023-04-24 18:36:42.000000 manifest-ml-0.1.7/manifest/clients/diffuser.py
--rw-r--r--   0 laurelorr   (501) staff       (20)     5717 2023-05-04 04:43:35.000000 manifest-ml-0.1.7/manifest/clients/dummy.py
--rw-r--r--   0 laurelorr   (501) staff       (20)     3751 2023-05-04 04:43:35.000000 manifest-ml-0.1.7/manifest/clients/huggingface.py
--rw-r--r--   0 laurelorr   (501) staff       (20)     2336 2023-04-24 18:36:42.000000 manifest-ml-0.1.7/manifest/clients/huggingface_embedding.py
--rw-r--r--   0 laurelorr   (501) staff       (20)     4810 2023-04-24 19:18:15.000000 manifest-ml-0.1.7/manifest/clients/openai.py
--rw-r--r--   0 laurelorr   (501) staff       (20)     5801 2023-05-17 05:53:01.000000 manifest-ml-0.1.7/manifest/clients/openai_chat.py
--rw-r--r--   0 laurelorr   (501) staff       (20)     6560 2023-04-24 18:36:42.000000 manifest-ml-0.1.7/manifest/clients/openai_embedding.py
--rw-r--r--   0 laurelorr   (501) staff       (20)     5164 2023-04-24 18:36:42.000000 manifest-ml-0.1.7/manifest/clients/toma.py
--rw-r--r--   0 laurelorr   (501) staff       (20)     1940 2023-04-24 18:36:42.000000 manifest-ml-0.1.7/manifest/clients/toma_diffuser.py
-drwxr-xr-x   0 laurelorr   (501) staff       (20)        0 2023-05-17 23:44:42.193220 manifest-ml-0.1.7/manifest/connections/
--rw-r--r--   0 laurelorr   (501) staff       (20)       23 2023-04-17 05:07:52.000000 manifest-ml-0.1.7/manifest/connections/__init__.py
--rw-r--r--   0 laurelorr   (501) staff       (20)     6196 2023-05-04 04:43:35.000000 manifest-ml-0.1.7/manifest/connections/client_pool.py
--rw-r--r--   0 laurelorr   (501) staff       (20)     1227 2023-05-03 06:44:32.000000 manifest-ml-0.1.7/manifest/connections/scheduler.py
--rw-r--r--   0 laurelorr   (501) staff       (20)    25003 2023-05-17 22:43:15.000000 manifest-ml-0.1.7/manifest/manifest.py
--rw-r--r--   0 laurelorr   (501) staff       (20)     3135 2023-05-04 04:43:35.000000 manifest-ml-0.1.7/manifest/request.py
--rw-r--r--   0 laurelorr   (501) staff       (20)    10950 2023-05-04 04:43:35.000000 manifest-ml-0.1.7/manifest/response.py
--rw-r--r--   0 laurelorr   (501) staff       (20)       22 2023-05-17 23:44:27.000000 manifest-ml-0.1.7/manifest/version.py
-drwxr-xr-x   0 laurelorr   (501) staff       (20)        0 2023-05-17 23:44:42.193973 manifest-ml-0.1.7/manifest_ml.egg-info/
--rw-r--r--   0 laurelorr   (501) staff       (20)    10728 2023-05-17 23:44:41.000000 manifest-ml-0.1.7/manifest_ml.egg-info/PKG-INFO
--rw-r--r--   0 laurelorr   (501) staff       (20)     1568 2023-05-17 23:44:42.000000 manifest-ml-0.1.7/manifest_ml.egg-info/SOURCES.txt
--rw-r--r--   0 laurelorr   (501) staff       (20)        1 2023-05-17 23:44:41.000000 manifest-ml-0.1.7/manifest_ml.egg-info/dependency_links.txt
--rw-r--r--   0 laurelorr   (501) staff       (20)     1653 2023-05-17 23:44:42.000000 manifest-ml-0.1.7/manifest_ml.egg-info/requires.txt
--rw-r--r--   0 laurelorr   (501) staff       (20)       17 2023-05-17 23:44:42.000000 manifest-ml-0.1.7/manifest_ml.egg-info/top_level.txt
--rw-r--r--   0 laurelorr   (501) staff       (20)      802 2023-05-17 05:53:01.000000 manifest-ml-0.1.7/pyproject.toml
--rw-r--r--   0 laurelorr   (501) staff       (20)       38 2023-05-17 23:44:42.198020 manifest-ml-0.1.7/setup.cfg
--rw-r--r--   0 laurelorr   (501) staff       (20)     5379 2023-05-17 05:53:01.000000 manifest-ml-0.1.7/setup.py
-drwxr-xr-x   0 laurelorr   (501) staff       (20)        0 2023-05-17 23:44:42.196494 manifest-ml-0.1.7/tests/
--rw-r--r--   0 laurelorr   (501) staff       (20)     2275 2023-02-14 19:01:23.000000 manifest-ml-0.1.7/tests/test_array_cache.py
--rw-r--r--   0 laurelorr   (501) staff       (20)     8152 2023-04-24 18:36:42.000000 manifest-ml-0.1.7/tests/test_cache.py
--rw-r--r--   0 laurelorr   (501) staff       (20)     2446 2023-04-24 18:36:42.000000 manifest-ml-0.1.7/tests/test_client.py
--rw-r--r--   0 laurelorr   (501) staff       (20)     2304 2023-05-04 04:43:35.000000 manifest-ml-0.1.7/tests/test_client_pool.py
--rw-r--r--   0 laurelorr   (501) staff       (20)     9132 2023-04-09 06:56:02.000000 manifest-ml-0.1.7/tests/test_huggingface_api.py
--rw-r--r--   0 laurelorr   (501) staff       (20)    38828 2023-05-17 23:08:48.000000 manifest-ml-0.1.7/tests/test_manifest.py
--rw-r--r--   0 laurelorr   (501) staff       (20)     1949 2023-03-12 04:05:54.000000 manifest-ml-0.1.7/tests/test_request.py
--rw-r--r--   0 laurelorr   (501) staff       (20)    10431 2023-04-24 18:36:42.000000 manifest-ml-0.1.7/tests/test_response.py
--rw-r--r--   0 laurelorr   (501) staff       (20)      769 2023-05-03 06:44:15.000000 manifest-ml-0.1.7/tests/test_scheduler.py
--rw-r--r--   0 laurelorr   (501) staff       (20)     1073 2023-04-24 18:36:42.000000 manifest-ml-0.1.7/tests/test_serializer.py
-drwxr-xr-x   0 laurelorr   (501) staff       (20)        0 2023-05-17 23:44:42.196929 manifest-ml-0.1.7/web_app/
--rw-r--r--   0 laurelorr   (501) staff       (20)       36 2023-02-14 19:01:23.000000 manifest-ml-0.1.7/web_app/__init__.py
--rw-r--r--   0 laurelorr   (501) staff       (20)     1737 2023-04-24 18:36:42.000000 manifest-ml-0.1.7/web_app/main.py
--rw-r--r--   0 laurelorr   (501) staff       (20)      721 2023-02-14 19:01:23.000000 manifest-ml-0.1.7/web_app/schemas.py
+drwxr-xr-x   0 laurelorr   (501) staff       (20)        0 2023-05-22 17:54:12.911432 manifest-ml-0.1.8/
+-rw-r--r--   0 laurelorr   (501) staff       (20)    11357 2023-02-14 19:01:23.000000 manifest-ml-0.1.8/LICENSE
+-rw-r--r--   0 laurelorr   (501) staff       (20)    11360 2023-05-22 17:54:12.911229 manifest-ml-0.1.8/PKG-INFO
+-rw-r--r--   0 laurelorr   (501) staff       (20)    10692 2023-05-21 22:56:03.000000 manifest-ml-0.1.8/README.md
+drwxr-xr-x   0 laurelorr   (501) staff       (20)        0 2023-05-22 17:54:12.898039 manifest-ml-0.1.8/manifest/
+-rw-r--r--   0 laurelorr   (501) staff       (20)      183 2023-03-12 04:05:54.000000 manifest-ml-0.1.8/manifest/__init__.py
+drwxr-xr-x   0 laurelorr   (501) staff       (20)        0 2023-05-22 17:54:12.899138 manifest-ml-0.1.8/manifest/api/
+-rw-r--r--   0 laurelorr   (501) staff       (20)       16 2023-02-14 19:01:23.000000 manifest-ml-0.1.8/manifest/api/__init__.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)     8947 2023-04-16 20:56:11.000000 manifest-ml-0.1.8/manifest/api/app.py
+drwxr-xr-x   0 laurelorr   (501) staff       (20)        0 2023-05-22 17:54:12.901270 manifest-ml-0.1.8/manifest/api/models/
+-rw-r--r--   0 laurelorr   (501) staff       (20)       19 2023-02-14 19:01:23.000000 manifest-ml-0.1.8/manifest/api/models/__init__.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)     4383 2023-04-09 06:56:02.000000 manifest-ml-0.1.8/manifest/api/models/diffuser.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)    23667 2023-05-17 05:53:01.000000 manifest-ml-0.1.8/manifest/api/models/huggingface.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)     2798 2023-04-09 06:56:02.000000 manifest-ml-0.1.8/manifest/api/models/model.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)     3880 2023-04-09 06:56:02.000000 manifest-ml-0.1.8/manifest/api/models/sentence_transformer.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)     1767 2023-04-17 05:07:52.000000 manifest-ml-0.1.8/manifest/api/response.py
+drwxr-xr-x   0 laurelorr   (501) staff       (20)        0 2023-05-22 17:54:12.903461 manifest-ml-0.1.8/manifest/caches/
+-rw-r--r--   0 laurelorr   (501) staff       (20)       18 2023-02-14 19:01:23.000000 manifest-ml-0.1.8/manifest/caches/__init__.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)     3725 2023-02-14 19:01:23.000000 manifest-ml-0.1.8/manifest/caches/array_cache.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)     4386 2023-04-24 18:36:42.000000 manifest-ml-0.1.8/manifest/caches/cache.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)     1131 2023-02-14 19:01:23.000000 manifest-ml-0.1.8/manifest/caches/noop.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)     3944 2023-03-12 04:05:54.000000 manifest-ml-0.1.8/manifest/caches/postgres.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)     1716 2023-02-14 19:01:23.000000 manifest-ml-0.1.8/manifest/caches/redis.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)     5997 2023-04-24 18:36:42.000000 manifest-ml-0.1.8/manifest/caches/serializers.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)     1772 2023-02-14 19:01:23.000000 manifest-ml-0.1.8/manifest/caches/sqlite.py
+drwxr-xr-x   0 laurelorr   (501) staff       (20)        0 2023-05-22 17:54:12.906627 manifest-ml-0.1.8/manifest/clients/
+-rw-r--r--   0 laurelorr   (501) staff       (20)       19 2023-02-14 19:01:23.000000 manifest-ml-0.1.8/manifest/clients/__init__.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)     3502 2023-05-21 22:50:13.000000 manifest-ml-0.1.8/manifest/clients/ai21.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)     3813 2023-05-22 17:53:58.000000 manifest-ml-0.1.8/manifest/clients/azureopenai.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)     3923 2023-05-22 17:53:58.000000 manifest-ml-0.1.8/manifest/clients/azureopenai_chat.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)    23102 2023-05-21 22:50:13.000000 manifest-ml-0.1.8/manifest/clients/client.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)     3660 2023-05-21 22:50:13.000000 manifest-ml-0.1.8/manifest/clients/cohere.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)     3014 2023-05-22 17:53:58.000000 manifest-ml-0.1.8/manifest/clients/diffuser.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)     5948 2023-05-21 22:50:13.000000 manifest-ml-0.1.8/manifest/clients/dummy.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)     5997 2023-05-22 17:53:58.000000 manifest-ml-0.1.8/manifest/clients/google.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)     5346 2023-05-22 17:53:58.000000 manifest-ml-0.1.8/manifest/clients/google_chat.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)     3946 2023-05-21 22:50:13.000000 manifest-ml-0.1.8/manifest/clients/huggingface.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)     2533 2023-05-21 22:50:13.000000 manifest-ml-0.1.8/manifest/clients/huggingface_embedding.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)     5011 2023-05-21 22:50:13.000000 manifest-ml-0.1.8/manifest/clients/openai.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)     4747 2023-05-21 22:50:13.000000 manifest-ml-0.1.8/manifest/clients/openai_chat.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)     6659 2023-05-21 22:50:13.000000 manifest-ml-0.1.8/manifest/clients/openai_embedding.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)     5361 2023-05-21 22:50:13.000000 manifest-ml-0.1.8/manifest/clients/toma.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)     1943 2023-05-21 06:36:52.000000 manifest-ml-0.1.8/manifest/clients/toma_diffuser.py
+drwxr-xr-x   0 laurelorr   (501) staff       (20)        0 2023-05-22 17:54:12.907417 manifest-ml-0.1.8/manifest/connections/
+-rw-r--r--   0 laurelorr   (501) staff       (20)       23 2023-04-17 05:07:52.000000 manifest-ml-0.1.8/manifest/connections/__init__.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)     6578 2023-05-21 06:39:08.000000 manifest-ml-0.1.8/manifest/connections/client_pool.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)     1227 2023-05-03 06:44:32.000000 manifest-ml-0.1.8/manifest/connections/scheduler.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)    28873 2023-05-21 22:55:58.000000 manifest-ml-0.1.8/manifest/manifest.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)     3135 2023-05-04 04:43:35.000000 manifest-ml-0.1.8/manifest/request.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)    15578 2023-05-21 22:50:13.000000 manifest-ml-0.1.8/manifest/response.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)       22 2023-05-22 17:19:02.000000 manifest-ml-0.1.8/manifest/version.py
+drwxr-xr-x   0 laurelorr   (501) staff       (20)        0 2023-05-22 17:54:12.908203 manifest-ml-0.1.8/manifest_ml.egg-info/
+-rw-r--r--   0 laurelorr   (501) staff       (20)    11360 2023-05-22 17:54:12.000000 manifest-ml-0.1.8/manifest_ml.egg-info/PKG-INFO
+-rw-r--r--   0 laurelorr   (501) staff       (20)     1696 2023-05-22 17:54:12.000000 manifest-ml-0.1.8/manifest_ml.egg-info/SOURCES.txt
+-rw-r--r--   0 laurelorr   (501) staff       (20)        1 2023-05-22 17:54:12.000000 manifest-ml-0.1.8/manifest_ml.egg-info/dependency_links.txt
+-rw-r--r--   0 laurelorr   (501) staff       (20)     1653 2023-05-22 17:54:12.000000 manifest-ml-0.1.8/manifest_ml.egg-info/requires.txt
+-rw-r--r--   0 laurelorr   (501) staff       (20)       17 2023-05-22 17:54:12.000000 manifest-ml-0.1.8/manifest_ml.egg-info/top_level.txt
+-rw-r--r--   0 laurelorr   (501) staff       (20)      830 2023-05-21 06:36:52.000000 manifest-ml-0.1.8/pyproject.toml
+-rw-r--r--   0 laurelorr   (501) staff       (20)       38 2023-05-22 17:54:12.911512 manifest-ml-0.1.8/setup.cfg
+-rw-r--r--   0 laurelorr   (501) staff       (20)     5379 2023-05-17 05:53:01.000000 manifest-ml-0.1.8/setup.py
+drwxr-xr-x   0 laurelorr   (501) staff       (20)        0 2023-05-22 17:54:12.910534 manifest-ml-0.1.8/tests/
+-rw-r--r--   0 laurelorr   (501) staff       (20)     2275 2023-02-14 19:01:23.000000 manifest-ml-0.1.8/tests/test_array_cache.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)     8152 2023-04-24 18:36:42.000000 manifest-ml-0.1.8/tests/test_cache.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)     2446 2023-04-24 18:36:42.000000 manifest-ml-0.1.8/tests/test_client.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)     2304 2023-05-04 04:43:35.000000 manifest-ml-0.1.8/tests/test_client_pool.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)     9132 2023-04-09 06:56:02.000000 manifest-ml-0.1.8/tests/test_huggingface_api.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)    41658 2023-05-21 22:50:13.000000 manifest-ml-0.1.8/tests/test_manifest.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)     1949 2023-03-12 04:05:54.000000 manifest-ml-0.1.8/tests/test_request.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)    13095 2023-05-21 22:50:13.000000 manifest-ml-0.1.8/tests/test_response.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)      769 2023-05-03 06:44:15.000000 manifest-ml-0.1.8/tests/test_scheduler.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)     1073 2023-04-24 18:36:42.000000 manifest-ml-0.1.8/tests/test_serializer.py
+drwxr-xr-x   0 laurelorr   (501) staff       (20)        0 2023-05-22 17:54:12.910990 manifest-ml-0.1.8/web_app/
+-rw-r--r--   0 laurelorr   (501) staff       (20)       36 2023-02-14 19:01:23.000000 manifest-ml-0.1.8/web_app/__init__.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)     1737 2023-04-24 18:36:42.000000 manifest-ml-0.1.8/web_app/main.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)      721 2023-02-14 19:01:23.000000 manifest-ml-0.1.8/web_app/schemas.py
```

### Comparing `manifest-ml-0.1.7/LICENSE` & `manifest-ml-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `manifest-ml-0.1.7/PKG-INFO` & `manifest-ml-0.1.8/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: manifest-ml
-Version: 0.1.7
+Version: 0.1.8
 Summary: Manifest for Prompting Foundation Models.
 Home-page: https://github.com/HazyResearch/manifest
 Author: Laurel Orr
 Author-email: laurel.orr@numbersstation.ai
 License: Apache 2.0
-Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
 Provides-Extra: api
@@ -26,17 +25,18 @@
 How to make prompt programming with Foundation Models a little easier.
 
 
 # Table of Contents
 - [Install](#install)
 - [Getting Started](#getting-started)
 - [Manifest](#manifest-components)
-- [Local HuggingFace Models](#local-huggingface-models)
-- [Chat Models](#chat-models)
-- [Embedding Models](#embedding-models)
+- [Other Models Types](#other-models)
+    - [Local HuggingFace Models](#local-huggingface-models)
+    - [Chat Models](#chat-models)
+    - [Embedding Models](#embedding-models)
 - [Road Map](#road-map)
 - [Development](#development)
 - [Cite](#cite)
 
 
 # Install
 Install:
@@ -63,15 +63,15 @@
 
 # Getting Started
 Running is simple to get started. If using OpenAI, set `export OPENAI_API_KEY=<OPENAIKEY>` (or pass key in through variable `client_connection`) then run
 
 ```python
 from manifest import Manifest
 
-# Start a manifest session to OpenAI - default `engine=text-davinci-002`
+# Start a manifest session to OpenAI - default `engine=text-davinci-003`
 manifest = Manifest(
     client_name = "openai",
 )
 manifest.run("Why is the grass green?")
 ```
 
 ## Examples
@@ -162,14 +162,24 @@
 ```
 
 If you want to change default parameters to a model, we pass those as `kwargs` to the client.
 ```python
 result = manifest.run(prompt, "Laurel", max_tokens=50)
 ```
 
+## Streaming Queries
+Manifest also supports streaming the model response back, assuming it's supported by the underlying client. When calling `run`, pass `stream=True` to get a streaming iterator in response.
+
+```python
+result_iterator = manifest.run("Tell me a story. Once upon a time", max_tokens=100, stream=True)
+for res_text in result_iterator:
+    print(res_text)
+```
+Streaming responses are only supported for single string queries (not batch mode) for text completion models.
+
 ## Model Pools
 Manifest supports querying multiple models with different schedulers. This is very much a work in progress effort, but Manifest will round robin select (or randomly select) the clients you want. You can use the same client multiple times with different connection strings (e.g. different API keys), or you can mix and match. The only requirement is that all clients are the same request type. I.e. you can't have a pool of generation models and embedding models.
 
 To query between a local model and OpenAI,
 ```python
 from manifest.connections.client_pool import ClientConnection
 from manifest import Manifest
@@ -189,15 +199,17 @@
 
 The speed benefit comes in with async batched runs. When calling `arun_batch` with a list of prompts, Manifest supports a `chunk_size` param. This will break the prompts into `chunk_size` chunks to spread across the client pool. By default `chunk_size` is `-1` which means only one client will get all the prompts to run asynchronously. You must set `chunk_size > 1` to distribute across the pool. There is a further `batch_size` param which control the individual client `batch_size` to send to the model.
 
 ```python
 responses = asyncio.run(manifest.arun_batch(prompts, max_tokens=30, chunk_size=20))
 ```
 
-# Local Huggingface Models
+# Other Models
+
+## Local Huggingface Models
 To use a HuggingFace generative model, in `manifest/api` we have a Flask application that hosts the models for you.
 
 In a separate terminal or Tmux/Screen session, to load 6B parameters models, run
 ```bash
 python3 -m manifest.api.app \
     --model_type huggingface \
     --model_name_or_path EleutherAI/gpt-j-6B \
@@ -237,27 +249,27 @@
 python3 -m manifest.api.app \
     --model_type huggingface \
     --model_name_or_path bigscience/bloom \
     --use_bitsandbytes \
     --percent_max_gpu_mem_reduction 0.85
 ```
 
-# Chat Models
+## Chat Models
 Manifest has specific support for executing against chat models in the more standard "system" / "user" dialogue. To pass in a dialogue history to Manifest, use the `run` command with a list of dictionary inputs with `role` and `content` keys using an associated chat model such as `openaichat`.
 
 ```python
 manifest = Manifest(client_name="openaichat")
 dialogue = [
     {"role": "system", "content": "You are a helpful assistant who also responds in rhymes"},
     {"role": "user", "content": "What is the date?"},
 ]
 res = manifest.run(dialogue, max_tokens=100)
 ```
 
-# Embedding Models
+## Embedding Models
 Manifest also supports getting embeddings from models and available APIs. We do this all through changing the `client_name` argument. You still use `run` and `abatch_run`.
 
 To use OpenAI's embedding models, simply run
 ```python
 manifest = Manifest(client_name="openaiembedding")
 embedding_as_np = manifest.run("Get me an embedding for a bunny")
 ```
@@ -270,19 +282,22 @@
     --device 0
 ```
 
 # Road Map
 Here's what's coming up next
 - [ ] Clients
   - [ ] HuggingFace Hub
-  - [ ] Azure OpenAI
+  - [x] Azure OpenAI
+  - [x] Google Vertex
   - [ ] Anthropic
+  - [x] Streaming Support Completions
+  - [ ] Streaming Support Chat Models
 - [ ] Data Types
   - [ ] Diffusion Models
-- [ ] Orchestration
+- [x] Orchestration
   - [x] Connection pools
 - [ ] Local Inference
   - [ ] FlexGen
 
 # Development
 Before submitting a PR, run
 ```bash
@@ -299,9 +314,7 @@
   author = {Orr, Laurel},
   title = {Manifest},
   year = {2022},
   publisher = {GitHub},
   howpublished = {\url{https://github.com/HazyResearch/manifest}},
 }
 ```
-
-
```

### Comparing `manifest-ml-0.1.7/README.md` & `manifest-ml-0.1.8/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -2,17 +2,18 @@
 How to make prompt programming with Foundation Models a little easier.
 
 
 # Table of Contents
 - [Install](#install)
 - [Getting Started](#getting-started)
 - [Manifest](#manifest-components)
-- [Local HuggingFace Models](#local-huggingface-models)
-- [Chat Models](#chat-models)
-- [Embedding Models](#embedding-models)
+- [Other Models Types](#other-models)
+    - [Local HuggingFace Models](#local-huggingface-models)
+    - [Chat Models](#chat-models)
+    - [Embedding Models](#embedding-models)
 - [Road Map](#road-map)
 - [Development](#development)
 - [Cite](#cite)
 
 
 # Install
 Install:
@@ -39,15 +40,15 @@
 
 # Getting Started
 Running is simple to get started. If using OpenAI, set `export OPENAI_API_KEY=<OPENAIKEY>` (or pass key in through variable `client_connection`) then run
 
 ```python
 from manifest import Manifest
 
-# Start a manifest session to OpenAI - default `engine=text-davinci-002`
+# Start a manifest session to OpenAI - default `engine=text-davinci-003`
 manifest = Manifest(
     client_name = "openai",
 )
 manifest.run("Why is the grass green?")
 ```
 
 ## Examples
@@ -138,14 +139,24 @@
 ```
 
 If you want to change default parameters to a model, we pass those as `kwargs` to the client.
 ```python
 result = manifest.run(prompt, "Laurel", max_tokens=50)
 ```
 
+## Streaming Queries
+Manifest also supports streaming the model response back, assuming it's supported by the underlying client. When calling `run`, pass `stream=True` to get a streaming iterator in response.
+
+```python
+result_iterator = manifest.run("Tell me a story. Once upon a time", max_tokens=100, stream=True)
+for res_text in result_iterator:
+    print(res_text)
+```
+Streaming responses are only supported for single string queries (not batch mode) for text completion models.
+
 ## Model Pools
 Manifest supports querying multiple models with different schedulers. This is very much a work in progress effort, but Manifest will round robin select (or randomly select) the clients you want. You can use the same client multiple times with different connection strings (e.g. different API keys), or you can mix and match. The only requirement is that all clients are the same request type. I.e. you can't have a pool of generation models and embedding models.
 
 To query between a local model and OpenAI,
 ```python
 from manifest.connections.client_pool import ClientConnection
 from manifest import Manifest
@@ -165,15 +176,17 @@
 
 The speed benefit comes in with async batched runs. When calling `arun_batch` with a list of prompts, Manifest supports a `chunk_size` param. This will break the prompts into `chunk_size` chunks to spread across the client pool. By default `chunk_size` is `-1` which means only one client will get all the prompts to run asynchronously. You must set `chunk_size > 1` to distribute across the pool. There is a further `batch_size` param which control the individual client `batch_size` to send to the model.
 
 ```python
 responses = asyncio.run(manifest.arun_batch(prompts, max_tokens=30, chunk_size=20))
 ```
 
-# Local Huggingface Models
+# Other Models
+
+## Local Huggingface Models
 To use a HuggingFace generative model, in `manifest/api` we have a Flask application that hosts the models for you.
 
 In a separate terminal or Tmux/Screen session, to load 6B parameters models, run
 ```bash
 python3 -m manifest.api.app \
     --model_type huggingface \
     --model_name_or_path EleutherAI/gpt-j-6B \
@@ -213,27 +226,27 @@
 python3 -m manifest.api.app \
     --model_type huggingface \
     --model_name_or_path bigscience/bloom \
     --use_bitsandbytes \
     --percent_max_gpu_mem_reduction 0.85
 ```
 
-# Chat Models
+## Chat Models
 Manifest has specific support for executing against chat models in the more standard "system" / "user" dialogue. To pass in a dialogue history to Manifest, use the `run` command with a list of dictionary inputs with `role` and `content` keys using an associated chat model such as `openaichat`.
 
 ```python
 manifest = Manifest(client_name="openaichat")
 dialogue = [
     {"role": "system", "content": "You are a helpful assistant who also responds in rhymes"},
     {"role": "user", "content": "What is the date?"},
 ]
 res = manifest.run(dialogue, max_tokens=100)
 ```
 
-# Embedding Models
+## Embedding Models
 Manifest also supports getting embeddings from models and available APIs. We do this all through changing the `client_name` argument. You still use `run` and `abatch_run`.
 
 To use OpenAI's embedding models, simply run
 ```python
 manifest = Manifest(client_name="openaiembedding")
 embedding_as_np = manifest.run("Get me an embedding for a bunny")
 ```
@@ -246,19 +259,22 @@
     --device 0
 ```
 
 # Road Map
 Here's what's coming up next
 - [ ] Clients
   - [ ] HuggingFace Hub
-  - [ ] Azure OpenAI
+  - [x] Azure OpenAI
+  - [x] Google Vertex
   - [ ] Anthropic
+  - [x] Streaming Support Completions
+  - [ ] Streaming Support Chat Models
 - [ ] Data Types
   - [ ] Diffusion Models
-- [ ] Orchestration
+- [x] Orchestration
   - [x] Connection pools
 - [ ] Local Inference
   - [ ] FlexGen
 
 # Development
 Before submitting a PR, run
 ```bash
```

### Comparing `manifest-ml-0.1.7/manifest/api/app.py` & `manifest-ml-0.1.8/manifest/api/app.py`

 * *Files identical despite different names*

### Comparing `manifest-ml-0.1.7/manifest/api/models/diffuser.py` & `manifest-ml-0.1.8/manifest/api/models/diffuser.py`

 * *Files identical despite different names*

### Comparing `manifest-ml-0.1.7/manifest/api/models/huggingface.py` & `manifest-ml-0.1.8/manifest/api/models/huggingface.py`

 * *Files identical despite different names*

### Comparing `manifest-ml-0.1.7/manifest/api/models/model.py` & `manifest-ml-0.1.8/manifest/api/models/model.py`

 * *Files identical despite different names*

### Comparing `manifest-ml-0.1.7/manifest/api/models/sentence_transformer.py` & `manifest-ml-0.1.8/manifest/api/models/sentence_transformer.py`

 * *Files identical despite different names*

### Comparing `manifest-ml-0.1.7/manifest/api/response.py` & `manifest-ml-0.1.8/manifest/api/response.py`

 * *Files identical despite different names*

### Comparing `manifest-ml-0.1.7/manifest/caches/array_cache.py` & `manifest-ml-0.1.8/manifest/caches/array_cache.py`

 * *Files identical despite different names*

### Comparing `manifest-ml-0.1.7/manifest/caches/cache.py` & `manifest-ml-0.1.8/manifest/caches/cache.py`

 * *Files identical despite different names*

### Comparing `manifest-ml-0.1.7/manifest/caches/noop.py` & `manifest-ml-0.1.8/manifest/caches/noop.py`

 * *Files identical despite different names*

### Comparing `manifest-ml-0.1.7/manifest/caches/postgres.py` & `manifest-ml-0.1.8/manifest/caches/postgres.py`

 * *Files identical despite different names*

### Comparing `manifest-ml-0.1.7/manifest/caches/redis.py` & `manifest-ml-0.1.8/manifest/caches/redis.py`

 * *Files identical despite different names*

### Comparing `manifest-ml-0.1.7/manifest/caches/serializers.py` & `manifest-ml-0.1.8/manifest/caches/serializers.py`

 * *Files identical despite different names*

### Comparing `manifest-ml-0.1.7/manifest/caches/sqlite.py` & `manifest-ml-0.1.8/manifest/caches/sqlite.py`

 * *Files identical despite different names*

### Comparing `manifest-ml-0.1.7/manifest/clients/ai21.py` & `manifest-ml-0.1.8/manifest/clients/ai21.py`

 * *Files 4% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 
         Args:
             connection_str: connection string.
             client_args: client arguments.
         """
         # Taken from https://studio.ai21.com/docs/api/
         self.host = "https://api.ai21.com/studio/v1"
-        self.api_key = os.environ.get("AI21_API_KEY", connection_str)
+        self.api_key = connection_str or os.environ.get("AI21_API_KEY")
         if self.api_key is None:
             raise ValueError(
                 "AI21 API key not set. Set AI21_API_KEY environment "
                 "variable or pass through `client_connection`."
             )
 
         for key in self.PARAMS:
@@ -78,27 +78,34 @@
         """
         return {"Authorization": f"Bearer {self.api_key}"}
 
     def supports_batch_inference(self) -> bool:
         """Return whether the client supports batch inference."""
         return False
 
+    def supports_streaming_inference(self) -> bool:
+        """Return whether the client supports streaming inference.
+
+        Override in child client class.
+        """
+        return False
+
     def get_model_params(self) -> Dict:
         """
         Get model params.
 
         By getting model params from the server, we can add to request
         and make sure cache keys are unique to model.
 
         Returns:
             model params.
         """
         return {"model_name": self.NAME, "engine": getattr(self, "engine")}
 
-    def validate_response(self, response: Dict, request: Dict) -> Dict[str, Any]:
+    def postprocess_response(self, response: Dict, request: Dict) -> Dict[str, Any]:
         """
         Format response to dict.
 
         Args:
             response: response
             request: request
```

### Comparing `manifest-ml-0.1.7/manifest/clients/cohere.py` & `manifest-ml-0.1.8/manifest/clients/cohere.py`

 * *Files 10% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 
         connection_str is passed as default COHERE_API_KEY if variable not set.
 
         Args:
             connection_str: connection string.
             client_args: client arguments.
         """
-        self.api_key = os.environ.get("COHERE_API_KEY", connection_str)
+        self.api_key = connection_str or os.environ.get("COHERE_API_KEY")
         if self.api_key is None:
             raise ValueError(
                 "Cohere API key not set. Set COHERE_API_KEY environment "
                 "variable or pass through `client_connection`."
             )
         self.host = "https://api.cohere.ai"
         for key in self.PARAMS:
@@ -77,27 +77,34 @@
             "Authorization": f"Bearer {self.api_key}",
         }
 
     def supports_batch_inference(self) -> bool:
         """Return whether the client supports batch inference."""
         return False
 
+    def supports_streaming_inference(self) -> bool:
+        """Return whether the client supports streaming inference.
+
+        Override in child client class.
+        """
+        return False
+
     def get_model_params(self) -> Dict:
         """
         Get model params.
 
         By getting model params from the server, we can add to request
         and make sure cache keys are unique to model.
 
         Returns:
             model params.
         """
         return {"model_name": self.NAME, "engine": getattr(self, "engine")}
 
-    def validate_response(self, response: Dict, request: Dict) -> Dict[str, Any]:
+    def postprocess_response(self, response: Dict, request: Dict) -> Dict[str, Any]:
         """
         Format response to dict.
 
         Args:
             response: response
             request: request
```

### Comparing `manifest-ml-0.1.7/manifest/clients/diffuser.py` & `manifest-ml-0.1.8/manifest/clients/diffuser.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Hugging Face client."""
+"""Diffuser client."""
 import logging
 from typing import Any, Dict, Optional
 
 import numpy as np
 import requests
 
 from manifest.clients.client import Client
@@ -68,29 +68,36 @@
         """
         return {}
 
     def supports_batch_inference(self) -> bool:
         """Return whether the client supports batch inference."""
         return True
 
+    def supports_streaming_inference(self) -> bool:
+        """Return whether the client supports streaming inference.
+
+        Override in child client class.
+        """
+        return False
+
     def get_model_params(self) -> Dict:
         """
         Get model params.
 
         By getting model params from the server, we can add to request
         and make sure cache keys are unique to model.
 
         Returns:
             model params.
         """
         res = requests.post(self.host + "/params").json()
         res["client_name"] = self.NAME
         return res
 
-    def validate_response(self, response: Dict, request: Dict) -> Dict[str, Any]:
+    def postprocess_response(self, response: Dict, request: Dict) -> Dict[str, Any]:
         """
         Format response to dict.
 
         Args:
             response: response
             request: request
```

### Comparing `manifest-ml-0.1.7/manifest/clients/dummy.py` & `manifest-ml-0.1.8/manifest/clients/dummy.py`

 * *Files 9% similar despite different names*

```diff
@@ -44,14 +44,21 @@
         """Get generation URL."""
         return "dummy"
 
     def supports_batch_inference(self) -> bool:
         """Return whether the client supports batch inference."""
         return True
 
+    def supports_streaming_inference(self) -> bool:
+        """Return whether the client supports streaming inference.
+
+        Override in child client class.
+        """
+        return False
+
     def get_generation_header(self) -> Dict[str, str]:
         """
         Get generation header.
 
         Returns:
             header.
         """
@@ -107,15 +114,17 @@
                 * int(request_params["num_results"])
                 * num_results
             ),
             response_type="text",
             request_type=self.REQUEST_CLS,
         )
 
-    async def arun_batch_request(self, request: Request) -> Response:
+    async def arun_batch_request(
+        self, request: Request, verbose: bool = False
+    ) -> Response:
         """
         Get async request string function.
 
         Args:
             request: request.
 
         Returns:
```

### Comparing `manifest-ml-0.1.7/manifest/clients/huggingface.py` & `manifest-ml-0.1.8/manifest/clients/huggingface.py`

 * *Files 4% similar despite different names*

```diff
@@ -62,14 +62,21 @@
         """
         return {}
 
     def supports_batch_inference(self) -> bool:
         """Return whether the client supports batch inference."""
         return True
 
+    def supports_streaming_inference(self) -> bool:
+        """Return whether the client supports streaming inference.
+
+        Override in child client class.
+        """
+        return False
+
     def get_model_params(self) -> Dict:
         """
         Get model params.
 
         By getting model params from the server, we can add to request
         and make sure cache keys are unique to model.
 
@@ -90,15 +97,15 @@
         Args:
             request: request.
 
         Returns:
             request function that takes no input.
             request parameters as dict.
         """
-        request_params = self.get_request_params(request)
+        request_params = self._get_request_params(request)
         retry_timeout = request_params.pop("client_timeout")
         for key in DEFAULT_REQUEST_KEYS:
             request_params.pop(key, None)
         # Do not add params like we do with request as the model isn't sampling
         request_params = {"prompt": request.prompt}
 
         post_str = self.host + "/score_sequence"
```

### Comparing `manifest-ml-0.1.7/manifest/clients/huggingface_embedding.py` & `manifest-ml-0.1.8/manifest/clients/huggingface_embedding.py`

 * *Files 6% similar despite different names*

```diff
@@ -54,29 +54,36 @@
         """
         return {}
 
     def supports_batch_inference(self) -> bool:
         """Return whether the client supports batch inference."""
         return True
 
+    def supports_streaming_inference(self) -> bool:
+        """Return whether the client supports streaming inference.
+
+        Override in child client class.
+        """
+        return False
+
     def get_model_params(self) -> Dict:
         """
         Get model params.
 
         By getting model params from the server, we can add to request
         and make sure cache keys are unique to model.
 
         Returns:
             model params.
         """
         res = requests.post(self.host + "/params").json()
         res["client_name"] = self.NAME
         return res
 
-    def validate_response(self, response: Dict, request: Dict) -> Dict[str, Any]:
+    def postprocess_response(self, response: Dict, request: Dict) -> Dict[str, Any]:
         """
         Format response to dict.
 
         Args:
             response: response
             request: request
```

### Comparing `manifest-ml-0.1.7/manifest/clients/openai.py` & `manifest-ml-0.1.8/manifest/clients/openai.py`

 * *Files 6% similar despite different names*

```diff
@@ -56,15 +56,15 @@
 
         connection_str is passed as default OPENAI_API_KEY if variable not set.
 
         Args:
             connection_str: connection string.
             client_args: client arguments.
         """
-        self.api_key = os.environ.get("OPENAI_API_KEY", connection_str)
+        self.api_key = connection_str or os.environ.get("OPENAI_API_KEY")
         if self.api_key is None:
             raise ValueError(
                 "OpenAI API key not set. Set OPENAI_API_KEY environment "
                 "variable or pass through `client_connection`."
             )
         self.host = "https://api.openai.com/v1"
         for key in self.PARAMS:
@@ -91,38 +91,45 @@
         """
         return {"Authorization": f"Bearer {self.api_key}"}
 
     def supports_batch_inference(self) -> bool:
         """Return whether the client supports batch inference."""
         return True
 
+    def supports_streaming_inference(self) -> bool:
+        """Return whether the client supports streaming inference.
+
+        Override in child client class.
+        """
+        return True
+
     def get_model_params(self) -> Dict:
         """
         Get model params.
 
         By getting model params from the server, we can add to request
         and make sure cache keys are unique to model.
 
         Returns:
             model params.
         """
         return {"model_name": self.NAME, "engine": getattr(self, "engine")}
 
-    def validate_response(self, response: Dict, request: Dict) -> Dict[str, Any]:
+    def postprocess_response(self, response: Dict, request: Dict) -> Dict[str, Any]:
         """
         Validate response as dict.
 
         Args:
             response: response
             request: request
 
         Return:
             response as dict
         """
-        validated_response = super().validate_response(response, request)
+        validated_response = super().postprocess_response(response, request)
         # Handle logprobs
         for choice in validated_response["choices"]:
             if "logprobs" in choice:
                 logprobs = choice.pop("logprobs")
                 if logprobs and "token_logprobs" in logprobs:
                     choice["token_logprobs"] = logprobs["token_logprobs"]
                     choice["tokens"] = logprobs["tokens"]
```

### Comparing `manifest-ml-0.1.7/manifest/clients/openai_chat.py` & `manifest-ml-0.1.8/manifest/clients/google.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,171 +1,197 @@
-"""OpenAIChat client."""
-import copy
+"""Google client."""
 import logging
 import os
-from typing import Any, Dict, Optional
+import subprocess
+from typing import Any, Dict, Optional, Type
 
-from manifest.clients.openai import OpenAIClient
-from manifest.request import LMRequest
+from manifest.clients.client import Client
+from manifest.request import LMRequest, Request
 
 logger = logging.getLogger(__name__)
 
-# List from https://platform.openai.com/docs/models/model-endpoint-compatibility
-OPENAICHAT_ENGINES = {"gpt-3.5-turbo", "gpt-4", "gpt-4-32k"}
+# https://cloud.google.com/vertex-ai/docs/generative-ai/start/quickstarts/api-quickstart
+GOOGLE_ENGINES = {
+    "text-bison",
+}
+
+
+def get_project_id() -> Optional[str]:
+    """Get project ID.
+
+    Run
+    `gcloud config get-value project`
+    """
+    try:
+        project_id = subprocess.run(
+            ["gcloud", "config", "get-value", "project"],
+            stdout=subprocess.PIPE,
+            stderr=subprocess.PIPE,
+        )
+        if project_id.stderr.decode("utf-8").strip():
+            return None
+        return project_id.stdout.decode("utf-8").strip()
+    except Exception:
+        return None
 
 
-class OpenAIChatClient(OpenAIClient):
-    """OpenAI Chat client."""
+class GoogleClient(Client):
+    """Google client."""
 
     # User param -> (client param, default value)
     PARAMS = {
-        "engine": ("model", "gpt-3.5-turbo"),
+        "engine": ("model", "text-bison"),
         "temperature": ("temperature", 1.0),
-        "max_tokens": ("max_tokens", 10),
-        "n": ("n", 1),
-        "top_p": ("top_p", 1.0),
-        "stop_sequences": ("stop", None),  # OpenAI doesn't like empty lists
-        "presence_penalty": ("presence_penalty", 0.0),
-        "frequency_penalty": ("frequency_penalty", 0.0),
+        "max_tokens": ("maxOutputTokens", 10),
+        "top_p": ("topP", 1.0),
+        "top_k": ("topK", 1),
+        "batch_size": ("batch_size", 20),
     }
-    REQUEST_CLS = LMRequest
-    NAME = "openaichat"
-    IS_CHAT = True
+    REQUEST_CLS: Type[Request] = LMRequest
+    NAME = "google"
 
     def connect(
         self,
         connection_str: Optional[str] = None,
         client_args: Dict[str, Any] = {},
     ) -> None:
         """
-        Connect to the OpenAI server.
+        Connect to the GoogleVertex API.
 
-        connection_str is passed as default OPENAI_API_KEY if variable not set.
+        connection_str is passed as default GOOGLE_API_KEY if variable not set.
 
         Args:
             connection_str: connection string.
             client_args: client arguments.
         """
-        self.api_key = os.environ.get("OPENAI_API_KEY", connection_str)
+        connection_parts = connection_str.split("::")
+        if len(connection_parts) == 1:
+            self.api_key = connection_parts[0]
+            self.project_id = None
+        elif len(connection_parts) == 2:
+            self.api_key, self.project_id = connection_parts
+        else:
+            raise ValueError(
+                "Invalid connection string. "
+                "Must be either API_KEY or API_KEY::PROJECT_ID"
+            )
+        self.api_key = self.api_key or os.environ.get("GOOGLE_API_KEY")
         if self.api_key is None:
             raise ValueError(
-                "OpenAI API key not set. Set OPENAI_API_KEY environment "
-                "variable or pass through `client_connection`."
+                "GoogleVertex API key not set. Set GOOGLE_API_KEY environment "
+                "variable or pass through `client_connection`. This can be "
+                "found by running `gcloud auth print-access-token`"
             )
-        self.host = "https://api.openai.com/v1"
+        self.project_id = (
+            self.project_id or os.environ.get("GOOGLE_PROJECT_ID") or get_project_id()
+        )
+        if self.project_id is None:
+            raise ValueError("GoogleVertex project ID not set. Set GOOGLE_PROJECT_ID")
+        self.host = f"https://us-central1-aiplatform.googleapis.com/v1/projects/{self.project_id}/locations/us-central1/publishers/google/models"  # noqa: E501
+
         for key in self.PARAMS:
             setattr(self, key, client_args.pop(key, self.PARAMS[key][1]))
-        if getattr(self, "engine") not in OPENAICHAT_ENGINES:
+        if getattr(self, "engine") not in GOOGLE_ENGINES:
             raise ValueError(
-                f"Invalid engine {getattr(self, 'engine')}. "
-                f"Must be {OPENAICHAT_ENGINES}."
+                f"Invalid engine {getattr(self, 'engine')}. Must be {GOOGLE_ENGINES}."
             )
 
+    def close(self) -> None:
+        """Close the client."""
+        pass
+
     def get_generation_url(self) -> str:
         """Get generation URL."""
-        return self.host + "/chat/completions"
+        model = getattr(self, "engine")
+        return self.host + f"/{model}:predict"
+
+    def get_generation_header(self) -> Dict[str, str]:
+        """
+        Get generation header.
+
+        Returns:
+            header.
+        """
+        return {"Authorization": f"Bearer {self.api_key}"}
 
     def supports_batch_inference(self) -> bool:
         """Return whether the client supports batch inference."""
+        return True
+
+    def supports_streaming_inference(self) -> bool:
+        """Return whether the client supports streaming inference.
+
+        Override in child client class.
+        """
         return False
 
     def get_model_params(self) -> Dict:
         """
         Get model params.
 
         By getting model params from the server, we can add to request
         and make sure cache keys are unique to model.
 
         Returns:
             model params.
         """
         return {"model_name": self.NAME, "engine": getattr(self, "engine")}
 
-    def _format_request_for_chat(self, request_params: Dict[str, Any]) -> Dict:
-        """Format request params for chat.
+    def preprocess_request_params(self, request: Dict[str, Any]) -> Dict[str, Any]:
+        """
+        Preprocess request params.
 
         Args:
-            request_params: request params.
+            request: request params.
 
         Returns:
-            formatted request params.
+            request params.
         """
-        # Format for chat model
-        request_params = copy.deepcopy(request_params)
-        prompt = request_params.pop("prompt")
+        # Refortmat the request params for google
+        prompt = request.pop("prompt")
         if isinstance(prompt, str):
-            messages = [{"role": "user", "content": prompt}]
-        elif isinstance(prompt, list) and isinstance(prompt[0], str):
-            prompt_list = prompt
-            messages = [{"role": "user", "content": prompt} for prompt in prompt_list]
-        elif isinstance(prompt, list) and isinstance(prompt[0], dict):
-            for pmt_dict in prompt:
-                if "role" not in pmt_dict or "content" not in pmt_dict:
-                    raise ValueError(
-                        "Prompt must be list of dicts with 'role' and 'content' "
-                        f"keys. Got {prompt}."
-                    )
-            messages = prompt
+            prompt_list = [prompt]
         else:
-            raise ValueError(
-                "Prompt must be string, list of strings, or list of dicts."
-                f"Got {prompt}"
-            )
-        request_params["messages"] = messages
-        return request_params
-
-    def _format_request_from_chat(self, response_dict: Dict[str, Any]) -> Dict:
-        """Format response for standard response from chat.
+            prompt_list = prompt
+        google_request = {
+            "instances": [{"prompt": prompt} for prompt in prompt_list],
+            "parameters": request,
+        }
+        return super().preprocess_request_params(google_request)
+
+    def postprocess_response(
+        self, response: Dict[str, Any], request: Dict[str, Any]
+    ) -> Dict[str, Any]:
+        """
+        Validate response as dict.
+
+        Assumes response is dict
+        {
+            "predictions": [
+                {
+                    "safetyAttributes": {
+                        "categories": ["Violent", "Sexual"],
+                        "blocked": false,
+                        "scores": [0.1, 0.1]
+                    },
+                    "content": "SELECT * FROM "WWW";"
+                }
+            ]
+        }
 
         Args:
-            response_dict: response.
+            response: response
+            request: request
 
         Return:
-            formatted response.
-        """
-        new_choices = []
-        response_dict = copy.deepcopy(response_dict)
-        for message in response_dict["choices"]:
-            new_choices.append({"text": message["message"]["content"]})
-        response_dict["choices"] = new_choices
-        return response_dict
-
-    def _run_completion(
-        self, request_params: Dict[str, Any], retry_timeout: int
-    ) -> Dict:
-        """Execute completion request.
-
-        Args:
-            request_params: request params.
-            retry_timeout: retry timeout.
-
-        Returns:
-            response as dict.
-        """
-        # Format for chat model
-        request_params = self._format_request_for_chat(request_params)
-        response_dict = super()._run_completion(request_params, retry_timeout)
-        # Reformat for text model
-        response_dict = self._format_request_from_chat(response_dict)
-        return response_dict
-
-    async def _arun_completion(
-        self, request_params: Dict[str, Any], retry_timeout: int, batch_size: int
-    ) -> Dict:
-        """Async execute completion request.
-
-        Args:
-            request_params: request params.
-            retry_timeout: retry timeout.
-            batch_size: batch size for requests.
-
-        Returns:
-            response as dict.
+            response as dict
         """
-        # Format for chat model
-        request_params = self._format_request_for_chat(request_params)
-        response_dict = await super()._arun_completion(
-            request_params, retry_timeout, batch_size
-        )
-        # Reformat for text model
-        response_dict = self._format_request_from_chat(response_dict)
-        return response_dict
+        google_predictions = response.pop("predictions")
+        new_response = {
+            "choices": [
+                {
+                    "text": prediction["content"],
+                }
+                for prediction in google_predictions
+            ]
+        }
+        return super().postprocess_response(new_response, request)
```

### Comparing `manifest-ml-0.1.7/manifest/clients/openai_embedding.py` & `manifest-ml-0.1.8/manifest/clients/openai_embedding.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 
         connection_str is passed as default OPENAI_API_KEY if variable not set.
 
         Args:
             connection_str: connection string.
             client_args: client arguments.
         """
-        self.api_key = os.environ.get("OPENAI_API_KEY", connection_str)
+        self.api_key = connection_str or os.environ.get("OPENAI_API_KEY")
         if self.api_key is None:
             raise ValueError(
                 "OpenAI API key not set. Set OPENAI_API_KEY environment "
                 "variable or pass through `client_connection`."
             )
         self.host = "https://api.openai.com/v1"
         for key in self.PARAMS:
@@ -72,15 +72,22 @@
         and make sure cache keys are unique to model.
 
         Returns:
             model params.
         """
         return {"model_name": self.NAME, "engine": getattr(self, "engine")}
 
-    def validate_response(self, response: Dict, request: Dict) -> Dict[str, Any]:
+    def supports_streaming_inference(self) -> bool:
+        """Return whether the client supports streaming inference.
+
+        Override in child client class.
+        """
+        return False
+
+    def postprocess_response(self, response: Dict, request: Dict) -> Dict[str, Any]:
         """
         Format response to dict.
 
         Args:
             response: response
             request: request
 
@@ -153,31 +160,28 @@
         request_params = self._format_request_for_embedding(request_params)
         response_dict = super()._run_completion(request_params, retry_timeout)
         # Reformat for text model
         response_dict = self._format_request_from_embedding(response_dict)
         return response_dict
 
     async def _arun_completion(
-        self, request_params: Dict[str, Any], retry_timeout: int, batch_size: int
+        self, request_params: Dict[str, Any], retry_timeout: int
     ) -> Dict:
         """Async execute completion request.
 
         Args:
             request_params: request params.
             retry_timeout: retry timeout.
-            batch_size: batch size for requests.
 
         Returns:
             response as dict.
         """
         # Format for embedding model
         request_params = self._format_request_for_embedding(request_params)
-        response_dict = await super()._arun_completion(
-            request_params, retry_timeout, batch_size
-        )
+        response_dict = await super()._arun_completion(request_params, retry_timeout)
         # Reformat for text model
         response_dict = self._format_request_from_embedding(response_dict)
         return response_dict
 
     def split_usage(self, request: Dict, choices: List[str]) -> List[Dict[str, int]]:
         """Split usage into list of usages for each prompt."""
         try:
```

### Comparing `manifest-ml-0.1.7/manifest/clients/toma.py` & `manifest-ml-0.1.8/manifest/clients/toma.py`

 * *Files 4% similar despite different names*

```diff
@@ -107,14 +107,21 @@
         """
         return {}
 
     def supports_batch_inference(self) -> bool:
         """Return whether the client supports batch inference."""
         return False
 
+    def supports_streaming_inference(self) -> bool:
+        """Return whether the client supports streaming inference.
+
+        Override in child client class.
+        """
+        return False
+
     def get_model_params(self) -> Dict:
         """
         Get model params.
 
         By getting model params from the server, we can add to request
         and make sure cache keys are unique to model.
 
@@ -139,15 +146,15 @@
             now = datetime.now(mod_time.tzinfo)
             heartbeats[mod["name"]] = {
                 "last_ping": (now - mod_time).total_seconds(),
                 "expected_runtime": mod["expected_runtime"],
             }
         return heartbeats
 
-    def validate_response(self, response: Dict, request: Dict) -> Dict[str, Any]:
+    def postprocess_response(self, response: Dict, request: Dict) -> Dict[str, Any]:
         """
         Format response to dict.
 
         Args:
             response: response
             request: request
```

### Comparing `manifest-ml-0.1.7/manifest/clients/toma_diffuser.py` & `manifest-ml-0.1.8/manifest/clients/toma_diffuser.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,15 +42,15 @@
         and make sure cache keys are unique to model.
 
         Returns:
             model params.
         """
         return {"model_name": self.NAME, "engine": getattr(self, "engine")}
 
-    def validate_response(self, response: Dict, request: Dict) -> Dict[str, Any]:
+    def postprocess_response(self, response: Dict, request: Dict) -> Dict[str, Any]:
         """
         Format response to dict.
 
         Args:
             response: response
             request: request
```

### Comparing `manifest-ml-0.1.7/manifest/connections/client_pool.py` & `manifest-ml-0.1.8/manifest/connections/client_pool.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,37 +2,45 @@
 import logging
 import time
 from typing import Any, Dict, List, Optional, Type
 
 from pydantic import BaseModel, Extra
 
 from manifest.clients.ai21 import AI21Client
+from manifest.clients.azureopenai import AzureClient
+from manifest.clients.azureopenai_chat import AzureChatClient
 from manifest.clients.client import Client
 from manifest.clients.cohere import CohereClient
 from manifest.clients.dummy import DummyClient
+from manifest.clients.google import GoogleClient
+from manifest.clients.google_chat import GoogleChatClient
 from manifest.clients.huggingface import HuggingFaceClient
 from manifest.clients.huggingface_embedding import HuggingFaceEmbeddingClient
 from manifest.clients.openai import OpenAIClient
 from manifest.clients.openai_chat import OpenAIChatClient
 from manifest.clients.openai_embedding import OpenAIEmbeddingClient
 from manifest.clients.toma import TOMAClient
 from manifest.connections.scheduler import RandomScheduler, RoundRobinScheduler
 
 logging.getLogger("openai").setLevel(logging.WARNING)
 logger = logging.getLogger(__name__)
 
 CLIENT_CONSTRUCTORS = {
-    OpenAIClient.NAME: OpenAIClient,
-    OpenAIChatClient.NAME: OpenAIChatClient,
-    OpenAIEmbeddingClient.NAME: OpenAIEmbeddingClient,
-    CohereClient.NAME: CohereClient,
     AI21Client.NAME: AI21Client,
+    AzureClient.NAME: AzureClient,
+    AzureChatClient.NAME: AzureChatClient,
+    CohereClient.NAME: CohereClient,
+    DummyClient.NAME: DummyClient,
+    GoogleClient.NAME: GoogleClient,
+    GoogleChatClient.NAME: GoogleChatClient,
     HuggingFaceClient.NAME: HuggingFaceClient,
     HuggingFaceEmbeddingClient.NAME: HuggingFaceEmbeddingClient,
-    DummyClient.NAME: DummyClient,
+    OpenAIClient.NAME: OpenAIClient,
+    OpenAIChatClient.NAME: OpenAIChatClient,
+    OpenAIEmbeddingClient.NAME: OpenAIEmbeddingClient,
     TOMAClient.NAME: TOMAClient,
 }
 
 CLIENT_REQUEST_TYPES: Dict[str, Type] = {
     k: v.REQUEST_CLS for k, v in CLIENT_CONSTRUCTORS.items()
 }
```

### Comparing `manifest-ml-0.1.7/manifest/connections/scheduler.py` & `manifest-ml-0.1.8/manifest/connections/scheduler.py`

 * *Files identical despite different names*

### Comparing `manifest-ml-0.1.7/manifest/manifest.py` & `manifest-ml-0.1.8/manifest/manifest.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,23 @@
 """Manifest class."""
 import asyncio
 import copy
 import logging
-from typing import Any, Dict, List, Optional, Tuple, Type, Union, cast
+from typing import (
+    Any,
+    Dict,
+    Generator,
+    Iterator,
+    List,
+    Optional,
+    Tuple,
+    Type,
+    Union,
+    cast,
+)
 
 import numpy as np
 
 from manifest.caches.noop import NoopCache
 from manifest.caches.postgres import PostgresCache
 from manifest.caches.redis import RedisCache
 from manifest.caches.sqlite import SQLiteCache
@@ -287,42 +298,71 @@
 
     def run(
         self,
         prompt: Union[str, List[str], List[Dict[str, str]]],
         overwrite_cache: bool = False,
         stop_token: Optional[str] = None,
         return_response: bool = False,
+        stream: bool = False,
         **kwargs: Any,
-    ) -> Union[str, List[str], np.ndarray, List[np.ndarray], Response]:
+    ) -> Union[
+        str,
+        List[str],
+        np.ndarray,
+        List[np.ndarray],
+        Response,
+        Iterator[str],
+        Iterator[Response],
+    ]:
         """
         Run the prompt.
 
         Orchestrates between the standard run and chat run and batch run.
 
         Args:
             prompt: prompt(s) to run.
             overwrite_cache: whether to overwrite cache.
             stop_token: stop token for prompt generation.
-                        Default is self.stop_token.
-                        "" for no stop token.
+                Default is self.stop_token.
+                "" for no stop token.
             return_response: whether to return Response object.
+            stream: whether to stream the prompt. Only supported
+                for single string prompts and LMs.
 
         Returns:
             response from prompt.
         """
         if not isinstance(prompt, list) and not isinstance(prompt, str):
             raise ValueError(
                 f"Invalid prompt type: {type(prompt)}. "
                 "Prompt must be a string or list of strings "
                 "or list of dicts."
             )
         if isinstance(prompt, list) and not prompt:
             raise ValueError("Prompt cannot be empty list")
         # Get the client to run
         client = self.client_pool.get_next_client()
+        if stream:
+            if not client.supports_streaming_inference():
+                raise ValueError(
+                    f"Client {client} does not support streaming inference."
+                )
+            if not isinstance(prompt, str):
+                raise ValueError(
+                    "Stream is only supported for single string prompts. "
+                    "It will soon be supported for chat dictionary prompts, too."
+                )
+            return self._run_stream(
+                prompt=cast(str, prompt),
+                client=client,
+                overwrite_cache=overwrite_cache,
+                stop_token=stop_token,
+                return_response=return_response,
+                **kwargs,
+            )
         if isinstance(prompt, list) and isinstance(prompt[0], dict):
             if not client.IS_CHAT:
                 raise ValueError(
                     f"Client {client} does not support dict chat prompt. "
                     "Please use a chat model."
                 )
             if stop_token:
@@ -333,23 +373,22 @@
             return self._run_chat(
                 prompt=cast(List[Dict[str, str]], prompt),
                 client=client,
                 overwrite_cache=overwrite_cache,
                 return_response=return_response,
                 **kwargs,
             )
-        else:
-            return self._run(
-                prompt=cast(Union[str, List[str]], prompt),
-                client=client,
-                overwrite_cache=overwrite_cache,
-                stop_token=stop_token,
-                return_response=return_response,
-                **kwargs,
-            )
+        return self._run(
+            prompt=cast(Union[str, List[str]], prompt),
+            client=client,
+            overwrite_cache=overwrite_cache,
+            stop_token=stop_token,
+            return_response=return_response,
+            **kwargs,
+        )
 
     def _run(
         self,
         prompt: Union[str, List[str]],
         client: Client,
         overwrite_cache: bool = False,
         stop_token: Optional[str] = None,
@@ -395,15 +434,14 @@
 
         final_response = self._stitch_responses_and_cache(
             request=request_params,
             client=client,
             response=response,
             cached_idx_to_response=cached_idx_to_response,
         )
-
         # Extract text results
         if return_response:
             return final_response
         else:
             return final_response.get_response(stop_token, is_batch)
 
     def _run_chat(
@@ -463,21 +501,93 @@
 
         # Extract text results
         if return_response:
             return final_response
         else:
             return cast(str, final_response.get_response("", is_batch))
 
+    def _run_stream(
+        self,
+        prompt: str,
+        client: Client,
+        overwrite_cache: bool = False,
+        stop_token: Optional[str] = None,
+        return_response: bool = False,
+        **kwargs: Any,
+    ) -> Union[Generator[str, None, None], Generator[Response, None, None]]:
+        """
+        Run the prompt in a stream.
+
+        Args:
+            prompt: prompt(s) to run.
+            client: client to run.
+            overwrite_cache: whether to overwrite cache.
+            stop_token: stop token for prompt generation.
+                        Default is self.stop_token.
+                        "" for no stop token.
+            return_response: whether to return Response object.
+
+        Returns:
+            response from prompt.
+        """
+        is_batch = False
+        stop_token = stop_token if stop_token is not None else self.stop_token
+        # Must pass kwargs as dict for client "pop" methods removed used arguments
+        request_params = client.get_request(prompt, kwargs)
+        # Avoid nested list of results - enforce n = 1 for batch
+        if request_params.n > 1:
+            raise ValueError("Stream mode does not support n > 1.")
+        self._validate_kwargs(kwargs, request_params)
+
+        cached_idx_to_response, request_params = self._split_cached_requests(
+            request_params, client, overwrite_cache
+        )
+        if request_params.prompt:
+            # Because we are streaming, we should have either a cached response
+            # a prompt to run
+            assert len(cached_idx_to_response) == 0
+            response_iter = client.run_streaming_request(request_params)
+            is_cached = False
+        else:
+            assert len(cached_idx_to_response) == 1
+            response_iter = cached_idx_to_response[0].as_iter()
+            is_cached = True
+
+        saved_responses = []
+        # Start timing metrics
+        self.client_pool.start_timer()
+        for response_token in response_iter:
+            saved_responses.append(response_token)
+            if return_response:
+                yield response_token
+            else:
+                yield cast(
+                    Union[str, Response], response_token.get_response("", is_batch)
+                )
+        self.client_pool.end_timer()
+
+        if not is_cached:
+            final_response = Response.union_all(
+                saved_responses, as_single_lmchoice=True
+            )
+            self._stitch_responses_and_cache(
+                request=request_params,
+                client=client,
+                response=final_response,
+                cached_idx_to_response=cached_idx_to_response,
+            )
+
     async def arun_batch(
         self,
         prompts: List[str],
         overwrite_cache: bool = False,
         stop_token: Optional[str] = None,
         return_response: bool = False,
         chunk_size: int = -1,
+        verbose: bool = False,
         **kwargs: Any,
     ) -> Union[List[str], List[np.ndarray], Response]:
         """
         Run a batch of prompts with async.
 
         If the client pool is a single client, all prompts will be sent
         to one client and batch_size (which is passed it as kwargs) will
@@ -496,26 +606,27 @@
             return_response: whether to return Response object.
             chunk_size: number of prompts to send to a client in chunks.
                 For each chunk, the client will split the chunk into
                 batch_sized prompts to send to the model.
                 For a single manifest client, there is no impact to
                 setting chunk_size. For a client pool, chunk_size
                 can be used to distribute the load across the clients.
+            verbose: whether to print progress of async tasks.
 
         Returns:
             response from prompt.
         """
         if not isinstance(prompts, list):
             raise ValueError("Prompts must be a list of strings.")
         if not prompts:
             raise ValueError("Prompts must not be empty.")
         if not isinstance(prompts[0], str):
             raise ValueError("Prompts must be a list of strings.")
 
-        # Split the prompts into chunks
+        # Split the prompts into chunks for connection pool
         prompt_chunks: List[Tuple[Client, List[str]]] = []
         if chunk_size > 0:
             for i in range(0, len(prompts), chunk_size):
                 prompt_chunks.append(
                     (self.client_pool.get_next_client(), prompts[i : i + chunk_size])
                 )
         else:
@@ -526,19 +637,19 @@
         for client, chunk in prompt_chunks:
             tasks.append(
                 asyncio.create_task(
                     self._arun_batch_client(
                         prompts=chunk,
                         client=client,
                         overwrite_cache=overwrite_cache,
+                        verbose=verbose,
                         **kwargs,
                     )
                 )
             )
-        print(f"Running {len(tasks)} tasks across all clients.")
         logger.info(f"Running {len(tasks)} tasks across all clients.")
         responses = await asyncio.gather(*tasks)
         final_response = Response.union_all(responses)
         stop_token = stop_token if stop_token is not None else self.stop_token
 
         # Extract text results
         if return_response:
@@ -550,23 +661,25 @@
             )
 
     async def _arun_batch_client(
         self,
         prompts: List[str],
         client: Client,
         overwrite_cache: bool = False,
+        verbose: bool = False,
         **kwargs: Any,
     ) -> Response:
         """
         Run a batch of prompts with async for single client.
 
         Args:
             prompts: prompts to run.
             client: client to run.
             overwrite_cache: whether to overwrite cache.
+            verbose: whether to print progress of async tasks.
 
         Returns:
             response from prompt.
         """
         # Must pass kwargs as dict for client "pop" methods removed used arguments
         request_params = client.get_request(prompts, kwargs)
         # Avoid nested list of results - enforce n = 1 for batch
@@ -576,15 +689,15 @@
 
         cached_idx_to_response, request_params = self._split_cached_requests(
             request_params, client, overwrite_cache
         )
         # If not None value or empty list - run new request
         if request_params.prompt:
             self.client_pool.start_timer()
-            response = await client.arun_batch_request(request_params)
+            response = await client.arun_batch_request(request_params, verbose=verbose)
             self.client_pool.end_timer()
         else:
             # Nothing to run
             response = None
 
         final_response = self._stitch_responses_and_cache(
             request=request_params,
```

### Comparing `manifest-ml-0.1.7/manifest/request.py` & `manifest-ml-0.1.8/manifest/request.py`

 * *Files identical despite different names*

### Comparing `manifest-ml-0.1.7/manifest/response.py` & `manifest-ml-0.1.8/manifest/response.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Client response."""
 import copy
 import json
-from typing import Any, Dict, List, Optional, Type, Union, cast
+from typing import Any, Dict, Generator, List, Optional, Type, Union, cast
 
 import numpy as np
 from pydantic import BaseModel
 
 from manifest.request import (
     ENGINE_SEP,
     DiffusionRequest,
@@ -150,17 +150,15 @@
         """
         Get all results from response.
 
         Args:
             stop_token: stop token for string generation
             is_batch: whether response is batched
         """
-        process_result = (
-            lambda x: x.strip().split(stop_token)[0] if stop_token else x.strip()
-        )
+        process_result = lambda x: x.split(stop_token)[0] if stop_token else x
         extracted_items = [
             choice.text if isinstance(choice, LMModelChoice) else choice.array
             for choice in self._response.choices
         ]
         if len(extracted_items) == 0:
             return None
         if isinstance(extracted_items[0], str):
@@ -169,39 +167,51 @@
             processed_results = extracted_items
         if len(processed_results) == 1 and not is_batch:
             return processed_results[0]
         else:
             return processed_results
 
     @classmethod
-    def union_all(cls, responses: List["Response"]) -> "Response":
-        """Union a list of response."""
+    def union_all(
+        cls, responses: List["Response"], as_single_lmchoice: bool = False
+    ) -> "Response":
+        """Union a list of response.
+
+        Args:
+            responses: list of responses to union.
+            as_single_lmchoice: if True, will concatenate all responses into a single
+                model choice. Useful for merging streaming responses. Only valid
+                for LMRequest responses.
+        """
         if not responses:
             raise ValueError("Response list is empty.")
         if len(responses) == 1:
             return responses[0]
         first_response = responses[0]
         request_type = first_response._request_type
         response_type = first_response._response_type
         request = first_response.get_request_obj()
 
+        if as_single_lmchoice and response_type != "text":
+            raise ValueError("as_single_lmchoice=True only works for text responses.")
+
         # Make sure all responses have the same keys
         if not all(
             [
                 (r._request_type == request_type)
                 and (r._response_type == response_type)
                 for r in responses
             ]
         ):
             raise ValueError("All responses must have the same keys.")
 
         # Get all the prompts and model choices
         all_prompts = []
         all_choices = []
-        all_usages = []
+        all_usages: List[Usage] = []
         all_engines = []
         for res in responses:
             all_engines.extend(res.get_request_obj().engine.split(ENGINE_SEP))
             res_prompt = res.get_request_obj().prompt
             if isinstance(res_prompt, str):
                 res_prompt = [res_prompt]
             all_prompts.extend(res_prompt)
@@ -209,26 +219,123 @@
             if res.get_usage_obj().usages:
                 all_usages.extend(res.get_usage_obj().usages)
             else:
                 # Add empty usages if not present
                 all_usages.extend([Usage()] * len(res_prompt))
         new_request = copy.deepcopy(request)
         new_request.engine = ENGINE_SEP.join(sorted(set(all_engines)))
-        new_request.prompt = all_prompts
-        new_response = ModelChoices(choices=all_choices)
-        new_usages = Usages(usages=all_usages)
-        response_obj = cls(
-            response=new_response,
-            cached=any(res.is_cached() for res in responses),
-            request=new_request,
-            usages=new_usages,
-            request_type=request_type,
-            response_type=response_type,
-        )
-        return response_obj
+
+        if as_single_lmchoice:
+            if len(set(all_prompts)) != 1:
+                raise ValueError("Prompts must be the same for as_single_lmchoice=True")
+            all_choices_txt = cast(List[LMModelChoice], all_choices)  # type: ignore
+            single_prompt = all_prompts[0]
+            single_text = "".join([choice.text for choice in all_choices_txt])
+            single_logprobs = [
+                logprob
+                for choice in all_choices_txt
+                for logprob in choice.token_logprobs or []
+            ]
+            single_tokens = [
+                token for choice in all_choices_txt for token in choice.tokens or []
+            ]
+            single_usage = Usage(
+                completion_tokens=sum(usg.completion_tokens for usg in all_usages),
+                prompt_tokens=sum(usg.prompt_tokens for usg in all_usages),
+                total_tokens=sum(usg.total_tokens for usg in all_usages),
+            )
+            new_choices = [
+                LMModelChoice(
+                    text=single_text,
+                    token_logprobs=single_logprobs,
+                    tokens=single_tokens,
+                )
+            ]
+            new_responses = ModelChoices(choices=new_choices)  # type: ignore
+            new_usages = Usages(usages=[single_usage])
+            new_request.prompt = single_prompt
+            response_obj = cls(
+                response=new_responses,
+                cached=any(res.is_cached() for res in responses),
+                request=new_request,
+                usages=new_usages,
+                request_type=request_type,
+                response_type=response_type,
+            )
+            return response_obj
+        else:
+            new_request.prompt = all_prompts
+            new_response = ModelChoices(choices=all_choices)
+            new_usages = Usages(usages=all_usages)
+            response_obj = cls(
+                response=new_response,
+                cached=any(res.is_cached() for res in responses),
+                request=new_request,
+                usages=new_usages,
+                request_type=request_type,
+                response_type=response_type,
+            )
+            return response_obj
+
+    # Return a token by token iterator over the response
+    def as_iter(self) -> Generator["Response", None, None]:
+        """Return a token by token iterator over the response.
+
+        Will return iterator of responses with one token each.
+        """
+        if self._response_type not in {"text"}:
+            raise ValueError(
+                f"Invalid response type {self._response_type} for as_iter()"
+            )
+        if not self._response.choices:
+            raise ValueError("No choices in response.")
+        if len(self._response.choices) > 1:
+            raise ValueError(
+                "Response has more than one choice. as_iter() "
+                "should be over single choice responses."
+            )
+        if not isinstance(self._response.choices[0], LMModelChoice):
+            raise ValueError(
+                "response_type is text but response is "
+                f"{self._response.choices[0].__class__}"
+            )
+        choice = cast(LMModelChoice, self._response.choices[0])
+        # If tokens, return iterator of tokens
+        if choice.tokens:
+            for token, logprob in zip(choice.tokens, choice.token_logprobs):
+                yield Response(
+                    response=ModelChoices(
+                        choices=[
+                            LMModelChoice(
+                                text=token, token_logprobs=[logprob], tokens=[token]
+                            )
+                        ]
+                    ),
+                    cached=self._cached,
+                    request=self._request,
+                    usages=self._usages,
+                    request_type=self._request_type,
+                    response_type=self._response_type,
+                )
+        # Otherwise, do it by words
+        else:
+            for i, word in enumerate(choice.text.split(" ")):
+                word = " " + word if i > 0 else word
+                yield Response(
+                    response=ModelChoices(
+                        choices=[
+                            LMModelChoice(text=word, token_logprobs=None, tokens=None)
+                        ]
+                    ),
+                    cached=self._cached,
+                    request=self._request,
+                    usages=self._usages,
+                    request_type=self._request_type,
+                    response_type=self._response_type,
+                )
 
     def serialize(self) -> str:
         """
         Serialize response to string.
 
         Returns:
             serialized response.
```

### Comparing `manifest-ml-0.1.7/manifest_ml.egg-info/PKG-INFO` & `manifest-ml-0.1.8/manifest_ml.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: manifest-ml
-Version: 0.1.7
+Version: 0.1.8
 Summary: Manifest for Prompting Foundation Models.
 Home-page: https://github.com/HazyResearch/manifest
 Author: Laurel Orr
 Author-email: laurel.orr@numbersstation.ai
 License: Apache 2.0
-Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
 Provides-Extra: api
@@ -26,17 +25,18 @@
 How to make prompt programming with Foundation Models a little easier.
 
 
 # Table of Contents
 - [Install](#install)
 - [Getting Started](#getting-started)
 - [Manifest](#manifest-components)
-- [Local HuggingFace Models](#local-huggingface-models)
-- [Chat Models](#chat-models)
-- [Embedding Models](#embedding-models)
+- [Other Models Types](#other-models)
+    - [Local HuggingFace Models](#local-huggingface-models)
+    - [Chat Models](#chat-models)
+    - [Embedding Models](#embedding-models)
 - [Road Map](#road-map)
 - [Development](#development)
 - [Cite](#cite)
 
 
 # Install
 Install:
@@ -63,15 +63,15 @@
 
 # Getting Started
 Running is simple to get started. If using OpenAI, set `export OPENAI_API_KEY=<OPENAIKEY>` (or pass key in through variable `client_connection`) then run
 
 ```python
 from manifest import Manifest
 
-# Start a manifest session to OpenAI - default `engine=text-davinci-002`
+# Start a manifest session to OpenAI - default `engine=text-davinci-003`
 manifest = Manifest(
     client_name = "openai",
 )
 manifest.run("Why is the grass green?")
 ```
 
 ## Examples
@@ -162,14 +162,24 @@
 ```
 
 If you want to change default parameters to a model, we pass those as `kwargs` to the client.
 ```python
 result = manifest.run(prompt, "Laurel", max_tokens=50)
 ```
 
+## Streaming Queries
+Manifest also supports streaming the model response back, assuming it's supported by the underlying client. When calling `run`, pass `stream=True` to get a streaming iterator in response.
+
+```python
+result_iterator = manifest.run("Tell me a story. Once upon a time", max_tokens=100, stream=True)
+for res_text in result_iterator:
+    print(res_text)
+```
+Streaming responses are only supported for single string queries (not batch mode) for text completion models.
+
 ## Model Pools
 Manifest supports querying multiple models with different schedulers. This is very much a work in progress effort, but Manifest will round robin select (or randomly select) the clients you want. You can use the same client multiple times with different connection strings (e.g. different API keys), or you can mix and match. The only requirement is that all clients are the same request type. I.e. you can't have a pool of generation models and embedding models.
 
 To query between a local model and OpenAI,
 ```python
 from manifest.connections.client_pool import ClientConnection
 from manifest import Manifest
@@ -189,15 +199,17 @@
 
 The speed benefit comes in with async batched runs. When calling `arun_batch` with a list of prompts, Manifest supports a `chunk_size` param. This will break the prompts into `chunk_size` chunks to spread across the client pool. By default `chunk_size` is `-1` which means only one client will get all the prompts to run asynchronously. You must set `chunk_size > 1` to distribute across the pool. There is a further `batch_size` param which control the individual client `batch_size` to send to the model.
 
 ```python
 responses = asyncio.run(manifest.arun_batch(prompts, max_tokens=30, chunk_size=20))
 ```
 
-# Local Huggingface Models
+# Other Models
+
+## Local Huggingface Models
 To use a HuggingFace generative model, in `manifest/api` we have a Flask application that hosts the models for you.
 
 In a separate terminal or Tmux/Screen session, to load 6B parameters models, run
 ```bash
 python3 -m manifest.api.app \
     --model_type huggingface \
     --model_name_or_path EleutherAI/gpt-j-6B \
@@ -237,27 +249,27 @@
 python3 -m manifest.api.app \
     --model_type huggingface \
     --model_name_or_path bigscience/bloom \
     --use_bitsandbytes \
     --percent_max_gpu_mem_reduction 0.85
 ```
 
-# Chat Models
+## Chat Models
 Manifest has specific support for executing against chat models in the more standard "system" / "user" dialogue. To pass in a dialogue history to Manifest, use the `run` command with a list of dictionary inputs with `role` and `content` keys using an associated chat model such as `openaichat`.
 
 ```python
 manifest = Manifest(client_name="openaichat")
 dialogue = [
     {"role": "system", "content": "You are a helpful assistant who also responds in rhymes"},
     {"role": "user", "content": "What is the date?"},
 ]
 res = manifest.run(dialogue, max_tokens=100)
 ```
 
-# Embedding Models
+## Embedding Models
 Manifest also supports getting embeddings from models and available APIs. We do this all through changing the `client_name` argument. You still use `run` and `abatch_run`.
 
 To use OpenAI's embedding models, simply run
 ```python
 manifest = Manifest(client_name="openaiembedding")
 embedding_as_np = manifest.run("Get me an embedding for a bunny")
 ```
@@ -270,19 +282,22 @@
     --device 0
 ```
 
 # Road Map
 Here's what's coming up next
 - [ ] Clients
   - [ ] HuggingFace Hub
-  - [ ] Azure OpenAI
+  - [x] Azure OpenAI
+  - [x] Google Vertex
   - [ ] Anthropic
+  - [x] Streaming Support Completions
+  - [ ] Streaming Support Chat Models
 - [ ] Data Types
   - [ ] Diffusion Models
-- [ ] Orchestration
+- [x] Orchestration
   - [x] Connection pools
 - [ ] Local Inference
   - [ ] FlexGen
 
 # Development
 Before submitting a PR, run
 ```bash
@@ -299,9 +314,7 @@
   author = {Orr, Laurel},
   title = {Manifest},
   year = {2022},
   publisher = {GitHub},
   howpublished = {\url{https://github.com/HazyResearch/manifest}},
 }
 ```
-
-
```

### Comparing `manifest-ml-0.1.7/manifest_ml.egg-info/SOURCES.txt` & `manifest-ml-0.1.8/manifest_ml.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -21,18 +21,22 @@
 manifest/caches/noop.py
 manifest/caches/postgres.py
 manifest/caches/redis.py
 manifest/caches/serializers.py
 manifest/caches/sqlite.py
 manifest/clients/__init__.py
 manifest/clients/ai21.py
+manifest/clients/azureopenai.py
+manifest/clients/azureopenai_chat.py
 manifest/clients/client.py
 manifest/clients/cohere.py
 manifest/clients/diffuser.py
 manifest/clients/dummy.py
+manifest/clients/google.py
+manifest/clients/google_chat.py
 manifest/clients/huggingface.py
 manifest/clients/huggingface_embedding.py
 manifest/clients/openai.py
 manifest/clients/openai_chat.py
 manifest/clients/openai_embedding.py
 manifest/clients/toma.py
 manifest/clients/toma_diffuser.py
```

### Comparing `manifest-ml-0.1.7/manifest_ml.egg-info/requires.txt` & `manifest-ml-0.1.8/manifest_ml.egg-info/requires.txt`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -5,53 +5,53 @@
 aiohttp>=3.8.0
 sqlitedict>=2.0.0
 tenacity>=8.2.0
 tiktoken>=0.3.0
 xxhash>=3.0.0
 
 [all]
+pytest-cov>=3.0.0
 mypy>=0.950
-types-setuptools>=57.4.17
+sentence_transformers>=2.2.0
+nbsphinx>=0.8.0
+types-python-dateutil>=2.8.16
+uvicorn>=0.18.0
+black>=22.3.0
 flake8-docstrings>=1.6.0
+twine
 python-dotenv>=0.20.0
-torch>=1.8.0
-recommonmark>=0.7.1
-pg8000
+transformers<4.31.0,>=4.29.0
+Flask>=2.1.2
 types-redis>=4.2.6
-types-pillow>=9.0.0
-isort>=5.9.3
-pre-commit>=2.14.0
-cloud-sql-python-connector[pg8000]>=1.0.0
-nbsphinx>=0.8.0
-pytest>=7.0.0
+flake8>=4.0.0
+sphinx-autobuild
+types-protobuf>=3.19.21
 sqlalchemy
-twine
 types-xxhash>=3.0.0
-types-python-dateutil>=2.8.16
+diffusers>=0.6.0
+isort>=5.9.3
 sphinx-rtd-theme>=0.5.1
-sphinx-autobuild
-Flask>=2.1.2
-pep8-naming>=0.12.1
-docformatter>=1.4
+types-requests>=2.27.29
+pg8000
 pillow>=9.0.0
-transformers<4.31.0,>=4.29.0
-black>=22.3.0
-uvicorn>=0.18.0
-autopep8>=1.6.0
+types-pillow>=9.0.0
 tokenizers>=0.13.3
-flake8>=4.0.0
-sentence_transformers>=2.2.0
+accelerate>=0.10.0
 types-PyYAML>=6.0.7
-types-protobuf>=3.19.21
+docformatter>=1.4
+torch>=1.8.0
+pep8-naming>=0.12.1
+pre-commit>=2.14.0
+recommonmark>=0.7.1
 fastapi>=0.70.0
-types-requests>=2.27.29
-pytest-cov>=3.0.0
-diffusers>=0.6.0
+cloud-sql-python-connector[pg8000]>=1.0.0
 deepspeed>=0.7.0
-accelerate>=0.10.0
+types-setuptools>=57.4.17
+autopep8>=1.6.0
+pytest>=7.0.0
 
 [api]
 accelerate>=0.10.0
 deepspeed>=0.7.0
 diffusers>=0.6.0
 Flask>=2.1.2
 sentence_transformers>=2.2.0
```

### Comparing `manifest-ml-0.1.7/pyproject.toml` & `manifest-ml-0.1.8/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -2,27 +2,29 @@
 [tool.mypy]
 disallow_untyped_defs = true
 strict_optional = false
 
 [[tool.mypy.overrides]]
 ignore_missing_imports = true
 module = [
+  "accelerate",
+  "accelerate.utils.modeling",
   "deepspeed",
-  "numpy",
   "diffusers",
-  "sentence_transformers",
-  "sqlitedict",
-  "sqlalchemy",
   "dill",
-  "accelerate",
-  "accelerate.utils.modeling",
-  "transformers",
   "flask",
-  "torch",
+  "numpy",
   "pyChatGPT",
+  "torch",
+  "transformers",
+  "tqdm",
+  "tqdm.asyncio",
+  "sentence_transformers",
+  "sqlalchemy",
+  "sqlitedict",
 ]
 
 [tool.isort]
 combine_as_imports = true
 force_grid_wrap = 0
 include_trailing_comma = true
 known_first_party = ["manifest"]
```

### Comparing `manifest-ml-0.1.7/setup.py` & `manifest-ml-0.1.8/setup.py`

 * *Files identical despite different names*

### Comparing `manifest-ml-0.1.7/tests/test_array_cache.py` & `manifest-ml-0.1.8/tests/test_array_cache.py`

 * *Files identical despite different names*

### Comparing `manifest-ml-0.1.7/tests/test_cache.py` & `manifest-ml-0.1.8/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `manifest-ml-0.1.7/tests/test_client.py` & `manifest-ml-0.1.8/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `manifest-ml-0.1.7/tests/test_client_pool.py` & `manifest-ml-0.1.8/tests/test_client_pool.py`

 * *Files identical despite different names*

### Comparing `manifest-ml-0.1.7/tests/test_huggingface_api.py` & `manifest-ml-0.1.8/tests/test_huggingface_api.py`

 * *Files identical despite different names*

### Comparing `manifest-ml-0.1.7/tests/test_manifest.py` & `manifest-ml-0.1.8/tests/test_manifest.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Manifest test."""
 import asyncio
 import os
-from typing import cast
+from typing import Iterator, cast
 from unittest.mock import MagicMock, Mock, patch
 
 import numpy as np
 import pytest
 import requests
 from requests import HTTPError
 
@@ -783,23 +783,63 @@
     assert response.get_usage_obj().usages[1].total_tokens == 15
 
     response = cast(
         Response, client.run("Why are there oranges?", return_response=True)
     )
     assert response.is_cached() is True
 
+    # Test streaming
+    num_responses = 0
+    streaming_response_text = cast(
+        Iterator[str], client.run("Why are there oranges?", stream=True)
+    )
+    for res_text in streaming_response_text:
+        num_responses += 1
+        assert isinstance(res_text, str) and len(res_text) > 0
+    assert num_responses == 8
+
+    streaming_response = cast(
+        Iterator[Response],
+        client.run("Why are there mandarines?", return_response=True, stream=True),
+    )
+    num_responses = 0
+    merged_res = []
+    for res in streaming_response:
+        num_responses += 1
+        assert isinstance(res, Response) and len(res.get_response()) > 0
+        merged_res.append(cast(str, res.get_response()))
+        assert not res.is_cached()
+    assert num_responses == 10
+
+    # Make sure cached
+    streaming_response = cast(
+        Iterator[Response],
+        client.run("Why are there mandarines?", return_response=True, stream=True),
+    )
+    num_responses = 0
+    merged_res_cachced = []
+    for res in streaming_response:
+        num_responses += 1
+        assert isinstance(res, Response) and len(res.get_response()) > 0
+        merged_res_cachced.append(cast(str, res.get_response()))
+        assert res.is_cached()
+    # OpenAI stream does not return logprobs, so this is by number of words
+    assert num_responses == 7
+    assert "".join(merged_res) == "".join(merged_res_cachced)
+
 
 @pytest.mark.skipif(not OPENAI_ALIVE, reason="No openai key set")
 @pytest.mark.usefixtures("sqlite_cache")
 def test_openaichat(sqlite_cache: str) -> None:
     """Test openaichat client."""
     client = Manifest(
         client_name="openaichat",
         cache_name="sqlite",
         cache_connection=sqlite_cache,
+        temperature=0.0,
     )
 
     res = client.run("Why are there apples?")
     assert isinstance(res, str) and len(res) > 0
 
     response = cast(Response, client.run("Why are there apples?", return_response=True))
     assert isinstance(response.get_response(), str) and len(response.get_response()) > 0
@@ -864,14 +904,53 @@
             "content": "The Los Angeles Dodgers won the World Series in 2020.",
         },
         {"role": "user", "content": "Where was it played?"},
     ]
     response = cast(Response, client.run(chat_dict, return_response=True))
     assert response.is_cached() is False
 
+    # Test streaming
+    num_responses = 0
+    streaming_response_text = cast(
+        Iterator[str], client.run("Why are there oranges?", stream=True)
+    )
+    for res_text in streaming_response_text:
+        num_responses += 1
+        assert isinstance(res_text, str) and len(res_text) > 0
+    assert num_responses == 9
+
+    streaming_response = cast(
+        Iterator[Response],
+        client.run("Why are there mandarines?", return_response=True, stream=True),
+    )
+    num_responses = 0
+    merged_res = []
+    for res in streaming_response:
+        num_responses += 1
+        assert isinstance(res, Response) and len(res.get_response()) > 0
+        merged_res.append(cast(str, res.get_response()))
+        assert not res.is_cached()
+    assert num_responses == 10
+
+    # Make sure cached
+    streaming_response = cast(
+        Iterator[Response],
+        client.run("Why are there mandarines?", return_response=True, stream=True),
+    )
+    num_responses = 0
+    merged_res_cachced = []
+    for res in streaming_response:
+        num_responses += 1
+        assert isinstance(res, Response) and len(res.get_response()) > 0
+        merged_res_cachced.append(cast(str, res.get_response()))
+        assert res.is_cached()
+    # OpenAI stream does not return logprobs, so this is by number of words
+    assert num_responses == 7
+    assert "".join(merged_res) == "".join(merged_res_cachced)
+
 
 @pytest.mark.skipif(not OPENAI_ALIVE, reason="No openai key set")
 @pytest.mark.usefixtures("sqlite_cache")
 def test_openaiembedding(sqlite_cache: str) -> None:
     """Test openaichat client."""
     client = Manifest(
         client_name="openaiembedding",
@@ -1152,15 +1231,15 @@
         "The sky is purple. This is because",
         "The sky is magnet. This is because",
         "The sky is fuzzy. This is because",
     ]
     with patch("manifest.clients.client.requests.post", mock_create):
         # Run manifest
         result = client.run(prompts, temperature=0, overwrite_cache=True)
-        assert result == ["WHATTT.", "UH OH.", "HARG"]
+        assert result == [" WHATTT.", " UH OH.", " HARG"]
 
         # Assert that OpenAI client was called twice
         assert mock_create.call_count == 2
 
     # Now make sure it errors when not a 429 or 500
     mock_create = MagicMock(
         side_effect=[
```

### Comparing `manifest-ml-0.1.7/tests/test_request.py` & `manifest-ml-0.1.8/tests/test_request.py`

 * *Files identical despite different names*

### Comparing `manifest-ml-0.1.7/tests/test_response.py` & `manifest-ml-0.1.8/tests/test_response.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,15 +2,21 @@
 from typing import List, cast
 
 import numpy as np
 import pytest
 
 from manifest import Response
 from manifest.request import EmbeddingRequest, LMRequest
-from manifest.response import ArrayModelChoice, ModelChoices, Usage, Usages
+from manifest.response import (
+    ArrayModelChoice,
+    LMModelChoice,
+    ModelChoices,
+    Usage,
+    Usages,
+)
 
 
 def test_init(
     model_choice: ModelChoices,
     model_choice_arr: ModelChoices,
     model_choice_arr_int: ModelChoices,
     request_lm: LMRequest,
@@ -271,17 +277,17 @@
         request_type=LMRequest,
         response_type="text",
     )
 
     final_response = Response.union_all([response1, response2])
     assert final_response.get_json_response() == {
         "choices": [
-            {"text": "hello", "token_logprobs": [0.1, 0.2], "tokens": None},
-            {"text": "bye", "token_logprobs": [0.3], "tokens": None},
-            {"text": "helloo", "token_logprobs": [0.1, 0.2], "tokens": None},
+            {"text": "hello", "token_logprobs": [0.1, 0.2], "tokens": ["hel", "lo"]},
+            {"text": "bye", "token_logprobs": [0.3], "tokens": ["bye"]},
+            {"text": "helloo", "token_logprobs": [0.1, 0.2], "tokens": ["hel", "loo"]},
         ]
     }
     assert final_response.get_usage_obj() == Usages(usages=[Usage(), Usage(), Usage()])
     merged_prompts: List[str] = request_lm.prompt + [request_lm_single.prompt]  # type: ignore  # noqa: E501
     assert final_response.get_request_obj().prompt == merged_prompts
     assert final_response.get_request_obj().engine == "dummy::text-ada-001"
 
@@ -295,7 +301,87 @@
         response_type="text",
     )
 
     final_response = Response.union_all([response1, response2])
     assert final_response.get_usage_obj() == Usages(
         usages=[Usage(total_tokens=4), Usage(total_tokens=6), Usage()]
     )
+
+    # Test merge to single
+    model_choices = ModelChoices(
+        choices=[
+            LMModelChoice(
+                text=" helloo this is a bug",
+                token_logprobs=[0.1, 0.2, 0.3],
+                tokens=[" helloo", " this is", " a bug"],
+            ),
+        ]
+    )
+    request = LMRequest(prompt="monkey", engine="dummy")
+    response1 = Response(
+        response=model_choices,
+        cached=False,
+        request=request,
+        usages=None,
+        request_type=LMRequest,
+        response_type="text",
+    )
+    final_response = Response.union_all([response1, response1], as_single_lmchoice=True)
+    assert final_response.get_json_response() == {
+        "choices": [
+            {
+                "text": " helloo this is a bug helloo this is a bug",
+                "token_logprobs": [0.1, 0.2, 0.3, 0.1, 0.2, 0.3],
+                "tokens": [
+                    " helloo",
+                    " this is",
+                    " a bug",
+                    " helloo",
+                    " this is",
+                    " a bug",
+                ],
+            },
+        ]
+    }
+    assert final_response.get_usage_obj() == Usages(usages=[Usage()])
+    assert final_response.get_request_obj().prompt == "monkey"
+    assert final_response.get_request_obj().engine == "dummy"
+
+
+def test_as_iter(
+    model_choice_single: ModelChoices, request_lm_single: LMRequest
+) -> None:
+    """Test as iter."""
+    response = Response(
+        response=model_choice_single,
+        cached=False,
+        request=request_lm_single,
+        usages=None,
+        request_type=LMRequest,
+        response_type="text",
+    )
+    response_iter_list = list(response.as_iter())
+    assert len(response_iter_list) == 2
+    assert response_iter_list[0].get_response() == "hel"
+    assert response_iter_list[1].get_response() == "loo"
+
+    model_choices = ModelChoices(
+        choices=[
+            LMModelChoice(text="helloo this is a bug"),
+        ]
+    )
+    request = LMRequest(prompt="monkey", engine="dummy")
+    response = Response(
+        response=model_choices,
+        cached=False,
+        request=request,
+        usages=None,
+        request_type=LMRequest,
+        response_type="text",
+    )
+    response_iter_list = list(response.as_iter())
+    assert len(response_iter_list) == 5
+    assert response_iter_list[0].get_response() == "helloo"
+    assert response_iter_list[1].get_response() == " this"
+    assert response_iter_list[2].get_response() == " is"
+    assert response_iter_list[3].get_response() == " a"
+    assert response_iter_list[4].get_response() == " bug"
```

### Comparing `manifest-ml-0.1.7/tests/test_scheduler.py` & `manifest-ml-0.1.8/tests/test_scheduler.py`

 * *Files identical despite different names*

### Comparing `manifest-ml-0.1.7/tests/test_serializer.py` & `manifest-ml-0.1.8/tests/test_serializer.py`

 * *Files identical despite different names*

### Comparing `manifest-ml-0.1.7/web_app/main.py` & `manifest-ml-0.1.8/web_app/main.py`

 * *Files identical despite different names*

### Comparing `manifest-ml-0.1.7/web_app/schemas.py` & `manifest-ml-0.1.8/web_app/schemas.py`

 * *Files identical despite different names*

