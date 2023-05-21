# Comparing `tmp/vbcore-1.3.0rc3.tar.gz` & `tmp/vbcore-2.0.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vbcore-1.3.0rc3.tar", last modified: Sat Nov 26 18:58:16 2022, max compression
+gzip compressed data, was "vbcore-2.0.0rc2.tar", last modified: Sun May 21 22:10:47 2023, max compression
```

## Comparing `vbcore-1.3.0rc3.tar` & `vbcore-2.0.0rc2.tar`

### file list

```diff
@@ -1,121 +1,142 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-26 18:58:16.041307 vbcore-1.3.0rc3/
--rw-rw-rw-   0 root         (0) root         (0)       23 2022-11-26 18:58:03.000000 vbcore-1.3.0rc3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      390 2022-11-26 18:58:16.041307 vbcore-1.3.0rc3/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      273 2022-11-26 18:58:03.000000 vbcore-1.3.0rc3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-26 18:58:16.017305 vbcore-1.3.0rc3/requirements/
--rw-rw-rw-   0 root         (0) root         (0)      209 2022-11-26 18:58:03.000000 vbcore-1.3.0rc3/requirements/requirements-all.in
--rw-rw-rw-   0 root         (0) root         (0)     3650 2022-11-26 18:58:03.000000 vbcore-1.3.0rc3/requirements/requirements-all.txt
--rw-rw-rw-   0 root         (0) root         (0)       37 2022-11-26 18:58:03.000000 vbcore-1.3.0rc3/requirements/requirements-build.in
--rw-rw-rw-   0 root         (0) root         (0)     2067 2022-11-26 18:58:03.000000 vbcore-1.3.0rc3/requirements/requirements-build.txt
--rw-rw-rw-   0 root         (0) root         (0)       37 2022-11-26 18:58:03.000000 vbcore-1.3.0rc3/requirements/requirements-crypto.in
--rw-rw-rw-   0 root         (0) root         (0)      638 2022-11-26 18:58:03.000000 vbcore-1.3.0rc3/requirements/requirements-crypto.txt
--rw-rw-rw-   0 root         (0) root         (0)       61 2022-11-26 18:58:03.000000 vbcore-1.3.0rc3/requirements/requirements-db.in
--rw-rw-rw-   0 root         (0) root         (0)      842 2022-11-26 18:58:03.000000 vbcore-1.3.0rc3/requirements/requirements-db.txt
--rw-rw-rw-   0 root         (0) root         (0)      323 2022-11-26 18:58:03.000000 vbcore-1.3.0rc3/requirements/requirements-dev.in
--rw-rw-rw-   0 root         (0) root         (0)     4464 2022-11-26 18:58:03.000000 vbcore-1.3.0rc3/requirements/requirements-dev.txt
--rw-rw-rw-   0 root         (0) root         (0)       56 2022-11-26 18:58:03.000000 vbcore-1.3.0rc3/requirements/requirements-extra.in
--rw-rw-rw-   0 root         (0) root         (0)     1340 2022-11-26 18:58:03.000000 vbcore-1.3.0rc3/requirements/requirements-extra.txt
--rw-rw-rw-   0 root         (0) root         (0)       54 2022-11-26 18:58:03.000000 vbcore-1.3.0rc3/requirements/requirements-http.in
--rw-rw-rw-   0 root         (0) root         (0)     1616 2022-11-26 18:58:03.000000 vbcore-1.3.0rc3/requirements/requirements-http.txt
--rw-rw-rw-   0 root         (0) root         (0)       54 2022-11-26 18:58:03.000000 vbcore-1.3.0rc3/requirements/requirements-net.in
--rw-rw-rw-   0 root         (0) root         (0)      912 2022-11-26 18:58:03.000000 vbcore-1.3.0rc3/requirements/requirements-net.txt
--rw-rw-rw-   0 root         (0) root         (0)       37 2022-11-26 18:58:03.000000 vbcore-1.3.0rc3/requirements/requirements-scheduler.in
--rw-rw-rw-   0 root         (0) root         (0)     1073 2022-11-26 18:58:03.000000 vbcore-1.3.0rc3/requirements/requirements-scheduler.txt
--rw-rw-rw-   0 root         (0) root         (0)       73 2022-11-26 18:58:03.000000 vbcore-1.3.0rc3/requirements/requirements-test.in
--rw-rw-rw-   0 root         (0) root         (0)     1612 2022-11-26 18:58:03.000000 vbcore-1.3.0rc3/requirements/requirements-test.txt
--rw-rw-rw-   0 root         (0) root         (0)      146 2022-11-26 18:58:03.000000 vbcore-1.3.0rc3/requirements/requirements.in
--rw-rw-rw-   0 root         (0) root         (0)      835 2022-11-26 18:58:03.000000 vbcore-1.3.0rc3/requirements/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2022-11-26 18:58:16.042307 vbcore-1.3.0rc3/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     4789 2022-11-26 18:58:03.000000 vbcore-1.3.0rc3/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-26 18:58:16.023305 vbcore-1.3.0rc3/vbcore/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-11-26 18:58:03.000000 vbcore-1.3.0rc3/vbcore/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       49 2022-11-26 18:58:03.000000 vbcore-1.3.0rc3/vbcore/__main__.py
--rw-rw-rw-   0 root         (0) root         (0)     2566 2022-11-26 18:58:03.000000 vbcore-1.3.0rc3/vbcore/base.py
--rw-rw-rw-   0 root         (0) root         (0)     8265 2022-11-26 18:58:03.000000 vbcore-1.3.0rc3/vbcore/batch.py
--rw-rw-rw-   0 root         (0) root         (0)     1484 2022-11-26 18:58:03.000000 vbcore-1.3.0rc3/vbcore/configurator.py
--rw-rw-rw-   0 root         (0) root         (0)     7979 2022-11-26 18:58:03.000000 vbcore-1.3.0rc3/vbcore/crc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-26 18:58:16.026306 vbcore-1.3.0rc3/vbcore/crypto/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-11-26 18:58:03.000000 vbcore-1.3.0rc3/vbcore/crypto/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      586 2022-11-26 18:58:03.000000 vbcore-1.3.0rc3/vbcore/crypto/argon.py
--rw-rw-rw-   0 root         (0) root         (0)      226 2022-11-26 18:58:03.000000 vbcore-1.3.0rc3/vbcore/crypto/base.py
--rw-rw-rw-   0 root         (0) root         (0)     3250 2022-11-26 18:58:03.000000 vbcore-1.3.0rc3/vbcore/csvfile.py
--rw-rw-rw-   0 root         (0) root         (0)    13267 2022-11-26 18:58:03.000000 vbcore-1.3.0rc3/vbcore/datastruct.py
--rw-rw-rw-   0 root         (0) root         (0)     4458 2022-11-26 18:58:03.000000 vbcore-1.3.0rc3/vbcore/date_helper.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-26 18:58:16.029306 vbcore-1.3.0rc3/vbcore/db/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-11-26 18:58:03.000000 vbcore-1.3.0rc3/vbcore/db/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    20852 2022-11-26 18:58:03.000000 vbcore-1.3.0rc3/vbcore/db/events.py
--rw-rw-rw-   0 root         (0) root         (0)     6557 2022-11-26 18:58:03.000000 vbcore-1.3.0rc3/vbcore/db/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)     1966 2022-11-26 18:58:03.000000 vbcore-1.3.0rc3/vbcore/db/mixins.py
--rw-rw-rw-   0 root         (0) root         (0)     6899 2022-11-26 18:58:03.000000 vbcore-1.3.0rc3/vbcore/db/mysql_dumper.py
--rw-rw-rw-   0 root         (0) root         (0)     1802 2022-11-26 18:58:03.000000 vbcore-1.3.0rc3/vbcore/db/schema.py
--rw-rw-rw-   0 root         (0) root         (0)     3687 2022-11-26 18:58:03.000000 vbcore-1.3.0rc3/vbcore/db/sqla.py
--rw-rw-rw-   0 root         (0) root         (0)     5267 2022-11-26 18:58:03.000000 vbcore-1.3.0rc3/vbcore/db/support.py
--rw-rw-rw-   0 root         (0) root         (0)     3716 2022-11-26 18:58:03.000000 vbcore-1.3.0rc3/vbcore/files.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-26 18:58:16.032306 vbcore-1.3.0rc3/vbcore/http/
--rw-rw-rw-   0 root         (0) root         (0)       69 2022-11-26 18:58:03.000000 vbcore-1.3.0rc3/vbcore/http/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3008 2022-11-26 18:58:03.000000 vbcore-1.3.0rc3/vbcore/http/batch.py
--rw-rw-rw-   0 root         (0) root         (0)     7848 2022-11-26 18:58:03.000000 vbcore-1.3.0rc3/vbcore/http/client.py
--rw-rw-rw-   0 root         (0) root         (0)     3238 2022-11-26 18:58:03.000000 vbcore-1.3.0rc3/vbcore/http/headers.py
--rw-rw-rw-   0 root         (0) root         (0)     2632 2022-11-26 18:58:03.000000 vbcore-1.3.0rc3/vbcore/http/httpcode.py
--rw-rw-rw-   0 root         (0) root         (0)     4009 2022-11-26 18:58:03.000000 vbcore-1.3.0rc3/vbcore/http/httpdumper.py
--rw-rw-rw-   0 root         (0) root         (0)      450 2022-11-26 18:58:03.000000 vbcore-1.3.0rc3/vbcore/http/methods.py
--rw-rw-rw-   0 root         (0) root         (0)     5946 2022-11-26 18:58:03.000000 vbcore-1.3.0rc3/vbcore/http/proxy.py
--rw-rw-rw-   0 root         (0) root         (0)     1850 2022-11-26 18:58:03.000000 vbcore-1.3.0rc3/vbcore/http/rpc.py
--rw-rw-rw-   0 root         (0) root         (0)     2194 2022-11-26 18:58:03.000000 vbcore-1.3.0rc3/vbcore/http/useragent.py
--rw-rw-rw-   0 root         (0) root         (0)     4484 2022-11-26 18:58:03.000000 vbcore-1.3.0rc3/vbcore/importer.py
--rw-rw-rw-   0 root         (0) root         (0)     4805 2022-11-26 18:58:03.000000 vbcore-1.3.0rc3/vbcore/json.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-26 18:58:16.032306 vbcore-1.3.0rc3/vbcore/jsonschema/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-11-26 18:58:03.000000 vbcore-1.3.0rc3/vbcore/jsonschema/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-26 18:58:16.033306 vbcore-1.3.0rc3/vbcore/jsonschema/schemas/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-11-26 18:58:03.000000 vbcore-1.3.0rc3/vbcore/jsonschema/schemas/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2146 2022-11-26 18:58:03.000000 vbcore-1.3.0rc3/vbcore/jsonschema/schemas/jsonrpc.py
--rw-rw-rw-   0 root         (0) root         (0)     6778 2022-11-26 18:58:03.000000 vbcore-1.3.0rc3/vbcore/jsonschema/support.py
--rw-rw-rw-   0 root         (0) root         (0)     3958 2022-11-26 18:58:03.000000 vbcore-1.3.0rc3/vbcore/loggers.py
--rw-rw-rw-   0 root         (0) root         (0)     4770 2022-11-26 18:58:03.000000 vbcore-1.3.0rc3/vbcore/misc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-26 18:58:16.034306 vbcore-1.3.0rc3/vbcore/net/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-11-26 18:58:03.000000 vbcore-1.3.0rc3/vbcore/net/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1827 2022-11-26 18:58:03.000000 vbcore-1.3.0rc3/vbcore/net/helpers.py
--rw-rw-rw-   0 root         (0) root         (0)     5818 2022-11-26 18:58:03.000000 vbcore-1.3.0rc3/vbcore/net/sendmail.py
--rw-rw-rw-   0 root         (0) root         (0)     3522 2022-11-26 18:58:03.000000 vbcore-1.3.0rc3/vbcore/net/sftp.py
--rw-rw-rw-   0 root         (0) root         (0)     1250 2022-11-26 18:58:03.000000 vbcore-1.3.0rc3/vbcore/net/socks_smtp.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-26 18:58:16.035306 vbcore-1.3.0rc3/vbcore/rule_engine/
--rw-rw-rw-   0 root         (0) root         (0)      106 2022-11-26 18:58:03.000000 vbcore-1.3.0rc3/vbcore/rule_engine/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1256 2022-11-26 18:58:03.000000 vbcore-1.3.0rc3/vbcore/rule_engine/base.py
--rw-rw-rw-   0 root         (0) root         (0)     3214 2022-11-26 18:58:03.000000 vbcore-1.3.0rc3/vbcore/rule_engine/engine.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-26 18:58:16.036306 vbcore-1.3.0rc3/vbcore/standalone/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-11-26 18:58:03.000000 vbcore-1.3.0rc3/vbcore/standalone/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3330 2022-11-26 18:58:03.000000 vbcore-1.3.0rc3/vbcore/standalone/scheduler.py
--rw-rw-rw-   0 root         (0) root         (0)     9034 2022-11-26 18:58:03.000000 vbcore-1.3.0rc3/vbcore/standalone/wsgi_gunicorn.py
--rw-rw-rw-   0 root         (0) root         (0)     4506 2022-11-26 18:58:03.000000 vbcore-1.3.0rc3/vbcore/system.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-26 18:58:16.038306 vbcore-1.3.0rc3/vbcore/tester/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-11-26 18:58:03.000000 vbcore-1.3.0rc3/vbcore/tester/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      346 2022-11-26 18:58:03.000000 vbcore-1.3.0rc3/vbcore/tester/cli.py
--rw-rw-rw-   0 root         (0) root         (0)     1455 2022-11-26 18:58:03.000000 vbcore-1.3.0rc3/vbcore/tester/fetchmail.py
--rw-rw-rw-   0 root         (0) root         (0)      785 2022-11-26 18:58:03.000000 vbcore-1.3.0rc3/vbcore/tester/helpers.py
--rw-rw-rw-   0 root         (0) root         (0)     7402 2022-11-26 18:58:03.000000 vbcore-1.3.0rc3/vbcore/tester/http.py
--rw-rw-rw-   0 root         (0) root         (0)    12006 2022-11-26 18:58:03.000000 vbcore-1.3.0rc3/vbcore/tester/mixins.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-26 18:58:16.039306 vbcore-1.3.0rc3/vbcore/tester/plugins/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-11-26 18:58:03.000000 vbcore-1.3.0rc3/vbcore/tester/plugins/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      163 2022-11-26 18:58:03.000000 vbcore-1.3.0rc3/vbcore/tester/plugins/fixtures.py
--rw-rw-rw-   0 root         (0) root         (0)      438 2022-11-26 18:58:03.000000 vbcore-1.3.0rc3/vbcore/tester/plugins/startup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-26 18:58:16.040306 vbcore-1.3.0rc3/vbcore/tools/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-11-26 18:58:03.000000 vbcore-1.3.0rc3/vbcore/tools/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5902 2022-11-26 18:58:03.000000 vbcore-1.3.0rc3/vbcore/tools/cli.py
--rw-rw-rw-   0 root         (0) root         (0)      977 2022-11-26 18:58:03.000000 vbcore-1.3.0rc3/vbcore/tools/crypto.py
--rw-rw-rw-   0 root         (0) root         (0)     2207 2022-11-26 18:58:03.000000 vbcore-1.3.0rc3/vbcore/tools/database.py
--rw-rw-rw-   0 root         (0) root         (0)      699 2022-11-26 18:58:03.000000 vbcore-1.3.0rc3/vbcore/tools/entrypoint.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-26 18:58:16.041307 vbcore-1.3.0rc3/vbcore/tools/initializer/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-11-26 18:58:03.000000 vbcore-1.3.0rc3/vbcore/tools/initializer/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1104 2022-11-26 18:58:03.000000 vbcore-1.3.0rc3/vbcore/tools/initializer/init.py
--rw-rw-rw-   0 root         (0) root         (0)      745 2022-11-26 18:58:03.000000 vbcore-1.3.0rc3/vbcore/tools/scheduler.py
--rw-rw-rw-   0 root         (0) root         (0)     1023 2022-11-26 18:58:03.000000 vbcore-1.3.0rc3/vbcore/uuid.py
--rw-rw-rw-   0 root         (0) root         (0)      256 2022-11-26 18:58:03.000000 vbcore-1.3.0rc3/vbcore/version.py
--rw-rw-rw-   0 root         (0) root         (0)     2868 2022-11-26 18:58:03.000000 vbcore-1.3.0rc3/vbcore/yaml.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-26 18:58:16.025305 vbcore-1.3.0rc3/vbcore.egg-info/
--rw-r--r--   0 root         (0) root         (0)      390 2022-11-26 18:58:15.000000 vbcore-1.3.0rc3/vbcore.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2674 2022-11-26 18:58:15.000000 vbcore-1.3.0rc3/vbcore.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-11-26 18:58:15.000000 vbcore-1.3.0rc3/vbcore.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       57 2022-11-26 18:58:15.000000 vbcore-1.3.0rc3/vbcore.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-11-26 18:58:15.000000 vbcore-1.3.0rc3/vbcore.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      623 2022-11-26 18:58:15.000000 vbcore-1.3.0rc3/vbcore.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2022-11-26 18:58:15.000000 vbcore-1.3.0rc3/vbcore.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 22:10:47.949563 vbcore-2.0.0rc2/
+-rw-rw-rw-   0 root         (0) root         (0)       60 2023-05-21 22:10:36.000000 vbcore-2.0.0rc2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      402 2023-05-21 22:10:47.949563 vbcore-2.0.0rc2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      273 2023-05-21 22:10:36.000000 vbcore-2.0.0rc2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 22:10:47.936563 vbcore-2.0.0rc2/requirements/
+-rw-rw-rw-   0 root         (0) root         (0)      222 2023-05-21 22:10:36.000000 vbcore-2.0.0rc2/requirements/requirements-all.in
+-rw-rw-rw-   0 root         (0) root         (0)     5938 2023-05-21 22:10:36.000000 vbcore-2.0.0rc2/requirements/requirements-all.txt
+-rw-rw-rw-   0 root         (0) root         (0)      245 2023-05-21 22:10:36.000000 vbcore-2.0.0rc2/requirements/requirements-build.in
+-rw-rw-rw-   0 root         (0) root         (0)     2068 2023-05-21 22:10:36.000000 vbcore-2.0.0rc2/requirements/requirements-build.txt
+-rw-rw-rw-   0 root         (0) root         (0)       59 2023-05-21 22:10:36.000000 vbcore-2.0.0rc2/requirements/requirements-crypto.in
+-rw-rw-rw-   0 root         (0) root         (0)      547 2023-05-21 22:10:36.000000 vbcore-2.0.0rc2/requirements/requirements-crypto.txt
+-rw-rw-rw-   0 root         (0) root         (0)       85 2023-05-21 22:10:36.000000 vbcore-2.0.0rc2/requirements/requirements-db.in
+-rw-rw-rw-   0 root         (0) root         (0)      582 2023-05-21 22:10:36.000000 vbcore-2.0.0rc2/requirements/requirements-db.txt
+-rw-rw-rw-   0 root         (0) root         (0)      410 2023-05-21 22:10:36.000000 vbcore-2.0.0rc2/requirements/requirements-dev.in
+-rw-rw-rw-   0 root         (0) root         (0)     6394 2023-05-21 22:10:36.000000 vbcore-2.0.0rc2/requirements/requirements-dev.txt
+-rw-rw-rw-   0 root         (0) root         (0)       91 2023-05-21 22:10:36.000000 vbcore-2.0.0rc2/requirements/requirements-extra.in
+-rw-rw-rw-   0 root         (0) root         (0)     1243 2023-05-21 22:10:36.000000 vbcore-2.0.0rc2/requirements/requirements-extra.txt
+-rw-rw-rw-   0 root         (0) root         (0)       76 2023-05-21 22:10:36.000000 vbcore-2.0.0rc2/requirements/requirements-http.in
+-rw-rw-rw-   0 root         (0) root         (0)     1173 2023-05-21 22:10:36.000000 vbcore-2.0.0rc2/requirements/requirements-http.txt
+-rw-rw-rw-   0 root         (0) root         (0)       80 2023-05-21 22:10:36.000000 vbcore-2.0.0rc2/requirements/requirements-net.in
+-rw-rw-rw-   0 root         (0) root         (0)      921 2023-05-21 22:10:36.000000 vbcore-2.0.0rc2/requirements/requirements-net.txt
+-rw-rw-rw-   0 root         (0) root         (0)       59 2023-05-21 22:10:36.000000 vbcore-2.0.0rc2/requirements/requirements-scheduler.in
+-rw-rw-rw-   0 root         (0) root         (0)      711 2023-05-21 22:10:36.000000 vbcore-2.0.0rc2/requirements/requirements-scheduler.txt
+-rw-rw-rw-   0 root         (0) root         (0)       99 2023-05-21 22:10:36.000000 vbcore-2.0.0rc2/requirements/requirements-test.in
+-rw-rw-rw-   0 root         (0) root         (0)     1955 2023-05-21 22:10:36.000000 vbcore-2.0.0rc2/requirements/requirements-test.txt
+-rw-rw-rw-   0 root         (0) root         (0)       93 2023-05-21 22:10:36.000000 vbcore-2.0.0rc2/requirements/requirements.in
+-rw-rw-rw-   0 root         (0) root         (0)      677 2023-05-21 22:10:36.000000 vbcore-2.0.0rc2/requirements/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-21 22:10:47.949563 vbcore-2.0.0rc2/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     4745 2023-05-21 22:10:36.000000 vbcore-2.0.0rc2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 22:10:47.939563 vbcore-2.0.0rc2/vbcore/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-21 22:10:36.000000 vbcore-2.0.0rc2/vbcore/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       49 2023-05-21 22:10:36.000000 vbcore-2.0.0rc2/vbcore/__main__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1161 2023-05-21 22:10:36.000000 vbcore-2.0.0rc2/vbcore/aio.py
+-rw-rw-rw-   0 root         (0) root         (0)     4706 2023-05-21 22:10:36.000000 vbcore-2.0.0rc2/vbcore/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     7460 2023-05-21 22:10:36.000000 vbcore-2.0.0rc2/vbcore/batch.py
+-rw-rw-rw-   0 root         (0) root         (0)     1396 2023-05-21 22:10:36.000000 vbcore-2.0.0rc2/vbcore/configurator.py
+-rw-rw-rw-   0 root         (0) root         (0)     7979 2023-05-21 22:10:36.000000 vbcore-2.0.0rc2/vbcore/crc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 22:10:47.941563 vbcore-2.0.0rc2/vbcore/crypto/
+-rw-rw-rw-   0 root         (0) root         (0)       85 2023-05-21 22:10:36.000000 vbcore-2.0.0rc2/vbcore/crypto/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1266 2023-05-21 22:10:36.000000 vbcore-2.0.0rc2/vbcore/crypto/argon.py
+-rw-rw-rw-   0 root         (0) root         (0)      942 2023-05-21 22:10:36.000000 vbcore-2.0.0rc2/vbcore/crypto/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     1093 2023-05-21 22:10:36.000000 vbcore-2.0.0rc2/vbcore/crypto/bcrypt.py
+-rw-rw-rw-   0 root         (0) root         (0)      285 2023-05-21 22:10:36.000000 vbcore-2.0.0rc2/vbcore/crypto/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     1077 2023-05-21 22:10:36.000000 vbcore-2.0.0rc2/vbcore/crypto/factory.py
+-rw-rw-rw-   0 root         (0) root         (0)     1213 2023-05-21 22:10:36.000000 vbcore-2.0.0rc2/vbcore/crypto/hashes.py
+-rw-rw-rw-   0 root         (0) root         (0)     3233 2023-05-21 22:10:36.000000 vbcore-2.0.0rc2/vbcore/csvfile.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 22:10:47.942563 vbcore-2.0.0rc2/vbcore/datastruct/
+-rw-rw-rw-   0 root         (0) root         (0)      209 2023-05-21 22:10:36.000000 vbcore-2.0.0rc2/vbcore/datastruct/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1108 2023-05-21 22:10:36.000000 vbcore-2.0.0rc2/vbcore/datastruct/buffer.py
+-rw-rw-rw-   0 root         (0) root         (0)     6012 2023-05-21 22:10:36.000000 vbcore-2.0.0rc2/vbcore/datastruct/cache.py
+-rw-rw-rw-   0 root         (0) root         (0)     2776 2023-05-21 22:10:36.000000 vbcore-2.0.0rc2/vbcore/datastruct/dictionaries.py
+-rw-rw-rw-   0 root         (0) root         (0)     2772 2023-05-21 22:10:36.000000 vbcore-2.0.0rc2/vbcore/datastruct/lazy.py
+-rw-rw-rw-   0 root         (0) root         (0)      346 2023-05-21 22:10:36.000000 vbcore-2.0.0rc2/vbcore/datastruct/misc.py
+-rw-rw-rw-   0 root         (0) root         (0)     1156 2023-05-21 22:10:36.000000 vbcore-2.0.0rc2/vbcore/datastruct/orderer_set.py
+-rw-rw-rw-   0 root         (0) root         (0)     4400 2023-05-21 22:10:36.000000 vbcore-2.0.0rc2/vbcore/date_helper.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 22:10:47.943563 vbcore-2.0.0rc2/vbcore/db/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-21 22:10:36.000000 vbcore-2.0.0rc2/vbcore/db/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    18546 2023-05-21 22:10:36.000000 vbcore-2.0.0rc2/vbcore/db/events.py
+-rw-rw-rw-   0 root         (0) root         (0)     6781 2023-05-21 22:10:36.000000 vbcore-2.0.0rc2/vbcore/db/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     2866 2023-05-21 22:10:36.000000 vbcore-2.0.0rc2/vbcore/db/listener.py
+-rw-rw-rw-   0 root         (0) root         (0)     2840 2023-05-21 22:10:36.000000 vbcore-2.0.0rc2/vbcore/db/mixins.py
+-rw-rw-rw-   0 root         (0) root         (0)     6775 2023-05-21 22:10:36.000000 vbcore-2.0.0rc2/vbcore/db/mysql_dumper.py
+-rw-rw-rw-   0 root         (0) root         (0)     1826 2023-05-21 22:10:36.000000 vbcore-2.0.0rc2/vbcore/db/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     4076 2023-05-21 22:10:36.000000 vbcore-2.0.0rc2/vbcore/db/sqla.py
+-rw-rw-rw-   0 root         (0) root         (0)     5455 2023-05-21 22:10:36.000000 vbcore-2.0.0rc2/vbcore/db/support.py
+-rw-rw-rw-   0 root         (0) root         (0)     2092 2023-05-21 22:10:36.000000 vbcore-2.0.0rc2/vbcore/db/views.py
+-rw-rw-rw-   0 root         (0) root         (0)     1032 2023-05-21 22:10:36.000000 vbcore-2.0.0rc2/vbcore/dispatcher.py
+-rw-rw-rw-   0 root         (0) root         (0)     2190 2023-05-21 22:10:36.000000 vbcore-2.0.0rc2/vbcore/enums.py
+-rw-rw-rw-   0 root         (0) root         (0)      730 2023-05-21 22:10:36.000000 vbcore-2.0.0rc2/vbcore/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     3883 2023-05-21 22:10:36.000000 vbcore-2.0.0rc2/vbcore/factory.py
+-rw-rw-rw-   0 root         (0) root         (0)     3901 2023-05-21 22:10:36.000000 vbcore-2.0.0rc2/vbcore/files.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 22:10:47.944563 vbcore-2.0.0rc2/vbcore/http/
+-rw-rw-rw-   0 root         (0) root         (0)       69 2023-05-21 22:10:36.000000 vbcore-2.0.0rc2/vbcore/http/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2938 2023-05-21 22:10:36.000000 vbcore-2.0.0rc2/vbcore/http/batch.py
+-rw-rw-rw-   0 root         (0) root         (0)     8176 2023-05-21 22:10:36.000000 vbcore-2.0.0rc2/vbcore/http/client.py
+-rw-rw-rw-   0 root         (0) root         (0)     3880 2023-05-21 22:10:36.000000 vbcore-2.0.0rc2/vbcore/http/gql.py
+-rw-rw-rw-   0 root         (0) root         (0)     3233 2023-05-21 22:10:36.000000 vbcore-2.0.0rc2/vbcore/http/headers.py
+-rw-rw-rw-   0 root         (0) root         (0)     2632 2023-05-21 22:10:36.000000 vbcore-2.0.0rc2/vbcore/http/httpcode.py
+-rw-rw-rw-   0 root         (0) root         (0)     4012 2023-05-21 22:10:36.000000 vbcore-2.0.0rc2/vbcore/http/httpdumper.py
+-rw-rw-rw-   0 root         (0) root         (0)      445 2023-05-21 22:10:36.000000 vbcore-2.0.0rc2/vbcore/http/methods.py
+-rw-rw-rw-   0 root         (0) root         (0)     6063 2023-05-21 22:10:36.000000 vbcore-2.0.0rc2/vbcore/http/proxy.py
+-rw-rw-rw-   0 root         (0) root         (0)     1894 2023-05-21 22:10:36.000000 vbcore-2.0.0rc2/vbcore/http/rpc.py
+-rw-rw-rw-   0 root         (0) root         (0)     2128 2023-05-21 22:10:36.000000 vbcore-2.0.0rc2/vbcore/http/useragent.py
+-rw-rw-rw-   0 root         (0) root         (0)     4631 2023-05-21 22:10:36.000000 vbcore-2.0.0rc2/vbcore/importer.py
+-rw-rw-rw-   0 root         (0) root         (0)     4808 2023-05-21 22:10:36.000000 vbcore-2.0.0rc2/vbcore/json.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 22:10:47.945563 vbcore-2.0.0rc2/vbcore/jsonschema/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-21 22:10:36.000000 vbcore-2.0.0rc2/vbcore/jsonschema/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 22:10:47.945563 vbcore-2.0.0rc2/vbcore/jsonschema/schemas/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-21 22:10:36.000000 vbcore-2.0.0rc2/vbcore/jsonschema/schemas/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2118 2023-05-21 22:10:36.000000 vbcore-2.0.0rc2/vbcore/jsonschema/schemas/jsonrpc.py
+-rw-rw-rw-   0 root         (0) root         (0)     7052 2023-05-21 22:10:36.000000 vbcore-2.0.0rc2/vbcore/jsonschema/support.py
+-rw-rw-rw-   0 root         (0) root         (0)     2620 2023-05-21 22:10:36.000000 vbcore-2.0.0rc2/vbcore/lambdas.py
+-rw-rw-rw-   0 root         (0) root         (0)     2524 2023-05-21 22:10:36.000000 vbcore-2.0.0rc2/vbcore/loggers.py
+-rw-rw-rw-   0 root         (0) root         (0)     4304 2023-05-21 22:10:36.000000 vbcore-2.0.0rc2/vbcore/misc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 22:10:47.946563 vbcore-2.0.0rc2/vbcore/net/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-21 22:10:36.000000 vbcore-2.0.0rc2/vbcore/net/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2078 2023-05-21 22:10:36.000000 vbcore-2.0.0rc2/vbcore/net/helpers.py
+-rw-rw-rw-   0 root         (0) root         (0)     5873 2023-05-21 22:10:36.000000 vbcore-2.0.0rc2/vbcore/net/sendmail.py
+-rw-rw-rw-   0 root         (0) root         (0)     3541 2023-05-21 22:10:36.000000 vbcore-2.0.0rc2/vbcore/net/sftp.py
+-rw-rw-rw-   0 root         (0) root         (0)     1566 2023-05-21 22:10:36.000000 vbcore-2.0.0rc2/vbcore/net/socks_smtp.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 22:10:47.946563 vbcore-2.0.0rc2/vbcore/rule_engine/
+-rw-rw-rw-   0 root         (0) root         (0)      106 2023-05-21 22:10:36.000000 vbcore-2.0.0rc2/vbcore/rule_engine/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1263 2023-05-21 22:10:36.000000 vbcore-2.0.0rc2/vbcore/rule_engine/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     3220 2023-05-21 22:10:36.000000 vbcore-2.0.0rc2/vbcore/rule_engine/engine.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 22:10:47.946563 vbcore-2.0.0rc2/vbcore/standalone/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-21 22:10:36.000000 vbcore-2.0.0rc2/vbcore/standalone/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3335 2023-05-21 22:10:36.000000 vbcore-2.0.0rc2/vbcore/standalone/scheduler.py
+-rw-rw-rw-   0 root         (0) root         (0)     9057 2023-05-21 22:10:36.000000 vbcore-2.0.0rc2/vbcore/standalone/wsgi_gunicorn.py
+-rw-rw-rw-   0 root         (0) root         (0)     4449 2023-05-21 22:10:36.000000 vbcore-2.0.0rc2/vbcore/system.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 22:10:47.947563 vbcore-2.0.0rc2/vbcore/tester/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-21 22:10:36.000000 vbcore-2.0.0rc2/vbcore/tester/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    16074 2023-05-21 22:10:36.000000 vbcore-2.0.0rc2/vbcore/tester/asserter.py
+-rw-rw-rw-   0 root         (0) root         (0)      346 2023-05-21 22:10:36.000000 vbcore-2.0.0rc2/vbcore/tester/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     1455 2023-05-21 22:10:36.000000 vbcore-2.0.0rc2/vbcore/tester/fetchmail.py
+-rw-rw-rw-   0 root         (0) root         (0)     1963 2023-05-21 22:10:36.000000 vbcore-2.0.0rc2/vbcore/tester/helpers.py
+-rw-rw-rw-   0 root         (0) root         (0)     7405 2023-05-21 22:10:36.000000 vbcore-2.0.0rc2/vbcore/tester/http.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 22:10:47.947563 vbcore-2.0.0rc2/vbcore/tester/plugins/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-21 22:10:36.000000 vbcore-2.0.0rc2/vbcore/tester/plugins/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      163 2023-05-21 22:10:36.000000 vbcore-2.0.0rc2/vbcore/tester/plugins/fixtures.py
+-rw-rw-rw-   0 root         (0) root         (0)      438 2023-05-21 22:10:36.000000 vbcore-2.0.0rc2/vbcore/tester/plugins/startup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 22:10:47.948563 vbcore-2.0.0rc2/vbcore/tools/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-21 22:10:36.000000 vbcore-2.0.0rc2/vbcore/tools/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5840 2023-05-21 22:10:36.000000 vbcore-2.0.0rc2/vbcore/tools/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)      948 2023-05-21 22:10:36.000000 vbcore-2.0.0rc2/vbcore/tools/crypto.py
+-rw-rw-rw-   0 root         (0) root         (0)     2227 2023-05-21 22:10:36.000000 vbcore-2.0.0rc2/vbcore/tools/database.py
+-rw-rw-rw-   0 root         (0) root         (0)      699 2023-05-21 22:10:36.000000 vbcore-2.0.0rc2/vbcore/tools/entrypoint.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 22:10:47.948563 vbcore-2.0.0rc2/vbcore/tools/initializer/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-21 22:10:36.000000 vbcore-2.0.0rc2/vbcore/tools/initializer/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1104 2023-05-21 22:10:36.000000 vbcore-2.0.0rc2/vbcore/tools/initializer/init.py
+-rw-rw-rw-   0 root         (0) root         (0)      765 2023-05-21 22:10:36.000000 vbcore-2.0.0rc2/vbcore/tools/scheduler.py
+-rw-rw-rw-   0 root         (0) root         (0)      773 2023-05-21 22:10:36.000000 vbcore-2.0.0rc2/vbcore/types.py
+-rw-rw-rw-   0 root         (0) root         (0)     1025 2023-05-21 22:10:36.000000 vbcore-2.0.0rc2/vbcore/uuid.py
+-rw-rw-rw-   0 root         (0) root         (0)      256 2023-05-21 22:10:36.000000 vbcore-2.0.0rc2/vbcore/version.py
+-rw-rw-rw-   0 root         (0) root         (0)     2877 2023-05-21 22:10:36.000000 vbcore-2.0.0rc2/vbcore/yaml.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 22:10:47.940563 vbcore-2.0.0rc2/vbcore.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      402 2023-05-21 22:10:47.000000 vbcore-2.0.0rc2/vbcore.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3144 2023-05-21 22:10:47.000000 vbcore-2.0.0rc2/vbcore.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-21 22:10:47.000000 vbcore-2.0.0rc2/vbcore.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       56 2023-05-21 22:10:47.000000 vbcore-2.0.0rc2/vbcore.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-21 22:10:47.000000 vbcore-2.0.0rc2/vbcore.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      528 2023-05-21 22:10:47.000000 vbcore-2.0.0rc2/vbcore.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-05-21 22:10:47.000000 vbcore-2.0.0rc2/vbcore.egg-info/top_level.txt
```

### Comparing `vbcore-1.3.0rc3/requirements/requirements-crypto.txt` & `vbcore-2.0.0rc2/requirements/requirements-net.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,22 +1,35 @@
 #
-# This file is autogenerated by pip-compile with python 3.8
-# To update, run:
+# This file is autogenerated by pip-compile with Python 3.10
+# by the following command:
 #
-#    pip-compile --no-emit-index-url --no-emit-trusted-host --output-file=requirements/requirements-crypto.txt requirements/requirements-crypto.in
+#    pip-compile --no-emit-index-url --no-emit-trusted-host --output-file=requirements/requirements-net.txt requirements/requirements-net.in
 #
-argon2-cffi==21.3.0
+bcrypt==4.0.1
+    # via paramiko
+cffi==1.15.1
     # via
-    #   -c requirements/requirements-all.txt
-    #   -r requirements/requirements-crypto.in
-argon2-cffi-bindings==21.2.0
+    #   -c requirements/requirements-build.txt
+    #   cryptography
+    #   pynacl
+cryptography==40.0.2
     # via
-    #   -c requirements/requirements-all.txt
-    #   argon2-cffi
-cffi==1.15.1
+    #   -c requirements/requirements-build.txt
+    #   paramiko
+dnspython==2.3.0
+    # via email-validator
+email-validator==2.0.0.post2
+    # via -r requirements/requirements-net.in
+idna==3.4
     # via
-    #   -c requirements/requirements-all.txt
-    #   argon2-cffi-bindings
+    #   -c requirements/requirements-build.txt
+    #   email-validator
+paramiko==3.1.0
+    # via -r requirements/requirements-net.in
 pycparser==2.21
     # via
-    #   -c requirements/requirements-all.txt
+    #   -c requirements/requirements-build.txt
     #   cffi
+pynacl==1.5.0
+    # via paramiko
+pysocks==1.7.1
+    # via -r requirements/requirements-net.in
```

### Comparing `vbcore-1.3.0rc3/requirements/requirements-db.txt` & `vbcore-2.0.0rc2/requirements/requirements-db.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,29 +1,19 @@
 #
-# This file is autogenerated by pip-compile with python 3.8
-# To update, run:
+# This file is autogenerated by pip-compile with Python 3.10
+# by the following command:
 #
 #    pip-compile --no-emit-index-url --no-emit-trusted-host --output-file=requirements/requirements-db.txt requirements/requirements-db.in
 #
-greenlet==1.1.3.post0
-    # via
-    #   -c requirements/requirements-all.txt
-    #   sqlalchemy
+greenlet==2.0.2
+    # via sqlalchemy
 pydot==1.4.2
-    # via
-    #   -c requirements/requirements-all.txt
-    #   sqlalchemy-schemadisplay
+    # via sqlalchemy-schemadisplay
 pyparsing==3.0.9
-    # via
-    #   -c requirements/requirements-all.txt
-    #   pydot
-sqlalchemy==1.4.42
-    # via
-    #   -c requirements/requirements-all.txt
-    #   -r requirements/requirements-db.in
+    # via pydot
+sqlalchemy==1.4.48
+    # via -r requirements/requirements-db.in
 sqlalchemy-schemadisplay==1.3
-    # via
-    #   -c requirements/requirements-all.txt
-    #   -r requirements/requirements-db.in
+    # via -r requirements/requirements-db.in
 
 # The following packages are considered to be unsafe in a requirements file:
 # setuptools
```

### Comparing `vbcore-1.3.0rc3/requirements/requirements-extra.txt` & `vbcore-2.0.0rc2/requirements/requirements-extra.txt`

 * *Files 25% similar despite different names*

```diff
@@ -1,50 +1,48 @@
 #
-# This file is autogenerated by pip-compile with python 3.8
-# To update, run:
+# This file is autogenerated by pip-compile with Python 3.10
+# by the following command:
 #
 #    pip-compile --no-emit-index-url --no-emit-trusted-host --output-file=requirements/requirements-extra.txt requirements/requirements-extra.in
 #
-attrs==22.1.0
+attrs==23.1.0
+    # via jsonschema
+backoff==2.2.1
+    # via gql
+chardet==5.1.0
     # via
-    #   -c requirements/requirements-all.txt
-    #   jsonschema
-chardet==5.0.0
-    # via
-    #   -c requirements/requirements-all.txt
-    #   -r requirements/requirements-extra.in
-importlib-resources==5.10.0
-    # via
-    #   -c requirements/requirements-all.txt
-    #   jsonschema
-jsonschema==4.16.0
-    # via
-    #   -c requirements/requirements-all.txt
+    #   -c requirements/requirements-build.txt
     #   -r requirements/requirements-extra.in
-pkgutil-resolve-name==1.3.10
-    # via
-    #   -c requirements/requirements-all.txt
-    #   jsonschema
+gql==3.4.1
+    # via -r requirements/requirements-extra.in
+graphql-core==3.2.3
+    # via gql
+gunicorn==20.1.0
+    # via -r requirements/requirements-extra.in
+idna==3.4
+    # via
+    #   -c requirements/requirements-build.txt
+    #   yarl
+jsonschema==4.17.3
+    # via -r requirements/requirements-extra.in
+multidict==6.0.4
+    # via yarl
 ply==3.11
-    # via
-    #   -c requirements/requirements-all.txt
-    #   rule-engine
-pyrsistent==0.18.1
-    # via
-    #   -c requirements/requirements-all.txt
-    #   jsonschema
+    # via rule-engine
+pyrsistent==0.19.3
+    # via jsonschema
 python-dateutil==2.8.2
     # via
-    #   -c requirements/requirements-all.txt
+    #   -c requirements/requirements.txt
     #   rule-engine
-rule-engine==3.5.0
-    # via
-    #   -c requirements/requirements-all.txt
-    #   -r requirements/requirements-extra.in
+rule-engine==3.5.1
+    # via -r requirements/requirements-extra.in
 six==1.16.0
     # via
-    #   -c requirements/requirements-all.txt
+    #   -c requirements/requirements-build.txt
+    #   -c requirements/requirements.txt
     #   python-dateutil
-zipp==3.9.0
-    # via
-    #   -c requirements/requirements-all.txt
-    #   importlib-resources
+yarl==1.9.2
+    # via gql
+
+# The following packages are considered to be unsafe in a requirements file:
+# setuptools
```

### Comparing `vbcore-1.3.0rc3/requirements/requirements-net.txt` & `vbcore-2.0.0rc2/requirements/requirements.txt`

 * *Files 24% similar despite different names*

```diff
@@ -1,37 +1,22 @@
 #
-# This file is autogenerated by pip-compile with python 3.8
-# To update, run:
+# This file is autogenerated by pip-compile with Python 3.10
+# by the following command:
 #
-#    pip-compile --no-emit-index-url --no-emit-trusted-host --output-file=requirements/requirements-net.txt requirements/requirements-net.in
+#    pip-compile --no-emit-index-url --no-emit-trusted-host --output-file=requirements/requirements.txt requirements/requirements.in
 #
-bcrypt==4.0.1
-    # via paramiko
-cffi==1.15.1
-    # via
-    #   -c requirements/requirements.txt
-    #   cryptography
-    #   pynacl
-cryptography==36.0.2
-    # via
-    #   -c requirements/requirements.txt
-    #   paramiko
-dnspython==2.2.1
-    # via email-validator
-email-validator==1.3.0
-    # via -r requirements/requirements-net.in
-idna==3.4
-    # via email-validator
-paramiko==2.11.0
-    # via -r requirements/requirements-net.in
-pycparser==2.21
-    # via
-    #   -c requirements/requirements.txt
-    #   cffi
-pynacl==1.5.0
-    # via paramiko
-pysocks==1.7.1
-    # via -r requirements/requirements-net.in
+click==8.1.3
+    # via -r requirements/requirements.in
+psutil==5.9.5
+    # via -r requirements/requirements.in
+python-dateutil==2.8.2
+    # via -r requirements/requirements.in
+python-decouple==3.8
+    # via -r requirements/requirements.in
+python-dotenv==1.0.0
+    # via -r requirements/requirements.in
+pyyaml==6.0
+    # via -r requirements/requirements.in
 six==1.16.0
     # via
-    #   -c requirements/requirements.txt
-    #   paramiko
+    #   -c requirements/requirements-build.txt
+    #   python-dateutil
```

### Comparing `vbcore-1.3.0rc3/requirements/requirements-scheduler.txt` & `vbcore-2.0.0rc2/requirements/requirements-scheduler.txt`

 * *Files 26% similar despite different names*

```diff
@@ -1,38 +1,24 @@
 #
-# This file is autogenerated by pip-compile with python 3.8
-# To update, run:
+# This file is autogenerated by pip-compile with Python 3.10
+# by the following command:
 #
 #    pip-compile --no-emit-index-url --no-emit-trusted-host --output-file=requirements/requirements-scheduler.txt requirements/requirements-scheduler.in
 #
-apscheduler==3.9.1
-    # via
-    #   -c requirements/requirements-all.txt
-    #   -r requirements/requirements-scheduler.in
-backports.zoneinfo==0.2.1 ; python_version < "3.9"
-    # via
-    #   -c requirements/requirements-all.txt
-    #   pytz-deprecation-shim
-    #   tzlocal
-pytz==2022.5
-    # via
-    #   -c requirements/requirements-all.txt
-    #   apscheduler
+apscheduler==3.10.1
+    # via -r requirements/requirements-scheduler.in
+pytz==2023.3
+    # via apscheduler
 pytz-deprecation-shim==0.1.0.post0
-    # via
-    #   -c requirements/requirements-all.txt
-    #   tzlocal
+    # via tzlocal
 six==1.16.0
     # via
-    #   -c requirements/requirements-all.txt
-    #   apscheduler
-tzdata==2022.5
-    # via
-    #   -c requirements/requirements-all.txt
-    #   pytz-deprecation-shim
-tzlocal==4.2
-    # via
-    #   -c requirements/requirements-all.txt
+    #   -c requirements/requirements-build.txt
+    #   -c requirements/requirements.txt
     #   apscheduler
+tzdata==2023.3
+    # via pytz-deprecation-shim
+tzlocal==4.3
+    # via apscheduler
 
 # The following packages are considered to be unsafe in a requirements file:
 # setuptools
```

### Comparing `vbcore-1.3.0rc3/requirements/requirements-test.txt` & `vbcore-2.0.0rc2/requirements/requirements-http.txt`

 * *Files 17% similar despite different names*

```diff
@@ -1,70 +1,50 @@
 #
-# This file is autogenerated by pip-compile with python 3.8
-# To update, run:
+# This file is autogenerated by pip-compile with Python 3.10
+# by the following command:
 #
-#    pip-compile --no-emit-index-url --no-emit-trusted-host --output-file=requirements/requirements-test.txt requirements/requirements-test.in
+#    pip-compile --no-emit-index-url --no-emit-trusted-host --output-file=requirements/requirements-http.txt requirements/requirements-http.in
 #
-attrs==22.1.0
+aiohttp==3.8.4
+    # via -r requirements/requirements-http.in
+aiosignal==1.3.1
+    # via aiohttp
+async-timeout==4.0.2
+    # via aiohttp
+attrs==23.1.0
+    # via aiohttp
+certifi==2023.5.7
     # via
-    #   -c requirements/requirements-all.txt
-    #   hypothesis
-    #   pytest
-certifi==2022.9.24
-    # via
-    #   -c requirements/requirements-all.txt
+    #   -c requirements/requirements-build.txt
     #   requests
 charset-normalizer==2.1.1
     # via
-    #   -c requirements/requirements-all.txt
+    #   -c requirements/requirements-build.txt
+    #   aiohttp
     #   requests
-coverage[toml]==6.5.0
+frozenlist==1.3.3
     # via
-    #   -r requirements/requirements-test.in
-    #   pytest-cov
-exceptiongroup==1.0.0rc9
-    # via hypothesis
-hypothesis==6.56.3
-    # via -r requirements/requirements-test.in
+    #   aiohttp
+    #   aiosignal
 idna==3.4
     # via
-    #   -c requirements/requirements-all.txt
+    #   -c requirements/requirements-build.txt
     #   requests
-iniconfig==1.1.1
-    # via pytest
-packaging==21.3
-    # via pytest
-pluggy==1.0.0
-    # via pytest
-py==1.11.0
-    # via pytest
-pyparsing==3.0.9
-    # via
-    #   -c requirements/requirements-all.txt
-    #   packaging
-pytest==7.1.3
-    # via
-    #   -r requirements/requirements-test.in
-    #   pytest-cov
-pytest-cov==4.0.0
-    # via -r requirements/requirements-test.in
-requests==2.28.1
-    # via
-    #   -c requirements/requirements-all.txt
-    #   responses
-responses==0.22.0
-    # via -r requirements/requirements-test.in
-sortedcontainers==2.4.0
-    # via hypothesis
-toml==0.10.2
-    # via responses
-tomli==2.0.1
-    # via
-    #   coverage
-    #   pytest
-types-toml==0.10.8
-    # via responses
-urllib3==1.26.12
+    #   yarl
+multidict==6.0.4
+    # via
+    #   aiohttp
+    #   yarl
+requests==2.30.0
+    # via
+    #   -c requirements/requirements-build.txt
+    #   -r requirements/requirements-http.in
+ua-parser==0.16.1
+    # via user-agents
+urllib3==2.0.2
     # via
-    #   -c requirements/requirements-all.txt
+    #   -c requirements/requirements-build.txt
     #   requests
-    #   responses
+user-agents==2.2.0
+    # via -r requirements/requirements-http.in
+yarl==1.9.2
+    # via aiohttp
```

### Comparing `vbcore-1.3.0rc3/requirements/requirements.txt` & `vbcore-2.0.0rc2/requirements/requirements-crypto.txt`

 * *Files 25% similar despite different names*

```diff
@@ -1,28 +1,18 @@
 #
-# This file is autogenerated by pip-compile with python 3.8
-# To update, run:
+# This file is autogenerated by pip-compile with Python 3.10
+# by the following command:
 #
-#    pip-compile --no-emit-index-url --no-emit-trusted-host --output-file=requirements/requirements.txt requirements/requirements.in
+#    pip-compile --no-emit-index-url --no-emit-trusted-host --output-file=requirements/requirements-crypto.txt requirements/requirements-crypto.in
 #
-backports-zoneinfo==0.2.1 ; python_version < "3.9"
-    # via -r requirements/requirements.in
+argon2-cffi==21.3.0
+    # via -r requirements/requirements-crypto.in
+argon2-cffi-bindings==21.2.0
+    # via argon2-cffi
 cffi==1.15.1
-    # via cryptography
-click==8.1.3
-    # via -r requirements/requirements.in
-cryptography==36.0.2
-    # via -r requirements/requirements.in
-psutil==5.9.3
-    # via -r requirements/requirements.in
+    # via
+    #   -c requirements/requirements-build.txt
+    #   argon2-cffi-bindings
 pycparser==2.21
-    # via cffi
-python-dateutil==2.8.2
-    # via -r requirements/requirements.in
-python-decouple==3.6
-    # via -r requirements/requirements.in
-python-dotenv==0.21.0
-    # via -r requirements/requirements.in
-pyyaml==6.0
-    # via -r requirements/requirements.in
-six==1.16.0
-    # via python-dateutil
+    # via
+    #   -c requirements/requirements-build.txt
+    #   cffi
```

### Comparing `vbcore-1.3.0rc3/setup.py` & `vbcore-2.0.0rc2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -127,15 +127,14 @@
 install_requires = read_requirements(os.path.join(REQ_PATH, "requirements.in"))
 tests_requires = read_requirements(os.path.join(REQ_PATH, "requirements-test.in"))
 db_requires = read_requirements(os.path.join(REQ_PATH, "requirements-db.in"))
 crypto_requires = read_requirements(os.path.join(REQ_PATH, "requirements-crypto.in"))
 http_requires = read_requirements(os.path.join(REQ_PATH, "requirements-http.in"))
 net_requires = read_requirements(os.path.join(REQ_PATH, "requirements-net.in"))
 extra_requires = read_requirements(os.path.join(REQ_PATH, "requirements-extra.in"))
-all_requires = read_requirements(os.path.join(REQ_PATH, "requirements-all.in"))
 scheduler_requires = read_requirements(
     os.path.join(REQ_PATH, "requirements-scheduler.in")
 )
 
 setup(
     name=PKG_NAME,
     url=URL,
@@ -157,20 +156,21 @@
     tests_requires=tests_requires,
     extras_require={
         "db": db_requires,
         "crypto": crypto_requires,
         "http": http_requires,
         "net": net_requires,
         "scheduler": scheduler_requires,
+        "extra": extra_requires,
         "all": [
+            *install_requires,
             *db_requires,
             *crypto_requires,
             *http_requires,
             *net_requires,
             *scheduler_requires,
             *extra_requires,
-            *all_requires,
         ],
     },
-    cmdclass=dict(test=PyTest),
+    cmdclass={"test": PyTest},
     classifiers=[],
 )
```

### Comparing `vbcore-1.3.0rc3/vbcore/batch.py` & `vbcore-2.0.0rc2/vbcore/batch.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,40 +1,26 @@
 import abc
-import asyncio
 import dataclasses
 import logging
 import threading
 import typing as t
 from contextlib import contextmanager
 from enum import auto
 from queue import Queue
 
-from vbcore.datastruct import StrEnum
-
-try:
-    import nest_asyncio
-except ImportError:
-    nest_asyncio = None
+from vbcore import aio
+from vbcore.enums import StrEnum
 
 
 class BatchExecutor:
     def __init__(self, tasks: t.Optional[list] = None, **__):
-        """
-
-        :param tasks:
-        """
         self._tasks = tasks or []
 
     @staticmethod
     def prepare_task(task: t.Union[t.Tuple, t.Callable]) -> t.Tuple[t.Callable, dict]:
-        """
-
-        :param task:
-        :return:
-        """
         if callable(task):
             return task, {}
 
         if len(task) > 1:
             return task[0], task[1] or {}
 
         return task[0], {}
@@ -45,51 +31,31 @@
             func, args = self.prepare_task(task)
             responses.append(func(**args))
         return responses
 
 
 class AsyncBatchExecutor(BatchExecutor):
     def __init__(self, return_exceptions: bool = False, **kwargs):
-        """
-
-        :param tasks:
-        :param return_exceptions:
-        """
         super().__init__(**kwargs)
         self._return_exceptions = return_exceptions
 
-    @staticmethod
-    async def _executor(fun: t.Callable, **kwargs):
-        return fun(**kwargs)  # pragma: no cover
-
-    @staticmethod
-    def is_async(fun: t.Callable):
-        return asyncio.iscoroutinefunction(fun)
-
     async def batch(self):
         tasks = []
         for task in self._tasks:
             func, args = self.prepare_task(task)
-            if not self.is_async(func):
-                tasks.append(self._executor(func, **args))  # pragma: no cover
-            else:
-                tasks.append(func(**args))
+            tasks.append(
+                aio.async_wrapper(func, **args)
+                if not aio.is_async(func)
+                else func(**args)
+            )
 
-        return await asyncio.gather(*tasks, return_exceptions=self._return_exceptions)
+        return await aio.collect(*tasks, return_exc=self._return_exceptions)
 
     def run(self) -> t.List:
-        try:
-            asyncio.get_running_loop()
-            if nest_asyncio is not None:
-                # noinspection PyUnresolvedReferences
-                nest_asyncio.apply()  # pragma: no cover
-        except RuntimeError:
-            asyncio.set_event_loop(asyncio.new_event_loop())
-
-        loop = asyncio.get_event_loop()
+        loop = aio.get_event_loop()
         return loop.run_until_complete(self.batch())
 
 
 class Thread(threading.Thread):
     def __init__(
         self,
         runnable: t.Callable,
@@ -173,15 +139,15 @@
     def __init__(self, *args, **kwargs):
         self._args = args
         self._kwargs = kwargs
         self._log = logging.getLogger(self.__module__)
 
     @abc.abstractmethod
     def perform(self, item):
-        pass  # pragma: no cover
+        raise NotImplementedError
 
 
 class IProducerConsumerBatchExecutor(abc.ABC):
     def __init__(
         self,
         producer: PCTask,
         consumer: PCTask,
@@ -204,23 +170,23 @@
         self.is_running = True
 
     def barrier(self):
         self.is_running = False
 
     @abc.abstractmethod
     def consumer(self):
-        pass  # pragma: no cover
+        raise NotImplementedError
 
     @abc.abstractmethod
     def producer(self):
-        pass  # pragma: no cover
+        raise NotImplementedError
 
     @abc.abstractmethod
     def load(self, item):
-        pass  # pragma: no cover
+        raise NotImplementedError
 
     def run_on(self, items: t.Iterable):
         with self.runner() as executor:
             for item in items:
                 executor.load(item)
```

### Comparing `vbcore-1.3.0rc3/vbcore/configurator.py` & `vbcore-2.0.0rc2/vbcore/configurator.py`

 * *Files 27% similar despite different names*

```diff
@@ -2,17 +2,14 @@
 import typing as t
 from collections import OrderedDict
 from functools import partial
 
 import decouple
 from dotenv import load_dotenv as base_load_dotenv
 
-# a special object for a default value interpreted as missing value
-MISSING = object()
-
 _conf_search_path = os.environ.get("ENV_PATH")
 _conf_file_name = os.environ.get("ENV_FILE")
 _conf_file_encoding = os.environ.get("ENV_FILE_ENCODING") or "UTF-8"
 
 
 class AutoConfig(decouple.AutoConfig):
     encoding: str = _conf_file_encoding
```

### Comparing `vbcore-1.3.0rc3/vbcore/crc.py` & `vbcore-2.0.0rc2/vbcore/crc.py`

 * *Files identical despite different names*

### Comparing `vbcore-1.3.0rc3/vbcore/csvfile.py` & `vbcore-2.0.0rc2/vbcore/csvfile.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import csv
 import typing as t
 from contextlib import contextmanager
 
-from vbcore.files import FileHandler
+from vbcore.files import FileHandler, OptStr
 
-OptStr = t.Optional[str]
 RecordType = t.Union[dict, t.Iterable[dict]]
 WriterCoroutineType = t.Generator[None, RecordType, None]
 
 
 class CustomUnixDialect(csv.unix_dialect):
     delimiter = ";"
     quoting = csv.QUOTE_MINIMAL
```

### Comparing `vbcore-1.3.0rc3/vbcore/date_helper.py` & `vbcore-2.0.0rc2/vbcore/date_helper.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 import typing as t
-from datetime import date as datetime_date, datetime
+from datetime import datetime
 
 from dateutil.parser import parse as date_parse
 
 from vbcore.base import Static
-
-DateType = t.Union[datetime_date, datetime]
-AnyDateType = t.Union[DateType, str]
+from vbcore.types import AnyDateType, DateType
 
 
 class Millis(metaclass=Static):
     seconds: t.ClassVar[int] = 1000
     minute: t.ClassVar[int] = seconds * 60
     hour: t.ClassVar[int] = minute * 60
     day: t.ClassVar[int] = hour * 24
```

### Comparing `vbcore-1.3.0rc3/vbcore/db/events.py` & `vbcore-2.0.0rc2/vbcore/db/events.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 # taken from: https://github.com/openstack/oslo.db
-
+# and adapted for my coding style and use cases
+#
+# latest ref: 7d62b3664e4acad9161d849a111bdb8b4d707f61
+#
+#
 #    Licensed under the Apache License, Version 2.0 (the "License"); you may
 #    not use this file except in compliance with the License. You may obtain
 #    a copy of the License at
 #
 #         http://www.apache.org/licenses/LICENSE-2.0
 #
 #    Unless required by applicable law or agreed to in writing, software
@@ -14,15 +18,15 @@
 
 import collections
 import logging
 import re
 import sys
 import typing as t
 
-from sqlalchemy import event, exc as sqla_exc
+from sqlalchemy import exc as sqla_exc
 from sqlalchemy.exc import DBAPIError
 
 from vbcore.db.exceptions import (
     DBConnectionError,
     DBConstraintError,
     DBDataError,
     DBDeadlock,
@@ -31,103 +35,93 @@
     DBInvalidUnicodeParameter,
     DBNonExistentConstraint,
     DBNonExistentDatabase,
     DBNonExistentTable,
     DBNotSupportedError,
     DBReferenceError,
 )
+from vbcore.db.listener import Listener
 
 LOG = logging.getLogger(__name__)
 
 ROLLBACK_CAUSE_KEY = "vbcore.db.sp_rollback_cause"
 
 ExcType = t.Union[t.Type[DBAPIError], t.Type[Exception]]
 FilterType = t.Callable[[ExcType, re.Match, str, bool], None]
 
 __REGISTRY: t.Dict[
     str, t.Dict[ExcType, t.List[t.Tuple[FilterType, re.Pattern]]]
 ] = collections.defaultdict(lambda: collections.defaultdict(list))
 
 
-class Listener:
-    @classmethod
-    def register_after_create(cls, target, callback):
-        event.listen(target, "after_create", callback)
-
-
 def try_match(match, key):
     try:
         return match.group(key)
     except IndexError:
         return None
 
 
-def filters(
-    dbname: str,
-    exception_type: ExcType,
-    regex: t.Union[re.Pattern, t.Tuple[re.Pattern, ...]],
-):
+def filters(dbname: str, exception_type: ExcType, *regexes: str) -> t.Callable:
     """
     Mark a function as receiving a filtered exception.
 
-    :param dbname: string database name, e.g. 'mysql'
-    :param exception_type: a SQLAlchemy database exception class, which
+    @param dbname: string database name, e.g. 'mysql'
+    @param exception_type: a SQLAlchemy database exception class, which
              extends from :class:`sqlalchemy.exc.DBAPIError`.
-    :param regex: a string, or a tuple of strings, that will be processed
-            as matching regular expressions.
+    @param regexes: strings that will be processed as matching regular expressions.
     """
 
     def _receive(fn: FilterType) -> FilterType:
         __REGISTRY[dbname][exception_type].extend(
-            (fn, reg) for reg in ((regex,) if not isinstance(regex, tuple) else regex)
+            (fn, re.compile(reg, re.DOTALL)) for reg in regexes
         )
         return fn
 
     return _receive
 
 
 # NOTE(zzzeek) - for Postgresql, catch both OperationalError, as the
 # actual error is
 # psycopg2.extensions.TransactionRollbackError(OperationalError),
 # as well as sqlalchemy.exc.DBAPIError, as SQLAlchemy will reraise it
 # as this until issue #3075 is fixed.
 @filters(
     "mysql",
     sqla_exc.OperationalError,
-    re.compile(r"^.*\b1213\b.*Deadlock found.*"),
+    r"^.*\b1213\b.*Deadlock found.*",
 )
 @filters(
     "mysql",
     sqla_exc.DatabaseError,
-    re.compile(r"^.*\b1205\b.*Lock wait timeout exceeded.*"),
+    r"^.*\b1205\b.*Lock wait timeout exceeded.*",
 )
 @filters(
     "mysql",
     sqla_exc.InternalError,
-    re.compile(r"^.*\b1213\b.*Deadlock found.*"),
+    r"^.*\b1213\b.*Deadlock found.*",
 )
 @filters(
     "mysql",
     sqla_exc.InternalError,
-    re.compile(r"^.*\b1213\b.*detected deadlock/conflict.*"),
+    r"^.*\b1213\b.*detected deadlock/conflict.*",
 )
 @filters(
     "mysql",
     sqla_exc.InternalError,
-    re.compile(r"^.*\b1213\b.*Deadlock: wsrep aborted.*"),
+    r"^.*\b1213\b.*Deadlock: wsrep aborted.*",
 )
 @filters(
     "postgresql",
     sqla_exc.OperationalError,
-    re.compile(r"^.*deadlock detected.*"),
+    r"^.*deadlock detected.*",
 )
 @filters(
     "postgresql",
     sqla_exc.DBAPIError,
-    re.compile(r"^.*deadlock detected.*"),
+    r"^.*deadlock detected.*",
 )
 def _deadlock_error(operational_error, match, engine_name, is_disconnect):
     """
     Filter for MySQL or Postgresql deadlock error.
     NOTE(comstud): In current versions of DB backends, Deadlock violation
     messages follow the structure:
 
@@ -143,38 +137,29 @@
     _ = match, engine_name, is_disconnect
     raise DBDeadlock(operational_error)
 
 
 @filters(
     "mysql",
     sqla_exc.IntegrityError,
-    re.compile(
-        r"^.*\b1062\b.*Duplicate entry '(?P<value>.*)' for key '(?P<columns>[^']+)'.*$"
-    ),
+    r"^.*\b1062\b.*Duplicate entry '(?P<value>.*)' for key '(?P<columns>[^']+)'.*$",
 )
-# NOTE(jd) For binary types
 @filters(
     "mysql",
     sqla_exc.IntegrityError,
-    re.compile(
-        r"^.*\b1062\b.*Duplicate entry \\'(?P<value>.*)\\' for key \\'(?P<columns>.+)\\'.*$"
-    ),
+    r"^.*\b1062\b.*Duplicate entry \\'(?P<value>.*)\\' for key \\'(?P<columns>.+)\\'.*$",
 )
-# NOTE(pkholkin): the first regex is suitable only for PostgreSQL 9.x versions
-#                 the second regex is suitable for PostgreSQL 8.x versions
 @filters(
     "postgresql",
     sqla_exc.IntegrityError,
     (
-        re.compile(
-            r'^.*duplicate\s+key.*"(?P<columns>[^"]+)"\s*\n.*'
-            r"Key\s+\((?P<key>.*)\)=\((?P<value>.*)\)\s+already\s+exists.*$"
-        ),
-        re.compile(r"^.*duplicate\s+key.*\"(?P<columns>[^\"]+)\"\s*\n.*$"),
+        r'^.*duplicate\s+key.*"(?P<columns>[^"]+)"\s*\n.*'
+        r"Key\s+\((?P<key>.*)\)=\((?P<value>.*)\)\s+already\s+exists.*$"
     ),
+    r"^.*duplicate\s+key.*\"(?P<columns>[^\"]+)\"\s*\n.*$",
 )
 def _default_dupe_key_error(integrity_error, match, engine_name, is_disconnect):
     """
     Filter for MySQL or Postgresql duplicate key error.
     note(boris-42): In current versions of DB backends unique constraint
     violation messages follow the structure:
 
@@ -219,28 +204,24 @@
     value = match.groupdict().get("value")
     raise DBDuplicateEntry(columns, value, integrity_error)
 
 
 @filters(
     "sqlite",
     sqla_exc.IntegrityError,
-    (
-        re.compile(r"^.*columns?(?P<columns>[^)]+)(is|are)\s+not\s+unique$"),
-        re.compile(r"^.*UNIQUE\s+constraint\s+failed:\s+(?P<columns>.+)$"),
-        re.compile(r"^.*PRIMARY\s+KEY\s+must\s+be\s+unique.*$"),
-    ),
+    r"^.*columns?(?P<columns>[^)]+)(is|are)\s+not\s+unique$",
+    r"^.*UNIQUE\s+constraint\s+failed:\s+(?P<columns>.+)$",
+    r"^.*PRIMARY\s+KEY\s+must\s+be\s+unique.*$",
 )
 @filters(
     "sqlite",
     sqla_exc.IntegrityError,
-    (
-        re.compile(r"^.*columns?(?P<columns>[^)]+)(is|are)\s+not\s+unique$"),
-        re.compile(r"^.*UNIQUE\s+constraint\s+failed:\s+(?P<columns>.+)$"),
-        re.compile(r"^.*PRIMARY\s+KEY\s+must\s+be\s+unique.*$"),
-    ),
+    r"^.*columns?(?P<columns>[^)]+)(is|are)\s+not\s+unique$",
+    r"^.*UNIQUE\s+constraint\s+failed:\s+(?P<columns>.+)$",
+    r"^.*PRIMARY\s+KEY\s+must\s+be\s+unique.*$",
 )
 def _sqlite_dupe_key_error(integrity_error, match, engine_name, is_disconnect):
     """
     Filter for SQLite duplicate key error.
     note(boris-42): In current versions of DB backends unique constraint
     violation messages follow the structure:
 
@@ -267,307 +248,280 @@
 
     raise DBDuplicateEntry(columns, inner_exception=integrity_error)
 
 
 @filters(
     "sqlite",
     sqla_exc.IntegrityError,
-    re.compile(r"(?i).*foreign key constraint failed"),
+    r"(?i).*foreign key constraint failed",
 )
 @filters(
     "postgresql",
     sqla_exc.IntegrityError,
-    re.compile(
+    (
         r".*on table \"(?P<table>[^\"]+)\" violates "
         r"foreign key constraint \"(?P<constraint>[^\"]+)\".*\n"
         r"DETAIL: {2}Key \((?P<key>.+)\)=\(.+\) "
         r"is (not present in|still referenced from) table "
         r"\"(?P<key_table>[^\"]+)\"."
     ),
 )
 @filters(
     "mysql",
     sqla_exc.IntegrityError,
-    re.compile(
+    (
         r".*Cannot (add|delete) or update a (child|parent) row: "
         r'a foreign key constraint fails \([`"].+[`"]\.[`"](?P<table>.+)[`"], '
         r'CONSTRAINT [`"](?P<constraint>.+)[`"] FOREIGN KEY '
         r'\([`"](?P<key>.+)[`"]\) REFERENCES [`"](?P<key_table>.+)[`"] '
     ),
 )
 def _foreign_key_error(integrity_error, match, engine_name, is_disconnect):
-    """
-    Filter for foreign key errors
-    """
     _ = engine_name, is_disconnect
     raise DBReferenceError(
         try_match(match, "table"),
         try_match(match, "constraint"),
         try_match(match, "key"),
         try_match(match, "key_table"),
         integrity_error,
     )
 
 
 @filters(
     "postgresql",
     sqla_exc.IntegrityError,
-    re.compile(
+    (
         r".*new row for relation \"(?P<table>.+)\" "
         "violates check constraint "
         '"(?P<check_name>.+)"'
     ),
 )
 def _check_constraint_error(integrity_error, match, engine_name, is_disconnect):
-    """
-    Filter for check constraint errors
-    """
     _ = engine_name, is_disconnect
     raise DBConstraintError(
         try_match(match, "table"),
         try_match(match, "check_name"),
         integrity_error,
     )
 
 
 @filters(
     "postgresql",
     sqla_exc.ProgrammingError,
-    re.compile(
+    (
         r".* constraint \"(?P<constraint>.+)\" "
         "of relation "
         '"(?P<relation>.+)" does not exist'
     ),
 )
 @filters(
     "mysql",
     sqla_exc.InternalError,
-    re.compile(
+    (
         ".*1091,.*Can't DROP (?:FOREIGN KEY )?['`](?P<constraint>.+)['`]; "
         "check that .* exists"
     ),
 )
 @filters(
     "mysql",
     sqla_exc.OperationalError,
-    re.compile(
+    (
         r".*1091,.*Can't DROP (?:FOREIGN KEY )?['`](?P<constraint>.+)['`]; "
         "check that .* exists"
     ),
 )
 @filters(
     "mysql",
     sqla_exc.InternalError,
-    re.compile(r".*1025,.*Error on rename of '.+/(?P<relation>.+)' to "),
+    r".*1025,.*Error on rename of '.+/(?P<relation>.+)' to ",
 )
 def _check_constraint_non_existing(
     programming_error, match, engine_name, is_disconnect
 ):
-    """
-    Filter for constraint non existing errors
-    """
     _ = engine_name, is_disconnect
     raise DBNonExistentConstraint(
         try_match(match, "relation"),
         try_match(match, "constraint"),
         programming_error,
     )
 
 
 @filters(
     "sqlite",
     sqla_exc.OperationalError,
-    re.compile(r".* no such table: (?P<table>.+)"),
+    r".* no such table: (?P<table>.+)",
 )
 @filters(
     "mysql",
     sqla_exc.InternalError,
-    re.compile(r".*1051,.*Unknown table '(.+\.)?(?P<table>.+)'\""),
+    r".*1051,.*Unknown table '(.+\.)?(?P<table>.+)'\"",
 )
 @filters(
     "mysql",
     sqla_exc.OperationalError,
-    re.compile(r".*1051,.*Unknown table '(.+\.)?(?P<table>.+)'\""),
+    r".*1051,.*Unknown table '(.+\.)?(?P<table>.+)'\"",
 )
 @filters(
     "postgresql",
     sqla_exc.ProgrammingError,
-    re.compile(r".* table \"(?P<table>.+)\" does not exist"),
+    r".* table \"(?P<table>.+)\" does not exist",
 )
 def _check_table_non_existing(programming_error, match, engine_name, is_disconnect):
-    """
-    Filter for table non existing errors
-    """
     _ = engine_name, is_disconnect
     raise DBNonExistentTable(match.group("table"), programming_error)
 
 
 @filters(
     "mysql",
     sqla_exc.InternalError,
-    re.compile(r".*1049,.*Unknown database '(?P<database>.+)'\""),
+    r".*1049,.*Unknown database '(?P<database>.+)'\"",
 )
 @filters(
     "mysql",
     sqla_exc.OperationalError,
-    re.compile(r".*1049,.*Unknown database '(?P<database>.+)'\""),
+    r".*1049,.*Unknown database '(?P<database>.+)'\"",
 )
 @filters(
     "postgresql",
     sqla_exc.OperationalError,
-    re.compile(r".*database \"(?P<database>.+)\" does not exist"),
+    r".*database \"(?P<database>.+)\" does not exist",
 )
 @filters(
     "sqlite",
     sqla_exc.OperationalError,
-    re.compile(r".*unable to open database file.*"),
+    r".*unable to open database file.*",
 )
 def _check_database_non_existing(error, match, engine_name, is_disconnect):
     _ = engine_name, is_disconnect
     raise DBNonExistentDatabase(try_match(match, "database"), error)
 
 
 @filters(
     "mysql",
     sqla_exc.DBAPIError,
-    re.compile(r".*\b1146\b"),
+    r".*\b1146\b",
 )
 def _raise_mysql_table_doesnt_exist_as_is(error, match, engine_name, is_disconnect):
     """
     Raise MySQL error 1146 as is.
     Raise MySQL error 1146 as is, so that it does not conflict with
     the MySQL dialect's checking a table not existing.
     """
     _ = match, engine_name, is_disconnect
     raise error
 
 
 @filters(
     "mysql",
     sqla_exc.OperationalError,
-    re.compile(r".*(1292|1366).*Incorrect \w+ value.*"),
+    r".*(1292|1366).*Incorrect \w+ value.*",
 )
 @filters(
     "mysql",
     sqla_exc.DataError,
-    re.compile(r".*1265.*Data truncated for column.*"),
+    r".*1265.*Data truncated for column.*",
 )
 @filters(
     "mysql",
     sqla_exc.DataError,
-    re.compile(r".*1264.*Out of range value for column.*"),
+    r".*1264.*Out of range value for column.*",
 )
 @filters(
     "mysql",
     sqla_exc.InternalError,
-    re.compile(r"^.*1366.*Incorrect string value:*"),
+    r"^.*1366.*Incorrect string value:*",
 )
 @filters(
     "sqlite",
     sqla_exc.ProgrammingError,
-    re.compile(r"(?i).*You must not use 8-bit bytestrings*"),
+    r"(?i).*You must not use 8-bit bytestrings*",
 )
 @filters(
     "mysql",
     sqla_exc.DataError,
-    re.compile(r".*1406.*Data too long for column.*"),
+    r".*1406.*Data too long for column.*",
 )
 def _raise_data_error(error, match, engine_name, is_disconnect):
-    """
-    Raise DBDataError exception for different data errors
-    """
     _ = match, engine_name, is_disconnect
     raise DBDataError(error)
 
 
 @filters(
     "mysql",
     sqla_exc.OperationalError,
-    re.compile(r".*\(1305,\s+\'SAVEPOINT\s+(.+)\s+does not exist\'\)"),
+    r".*\(1305,\s+\'SAVEPOINT\s+(.+)\s+does not exist\'\)",
 )
 def _raise_savepoints_as_dberrors(error, match, engine_name, is_disconnect):
     # NOTE(rpodolyaka): this is a special case of an OperationalError that used
     # to be an InternalError. It's expected to be wrapped into oslo.db error.
     _ = match, engine_name, is_disconnect
     raise DBError(error)
 
 
-@filters("*", sqla_exc.OperationalError, re.compile(r".*"))
+@filters("*", sqla_exc.OperationalError, r".*")
 def _raise_operational_errors_directly_filter(
     operational_error, match, engine_name, is_disconnect
 ):
-    """
-    Filter for all remaining OperationalError classes and apply.
-    Filter for all remaining OperationalError classes and apply
-    special rules.
-    """
     _ = match, engine_name
     if is_disconnect:
         # operational errors that represent disconnect
         # should be wrapped
         raise DBConnectionError(operational_error)
     # NOTE(comstud): A lot of code is checking for OperationalError
     # so let's not wrap it for now.
     raise DBError(operational_error)
 
 
 @filters(
     "mysql",
     sqla_exc.OperationalError,
-    re.compile(r".*\(.*(?:2002|2003|2006|2013|1047)"),
+    r".*\(.*(?:2002|2003|2006|2013|1047)",
 )
 @filters(
     "mysql",
     sqla_exc.InternalError,
-    re.compile(r".*\(.*(?:1927)"),
+    r".*\(.*(?:1927)",
 )
 @filters(
     "mysql",
     sqla_exc.InternalError,
-    re.compile(r".*Packet sequence number wrong"),
+    r".*Packet sequence number wrong",
 )
 @filters(
     "postgresql",
     sqla_exc.OperationalError,
-    re.compile(r".*could not connect to server"),
+    r".*could not connect to server",
 )
 def _is_db_connection_error(operational_error, match, engine_name, is_disconnect):
-    """
-    Detect the exception as indicating a recoverable error on connect
-    """
     _ = match, engine_name, is_disconnect
     raise DBConnectionError(operational_error)
 
 
-@filters("*", sqla_exc.NotSupportedError, re.compile(r".*"))
+@filters("*", sqla_exc.NotSupportedError, r".*")
 def _raise_for_not_supported_error(error, match, engine_name, is_disconnect):
     _ = match, engine_name, is_disconnect
     raise DBNotSupportedError(error)
 
 
-@filters("*", sqla_exc.DBAPIError, re.compile(r".*"))
+@filters("*", sqla_exc.DBAPIError, r".*")
 def _raise_for_remaining_db_api_error(error, match, engine_name, is_disconnect):
-    """
-    Filter for remaining DBAPIErrors.
-    Filter for remaining DBAPIErrors and wrap if they represent a disconnect error
-    """
     _ = match, engine_name
     if is_disconnect:
         raise DBConnectionError(error)
     LOG.warning("DBAPIError exception wrapped.", exc_info=True)
     raise DBError(error)
 
 
-@filters("*", UnicodeEncodeError, re.compile(r".*"))
+@filters("*", UnicodeEncodeError, r".*")
 def _raise_for_unicode_encode(error, match, engine_name, is_disconnect):
     _ = error, match, engine_name, is_disconnect
     raise DBInvalidUnicodeParameter()
 
 
-@filters("*", Exception, re.compile(r".*"))
+@filters("*", Exception, r".*")
 def _raise_for_all_others(error, match, engine_name, is_disconnect):
     _ = match, engine_name, is_disconnect
     LOG.warning("DB exception wrapped.", exc_info=True)
     raise DBError(error)
 
 
 def _dialect_registries(engine):
@@ -598,14 +552,20 @@
             and not context.connection.invalidated
             and ROLLBACK_CAUSE_KEY in context.connection.info
         ):
             dbe.cause = context.connection.info.pop(ROLLBACK_CAUSE_KEY)
 
         if isinstance(dbe, DBConnectionError):
             context.is_disconnect = True
+
+            if hasattr(context, "is_pre_ping") and context.is_pre_ping:
+                # if this is a pre-ping, need to integrate
+                # with the built-in pre-ping handler that doesn't know
+                # about DBConnectionError, just needs the updated status
+                return None
         return dbe
 
 
 def _per_dialect_handler(context, per_dialect):
     for exc in (context.sqlalchemy_exception, context.original_exception):
         for super_ in exc.__class__.__mro__:
             for fn, regexp in per_dialect.get(super_) or ():
@@ -627,44 +587,28 @@
     for per_dialect in _dialect_registries(context.engine):
         handled = _per_dialect_handler(context, per_dialect)
         if handled:
             return handled
     return None
 
 
-def register_engine_events(engine):
-    event.listen(engine, "handle_error", handler, retval=True)
+def register_error_handlers(engine):
+    Listener.register_handle_error(engine, handler, retval=True)
 
-    @event.listens_for(engine, "rollback_savepoint")
-    def rollback_savepoint(conn, name, context):
+    @Listener.listens_for_rollback_savepoint(engine)
+    def save_cause_on_rollback_savepoint(conn, name, context):
         _ = name, context
         exc_info = sys.exc_info()
         if exc_info[1] and not conn.invalidated:
-            # NOTE(zzzeek) accessing conn.info on an invalidated
-            # connection causes it to reconnect, which we don't
-            # want to do inside a rollback handler
             conn.info[ROLLBACK_CAUSE_KEY] = exc_info[1]
-        # NOTE(zzzeek) this eliminates a reference cycle between tracebacks
-        # that would occur in Python 3 only, which has been shown to occur if
-        # this function were in fact part of the traceback.  That's not the
-        # case here however this is left as a defensive measure.
         del exc_info
 
-    # try to clear the "cause" ASAP outside of savepoints,
-    # by grabbing the end of transaction events...
-    @event.listens_for(engine, "rollback")
-    @event.listens_for(engine, "commit")
-    def pop_exc_tx(conn):
-        # NOTE(zzzeek) accessing conn.info on an invalidated
-        # connection causes it to reconnect, which we don't
-        # want to do inside a rollback handler
+    @Listener.listens_for_rollback(engine)
+    @Listener.listens_for_commit(engine)
+    def pop_cause_on_transaction(conn):
         if not conn.invalidated:
             conn.info.pop(ROLLBACK_CAUSE_KEY, None)
 
-    # .. as well as connection pool checkin (just in case).
-    # the .info dictionary lasts as long as the DBAPI connection itself
-    # and is cleared out when the connection is recycled or closed
-    # due to invalidate etc.
-    @event.listens_for(engine, "checkin")
-    def pop_exc_checkin(dbapi_conn, connection_record):
+    @Listener.listens_for_checkin(engine)
+    def pop_cause_on_checkin(dbapi_conn, connection_record):
         _ = dbapi_conn
         connection_record.info.pop(ROLLBACK_CAUSE_KEY, None)
```

### Comparing `vbcore-1.3.0rc3/vbcore/db/exceptions.py` & `vbcore-2.0.0rc2/vbcore/db/exceptions.py`

 * *Files 15% similar despite different names*

```diff
@@ -17,28 +17,29 @@
 """
 from sqlalchemy.exc import SQLAlchemyError
 
 
 class DBError(SQLAlchemyError):
     """
     Base exception for all custom database exceptions.
-
-    :kwarg inner_exception: an original exception which was wrapped with
-        DBError or its subclasses.
     """
 
     def __init__(self, inner_exception=None):
+        """
+        @param inner_exception: an original exception which was wrapped
+            with DBError or its subclasses
+        """
         self.inner_exception = inner_exception
         super().__init__(str(inner_exception))
 
     @property
-    def error_type(self):
+    def error_type(self) -> str:
         return self.__class__.__name__
 
-    def as_dict(self):
+    def as_dict(self) -> dict:
         return {
             "error": self.error_type,
             "message": (
                 ", ".join(self.inner_exception.args)
                 if isinstance(self.inner_exception, Exception)
                 else self.inner_exception
             ),
@@ -51,25 +52,26 @@
     Raised when made an attempt to write to a unique column the same entry as
     existing one. :attr: `columns` available on an instance of the exception
     and could be used at error handling::
        try:
            instance_type_ref.save()
        except DBDuplicateEntry as e:
            if 'colname' in e.columns:
-               # Handle error.
-
-    :kwarg columns: a list of unique columns have been attempted to write a
-        duplicate entry.
-    :type columns: list
-    :kwarg value: a value which has been attempted to write. The value will
-        be None, if we can't extract it for a particular database backend. Only
-        MySQL and PostgreSQL 9.x are supported right now.
+               # Handle error
     """
 
     def __init__(self, columns=None, value=None, inner_exception=None):
+        """
+        @param columns: a list of unique columns have been attempted to write
+            a duplicate entry.
+        @param value: a value which has been attempted to write. The value will be None,
+            if we can't extract it for a particular database backend.
+            Only MySQL and PostgreSQL 9.x are supported right now.
+        @param inner_exception:
+        """
         self.value = value
         self.columns = columns or []
         super().__init__(inner_exception)
 
     def as_dict(self):
         return {
             "error": self.error_type,
@@ -79,129 +81,129 @@
 
 
 class DBConstraintError(DBError):
     """
     Check constraint fails for column error.
     Raised when made an attempt to write to a column a value that does not
     satisfy a CHECK constraint.
-
-    :kwarg table: the table name for which the check fails
-    :type table: str
-    :kwarg check_name: the table of the check that failed to be satisfied
-    :type check_name: str
     """
 
     def __init__(self, table, check_name, inner_exception=None):
+        """
+        @param table: the table name for which the check fails
+        @param check_name: the table of the check that failed to be satisfied
+        @param inner_exception:
+        """
         self.table = table
         self.check_name = check_name
         super().__init__(inner_exception)
 
-    def as_dict(self):
+    def as_dict(self) -> dict:
         return {
             "error": self.error_type,
             "table": self.table,
             "check_name": self.check_name,
         }
 
 
 class DBReferenceError(DBError):
     """
     Foreign key violation error.
-
-    :param table: a table name in which the reference is directed.
-    :type table: str
-    :param constraint: a problematic constraint name.
-    :type constraint: str
-    :param key: a broken reference key name.
-    :type key: str
-    :param key_table: a table name which contains the key.
-    :type key_table: str
     """
 
     def __init__(self, table, constraint, key, key_table, inner_exception=None):
+        """
+        @param table: a table name in which the reference is directed.
+        @param constraint: a problematic constraint name.
+        @param key: a broken reference key name.
+        @param key_table: a table name which contains the key.
+        @param inner_exception:
+        """
         self.key = key
         self.table = table
         self.key_table = key_table
         self.constraint = constraint
         super().__init__(inner_exception)
 
-    def as_dict(self):
+    def as_dict(self) -> dict:
         return {
             "error": self.error_type,
             "table": self.table,
             "key_table": self.key_table,
             "key": self.key,
             "constraint": self.constraint,
         }
 
 
 class DBNonExistentConstraint(DBError):
     """
     Constraint does not exist.
-
-    :param table: table name
-    :type table: str
-    :param constraint: constraint name
-    :type table: str
     """
 
     def __init__(self, table, constraint, inner_exception=None):
+        """
+        @param table: table name
+        @param constraint: constraint name
+        @param inner_exception:
+        """
         self.table = table
         self.constraint = constraint
         super().__init__(inner_exception)
 
-    def as_dict(self):
+    def as_dict(self) -> dict:
         return {
             "error": self.error_type,
             "table": self.table,
             "constraint": self.constraint,
         }
 
 
 class DBNonExistentTable(DBError):
     """
     Table does not exist.
-
-    :param table: table name
-    :type table: str
     """
 
     def __init__(self, table, inner_exception=None):
+        """
+        @param table: table name
+        @param inner_exception:
+        """
         self.table = table
         super().__init__(inner_exception)
 
-    def as_dict(self):
+    def as_dict(self) -> dict:
         return {
             "error": self.error_type,
             "table": self.table,
         }
 
 
 class DBNonExistentDatabase(DBError):
     """
     Database does not exist.
-
-    :param database: database name
-    :type database: str
     """
 
     def __init__(self, database, inner_exception=None):
+        """
+        @param database: database name
+        @param inner_exception:
+        """
         self.database = database
         super().__init__(inner_exception)
 
-    def as_dict(self):
+    def as_dict(self) -> dict:
         return {
             "error": self.error_type,
             "database": self.database,
         }
 
 
 class DBDeadlock(DBError):
     """
-    Database dead lock error.
+    Database deadlock error.
     Deadlock is a situation that occurs when two or more different database
     sessions have some data locked, and each database session requests a lock
     on the data that another, different, session has already locked.
     """
 
 
 class DBInvalidUnicodeParameter(DBError):
```

### Comparing `vbcore-1.3.0rc3/vbcore/db/mysql_dumper.py` & `vbcore-2.0.0rc2/vbcore/db/mysql_dumper.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,38 +1,39 @@
 import io
 import os
 import tarfile
 import typing as t
 from dataclasses import dataclass
 from datetime import datetime
 from itertools import groupby
-from subprocess import CompletedProcess, PIPE, run as run_subprocess
+from subprocess import CompletedProcess, PIPE, run as run_subprocess  # nosec
 
 from vbcore.base import BaseLoggerMixin
 from vbcore.date_helper import DateTimeFmt
 from vbcore.net.helpers import Url
+from vbcore.types import CoupleStr, OptInt, OptStr, StrList, StrTuple
 
-CmdLine = t.List[str]
+CmdLine = StrList
 
 
 @dataclass(frozen=True)
 class MySQLDump:
     database: str
     table: str
     dump: bytes
 
 
 class MySQLDumper:
     def __init__(
         self,
         username: str,
         password: str,
-        hostname: t.Optional[str] = None,
-        port: t.Optional[int] = None,
-        ignore_databases: t.Optional[t.List[str]] = None,
+        hostname: OptStr = None,
+        port: OptInt = None,
+        ignore_databases: t.Optional[StrList] = None,
     ):
         self.username = username
         self.password = password
         self.port = port or 3306
         self.hostname = hostname or "localhost"
         self.ignore_databases = (ignore_databases or []) + [
             "information_schema",
@@ -48,66 +49,64 @@
             f"--host={self.hostname}",
             f"--port={self.port}",
         ]
 
     def mysql_cmdline(
         self,
         statement: str,
-        *args,
-        database: t.Optional[str] = None,
+        *args: str,
+        database: OptStr = None,
     ) -> CmdLine:
         return [
             "mysql",
             *self.base_options,
             f"--database={database}" if database else "",
             "--skip-column-names",
             "--execute",
             *args,
             f"{statement};",
         ]
 
     def mysqldump_cmdline(
         self,
-        *args,
-        database: t.Optional[str] = None,
-        table: t.Optional[str] = None,
+        *args: str,
+        database: OptStr = None,
+        table: OptStr = None,
     ) -> CmdLine:
-        dump_args: t.Tuple[str, ...]
+        dump_args: StrTuple
         if database:
             dump_args = ("--databases", database) if not table else (database, table)
         else:
             dump_args = ("--all-databases",)
 
         return ["mysqldump", *self.base_options, *args, *dump_args]
 
     @classmethod
     def execute_binary(cls, cmdline: CmdLine, **kwargs) -> CompletedProcess:
-        return run_subprocess(cmdline, check=True, stdout=PIPE, **kwargs)
+        return run_subprocess(cmdline, check=True, stdout=PIPE, **kwargs)  # nosec
 
     @classmethod
     def execute_text(cls, cmdline: CmdLine) -> t.Iterator[str]:
         result = cls.execute_binary(cmdline, text=True)
         return filter(None, result.stdout.split(os.linesep))
 
-    def get_databases(
-        self, prefix: t.Optional[str] = None
-    ) -> t.Generator[str, None, None]:
+    def get_databases(self, prefix: OptStr = None) -> t.Generator[str, None, None]:
         filter_arg = f"like '{prefix}%'" if prefix else ""
         cmdline = self.mysql_cmdline(f"show databases {filter_arg}")
         for database in self.execute_text(cmdline):
             if database not in self.ignore_databases:
                 yield database
 
     def get_tables(self, database: str) -> t.Iterator[str]:
         cmdline = self.mysql_cmdline("show tables", database=database)
         return self.execute_text(cmdline)
 
     def all_tables(
-        self, db_prefix: t.Optional[str] = None
-    ) -> t.Generator[t.Tuple[str, str], None, None]:
+        self, db_prefix: OptStr = None
+    ) -> t.Generator[CoupleStr, None, None]:
         for database in self.get_databases(db_prefix):
             for table in self.get_tables(database):
                 yield database, table
 
     def dump_table(self, database: str, table: str) -> MySQLDump:
         cmdline = self.mysqldump_cmdline(database=database, table=table)
         result = self.execute_binary(cmdline)
@@ -116,34 +115,30 @@
 
 class MysqlBackup(BaseLoggerMixin):
     def __init__(
         self,
         dumper: MySQLDumper,
         folder: str = ".",
         add_datetime: bool = True,
-        datetime_format: t.Optional[str] = None,
+        datetime_format: OptStr = None,
     ):
         self.dumper = dumper
         self.folder = folder
         self.add_datetime = add_datetime
         self.datetime_format = datetime_format
 
-    def prepare_filename(self, *args, ext: str) -> str:
+    def prepare_filename(self, *args: str, ext: str) -> str:
         current_datetime = None
         if self.add_datetime:
             _datetime_format = self.datetime_format or DateTimeFmt.AS_NUM
             current_datetime = datetime.utcnow().strftime(_datetime_format)
         filename = "_".join(filter(None, (*args, current_datetime)))
         return os.path.join(self.folder, f"{filename}.{ext}")
 
-    def backup_single_files(
-        self,
-        file_prefix: t.Optional[str] = None,
-        db_prefix: t.Optional[str] = None,
-    ):
+    def backup_single_files(self, file_prefix: OptStr = None, db_prefix: OptStr = None):
         for database, table in self.dumper.all_tables(db_prefix):
             self.log.info("dumping table: %s.%s ......", database, table)
             dump = self.dumper.dump_table(database, table)
             filename = self.prepare_filename(
                 file_prefix, f"{database}.{table}", ext="sql"
             )
             with open(filename, mode="wb") as file:
@@ -154,18 +149,18 @@
                 database,
                 table,
                 filename,
             )
 
     def backup_as_archive(
         self,
-        file_prefix: t.Optional[str] = None,
-        db_prefix: t.Optional[str] = None,
-        mode: t.Optional[str] = None,
-        ext: t.Optional[str] = None,
+        file_prefix: OptStr = None,
+        db_prefix: OptStr = None,
+        mode: OptStr = None,
+        ext: OptStr = None,
     ):
         _mode = mode or "w:gz"
         _ext = ext or "tar.gz"
         cursor = self.dumper.all_tables(db_prefix)
         for database, tables in groupby(cursor, key=lambda x: x[0]):
             filename = self.prepare_filename(file_prefix, database, ext=_ext)
             with tarfile.open(filename, mode=_mode) as file:
@@ -177,21 +172,21 @@
                     file.addfile(tarinfo, fileobj=io.BytesIO(dump.dump))
             self.log.info("database: %s successfully dumped at: %s", database, filename)
 
 
 def cli_wrapper(
     *,
     db_url: str,
-    ignore_databases: t.Optional[t.List[str]] = None,
+    ignore_databases: t.Optional[StrList] = None,
     folder: str = ".",
     add_datetime: bool = True,
-    datetime_format: t.Optional[str] = None,
+    datetime_format: OptStr = None,
     as_archive: bool = True,
-    file_prefix: t.Optional[str] = None,
-    db_prefix: t.Optional[str] = None,
+    file_prefix: OptStr = None,
+    db_prefix: OptStr = None,
 ):
     url = Url.from_raw(db_url)
     _db_prefix = db_prefix or url.path.strip("/")
 
     service = MysqlBackup(
         dumper=MySQLDumper(
             username=url.username,
```

### Comparing `vbcore-1.3.0rc3/vbcore/db/schema.py` & `vbcore-2.0.0rc2/vbcore/db/schema.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 
 from sqlalchemy import create_mock_engine, MetaData  # type: ignore
 from sqlalchemy.engine import Engine
 from sqlalchemy.exc import SQLAlchemyError
 from sqlalchemy.orm import class_mapper
 from sqlalchemy_schemadisplay import create_schema_graph, create_uml_graph
 
+from vbcore.types import OptStr
+
 
 def model_to_uml(
     module: str,
     show_operations: bool = False,
     show_attributes: bool = True,
     show_inherited: bool = True,
     show_datatypes: bool = True,
@@ -52,15 +54,15 @@
         show_indexes=show_indexes,
         concentrate=concentrate,
         rankdir=rankdir,
         **kwargs,
     )
 
 
-def dump_model_ddl(metadata: MetaData, dialect: t.Optional[str] = None):
+def dump_model_ddl(metadata: MetaData, dialect: OptStr = None):
     dialect = dialect or "sqlite"
 
     def executor(sql, *_, **__):
         compiled = sql.compile(dialect=engine.dialect).replace("\n\n", "")
         print(compiled, ";", sep="")  # type: ignore
 
     engine = create_mock_engine(f"{dialect}://", executor=executor)
```

### Comparing `vbcore-1.3.0rc3/vbcore/db/sqla.py` & `vbcore-2.0.0rc2/vbcore/db/sqla.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,60 +2,30 @@
 import typing as t
 from contextlib import contextmanager
 from dataclasses import make_dataclass
 from functools import partial
 
 import sqlalchemy as sa
 import sqlalchemy.exc
-from sqlalchemy.orm import declarative_base  # type: ignore
+from sqlalchemy.ext.declarative import as_declarative
 from sqlalchemy.orm import scoped_session, Session, sessionmaker
 
 from ..base import BaseDTO
+from ..types import StrDict, StrTuple
 from .events import Listener
 
 SessionType = t.Union[scoped_session, Session]
 LoadersType = t.Tuple[t.Type["LoaderModel"], ...]
 
 logger = logging.getLogger(__name__)
 
 
-class BaseModel:
-    __table__ = None
-    dto_class = None
-
-    def columns(self) -> t.Tuple[str, ...]:
-        if self.__table__ is None:
-            return ()
-        return tuple(self.__table__.columns.keys())
-
-    def to_dict(self) -> t.Dict[str, t.Any]:
-        return {col: getattr(self, col, None) for col in self.columns()}
-
-    # noinspection PyArgumentList
-    @classmethod
-    def from_dto(cls, dto):
-        if isinstance(dto, BaseDTO):
-            return cls(**dto.to_dict())
-        return cls(**dto)
-
-    def to_dto(self):
-        items = tuple((col, getattr(self, col, None)) for col in self.columns())
-        dto_class = self.dto_class
-        if self.dto_class is None:
-            dto_class = make_dataclass(
-                f"{self.__class__.__name__}DTO",
-                [(col, type(value)) for col, value in items],
-                bases=(BaseDTO,),
-                frozen=True,
-            )
-        return dto_class(**dict(items))
-
-
 class SQLAConnector:
     metadata = sa.MetaData()
+    views_metadata = sa.MetaData()
     session_class = scoped_session
 
     def __init__(
         self,
         str_conn: str,
         session_options: t.Optional[dict] = None,
         **kwargs,
@@ -66,20 +36,23 @@
 
     @staticmethod
     def register_loaders(session: SessionType, loaders: LoadersType):
         for loader in loaders:
             callback = partial(loader.load_values, session)
             Listener.register_after_create(loader.__table__, callback)
 
-    def create_all(self, loaders: LoadersType = ()):
+    def create_all(self, loaders: LoadersType = ()) -> None:
         if loaders:
             with self.connection() as session:
                 self.register_loaders(session, loaders)
         self.metadata.create_all(self.engine)
 
+    def drop_all(self) -> None:
+        self.metadata.drop_all(self.engine)
+
     def get_session(self, **options) -> SessionType:
         if options:
             return self.session_class(sessionmaker(self.engine, **options))
         if self._factory is None:
             self._factory = sessionmaker(self.engine, **self._session_options)
         return self.session_class(self._factory)
 
@@ -96,25 +69,65 @@
                 yield conn
                 conn.commit()
             except Exception:
                 conn.rollback()
                 raise
 
 
-Model = declarative_base(
-    metadata=SQLAConnector.metadata,
-    cls=BaseModel,
-    name=BaseModel.__name__,
-)
+class BaseModel:
+    __table__: sa.Table
+    dto_class: t.Type[BaseDTO]
+
+    def __init__(self, *_, **__):
+        """only to avoid warnings"""
+
+    def columns(self) -> StrTuple:
+        if self.__table__ is None:
+            return ()
+        return tuple(self.__table__.columns.keys())
+
+    def to_dict(self) -> StrDict:
+        return {col: getattr(self, col, None) for col in self.columns()}
+
+    @classmethod
+    def from_dto(cls, dto: t.Union[BaseDTO, dict]):
+        if isinstance(dto, BaseDTO):
+            return cls(**dto.to_dict())
+        return cls(**dto)
+
+    def to_dto(self):
+        items = tuple((col, getattr(self, col, None)) for col in self.columns())
+        dto_class = self.dto_class
+        if self.dto_class is None:
+            dto_class = make_dataclass(
+                f"{self.__class__.__name__}DTO",
+                [(col, type(value)) for col, value in items],
+                bases=(BaseDTO,),
+                frozen=True,
+            )
+        return dto_class(**dict(items))
+
+
+@as_declarative(metadata=SQLAConnector.metadata)
+class Model(BaseModel):
+    pass
+
+
+@as_declarative(metadata=SQLAConnector.views_metadata)
+class ViewModel(BaseModel):
+    """
+    NOTE: the models that maps the views must be in a separate declarative base
+    so the views are not affected by create_all and drop_all
+    """
 
 
-class LoaderModel(Model):  # type: ignore
+class LoaderModel(Model):
     __abstract__ = True
 
-    values: t.Tuple[t.Dict[str, t.Any], ...] = ()
+    values: t.Sequence[StrDict] = ()
 
     @classmethod
     def load_values(cls, session: Session, *_, **__):
         try:
             session.add_all(cls(**d) for d in cls.values)
             session.commit()
         except sqlalchemy.exc.SQLAlchemyError as exc:
```

### Comparing `vbcore-1.3.0rc3/vbcore/db/support.py` & `vbcore-2.0.0rc2/vbcore/db/support.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,96 +1,91 @@
-# based on https://github.com/enricobarzetti/sqlalchemy_get_or_create
 import typing as t
 
 from sqlalchemy import create_engine, inspect, tuple_
-from sqlalchemy.exc import (  # type: ignore
-    IntegrityError,
-    NoResultFound as NoResultError,
-)
+from sqlalchemy.exc import IntegrityError
 from sqlalchemy.orm import Query, Session
+from sqlalchemy.orm.exc import NoResultFound as NoResultError
 from sqlalchemy.sql import text as text_sql
 
-from vbcore.db.events import register_engine_events
+from vbcore.db.events import register_error_handlers
 from vbcore.db.sqla import Model
+from vbcore.db.views import register_views_compiler
+from vbcore.files import FileHandler
+from vbcore.types import StrTuple
 
 
 class SQLASupport:
-    def __init__(self, model: Model, session: Session, commit: bool = True):
+    def __init__(self, model: t.Type[Model], session: Session, commit: bool = True):
         """
-
-        :param model: a model class
-        :param session: a session object
+        @param model: a model class
+        @param session: a session object
+        @param commit: enable auto commit
         """
         self.session = session
         self.model = model
         self._commit = commit
 
     @staticmethod
     def _prepare_params(defaults: t.Optional[dict] = None, **kwargs) -> dict:
         """
-
-        :param defaults: overrides kwargs
-        :param kwargs: overridden by defaults
-        :return: merge of kwargs and defaults
+        @param defaults: overrides kwargs
+        @param kwargs: overridden by defaults
+        @return merge of kwargs and defaults
         """
         ret = {}
         defaults = defaults or {}
         ret.update(kwargs)
         ret.update(defaults)
         return ret
 
     def _create_object(
         self, lookup: dict, params: dict, lock: bool = False
     ) -> t.Tuple[t.Any, bool]:
         """
-
-        :param lookup: attributes used to find record
-        :param params: attributes used to create record
-        :param lock: flag used for atomic update
-        :return:
+        @param lookup: attributes used to find record
+        @param params: attributes used to create record
+        @param lock: flag used for atomic update
+        @return created object and is_created flag
         """
         obj = self.model(**params)  # type: ignore
         self.session.add(obj)
 
         with self.session.begin_nested():
             try:
                 self.session.flush()
             except IntegrityError:
                 self.session.rollback()
                 query = self.fetch(**lookup)
                 if lock:
                     query = query.with_for_update()
                     obj = query.one()
                 return obj, False
-            else:
-                return obj, True
+            return obj, True
 
     def get_or_create(
         self, defaults: t.Optional[dict] = None, **kwargs
     ) -> t.Tuple[t.Any, bool]:
         """
-
-        :param defaults: attribute used to create record
-        :param kwargs: filters used to fetch record or create
-        :return:
+        @param defaults: attribute used to create record
+        @param kwargs: filters used to fetch record or create
+        @return created object and is_created flag
         """
         try:
             return self.fetch(**kwargs).one(), False
         except NoResultError:
             params = self._prepare_params(defaults, **kwargs)
             return self._create_object(kwargs, params)
 
     def update_or_create(
         self, defaults: t.Optional[dict] = None, **kwargs
     ) -> t.Tuple[t.Any, bool]:
         """
-
-        :param defaults: attribute used to create record
-        :param kwargs: filters used to fetch record or create
-        :return:
+        @param defaults: attribute used to create record
+        @param kwargs: filters used to fetch record or create
+        @return updated object and is_created flag
         """
         defaults = defaults or {}
         with self.session.begin_nested():
             try:
                 query = self.fetch().with_for_update()
                 obj = query.filter_by(**kwargs).one()
             except NoResultError:
@@ -107,16 +102,16 @@
 
         return obj, False
 
     def fetch(self, *args, fields: tuple = (), **kwargs) -> Query:
         columns = fields or (self.model,)
         return self.session.query(*columns).filter(*args).filter_by(**kwargs)
 
-    def delete(self, *args, synchronize_session: str = "evaluate", **kwargs) -> int:
-        row_count = self.fetch(*args, **kwargs).delete(synchronize_session)
+    def delete(self, *args, synchronize: str = "evaluate", **kwargs) -> int:
+        row_count = self.fetch(*args, **kwargs).delete(synchronize)
         if self._commit:
             self.session.commit()
         return row_count
 
     def bulk_insert(self, records: t.Iterable[Model]):
         self.session.add_all(records)
         if self._commit:
@@ -125,41 +120,40 @@
     def get_primary_key(self, record: t.Optional[Model] = None) -> t.Tuple:
         return tuple(
             getattr(record or self.model, pk_item.name)
             for pk_item in inspect(self.model).primary_key  # type: ignore
         )
 
     def bulk_upsert(self, records: t.Iterable[Model]):
-        db_objects = {}
-        for record in records:
-            db_objects[self.get_primary_key(record)] = record
-
-        self.delete(
-            tuple_(*self.get_primary_key()).in_(list(db_objects.keys())),
-            synchronize_session="fetch",
-        )
+        entities = {self.get_primary_key(record): record for record in records}
+
+        pk_cols = self.get_primary_key()
+        pk_values = list(entities.keys())
+        self.delete(tuple_(*pk_cols).in_(pk_values), synchronize="fetch")
 
         self.session.flush()
-        self.session.add_all(list(db_objects.values()))
+        self.session.add_all(list(entities.values()))
         if self._commit:
             self.session.commit()
 
-    @staticmethod
-    def register_events(engine):
-        register_engine_events(engine)
+    @classmethod
+    def register_custom_handlers(cls, engine):
+        register_error_handlers(engine)
+        register_views_compiler()
 
-    @staticmethod
+    @classmethod
     def exec_from_file(
+        cls,
         url: str,
         filename: str,
         echo: bool = False,
         separator: str = ";\n",
-        skip_line_prefixes: tuple = ("--",),
+        skip_line_prefixes: StrTuple = ("--",),
     ):
         engine = create_engine(url, echo=echo)
-        with engine.connect() as conn, open(filename, encoding="utf-8") as f:
+        with engine.connect() as conn, FileHandler().open(filename) as f:
             for statement in f.read().split(separator):
-                for skip_line in skip_line_prefixes:
-                    if statement.startswith(skip_line):
+                for prefix in skip_line_prefixes:
+                    if statement.startswith(prefix):
                         break
                 else:
                     conn.execute(text_sql(statement))
```

### Comparing `vbcore-1.3.0rc3/vbcore/files.py` & `vbcore-2.0.0rc2/vbcore/files.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,36 +1,37 @@
 import os
 import tempfile
 import typing as t
 from dataclasses import dataclass
 
-try:
-    from chardet import UniversalDetector as Detector
-except ImportError:
-    Detector = None  # type: ignore
-
-
-OptStr = t.Optional[str]
+from vbcore.datastruct.lazy import LazyImporter
+from vbcore.exceptions import VBException
+from vbcore.types import OptStr
+
+Detector = LazyImporter.do_import(
+    "chardet:UniversalDetector",
+    message="'chardet' required, install it!",
+)
 
 
 @dataclass(frozen=True)
 class EncodingData:
     confidence: float
-    encoding: t.Optional[str]
-    language: t.Optional[str] = None
+    encoding: OptStr
+    language: OptStr = None
 
 
-class VBEncodingError(Exception):
+class VBEncodingError(VBException):
     def __init__(
         self,
         filename: str,
-        encoding: t.Optional[str],
+        encoding: OptStr,
         supported: t.List[str],
         confidence: t.Optional[float] = None,
-        language: t.Optional[str] = None,
+        language: OptStr = None,
     ):
         self.filename = filename
         self.encoding = encoding
         self.language = language
         self.supported = supported
         self.confidence = confidence
 
@@ -58,18 +59,21 @@
         encoding: OptStr = None,
         supporter_encodings: t.Sequence[str] = (),
     ):
         self.filename = filename
         self.encoding = encoding or "utf-8"
         self.supporter_encodings = supporter_encodings
 
-    def open(self, filename: OptStr = None, **kwargs):
+    def open(self, filename: OptStr = None, **kwargs) -> t.IO:
         encoding = kwargs.pop("encoding", self.encoding)
         return open(filename or self.filename, encoding=encoding, **kwargs)
 
+    def open_binary(self, filename: OptStr = None, **kwargs) -> t.IO:
+        return open(filename or self.filename, mode="rb", **kwargs)
+
     def num_lines(self, filename: OptStr = None) -> int:
         with self.open(filename) as file:
             return sum(1 for _ in file)
 
     @classmethod
     def skip(cls, file: t.IO, lines: int):
         for _ in range(0, lines):
@@ -78,28 +82,28 @@
             except StopIteration:
                 return
 
     def read_text(self, filename: OptStr = None, **kwargs) -> str:
         with self.open(filename, **kwargs) as file:
             return file.read()
 
-    @classmethod
-    def detect_encoding(cls, filename: str) -> EncodingData:
-        assert Detector is not None, "'chardet' required, install it!"
+    def detect_encoding(self, filename: OptStr = None) -> EncodingData:
         detector = Detector()
-        with open(filename, "rb") as file:
+        with self.open_binary(filename) as file:
             for line in file:
                 detector.feed(line)
                 if detector.done:
                     break
             detector.close()
 
         return EncodingData(**detector.result)
 
-    def check_encoding(self, filename: str, *extra_supported):
+    def check_encoding(
+        self, filename: OptStr = None, extra_supported: t.Sequence[str] = ()
+    ):
         encoding = self.detect_encoding(filename)
         supported_encodings = [
             self.encoding,
             *self.supporter_encodings,
             *extra_supported,
         ]
         if encoding.encoding not in supported_encodings:
```

### Comparing `vbcore-1.3.0rc3/vbcore/http/batch.py` & `vbcore-2.0.0rc2/vbcore/http/batch.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,40 +2,38 @@
 import typing as t
 
 import aiohttp
 
 from vbcore.batch import AsyncBatchExecutor
 from vbcore.datastruct import ObjectDict
 
+from ..types import OptInt, OptStr
 from . import HttpMethod
 from .client import DumpBodyType, HTTPBase, httpcode, ResponseData
 
 
 class HTTPBatch(HTTPBase, AsyncBatchExecutor):
     def __init__(
         self,
-        endpoint: t.Optional[str] = None,
+        endpoint: OptStr = None,
         dump_body: DumpBodyType = False,
         timeout: int = 10,
         raise_on_exc: bool = False,
         logger=None,
     ):
         HTTPBase.__init__(self, endpoint, dump_body, timeout, raise_on_exc, logger)
         AsyncBatchExecutor.__init__(self, return_exceptions=not self._raise_on_exc)
 
     async def http_request(
         self,
         dump_body: t.Optional[DumpBodyType] = None,
-        timeout: t.Optional[int] = None,
+        timeout: OptInt = None,
         **kwargs,
     ) -> ResponseData:
-        if dump_body is None:
-            dump_body = self._dump_body
-        else:
-            dump_body = self._normalize_dump_flag(dump_body)
+        dump_body = self.dump_body_flags(dump_body, **kwargs)
 
         try:
             self._logger.info(
                 "%s", self.dump_request(ObjectDict(**kwargs), dump_body[0])
             )
             async with aiohttp.ClientSession(
                 timeout=aiohttp.ClientTimeout(
@@ -48,15 +46,15 @@
                 except (aiohttp.ContentTypeError, ValueError, TypeError):
                     body = await resp.text()
 
                 try:
                     response = ResponseData(
                         body=body,
                         status=resp.status,
-                        headers=dict(**resp.headers),
+                        headers={**resp.headers},
                     )
                     log_resp = response
                     log_resp.text = response.body
                     log_resp = self.dump_response(log_resp, dump_body[1])
                     resp.raise_for_status()
                     self._logger.info("%s", log_resp)
                 except aiohttp.ClientResponseError as exc:
```

### Comparing `vbcore-1.3.0rc3/vbcore/http/client.py` & `vbcore-2.0.0rc2/vbcore/http/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 from requests import auth, exceptions as http_exc, request as send_request, Response
 
 from vbcore.datastruct import ObjectDict
 from vbcore.http.headers import HeaderEnum
 from vbcore.uuid import get_uuid
 
+from ..types import OptStr
 from . import httpcode
 from .httpdumper import LazyHTTPDumper
 from .methods import HttpMethod
 
 HTTPStatusError = (http_exc.HTTPError,)
 NetworkError = (http_exc.ConnectionError, http_exc.Timeout)
 all_errors = (*HTTPStatusError, *NetworkError)
@@ -30,15 +31,15 @@
         self.body = body
         self.status = status
         self.headers = headers
         self.exception = exception
 
 
 class HTTPTokenAuth(auth.AuthBase):
-    def __init__(self, token: str, token_type: t.Optional[str] = None):
+    def __init__(self, token: str, token_type: OptStr = None):
         self.token = token
         self.token_type = token_type or "Bearer"
 
     def __eq__(self, other):
         other_token = getattr(other, "token", None)
         other_token_type = getattr(other, "token_type", None)
         return self.token_type == other_token_type and self.token == other_token
@@ -59,51 +60,69 @@
         timeout: int = 10,
         raise_on_exc: bool = False,
         logger=None,
     ):
         self._timeout = timeout
         self._endpoint = endpoint
         self._raise_on_exc = raise_on_exc
-        self._dump_body = self._normalize_dump_flag(dump_body)
+        self._dump_body = self.normalize_dump_flags(dump_body)
         self._logger = logger or logging.getLogger(self.__module__)
 
-    @staticmethod
-    def _normalize_dump_flag(
+    @classmethod
+    def normalize_dump_flags(
+        cls,
         dump_body: t.Optional[DumpBodyType] = None,
     ) -> t.Tuple[bool, bool]:
         if isinstance(dump_body, bool):
             return dump_body, dump_body
         if not dump_body:
             return False, False
         return dump_body
 
+    def dump_body_flags(
+        self, dump_body: t.Optional[DumpBodyType] = None, **kwargs
+    ) -> t.Tuple[bool, bool]:
+        if dump_body is None:
+            dump_body = self._dump_body
+        else:
+            dump_body = self.normalize_dump_flags(dump_body)
+        if kwargs.get("stream") is True:  # if stream not dump response body
+            dump_body = (dump_body[0], False)
+        return dump_body
+
     def normalize_url(self, url: str) -> str:
         if url.startswith("http"):
             return url
 
         return f"{self._endpoint}/{url.lstrip('/')}"
 
     def request(
         self,
         uri: str,
         method: str = HttpMethod.GET,
         dump_body: t.Optional[DumpBodyType] = None,
         raise_on_exc: bool = False,
         **kwargs,
     ) -> ResponseData:
-        raise NotImplementedError  # pragma: no cover
+        """
+        @param uri:
+        @param method:
+        @param dump_body:
+        @param raise_on_exc:
+        @param kwargs:
+        """
 
 
 class HTTPClient(HTTPBase):
     def __init__(
         self,
         endpoint: str,
-        token: t.Optional[str] = None,
-        username: t.Optional[str] = None,
-        password: t.Optional[str] = None,
+        token: OptStr = None,
+        username: OptStr = None,
+        password: OptStr = None,
         auth_with: t.Optional[auth.AuthBase] = None,
         **kwargs,
     ):
         super().__init__(endpoint, **kwargs)
         self._token = token
         self._username = username
         self._password = password
@@ -132,21 +151,15 @@
         uri: str,
         method: str = HttpMethod.GET,
         dump_body: t.Optional[DumpBodyType] = None,
         raise_on_exc: bool = False,
         **kwargs,
     ) -> ResponseData:
         kwargs["auth"] = self.get_auth()
-
-        if dump_body is None:
-            dump_body = self._dump_body
-        else:
-            dump_body = self._normalize_dump_flag(dump_body)
-        if kwargs.get("stream") is True:  # if stream not dump response body
-            dump_body = (dump_body[0], False)
+        dump_body = self.dump_body_flags(dump_body, **kwargs)
 
         try:
             url = self.normalize_url(uri)
             req = ObjectDict(method=method, url=url, **kwargs)
             self._logger.info("%s", self.dump_request(req, dump_body=dump_body[0]))
             timeout = kwargs.pop("timeout", None) or self._timeout
             response = send_request(method, url, timeout=timeout, **kwargs)
@@ -200,15 +213,15 @@
         return self.request(uri, method=HttpMethod.OPTIONS, **kwargs)
 
     def head(self, uri: str, **kwargs) -> ResponseData:
         return self.request(uri, method=HttpMethod.HEAD, **kwargs)
 
 
 class JsonRPCClient(HTTPClient):
-    def __init__(self, endpoint, uri, version="2.0", **kwargs):
+    def __init__(self, endpoint: str, uri: str, version: str = "2.0", **kwargs):
         super().__init__(endpoint, raise_on_exc=True, **kwargs)
         self._uri = uri
         self._version = version
         self._request_id = None
 
     @property
     def request_id(self):
@@ -225,17 +238,17 @@
         return self._request(method, **kwargs)
 
     def _request(self, method, params=None, **kwargs):
         kwargs.setdefault("raise_on_exc", True)
         resp = super().request(
             self._uri,
             method=HttpMethod.POST,
-            json=dict(
-                jsonrpc=self._version,
-                method=method,
-                params=params or {},
-                id=self._request_id,
-            ),
+            json={
+                "jsonrpc": self._version,
+                "method": method,
+                "params": params or {},
+                "id": self._request_id,
+            },
             **kwargs,
         )
 
         return resp.body or ObjectDict()
```

### Comparing `vbcore-1.3.0rc3/vbcore/http/headers.py` & `vbcore-2.0.0rc2/vbcore/http/headers.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import enum
 
-from vbcore.datastruct import IStrEnum, LStrEnum, StrEnum
+from vbcore.enums import IStrEnum, LStrEnum, StrEnum
 
 
 class TypeEnum(LStrEnum):
     APPLICATION = enum.auto()
     AUDIO = enum.auto()
     IMAGE = enum.auto()
     TEXT = enum.auto()
```

### Comparing `vbcore-1.3.0rc3/vbcore/http/httpcode.py` & `vbcore-2.0.0rc2/vbcore/http/httpcode.py`

 * *Files identical despite different names*

### Comparing `vbcore-1.3.0rc3/vbcore/http/httpdumper.py` & `vbcore-2.0.0rc2/vbcore/http/httpdumper.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from vbcore import json
-from vbcore.datastruct import Dumper
+from vbcore.datastruct.lazy import Dumper
 
 
 class BaseHTTPDumper:
     @classmethod
     def dump_headers(cls, hdr, only=()):
         """
         dumps http headers: useful for logging
 
-        :param hdr: headers' dictionary
-        :param only: list of headers key to dump
-        :return: string representation of headers
+        @param hdr: headers' dictionary
+        @param only: list of headers key to dump
+        @return: string representation of headers
                 k1: v1
                 k2: v2
         """
         hdr = hdr or {}
         if only:
             hdr = {k: hdr[k] for k in only if k in hdr}
 
@@ -23,16 +23,16 @@
 
     @classmethod
     def response_filename(cls, headers):
         """
         get filename from Content-Disposition header.
         i.e.: attachment; filename="<file name.ext>"
 
-        :param headers: http headers dict
-        :return: only the file name
+        @param headers: http headers dict
+        @return: only the file name
         """
         headers = headers or {}
         hdr = headers.get("Content-Disposition")
         if not hdr:
             return None  # pragma: no cover
 
         tmp = hdr.split(";")
@@ -42,42 +42,40 @@
         if len(tmp) > 1:
             return tmp[1].strip('"').lstrip("<").rstrip(">")
         return None
 
     @classmethod
     def dump_body(cls, resp):
         """
-
-        :param resp: Response instance
-        :return:
+        @param resp: Response instance
+        @return:
         """
         return (
             getattr(resp, "text", None)
             or getattr(resp, "data", None)
             or getattr(resp, "body", None)
         )
 
     @classmethod
     def dump_status(cls, resp):
         """
-
-        :param resp: Response instance
-        :return:
+        @param resp: Response instance
+        @return:
         """
         return getattr(resp, "status_code", None) or getattr(resp, "status", None)
 
     @classmethod
     def dump_request(cls, req, dump_body=None, only_hdr=()):
         """
         dump http request: useful for logging
 
-        :param req: Request instance
-        :param dump_body: flag to enable or disable dump of request's body (overrides default)
-        :param only_hdr: dump only a subset of headers
-        :return: prettified representation of input as string
+        @param req: Request instance
+        @param dump_body: flag to enable or disable dump of request's body (overrides default)
+        @param only_hdr: dump only a subset of headers
+        @return: prettified representation of input as string
         """
         body = ""
         if dump_body is True:
             body = getattr(req, "json", None)
             if body:
                 body = json.dumps(body)
             else:
@@ -91,18 +89,18 @@
         return f"requested {req.method} {req.url}{headers}{body}"
 
     @classmethod
     def dump_response(cls, resp, dump_body=None, only_hdr=()):
         """
         dump http response: useful for logging
 
-        :param resp: Response instance
-        :param dump_body: flag to enable or disable dump of response's body (overrides default)
-        :param only_hdr: dump only a subset of headers
-        :return: prettified representation of input as string
+        @param resp: Response instance
+        @param dump_body: flag to enable or disable dump of response's body (overrides default)
+        @param only_hdr: dump only a subset of headers
+        @return: prettified representation of input as string
         """
         body = ""
         if dump_body is True:
             body = cls.response_filename(resp.headers) or cls.dump_body(resp)
             body = f"\nbody:\n{body}" if body else ""
 
         try:
```

### Comparing `vbcore-1.3.0rc3/vbcore/http/proxy.py` & `vbcore-2.0.0rc2/vbcore/http/proxy.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from abc import ABC, abstractmethod
 
 from vbcore.datastruct import ObjectDict
 from vbcore.http import httpcode, HttpMethod
 from vbcore.http.client import HTTPBase, HTTPClient, JsonRPCClient
 from vbcore.http.headers import ContentTypeEnum, HeaderEnum
 from vbcore.http.rpc import rpc_error_to_httpcode
+from vbcore.types import OptBool, OptStr
 
 
 class Request(t.NamedTuple):
     host: str
     url: str
     method: str
     headers: dict
@@ -20,54 +21,54 @@
 class Response(t.NamedTuple):
     status: int
     headers: dict
     body: t.Any = None
     exception: t.Optional[Exception] = None
 
 
-class IncomingRequestData(ABC):
+class IncomingRequestData(ABC):  # TODO refactor this
     @classmethod
     @abstractmethod
     def url(cls) -> str:
-        pass
+        raise NotImplementedError
 
     @classmethod
     @abstractmethod
     def method(cls) -> str:
-        pass
+        raise NotImplementedError
 
     @classmethod
     @abstractmethod
     def body(cls):
-        pass
+        raise NotImplementedError
 
     @classmethod
     @abstractmethod
     def headers(cls) -> t.Dict[str, str]:
-        pass
+        raise NotImplementedError
 
     @classmethod
     @abstractmethod
     def params(cls) -> t.Dict[str, t.Any]:
-        pass
+        raise NotImplementedError
 
 
 class ProxyRequest(ABC):
     client_class: t.Type[HTTPBase] = HTTPClient
 
     @property
     @abstractmethod
     def request_dto(self) -> t.Type[IncomingRequestData]:
-        ...
+        raise NotImplementedError
 
     def __init__(
         self,
-        host: t.Optional[str] = None,
-        url: t.Optional[str] = None,
-        method: t.Optional[str] = None,
+        host: OptStr = None,
+        url: OptStr = None,
+        method: OptStr = None,
         proxy_body: bool = False,
         proxy_headers: bool = False,
         proxy_params: bool = False,
         stream: bool = True,
         **kwargs,
     ):
         self._host = host
@@ -80,17 +81,15 @@
         self._stream = stream
 
     def perform(self, **kwargs) -> Response:
         request = self.prepare_request()
         response = self.proxy(request, **kwargs)
         return self.prepare_response(response)
 
-    def proxy(
-        self, data: Request, stream: t.Optional[bool] = None, **kwargs
-    ) -> ObjectDict:
+    def proxy(self, data: Request, stream: OptBool = None, **kwargs) -> ObjectDict:
         options = {**self._options, **kwargs}
         client = self.client_class(data.host, **options)
         return client.request(
             data.url,
             method=data.method,
             headers=data.headers,
             params=data.params,
@@ -145,17 +144,15 @@
     response_content_type: str = ContentTypeEnum.JSON
     client_class: t.Type[JsonRPCClient] = JsonRPCClient
 
     def __init__(self, *args, **kwargs):
         kwargs.setdefault("stream", False)
         super().__init__(*args, **kwargs)
 
-    def proxy(
-        self, data: Request, stream: t.Optional[bool] = None, **kwargs
-    ) -> ObjectDict:
+    def proxy(self, data: Request, stream: OptBool = None, **kwargs) -> ObjectDict:
         url = self.upstream_host()
         client = self.client_class(url, url, **kwargs)
 
         if self.request_method() == HttpMethod.GET:
             return client.request(
                 self.request_method(),
                 request_id=self.get_request_id(),
```

### Comparing `vbcore-1.3.0rc3/vbcore/http/rpc.py` & `vbcore-2.0.0rc2/vbcore/http/rpc.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from vbcore.datastruct import ObjectDict
+from vbcore.exceptions import VBException
 from vbcore.http import httpcode
 
 
-class RPCError(Exception):
+class RPCError(VBException):
     def __init__(self, code: int, message: str, data=None):
-        super().__init__(code, message)
+        super().__init__(message, code)
         self.code = code
         self.message = message
         self.data = data
 
     def as_dict(self) -> ObjectDict:
         return ObjectDict(code=self.code, message=self.message, data=self.data)
```

### Comparing `vbcore-1.3.0rc3/vbcore/http/useragent.py` & `vbcore-2.0.0rc2/vbcore/http/useragent.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,53 +1,53 @@
 import typing as t
 from dataclasses import dataclass
 
 from user_agents import parsers
 
-from vbcore.datastruct import DataClassDictable
+from vbcore.base import BaseDTO
 
 
 @dataclass(frozen=True)
-class Version(DataClassDictable):
+class Version(BaseDTO):
     string: str
     number: int
 
     def __str__(self):
         return f"{self.string}"
 
 
 @dataclass(frozen=True)
-class Client(DataClassDictable):
+class Client(BaseDTO):
     family: str
     version: Version
 
     def __str__(self):
         return f"{self.family} {self.version}"
 
 
 @dataclass(frozen=True)
-class DeviceType(DataClassDictable):
+class DeviceType(BaseDTO):
     computer: bool
     bot: bool
     mobile: bool
     tablet: bool
     email_client: bool
     touch_capable: bool
 
 
 @dataclass(frozen=True)
-class Device(DataClassDictable):
+class Device(BaseDTO):
     family: str
     brand: str
     model: str
     type: DeviceType
 
 
 @dataclass(frozen=True)
-class UserAgent(DataClassDictable):
+class UserAgent(BaseDTO):
     parser_class: t.ClassVar[t.Type[parsers.UserAgent]] = parsers.UserAgent
 
     raw: str
     operating_system: Client
     browser: Client
     device: Device
```

### Comparing `vbcore-1.3.0rc3/vbcore/importer.py` & `vbcore-2.0.0rc2/vbcore/importer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 import importlib
 import typing as t
 from types import ModuleType
 
+from vbcore.exceptions import VBException
 
-class ImporterError(Exception):
+
+class ImporterError(VBException):
     pass
 
 
 class ImporterModuleError(ImporterError):
     def __init__(self, name, exc: Exception):
-        self.exception = exc
         self.name = name
-        super().__init__(exc)
+        self.exception = exc
+        super().__init__(f"unable to import module: {name}", orig=exc)
 
 
 class ImporterValueError(ImporterError):
     def __init__(self, name: str):
         self.name = name
         super().__init__(f"class not registered: '{name}'")
 
@@ -77,15 +79,16 @@
     ) -> t.Any:
         mod, attr = cls.parse_string(name)
 
         try:
             module = importlib.import_module(mod, package)
         except ModuleNotFoundError as exc:
             if raise_exc:
-                raise ImporterModuleError(mod, exc) from exc
+                name = f"{package}.{mod}" if package else mod
+                raise ImporterModuleError(name, exc) from exc
             return None
 
         if attr is None:
             return module
 
         if raise_exc:
             try:
@@ -103,29 +106,28 @@
 
         return imported(*args, **kwargs) if args or kwargs else imported()
 
 
 class ImporterFactory:
     def __init__(
         self,
-        base_class: t.Optional[t.Type] = None,
         package: t.Optional[str] = None,
+        base_class: t.Optional[t.Type] = None,
         classes: t.Optional[t.Dict[str, str]] = None,
     ):
-        self.base_class = base_class
         self.package = package
+        self.base_class = base_class
         self.classes: t.Optional[t.Dict[str, str]] = {}
-        if classes:
-            self.register_classes(classes)
+        self.register_classes(classes or {})
 
-    def register_classes(self, classes: t.Optional[t.Dict[str, str]]):
+    def register_classes(self, classes: t.Optional[t.Dict[str, str]]) -> None:
         for key, value in classes.items():
             self.register_class(key, value)
 
-    def register_class(self, name: str, module_class: str):
+    def register_class(self, name: str, module_class: str) -> None:
         self.classes[name] = f".{module_class}" if self.package else module_class
 
     def get_instance(self, name: str, *args, **kwargs):
         return self.get_class(name, *args, call_with=True, **kwargs)
 
     def get_class(self, name: str, *args, call_with: bool = False, **kwargs):
         if name not in self.classes:
```

### Comparing `vbcore-1.3.0rc3/vbcore/json.py` & `vbcore-2.0.0rc2/vbcore/json.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 JSONDecodeError = json.JSONDecodeError
 
 try:
     # noinspection PyUnresolvedReferences
     from bson import ObjectId
     from bson.errors import InvalidId
-except ImportError:
+except ImportError:  # pragma: no cover
     ObjectId = str
     InvalidId = ValueError
 
 
 class SetsEncoderMixin(json.JSONEncoder):
     def default(self, o, *_, **__):
         if isinstance(o, (set, frozenset)):
@@ -45,15 +45,15 @@
         if isinstance(o, (datetime.datetime, datetime.date, datetime.time)):
             return o.isoformat()
         if isinstance(o, datetime.timedelta):
             return o.total_seconds()
         return super().default(o)
 
 
-class TypesEncoderMixin(json.JSONEncoder):
+class NamespaceEncoderMixin(json.JSONEncoder):
     def default(self, o, *_, **__):
         if isinstance(o, SimpleNamespace):
             return o.__dict__
         return super().default(o)
 
 
 class CollectionsEncoderMixin(json.JSONEncoder):
@@ -62,15 +62,15 @@
             return list(o)
         if isinstance(o, (defaultdict, OrderedDict, Counter)):
             return dict(o)
         try:
             # check for namedtuple compliant
             # noinspection PyProtectedMember
             return o._asdict()
-        except (AttributeError, TypeError):
+        except AttributeError:
             pass
 
         return super().default(o)
 
 
 class HexUUIDMixin(json.JSONEncoder):
     def default(self, o, *_, **__):
@@ -82,33 +82,33 @@
 class ObjectIdMixin(json.JSONEncoder):
     def default(self, o, *_, **__):
         if isinstance(o, ObjectId):
             return {"$oid": str(o)}
         return super().default(o)
 
 
-class DictableMethodMixin(json.JSONEncoder):
+class DictableMixin(json.JSONEncoder):
     methods = ("to_dict", "asdict", "dict", "as_dict", "todict")
 
     def default(self, o, *_, **__):
         for name in self.methods:
             method = getattr(o, name, None)
             if method is not None:
                 return method()
         return super().default(o)
 
 
 class JsonEncoder(
     BuiltinEncoderMixin,
     DateTimeEncoderMixin,
-    TypesEncoderMixin,
+    NamespaceEncoderMixin,
     CollectionsEncoderMixin,
     HexUUIDMixin,
     ObjectIdMixin,
-    DictableMethodMixin,
+    DictableMixin,
 ):
     """
     Extends all encoders provided with this module
     """
 
     def default(self, o, *_, **__):
         return super().default(o)
```

### Comparing `vbcore-1.3.0rc3/vbcore/jsonschema/schemas/jsonrpc.py` & `vbcore-2.0.0rc2/vbcore/jsonschema/schemas/jsonrpc.py`

 * *Files 6% similar despite different names*

```diff
@@ -41,15 +41,15 @@
             "response": Fields.type(
                 "array",
                 "object",
                 required=["jsonrpc"],
                 properties={
                     "jsonrpc": Fields.enum("2.0"),
                     "id": Fields.type("string", "number", "null"),
-                    "result": Fields.type("array", "object", "null"),
+                    "result": Fields.any,
                     "error": Fields.type(
                         "array",
                         "object",
                         properties={
                             "code": Fields.number,
                             "message": Fields.string,
                         },
```

### Comparing `vbcore-1.3.0rc3/vbcore/jsonschema/support.py` & `vbcore-2.0.0rc2/vbcore/jsonschema/support.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,25 @@
 import io
 import typing as t
 from functools import partial
 
 from vbcore import json
 from vbcore.datastruct import ObjectDict
+from vbcore.files import FileHandler
 from vbcore.http.client import HTTPClient
+from vbcore.net.helpers import Url
+from vbcore.types import StrDict, StrList, StrTuple
 
 try:
     import jsonschema as json_schema
-except ImportError as _exc:
+except ImportError as _exc:  # pragma: no cover
     raise ImportError("you must install 'jsonschema'") from _exc
 
 SchemaError = (json_schema.ValidationError, json_schema.SchemaError)
+SchemaErrorType = t.Union[json_schema.ValidationError, json_schema.SchemaError]
 
 
 class JSONSchema:
     service = json_schema
     schema_error = SchemaError
 
     loader = partial(json.loads)
@@ -25,50 +29,52 @@
 
     @classmethod
     def load_from_url(cls, url: str) -> ObjectDict:
         res = HTTPClient(url, raise_on_exc=True).get(url)
         return t.cast(ObjectDict, res.body)
 
     @classmethod
-    def load_from_file(cls, file: str, encoding: str = "utf-8", **kwargs) -> dict:
-        if file.startswith("file://"):
-            file = file[7:]
-
-        with open(file, encoding=encoding, **kwargs) as f:
-            return cls.loader(f.read())
+    def load_from_file(cls, filename: str, **kwargs) -> dict:
+        with FileHandler(filename).open(**kwargs) as file:
+            return cls.loader(file.read())
 
     @classmethod
     def validate(
         cls,
         data: dict,
         schema: t.Union[dict, str],
         raise_exc: bool = False,
         pretty_error: bool = False,
         checker=None,
     ) -> bool:
         if isinstance(schema, str):
-            if schema.startswith("https://") or schema.startswith("http://"):
+            url_schema = Url.from_raw(schema)
+            if url_schema.protocol in ("https", "http"):
                 schema = cls.load_from_url(schema)
-            elif schema.startswith("file://"):
-                schema = cls.load_from_file(schema)
+            elif url_schema.protocol in (None, "file"):
+                schema = cls.load_from_file(url_schema.path)
 
         try:
             checker = checker or cls.service.FormatChecker()
             cls.service.validate(data, schema, format_checker=checker)
         except cls.schema_error as exc:
             if not raise_exc:
                 return False
             if pretty_error:
                 raise ValueError(cls.error_report(exc, data)) from exc
             raise
         return True
 
     @classmethod
     def error_report(
-        cls, e, json_object: dict, lines_before: int = 8, lines_after: int = 8
+        cls,
+        e: SchemaErrorType,
+        json_object: dict,
+        lines_before: int = 8,
+        lines_after: int = 8,
     ) -> str:
         """
         From: https://github.com/ccpgames/jsonschema-errorprinter/blob/master/jsonschemaerror.py
 
         Generate a detailed report of a schema validation error.
         'e' is a jsonschema.ValidationError exception raised on 'json_object'.
 
@@ -140,38 +146,42 @@
         integer = ObjectDict(type=["integer", "null"])
         string = ObjectDict(type=["string", "null"])
         number = ObjectDict(type=["number", "null"])
         boolean = ObjectDict(type=["boolean", "null"])
 
     @classmethod
     def oneof(cls, *args, **kwargs) -> ObjectDict:
-        return ObjectDict(oneOf=args if len(args) > 1 else (*args, cls.null), **kwargs)
+        return ObjectDict(
+            oneOf=list(args) if len(args) > 1 else [*args, cls.null], **kwargs
+        )
 
     @classmethod
     def anyof(cls, *args, **kwargs) -> ObjectDict:
-        return ObjectDict(anyOf=args if len(args) > 1 else (*args, cls.null), **kwargs)
+        return ObjectDict(
+            anyOf=list(args) if len(args) > 1 else [*args, cls.null], **kwargs
+        )
 
     @classmethod
     def ref(cls, path: str, **kwargs) -> ObjectDict:
         return ObjectDict(**{"$ref": f"#{path}", **kwargs})
 
     @classmethod
     def enum(cls, *args, **kwargs) -> ObjectDict:
-        return ObjectDict(enum=args, **kwargs)
+        return ObjectDict(enum=list(args), **kwargs)
 
     @classmethod
     def type(cls, *args, **kwargs) -> ObjectDict:
-        return ObjectDict(type=args, **kwargs)
+        return ObjectDict(type=list(args), **kwargs)
 
     @classmethod
     def object(
         cls,
-        required: t.Union[t.List[str], t.Tuple[str, ...]] = (),
-        not_required: t.Union[t.List[str], t.Tuple[str, ...]] = (),
-        properties: t.Dict[str, t.Any] = None,
+        required: t.Union[StrList, StrTuple] = (),
+        not_required: t.Union[StrList, StrTuple] = (),
+        properties: t.Optional[StrDict] = None,
         all_required: bool = True,
         additional: bool = False,
         **kwargs,
     ) -> ObjectDict:
         properties = properties or {}
         if not required and all_required is True:
             required = [i for i in properties.keys() if i not in not_required]
```

### Comparing `vbcore-1.3.0rc3/vbcore/misc.py` & `vbcore-2.0.0rc2/vbcore/misc.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,17 @@
 import functools
 import math
 import re
 import signal
 import string
 import sys
 import typing as t
-from decimal import Decimal
 from random import SystemRandom
 from threading import Lock
 
-T = t.TypeVar("T")
-
 
 class Printer:
     function = print
     thread_lock = Lock()
 
     @classmethod
     def safe(cls, *args, **kwargs):
@@ -46,28 +43,14 @@
         if value.lower() in ("true", "false"):
             return value.lower() == "true"
         if value.lower() in ("y", "n"):
             return value.lower() == "y"
     return value
 
 
-def get_from_dict(d: dict, k, default=None):
-    """
-    get a value from dict without raising exceptions
-
-    :param d: dict
-    :param k: key
-    :param default: default value if k is missing
-    :return: d[k] or default
-    """
-    if isinstance(d, dict):
-        return d.get(k, default)
-    return default
-
-
 def to_int(n) -> t.Optional[int]:
     """
     cast input to int if an error occurred returns None
 
     :param n: input
     :return: int or None
     """
@@ -86,20 +69,34 @@
     """
     try:
         return float(n)
     except (TypeError, ValueError):
         return None
 
 
-def format_decimal(value: Decimal, precision: int = 8) -> str:
-    if value.is_zero():
-        return "0"
+def split_kwargs(
+    options: t.Iterable[str], **kwargs
+) -> t.Tuple[t.Dict[str, t.Any], t.Dict[str, t.Any]]:
+    """
+    split kwargs into 2 dict:
+        one with only `options` keys and another with the others
+
+    :param options: wanted keys
+    :param kwargs: all params
+    :return: 2 dict: wanted and unwanted
+    """
+    wanted = {}
+
+    for opt in options:
+        try:
+            wanted[opt] = kwargs.pop(opt)
+        except KeyError:
+            pass
 
-    str_fmt = f"{{:.{precision}f}}"
-    return str_fmt.format(value).rstrip("0").rstrip(".")
+    return wanted, kwargs
 
 
 def static_attr(name: str, value):
     def wrapper(func):
         setattr(func, name, value)
 
         @functools.wraps(func)
@@ -107,31 +104,14 @@
             return func(*args, **kwargs)
 
         return inner
 
     return wrapper
 
 
-def chunk_iterator(
-    iterable: t.Iterable[T], chunk_size: int
-) -> t.Generator[t.List[T], None, None]:
-    _iterable = iter(iterable)
-
-    while True:
-        chunk = []
-        try:
-            for _ in range(chunk_size):
-                chunk.append(next(_iterable))
-            yield chunk
-        except StopIteration:
-            if chunk:
-                yield chunk
-            break
-
-
 def random_string(length: int, alphabet: str = string.printable) -> str:
     return "".join(SystemRandom().choice(alphabet) for _ in range(length))
 
 
 class Signal:
     @classmethod
     def handle_terminate(cls, signum, frame, callback: t.Callable = lambda: None):
```

### Comparing `vbcore-1.3.0rc3/vbcore/net/sendmail.py` & `vbcore-2.0.0rc2/vbcore/net/sendmail.py`

 * *Files 24% similar despite different names*

```diff
@@ -4,22 +4,24 @@
 import smtplib
 import typing as t
 from email.mime.application import MIMEApplication
 from email.mime.base import MIMEBase
 from email.mime.multipart import MIMEMultipart
 from email.mime.text import MIMEText
 from email.utils import formatdate, make_msgid, parseaddr
-from smtplib import SMTP
 
 from email_validator import caching_resolver, validate_email, ValidatedEmail
 
+from vbcore.files import FileHandler
 from vbcore.misc import CommonRegex
+from vbcore.types import OptStr, StrList, StrTuple
 from vbcore.uuid import get_uuid
 
-AddressType = t.Union[str, t.Tuple[str, ...]]
+AddressType = t.Union[str, StrTuple]
+HeadersType = t.Dict[str, str]
 
 
 @dataclasses.dataclass
 class SMTPResponse:
     message_id: str
     response: t.Dict[str, t.Tuple[int, bytes]]
 
@@ -28,42 +30,40 @@
 class SMTPParams:
     host: str
     port: int
     timeout: int = 10
     debug: bool = False
     is_ssl: bool = False
     is_tls: bool = False
-    user: t.Optional[str] = None
-    password: t.Optional[str] = None
+    user: OptStr = None
+    password: OptStr = None
     sender: t.Optional[t.Union[str, t.Tuple[str, str]]] = None
 
 
 @dataclasses.dataclass(frozen=True)
 class MessageData:
     subject: str
     priority: int = 3
-    html: t.Optional[str] = None
-    text: t.Optional[str] = None
-    headers: t.Optional[t.Dict[str, str]] = None
-    message_id: t.Optional[str] = None
-    attachments: t.Optional[t.List[str]] = None
+    html: OptStr = None
+    text: OptStr = None
+    headers: t.Optional[HeadersType] = None
+    message_id: OptStr = None
+    attachments: t.Optional[StrList] = None
 
 
 @dataclasses.dataclass(frozen=True)
 class MessageAddresses:
     sender: str
     to: AddressType  # pylint: disable=invalid-name
     cc: AddressType = ()  # pylint: disable=invalid-name
     bcc: AddressType = ()
-    reply_to: t.Optional[str] = None
+    reply_to: OptStr = None
 
 
 class SendMail:
-    smtp_class: t.Type[smtplib.SMTP] = smtplib.SMTP
-
     def __init__(self, params: SMTPParams, **kwargs):
         self.params = params
         self._smtp_args = kwargs
         self._log = logging.getLogger(self.__module__)
 
     @classmethod
     def validate_email(cls, email: str, restricted: bool = True) -> ValidatedEmail:
@@ -72,17 +72,17 @@
         return validate_email(email, dns_resolver=caching_resolver())
 
     @classmethod
     def prepare_addresses(cls, addr: AddressType) -> str:
         return ",".join(addr) if isinstance(addr, tuple) else addr
 
     @classmethod
-    def add_attachments(cls, message: MIMEBase, files: t.List[str]):
+    def add_attachments(cls, message: MIMEBase, files: StrList):
         for filename in files:
-            with open(filename, "rb") as file:
+            with FileHandler(filename).open_binary() as file:
                 attach = MIMEApplication(file.read())
                 filename = os.path.basename(filename)
                 attach.add_header(
                     "Content-Disposition", f"attachment; filename={filename}"
                 )
                 message.attach(attach)
 
@@ -113,19 +113,21 @@
             message.attach(MIMEText(data.text, "plain"))
         if data.html:
             message.attach(MIMEText(data.html, "html"))
 
         cls.add_attachments(message, data.attachments or [])
         return message
 
-    def get_instance(self, **kwargs) -> SMTP:
-        params = self.params
-        smtp_class = smtplib.SMTP_SSL if params.is_ssl else self.smtp_class
+    def get_smtp_class(self) -> t.Union[t.Type[smtplib.SMTP_SSL], t.Type[smtplib.SMTP]]:
+        return smtplib.SMTP_SSL if self.params.is_ssl else smtplib.SMTP
+
+    def get_instance(self, **kwargs) -> t.Union[smtplib.SMTP_SSL, smtplib.SMTP]:
+        smtp_class = self.get_smtp_class()
         smtp_options = {**self._smtp_args, **kwargs}
-        return smtp_class(params.host, params.port, **smtp_options)  # type: ignore
+        return smtp_class(self.params.host, self.params.port, **smtp_options)
 
     def send(self, message: MIMEMultipart, **kwargs) -> SMTPResponse:
         params = self.params
         with self.get_instance(**kwargs) as server:
             if params.is_tls:
                 server.starttls()
             if params.user:
@@ -138,24 +140,24 @@
             )
 
     # pylint: disable=too-many-arguments,too-many-locals
     def send_message(
         self,
         subject: str,
         to: AddressType,
-        sender: t.Optional[str] = None,
+        sender: OptStr = None,
         priority: int = 3,
-        html: t.Optional[str] = None,
-        text: t.Optional[str] = None,
-        reply_to: t.Optional[str] = None,
+        html: OptStr = None,
+        text: OptStr = None,
+        reply_to: OptStr = None,
         cc: t.Optional[AddressType] = (),
         bcc: t.Optional[AddressType] = (),
-        headers: t.Optional[t.Dict[str, str]] = None,
-        message_id: t.Optional[str] = None,
-        attachments: t.Optional[t.List[str]] = None,
+        headers: t.Optional[HeadersType] = None,
+        message_id: OptStr = None,
+        attachments: t.Optional[StrList] = None,
         **kwargs,
     ) -> SMTPResponse:
         _sender = sender or str(self.params.sender) or self.params.user
         message = self.message(
             MessageAddresses(
                 to=to,
                 sender=_sender,
```

### Comparing `vbcore-1.3.0rc3/vbcore/net/sftp.py` & `vbcore-2.0.0rc2/vbcore/net/sftp.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,22 +2,24 @@
 import os.path
 import re
 from dataclasses import dataclass
 from typing import cast, Generator, Optional
 
 from paramiko import PKey, SFTPClient, Transport
 
+from vbcore.types import OptStr
+
 
 @dataclass(frozen=True)
 class SFTPOptions:
     host: str
     port: int
     user: str
-    password: Optional[str] = None
-    host_key: Optional[str] = None
+    password: OptStr = None
+    host_key: OptStr = None
 
 
 class SFTPHandler:
     def __init__(self, options: SFTPOptions):
         self.host = options.host
         self.port = options.port
         self.user = options.user
```

### Comparing `vbcore-1.3.0rc3/vbcore/net/socks_smtp.py` & `vbcore-2.0.0rc2/vbcore/net/socks_smtp.py`

 * *Files 24% similar despite different names*

```diff
@@ -22,23 +22,30 @@
         proxy_type: t.Optional[ProxyType] = None,
         **kwargs,
     ):
         self.proxy_args = kwargs
         self.proxy_type = proxy_type
         super().__init__(host, port, local_hostname, timeout, source_address)
 
-    def _get_socket(self, host, port, timeout):
+    def create_socks_connection(
+        self, host: str, port: int, timeout: int
+    ) -> socks.socksocket:
         if self.proxy_type is None:
             # noinspection PyProtectedMember,PyUnresolvedReferences
-            return super()._get_socket(host, port, timeout)
+            get_socket = super()._get_socket  # type: ignore
+            return get_socket(host, port, timeout)
 
         if self.debuglevel > 0:
             # noinspection PyUnresolvedReferences
-            self._print_debug("connect: to", (host, port), self.source_address)
+            print_debug = self._print_debug  # type: ignore
+            print_debug("connect to:", (host, port), self.source_address)
 
         return socks.create_connection(
             (host, port),
             timeout=timeout,
             source_address=self.source_address,
             proxy_type=self.proxy_type.value,
             **self.proxy_args,
         )
+
+    def _get_socket(self, host: str, port: int, timeout: int) -> socks.socksocket:
+        return self.create_socks_connection(host, port, timeout)
```

### Comparing `vbcore-1.3.0rc3/vbcore/rule_engine/base.py` & `vbcore-2.0.0rc2/vbcore/rule_engine/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,9 +48,9 @@
 @dataclass(frozen=True)
 class RuleInfo:
     id: str  # pylint: disable=invalid-name
     rule: RuleType
     evaluate: bool = False
     action: t.Optional[ActionRule] = NoneActionRule()
 
-    def __str__(self):
+    def __str__(self) -> str:
         return f"<{self.id} - {self.rule}>"
```

### Comparing `vbcore-1.3.0rc3/vbcore/rule_engine/engine.py` & `vbcore-2.0.0rc2/vbcore/rule_engine/engine.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,27 +16,27 @@
     ):
         self.raise_exc = raise_exc
         self.case_insensitive = case_insensitive
         self._context = context or Context(resolver=self.resolver)
         self._logger: logging.Logger = logging.getLogger(self.__module__)
 
     @property
-    def context(self):
+    def context(self) -> Context:
         return self._context
 
     @context.setter
     def context(self, context: Context):
         self._context = context
 
-    def resolver(self, thing, name):
+    def resolver(self, thing, name: str):
         if self.case_insensitive is True:
             return resolve_item(thing, name.lower())
         return resolve_item(thing, name)
 
-    def prepare_rule(self, rule: t.Union[str, Rule]) -> Rule:
+    def prepare_rule(self, rule: RuleType) -> Rule:
         if isinstance(rule, str):
             return Rule(rule, context=self.context)
         return rule
 
     def evaluate(self, rule: RuleType, data: dict) -> t.Any:
         rule = self.prepare_rule(rule)
         try:
```

### Comparing `vbcore-1.3.0rc3/vbcore/standalone/scheduler.py` & `vbcore-2.0.0rc2/vbcore/standalone/scheduler.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from io import StringIO
 
 from apscheduler import events as scheduler_events
 from apscheduler.job import Job
 from apscheduler.schedulers.base import BaseScheduler
 from apscheduler.schedulers.blocking import BlockingScheduler
 
-from vbcore.datastruct import Dumper, LazyDump
+from vbcore.datastruct.lazy import Dumper, LazyDump
 from vbcore.uuid import get_uuid
 
 
 class APScheduler:
     def __init__(
         self,
         *args,
@@ -21,15 +21,15 @@
         auto_start: bool = False,
         **kwargs,
     ):
         self.logger = logging.getLogger(self.__module__)
         super().__init__(*args, **kwargs)
         self._scheduler = scheduler(gconfig or {})
         self._events = events_to_listen or scheduler_events.EVENT_ALL
-        self._scheduler.add_listener(self._event_listener, self._events)
+        self._scheduler.add_listener(self.event_listener, self._events)
         if auto_start:
             self._scheduler.start()
 
     @classmethod
     def factory(
         cls, config: dict, scheduler_class: t.Optional[t.Type[BaseScheduler]] = None
     ) -> "APScheduler":
@@ -43,26 +43,26 @@
         return self._scheduler
 
     def dump_jobs(self) -> str:
         dump = StringIO()
         self._scheduler.print_jobs(out=dump)
         return dump.getvalue()
 
-    @staticmethod
-    def _repr_job_event(event: scheduler_events.SchedulerEvent):
+    @classmethod
+    def repr_job_event(cls, event: scheduler_events.SchedulerEvent):
         if isinstance(event, scheduler_events.JobEvent):
             return f"{repr(event)}-<{event.job_id}>-<{event.jobstore}>"
         return repr(event)
 
-    def _event_listener(self, event):
+    def event_listener(self, event):
         if not event.code & self._events:
             return
 
         self.logger.debug(
-            "received event %s", Dumper(event, callback=self._repr_job_event)
+            "received event %s", Dumper(event, callback=self.repr_job_event)
         )
         if event.code == scheduler_events.EVENT_JOB_ERROR:
             self.logger.error("An error occurred when executing job: %s", event.job_id)
             self.logger.exception(event.exception)
             self.logger.error(event.traceback)
         elif event.code == scheduler_events.EVENT_JOB_ADDED:
             self.logger.info("successfully added job: %s", event.job_id)
```

### Comparing `vbcore-1.3.0rc3/vbcore/standalone/wsgi_gunicorn.py` & `vbcore-2.0.0rc2/vbcore/standalone/wsgi_gunicorn.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 import os
 import typing as t
+from dataclasses import MISSING
 from functools import partial
 from multiprocessing import cpu_count
 
 from decouple import Choices, Csv, UndefinedValueError
 from gunicorn import util
 from gunicorn.app.base import BaseApplication  # type: ignore
 
-from vbcore.configurator import config, load_dotenv, MISSING
+from vbcore.configurator import config, load_dotenv
 from vbcore.importer import Importer
 
 # Supported env vars:
 #  - GU_BIND
 #  - GU_PID_FILE
 #  - GU_PROC_NAME
 #  - GU_TIMEOUT
```

### Comparing `vbcore-1.3.0rc3/vbcore/system.py` & `vbcore-2.0.0rc2/vbcore/system.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 import dataclasses
 import typing as t
 
 import psutil
 
-from vbcore.datastruct import DataClassDictable, ObjectDict
+from vbcore.base import BaseDTO
+from vbcore.datastruct import ObjectDict
 
 
 @dataclasses.dataclass(frozen=True)
-class SwapStat(DataClassDictable):
+class SwapStat(BaseDTO):
     total: int
     percent: float
     used: int
     free: int
     sin: int = 0
     sout: int = 0
 
 
 @dataclasses.dataclass(frozen=True)
-class MemoryStat(DataClassDictable):  # pylint: disable=too-many-instance-attributes
+class MemoryStat(BaseDTO):  # pylint: disable=too-many-instance-attributes
     total: int
     available: int
     percent: float
     used: int
     free: int
     active: int
     inactive: int
@@ -29,52 +30,52 @@
     cached: int
     shared: int
     slab: int
     swap: SwapStat
 
 
 @dataclasses.dataclass(frozen=True)
-class CpuFreq(DataClassDictable):
+class CpuFreq(BaseDTO):
     current: float
     min: float
     max: float
 
 
 @dataclasses.dataclass(frozen=True)
-class CpuTimes(DataClassDictable):
+class CpuTimes(BaseDTO):
     user: float
     nice: float
     system: float
     idle: float
     iowait: float
     irq: float
     softirq: float
     steal: float
     guest: float
     guest_nice: float
 
 
 @dataclasses.dataclass(frozen=True)
-class CpuStat(DataClassDictable):
+class CpuStat(BaseDTO):
     count: int
     percent: float
     freq: CpuFreq
     times: CpuTimes
 
 
 @dataclasses.dataclass(frozen=True)
-class DiskStat(DataClassDictable):
+class DiskStat(BaseDTO):
     total: int
     percent: float
     used: int
     free: int
 
 
 @dataclasses.dataclass(frozen=True)
-class NetStat(DataClassDictable):
+class NetStat(BaseDTO):
     bytes_sent: int
     bytes_recv: int
     packets_sent: int
     packets_recv: int
     errin: int
     errout: int
     dropin: int = 0
```

### Comparing `vbcore-1.3.0rc3/vbcore/tester/fetchmail.py` & `vbcore-2.0.0rc2/vbcore/tester/fetchmail.py`

 * *Files identical despite different names*

### Comparing `vbcore-1.3.0rc3/vbcore/tester/http.py` & `vbcore-2.0.0rc2/vbcore/tester/http.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,23 +2,23 @@
 import logging
 import typing as t
 
 from requests import request as http_client
 
 from vbcore.datastruct import ObjectDict
 from vbcore.http import httpcode, HttpMethod
+from vbcore.http.headers import ContentTypeEnum, HeaderEnum
 from vbcore.http.httpdumper import BaseHTTPDumper as HTTPDumper
 from vbcore.jsonschema.schemas.jsonrpc import JSONRPC
 
-from ..http.headers import ContentTypeEnum, HeaderEnum
+from .asserter import Asserter
 from .helpers import basic_auth_header
-from .mixins import JSONValidatorMixin, RegexMixin
 
 
-class TestHttpCall(HTTPDumper, JSONValidatorMixin, RegexMixin):
+class TestHttpCall(HTTPDumper):
     __test__ = False
     default_status_code = (httpcode.SUCCESS, 299)
     default_content_type = ContentTypeEnum.HTML
 
     def __init__(self, endpoint=None, auth=None, **__):
         self.auth = None
         self.response = None
@@ -43,30 +43,30 @@
 
     def assert_status_code(
         self, code: int, in_range: bool = False, is_in: bool = False
     ):
         status_code = self.response.status_code
         if type(code) in (list, tuple):
             if in_range:
-                self.assert_range(status_code, code)
+                Asserter.assert_range(status_code, code)
             if is_in:
-                self.assert_in(status_code, code)
+                Asserter.assert_in(status_code, code)
         else:
-            self.assert_equals(status_code, code)
+            Asserter.assert_equals(status_code, code)
 
     def assert_header(
         self, name: str, value: str, is_in: bool = False, regex: bool = False
     ):
         header = self.response.headers.get(name)
         if is_in:
-            self.assert_in(value, header)
+            Asserter.assert_in(value, header)
         elif regex:
-            self.assert_match(value, header)
+            Asserter.assert_match(value, header)
         else:
-            self.assert_equals(header, value)
+            Asserter.assert_equals(header, value)
 
     def assert_response(self, **kwargs):
         code = kwargs.get("status") or {
             "code": self.default_status_code,
             "in_range": True,
         }
         headers = kwargs.get("headers") or {}
@@ -111,21 +111,21 @@
     def json(self):
         try:
             if self.response.status_code != httpcode.NO_CONTENT and "json" in (
                 self.response.headers.get(HeaderEnum.CONTENT_TYPE) or ""
             ):
                 return self.response.get_json()
         except json.decoder.JSONDecodeError as exc:
-            assert False, f"Test that json is valid failed, got: {exc}"
+            raise AssertionError(f"Test that json is valid failed, got: {exc}") from exc
         return None
 
     def assert_response(self, **kwargs):
         super().assert_response(**kwargs)
         if kwargs.get("schema") is not None:
-            self.assert_schema(self.json, kwargs.get("schema"))
+            Asserter.assert_json_schema(self.json, kwargs.get("schema"))
 
 
 class TestJsonRPC(TestHttpApi):
     version = "2.0"
     default_schema = JSONRPC.RESPONSE
 
     # noinspection PyShadowingBuiltins
@@ -194,21 +194,21 @@
         request["url"] = url or self.endpoint
         return request, response
 
     def test_collection(self, request=None, response=None):
         req, res = self._normalize(request, response)
         res.setdefault(
             "status",
-            dict(code=(httpcode.SUCCESS, httpcode.PARTIAL_CONTENT), is_in=True),
+            {"code": (httpcode.SUCCESS, httpcode.PARTIAL_CONTENT), "is_in": True},
         )
         self.perform(req, res)
 
     def test_post(self, request=None, response=None):
         req, res = self._normalize(request, response, HttpMethod.POST)
-        res.setdefault("status", dict(code=httpcode.CREATED))
+        res.setdefault("status", {"code": httpcode.CREATED})
         self.perform(req, res)
 
     def test_get(self, res_id, request=None, response=None):
         req, res = self._normalize(request, response, url=self.resource_url(res_id))
         self.perform(req, res)
 
     def test_put(self, res_id, request=None, response=None):
@@ -217,11 +217,11 @@
         )
         self.perform(req, res)
 
     def test_delete(self, res_id, request=None, response=None):
         req, res = self._normalize(
             request, response, HttpMethod.DELETE, self.resource_url(res_id)
         )
-        res.setdefault("status", dict(code=httpcode.NO_CONTENT))
+        res.setdefault("status", {"code": httpcode.NO_CONTENT})
         res.setdefault("headers", {})
         res["headers"][HeaderEnum.CONTENT_TYPE] = None
         self.perform(req, res)
```

### Comparing `vbcore-1.3.0rc3/vbcore/tools/cli.py` & `vbcore-2.0.0rc2/vbcore/tools/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 import typing as t
 from functools import partial
 
 import click
 
 from vbcore.date_helper import DateFmt, DateTimeFmt
-from vbcore.misc import parse_value
 
 
 def option_as_dict(ctx, param, value):
     _ = ctx, param
     option = {}
     for opt in value:
         tokens = opt.split("=", 2)
         key, val = tokens if len(tokens) > 1 else (tokens, None)
-        option[key] = parse_value(val)
+        option[key] = val
     return option
 
 
 CliFile = partial(click.Path, file_okay=True, dir_okay=False)
 CliDir = partial(click.Path, file_okay=False, dir_okay=True)
 
 CliOutputFile = partial(CliFile, writable=True)
@@ -46,15 +45,15 @@
     date: t.ClassVar = partial(Cli.option, type=click.DateTime(DateFmt.ISO))
     datetime: t.ClassVar = partial(Cli.option, type=click.DateTime(DateTimeFmt.ISO))
     multi: t.ClassVar = partial(Cli.option, multiple=True, metavar="(multiple)")
     flag: t.ClassVar = partial(
         boolean, is_flag=True, default=False, help="[default: False]"
     )
     dict: t.ClassVar = partial(
-        multi, default={}, multiple=True, callback=option_as_dict, metavar="KEY=VAL"
+        multi, default={}, callback=option_as_dict, metavar="KEY[=VAL]"
     )
     verbose: t.ClassVar = partial(Cli.option, "-v", "--verbose", count=True)
 
     @classmethod
     def choice(
         cls, *args, values: t.Sequence[str], case_sensitive: bool = True, **kwargs
     ):
```

### Comparing `vbcore-1.3.0rc3/vbcore/tools/database.py` & `vbcore-2.0.0rc2/vbcore/tools/database.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from vbcore.db.mysql_dumper import cli_wrapper as mysql_dump_cli_wrapper
 from vbcore.loggers import Loggers
 from vbcore.tools.cli import Cli, CliOpt, CliOutputDir, CliReqOpt
 
 try:
     from vbcore.db.schema import db_to_schema, dump_model_ddl, model_to_uml
-except ImportError:
+except ImportError:  # pragma: no cover
     db_to_schema = dump_model_ddl = model_to_uml = None
 
 
 DIALECTS = ["sqlite", "mysql", "oracle", "postgresql", "mssql"]
 
 main = click.Group(name="database", help="tools for database")
```

### Comparing `vbcore-1.3.0rc3/vbcore/tools/entrypoint.py` & `vbcore-2.0.0rc2/vbcore/tools/entrypoint.py`

 * *Files identical despite different names*

### Comparing `vbcore-1.3.0rc3/vbcore/tools/initializer/init.py` & `vbcore-2.0.0rc2/vbcore/tools/initializer/init.py`

 * *Files identical despite different names*

### Comparing `vbcore-1.3.0rc3/vbcore/tools/scheduler.py` & `vbcore-2.0.0rc2/vbcore/tools/scheduler.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import click
 
 from vbcore.tools.cli import Cli, CliInputFile, CliReqOpt
 
 try:
     from vbcore.standalone.scheduler import APScheduler
-except ImportError:
+except ImportError:  # pragma: no cover
     APScheduler = None  # type: ignore
 
 from vbcore.yaml import load_yaml_file
 
 main = click.Group(name="scheduler", help="start the scheduler")
```

### Comparing `vbcore-1.3.0rc3/vbcore/uuid.py` & `vbcore-2.0.0rc2/vbcore/uuid.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,47 +1,41 @@
 import typing as t
 import uuid
 
+from vbcore.types import OptStr
+
 
 def get_uuid(
-    ver: int = 4, hexify: bool = True, ns=None, name=None
+    ver: int = 4,
+    hex_: bool = True,
+    name: OptStr = None,
+    ns: t.Optional[uuid.UUID] = None,
 ) -> t.Union[str, uuid.UUID]:
-    """
-
-    :param ver:
-    :param hexify:
-    :param ns:
-    :param name:
-    :return:
-    """
-    _uuid = None
-
     if ver == 1:
         _uuid = uuid.uuid1()
     elif ver == 3:
         _uuid = uuid.uuid3(ns or uuid.NAMESPACE_DNS, name)
     elif ver == 4:
         _uuid = uuid.uuid4()
     elif ver == 5:
         _uuid = uuid.uuid5(ns or uuid.NAMESPACE_DNS, name)
+    else:
+        raise TypeError(f"invalid uuid version {ver}")
 
-    return _uuid.hex if hexify else _uuid
-
+    return _uuid.hex if hex_ else _uuid
 
-def check_uuid(u: str, ver: int = 4, exc: bool = False) -> bool:
-    """
 
-    :param u:
-    :param ver:
-    :param exc:
-    :return:
-    """
+def check_uuid(
+    u: t.Union[str, uuid.UUID],
+    ver: int = 4,
+    raise_exc: bool = False,
+) -> bool:
     try:
         if isinstance(u, uuid.UUID):
             return True
 
         _uuid = uuid.UUID(u, version=ver)
         return u == (str(_uuid) if "-" in u else _uuid.hex)
-    except (ValueError, TypeError, AttributeError) as e:
-        if exc:
-            raise ValueError(f"'{u}' is an invalid UUID{ver}") from e
+    except (ValueError, TypeError, AttributeError) as exc:
+        if raise_exc:
+            raise ValueError(f"'{u}' is an invalid UUID{ver}") from exc
         return False
```

### Comparing `vbcore-1.3.0rc3/vbcore/yaml.py` & `vbcore-2.0.0rc2/vbcore/yaml.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
         .*      # matches any number of any characters
     """,
     re.VERBOSE,
 )
 
 
 def loads(data, loader=None, as_object: bool = True):
-    data = yaml.load(data, Loader=loader or yaml.Loader)
+    data = yaml.load(data, Loader=loader or yaml.Loader)  # nosec
     if as_object:
         return ObjectDict.normalize(data)
     return data
 
 
 def load_yaml_file(filename: str, encoding="utf-8", **kwargs):
     with open(filename, encoding=encoding) as f:
```

### Comparing `vbcore-1.3.0rc3/vbcore.egg-info/SOURCES.txt` & `vbcore-2.0.0rc2/vbcore.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -21,51 +21,71 @@
 requirements/requirements-scheduler.txt
 requirements/requirements-test.in
 requirements/requirements-test.txt
 requirements/requirements.in
 requirements/requirements.txt
 vbcore/__init__.py
 vbcore/__main__.py
+vbcore/aio.py
 vbcore/base.py
 vbcore/batch.py
 vbcore/configurator.py
 vbcore/crc.py
 vbcore/csvfile.py
-vbcore/datastruct.py
 vbcore/date_helper.py
+vbcore/dispatcher.py
+vbcore/enums.py
+vbcore/exceptions.py
+vbcore/factory.py
 vbcore/files.py
 vbcore/importer.py
 vbcore/json.py
+vbcore/lambdas.py
 vbcore/loggers.py
 vbcore/misc.py
 vbcore/system.py
+vbcore/types.py
 vbcore/uuid.py
 vbcore/version.py
 vbcore/yaml.py
 vbcore.egg-info/PKG-INFO
 vbcore.egg-info/SOURCES.txt
 vbcore.egg-info/dependency_links.txt
 vbcore.egg-info/entry_points.txt
 vbcore.egg-info/not-zip-safe
 vbcore.egg-info/requires.txt
 vbcore.egg-info/top_level.txt
 vbcore/crypto/__init__.py
 vbcore/crypto/argon.py
 vbcore/crypto/base.py
+vbcore/crypto/bcrypt.py
+vbcore/crypto/exceptions.py
+vbcore/crypto/factory.py
+vbcore/crypto/hashes.py
+vbcore/datastruct/__init__.py
+vbcore/datastruct/buffer.py
+vbcore/datastruct/cache.py
+vbcore/datastruct/dictionaries.py
+vbcore/datastruct/lazy.py
+vbcore/datastruct/misc.py
+vbcore/datastruct/orderer_set.py
 vbcore/db/__init__.py
 vbcore/db/events.py
 vbcore/db/exceptions.py
+vbcore/db/listener.py
 vbcore/db/mixins.py
 vbcore/db/mysql_dumper.py
 vbcore/db/schema.py
 vbcore/db/sqla.py
 vbcore/db/support.py
+vbcore/db/views.py
 vbcore/http/__init__.py
 vbcore/http/batch.py
 vbcore/http/client.py
+vbcore/http/gql.py
 vbcore/http/headers.py
 vbcore/http/httpcode.py
 vbcore/http/httpdumper.py
 vbcore/http/methods.py
 vbcore/http/proxy.py
 vbcore/http/rpc.py
 vbcore/http/useragent.py
@@ -81,19 +101,19 @@
 vbcore/rule_engine/__init__.py
 vbcore/rule_engine/base.py
 vbcore/rule_engine/engine.py
 vbcore/standalone/__init__.py
 vbcore/standalone/scheduler.py
 vbcore/standalone/wsgi_gunicorn.py
 vbcore/tester/__init__.py
+vbcore/tester/asserter.py
 vbcore/tester/cli.py
 vbcore/tester/fetchmail.py
 vbcore/tester/helpers.py
 vbcore/tester/http.py
-vbcore/tester/mixins.py
 vbcore/tester/plugins/__init__.py
 vbcore/tester/plugins/fixtures.py
 vbcore/tester/plugins/startup.py
 vbcore/tools/__init__.py
 vbcore/tools/cli.py
 vbcore/tools/crypto.py
 vbcore/tools/database.py
```

