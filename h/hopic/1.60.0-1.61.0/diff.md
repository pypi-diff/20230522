# Comparing `tmp/hopic-1.60.0.tar.gz` & `tmp/hopic-1.61.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/jenkins/workspace/hopic_release_1/dist/tmpxrfasv9t/hopic-1.60.0.tar", last modified: Mon Apr  3 07:40:05 2023, max compression
+gzip compressed data, was "/jenkins/workspace/hopic_release_1/dist/tmp0nf7l9tz/hopic-1.61.0.tar", last modified: Mon May 22 07:41:46 2023, max compression
```

## Comparing `hopic-1.60.0.tar` & `hopic-1.61.0.tar`

### file list

```diff
@@ -1,140 +1,147 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 07:40:05.000000 hopic-1.60.0/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6351 2022-03-18 16:12:34.000000 hopic-1.60.0/hopic-ci-config.yaml
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1728 2023-03-21 12:05:25.000000 hopic-1.60.0/tox.ini
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 07:40:05.000000 hopic-1.60.0/vars/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5706 2021-05-11 08:24:17.000000 hopic-1.60.0/vars/printMetrics.groovy
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    84346 2023-03-24 13:43:41.000000 hopic-1.60.0/vars/getCiDriver.groovy
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 07:40:05.000000 hopic-1.60.0/src/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 07:40:05.000000 hopic-1.60.0/src/com/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 07:40:05.000000 hopic-1.60.0/src/com/tomtom/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 07:40:05.000000 hopic-1.60.0/src/com/tomtom/hopic/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6753 2022-06-14 09:15:10.000000 hopic-1.60.0/src/com/tomtom/hopic/HopicEventCallbacks.groovy
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      855 2019-01-04 15:25:30.000000 hopic-1.60.0/REQUIREMENTS.md
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      277 2021-11-15 13:30:02.000000 hopic-1.60.0/doc-requirements.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2260 2022-01-28 10:24:00.000000 hopic-1.60.0/Jenkinsfile
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      557 2021-05-07 15:03:02.000000 hopic-1.60.0/mypy.ini
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 07:40:05.000000 hopic-1.60.0/examples/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2545 2019-10-29 14:49:42.000000 hopic-1.60.0/examples/parallel-phases.yaml
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      195 2019-11-07 14:38:21.000000 hopic-1.60.0/examples/junit.yaml
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      140 2021-10-06 13:00:51.000000 hopic-1.60.0/examples/allow-failures-junit.yaml
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      188 2020-12-04 14:21:57.000000 hopic-1.60.0/examples/pass-through-env-vars.yaml
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      823 2019-11-07 14:38:21.000000 hopic-1.60.0/examples/artifactory-promote.yaml
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      661 2019-11-07 14:38:21.000000 hopic-1.60.0/examples/upload-artifactory.yaml
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      274 2020-01-10 14:03:05.000000 hopic-1.60.0/examples/image-mapping.yaml
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      190 2021-06-09 12:02:18.000000 hopic-1.60.0/examples/timeout-variant.yaml
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      127 2021-02-09 11:51:15.000000 hopic-1.60.0/examples/allow-missing-archive.yaml
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      151 2019-11-07 14:38:21.000000 hopic-1.60.0/examples/node-label.yaml
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 07:40:05.000000 hopic-1.60.0/examples/simple/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1839 2020-09-28 15:18:56.000000 hopic-1.60.0/examples/simple/Jenkinsfile
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      379 2019-01-04 14:47:49.000000 hopic-1.60.0/examples/simple/dependency_manifest.xml
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2492 2021-01-21 19:52:27.000000 hopic-1.60.0/examples/simple/hopic-ci-config.yml
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      338 2022-03-22 15:11:48.000000 hopic-1.60.0/examples/finally.yaml
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      930 2021-01-21 19:52:27.000000 hopic-1.60.0/examples/volumes-override.yaml
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      235 2020-08-19 12:54:41.000000 hopic-1.60.0/examples/with-keyring-credentials.yaml
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      299 2020-11-30 14:08:37.000000 hopic-1.60.0/examples/ci-locks.yaml
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      259 2021-01-21 19:52:27.000000 hopic-1.60.0/examples/docker-in-docker.yaml
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      379 2019-01-04 14:47:49.000000 hopic-1.60.0/examples/dependency_manifest.xml
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      405 2021-06-09 10:59:19.000000 hopic-1.60.0/examples/timeout.yaml
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      515 2019-11-05 15:44:39.000000 hopic-1.60.0/examples/archive.yaml
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       59 2019-11-25 06:27:20.000000 hopic-1.60.0/examples/clean.yaml
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      192 2020-10-19 07:55:45.000000 hopic-1.60.0/examples/config.yaml
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      337 2020-12-03 13:52:01.000000 hopic-1.60.0/examples/environment.yaml
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      205 2021-01-21 19:52:27.000000 hopic-1.60.0/examples/upload-on-fail.yaml
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       90 2020-08-12 13:05:54.000000 hopic-1.60.0/examples/disable-etc-volumes.yaml
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      428 2019-11-05 15:44:39.000000 hopic-1.60.0/examples/with-volumes.yaml
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      452 2021-01-21 19:52:27.000000 hopic-1.60.0/examples/post-submit.yaml
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      283 2019-11-07 14:38:21.000000 hopic-1.60.0/examples/fingerprint.yaml
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      139 2021-02-09 11:51:15.000000 hopic-1.60.0/examples/allow-missing-junit.yaml
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      367 2019-11-18 07:58:57.000000 hopic-1.60.0/examples/description.yaml
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      284 2021-01-21 19:52:27.000000 hopic-1.60.0/examples/version-bump-conventional.yaml
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      223 2019-11-05 15:44:39.000000 hopic-1.60.0/examples/image-ivy-manifest.yaml
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      166 2020-09-14 14:10:55.000000 hopic-1.60.0/examples/pip.yaml
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      131 2019-11-19 12:22:45.000000 hopic-1.60.0/examples/version-bump-constant.yaml
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      358 2021-01-22 15:16:09.000000 hopic-1.60.0/examples/docker-extra-args.yaml
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1051 2020-12-04 14:21:57.000000 hopic-1.60.0/examples/with-credentials.yaml
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      473 2020-10-28 13:20:54.000000 hopic-1.60.0/examples/stash.yaml
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 07:40:05.000000 hopic-1.60.0/examples/embed/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      114 2020-05-15 09:48:27.000000 hopic-1.60.0/examples/embed/embed.yaml
--rwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)      230 2020-08-27 06:38:21.000000 hopic-1.60.0/examples/embed/yaml-generation.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      302 2019-11-07 14:38:21.000000 hopic-1.60.0/examples/run-on-change.yaml
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-04-03 07:40:05.000000 hopic-1.60.0/setup.cfg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1279 2020-08-21 14:01:27.000000 hopic-1.60.0/README.rst
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2189 2023-04-03 07:40:05.000000 hopic-1.60.0/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2778 2023-03-17 09:31:31.000000 hopic-1.60.0/setup.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       48 2019-11-11 15:31:32.000000 hopic-1.60.0/.gitattributes
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 07:40:05.000000 hopic-1.60.0/hopic.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2994 2023-04-03 07:40:05.000000 hopic-1.60.0/hopic.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       61 2023-04-03 07:40:05.000000 hopic-1.60.0/hopic.egg-info/entry_points.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        6 2023-04-03 07:40:05.000000 hopic-1.60.0/hopic.egg-info/top_level.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2189 2023-04-03 07:40:05.000000 hopic-1.60.0/hopic.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-04-03 07:40:05.000000 hopic-1.60.0/hopic.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-04-03 07:40:05.000000 hopic-1.60.0/hopic.egg-info/zip-safe
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      291 2023-04-03 07:40:05.000000 hopic-1.60.0/hopic.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      149 2021-02-19 11:08:41.000000 hopic-1.60.0/pytest.ini
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 07:40:05.000000 hopic-1.60.0/hopic/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 07:40:05.000000 hopic-1.60.0/hopic/test/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2332 2020-08-29 06:53:11.000000 hopic-1.60.0/hopic/test/test_credentials.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3292 2021-04-28 11:03:59.000000 hopic-1.60.0/hopic/test/test_template_utils.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    57112 2022-03-17 09:16:40.000000 hopic-1.60.0/hopic/test/test_config_reader.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7576 2021-05-21 10:41:19.000000 hopic-1.60.0/hopic/test/test_version_bump.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    12161 2023-03-22 11:36:07.000000 hopic-1.60.0/hopic/test/test_checkout.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2491 2021-05-21 10:41:19.000000 hopic-1.60.0/hopic/test/test_execution.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    26412 2022-02-01 16:50:00.000000 hopic-1.60.0/hopic/test/test_extensions.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10668 2022-03-22 15:11:48.000000 hopic-1.60.0/hopic/test/test_getinfo.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      871 2021-07-09 16:01:55.000000 hopic-1.60.0/hopic/test/test_examples.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 07:40:05.000000 hopic-1.60.0/hopic/test/docker-images/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 07:40:05.000000 hopic-1.60.0/hopic/test/docker-images/python/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1383 2020-08-27 06:38:21.000000 hopic-1.60.0/hopic/test/docker-images/python/Dockerfile
--rwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)      671 2020-08-13 10:49:20.000000 hopic-1.60.0/hopic/test/docker-images/python/ssh.sh
--rwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)     1325 2020-08-13 10:49:20.000000 hopic-1.60.0/hopic/test/docker-images/python/entrypoint.sh
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8150 2021-03-31 09:46:20.000000 hopic-1.60.0/hopic/test/test_approvals.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1298 2021-08-16 11:43:03.000000 hopic-1.60.0/hopic/test/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    54517 2022-08-05 08:34:03.000000 hopic-1.60.0/hopic/test/test_build.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8679 2021-08-17 09:13:44.000000 hopic-1.60.0/hopic/test/conftest.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    85299 2023-03-22 11:36:07.000000 hopic-1.60.0/hopic/test/test_merge.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11571 2022-07-28 12:30:27.000000 hopic-1.60.0/hopic/test/test_show_config.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      923 2020-08-29 06:53:11.000000 hopic-1.60.0/hopic/test/test_versioning.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       55 2023-04-03 07:25:31.000000 hopic-1.60.0/hopic/test/markers.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 07:40:05.000000 hopic-1.60.0/hopic/cli/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8214 2022-11-01 11:29:21.000000 hopic-1.60.0/hopic/cli/main.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4674 2021-12-23 16:07:43.000000 hopic-1.60.0/hopic/cli/global_obj.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    32740 2022-11-01 11:29:21.000000 hopic-1.60.0/hopic/cli/build.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3055 2021-08-16 11:43:03.000000 hopic-1.60.0/hopic/cli/utils.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    67193 2022-03-23 12:49:15.000000 hopic-1.60.0/hopic/cli/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6427 2021-08-16 11:43:03.000000 hopic-1.60.0/hopic/cli/extensions.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2889 2021-02-12 14:05:19.000000 hopic-1.60.0/hopic/cli/autocomplete.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 07:40:05.000000 hopic-1.60.0/hopic/template/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2919 2021-05-07 15:03:02.000000 hopic-1.60.0/hopic/template/utils.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2021-03-23 14:28:09.000000 hopic-1.60.0/hopic/template/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    71062 2023-03-23 08:27:04.000000 hopic-1.60.0/hopic/config_reader.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7240 2021-07-16 13:21:22.000000 hopic-1.60.0/hopic/build.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      946 2021-08-16 11:43:03.000000 hopic-1.60.0/hopic/compat.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    15611 2022-07-22 09:51:20.000000 hopic-1.60.0/hopic/binary_normalize.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3805 2021-06-10 12:40:43.000000 hopic-1.60.0/hopic/errors.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    23237 2021-12-23 16:07:43.000000 hopic-1.60.0/hopic/versioning.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2019-09-09 14:49:54.000000 hopic-1.60.0/hopic/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      725 2021-06-16 17:22:49.000000 hopic-1.60.0/hopic/types.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8331 2022-02-25 14:42:15.000000 hopic-1.60.0/hopic/git_time.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3316 2022-07-01 09:56:14.000000 hopic-1.60.0/hopic/execution.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      637 2020-09-30 09:14:13.000000 hopic-1.60.0/hopic/__main__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4759 2021-05-07 15:03:02.000000 hopic-1.60.0/hopic/credentials.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      455 2023-03-17 09:31:31.000000 hopic-1.60.0/pyproject.toml
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 07:40:05.000000 hopic-1.60.0/doc/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 07:40:05.000000 hopic-1.60.0/doc/source/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11086 2020-11-20 17:31:32.000000 hopic-1.60.0/doc/source/conf.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      378 2019-10-29 14:49:42.000000 hopic-1.60.0/doc/source/intro.rst
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    26379 2019-10-29 14:49:42.000000 hopic-1.60.0/doc/source/parallel-phases.svg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    37971 2023-03-22 14:23:47.000000 hopic-1.60.0/doc/source/changes.rst
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1097 2021-01-22 10:18:40.000000 hopic-1.60.0/doc/source/index.rst
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3855 2021-05-21 10:41:19.000000 hopic-1.60.0/doc/source/hotfix.rst
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    46784 2022-03-24 15:28:49.000000 hopic-1.60.0/doc/source/config.rst
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       77 2020-09-21 14:42:29.000000 hopic-1.60.0/doc/source/usage.rst
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8498 2020-10-27 10:52:16.000000 hopic-1.60.0/doc/source/CONTRIBUTING.md
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7693 2019-02-04 16:02:23.000000 hopic-1.60.0/doc/Makefile
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        7 2019-02-04 16:02:23.000000 hopic-1.60.0/doc/.gitignore
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       23 2018-09-11 09:38:00.000000 hopic-1.60.0/.git_archival.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      118 2019-01-17 16:44:37.000000 hopic-1.60.0/USAGE.md
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1359 2021-11-04 10:44:59.000000 hopic-1.60.0/permissions.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8498 2020-10-27 10:52:16.000000 hopic-1.60.0/CONTRIBUTING.md
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10757 2019-09-25 13:48:29.000000 hopic-1.60.0/LICENSE
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       93 2021-05-07 15:03:02.000000 hopic-1.60.0/.gitignore
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-22 07:41:46.000000 hopic-1.61.0/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1359 2021-11-04 10:44:59.000000 hopic-1.61.0/permissions.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      855 2019-01-04 15:25:30.000000 hopic-1.61.0/REQUIREMENTS.md
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-22 07:41:46.000000 hopic-1.61.0/.github/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-22 07:41:46.000000 hopic-1.61.0/.github/actions/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-22 07:41:46.000000 hopic-1.61.0/.github/actions/submit/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3387 2023-05-17 13:31:10.000000 hopic-1.61.0/.github/actions/submit/action.yaml
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-22 07:41:46.000000 hopic-1.61.0/.github/actions/checkout/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      908 2023-05-05 13:49:16.000000 hopic-1.61.0/.github/actions/checkout/hopic-version-dump.yaml
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9668 2023-05-17 13:31:10.000000 hopic-1.61.0/.github/actions/checkout/action.yaml
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      277 2021-11-15 13:30:02.000000 hopic-1.61.0/doc-requirements.txt
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-22 07:41:46.000000 hopic-1.61.0/vars/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5706 2021-05-11 08:24:17.000000 hopic-1.61.0/vars/printMetrics.groovy
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    84346 2023-03-24 13:43:41.000000 hopic-1.61.0/vars/getCiDriver.groovy
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-22 07:41:46.000000 hopic-1.61.0/doc/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7693 2019-02-04 16:02:23.000000 hopic-1.61.0/doc/Makefile
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-22 07:41:46.000000 hopic-1.61.0/doc/source/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1097 2021-01-22 10:18:40.000000 hopic-1.61.0/doc/source/index.rst
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3855 2021-05-21 10:41:19.000000 hopic-1.61.0/doc/source/hotfix.rst
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    46784 2022-03-24 15:28:49.000000 hopic-1.61.0/doc/source/config.rst
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      378 2019-10-29 14:49:42.000000 hopic-1.61.0/doc/source/intro.rst
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11086 2020-11-20 17:31:32.000000 hopic-1.61.0/doc/source/conf.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8498 2020-10-27 10:52:16.000000 hopic-1.61.0/doc/source/CONTRIBUTING.md
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       77 2020-09-21 14:42:29.000000 hopic-1.61.0/doc/source/usage.rst
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    37971 2023-03-22 14:23:47.000000 hopic-1.61.0/doc/source/changes.rst
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    26379 2019-10-29 14:49:42.000000 hopic-1.61.0/doc/source/parallel-phases.svg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        7 2019-02-04 16:02:23.000000 hopic-1.61.0/doc/.gitignore
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      118 2019-01-17 16:44:37.000000 hopic-1.61.0/USAGE.md
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      557 2021-05-07 15:03:02.000000 hopic-1.61.0/mypy.ini
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1728 2023-03-21 12:05:25.000000 hopic-1.61.0/tox.ini
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2189 2023-05-22 07:41:46.000000 hopic-1.61.0/PKG-INFO
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-22 07:41:46.000000 hopic-1.61.0/hopic/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      637 2020-09-30 09:14:13.000000 hopic-1.61.0/hopic/__main__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8331 2022-02-25 14:42:15.000000 hopic-1.61.0/hopic/git_time.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2019-09-09 14:49:54.000000 hopic-1.61.0/hopic/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-22 07:41:46.000000 hopic-1.61.0/hopic/template/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2021-03-23 14:28:09.000000 hopic-1.61.0/hopic/template/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2919 2021-05-07 15:03:02.000000 hopic-1.61.0/hopic/template/utils.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-22 07:41:46.000000 hopic-1.61.0/hopic/test/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1298 2021-08-16 11:43:03.000000 hopic-1.61.0/hopic/test/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    85299 2023-03-22 11:36:07.000000 hopic-1.61.0/hopic/test/test_merge.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3292 2021-04-28 11:03:59.000000 hopic-1.61.0/hopic/test/test_template_utils.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    12161 2023-03-22 11:36:07.000000 hopic-1.61.0/hopic/test/test_checkout.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7576 2021-05-21 10:41:19.000000 hopic-1.61.0/hopic/test/test_version_bump.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11571 2022-07-28 12:30:27.000000 hopic-1.61.0/hopic/test/test_show_config.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8150 2021-03-31 09:46:20.000000 hopic-1.61.0/hopic/test/test_approvals.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2332 2020-08-29 06:53:11.000000 hopic-1.61.0/hopic/test/test_credentials.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    54517 2022-08-05 08:34:03.000000 hopic-1.61.0/hopic/test/test_build.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      923 2020-08-29 06:53:11.000000 hopic-1.61.0/hopic/test/test_versioning.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      871 2021-07-09 16:01:55.000000 hopic-1.61.0/hopic/test/test_examples.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-22 07:41:46.000000 hopic-1.61.0/hopic/test/docker-images/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-22 07:41:46.000000 hopic-1.61.0/hopic/test/docker-images/python/
+-rwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)     1325 2020-08-13 10:49:20.000000 hopic-1.61.0/hopic/test/docker-images/python/entrypoint.sh
+-rwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)      671 2020-08-13 10:49:20.000000 hopic-1.61.0/hopic/test/docker-images/python/ssh.sh
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1383 2020-08-27 06:38:21.000000 hopic-1.61.0/hopic/test/docker-images/python/Dockerfile
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10668 2022-03-22 15:11:48.000000 hopic-1.61.0/hopic/test/test_getinfo.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    57112 2022-03-17 09:16:40.000000 hopic-1.61.0/hopic/test/test_config_reader.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2491 2021-05-21 10:41:19.000000 hopic-1.61.0/hopic/test/test_execution.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    26412 2022-02-01 16:50:00.000000 hopic-1.61.0/hopic/test/test_extensions.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8679 2021-08-17 09:13:44.000000 hopic-1.61.0/hopic/test/conftest.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       55 2023-05-22 07:40:54.000000 hopic-1.61.0/hopic/test/markers.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      725 2021-06-16 17:22:49.000000 hopic-1.61.0/hopic/types.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    15611 2022-07-22 09:51:20.000000 hopic-1.61.0/hopic/binary_normalize.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3805 2021-06-10 12:40:43.000000 hopic-1.61.0/hopic/errors.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3316 2022-07-01 09:56:14.000000 hopic-1.61.0/hopic/execution.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4759 2021-05-07 15:03:02.000000 hopic-1.61.0/hopic/credentials.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    23237 2021-12-23 16:07:43.000000 hopic-1.61.0/hopic/versioning.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      946 2021-08-16 11:43:03.000000 hopic-1.61.0/hopic/compat.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-22 07:41:46.000000 hopic-1.61.0/hopic/cli/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    67209 2023-05-05 13:49:16.000000 hopic-1.61.0/hopic/cli/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2889 2021-02-12 14:05:19.000000 hopic-1.61.0/hopic/cli/autocomplete.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6427 2021-08-16 11:43:03.000000 hopic-1.61.0/hopic/cli/extensions.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8214 2022-11-01 11:29:21.000000 hopic-1.61.0/hopic/cli/main.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4674 2021-12-23 16:07:43.000000 hopic-1.61.0/hopic/cli/global_obj.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3083 2023-05-17 13:31:10.000000 hopic-1.61.0/hopic/cli/utils.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    32740 2022-11-01 11:29:21.000000 hopic-1.61.0/hopic/cli/build.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    71062 2023-03-23 08:27:04.000000 hopic-1.61.0/hopic/config_reader.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7240 2021-07-16 13:21:22.000000 hopic-1.61.0/hopic/build.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      149 2021-02-19 11:08:41.000000 hopic-1.61.0/pytest.ini
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-05-22 07:41:46.000000 hopic-1.61.0/setup.cfg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       48 2019-11-11 15:31:32.000000 hopic-1.61.0/.gitattributes
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       23 2018-09-11 09:38:00.000000 hopic-1.61.0/.git_archival.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8498 2020-10-27 10:52:16.000000 hopic-1.61.0/CONTRIBUTING.md
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6351 2022-03-18 16:12:34.000000 hopic-1.61.0/hopic-ci-config.yaml
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2778 2023-03-17 09:31:31.000000 hopic-1.61.0/setup.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2260 2022-01-28 10:24:00.000000 hopic-1.61.0/Jenkinsfile
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-22 07:41:46.000000 hopic-1.61.0/examples/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      166 2020-09-14 14:10:55.000000 hopic-1.61.0/examples/pip.yaml
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      190 2021-06-09 12:02:18.000000 hopic-1.61.0/examples/timeout-variant.yaml
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      259 2021-01-21 19:52:27.000000 hopic-1.61.0/examples/docker-in-docker.yaml
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-22 07:41:46.000000 hopic-1.61.0/examples/embed/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      114 2020-05-15 09:48:27.000000 hopic-1.61.0/examples/embed/embed.yaml
+-rwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)      230 2020-08-27 06:38:21.000000 hopic-1.61.0/examples/embed/yaml-generation.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      131 2019-11-19 12:22:45.000000 hopic-1.61.0/examples/version-bump-constant.yaml
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      661 2019-11-07 14:38:21.000000 hopic-1.61.0/examples/upload-artifactory.yaml
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      473 2020-10-28 13:20:54.000000 hopic-1.61.0/examples/stash.yaml
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      930 2021-01-21 19:52:27.000000 hopic-1.61.0/examples/volumes-override.yaml
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      405 2021-06-09 10:59:19.000000 hopic-1.61.0/examples/timeout.yaml
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      151 2019-11-07 14:38:21.000000 hopic-1.61.0/examples/node-label.yaml
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      299 2020-11-30 14:08:37.000000 hopic-1.61.0/examples/ci-locks.yaml
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      139 2021-02-09 11:51:15.000000 hopic-1.61.0/examples/allow-missing-junit.yaml
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      452 2021-01-21 19:52:27.000000 hopic-1.61.0/examples/post-submit.yaml
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      338 2022-03-22 15:11:48.000000 hopic-1.61.0/examples/finally.yaml
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      205 2021-01-21 19:52:27.000000 hopic-1.61.0/examples/upload-on-fail.yaml
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      127 2021-02-09 11:51:15.000000 hopic-1.61.0/examples/allow-missing-archive.yaml
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      195 2019-11-07 14:38:21.000000 hopic-1.61.0/examples/junit.yaml
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      284 2021-01-21 19:52:27.000000 hopic-1.61.0/examples/version-bump-conventional.yaml
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      428 2019-11-05 15:44:39.000000 hopic-1.61.0/examples/with-volumes.yaml
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      823 2019-11-07 14:38:21.000000 hopic-1.61.0/examples/artifactory-promote.yaml
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      140 2021-10-06 13:00:51.000000 hopic-1.61.0/examples/allow-failures-junit.yaml
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      235 2020-08-19 12:54:41.000000 hopic-1.61.0/examples/with-keyring-credentials.yaml
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      337 2020-12-03 13:52:01.000000 hopic-1.61.0/examples/environment.yaml
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      302 2019-11-07 14:38:21.000000 hopic-1.61.0/examples/run-on-change.yaml
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1051 2020-12-04 14:21:57.000000 hopic-1.61.0/examples/with-credentials.yaml
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       59 2019-11-25 06:27:20.000000 hopic-1.61.0/examples/clean.yaml
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      283 2019-11-07 14:38:21.000000 hopic-1.61.0/examples/fingerprint.yaml
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      274 2020-01-10 14:03:05.000000 hopic-1.61.0/examples/image-mapping.yaml
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-22 07:41:46.000000 hopic-1.61.0/examples/simple/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      379 2019-01-04 14:47:49.000000 hopic-1.61.0/examples/simple/dependency_manifest.xml
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1839 2020-09-28 15:18:56.000000 hopic-1.61.0/examples/simple/Jenkinsfile
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2492 2021-01-21 19:52:27.000000 hopic-1.61.0/examples/simple/hopic-ci-config.yml
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      379 2019-01-04 14:47:49.000000 hopic-1.61.0/examples/dependency_manifest.xml
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       90 2020-08-12 13:05:54.000000 hopic-1.61.0/examples/disable-etc-volumes.yaml
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2545 2019-10-29 14:49:42.000000 hopic-1.61.0/examples/parallel-phases.yaml
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      515 2019-11-05 15:44:39.000000 hopic-1.61.0/examples/archive.yaml
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      192 2020-10-19 07:55:45.000000 hopic-1.61.0/examples/config.yaml
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      358 2021-01-22 15:16:09.000000 hopic-1.61.0/examples/docker-extra-args.yaml
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      367 2019-11-18 07:58:57.000000 hopic-1.61.0/examples/description.yaml
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      223 2019-11-05 15:44:39.000000 hopic-1.61.0/examples/image-ivy-manifest.yaml
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      188 2020-12-04 14:21:57.000000 hopic-1.61.0/examples/pass-through-env-vars.yaml
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1279 2020-08-21 14:01:27.000000 hopic-1.61.0/README.rst
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      455 2023-03-17 09:31:31.000000 hopic-1.61.0/pyproject.toml
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       93 2021-05-07 15:03:02.000000 hopic-1.61.0/.gitignore
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-22 07:41:46.000000 hopic-1.61.0/hopic.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3115 2023-05-22 07:41:46.000000 hopic-1.61.0/hopic.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        6 2023-05-22 07:41:46.000000 hopic-1.61.0/hopic.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-05-22 07:41:46.000000 hopic-1.61.0/hopic.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2189 2023-05-22 07:41:46.000000 hopic-1.61.0/hopic.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       61 2023-05-22 07:41:46.000000 hopic-1.61.0/hopic.egg-info/entry_points.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      291 2023-05-22 07:41:46.000000 hopic-1.61.0/hopic.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-05-22 07:41:46.000000 hopic-1.61.0/hopic.egg-info/zip-safe
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-22 07:41:46.000000 hopic-1.61.0/src/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-22 07:41:46.000000 hopic-1.61.0/src/com/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-22 07:41:46.000000 hopic-1.61.0/src/com/tomtom/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-22 07:41:46.000000 hopic-1.61.0/src/com/tomtom/hopic/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6753 2022-06-14 09:15:10.000000 hopic-1.61.0/src/com/tomtom/hopic/HopicEventCallbacks.groovy
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10757 2019-09-25 13:48:29.000000 hopic-1.61.0/LICENSE
```

### Comparing `hopic-1.60.0/hopic-ci-config.yaml` & `hopic-1.61.0/hopic-ci-config.yaml`

 * *Files identical despite different names*

### Comparing `hopic-1.60.0/tox.ini` & `hopic-1.61.0/tox.ini`

 * *Files identical despite different names*

### Comparing `hopic-1.60.0/vars/printMetrics.groovy` & `hopic-1.61.0/vars/printMetrics.groovy`

 * *Files identical despite different names*

### Comparing `hopic-1.60.0/vars/getCiDriver.groovy` & `hopic-1.61.0/vars/getCiDriver.groovy`

 * *Files identical despite different names*

### Comparing `hopic-1.60.0/src/com/tomtom/hopic/HopicEventCallbacks.groovy` & `hopic-1.61.0/src/com/tomtom/hopic/HopicEventCallbacks.groovy`

 * *Files identical despite different names*

### Comparing `hopic-1.60.0/REQUIREMENTS.md` & `hopic-1.61.0/REQUIREMENTS.md`

 * *Files identical despite different names*

### Comparing `hopic-1.60.0/Jenkinsfile` & `hopic-1.61.0/Jenkinsfile`

 * *Files identical despite different names*

### Comparing `hopic-1.60.0/mypy.ini` & `hopic-1.61.0/mypy.ini`

 * *Files identical despite different names*

### Comparing `hopic-1.60.0/examples/parallel-phases.yaml` & `hopic-1.61.0/examples/parallel-phases.yaml`

 * *Files identical despite different names*

### Comparing `hopic-1.60.0/examples/artifactory-promote.yaml` & `hopic-1.61.0/examples/artifactory-promote.yaml`

 * *Files identical despite different names*

### Comparing `hopic-1.60.0/examples/upload-artifactory.yaml` & `hopic-1.61.0/examples/upload-artifactory.yaml`

 * *Files identical despite different names*

### Comparing `hopic-1.60.0/examples/simple/Jenkinsfile` & `hopic-1.61.0/examples/simple/Jenkinsfile`

 * *Files identical despite different names*

### Comparing `hopic-1.60.0/examples/simple/hopic-ci-config.yml` & `hopic-1.61.0/examples/simple/hopic-ci-config.yml`

 * *Files identical despite different names*

### Comparing `hopic-1.60.0/examples/volumes-override.yaml` & `hopic-1.61.0/examples/volumes-override.yaml`

 * *Files identical despite different names*

### Comparing `hopic-1.60.0/examples/archive.yaml` & `hopic-1.61.0/examples/archive.yaml`

 * *Files identical despite different names*

### Comparing `hopic-1.60.0/examples/with-credentials.yaml` & `hopic-1.61.0/examples/with-credentials.yaml`

 * *Files identical despite different names*

### Comparing `hopic-1.60.0/README.rst` & `hopic-1.61.0/README.rst`

 * *Files identical despite different names*

### Comparing `hopic-1.60.0/PKG-INFO` & `hopic-1.61.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hopic
-Version: 1.60.0
+Version: 1.61.0
 Summary: In order to simplify the CI configuration we are switching away from the generic jenkins shared pipeline which is completely written in Groovy. Instead we are switching to the Hopic project which only has a minimal CI driver component written in Groovy with the rest written in Python. With Hopic local debugging is made significantly easier.
 Home-page: https://github.com/tomtom-international/hopic
 Author: TomTom N.V.
 License: Apache License 2.0
 Project-URL: Documentation, https://tomtom-international.github.io/hopic/
 Project-URL: Change Log, https://tomtom-international.github.io/hopic/changes.html
 Project-URL: Source Code, https://github.com/tomtom-international/hopic
```

### Comparing `hopic-1.60.0/setup.py` & `hopic-1.61.0/setup.py`

 * *Files identical despite different names*

### Comparing `hopic-1.60.0/hopic.egg-info/SOURCES.txt` & `hopic-1.61.0/hopic.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -11,14 +11,17 @@
 hopic-ci-config.yaml
 mypy.ini
 permissions.txt
 pyproject.toml
 pytest.ini
 setup.py
 tox.ini
+.github/actions/checkout/action.yaml
+.github/actions/checkout/hopic-version-dump.yaml
+.github/actions/submit/action.yaml
 doc/.gitignore
 doc/Makefile
 doc/source/CONTRIBUTING.md
 doc/source/changes.rst
 doc/source/conf.py
 doc/source/config.rst
 doc/source/hotfix.rst
```

### Comparing `hopic-1.60.0/hopic.egg-info/PKG-INFO` & `hopic-1.61.0/hopic.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hopic
-Version: 1.60.0
+Version: 1.61.0
 Summary: In order to simplify the CI configuration we are switching away from the generic jenkins shared pipeline which is completely written in Groovy. Instead we are switching to the Hopic project which only has a minimal CI driver component written in Groovy with the rest written in Python. With Hopic local debugging is made significantly easier.
 Home-page: https://github.com/tomtom-international/hopic
 Author: TomTom N.V.
 License: Apache License 2.0
 Project-URL: Documentation, https://tomtom-international.github.io/hopic/
 Project-URL: Change Log, https://tomtom-international.github.io/hopic/changes.html
 Project-URL: Source Code, https://github.com/tomtom-international/hopic
```

### Comparing `hopic-1.60.0/hopic/test/test_credentials.py` & `hopic-1.61.0/hopic/test/test_credentials.py`

 * *Files identical despite different names*

### Comparing `hopic-1.60.0/hopic/test/test_template_utils.py` & `hopic-1.61.0/hopic/test/test_template_utils.py`

 * *Files identical despite different names*

### Comparing `hopic-1.60.0/hopic/test/test_config_reader.py` & `hopic-1.61.0/hopic/test/test_config_reader.py`

 * *Files identical despite different names*

### Comparing `hopic-1.60.0/hopic/test/test_version_bump.py` & `hopic-1.61.0/hopic/test/test_version_bump.py`

 * *Files identical despite different names*

### Comparing `hopic-1.60.0/hopic/test/test_checkout.py` & `hopic-1.61.0/hopic/test/test_checkout.py`

 * *Files identical despite different names*

### Comparing `hopic-1.60.0/hopic/test/test_execution.py` & `hopic-1.61.0/hopic/test/test_execution.py`

 * *Files identical despite different names*

### Comparing `hopic-1.60.0/hopic/test/test_extensions.py` & `hopic-1.61.0/hopic/test/test_extensions.py`

 * *Files identical despite different names*

### Comparing `hopic-1.60.0/hopic/test/test_getinfo.py` & `hopic-1.61.0/hopic/test/test_getinfo.py`

 * *Files identical despite different names*

### Comparing `hopic-1.60.0/hopic/test/test_examples.py` & `hopic-1.61.0/hopic/test/test_examples.py`

 * *Files identical despite different names*

### Comparing `hopic-1.60.0/hopic/test/docker-images/python/Dockerfile` & `hopic-1.61.0/hopic/test/docker-images/python/Dockerfile`

 * *Files identical despite different names*

### Comparing `hopic-1.60.0/hopic/test/docker-images/python/ssh.sh` & `hopic-1.61.0/hopic/test/docker-images/python/ssh.sh`

 * *Files identical despite different names*

### Comparing `hopic-1.60.0/hopic/test/docker-images/python/entrypoint.sh` & `hopic-1.61.0/hopic/test/docker-images/python/entrypoint.sh`

 * *Files identical despite different names*

### Comparing `hopic-1.60.0/hopic/test/test_approvals.py` & `hopic-1.61.0/hopic/test/test_approvals.py`

 * *Files identical despite different names*

### Comparing `hopic-1.60.0/hopic/test/__init__.py` & `hopic-1.61.0/hopic/test/__init__.py`

 * *Files identical despite different names*

### Comparing `hopic-1.60.0/hopic/test/test_build.py` & `hopic-1.61.0/hopic/test/test_build.py`

 * *Files identical despite different names*

### Comparing `hopic-1.60.0/hopic/test/conftest.py` & `hopic-1.61.0/hopic/test/conftest.py`

 * *Files identical despite different names*

### Comparing `hopic-1.60.0/hopic/test/test_merge.py` & `hopic-1.61.0/hopic/test/test_merge.py`

 * *Files identical despite different names*

### Comparing `hopic-1.60.0/hopic/test/test_show_config.py` & `hopic-1.61.0/hopic/test/test_show_config.py`

 * *Files identical despite different names*

### Comparing `hopic-1.60.0/hopic/test/test_versioning.py` & `hopic-1.61.0/hopic/test/test_versioning.py`

 * *Files identical despite different names*

### Comparing `hopic-1.60.0/hopic/cli/main.py` & `hopic-1.61.0/hopic/cli/main.py`

 * *Files identical despite different names*

### Comparing `hopic-1.60.0/hopic/cli/global_obj.py` & `hopic-1.61.0/hopic/cli/global_obj.py`

 * *Files identical despite different names*

### Comparing `hopic-1.60.0/hopic/cli/build.py` & `hopic-1.61.0/hopic/cli/build.py`

 * *Files identical despite different names*

### Comparing `hopic-1.60.0/hopic/cli/utils.py` & `hopic-1.61.0/hopic/cli/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 
     try:
         publish_from_branch = ctx.obj.config['publish-from-branch']
     except KeyError:
         return True
 
     publish_branch_pattern = re.compile(f"(?:{publish_from_branch})$")
-    return publish_branch_pattern.match(hopic_git_info.submit_ref) is not None
+    return publish_branch_pattern.match(re.sub("^refs/heads/", "", hopic_git_info.submit_ref)) is not None
 
 
 def determine_config_file_name(ctx, workspace: Optional[Path] = None):
     """
     Determines the location of the config file, possibly falling back to a default.
     """
     try:
```

### Comparing `hopic-1.60.0/hopic/cli/__init__.py` & `hopic-1.61.0/hopic/cli/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1477,16 +1477,16 @@
             if code_fresh:
                 # Only restore mtimes when doing a clean build or working on a fresh clone. This prevents problems with timestamp-based build sytems.
                 # I.e. make and ninja and probably half the world.
                 restore_mtime_from_git(repo)
         git_cfg = ctx.obj.config["scm"]["git"]
     except (click.BadParameter, KeyError, TypeError, OSError, IOError, YAMLError):
         return
-
-    log.info("%s", repo.git.show(submit_commit, format="fuller", stat=True, notes="*"))
+    finally:
+        log.info("%s", repo.git.show(submit_commit, format="fuller", stat=True, notes="*"))
 
     checkout_worktrees(workspace, git_cfg["worktrees"])
 
     if "remote" not in git_cfg and "ref" not in git_cfg:
         return
 
     code_dir = find_code_dir(workspace)
```

### Comparing `hopic-1.60.0/hopic/cli/extensions.py` & `hopic-1.61.0/hopic/cli/extensions.py`

 * *Files identical despite different names*

### Comparing `hopic-1.60.0/hopic/cli/autocomplete.py` & `hopic-1.61.0/hopic/cli/autocomplete.py`

 * *Files identical despite different names*

### Comparing `hopic-1.60.0/hopic/template/utils.py` & `hopic-1.61.0/hopic/template/utils.py`

 * *Files identical despite different names*

### Comparing `hopic-1.60.0/hopic/config_reader.py` & `hopic-1.61.0/hopic/config_reader.py`

 * *Files identical despite different names*

### Comparing `hopic-1.60.0/hopic/build.py` & `hopic-1.61.0/hopic/build.py`

 * *Files identical despite different names*

### Comparing `hopic-1.60.0/hopic/compat.py` & `hopic-1.61.0/hopic/compat.py`

 * *Files identical despite different names*

### Comparing `hopic-1.60.0/hopic/binary_normalize.py` & `hopic-1.61.0/hopic/binary_normalize.py`

 * *Files identical despite different names*

### Comparing `hopic-1.60.0/hopic/errors.py` & `hopic-1.61.0/hopic/errors.py`

 * *Files identical despite different names*

### Comparing `hopic-1.60.0/hopic/versioning.py` & `hopic-1.61.0/hopic/versioning.py`

 * *Files identical despite different names*

### Comparing `hopic-1.60.0/hopic/types.py` & `hopic-1.61.0/hopic/types.py`

 * *Files identical despite different names*

### Comparing `hopic-1.60.0/hopic/git_time.py` & `hopic-1.61.0/hopic/git_time.py`

 * *Files identical despite different names*

### Comparing `hopic-1.60.0/hopic/execution.py` & `hopic-1.61.0/hopic/execution.py`

 * *Files identical despite different names*

### Comparing `hopic-1.60.0/hopic/__main__.py` & `hopic-1.61.0/hopic/__main__.py`

 * *Files identical despite different names*

### Comparing `hopic-1.60.0/hopic/credentials.py` & `hopic-1.61.0/hopic/credentials.py`

 * *Files identical despite different names*

### Comparing `hopic-1.60.0/doc/source/conf.py` & `hopic-1.61.0/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `hopic-1.60.0/doc/source/parallel-phases.svg` & `hopic-1.61.0/doc/source/parallel-phases.svg`

 * *Files identical despite different names*

### Comparing `hopic-1.60.0/doc/source/changes.rst` & `hopic-1.61.0/doc/source/changes.rst`

 * *Files identical despite different names*

### Comparing `hopic-1.60.0/doc/source/index.rst` & `hopic-1.61.0/doc/source/index.rst`

 * *Files identical despite different names*

### Comparing `hopic-1.60.0/doc/source/hotfix.rst` & `hopic-1.61.0/doc/source/hotfix.rst`

 * *Files identical despite different names*

### Comparing `hopic-1.60.0/doc/source/config.rst` & `hopic-1.61.0/doc/source/config.rst`

 * *Files identical despite different names*

### Comparing `hopic-1.60.0/doc/source/CONTRIBUTING.md` & `hopic-1.61.0/doc/source/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `hopic-1.60.0/doc/Makefile` & `hopic-1.61.0/doc/Makefile`

 * *Files identical despite different names*

### Comparing `hopic-1.60.0/permissions.txt` & `hopic-1.61.0/permissions.txt`

 * *Files identical despite different names*

### Comparing `hopic-1.60.0/CONTRIBUTING.md` & `hopic-1.61.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `hopic-1.60.0/LICENSE` & `hopic-1.61.0/LICENSE`

 * *Files identical despite different names*

