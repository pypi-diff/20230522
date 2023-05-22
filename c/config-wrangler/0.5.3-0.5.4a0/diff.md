# Comparing `tmp/config_wrangler-0.5.3.tar.gz` & `tmp/config_wrangler-0.5.4a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "config_wrangler-0.5.3.tar", max compression
+gzip compressed data, was "config_wrangler-0.5.4a0.tar", max compression
```

## Comparing `config_wrangler-0.5.3.tar` & `config_wrangler-0.5.4a0.tar`

### file list

```diff
@@ -1,75 +1,74 @@
--rw-r--r--   0        0        0        0 2022-04-04 16:58:45.000000 config_wrangler-0.5.3/config_wrangler/__init__.py
--rw-r--r--   0        0        0       61 2021-10-15 15:29:20.000000 config_wrangler-0.5.3/config_wrangler/config_data_loaders/__init__.py
--rw-r--r--   0        0        0      302 2023-01-19 18:10:28.528146 config_wrangler-0.5.3/config_wrangler/config_data_loaders/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      372 2023-01-19 18:40:29.151992 config_wrangler-0.5.3/config_wrangler/config_data_loaders/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     1481 2023-01-19 18:10:28.709147 config_wrangler-0.5.3/config_wrangler/config_data_loaders/__pycache__/base_config_data_loader.cpython-310.pyc
--rw-r--r--   0        0        0     2279 2023-01-19 18:40:29.302749 config_wrangler-0.5.3/config_wrangler/config_data_loaders/__pycache__/base_config_data_loader.cpython-311.pyc
--rw-r--r--   0        0        0     2610 2023-01-19 18:10:28.537147 config_wrangler-0.5.3/config_wrangler/config_data_loaders/__pycache__/env_config_data_loader.cpython-310.pyc
--rw-r--r--   0        0        0     4364 2023-01-19 18:40:29.157963 config_wrangler-0.5.3/config_wrangler/config_data_loaders/__pycache__/env_config_data_loader.cpython-311.pyc
--rw-r--r--   0        0        0     3154 2023-01-19 18:10:28.767146 config_wrangler-0.5.3/config_wrangler/config_data_loaders/__pycache__/file_config_data_loader.cpython-310.pyc
--rw-r--r--   0        0        0     5475 2023-01-19 18:40:29.370771 config_wrangler-0.5.3/config_wrangler/config_data_loaders/__pycache__/file_config_data_loader.cpython-311.pyc
--rw-r--r--   0        0        0     5224 2023-01-19 18:10:28.758164 config_wrangler-0.5.3/config_wrangler/config_data_loaders/__pycache__/ini_config_data_loader.cpython-310.pyc
--rw-r--r--   0        0        0    10394 2023-01-19 18:40:29.358749 config_wrangler-0.5.3/config_wrangler/config_data_loaders/__pycache__/ini_config_data_loader.cpython-311.pyc
--rw-r--r--   0        0        0     1058 2022-10-04 13:22:12.000000 config_wrangler-0.5.3/config_wrangler/config_data_loaders/base_config_data_loader.py
--rw-r--r--   0        0        0     3546 2022-10-04 13:22:12.000000 config_wrangler-0.5.3/config_wrangler/config_data_loaders/env_config_data_loader.py
--rw-r--r--   0        0        0     3894 2022-10-04 13:22:12.000000 config_wrangler-0.5.3/config_wrangler/config_data_loaders/file_config_data_loader.py
--rw-r--r--   0        0        0     7018 2022-10-04 13:22:12.000000 config_wrangler-0.5.3/config_wrangler/config_data_loaders/ini_config_data_loader.py
--rw-r--r--   0        0        0     5064 2022-10-04 13:22:12.000000 config_wrangler-0.5.3/config_wrangler/config_data_loaders/toml_config_data_loader.py
--rw-r--r--   0        0        0       40 2021-10-15 15:29:20.000000 config_wrangler-0.5.3/config_wrangler/config_exception.py
--rw-r--r--   0        0        0      763 2022-10-04 13:22:12.000000 config_wrangler-0.5.3/config_wrangler/config_from_ini.py
--rw-r--r--   0        0        0      952 2022-10-04 13:22:12.000000 config_wrangler-0.5.3/config_wrangler/config_from_ini_env.py
--rw-r--r--   0        0        0     2119 2022-06-17 21:01:06.000000 config_wrangler-0.5.3/config_wrangler/config_from_loaders.py
--rw-r--r--   0        0        0     4324 2023-01-19 18:17:35.428775 config_wrangler-0.5.3/config_wrangler/config_root.py
--rw-r--r--   0        0        0        0 2022-08-11 15:33:26.000000 config_wrangler-0.5.3/config_wrangler/config_templates/__init__.py
--rw-r--r--   0        0        0      161 2023-01-19 18:10:28.741146 config_wrangler-0.5.3/config_wrangler/config_templates/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      177 2023-01-19 18:40:29.340750 config_wrangler-0.5.3/config_wrangler/config_templates/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     8028 2023-01-19 18:10:28.749146 config_wrangler-0.5.3/config_wrangler/config_templates/__pycache__/config_hierarchy.cpython-310.pyc
--rw-r--r--   0        0        0    11768 2023-01-19 18:40:29.347749 config_wrangler-0.5.3/config_wrangler/config_templates/__pycache__/config_hierarchy.cpython-311.pyc
--rw-r--r--   0        0        0     7151 2023-01-20 17:31:46.043198 config_wrangler-0.5.3/config_wrangler/config_templates/__pycache__/credentials.cpython-310.pyc
--rw-r--r--   0        0        0    12121 2023-01-20 17:25:24.935289 config_wrangler-0.5.3/config_wrangler/config_templates/__pycache__/credentials.cpython-311.pyc
--rw-r--r--   0        0        0     3685 2023-01-20 17:31:46.055202 config_wrangler-0.5.3/config_wrangler/config_templates/__pycache__/keepass_config.cpython-310.pyc
--rw-r--r--   0        0        0     6724 2023-01-19 22:24:32.125487 config_wrangler-0.5.3/config_wrangler/config_templates/__pycache__/keepass_config.cpython-311.pyc
--rw-r--r--   0        0        0     6988 2023-01-20 17:31:46.662180 config_wrangler-0.5.3/config_wrangler/config_templates/__pycache__/logging_config.cpython-310.pyc
--rw-r--r--   0        0        0    14658 2023-03-16 14:56:27.659745 config_wrangler-0.5.3/config_wrangler/config_templates/__pycache__/logging_config.cpython-311.pyc
--rw-r--r--   0        0        0      993 2023-01-20 17:31:46.506204 config_wrangler-0.5.3/config_wrangler/config_templates/__pycache__/password_defaults.cpython-310.pyc
--rw-r--r--   0        0        0     1336 2023-01-20 17:21:34.973531 config_wrangler-0.5.3/config_wrangler/config_templates/__pycache__/password_defaults.cpython-311.pyc
--rw-r--r--   0        0        0      463 2023-01-20 17:31:46.066200 config_wrangler-0.5.3/config_wrangler/config_templates/__pycache__/password_source.cpython-310.pyc
--rw-r--r--   0        0        0      649 2023-01-19 22:24:32.131486 config_wrangler-0.5.3/config_wrangler/config_templates/__pycache__/password_source.cpython-311.pyc
--rw-r--r--   0        0        0     7082 2023-01-19 18:10:29.377731 config_wrangler-0.5.3/config_wrangler/config_templates/__pycache__/sqlalchemy_database.cpython-310.pyc
--rw-r--r--   0        0        0    12245 2023-01-19 18:40:29.833455 config_wrangler-0.5.3/config_wrangler/config_templates/__pycache__/sqlalchemy_database.cpython-311.pyc
--rw-r--r--   0        0        0        0 2022-08-11 13:26:46.000000 config_wrangler-0.5.3/config_wrangler/config_templates/aws/__init__.py
--rw-r--r--   0        0        0      165 2023-01-19 18:12:31.247280 config_wrangler-0.5.3/config_wrangler/config_templates/aws/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      181 2023-01-19 18:40:30.694299 config_wrangler-0.5.3/config_wrangler/config_templates/aws/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     3596 2023-03-02 17:17:56.052265 config_wrangler-0.5.3/config_wrangler/config_templates/aws/__pycache__/aws_session.cpython-310.pyc
--rw-r--r--   0        0        0     5908 2023-03-15 17:13:27.230489 config_wrangler-0.5.3/config_wrangler/config_templates/aws/__pycache__/aws_session.cpython-311.pyc
--rw-r--r--   0        0        0    14179 2023-01-19 18:12:31.260286 config_wrangler-0.5.3/config_wrangler/config_templates/aws/__pycache__/s3_bucket.cpython-310.pyc
--rw-r--r--   0        0        0    24274 2023-01-19 18:40:30.705300 config_wrangler-0.5.3/config_wrangler/config_templates/aws/__pycache__/s3_bucket.cpython-311.pyc
--rw-r--r--   0        0        0     3568 2023-02-16 16:55:47.006011 config_wrangler-0.5.3/config_wrangler/config_templates/aws/aws_session.py
--rw-r--r--   0        0        0     5311 2023-02-16 17:45:03.096268 config_wrangler-0.5.3/config_wrangler/config_templates/aws/dynamodb.py
--rw-r--r--   0        0        0    14733 2022-10-04 13:22:13.000000 config_wrangler-0.5.3/config_wrangler/config_templates/aws/s3_bucket.py
--rw-r--r--   0        0        0     8553 2022-10-04 13:22:12.000000 config_wrangler-0.5.3/config_wrangler/config_templates/config_hierarchy.py
--rw-r--r--   0        0        0    11433 2023-01-20 17:25:24.488708 config_wrangler-0.5.3/config_wrangler/config_templates/credentials.py
--rw-r--r--   0        0        0     5027 2023-01-19 22:24:31.736478 config_wrangler-0.5.3/config_wrangler/config_templates/keepass_config.py
--rw-r--r--   0        0        0    13868 2023-03-16 14:56:25.692059 config_wrangler-0.5.3/config_wrangler/config_templates/logging_config.py
--rw-r--r--   0        0        0     1110 2023-01-20 17:09:25.490777 config_wrangler-0.5.3/config_wrangler/config_templates/password_defaults.py
--rw-r--r--   0        0        0      158 2023-01-19 22:23:52.308314 config_wrangler-0.5.3/config_wrangler/config_templates/password_source.py
--rw-r--r--   0        0        0    10163 2022-06-07 18:18:22.000000 config_wrangler-0.5.3/config_wrangler/config_templates/sqlalchemy_database.py
--rw-r--r--   0        0        0        0 2022-02-14 17:48:00.000000 config_wrangler-0.5.3/config_wrangler/config_types/__init__.py
--rw-r--r--   0        0        0      157 2023-01-19 18:10:28.731147 config_wrangler-0.5.3/config_wrangler/config_types/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      173 2023-01-19 18:40:29.328750 config_wrangler-0.5.3/config_wrangler/config_types/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     2020 2023-01-20 17:31:46.519194 config_wrangler-0.5.3/config_wrangler/config_types/__pycache__/dynamically_referenced.cpython-310.pyc
--rw-r--r--   0        0        0     2966 2023-01-19 22:18:20.497962 config_wrangler-0.5.3/config_wrangler/config_types/__pycache__/dynamically_referenced.cpython-311.pyc
--rw-r--r--   0        0        0      354 2023-01-20 17:31:46.672182 config_wrangler-0.5.3/config_wrangler/config_types/__pycache__/enum.cpython-310.pyc
--rw-r--r--   0        0        0      453 2023-03-16 13:23:06.383418 config_wrangler-0.5.3/config_wrangler/config_types/__pycache__/enum.cpython-311.pyc
--rw-r--r--   0        0        0     4217 2023-01-19 18:10:28.913147 config_wrangler-0.5.3/config_wrangler/config_types/__pycache__/path_types.cpython-310.pyc
--rw-r--r--   0        0        0     7374 2023-01-19 18:40:29.441803 config_wrangler-0.5.3/config_wrangler/config_types/__pycache__/path_types.cpython-311.pyc
--rw-r--r--   0        0        0     1600 2023-01-19 22:18:19.854961 config_wrangler-0.5.3/config_wrangler/config_types/dynamically_referenced.py
--rw-r--r--   0        0        0      255 2022-04-27 17:59:32.000000 config_wrangler-0.5.3/config_wrangler/config_types/enum.py
--rw-r--r--   0        0        0     3045 2022-06-02 20:11:39.000000 config_wrangler-0.5.3/config_wrangler/config_types/path_types.py
--rw-r--r--   0        0        0    17593 2023-03-02 17:43:02.517669 config_wrangler-0.5.3/config_wrangler/utils.py
--rw-r--r--   0        0        0     1067 2021-10-15 15:29:20.000000 config_wrangler-0.5.3/LICENSE
--rw-r--r--   0        0        0     1066 2021-10-15 15:29:20.000000 config_wrangler-0.5.3/LICENSE.txt
--rw-r--r--   0        0        0     1283 2023-03-16 14:58:08.013429 config_wrangler-0.5.3/pyproject.toml
--rw-r--r--   0        0        0     6157 2022-10-04 13:22:12.000000 config_wrangler-0.5.3/README.md
--rw-r--r--   0        0        0     7596 1970-01-01 00:00:00.000000 config_wrangler-0.5.3/setup.py
--rw-r--r--   0        0        0     7367 1970-01-01 00:00:00.000000 config_wrangler-0.5.3/PKG-INFO
+-rw-r--r--   0        0        0        0 2022-04-04 16:58:45.000000 config_wrangler-0.5.4a0/config_wrangler/__init__.py
+-rw-r--r--   0        0        0       61 2021-10-15 15:29:20.000000 config_wrangler-0.5.4a0/config_wrangler/config_data_loaders/__init__.py
+-rw-r--r--   0        0        0      302 2023-01-19 18:10:28.528146 config_wrangler-0.5.4a0/config_wrangler/config_data_loaders/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      372 2023-01-19 18:40:29.151992 config_wrangler-0.5.4a0/config_wrangler/config_data_loaders/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     1481 2023-01-19 18:10:28.709147 config_wrangler-0.5.4a0/config_wrangler/config_data_loaders/__pycache__/base_config_data_loader.cpython-310.pyc
+-rw-r--r--   0        0        0     2279 2023-01-19 18:40:29.302749 config_wrangler-0.5.4a0/config_wrangler/config_data_loaders/__pycache__/base_config_data_loader.cpython-311.pyc
+-rw-r--r--   0        0        0     2610 2023-01-19 18:10:28.537147 config_wrangler-0.5.4a0/config_wrangler/config_data_loaders/__pycache__/env_config_data_loader.cpython-310.pyc
+-rw-r--r--   0        0        0     4364 2023-01-19 18:40:29.157963 config_wrangler-0.5.4a0/config_wrangler/config_data_loaders/__pycache__/env_config_data_loader.cpython-311.pyc
+-rw-r--r--   0        0        0     3154 2023-01-19 18:10:28.767146 config_wrangler-0.5.4a0/config_wrangler/config_data_loaders/__pycache__/file_config_data_loader.cpython-310.pyc
+-rw-r--r--   0        0        0     5475 2023-01-19 18:40:29.370771 config_wrangler-0.5.4a0/config_wrangler/config_data_loaders/__pycache__/file_config_data_loader.cpython-311.pyc
+-rw-r--r--   0        0        0     5224 2023-01-19 18:10:28.758164 config_wrangler-0.5.4a0/config_wrangler/config_data_loaders/__pycache__/ini_config_data_loader.cpython-310.pyc
+-rw-r--r--   0        0        0    10394 2023-01-19 18:40:29.358749 config_wrangler-0.5.4a0/config_wrangler/config_data_loaders/__pycache__/ini_config_data_loader.cpython-311.pyc
+-rw-r--r--   0        0        0     1058 2022-10-04 13:22:12.000000 config_wrangler-0.5.4a0/config_wrangler/config_data_loaders/base_config_data_loader.py
+-rw-r--r--   0        0        0     3546 2022-10-04 13:22:12.000000 config_wrangler-0.5.4a0/config_wrangler/config_data_loaders/env_config_data_loader.py
+-rw-r--r--   0        0        0     3894 2022-10-04 13:22:12.000000 config_wrangler-0.5.4a0/config_wrangler/config_data_loaders/file_config_data_loader.py
+-rw-r--r--   0        0        0     7018 2022-10-04 13:22:12.000000 config_wrangler-0.5.4a0/config_wrangler/config_data_loaders/ini_config_data_loader.py
+-rw-r--r--   0        0        0     5064 2022-10-04 13:22:12.000000 config_wrangler-0.5.4a0/config_wrangler/config_data_loaders/toml_config_data_loader.py
+-rw-r--r--   0        0        0       40 2021-10-15 15:29:20.000000 config_wrangler-0.5.4a0/config_wrangler/config_exception.py
+-rw-r--r--   0        0        0      763 2022-10-04 13:22:12.000000 config_wrangler-0.5.4a0/config_wrangler/config_from_ini.py
+-rw-r--r--   0        0        0      952 2022-10-04 13:22:12.000000 config_wrangler-0.5.4a0/config_wrangler/config_from_ini_env.py
+-rw-r--r--   0        0        0     2119 2022-06-17 21:01:06.000000 config_wrangler-0.5.4a0/config_wrangler/config_from_loaders.py
+-rw-r--r--   0        0        0     4324 2023-01-19 18:17:35.428775 config_wrangler-0.5.4a0/config_wrangler/config_root.py
+-rw-r--r--   0        0        0        0 2022-08-11 15:33:26.000000 config_wrangler-0.5.4a0/config_wrangler/config_templates/__init__.py
+-rw-r--r--   0        0        0      161 2023-01-19 18:10:28.741146 config_wrangler-0.5.4a0/config_wrangler/config_templates/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      177 2023-01-19 18:40:29.340750 config_wrangler-0.5.4a0/config_wrangler/config_templates/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     8028 2023-01-19 18:10:28.749146 config_wrangler-0.5.4a0/config_wrangler/config_templates/__pycache__/config_hierarchy.cpython-310.pyc
+-rw-r--r--   0        0        0    11768 2023-01-19 18:40:29.347749 config_wrangler-0.5.4a0/config_wrangler/config_templates/__pycache__/config_hierarchy.cpython-311.pyc
+-rw-r--r--   0        0        0     7151 2023-01-20 17:31:46.043198 config_wrangler-0.5.4a0/config_wrangler/config_templates/__pycache__/credentials.cpython-310.pyc
+-rw-r--r--   0        0        0    12121 2023-01-20 17:25:24.935289 config_wrangler-0.5.4a0/config_wrangler/config_templates/__pycache__/credentials.cpython-311.pyc
+-rw-r--r--   0        0        0     3685 2023-01-20 17:31:46.055202 config_wrangler-0.5.4a0/config_wrangler/config_templates/__pycache__/keepass_config.cpython-310.pyc
+-rw-r--r--   0        0        0     6724 2023-01-19 22:24:32.125487 config_wrangler-0.5.4a0/config_wrangler/config_templates/__pycache__/keepass_config.cpython-311.pyc
+-rw-r--r--   0        0        0     6988 2023-01-20 17:31:46.662180 config_wrangler-0.5.4a0/config_wrangler/config_templates/__pycache__/logging_config.cpython-310.pyc
+-rw-r--r--   0        0        0    14658 2023-03-16 14:56:27.659745 config_wrangler-0.5.4a0/config_wrangler/config_templates/__pycache__/logging_config.cpython-311.pyc
+-rw-r--r--   0        0        0      993 2023-01-20 17:31:46.506204 config_wrangler-0.5.4a0/config_wrangler/config_templates/__pycache__/password_defaults.cpython-310.pyc
+-rw-r--r--   0        0        0     1336 2023-01-20 17:21:34.973531 config_wrangler-0.5.4a0/config_wrangler/config_templates/__pycache__/password_defaults.cpython-311.pyc
+-rw-r--r--   0        0        0      463 2023-01-20 17:31:46.066200 config_wrangler-0.5.4a0/config_wrangler/config_templates/__pycache__/password_source.cpython-310.pyc
+-rw-r--r--   0        0        0      649 2023-01-19 22:24:32.131486 config_wrangler-0.5.4a0/config_wrangler/config_templates/__pycache__/password_source.cpython-311.pyc
+-rw-r--r--   0        0        0     7082 2023-01-19 18:10:29.377731 config_wrangler-0.5.4a0/config_wrangler/config_templates/__pycache__/sqlalchemy_database.cpython-310.pyc
+-rw-r--r--   0        0        0    12245 2023-01-19 18:40:29.833455 config_wrangler-0.5.4a0/config_wrangler/config_templates/__pycache__/sqlalchemy_database.cpython-311.pyc
+-rw-r--r--   0        0        0        0 2022-08-11 13:26:46.000000 config_wrangler-0.5.4a0/config_wrangler/config_templates/aws/__init__.py
+-rw-r--r--   0        0        0      165 2023-01-19 18:12:31.247280 config_wrangler-0.5.4a0/config_wrangler/config_templates/aws/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      181 2023-01-19 18:40:30.694299 config_wrangler-0.5.4a0/config_wrangler/config_templates/aws/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     3596 2023-03-02 17:17:56.052265 config_wrangler-0.5.4a0/config_wrangler/config_templates/aws/__pycache__/aws_session.cpython-310.pyc
+-rw-r--r--   0        0        0     5908 2023-03-15 17:13:27.230489 config_wrangler-0.5.4a0/config_wrangler/config_templates/aws/__pycache__/aws_session.cpython-311.pyc
+-rw-r--r--   0        0        0    14179 2023-01-19 18:12:31.260286 config_wrangler-0.5.4a0/config_wrangler/config_templates/aws/__pycache__/s3_bucket.cpython-310.pyc
+-rw-r--r--   0        0        0    24274 2023-01-19 18:40:30.705300 config_wrangler-0.5.4a0/config_wrangler/config_templates/aws/__pycache__/s3_bucket.cpython-311.pyc
+-rw-r--r--   0        0        0     3568 2023-02-16 16:55:47.006011 config_wrangler-0.5.4a0/config_wrangler/config_templates/aws/aws_session.py
+-rw-r--r--   0        0        0     5311 2023-02-16 17:45:03.096268 config_wrangler-0.5.4a0/config_wrangler/config_templates/aws/dynamodb.py
+-rw-r--r--   0        0        0    14856 2023-05-22 18:55:50.987295 config_wrangler-0.5.4a0/config_wrangler/config_templates/aws/s3_bucket.py
+-rw-r--r--   0        0        0     8553 2022-10-04 13:22:12.000000 config_wrangler-0.5.4a0/config_wrangler/config_templates/config_hierarchy.py
+-rw-r--r--   0        0        0    11433 2023-01-20 17:25:24.488708 config_wrangler-0.5.4a0/config_wrangler/config_templates/credentials.py
+-rw-r--r--   0        0        0     5027 2023-01-19 22:24:31.736478 config_wrangler-0.5.4a0/config_wrangler/config_templates/keepass_config.py
+-rw-r--r--   0        0        0    14413 2023-05-03 21:30:39.090898 config_wrangler-0.5.4a0/config_wrangler/config_templates/logging_config.py
+-rw-r--r--   0        0        0     1110 2023-01-20 17:09:25.490777 config_wrangler-0.5.4a0/config_wrangler/config_templates/password_defaults.py
+-rw-r--r--   0        0        0      158 2023-01-19 22:23:52.308314 config_wrangler-0.5.4a0/config_wrangler/config_templates/password_source.py
+-rw-r--r--   0        0        0    10163 2022-06-07 18:18:22.000000 config_wrangler-0.5.4a0/config_wrangler/config_templates/sqlalchemy_database.py
+-rw-r--r--   0        0        0        0 2022-02-14 17:48:00.000000 config_wrangler-0.5.4a0/config_wrangler/config_types/__init__.py
+-rw-r--r--   0        0        0      157 2023-01-19 18:10:28.731147 config_wrangler-0.5.4a0/config_wrangler/config_types/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      173 2023-01-19 18:40:29.328750 config_wrangler-0.5.4a0/config_wrangler/config_types/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     2020 2023-01-20 17:31:46.519194 config_wrangler-0.5.4a0/config_wrangler/config_types/__pycache__/dynamically_referenced.cpython-310.pyc
+-rw-r--r--   0        0        0     2966 2023-01-19 22:18:20.497962 config_wrangler-0.5.4a0/config_wrangler/config_types/__pycache__/dynamically_referenced.cpython-311.pyc
+-rw-r--r--   0        0        0      354 2023-01-20 17:31:46.672182 config_wrangler-0.5.4a0/config_wrangler/config_types/__pycache__/enum.cpython-310.pyc
+-rw-r--r--   0        0        0      453 2023-03-16 13:23:06.383418 config_wrangler-0.5.4a0/config_wrangler/config_types/__pycache__/enum.cpython-311.pyc
+-rw-r--r--   0        0        0     4217 2023-01-19 18:10:28.913147 config_wrangler-0.5.4a0/config_wrangler/config_types/__pycache__/path_types.cpython-310.pyc
+-rw-r--r--   0        0        0     7374 2023-01-19 18:40:29.441803 config_wrangler-0.5.4a0/config_wrangler/config_types/__pycache__/path_types.cpython-311.pyc
+-rw-r--r--   0        0        0     1600 2023-01-19 22:18:19.854961 config_wrangler-0.5.4a0/config_wrangler/config_types/dynamically_referenced.py
+-rw-r--r--   0        0        0      255 2022-04-27 17:59:32.000000 config_wrangler-0.5.4a0/config_wrangler/config_types/enum.py
+-rw-r--r--   0        0        0     3045 2022-06-02 20:11:39.000000 config_wrangler-0.5.4a0/config_wrangler/config_types/path_types.py
+-rw-r--r--   0        0        0    17593 2023-03-02 17:43:02.517669 config_wrangler-0.5.4a0/config_wrangler/utils.py
+-rw-r--r--   0        0        0     1067 2021-10-15 15:29:20.000000 config_wrangler-0.5.4a0/LICENSE
+-rw-r--r--   0        0        0     1066 2021-10-15 15:29:20.000000 config_wrangler-0.5.4a0/LICENSE.txt
+-rw-r--r--   0        0        0     1284 2023-05-22 19:01:32.782536 config_wrangler-0.5.4a0/pyproject.toml
+-rw-r--r--   0        0        0     6157 2022-10-04 13:22:12.000000 config_wrangler-0.5.4a0/README.md
+-rw-r--r--   0        0        0     7369 1970-01-01 00:00:00.000000 config_wrangler-0.5.4a0/PKG-INFO
```

### Comparing `config_wrangler-0.5.3/config_wrangler/config_data_loaders/__pycache__/base_config_data_loader.cpython-310.pyc` & `config_wrangler-0.5.4a0/config_wrangler/config_data_loaders/__pycache__/base_config_data_loader.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `config_wrangler-0.5.3/config_wrangler/config_data_loaders/__pycache__/base_config_data_loader.cpython-311.pyc` & `config_wrangler-0.5.4a0/config_wrangler/config_data_loaders/__pycache__/base_config_data_loader.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `config_wrangler-0.5.3/config_wrangler/config_data_loaders/__pycache__/env_config_data_loader.cpython-310.pyc` & `config_wrangler-0.5.4a0/config_wrangler/config_data_loaders/__pycache__/env_config_data_loader.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `config_wrangler-0.5.3/config_wrangler/config_data_loaders/__pycache__/env_config_data_loader.cpython-311.pyc` & `config_wrangler-0.5.4a0/config_wrangler/config_data_loaders/__pycache__/env_config_data_loader.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `config_wrangler-0.5.3/config_wrangler/config_data_loaders/__pycache__/file_config_data_loader.cpython-310.pyc` & `config_wrangler-0.5.4a0/config_wrangler/config_data_loaders/__pycache__/file_config_data_loader.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `config_wrangler-0.5.3/config_wrangler/config_data_loaders/__pycache__/file_config_data_loader.cpython-311.pyc` & `config_wrangler-0.5.4a0/config_wrangler/config_data_loaders/__pycache__/file_config_data_loader.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `config_wrangler-0.5.3/config_wrangler/config_data_loaders/__pycache__/ini_config_data_loader.cpython-310.pyc` & `config_wrangler-0.5.4a0/config_wrangler/config_data_loaders/__pycache__/ini_config_data_loader.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `config_wrangler-0.5.3/config_wrangler/config_data_loaders/__pycache__/ini_config_data_loader.cpython-311.pyc` & `config_wrangler-0.5.4a0/config_wrangler/config_data_loaders/__pycache__/ini_config_data_loader.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `config_wrangler-0.5.3/config_wrangler/config_data_loaders/base_config_data_loader.py` & `config_wrangler-0.5.4a0/config_wrangler/config_data_loaders/base_config_data_loader.py`

 * *Files identical despite different names*

### Comparing `config_wrangler-0.5.3/config_wrangler/config_data_loaders/env_config_data_loader.py` & `config_wrangler-0.5.4a0/config_wrangler/config_data_loaders/env_config_data_loader.py`

 * *Files identical despite different names*

### Comparing `config_wrangler-0.5.3/config_wrangler/config_data_loaders/file_config_data_loader.py` & `config_wrangler-0.5.4a0/config_wrangler/config_data_loaders/file_config_data_loader.py`

 * *Files identical despite different names*

### Comparing `config_wrangler-0.5.3/config_wrangler/config_data_loaders/ini_config_data_loader.py` & `config_wrangler-0.5.4a0/config_wrangler/config_data_loaders/ini_config_data_loader.py`

 * *Files identical despite different names*

### Comparing `config_wrangler-0.5.3/config_wrangler/config_data_loaders/toml_config_data_loader.py` & `config_wrangler-0.5.4a0/config_wrangler/config_data_loaders/toml_config_data_loader.py`

 * *Files identical despite different names*

### Comparing `config_wrangler-0.5.3/config_wrangler/config_from_ini.py` & `config_wrangler-0.5.4a0/config_wrangler/config_from_ini.py`

 * *Files identical despite different names*

### Comparing `config_wrangler-0.5.3/config_wrangler/config_from_ini_env.py` & `config_wrangler-0.5.4a0/config_wrangler/config_from_ini_env.py`

 * *Files identical despite different names*

### Comparing `config_wrangler-0.5.3/config_wrangler/config_from_loaders.py` & `config_wrangler-0.5.4a0/config_wrangler/config_from_loaders.py`

 * *Files identical despite different names*

### Comparing `config_wrangler-0.5.3/config_wrangler/config_root.py` & `config_wrangler-0.5.4a0/config_wrangler/config_root.py`

 * *Files identical despite different names*

### Comparing `config_wrangler-0.5.3/config_wrangler/config_templates/__pycache__/config_hierarchy.cpython-310.pyc` & `config_wrangler-0.5.4a0/config_wrangler/config_templates/__pycache__/config_hierarchy.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `config_wrangler-0.5.3/config_wrangler/config_templates/__pycache__/config_hierarchy.cpython-311.pyc` & `config_wrangler-0.5.4a0/config_wrangler/config_templates/__pycache__/config_hierarchy.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `config_wrangler-0.5.3/config_wrangler/config_templates/__pycache__/credentials.cpython-310.pyc` & `config_wrangler-0.5.4a0/config_wrangler/config_templates/__pycache__/credentials.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `config_wrangler-0.5.3/config_wrangler/config_templates/__pycache__/credentials.cpython-311.pyc` & `config_wrangler-0.5.4a0/config_wrangler/config_templates/__pycache__/credentials.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `config_wrangler-0.5.3/config_wrangler/config_templates/__pycache__/keepass_config.cpython-310.pyc` & `config_wrangler-0.5.4a0/config_wrangler/config_templates/__pycache__/keepass_config.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `config_wrangler-0.5.3/config_wrangler/config_templates/__pycache__/keepass_config.cpython-311.pyc` & `config_wrangler-0.5.4a0/config_wrangler/config_templates/__pycache__/keepass_config.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `config_wrangler-0.5.3/config_wrangler/config_templates/__pycache__/logging_config.cpython-310.pyc` & `config_wrangler-0.5.4a0/config_wrangler/config_templates/__pycache__/logging_config.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `config_wrangler-0.5.3/config_wrangler/config_templates/__pycache__/logging_config.cpython-311.pyc` & `config_wrangler-0.5.4a0/config_wrangler/config_templates/__pycache__/logging_config.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `config_wrangler-0.5.3/config_wrangler/config_templates/__pycache__/password_defaults.cpython-310.pyc` & `config_wrangler-0.5.4a0/config_wrangler/config_templates/__pycache__/password_defaults.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `config_wrangler-0.5.3/config_wrangler/config_templates/__pycache__/password_defaults.cpython-311.pyc` & `config_wrangler-0.5.4a0/config_wrangler/config_templates/__pycache__/password_defaults.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `config_wrangler-0.5.3/config_wrangler/config_templates/__pycache__/password_source.cpython-311.pyc` & `config_wrangler-0.5.4a0/config_wrangler/config_templates/__pycache__/password_source.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `config_wrangler-0.5.3/config_wrangler/config_templates/__pycache__/sqlalchemy_database.cpython-310.pyc` & `config_wrangler-0.5.4a0/config_wrangler/config_templates/__pycache__/sqlalchemy_database.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `config_wrangler-0.5.3/config_wrangler/config_templates/__pycache__/sqlalchemy_database.cpython-311.pyc` & `config_wrangler-0.5.4a0/config_wrangler/config_templates/__pycache__/sqlalchemy_database.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `config_wrangler-0.5.3/config_wrangler/config_templates/aws/__pycache__/aws_session.cpython-310.pyc` & `config_wrangler-0.5.4a0/config_wrangler/config_templates/aws/__pycache__/aws_session.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `config_wrangler-0.5.3/config_wrangler/config_templates/aws/__pycache__/aws_session.cpython-311.pyc` & `config_wrangler-0.5.4a0/config_wrangler/config_templates/aws/__pycache__/aws_session.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `config_wrangler-0.5.3/config_wrangler/config_templates/aws/__pycache__/s3_bucket.cpython-310.pyc` & `config_wrangler-0.5.4a0/config_wrangler/config_templates/aws/__pycache__/s3_bucket.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `config_wrangler-0.5.3/config_wrangler/config_templates/aws/__pycache__/s3_bucket.cpython-311.pyc` & `config_wrangler-0.5.4a0/config_wrangler/config_templates/aws/__pycache__/s3_bucket.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `config_wrangler-0.5.3/config_wrangler/config_templates/aws/aws_session.py` & `config_wrangler-0.5.4a0/config_wrangler/config_templates/aws/aws_session.py`

 * *Files identical despite different names*

### Comparing `config_wrangler-0.5.3/config_wrangler/config_templates/aws/dynamodb.py` & `config_wrangler-0.5.4a0/config_wrangler/config_templates/aws/dynamodb.py`

 * *Files identical despite different names*

### Comparing `config_wrangler-0.5.3/config_wrangler/config_templates/aws/s3_bucket.py` & `config_wrangler-0.5.4a0/config_wrangler/config_templates/aws/s3_bucket.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,14 +61,17 @@
     def upload_file(
             self,
             local_filename: Union[str, Path],
             key: Union[str, PurePosixPath],
             extra_args: Optional[dict] = None,
             transfer_config: Optional[TransferConfig] = None,
     ):
+        if transfer_config is None:
+            transfer_config = TransferConfig(multipart_threshold=5* (1024**3)) # 5 GB
+
         self.client.upload_file(
             Filename=str(local_filename),
             Bucket=self.bucket_name,
             Key=str(key),
             ExtraArgs=extra_args,
             Config=transfer_config,
         )
```

### Comparing `config_wrangler-0.5.3/config_wrangler/config_templates/config_hierarchy.py` & `config_wrangler-0.5.4a0/config_wrangler/config_templates/config_hierarchy.py`

 * *Files identical despite different names*

### Comparing `config_wrangler-0.5.3/config_wrangler/config_templates/credentials.py` & `config_wrangler-0.5.4a0/config_wrangler/config_templates/credentials.py`

 * *Files identical despite different names*

### Comparing `config_wrangler-0.5.3/config_wrangler/config_templates/keepass_config.py` & `config_wrangler-0.5.4a0/config_wrangler/config_templates/keepass_config.py`

 * *Files identical despite different names*

### Comparing `config_wrangler-0.5.3/config_wrangler/config_templates/logging_config.py` & `config_wrangler-0.5.4a0/config_wrangler/config_templates/logging_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 
 
 class LoggingConfig(ConfigHierarchy):
     console_log_level: LogLevel = LogLevel.INFO
     console_entry_format: str = '%(asctime)s - %(levelname)-8s - %(name)s: %(message)s'
     log_folder: AutoCreateDirectoryPath = None
     log_file_name: str = None
-    add_date_to_log_file_name: bool = True
+    add_date_to_log_file_name: bool = None
     log_file_name_date_time_format: str = '_%Y_%m_%d_at_%H_%M_%S'
     file_log_level: LogLevel = LogLevel.DEBUG
     log_file_entry_format: str = '%(asctime)s - %(levelname)-8s - %(name)s: %(message)s'
     log_file_rotation_class: FileHandlerClass = FileHandlerClass.RotatingFileHandler
 
     # RotatingFileHandler specific settings
     # https://docs.python.org/3/library/logging.handlers.html#rotatingfilehandler
@@ -107,22 +107,29 @@
             add_date_to_log_file_name = self.add_date_to_log_file_name
         if log_file_prefix is None:
             if self.log_file_name is not None:
                 log_file_name = self.log_file_name
             else:
                 log_file_name = None
         else:
+            log.info(f'Using code provided prefix {log_file_prefix}')
+            if add_date_to_log_file_name is None:
+                if self.log_file_rotation_class == FileHandlerClass.TimedRotatingFileHandler:
+                    add_date_to_log_file_name = False
+                else:
+                    add_date_to_log_file_name = True
+
             if add_date_to_log_file_name:
                 log_file_name = LoggingConfig.get_dated_log_file_name(
                     log_file_prefix=log_file_prefix,
                     date_time_format=self.log_file_name_date_time_format,
                     log_file_suffix=log_file_suffix,
                 )
             else:
-                log_file_name = f"{log_file_prefix}.{log_file_suffix}"
+                log_file_name = f"{log_file_prefix}{log_file_suffix}"
 
         file_handler = None
         if log_file_name is not None:
             if self.log_folder is not None and not Path(log_file_name).is_absolute():
                 log_file_path = Path(self.log_folder, log_file_name)
             else:
                 log_file_path = Path(log_file_name)
@@ -130,14 +137,16 @@
             if self.trace_logging_setup:
                 log.info(f'Logging path = {log_file_path}')
 
             # Setup file logging
 
             # Make sure the directory exists
             dir_name = log_file_path.parent
+            # TODO: We should mkdir on relative paths as well
+            #       Check only that dir_name is not '.'
             if dir_name.is_absolute():
                 dir_name.mkdir(parents=True, exist_ok=True)
 
             if self.log_file_rotation_class == FileHandlerClass.RotatingFileHandler:
                 file_handler = RotatingFileHandler(
                     filename=log_file_path,
                     maxBytes=self.log_file_max_size,
@@ -150,14 +159,15 @@
                     when=self.log_file_timed_rotation_when,
                     interval=self.log_file_timed_rotation_interval,
                     atTime=self.log_file_timed_rotation_attime,
                     utc=self.log_file_timed_rotation_utc,
                     backupCount=self.log_files_to_keep,
                     encoding='utf8',
                 )
+                file_handler.namer = lambda name: name.replace(".log", "") + ".log"
             else:
                 raise ValueError(f"Bad log_file_rotation_class of {self.log_file_rotation_class}")
 
             log_file_entry_formatter = TZFormatter(self.log_file_entry_format, self.logging_date_format)
             file_handler.setFormatter(log_file_entry_formatter)
             file_handler.setLevel(self.file_log_level)
             root_logger.addHandler(file_handler)
```

### Comparing `config_wrangler-0.5.3/config_wrangler/config_templates/password_defaults.py` & `config_wrangler-0.5.4a0/config_wrangler/config_templates/password_defaults.py`

 * *Files identical despite different names*

### Comparing `config_wrangler-0.5.3/config_wrangler/config_templates/sqlalchemy_database.py` & `config_wrangler-0.5.4a0/config_wrangler/config_templates/sqlalchemy_database.py`

 * *Files identical despite different names*

### Comparing `config_wrangler-0.5.3/config_wrangler/config_types/__pycache__/dynamically_referenced.cpython-310.pyc` & `config_wrangler-0.5.4a0/config_wrangler/config_types/__pycache__/dynamically_referenced.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `config_wrangler-0.5.3/config_wrangler/config_types/__pycache__/dynamically_referenced.cpython-311.pyc` & `config_wrangler-0.5.4a0/config_wrangler/config_types/__pycache__/dynamically_referenced.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `config_wrangler-0.5.3/config_wrangler/config_types/__pycache__/path_types.cpython-310.pyc` & `config_wrangler-0.5.4a0/config_wrangler/config_types/__pycache__/path_types.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `config_wrangler-0.5.3/config_wrangler/config_types/__pycache__/path_types.cpython-311.pyc` & `config_wrangler-0.5.4a0/config_wrangler/config_types/__pycache__/path_types.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `config_wrangler-0.5.3/config_wrangler/config_types/dynamically_referenced.py` & `config_wrangler-0.5.4a0/config_wrangler/config_types/dynamically_referenced.py`

 * *Files identical despite different names*

### Comparing `config_wrangler-0.5.3/config_wrangler/config_types/path_types.py` & `config_wrangler-0.5.4a0/config_wrangler/config_types/path_types.py`

 * *Files identical despite different names*

### Comparing `config_wrangler-0.5.3/config_wrangler/utils.py` & `config_wrangler-0.5.4a0/config_wrangler/utils.py`

 * *Files identical despite different names*

### Comparing `config_wrangler-0.5.3/LICENSE` & `config_wrangler-0.5.4a0/LICENSE`

 * *Files identical despite different names*

### Comparing `config_wrangler-0.5.3/LICENSE.txt` & `config_wrangler-0.5.4a0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `config_wrangler-0.5.3/pyproject.toml` & `config_wrangler-0.5.4a0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "config_wrangler"
-version = "0.5.3"
+version = "0.5.4a"
 license = "MIT"
 authors = ["Derek Wood"]
 description = "pydantic based configuration wrangler. Handles reading multiple ini or toml files with inheritance rules and variable expansions."
 readme = "README.md"
 repository = "https://github.com/arcann/config_wrangler"
```

### Comparing `config_wrangler-0.5.3/README.md` & `config_wrangler-0.5.4a0/README.md`

 * *Files identical despite different names*

### Comparing `config_wrangler-0.5.3/PKG-INFO` & `config_wrangler-0.5.4a0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: config-wrangler
-Version: 0.5.3
+Version: 0.5.4a0
 Summary: pydantic based configuration wrangler. Handles reading multiple ini or toml files with inheritance rules and variable expansions.
 Home-page: https://github.com/arcann/config_wrangler
 License: MIT
 Author: Derek Wood
 Requires-Python: >=3.7,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

