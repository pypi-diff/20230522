# Comparing `tmp/dstack-0.8.1.tar.gz` & `tmp/dstack-0.9.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dstack-0.8.1.tar", last modified: Fri May 12 16:49:00 2023, max compression
+gzip compressed data, was "dstack-0.9.post1.tar", last modified: Mon May 22 08:55:00 2023, max compression
```

## Comparing `dstack-0.8.1.tar` & `dstack-0.9.post1.tar`

### file list

```diff
@@ -1,256 +1,273 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:49:00.777871 dstack-0.8.1/
--rw-r--r--   0 runner    (1001) docker     (123)    15976 2023-05-12 16:47:49.000000 dstack-0.8.1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     6417 2023-05-12 16:49:00.777871 dstack-0.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5965 2023-05-12 16:47:49.000000 dstack-0.8.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:49:00.753870 dstack-0.8.1/cli/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:49:00.757870 dstack-0.8.1/cli/dstack/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:49:00.757870 dstack-0.8.1/cli/dstack/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:49:00.757870 dstack-0.8.1/cli/dstack/api/hub/
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/api/hub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19505 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/api/hub/_api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    11650 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/api/hub/_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/api/hub/_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/api/hub/_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/api/hub/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:49:00.757870 dstack-0.8.1/cli/dstack/api/internal/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/api/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/api/internal/backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     4225 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/api/repos.py
--rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/api/runs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:49:00.757870 dstack-0.8.1/cli/dstack/backend/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/backend/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:49:00.761870 dstack-0.8.1/cli/dstack/backend/aws/
--rw-r--r--   0 runner    (1001) docker     (123)     9192 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/backend/aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1994 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/backend/aws/compute.py
--rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/backend/aws/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/backend/aws/logs.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/backend/aws/repos.py
--rw-r--r--   0 runner    (1001) docker     (123)    22377 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/backend/aws/runners.py
--rw-r--r--   0 runner    (1001) docker     (123)     5485 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/backend/aws/secrets.py
--rw-r--r--   0 runner    (1001) docker     (123)     3866 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/backend/aws/storage.py
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/backend/aws/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:49:00.761870 dstack-0.8.1/cli/dstack/backend/base/
--rw-r--r--   0 runner    (1001) docker     (123)     5756 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/backend/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4756 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/backend/base/artifacts.py
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/backend/base/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     3720 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/backend/base/compute.py
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/backend/base/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     9539 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/backend/base/jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/backend/base/logs.py
--rw-r--r--   0 runner    (1001) docker     (123)     5192 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/backend/base/repos.py
--rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/backend/base/runners.py
--rw-r--r--   0 runner    (1001) docker     (123)     5970 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/backend/base/runs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/backend/base/secrets.py
--rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/backend/base/storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     7392 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/backend/base/tags.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:49:00.761870 dstack-0.8.1/cli/dstack/backend/gcp/
--rw-r--r--   0 runner    (1001) docker     (123)     8753 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/backend/gcp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    28759 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/backend/gcp/compute.py
--rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/backend/gcp/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2633 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/backend/gcp/logs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4167 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/backend/gcp/secrets.py
--rw-r--r--   0 runner    (1001) docker     (123)     3802 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/backend/gcp/storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/backend/gcp/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:49:00.761870 dstack-0.8.1/cli/dstack/backend/local/
--rw-r--r--   0 runner    (1001) docker     (123)     7654 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/backend/local/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/backend/local/artifacts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/backend/local/compute.py
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/backend/local/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/backend/local/logs.py
--rw-r--r--   0 runner    (1001) docker     (123)     6225 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/backend/local/runners.py
--rw-r--r--   0 runner    (1001) docker     (123)     4107 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/backend/local/secrets.py
--rw-r--r--   0 runner    (1001) docker     (123)     5344 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/backend/local/storage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:49:00.765870 dstack-0.8.1/cli/dstack/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:49:00.765870 dstack-0.8.1/cli/dstack/cli/commands/
--rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/cli/commands/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:49:00.765870 dstack-0.8.1/cli/dstack/cli/commands/config/
--rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/cli/commands/config/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:49:00.765870 dstack-0.8.1/cli/dstack/cli/commands/cp/
--rw-r--r--   0 runner    (1001) docker     (123)     3738 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/cli/commands/cp/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:49:00.765870 dstack-0.8.1/cli/dstack/cli/commands/init/
--rw-r--r--   0 runner    (1001) docker     (123)     3886 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/cli/commands/init/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:49:00.765870 dstack-0.8.1/cli/dstack/cli/commands/logs/
--rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/cli/commands/logs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:49:00.765870 dstack-0.8.1/cli/dstack/cli/commands/ls/
--rw-r--r--   0 runner    (1001) docker     (123)     2374 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/cli/commands/ls/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:49:00.765870 dstack-0.8.1/cli/dstack/cli/commands/prune/
--rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/cli/commands/prune/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:49:00.765870 dstack-0.8.1/cli/dstack/cli/commands/ps/
--rw-r--r--   0 runner    (1001) docker     (123)     2112 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/cli/commands/ps/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:49:00.765870 dstack-0.8.1/cli/dstack/cli/commands/rm/
--rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/cli/commands/rm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:49:00.765870 dstack-0.8.1/cli/dstack/cli/commands/run/
--rw-r--r--   0 runner    (1001) docker     (123)    11351 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/cli/commands/run/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/cli/commands/run/ssh_tunnel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:49:00.765870 dstack-0.8.1/cli/dstack/cli/commands/secrets/
--rw-r--r--   0 runner    (1001) docker     (123)     4710 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/cli/commands/secrets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:49:00.765870 dstack-0.8.1/cli/dstack/cli/commands/start/
--rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/cli/commands/start/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:49:00.765870 dstack-0.8.1/cli/dstack/cli/commands/stop/
--rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/cli/commands/stop/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:49:00.765870 dstack-0.8.1/cli/dstack/cli/commands/tags/
--rw-r--r--   0 runner    (1001) docker     (123)     4672 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/cli/commands/tags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4759 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/cli/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     6023 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/cli/config.py
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/cli/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/cli/handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/cli/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     2609 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/cli/updates.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:49:00.765870 dstack-0.8.1/cli/dstack/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/core/app.py
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/core/artifact.py
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/core/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/core/dependents.py
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/core/error.py
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/core/instance.py
--rw-r--r--   0 runner    (1001) docker     (123)    16854 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/core/job.py
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/core/log_event.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:49:00.769870 dstack-0.8.1/cli/dstack/core/repo/
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/core/repo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/core/repo/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/core/repo/head.py
--rw-r--r--   0 runner    (1001) docker     (123)     4484 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/core/repo/local.py
--rw-r--r--   0 runner    (1001) docker     (123)     6322 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/core/repo/remote.py
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/core/repo/spec.py
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/core/request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/core/run.py
--rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/core/runners.py
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/core/secret.py
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/core/storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/core/tag.py
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/core/userconfig.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:49:00.769870 dstack-0.8.1/cli/dstack/hub/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/hub/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:49:00.769870 dstack-0.8.1/cli/dstack/hub/background/
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/hub/background/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:49:00.769870 dstack-0.8.1/cli/dstack/hub/background/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/hub/background/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/hub/background/tasks/resubmit_jobs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:49:00.769870 dstack-0.8.1/cli/dstack/hub/db/
--rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/hub/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/hub/db/migrate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/hub/db/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     4439 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/hub/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:49:00.769870 dstack-0.8.1/cli/dstack/hub/migration/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/hub/migration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/hub/migration/env.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:49:00.769870 dstack-0.8.1/cli/dstack/hub/migration/versions/
--rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/hub/migration/versions/3b900659c822_.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/hub/migration/versions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:49:00.769870 dstack-0.8.1/cli/dstack/hub/models/
--rw-r--r--   0 runner    (1001) docker     (123)     6051 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/hub/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:49:00.769870 dstack-0.8.1/cli/dstack/hub/repository/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/hub/repository/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9403 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/hub/repository/projects.py
--rw-r--r--   0 runner    (1001) docker     (123)     2359 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/hub/repository/users.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:49:00.773871 dstack-0.8.1/cli/dstack/hub/routers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/hub/routers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/hub/routers/artifacts.py
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/hub/routers/backends.py
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/hub/routers/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/hub/routers/jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/hub/routers/link.py
--rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/hub/routers/logs.py
--rw-r--r--   0 runner    (1001) docker     (123)     5537 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/hub/routers/projects.py
--rw-r--r--   0 runner    (1001) docker     (123)     2477 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/hub/routers/repos.py
--rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/hub/routers/runners.py
--rw-r--r--   0 runner    (1001) docker     (123)     3377 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/hub/routers/runs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/hub/routers/secrets.py
--rw-r--r--   0 runner    (1001) docker     (123)     2890 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/hub/routers/storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     2369 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/hub/routers/tags.py
--rw-r--r--   0 runner    (1001) docker     (123)     3613 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/hub/routers/users.py
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/hub/routers/util.py
--rw-r--r--   0 runner    (1001) docker     (123)      855 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/hub/routers/workflows.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:49:00.773871 dstack-0.8.1/cli/dstack/hub/security/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/hub/security/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2423 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/hub/security/permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/hub/security/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:49:00.773871 dstack-0.8.1/cli/dstack/hub/services/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/hub/services/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:49:00.773871 dstack-0.8.1/cli/dstack/hub/services/backends/
--rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/hub/services/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5120 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/hub/services/backends/aws.py
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/hub/services/backends/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    10263 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/hub/services/backends/gcp.py
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/hub/services/backends/local.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:49:00.773871 dstack-0.8.1/cli/dstack/hub/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/hub/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/hub/utils/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:49:00.773871 dstack-0.8.1/cli/dstack/providers/
--rw-r--r--   0 runner    (1001) docker     (123)    18594 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/providers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:49:00.773871 dstack-0.8.1/cli/dstack/providers/_torchrun/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/providers/_torchrun/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5086 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/providers/_torchrun/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:49:00.773871 dstack-0.8.1/cli/dstack/providers/bash/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/providers/bash/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4000 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/providers/bash/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:49:00.773871 dstack-0.8.1/cli/dstack/providers/code/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/providers/code/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5690 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/providers/code/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:49:00.773871 dstack-0.8.1/cli/dstack/providers/docker/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/providers/docker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3775 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/providers/docker/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:49:00.773871 dstack-0.8.1/cli/dstack/providers/lab/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/providers/lab/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4740 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/providers/lab/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:49:00.773871 dstack-0.8.1/cli/dstack/providers/notebook/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/providers/notebook/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4642 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/providers/notebook/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:49:00.773871 dstack-0.8.1/cli/dstack/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/schemas/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:49:00.777871 dstack-0.8.1/cli/dstack/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4299 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/utils/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1995 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/utils/escape.py
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/utils/hash.py
--rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/utils/interpolator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3537 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/utils/random_names.py
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/utils/ssh.py
--rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/dstack/utils/workflows.py
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-12 16:49:00.000000 dstack-0.8.1/cli/dstack/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:49:00.757870 dstack-0.8.1/cli/dstack.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6417 2023-05-12 16:49:00.000000 dstack-0.8.1/cli/dstack.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6399 2023-05-12 16:49:00.000000 dstack-0.8.1/cli/dstack.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 16:49:00.000000 dstack-0.8.1/cli/dstack.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-12 16:49:00.000000 dstack-0.8.1/cli/dstack.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-05-12 16:49:00.000000 dstack-0.8.1/cli/dstack.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-12 16:49:00.000000 dstack-0.8.1/cli/dstack.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:49:00.777871 dstack-0.8.1/cli/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:49:00.777871 dstack-0.8.1/cli/tests/backend/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/tests/backend/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:49:00.777871 dstack-0.8.1/cli/tests/backend/base/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/tests/backend/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3772 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/tests/backend/base/test_logs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:49:00.777871 dstack-0.8.1/cli/tests/hub/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/tests/hub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/tests/hub/common.py
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/tests/hub/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:49:00.777871 dstack-0.8.1/cli/tests/hub/routers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/tests/hub/routers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/tests/hub/routers/test_jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3993 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/tests/hub/routers/test_projects.py
--rw-r--r--   0 runner    (1001) docker     (123)     2840 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/tests/hub/routers/test_users.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:49:00.777871 dstack-0.8.1/cli/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/tests/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3215 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/tests/integration/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     2626 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/tests/integration/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     6898 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/tests/integration/test_commands.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:49:00.777871 dstack-0.8.1/cli/tests/providers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/tests/providers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:49:00.777871 dstack-0.8.1/cli/tests/providers/docker/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/tests/providers/docker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/tests/providers/docker/test_entrypoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/tests/providers/test_local_path.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:49:00.777871 dstack-0.8.1/cli/tests/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/tests/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/tests/utils/escape.py
--rw-r--r--   0 runner    (1001) docker     (123)     1894 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/tests/utils/test_interpolator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/tests/utils/test_merge_workflow_data.py
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-05-12 16:47:49.000000 dstack-0.8.1/cli/tests/utils/test_tarignore.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 16:49:00.777871 dstack-0.8.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2729 2023-05-12 16:47:49.000000 dstack-0.8.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:55:00.895295 dstack-0.9.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)    15976 2023-05-22 08:54:04.000000 dstack-0.9.post1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6405 2023-05-22 08:55:00.895295 dstack-0.9.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5858 2023-05-22 08:54:04.000000 dstack-0.9.post1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:55:00.875295 dstack-0.9.post1/cli/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:55:00.875295 dstack-0.9.post1/cli/dstack/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:55:00.875295 dstack-0.9.post1/cli/dstack/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:55:00.879295 dstack-0.9.post1/cli/dstack/api/hub/
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/api/hub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19505 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/api/hub/_api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11650 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/api/hub/_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/api/hub/_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2211 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/api/hub/_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/api/hub/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4225 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/api/repos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/api/runs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:55:00.879295 dstack-0.9.post1/cli/dstack/backend/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/backend/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:55:00.879295 dstack-0.9.post1/cli/dstack/backend/aws/
+-rw-r--r--   0 runner    (1001) docker     (123)     9192 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/backend/aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1994 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/backend/aws/compute.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/backend/aws/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/backend/aws/logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/backend/aws/repos.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22378 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/backend/aws/runners.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5485 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/backend/aws/secrets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3821 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/backend/aws/storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/backend/aws/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:55:00.879295 dstack-0.9.post1/cli/dstack/backend/azure/
+-rw-r--r--   0 runner    (1001) docker     (123)     8417 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/backend/azure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14195 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/backend/azure/compute.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/backend/azure/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3953 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/backend/azure/logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2570 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/backend/azure/secrets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4712 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/backend/azure/storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3002 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/backend/azure/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:55:00.879295 dstack-0.9.post1/cli/dstack/backend/base/
+-rw-r--r--   0 runner    (1001) docker     (123)     5756 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/backend/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4756 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/backend/base/artifacts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/backend/base/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3720 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/backend/base/compute.py
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/backend/base/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9539 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/backend/base/jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/backend/base/logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5192 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/backend/base/repos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/backend/base/runners.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5970 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/backend/base/runs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/backend/base/secrets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/backend/base/storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7392 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/backend/base/tags.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:55:00.879295 dstack-0.9.post1/cli/dstack/backend/gcp/
+-rw-r--r--   0 runner    (1001) docker     (123)     8753 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/backend/gcp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28759 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/backend/gcp/compute.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/backend/gcp/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2633 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/backend/gcp/logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4167 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/backend/gcp/secrets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3802 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/backend/gcp/storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/backend/gcp/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:55:00.883295 dstack-0.9.post1/cli/dstack/backend/local/
+-rw-r--r--   0 runner    (1001) docker     (123)     7654 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/backend/local/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/backend/local/artifacts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/backend/local/compute.py
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/backend/local/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/backend/local/logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6225 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/backend/local/runners.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4107 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/backend/local/secrets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5344 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/backend/local/storage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:55:00.883295 dstack-0.9.post1/cli/dstack/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:55:00.883295 dstack-0.9.post1/cli/dstack/cli/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/cli/commands/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:55:00.883295 dstack-0.9.post1/cli/dstack/cli/commands/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/cli/commands/config/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:55:00.883295 dstack-0.9.post1/cli/dstack/cli/commands/cp/
+-rw-r--r--   0 runner    (1001) docker     (123)     3738 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/cli/commands/cp/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:55:00.883295 dstack-0.9.post1/cli/dstack/cli/commands/init/
+-rw-r--r--   0 runner    (1001) docker     (123)     4899 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/cli/commands/init/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:55:00.883295 dstack-0.9.post1/cli/dstack/cli/commands/logs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/cli/commands/logs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:55:00.883295 dstack-0.9.post1/cli/dstack/cli/commands/ls/
+-rw-r--r--   0 runner    (1001) docker     (123)     2374 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/cli/commands/ls/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:55:00.883295 dstack-0.9.post1/cli/dstack/cli/commands/prune/
+-rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/cli/commands/prune/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:55:00.883295 dstack-0.9.post1/cli/dstack/cli/commands/ps/
+-rw-r--r--   0 runner    (1001) docker     (123)     2112 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/cli/commands/ps/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:55:00.883295 dstack-0.9.post1/cli/dstack/cli/commands/resubmit/
+-rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/cli/commands/resubmit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:55:00.883295 dstack-0.9.post1/cli/dstack/cli/commands/rm/
+-rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/cli/commands/rm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:55:00.883295 dstack-0.9.post1/cli/dstack/cli/commands/run/
+-rw-r--r--   0 runner    (1001) docker     (123)    11390 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/cli/commands/run/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/cli/commands/run/ssh_tunnel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:55:00.883295 dstack-0.9.post1/cli/dstack/cli/commands/secrets/
+-rw-r--r--   0 runner    (1001) docker     (123)     4710 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/cli/commands/secrets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:55:00.883295 dstack-0.9.post1/cli/dstack/cli/commands/start/
+-rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/cli/commands/start/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:55:00.883295 dstack-0.9.post1/cli/dstack/cli/commands/stop/
+-rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/cli/commands/stop/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:55:00.883295 dstack-0.9.post1/cli/dstack/cli/commands/tags/
+-rw-r--r--   0 runner    (1001) docker     (123)     4672 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/cli/commands/tags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4759 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/cli/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6140 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/cli/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/cli/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/cli/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/cli/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2609 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/cli/updates.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:55:00.887295 dstack-0.9.post1/cli/dstack/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/core/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/core/artifact.py
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/core/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/core/dependents.py
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/core/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/core/instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16854 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/core/job.py
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/core/log_event.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:55:00.887295 dstack-0.9.post1/cli/dstack/core/repo/
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/core/repo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/core/repo/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/core/repo/head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4484 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/core/repo/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6322 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/core/repo/remote.py
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/core/repo/spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/core/request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/core/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/core/runners.py
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/core/secret.py
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/core/storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/core/tag.py
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/core/userconfig.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:55:00.887295 dstack-0.9.post1/cli/dstack/hub/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/hub/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:55:00.887295 dstack-0.9.post1/cli/dstack/hub/background/
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/hub/background/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:55:00.887295 dstack-0.9.post1/cli/dstack/hub/background/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/hub/background/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/hub/background/tasks/resubmit_jobs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:55:00.887295 dstack-0.9.post1/cli/dstack/hub/db/
+-rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/hub/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/hub/db/migrate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/hub/db/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4439 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/hub/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:55:00.887295 dstack-0.9.post1/cli/dstack/hub/migration/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/hub/migration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/hub/migration/env.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:55:00.887295 dstack-0.9.post1/cli/dstack/hub/migration/versions/
+-rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/hub/migration/versions/3b900659c822_.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/hub/migration/versions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:55:00.887295 dstack-0.9.post1/cli/dstack/hub/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     7094 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/hub/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:55:00.887295 dstack-0.9.post1/cli/dstack/hub/repository/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/hub/repository/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6778 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/hub/repository/projects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2359 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/hub/repository/users.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:55:00.887295 dstack-0.9.post1/cli/dstack/hub/routers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/hub/routers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/hub/routers/artifacts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/hub/routers/backends.py
+-rw-r--r--   0 runner    (1001) docker     (123)      901 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/hub/routers/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/hub/routers/jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/hub/routers/link.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/hub/routers/logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4849 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/hub/routers/projects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2477 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/hub/routers/repos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/hub/routers/runners.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3377 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/hub/routers/runs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/hub/routers/secrets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2890 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/hub/routers/storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2369 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/hub/routers/tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3613 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/hub/routers/users.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/hub/routers/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/hub/routers/workflows.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:55:00.887295 dstack-0.9.post1/cli/dstack/hub/security/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/hub/security/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2423 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/hub/security/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/hub/security/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:55:00.887295 dstack-0.9.post1/cli/dstack/hub/services/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/hub/services/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:55:00.887295 dstack-0.9.post1/cli/dstack/hub/services/backends/
+-rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/hub/services/backends/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:55:00.887295 dstack-0.9.post1/cli/dstack/hub/services/backends/aws/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/hub/services/backends/aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6802 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/hub/services/backends/aws/configurator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:55:00.891295 dstack-0.9.post1/cli/dstack/hub/services/backends/azure/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/hub/services/backends/azure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2421 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/hub/services/backends/azure/azure_identity_credential_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34538 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/hub/services/backends/azure/configurator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/hub/services/backends/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:55:00.891295 dstack-0.9.post1/cli/dstack/hub/services/backends/gcp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/hub/services/backends/gcp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11910 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/hub/services/backends/gcp/configurator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:55:00.891295 dstack-0.9.post1/cli/dstack/hub/services/backends/local/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/hub/services/backends/local/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/hub/services/backends/local/configurator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:55:00.891295 dstack-0.9.post1/cli/dstack/hub/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/hub/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/hub/utils/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:55:00.891295 dstack-0.9.post1/cli/dstack/providers/
+-rw-r--r--   0 runner    (1001) docker     (123)    18660 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/providers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:55:00.891295 dstack-0.9.post1/cli/dstack/providers/_torchrun/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/providers/_torchrun/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5086 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/providers/_torchrun/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:55:00.891295 dstack-0.9.post1/cli/dstack/providers/bash/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/providers/bash/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4000 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/providers/bash/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:55:00.891295 dstack-0.9.post1/cli/dstack/providers/code/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/providers/code/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5729 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/providers/code/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:55:00.891295 dstack-0.9.post1/cli/dstack/providers/docker/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/providers/docker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3775 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/providers/docker/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:55:00.891295 dstack-0.9.post1/cli/dstack/providers/lab/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/providers/lab/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4740 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/providers/lab/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:55:00.891295 dstack-0.9.post1/cli/dstack/providers/notebook/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/providers/notebook/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4642 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/providers/notebook/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:55:00.891295 dstack-0.9.post1/cli/dstack/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/schemas/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:55:00.891295 dstack-0.9.post1/cli/dstack/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4428 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/utils/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1995 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/utils/escape.py
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/utils/hash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/utils/interpolator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3537 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/utils/random_names.py
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/utils/ssh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/dstack/utils/workflows.py
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-22 08:54:59.000000 dstack-0.9.post1/cli/dstack/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:55:00.875295 dstack-0.9.post1/cli/dstack.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6405 2023-05-22 08:55:00.000000 dstack-0.9.post1/cli/dstack.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6990 2023-05-22 08:55:00.000000 dstack-0.9.post1/cli/dstack.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 08:55:00.000000 dstack-0.9.post1/cli/dstack.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-22 08:55:00.000000 dstack-0.9.post1/cli/dstack.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-05-22 08:55:00.000000 dstack-0.9.post1/cli/dstack.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-22 08:55:00.000000 dstack-0.9.post1/cli/dstack.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:55:00.891295 dstack-0.9.post1/cli/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:55:00.891295 dstack-0.9.post1/cli/tests/backend/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/tests/backend/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:55:00.891295 dstack-0.9.post1/cli/tests/backend/base/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/tests/backend/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3772 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/tests/backend/base/test_logs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:55:00.891295 dstack-0.9.post1/cli/tests/hub/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/tests/hub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/tests/hub/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/tests/hub/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:55:00.891295 dstack-0.9.post1/cli/tests/hub/routers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/tests/hub/routers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/tests/hub/routers/test_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3993 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/tests/hub/routers/test_projects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2840 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/tests/hub/routers/test_users.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:55:00.891295 dstack-0.9.post1/cli/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/tests/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3373 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/tests/integration/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/tests/integration/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7213 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/tests/integration/test_commands.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:55:00.891295 dstack-0.9.post1/cli/tests/providers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/tests/providers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:55:00.891295 dstack-0.9.post1/cli/tests/providers/docker/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/tests/providers/docker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/tests/providers/docker/test_entrypoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/tests/providers/test_local_path.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:55:00.895295 dstack-0.9.post1/cli/tests/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/tests/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/tests/utils/escape.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1894 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/tests/utils/test_interpolator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/tests/utils/test_merge_workflow_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-05-22 08:54:04.000000 dstack-0.9.post1/cli/tests/utils/test_tarignore.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 08:55:00.895295 dstack-0.9.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3507 2023-05-22 08:54:04.000000 dstack-0.9.post1/setup.py
```

### Comparing `dstack-0.8.1/LICENSE.md` & `dstack-0.9.post1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `dstack-0.8.1/cli/dstack/api/hub/_api_client.py` & `dstack-0.9.post1/cli/dstack/api/hub/_api_client.py`

 * *Files identical despite different names*

### Comparing `dstack-0.8.1/cli/dstack/api/hub/_client.py` & `dstack-0.9.post1/cli/dstack/api/hub/_client.py`

 * *Files identical despite different names*

### Comparing `dstack-0.8.1/cli/dstack/api/hub/_storage.py` & `dstack-0.9.post1/cli/dstack/api/hub/_storage.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,16 +13,21 @@
     def __init__(self, _client: HubAPIClient):
         self._client = _client
 
     def upload_file(self, source_path: str, dest_path: str, callback: Callable[[int], None]):
         url = self._client.upload_file(dest_path=dest_path)
         if not (url is None):
             with open(source_path, "rb") as f:
+                headers = {}
+                # Azure requires special headers
+                if "blob.core.windows.net" in url:
+                    headers["x-ms-blob-type"] = "BlockBlob"
                 # AWS: requests.put() produces bad headers from empty file descriptor
-                resp = requests.put(url, data=f if os.stat(source_path).st_size > 0 else None)
+                data = f if os.stat(source_path).st_size > 0 else None
+                resp = requests.put(url, data=data, headers=headers)
                 if resp.ok:
                     file_stat = os.stat(source_path)
                     callback(file_stat.st_size)
 
     def download_file(self, source_path: str, dest_path: str, callback: Callable[[int], None]):
         url = self._client.download_file(dest_path=source_path)
         if not (url is None):
```

### Comparing `dstack-0.8.1/cli/dstack/api/repos.py` & `dstack-0.9.post1/cli/dstack/api/repos.py`

 * *Files identical despite different names*

### Comparing `dstack-0.8.1/cli/dstack/api/runs.py` & `dstack-0.9.post1/cli/dstack/api/runs.py`

 * *Files identical despite different names*

### Comparing `dstack-0.8.1/cli/dstack/backend/aws/__init__.py` & `dstack-0.9.post1/cli/dstack/backend/aws/__init__.py`

 * *Files identical despite different names*

### Comparing `dstack-0.8.1/cli/dstack/backend/aws/compute.py` & `dstack-0.9.post1/cli/dstack/backend/aws/compute.py`

 * *Files identical despite different names*

### Comparing `dstack-0.8.1/cli/dstack/backend/aws/config.py` & `dstack-0.9.post1/cli/dstack/backend/aws/config.py`

 * *Files identical despite different names*

### Comparing `dstack-0.8.1/cli/dstack/backend/aws/logs.py` & `dstack-0.9.post1/cli/dstack/backend/aws/logs.py`

 * *Files identical despite different names*

### Comparing `dstack-0.8.1/cli/dstack/backend/aws/runners.py` & `dstack-0.9.post1/cli/dstack/backend/aws/runners.py`

 * *Files 0% similar despite different names*

```diff
@@ -327,15 +327,15 @@
     if images:
         ami = next(iter(sorted(images, key=lambda i: i["CreationDate"], reverse=True)))
         return ami["ImageId"], ami["Name"]
     else:
         if _version:
             return _get_ami_image(ec2_client, cuda, _version=None)
         else:
-            raise Exception(f"Can't find an AMI image prefix='{ami_name}")
+            raise Exception(f"Can't find an AMI image prefix={ami_name!r}")
 
 
 def _run_instance(
     ec2_client: BaseClient,
     iam_client: BaseClient,
     bucket_name: str,
     region_name: str,
```

### Comparing `dstack-0.8.1/cli/dstack/backend/aws/secrets.py` & `dstack-0.9.post1/cli/dstack/backend/aws/secrets.py`

 * *Files identical despite different names*

### Comparing `dstack-0.8.1/cli/dstack/backend/aws/storage.py` & `dstack-0.9.post1/cli/dstack/backend/aws/storage.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 
 import botocore.exceptions
 from boto3.s3 import transfer
 from botocore.client import BaseClient
 
 from dstack.backend.base.storage import SIGNED_URL_EXPIRATION, CloudStorage
 from dstack.core.storage import StorageFile
-from dstack.utils.common import removeprefix
 
 
 class AWSStorage(CloudStorage):
     def __init__(self, s3_client: BaseClient, bucket_name: str):
         self.s3_client = s3_client
         self.bucket_name = bucket_name
```

### Comparing `dstack-0.8.1/cli/dstack/backend/aws/utils.py` & `dstack-0.9.post1/cli/dstack/backend/aws/utils.py`

 * *Files identical despite different names*

### Comparing `dstack-0.8.1/cli/dstack/backend/base/__init__.py` & `dstack-0.9.post1/cli/dstack/backend/base/__init__.py`

 * *Files identical despite different names*

### Comparing `dstack-0.8.1/cli/dstack/backend/base/artifacts.py` & `dstack-0.9.post1/cli/dstack/backend/base/artifacts.py`

 * *Files identical despite different names*

### Comparing `dstack-0.8.1/cli/dstack/backend/base/compute.py` & `dstack-0.9.post1/cli/dstack/backend/base/compute.py`

 * *Files identical despite different names*

### Comparing `dstack-0.8.1/cli/dstack/backend/base/config.py` & `dstack-0.9.post1/cli/dstack/backend/base/config.py`

 * *Files identical despite different names*

### Comparing `dstack-0.8.1/cli/dstack/backend/base/jobs.py` & `dstack-0.9.post1/cli/dstack/backend/base/jobs.py`

 * *Files identical despite different names*

### Comparing `dstack-0.8.1/cli/dstack/backend/base/logs.py` & `dstack-0.9.post1/cli/dstack/backend/base/logs.py`

 * *Files identical despite different names*

### Comparing `dstack-0.8.1/cli/dstack/backend/base/repos.py` & `dstack-0.9.post1/cli/dstack/backend/base/repos.py`

 * *Files identical despite different names*

### Comparing `dstack-0.8.1/cli/dstack/backend/base/runners.py` & `dstack-0.9.post1/cli/dstack/backend/base/runners.py`

 * *Files identical despite different names*

### Comparing `dstack-0.8.1/cli/dstack/backend/base/runs.py` & `dstack-0.9.post1/cli/dstack/backend/base/runs.py`

 * *Files identical despite different names*

### Comparing `dstack-0.8.1/cli/dstack/backend/base/secrets.py` & `dstack-0.9.post1/cli/dstack/backend/base/secrets.py`

 * *Files identical despite different names*

### Comparing `dstack-0.8.1/cli/dstack/backend/base/storage.py` & `dstack-0.9.post1/cli/dstack/backend/base/storage.py`

 * *Files identical despite different names*

### Comparing `dstack-0.8.1/cli/dstack/backend/base/tags.py` & `dstack-0.9.post1/cli/dstack/backend/base/tags.py`

 * *Files identical despite different names*

### Comparing `dstack-0.8.1/cli/dstack/backend/gcp/__init__.py` & `dstack-0.9.post1/cli/dstack/backend/gcp/__init__.py`

 * *Files identical despite different names*

### Comparing `dstack-0.8.1/cli/dstack/backend/gcp/compute.py` & `dstack-0.9.post1/cli/dstack/backend/gcp/compute.py`

 * *Files identical despite different names*

### Comparing `dstack-0.8.1/cli/dstack/backend/gcp/config.py` & `dstack-0.9.post1/cli/dstack/backend/gcp/config.py`

 * *Files identical despite different names*

### Comparing `dstack-0.8.1/cli/dstack/backend/gcp/logs.py` & `dstack-0.9.post1/cli/dstack/backend/gcp/logs.py`

 * *Files identical despite different names*

### Comparing `dstack-0.8.1/cli/dstack/backend/gcp/secrets.py` & `dstack-0.9.post1/cli/dstack/backend/gcp/secrets.py`

 * *Files identical despite different names*

### Comparing `dstack-0.8.1/cli/dstack/backend/gcp/storage.py` & `dstack-0.9.post1/cli/dstack/backend/gcp/storage.py`

 * *Files identical despite different names*

### Comparing `dstack-0.8.1/cli/dstack/backend/gcp/utils.py` & `dstack-0.9.post1/cli/dstack/backend/gcp/utils.py`

 * *Files identical despite different names*

### Comparing `dstack-0.8.1/cli/dstack/backend/local/__init__.py` & `dstack-0.9.post1/cli/dstack/backend/local/__init__.py`

 * *Files identical despite different names*

### Comparing `dstack-0.8.1/cli/dstack/backend/local/compute.py` & `dstack-0.9.post1/cli/dstack/backend/local/compute.py`

 * *Files identical despite different names*

### Comparing `dstack-0.8.1/cli/dstack/backend/local/config.py` & `dstack-0.9.post1/cli/dstack/backend/local/config.py`

 * *Files identical despite different names*

### Comparing `dstack-0.8.1/cli/dstack/backend/local/logs.py` & `dstack-0.9.post1/cli/dstack/backend/local/logs.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,14 +5,16 @@
 from file_read_backwards import FileReadBackwards
 
 from dstack.backend.base.logs import render_log_message
 from dstack.backend.base.storage import Storage
 from dstack.backend.local.config import LocalConfig
 from dstack.core.log_event import LogEvent
 
+LOGS_TIME_FORMAT = "%Y-%m-%dT%H:%M:%S.%f%z"
+
 
 def poll_logs(
     backend_config: LocalConfig,
     storage: Storage,
     repo_id: str,
     run_name: str,
     start_time: datetime,
@@ -38,19 +40,19 @@
                 yield render_log_message(storage, event, repo_id, jobs_cache)
             else:
                 if found_log:
                     break
 
 
 def _log_line_to_log_event(line: str) -> Dict:
-    log_line_dict = dict(record.split("=") for record in line.split(" "))
+    log_line_dict = dict(record.split("=", maxsplit=1) for record in line.split(" ", maxsplit=2))
     log_line_dict = {k: v.strip().strip('"') for k, v in log_line_dict.items()}
     log_msg = json.loads(log_line_dict["msg"].encode().decode("unicode_escape"))
     return {
         "eventId": log_msg["event_id"],
-        "timestamp": datetime.fromisoformat(log_line_dict["time"]),
+        "timestamp": datetime.strptime(log_line_dict["time"], LOGS_TIME_FORMAT),
         "message": {
             "source": "stdout",
             "log": log_msg["log"],
             "job_id": log_msg["job_id"],
         },
     }
```

### Comparing `dstack-0.8.1/cli/dstack/backend/local/runners.py` & `dstack-0.9.post1/cli/dstack/backend/local/runners.py`

 * *Files identical despite different names*

### Comparing `dstack-0.8.1/cli/dstack/backend/local/secrets.py` & `dstack-0.9.post1/cli/dstack/backend/local/secrets.py`

 * *Files identical despite different names*

### Comparing `dstack-0.8.1/cli/dstack/backend/local/storage.py` & `dstack-0.9.post1/cli/dstack/backend/local/storage.py`

 * *Files identical despite different names*

### Comparing `dstack-0.8.1/cli/dstack/cli/commands/__init__.py` & `dstack-0.9.post1/cli/dstack/cli/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `dstack-0.8.1/cli/dstack/cli/commands/config/__init__.py` & `dstack-0.9.post1/cli/dstack/cli/commands/config/__init__.py`

 * *Files identical despite different names*

### Comparing `dstack-0.8.1/cli/dstack/cli/commands/cp/__init__.py` & `dstack-0.9.post1/cli/dstack/cli/commands/cp/__init__.py`

 * *Files identical despite different names*

### Comparing `dstack-0.8.1/cli/dstack/cli/commands/logs/__init__.py` & `dstack-0.9.post1/cli/dstack/cli/commands/logs/__init__.py`

 * *Files identical despite different names*

### Comparing `dstack-0.8.1/cli/dstack/cli/commands/ls/__init__.py` & `dstack-0.9.post1/cli/dstack/cli/commands/ls/__init__.py`

 * *Files identical despite different names*

### Comparing `dstack-0.8.1/cli/dstack/cli/commands/prune/__init__.py` & `dstack-0.9.post1/cli/dstack/cli/commands/prune/__init__.py`

 * *Files identical despite different names*

### Comparing `dstack-0.8.1/cli/dstack/cli/commands/ps/__init__.py` & `dstack-0.9.post1/cli/dstack/cli/commands/ps/__init__.py`

 * *Files identical despite different names*

### Comparing `dstack-0.8.1/cli/dstack/cli/commands/rm/__init__.py` & `dstack-0.9.post1/cli/dstack/cli/commands/rm/__init__.py`

 * *Files identical despite different names*

### Comparing `dstack-0.8.1/cli/dstack/cli/commands/run/__init__.py` & `dstack-0.9.post1/cli/dstack/cli/commands/run/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,15 +46,15 @@
             load_workflows(os.path.join(os.getcwd(), ".dstack")).keys()
         )  # todo use repo
         provider_names = providers.get_provider_names()
         workflow_or_provider_names = workflow_names + provider_names
         workflow_help = "{" + ",".join(workflow_or_provider_names) + "}"
         self._parser.add_argument(
             "workflow_or_provider",
-            metavar="WORKFLOW | PROVIDER",
+            metavar="WORKFLOW",
             type=str,
             help=workflow_help,
             choices=workflow_or_provider_names,
             nargs="?",
         )
         add_project_argument(self._parser)
         self._parser.add_argument(
@@ -178,19 +178,20 @@
                     progress.update(
                         task, description="Provisioning... It may take up to a minute."
                     )
                     request_errors_printed = False
 
         ports = {}
         jobs = [hub_client.get_job(job_head.job_id) for job_head in job_heads]
-        if hub_client.get_project_backend_type() != "local":
+        backend_type = hub_client.get_project_backend_type()
+        if backend_type != "local":
             console.print("Starting SSH tunnel...")
             ports = allocate_local_ports(jobs)
             if not run_ssh_tunnel(
-                ssh_key, jobs[0].host_name, ports
+                ssh_key, jobs[0].host_name, ports, backend_type
             ):  # todo: cleanup explicitly (stop tunnel)
                 console.print("[warning]Warning: failed to start SSH tunnel[/warning] [red]✗[/]")
         else:
             console.print("Provisioning... It may take up to a minute. [green]✓[/]")
         console.print()
         console.print("[grey58]To exit, press Ctrl+C.[/]")
         console.print()
```

### Comparing `dstack-0.8.1/cli/dstack/cli/commands/run/ssh_tunnel.py` & `dstack-0.9.post1/cli/dstack/cli/commands/run/ssh_tunnel.py`

 * *Files 12% similar despite different names*

```diff
@@ -22,30 +22,39 @@
             ports[ws_logs_port] = get_free_port()
         for app_spec in job.app_specs or []:
             port = job.ports[app_spec.port_index]
             ports[port] = get_free_port()
     return ports
 
 
-def make_ssh_tunnel_args(ssh_key: PathLike, hostname: str, ports: Dict[int, int]) -> List[str]:
+def make_ssh_tunnel_args(
+    ssh_key: PathLike, hostname: str, ports: Dict[int, int], backend_type: str
+) -> List[str]:
+    username = "root"
+    if backend_type == "azure":
+        # root login is disabled on azure
+        # TODO: use non-root for all backends
+        username = "ubuntu"
     args = [
         "ssh",
         "-o",
         "StrictHostKeyChecking=no",
         "-o",
         "UserKnownHostsFile=/dev/null",
         "-i",
         str(ssh_key),
-        f"root@{hostname}",
+        f"{username}@{hostname}",
         "-N",
         "-f",
     ]
     for port_remote, local_port in ports.items():
         args.extend(["-L", f"{local_port}:{hostname}:{port_remote}"])
     return args
 
 
-def run_ssh_tunnel(ssh_key: PathLike, hostname: str, ports: Dict[int, int]) -> bool:
-    args = make_ssh_tunnel_args(ssh_key, hostname, ports)
+def run_ssh_tunnel(
+    ssh_key: PathLike, hostname: str, ports: Dict[int, int], backend_type: str
+) -> bool:
+    args = make_ssh_tunnel_args(ssh_key, hostname, ports, backend_type)
     return (
         subprocess.run(args, stdout=subprocess.DEVNULL, stderr=subprocess.DEVNULL).returncode == 0
     )
```

### Comparing `dstack-0.8.1/cli/dstack/cli/commands/secrets/__init__.py` & `dstack-0.9.post1/cli/dstack/cli/commands/secrets/__init__.py`

 * *Files identical despite different names*

### Comparing `dstack-0.8.1/cli/dstack/cli/commands/start/__init__.py` & `dstack-0.9.post1/cli/dstack/cli/commands/start/__init__.py`

 * *Files identical despite different names*

### Comparing `dstack-0.8.1/cli/dstack/cli/commands/stop/__init__.py` & `dstack-0.9.post1/cli/dstack/cli/commands/stop/__init__.py`

 * *Files identical despite different names*

### Comparing `dstack-0.8.1/cli/dstack/cli/commands/tags/__init__.py` & `dstack-0.9.post1/cli/dstack/cli/commands/tags/__init__.py`

 * *Files identical despite different names*

### Comparing `dstack-0.8.1/cli/dstack/cli/common.py` & `dstack-0.9.post1/cli/dstack/cli/common.py`

 * *Files identical despite different names*

### Comparing `dstack-0.8.1/cli/dstack/cli/config.py` & `dstack-0.9.post1/cli/dstack/cli/config.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,14 +17,17 @@
 
 # TODO: Move ConfigManager functionality to CLIConfigManager
 class ConfigManager:
     def __init__(self, home: PathLike = "~/.dstack"):
         self.home = Path(home).expanduser().resolve()
         self._cache: Dict[str, BaseModel] = {}
 
+    def dstack_key_path(self, repo_dir: Optional[PathLike] = None) -> Path:
+        return self.home / "dstack_rsa"
+
     @property
     def repos(self) -> Path:
         return self.home / "repos"
 
     def repo_user_config_path(self, repo_dir: Optional[PathLike] = None) -> Path:
         """
         :param repo_dir: target repo directory path (default is cwd)
```

### Comparing `dstack-0.8.1/cli/dstack/cli/handlers.py` & `dstack-0.9.post1/cli/dstack/cli/handlers.py`

 * *Files identical despite different names*

### Comparing `dstack-0.8.1/cli/dstack/cli/main.py` & `dstack-0.9.post1/cli/dstack/cli/main.py`

 * *Files identical despite different names*

### Comparing `dstack-0.8.1/cli/dstack/cli/updates.py` & `dstack-0.9.post1/cli/dstack/cli/updates.py`

 * *Files identical despite different names*

### Comparing `dstack-0.8.1/cli/dstack/core/app.py` & `dstack-0.9.post1/cli/dstack/core/app.py`

 * *Files identical despite different names*

### Comparing `dstack-0.8.1/cli/dstack/core/error.py` & `dstack-0.9.post1/cli/dstack/core/error.py`

 * *Files identical despite different names*

### Comparing `dstack-0.8.1/cli/dstack/core/job.py` & `dstack-0.9.post1/cli/dstack/core/job.py`

 * *Files identical despite different names*

### Comparing `dstack-0.8.1/cli/dstack/core/repo/base.py` & `dstack-0.9.post1/cli/dstack/core/repo/base.py`

 * *Files identical despite different names*

### Comparing `dstack-0.8.1/cli/dstack/core/repo/head.py` & `dstack-0.9.post1/cli/dstack/core/repo/head.py`

 * *Files identical despite different names*

### Comparing `dstack-0.8.1/cli/dstack/core/repo/local.py` & `dstack-0.9.post1/cli/dstack/core/repo/local.py`

 * *Files identical despite different names*

### Comparing `dstack-0.8.1/cli/dstack/core/repo/remote.py` & `dstack-0.9.post1/cli/dstack/core/repo/remote.py`

 * *Files identical despite different names*

### Comparing `dstack-0.8.1/cli/dstack/core/repo/spec.py` & `dstack-0.9.post1/cli/dstack/core/repo/spec.py`

 * *Files identical despite different names*

### Comparing `dstack-0.8.1/cli/dstack/core/request.py` & `dstack-0.9.post1/cli/dstack/core/request.py`

 * *Files identical despite different names*

### Comparing `dstack-0.8.1/cli/dstack/core/run.py` & `dstack-0.9.post1/cli/dstack/core/run.py`

 * *Files identical despite different names*

### Comparing `dstack-0.8.1/cli/dstack/core/runners.py` & `dstack-0.9.post1/cli/dstack/core/runners.py`

 * *Files identical despite different names*

### Comparing `dstack-0.8.1/cli/dstack/core/tag.py` & `dstack-0.9.post1/cli/dstack/core/tag.py`

 * *Files identical despite different names*

### Comparing `dstack-0.8.1/cli/dstack/hub/background/tasks/resubmit_jobs.py` & `dstack-0.9.post1/cli/dstack/hub/background/tasks/resubmit_jobs.py`

 * *Files identical despite different names*

### Comparing `dstack-0.8.1/cli/dstack/hub/db/__init__.py` & `dstack-0.9.post1/cli/dstack/hub/db/__init__.py`

 * *Files identical despite different names*

### Comparing `dstack-0.8.1/cli/dstack/hub/db/models.py` & `dstack-0.9.post1/cli/dstack/hub/db/models.py`

 * *Files identical despite different names*

### Comparing `dstack-0.8.1/cli/dstack/hub/main.py` & `dstack-0.9.post1/cli/dstack/hub/main.py`

 * *Files identical despite different names*

### Comparing `dstack-0.8.1/cli/dstack/hub/migration/env.py` & `dstack-0.9.post1/cli/dstack/hub/migration/env.py`

 * *Files identical despite different names*

### Comparing `dstack-0.8.1/cli/dstack/hub/migration/versions/3b900659c822_.py` & `dstack-0.9.post1/cli/dstack/hub/migration/versions/3b900659c822_.py`

 * *Files identical despite different names*

### Comparing `dstack-0.8.1/cli/dstack/hub/models/__init__.py` & `dstack-0.9.post1/cli/dstack/hub/models/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 
 
 class Member(BaseModel):
     user_name: str
     project_role: ProjectRole
 
 
-BackendType = Union[Literal["local"], Literal["aws"], Literal["gcp"]]
+BackendType = Union[Literal["local"], Literal["aws"], Literal["gcp"], Literal["azure"]]
 
 
 class LocalProjectConfig(BaseModel):
     type: Literal["local"] = "local"
     path: Optional[str]
 
 
@@ -96,20 +96,57 @@
     pass
 
 
 class GCPProjectConfigWithCreds(GCPProjectConfig, GCPProjectCreds):
     pass
 
 
-AnyProjectConfig = Union[LocalProjectConfig, AWSProjectConfig, GCPProjectConfig]
+class AzureProjectConfigPartial(BaseModel):
+    type: Literal["azure"] = "azure"
+    tenant_id: str
+    subscription_id: Optional[str]
+    location: Optional[str]
+    storage_account: Optional[str]
+
+
+class AzureProjectCreds(BaseModel):
+    client_id: str
+    client_secret: str
+
+
+class AzureProjectConfigWithCredsPartial(AzureProjectConfigPartial, AzureProjectCreds):
+    pass
+
+
+class AzureProjectConfig(BaseModel):
+    type: Literal["azure"] = "azure"
+    tenant_id: str
+    subscription_id: str
+    location: str
+    storage_account: str
+
+
+class AzureProjectConfigWithCreds(AzureProjectConfig, AzureProjectCreds):
+    pass
+
+
+AnyProjectConfig = Union[
+    LocalProjectConfig, AWSProjectConfig, GCPProjectConfig, AzureProjectConfig
+]
 AnyProjectConfigWithCredsPartial = Union[
-    LocalProjectConfig, AWSProjectConfigWithCredsPartial, GCPProjectConfigWithCredsPartial
+    LocalProjectConfig,
+    AWSProjectConfigWithCredsPartial,
+    GCPProjectConfigWithCredsPartial,
+    AzureProjectConfigWithCredsPartial,
 ]
 AnyProjectConfigWithCreds = Union[
-    LocalProjectConfig, AWSProjectConfigWithCreds, GCPProjectConfigWithCreds
+    LocalProjectConfig,
+    AWSProjectConfigWithCreds,
+    GCPProjectConfigWithCreds,
+    AzureProjectConfigWithCreds,
 ]
 
 
 class ProjectConfig(BaseModel):
     __root__: AnyProjectConfig = Field(..., discriminator="type")
 
 
@@ -272,16 +309,26 @@
     area: Optional[ProjectElement]
     region: Optional[ProjectElement]
     zone: Optional[ProjectElement]
     bucket_name: Optional[ProjectElement]
     vpc_subnet: Optional[GCPVPCSubnetProjectElement]
 
 
+class AzureProjectValues(BaseModel):
+    type: Literal["azure"] = "azure"
+    tenant_id: Optional[ProjectElement]
+    subscription_id: Optional[ProjectElement]
+    location: Optional[ProjectElement]
+    storage_account: Optional[ProjectElement]
+
+
 class ProjectValues(BaseModel):
-    __root__: Union[None, AWSProjectValues, GCPProjectValues] = Field(..., discriminator="type")
+    __root__: Union[None, AWSProjectValues, GCPProjectValues, AzureProjectValues] = Field(
+        ..., discriminator="type"
+    )
 
 
 class UserPatch(BaseModel):
     global_role: GlobalRole
 
 
 class AddMembers(BaseModel):
```

### Comparing `dstack-0.8.1/cli/dstack/hub/repository/users.py` & `dstack-0.9.post1/cli/dstack/hub/repository/users.py`

 * *Files identical despite different names*

### Comparing `dstack-0.8.1/cli/dstack/hub/routers/artifacts.py` & `dstack-0.9.post1/cli/dstack/hub/routers/artifacts.py`

 * *Files identical despite different names*

### Comparing `dstack-0.8.1/cli/dstack/hub/routers/cache.py` & `dstack-0.9.post1/cli/dstack/hub/routers/cache.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 import json
 from typing import Optional
 
-from dstack.api.internal.backend import get_backend_class
 from dstack.backend.base import Backend
-from dstack.core.repo import Repo
 from dstack.hub.db.models import Project
 from dstack.hub.services.backends import get_configurator
 
 cache = {}
 
 
-def get_backend(project: Project) -> Backend:
+def get_backend(project: Project) -> Optional[Backend]:
+    configurator = get_configurator(project.backend)
+    if configurator is None:
+        return None
     key = project.name
     if cache.get(key) is not None:
         return cache[key]
-    backend_cls = get_backend_class(project.backend)
-    configurator = get_configurator(project.backend)
     json_data = json.loads(str(project.config))
     auth_data = json.loads(str(project.auth))
-    config = configurator.get_config_from_hub_config_data(project.name, json_data, auth_data)
+    config = configurator.get_backend_config_from_hub_config_data(
+        project.name, json_data, auth_data
+    )
+    backend_cls = configurator.get_backend_class()
     backend = backend_cls(backend_config=config)
     cache[key] = backend
     return cache[key]
 
 
 def clear_backend_cache(project_name: str):
     if project_name in cache:
```

### Comparing `dstack-0.8.1/cli/dstack/hub/routers/jobs.py` & `dstack-0.9.post1/cli/dstack/hub/routers/jobs.py`

 * *Files identical despite different names*

### Comparing `dstack-0.8.1/cli/dstack/hub/routers/link.py` & `dstack-0.9.post1/cli/dstack/hub/routers/link.py`

 * *Files identical despite different names*

### Comparing `dstack-0.8.1/cli/dstack/hub/routers/logs.py` & `dstack-0.9.post1/cli/dstack/hub/routers/logs.py`

 * *Files identical despite different names*

### Comparing `dstack-0.8.1/cli/dstack/hub/routers/projects.py` & `dstack-0.9.post1/cli/dstack/hub/routers/projects.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,36 +10,35 @@
     ProjectDelete,
     ProjectInfo,
     ProjectInfoWithCreds,
     ProjectValues,
 )
 from dstack.hub.repository.projects import ProjectManager
 from dstack.hub.routers.cache import clear_backend_cache
-from dstack.hub.routers.util import error_detail, get_project
+from dstack.hub.routers.util import error_detail, get_backend_configurator, get_project
 from dstack.hub.security.permissions import (
     Authenticated,
     ProjectAdmin,
     ProjectMember,
     ensure_user_project_admin,
 )
-from dstack.hub.services.backends import get_configurator, local_backend_available
-from dstack.hub.services.backends.base import BackendConfigError, Configurator
+from dstack.hub.services.backends.base import BackendConfigError
 
 router = APIRouter(prefix="/api/projects", tags=["project"])
 
 
 @router.post("/backends/values")
 async def get_backend_config_values(
     config: ProjectConfigWithCredsPartial = Body(),
     user: User = Depends(Authenticated()),
 ) -> ProjectValues:
-    configurator = _get_backend_configurator(config.__root__.type)
+    configurator = get_backend_configurator(config.__root__.type)
     try:
         result = await asyncio.get_running_loop().run_in_executor(
-            None, configurator.configure_hub, config.__root__.dict()
+            None, configurator.configure_project, config.__root__.dict()
         )
     except BackendConfigError as e:
         _error_response_on_config_error(e, path_to_config=[])
     return result
 
 
 @router.get(
@@ -59,25 +58,18 @@
             status_code=status.HTTP_400_BAD_REQUEST,
             detail=[
                 error_detail(
                     "Project exists", code="project_name_not_unique", loc=["project_name"]
                 )
             ],
         )
-    configurator = _get_backend_configurator(project_info.backend.__root__.type)
-    if configurator.name == "local" and not local_backend_available():
-        raise HTTPException(
-            status_code=status.HTTP_400_BAD_REQUEST,
-            detail=[
-                error_detail("Local backend not available", code="local_backend_not_available")
-            ],
-        )
+    configurator = get_backend_configurator(project_info.backend.__root__.type)
     try:
         await asyncio.get_running_loop().run_in_executor(
-            None, configurator.configure_hub, project_info.backend.__root__.dict()
+            None, configurator.configure_project, project_info.backend.__root__.dict()
         )
     except BackendConfigError as e:
         _error_response_on_config_error(e, path_to_config=["backend"])
     await ProjectManager.create_project_from_info(user=user, project_info=project_info)
     return project_info
 
 
@@ -119,36 +111,26 @@
 
 
 @router.patch("/{project_name}")
 async def update_project(
     project_info: ProjectInfoWithCreds = Body(),
     user_project: Tuple[User, Project] = Depends(ProjectAdmin()),
 ) -> ProjectInfoWithCreds:
-    configurator = _get_backend_configurator(project_info.backend.__root__.type)
+    configurator = get_backend_configurator(project_info.backend.__root__.type)
     try:
         await asyncio.get_running_loop().run_in_executor(
-            None, configurator.configure_hub, project_info.backend.__root__.dict()
+            None, configurator.configure_project, project_info.backend.__root__.dict()
         )
     except BackendConfigError as e:
         _error_response_on_config_error(e, path_to_config=["backend"])
     await ProjectManager.update_project_from_info(project_info)
     clear_backend_cache(project_info.project_name)
     return project_info
 
 
-def _get_backend_configurator(backend_type: str) -> Configurator:
-    configurator = get_configurator(backend_type)
-    if configurator is None:
-        raise HTTPException(
-            status_code=status.HTTP_400_BAD_REQUEST,
-            detail=error_detail(f"Unknown backend {backend_type}"),
-        )
-    return configurator
-
-
 def _error_response_on_config_error(e: BackendConfigError, path_to_config: List[str]):
     if len(e.fields) > 0:
         error_details = [
             error_detail(e.message, code=e.code, loc=path_to_config + [f]) for f in e.fields
         ]
         raise HTTPException(
             status_code=status.HTTP_400_BAD_REQUEST,
```

### Comparing `dstack-0.8.1/cli/dstack/hub/routers/repos.py` & `dstack-0.9.post1/cli/dstack/hub/routers/repos.py`

 * *Files identical despite different names*

### Comparing `dstack-0.8.1/cli/dstack/hub/routers/runners.py` & `dstack-0.9.post1/cli/dstack/hub/routers/runners.py`

 * *Files identical despite different names*

### Comparing `dstack-0.8.1/cli/dstack/hub/routers/runs.py` & `dstack-0.9.post1/cli/dstack/hub/routers/runs.py`

 * *Files identical despite different names*

### Comparing `dstack-0.8.1/cli/dstack/hub/routers/secrets.py` & `dstack-0.9.post1/cli/dstack/hub/routers/secrets.py`

 * *Files identical despite different names*

### Comparing `dstack-0.8.1/cli/dstack/hub/routers/storage.py` & `dstack-0.9.post1/cli/dstack/hub/routers/storage.py`

 * *Files identical despite different names*

### Comparing `dstack-0.8.1/cli/dstack/hub/routers/tags.py` & `dstack-0.9.post1/cli/dstack/hub/routers/tags.py`

 * *Files identical despite different names*

### Comparing `dstack-0.8.1/cli/dstack/hub/routers/users.py` & `dstack-0.9.post1/cli/dstack/hub/routers/users.py`

 * *Files identical despite different names*

### Comparing `dstack-0.8.1/cli/dstack/hub/routers/workflows.py` & `dstack-0.9.post1/cli/dstack/hub/routers/workflows.py`

 * *Files identical despite different names*

### Comparing `dstack-0.8.1/cli/dstack/hub/security/permissions.py` & `dstack-0.9.post1/cli/dstack/hub/security/permissions.py`

 * *Files identical despite different names*

### Comparing `dstack-0.8.1/cli/dstack/hub/services/backends/__init__.py` & `dstack-0.9.post1/cli/dstack/hub/services/backends/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,46 +1,63 @@
 import subprocess
 from typing import List, Optional
 
 from dstack.hub.models import BackendType
-from dstack.hub.services.backends.aws import AWSConfigurator
 from dstack.hub.services.backends.base import Configurator
-from dstack.hub.services.backends.gcp import GCPConfigurator
-from dstack.hub.services.backends.local import LocalConfigurator
+from dstack.hub.services.backends.local.configurator import LocalConfigurator
 
-configurators = [
-    AWSConfigurator(),
-    GCPConfigurator(),
-    LocalConfigurator(),
-]
+configurators_classes = []
 
+try:
+    from dstack.hub.services.backends.aws.configurator import AWSConfigurator
 
-backend_type_to_configurator_map = {c.name: c for c in configurators}
+    configurators_classes.append(AWSConfigurator)
+except ImportError:
+    pass
 
+try:
+    from dstack.hub.services.backends.azure.configurator import AzureConfigurator
 
-def get_configurator(backend_type: str) -> Optional[Configurator]:
-    return backend_type_to_configurator_map[backend_type]
-
+    configurators_classes.append(AzureConfigurator)
+except ImportError:
+    pass
 
-docker_available = None
+try:
+    from dstack.hub.services.backends.gcp.configurator import GCPConfigurator
 
-
-def list_avaialble_backend_types() -> List[BackendType]:
-    configurators = [AWSConfigurator(), GCPConfigurator()]
-    if local_backend_available():
-        configurators.append(LocalConfigurator())
-    return [c.name for c in configurators]
+    configurators_classes.append(GCPConfigurator)
+except ImportError:
+    pass
 
 
 def local_backend_available() -> bool:
-    global docker_available
-    if docker_available is None:
-        # docker version will exit with 1 if daemon is not running
-        try:
-            docker_proc = subprocess.run(
-                ["docker", "version"],
-                stdout=subprocess.DEVNULL,
-            )
-            docker_available = docker_proc.returncode == 0
-        except FileNotFoundError:
-            docker_available = False
+    # docker version will exit with 1 if daemon is not running
+    try:
+        docker_proc = subprocess.run(
+            ["docker", "version"],
+            stdout=subprocess.DEVNULL,
+        )
+        docker_available = docker_proc.returncode == 0
+    except FileNotFoundError:
+        docker_available = False
     return docker_available
+
+
+if local_backend_available():
+    configurators_classes.append(LocalConfigurator)
+
+
+backend_type_to_configurator_class_map = {c.NAME: c for c in configurators_classes}
+
+
+def get_configurator(backend_type: str) -> Optional[Configurator]:
+    configurator_class = backend_type_to_configurator_class_map.get(backend_type)
+    if configurator_class is None:
+        return None
+    return configurator_class()
+
+
+def list_avaialble_backend_types() -> List[BackendType]:
+    available_backend_types = []
+    for configurator_class in configurators_classes:
+        available_backend_types.append(configurator_class.NAME)
+    return available_backend_types
```

### Comparing `dstack-0.8.1/cli/dstack/hub/services/backends/aws.py` & `dstack-0.9.post1/cli/dstack/hub/services/backends/aws/configurator.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,18 +1,24 @@
-from typing import Dict, Optional
+import json
+from typing import Dict, Optional, Tuple, Union
 
 import botocore.exceptions
 from boto3.session import Session
 
+from dstack.backend.aws import AwsBackend
 from dstack.backend.aws.config import AWSConfig
 from dstack.backend.base.config import BackendConfig
 from dstack.hub.models import (
     AWSBucketProjectElement,
     AWSBucketProjectElementValue,
+    AWSProjectConfig,
+    AWSProjectConfigWithCreds,
+    AWSProjectCreds,
     AWSProjectValues,
+    Project,
     ProjectElement,
     ProjectElementValue,
 )
 from dstack.hub.services.backends.base import BackendConfigError, Configurator
 
 regions = [
     ("US East, N. Virginia", "us-east-1"),
@@ -26,24 +32,20 @@
     ("Europe, London", "eu-west-2"),
     ("Europe, Paris", "eu-west-3"),
     ("Europe, Stockholm", "eu-north-1"),
 ]
 
 
 class AWSConfigurator(Configurator):
-    @property
-    def name(self):
-        return "aws"
+    NAME = "aws"
 
-    def get_config_from_hub_config_data(
-        self, project_name: str, config_data: Dict, auth_data: Dict
-    ) -> BackendConfig:
-        return AWSConfig.deserialize(config_data, auth_data)
+    def get_backend_class(self) -> type:
+        return AwsBackend
 
-    def configure_hub(self, config_data: Dict) -> AWSProjectValues:
+    def configure_project(self, config_data: Dict) -> AWSProjectValues:
         config = AWSConfig.deserialize(config_data)
 
         if config.region_name is not None and config.region_name not in {r[1] for r in regions}:
             raise BackendConfigError(f"Invalid AWS region {config.region_name}")
 
         try:
             session = Session(
@@ -67,14 +69,55 @@
             session=session, region=config.region_name, default_bucket=config.bucket_name
         )
         project_values.ec2_subnet_id = self._get_hub_subnet(
             session=session, default_subnet=config.subnet_id
         )
         return project_values
 
+    def create_config_auth_data_from_project_config(
+        self, project_config: AWSProjectConfigWithCreds
+    ) -> Tuple[Dict, Dict]:
+        project_config.backend.s3_bucket_name = project_config.backend.s3_bucket_name.replace(
+            "s3://", ""
+        )
+        config = AWSProjectConfig.parse_obj(project_config).dict()
+        auth = AWSProjectCreds.parse_obj(project_config).dict()
+        return config, auth
+
+    def get_backend_config_from_hub_config_data(
+        self, project_name: str, config_data: Dict, auth_data: Dict
+    ) -> BackendConfig:
+        return AWSConfig.deserialize(config_data, auth_data)
+
+    def get_project_config_from_project(
+        self, project: Project, include_creds: bool
+    ) -> Union[AWSProjectConfig, AWSProjectConfigWithCreds]:
+        json_config = json.loads(project.config)
+        region_name = json_config["region_name"]
+        s3_bucket_name = json_config["s3_bucket_name"]
+        ec2_subnet_id = json_config["ec2_subnet_id"]
+        if include_creds:
+            json_auth = json.loads(project.auth)
+            access_key = json_auth["access_key"]
+            secret_key = json_auth["secret_key"]
+            return AWSProjectConfigWithCreds(
+                access_key=access_key,
+                secret_key=secret_key,
+                region_name=region_name,
+                region_name_title=region_name,
+                s3_bucket_name=s3_bucket_name,
+                ec2_subnet_id=ec2_subnet_id,
+            )
+        return AWSProjectConfig(
+            region_name=region_name,
+            region_name_title=region_name,
+            s3_bucket_name=s3_bucket_name,
+            ec2_subnet_id=ec2_subnet_id,
+        )
+
     def _get_hub_regions(self, default_region: Optional[str]) -> ProjectElement:
         element = ProjectElement(selected=default_region)
         for r in regions:
             element.values.append(ProjectElementValue(value=r[1], label=r[0]))
         return element
 
     def _get_hub_buckets(
```

### Comparing `dstack-0.8.1/cli/dstack/hub/services/backends/gcp.py` & `dstack-0.9.post1/cli/dstack/hub/services/backends/gcp/configurator.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,24 @@
 import json
-from typing import Dict, Optional, Tuple
+from typing import Dict, Optional, Tuple, Union
 
 from google.cloud import compute_v1, storage
 from google.oauth2 import service_account
 
 from dstack.backend.base.config import BackendConfig
+from dstack.backend.gcp import GCPBackend
 from dstack.backend.gcp.config import GCPConfig
 from dstack.hub.models import (
+    GCPProjectConfig,
+    GCPProjectConfigWithCreds,
+    GCPProjectCreds,
     GCPProjectValues,
     GCPVPCSubnetProjectElement,
     GCPVPCSubnetProjectElementValue,
+    Project,
     ProjectElement,
     ProjectElementValue,
 )
 from dstack.hub.services.backends.base import BackendConfigError, Configurator
 
 DEFAULT_GEOGRAPHIC_AREA = "North America"
 
@@ -95,35 +100,20 @@
         "default_region": "australia-southeast1",
         "default_zone": "australia-southeast1-c",
     },
 ]
 
 
 class GCPConfigurator(Configurator):
-    @property
-    def name(self):
-        return "gcp"
+    NAME = "gcp"
 
-    def get_config_from_hub_config_data(
-        self, project_name: str, config_data: Dict, auth_data: Dict
-    ) -> BackendConfig:
-        credentials = json.loads(auth_data["credentials"])
-        data = {
-            "backend": "gcp",
-            "credentials": credentials,
-            "project": credentials["project_id"],
-            "region": config_data["region"],
-            "zone": config_data["zone"],
-            "bucket": config_data["bucket_name"],
-            "vpc": config_data["vpc"],
-            "subnet": config_data["subnet"],
-        }
-        return GCPConfig.deserialize(data)
+    def get_backend_class(self) -> type:
+        return GCPBackend
 
-    def configure_hub(self, config_data: Dict) -> GCPProjectValues:
+    def configure_project(self, config_data: Dict) -> GCPProjectValues:
         try:
             service_account_info = json.loads(config_data.get("credentials"))
             self.credentials = service_account.Credentials.from_service_account_info(
                 info=service_account_info
             )
             storage_client = storage.Client(credentials=self.credentials)
             storage_client.list_buckets(max_results=1)
@@ -150,14 +140,70 @@
         project_values.vpc_subnet = self._get_hub_vpc_subnet(
             region=project_values.region.selected,
             default_vpc=config_data.get("vpc"),
             default_subnet=config_data.get("subnet"),
         )
         return project_values
 
+    def create_config_auth_data_from_project_config(
+        self, project_config: GCPProjectConfigWithCreds
+    ) -> Tuple[Dict, Dict]:
+        config = GCPProjectConfig.parse_obj(project_config).dict()
+        auth = GCPProjectCreds.parse_obj(project_config).dict()
+        return config, auth
+
+    def get_backend_config_from_hub_config_data(
+        self, project_name: str, config_data: Dict, auth_data: Dict
+    ) -> BackendConfig:
+        credentials = json.loads(auth_data["credentials"])
+        data = {
+            "backend": "gcp",
+            "credentials": credentials,
+            "project": credentials["project_id"],
+            "region": config_data["region"],
+            "zone": config_data["zone"],
+            "bucket": config_data["bucket_name"],
+            "vpc": config_data["vpc"],
+            "subnet": config_data["subnet"],
+        }
+        return GCPConfig.deserialize(data)
+
+    def get_project_config_from_project(
+        self, project: Project, include_creds: bool
+    ) -> Union[GCPProjectConfig, GCPProjectConfigWithCreds]:
+        json_config = json.loads(project.config)
+        area = json_config["area"]
+        region = json_config["region"]
+        zone = json_config["zone"]
+        bucket_name = json_config["bucket_name"]
+        vpc = json_config["vpc"]
+        subnet = json_config["subnet"]
+        if include_creds:
+            json_auth = json.loads(project.auth)
+            credentials = json_auth["credentials"]
+            credentials_filename = json_auth["credentials_filename"]
+            return GCPProjectConfigWithCreds(
+                credentials=credentials,
+                credentials_filename=credentials_filename,
+                area=area,
+                region=region,
+                zone=zone,
+                bucket_name=bucket_name,
+                vpc=vpc,
+                subnet=subnet,
+            )
+        return GCPProjectConfig(
+            area=area,
+            region=region,
+            zone=zone,
+            bucket_name=bucket_name,
+            vpc=vpc,
+            subnet=subnet,
+        )
+
     def _get_hub_geographic_area(self, default_area: Optional[str]) -> ProjectElement:
         area_names = sorted([l["name"] for l in GCP_LOCATIONS])
         if default_area is None:
             default_area = DEFAULT_GEOGRAPHIC_AREA
         if default_area not in area_names:
             raise BackendConfigError(f"Invalid GCP area {default_area}")
         element = ProjectElement(selected=default_area)
```

### Comparing `dstack-0.8.1/cli/dstack/hub/utils/logging.py` & `dstack-0.9.post1/cli/dstack/hub/utils/logging.py`

 * *Files identical despite different names*

### Comparing `dstack-0.8.1/cli/dstack/providers/__init__.py` & `dstack-0.9.post1/cli/dstack/providers/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -232,14 +232,15 @@
         if not self.loaded:
             raise Exception("The provider is not loaded")
         job_specs = self.create_job_specs()
 
         with tempfile.NamedTemporaryFile("w+b") as f:
             repo_code_filename = hub_client.repo.repo_data.write_code_file(f)
             f.seek(0)
+            # FIXME: this should be replaced with public API call
             hub_client._storage.upload_file(f.name, repo_code_filename, lambda _: ...)
 
         # [TODO] Handle master job
         jobs = []
         for i, job_spec in enumerate(job_specs):
             job = Job(
                 job_id=f"{self.run_name},{self.workflow_name or ''},{i}",
```

### Comparing `dstack-0.8.1/cli/dstack/providers/_torchrun/main.py` & `dstack-0.9.post1/cli/dstack/providers/_torchrun/main.py`

 * *Files identical despite different names*

### Comparing `dstack-0.8.1/cli/dstack/providers/bash/main.py` & `dstack-0.9.post1/cli/dstack/providers/bash/main.py`

 * *Files identical despite different names*

### Comparing `dstack-0.8.1/cli/dstack/providers/code/main.py` & `dstack-0.9.post1/cli/dstack/providers/code/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,15 @@
         run_name: str,
         ssh_key_pub: Optional[str] = None,
     ):
         super().load(hub_client, args, workflow_name, provider_data, run_name, ssh_key_pub)
         self.setup = self._get_list_data("setup") or self._get_list_data("before_run")
         self.ports = self.provider_data.get("ports")
         self.python = self._safe_python_version("python")
-        self.version = self.provider_data.get("version") or "1.74.3"
+        self.version = self.provider_data.get("version") or "1.78.1"
         self.env = self._env()
         self.artifact_specs = self._artifact_specs()
         self.working_dir = self.provider_data.get("working_dir")
         self.resources = self._resources()
         self.image_name = self._image_name()
 
     def _create_parser(self, workflow_name: Optional[str]) -> Optional[ArgumentParser]:
@@ -125,15 +125,15 @@
                 "pip install ipykernel -q",
                 "mkdir -p /tmp",
                 'if [ $(uname -m) = "aarch64" ]; then arch="arm64"; else arch="x64"; fi',
                 f"wget -q https://github.com/gitpod-io/openvscode-server/releases/download/"
                 f"openvscode-server-v{self.version}/openvscode-server-v{self.version}-linux-$arch.tar.gz -O "
                 f"/tmp/openvscode-server-v{self.version}-linux-$arch.tar.gz",
                 f"tar -xzf /tmp/openvscode-server-v{self.version}-linux-$arch.tar.gz -C /tmp",
-                f"/tmp/openvscode-server-v{self.version}-linux-$arch/bin/openvscode-server --install-extension ms-python.python",
+                f"/tmp/openvscode-server-v{self.version}-linux-$arch/bin/openvscode-server --install-extension ms-python.python --install-extension ms-toolsai.jupyter",
                 "rm /usr/bin/python2*",
             ]
         )
         if self.setup:
             commands.extend(self.setup)
         commands.append(
             f"/tmp/openvscode-server-v{self.version}-linux-$arch/bin/openvscode-server --port $_PORT --host 0.0.0.0 --connection-token $CONNECTION_TOKEN --default-folder /workflow"
```

### Comparing `dstack-0.8.1/cli/dstack/providers/docker/main.py` & `dstack-0.9.post1/cli/dstack/providers/docker/main.py`

 * *Files identical despite different names*

### Comparing `dstack-0.8.1/cli/dstack/providers/lab/main.py` & `dstack-0.9.post1/cli/dstack/providers/lab/main.py`

 * *Files identical despite different names*

### Comparing `dstack-0.8.1/cli/dstack/providers/notebook/main.py` & `dstack-0.9.post1/cli/dstack/providers/notebook/main.py`

 * *Files identical despite different names*

### Comparing `dstack-0.8.1/cli/dstack/utils/common.py` & `dstack-0.9.post1/cli/dstack/utils/common.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,16 +2,14 @@
 import os
 import re
 import time
 from datetime import datetime, timedelta, timezone
 from pathlib import Path
 from typing import Any, Dict, Optional, Union
 
-from botocore.utils import parse_timestamp
-
 PathLike = Union[str, os.PathLike]
 
 
 def get_dstack_dir() -> Path:
     return Path.joinpath(Path.home(), ".dstack")
 
 
@@ -77,17 +75,23 @@
 def since(timestamp: str) -> datetime:
     regex = re.compile(r"(?P<amount>\d+)(?P<unit>s|m|h|d|w)$")
     re_match = regex.match(timestamp)
     if re_match:
         datetime_value = _relative_timestamp_to_datetime(
             int(re_match.group("amount")), re_match.group("unit")
         )
-    else:
-        datetime_value = parse_timestamp(timestamp)
-    return datetime_value
+        return datetime_value
+    try:
+        return datetime.fromisoformat(timestamp)
+    except ValueError:
+        pass
+    try:
+        return datetime.fromtimestamp(int(timestamp))
+    except Exception:
+        raise ValueError("Invalid datetime format")
 
 
 def _relative_timestamp_to_datetime(amount, unit):
     multiplier = {
         "s": 1,
         "m": 60,
         "h": 3600,
```

### Comparing `dstack-0.8.1/cli/dstack/utils/escape.py` & `dstack-0.9.post1/cli/dstack/utils/escape.py`

 * *Files identical despite different names*

### Comparing `dstack-0.8.1/cli/dstack/utils/hash.py` & `dstack-0.9.post1/cli/dstack/utils/hash.py`

 * *Files identical despite different names*

### Comparing `dstack-0.8.1/cli/dstack/utils/interpolator.py` & `dstack-0.9.post1/cli/dstack/utils/interpolator.py`

 * *Files identical despite different names*

### Comparing `dstack-0.8.1/cli/dstack/utils/random_names.py` & `dstack-0.9.post1/cli/dstack/utils/random_names.py`

 * *Files identical despite different names*

### Comparing `dstack-0.8.1/cli/dstack/utils/ssh.py` & `dstack-0.9.post1/cli/dstack/utils/ssh.py`

 * *Files identical despite different names*

### Comparing `dstack-0.8.1/cli/dstack/utils/workflows.py` & `dstack-0.9.post1/cli/dstack/utils/workflows.py`

 * *Files identical despite different names*

### Comparing `dstack-0.8.1/cli/dstack.egg-info/SOURCES.txt` & `dstack-0.9.post1/cli/dstack.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -14,26 +14,31 @@
 cli/dstack/api/runs.py
 cli/dstack/api/hub/__init__.py
 cli/dstack/api/hub/_api_client.py
 cli/dstack/api/hub/_client.py
 cli/dstack/api/hub/_config.py
 cli/dstack/api/hub/_storage.py
 cli/dstack/api/hub/errors.py
-cli/dstack/api/internal/__init__.py
-cli/dstack/api/internal/backend.py
 cli/dstack/backend/__init__.py
 cli/dstack/backend/aws/__init__.py
 cli/dstack/backend/aws/compute.py
 cli/dstack/backend/aws/config.py
 cli/dstack/backend/aws/logs.py
 cli/dstack/backend/aws/repos.py
 cli/dstack/backend/aws/runners.py
 cli/dstack/backend/aws/secrets.py
 cli/dstack/backend/aws/storage.py
 cli/dstack/backend/aws/utils.py
+cli/dstack/backend/azure/__init__.py
+cli/dstack/backend/azure/compute.py
+cli/dstack/backend/azure/config.py
+cli/dstack/backend/azure/logs.py
+cli/dstack/backend/azure/secrets.py
+cli/dstack/backend/azure/storage.py
+cli/dstack/backend/azure/utils.py
 cli/dstack/backend/base/__init__.py
 cli/dstack/backend/base/artifacts.py
 cli/dstack/backend/base/cache.py
 cli/dstack/backend/base/compute.py
 cli/dstack/backend/base/config.py
 cli/dstack/backend/base/jobs.py
 cli/dstack/backend/base/logs.py
@@ -69,14 +74,15 @@
 cli/dstack/cli/commands/config/__init__.py
 cli/dstack/cli/commands/cp/__init__.py
 cli/dstack/cli/commands/init/__init__.py
 cli/dstack/cli/commands/logs/__init__.py
 cli/dstack/cli/commands/ls/__init__.py
 cli/dstack/cli/commands/prune/__init__.py
 cli/dstack/cli/commands/ps/__init__.py
+cli/dstack/cli/commands/resubmit/__init__.py
 cli/dstack/cli/commands/rm/__init__.py
 cli/dstack/cli/commands/run/__init__.py
 cli/dstack/cli/commands/run/ssh_tunnel.py
 cli/dstack/cli/commands/secrets/__init__.py
 cli/dstack/cli/commands/start/__init__.py
 cli/dstack/cli/commands/stop/__init__.py
 cli/dstack/cli/commands/tags/__init__.py
@@ -136,18 +142,24 @@
 cli/dstack/hub/routers/util.py
 cli/dstack/hub/routers/workflows.py
 cli/dstack/hub/security/__init__.py
 cli/dstack/hub/security/permissions.py
 cli/dstack/hub/security/utils.py
 cli/dstack/hub/services/__init__.py
 cli/dstack/hub/services/backends/__init__.py
-cli/dstack/hub/services/backends/aws.py
 cli/dstack/hub/services/backends/base.py
-cli/dstack/hub/services/backends/gcp.py
-cli/dstack/hub/services/backends/local.py
+cli/dstack/hub/services/backends/aws/__init__.py
+cli/dstack/hub/services/backends/aws/configurator.py
+cli/dstack/hub/services/backends/azure/__init__.py
+cli/dstack/hub/services/backends/azure/azure_identity_credential_adapter.py
+cli/dstack/hub/services/backends/azure/configurator.py
+cli/dstack/hub/services/backends/gcp/__init__.py
+cli/dstack/hub/services/backends/gcp/configurator.py
+cli/dstack/hub/services/backends/local/__init__.py
+cli/dstack/hub/services/backends/local/configurator.py
 cli/dstack/hub/utils/__init__.py
 cli/dstack/hub/utils/logging.py
 cli/dstack/providers/__init__.py
 cli/dstack/providers/_torchrun/__init__.py
 cli/dstack/providers/_torchrun/main.py
 cli/dstack/providers/bash/__init__.py
 cli/dstack/providers/bash/main.py
```

### Comparing `dstack-0.8.1/cli/tests/backend/base/test_logs.py` & `dstack-0.9.post1/cli/tests/backend/base/test_logs.py`

 * *Files identical despite different names*

### Comparing `dstack-0.8.1/cli/tests/hub/common.py` & `dstack-0.9.post1/cli/tests/hub/common.py`

 * *Files identical despite different names*

### Comparing `dstack-0.8.1/cli/tests/hub/routers/test_jobs.py` & `dstack-0.9.post1/cli/tests/hub/routers/test_jobs.py`

 * *Files identical despite different names*

### Comparing `dstack-0.8.1/cli/tests/hub/routers/test_projects.py` & `dstack-0.9.post1/cli/tests/hub/routers/test_projects.py`

 * *Files identical despite different names*

### Comparing `dstack-0.8.1/cli/tests/hub/routers/test_users.py` & `dstack-0.9.post1/cli/tests/hub/routers/test_users.py`

 * *Files identical despite different names*

### Comparing `dstack-0.8.1/cli/tests/integration/common.py` & `dstack-0.9.post1/cli/tests/integration/common.py`

 * *Files 6% similar despite different names*

```diff
@@ -80,16 +80,22 @@
 @contextmanager
 def terminate_on_exit(proc: subprocess.Popen) -> subprocess.Popen:
     try:
         yield proc
     finally:
         process = psutil.Process(proc.pid)
         for child in process.children(recursive=True):
-            child.kill()
-        process.kill()
+            try:
+                child.kill()
+            except psutil.NoSuchProcess:
+                continue
+        try:
+            process.kill()
+        except psutil.NoSuchProcess:
+            pass
 
 
 # TODO: Figure out a way to read process stderr reliably.
 # proc.communicate() may hang even with timeout.
 #
 # @contextmanager
 # def terminate_on_exit(proc: subprocess.Popen) -> subprocess.Popen:
```

### Comparing `dstack-0.8.1/cli/tests/integration/test_commands.py` & `dstack-0.9.post1/cli/tests/integration/test_commands.py`

 * *Files 11% similar despite different names*

```diff
@@ -36,22 +36,24 @@
             ]
         )
         assert exit_code == 1
         assert "Cannot connect to hub" in capsys.readouterr().out
 
 
 class TestInit:
-    def test_warns_if_no_ssh_key(
+    def test_generate_default_ssh_key(
         self, capsys: CaptureFixture, dstack_dir: Path, tests_local_repo: Path
     ):
+        dstack_key_path = dstack_dir / "dstack_rsa"
         with hub_process(dstack_dir):
+            assert not dstack_key_path.exists()
             exit_code = run_dstack_cli(["init"], dstack_dir=dstack_dir, repo_dir=tests_local_repo)
             assert exit_code == 0
-            stdout = capsys.readouterr().out
-            assert "WARNING" in stdout and "SSH is not enabled" in stdout
+            print(list(dstack_dir.iterdir()))
+            assert dstack_key_path.exists()
 
 
 class TestRun:
     def test_requires_config(
         self, capsys: CaptureFixture, dstack_dir: Path, tests_local_repo: Path
     ):
         exit_code = run_dstack_cli(
@@ -70,38 +72,40 @@
             assert exit_code == 1
             assert "Call `dstack init` first" in capsys.readouterr().out
 
     def test_runs_workflow_from_bash_provider(
         self, capsys: CaptureFixture, dstack_dir: Path, tests_local_repo: Path
     ):
         with hub_process(dstack_dir):
+            exit_code = run_dstack_cli(["init"], dstack_dir=dstack_dir, repo_dir=tests_local_repo)
+            assert exit_code == 0
             exit_code = run_dstack_cli(
                 ["run", "bash", "-c", "echo 'Hello, world!'"],
                 dstack_dir=dstack_dir,
                 repo_dir=tests_local_repo,
             )
             assert exit_code == 0
             assert "Hello, world!" in capsys.readouterr().out
 
     def test_runs_workflow_from_yaml_file(
-        self, capsys: CaptureFixture, dstack_dir: Path, tests_public_repo: Path, ssh_key
+        self, capsys: CaptureFixture, dstack_dir: Path, tests_public_repo: Path
     ):
         with hub_process(dstack_dir):
             exit_code = run_dstack_cli(["init"], dstack_dir=dstack_dir, repo_dir=tests_public_repo)
             assert exit_code == 0
             exit_code = run_dstack_cli(
                 ["run", "hello"], dstack_dir=dstack_dir, repo_dir=tests_public_repo
             )
             assert exit_code == 0
             assert "Hello, world!" in capsys.readouterr().out
 
 
 class TestArtifacts:
     def test_lists_artifacts(
-        self, capsys: CaptureFixture, dstack_dir: Path, tests_public_repo: Path, ssh_key
+        self, capsys: CaptureFixture, dstack_dir: Path, tests_public_repo: Path
     ):
         with hub_process(dstack_dir):
             exit_code = run_dstack_cli(["init"], dstack_dir=dstack_dir, repo_dir=tests_public_repo)
             assert exit_code == 0
             capsys.readouterr()
             exit_code = run_dstack_cli(
                 ["run", "artifacts-ls"], dstack_dir=dstack_dir, repo_dir=tests_public_repo
@@ -131,15 +135,15 @@
                 ["22.txt", "2.0B"],
             ]
             _assert_table_output(capsys.readouterr().out, expected_table)
 
 
 class TestDeps:
     def test_reads_artifacts_from_dep_workflow(
-        self, capsys: CaptureFixture, dstack_dir: Path, tests_public_repo: Path, ssh_key
+        self, capsys: CaptureFixture, dstack_dir: Path, tests_public_repo: Path
     ):
         with hub_process(dstack_dir):
             exit_code = run_dstack_cli(["init"], dstack_dir=dstack_dir, repo_dir=tests_public_repo)
             assert exit_code == 0
             exit_code = run_dstack_cli(
                 ["run", "hello-txt"], dstack_dir=dstack_dir, repo_dir=tests_public_repo
             )
@@ -152,14 +156,16 @@
 
 
 class TestSecrets:
     def test_adds_and_reads_secret(
         self, capsys: CaptureFixture, dstack_dir: Path, tests_local_repo: Path
     ):
         with hub_process(dstack_dir):
+            exit_code = run_dstack_cli(["init"], dstack_dir=dstack_dir, repo_dir=tests_local_repo)
+            assert exit_code == 0
             exit_code = run_dstack_cli(
                 ["secrets", "add", "MY_SECRET", "my_secret_value"],
                 dstack_dir=dstack_dir,
                 repo_dir=tests_local_repo,
             )
             assert exit_code == 0
             exit_code = run_dstack_cli(
```

### Comparing `dstack-0.8.1/cli/tests/providers/docker/test_entrypoint.py` & `dstack-0.9.post1/cli/tests/providers/docker/test_entrypoint.py`

 * *Files identical despite different names*

### Comparing `dstack-0.8.1/cli/tests/providers/test_local_path.py` & `dstack-0.9.post1/cli/tests/providers/test_local_path.py`

 * *Files identical despite different names*

### Comparing `dstack-0.8.1/cli/tests/utils/escape.py` & `dstack-0.9.post1/cli/tests/utils/escape.py`

 * *Files identical despite different names*

### Comparing `dstack-0.8.1/cli/tests/utils/test_interpolator.py` & `dstack-0.9.post1/cli/tests/utils/test_interpolator.py`

 * *Files identical despite different names*

### Comparing `dstack-0.8.1/cli/tests/utils/test_merge_workflow_data.py` & `dstack-0.9.post1/cli/tests/utils/test_merge_workflow_data.py`

 * *Files identical despite different names*

### Comparing `dstack-0.8.1/cli/tests/utils/test_tarignore.py` & `dstack-0.9.post1/cli/tests/utils/test_tarignore.py`

 * *Files identical despite different names*

