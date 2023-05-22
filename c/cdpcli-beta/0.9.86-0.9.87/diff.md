# Comparing `tmp/cdpcli-beta-0.9.86.tar.gz` & `tmp/cdpcli-beta-0.9.87.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdpcli-beta-0.9.86.tar", last modified: Fri May  5 02:26:28 2023, max compression
+gzip compressed data, was "cdpcli-beta-0.9.87.tar", last modified: Fri May 19 07:55:44 2023, max compression
```

## Comparing `cdpcli-beta-0.9.86.tar` & `cdpcli-beta-0.9.87.tar`

### file list

```diff
@@ -1,185 +1,185 @@
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-05-05 02:26:28.290208 cdpcli-beta-0.9.86/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    11358 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/LICENSE.txt
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     2309 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/LICENSE_SUPPLEMENTAL_DISCLAIMER.txt
--rw-rw-r--   0 jenkins    (108) jenkins    (109)      301 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/MANIFEST.in
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     7818 2023-05-05 02:26:28.290208 cdpcli-beta-0.9.86/PKG-INFO
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     5510 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/README.md
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-05-05 02:26:28.294208 cdpcli-beta-0.9.86/cdpcli/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     3972 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/cdpcli/__init__.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)      497 2023-05-05 02:26:28.294208 cdpcli-beta-0.9.86/cdpcli/_version.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     8594 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/cdpcli/argparser.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    16126 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/cdpcli/argprocess.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    13419 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/cdpcli/arguments.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    11535 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/cdpcli/auth.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    16324 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/cdpcli/cdprequest.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     1207 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/cdpcli/clicommand.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    31143 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/cdpcli/clidriver.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    22668 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/cdpcli/client.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     6574 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/cdpcli/compat.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     6562 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/cdpcli/completer.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     4116 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/cdpcli/config.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     8338 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/cdpcli/configloader.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    15597 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/cdpcli/credentials.py
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-05-05 02:26:28.278208 cdpcli-beta-0.9.86/cdpcli/data/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     1002 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/cdpcli/data/_retry.json
--rw-rw-r--   0 jenkins    (108) jenkins    (109)      246 2023-05-05 02:26:27.000000 cdpcli-beta-0.9.86/cdpcli/data/aliases.yaml
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-05-05 02:26:28.278208 cdpcli-beta-0.9.86/cdpcli/data/audit/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    32709 2023-05-05 02:26:27.000000 cdpcli-beta-0.9.86/cdpcli/data/audit/audit.yaml
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     3965 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/cdpcli/data/cli.json
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-05-05 02:26:28.278208 cdpcli-beta-0.9.86/cdpcli/data/cloudprivatelinks/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     8803 2023-05-05 02:26:24.000000 cdpcli-beta-0.9.86/cdpcli/data/cloudprivatelinks/cloudprivatelinks.yaml
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-05-05 02:26:28.278208 cdpcli-beta-0.9.86/cdpcli/data/compute/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    95423 2023-05-05 02:26:23.000000 cdpcli-beta-0.9.86/cdpcli/data/compute/compute.yaml
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-05-05 02:26:28.278208 cdpcli-beta-0.9.86/cdpcli/data/datacatalog/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     4002 2023-05-05 02:26:26.000000 cdpcli-beta-0.9.86/cdpcli/data/datacatalog/datacatalog.yaml
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-05-05 02:26:28.278208 cdpcli-beta-0.9.86/cdpcli/data/datahub/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)   142870 2023-05-05 02:26:25.000000 cdpcli-beta-0.9.86/cdpcli/data/datahub/datahub.yaml
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-05-05 02:26:28.278208 cdpcli-beta-0.9.86/cdpcli/data/datalake/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)   102900 2023-05-05 02:26:24.000000 cdpcli-beta-0.9.86/cdpcli/data/datalake/datalake.yaml
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-05-05 02:26:28.278208 cdpcli-beta-0.9.86/cdpcli/data/de/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    31579 2023-05-05 02:26:26.000000 cdpcli-beta-0.9.86/cdpcli/data/de/de.yaml
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-05-05 02:26:28.278208 cdpcli-beta-0.9.86/cdpcli/data/df/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    91702 2023-05-05 02:26:25.000000 cdpcli-beta-0.9.86/cdpcli/data/df/df.yaml
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-05-05 02:26:28.278208 cdpcli-beta-0.9.86/cdpcli/data/dfworkload/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    81768 2023-05-05 02:26:26.000000 cdpcli-beta-0.9.86/cdpcli/data/dfworkload/dfworkload.yaml
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-05-05 02:26:28.278208 cdpcli-beta-0.9.86/cdpcli/data/drscp/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    21583 2023-05-05 02:26:24.000000 cdpcli-beta-0.9.86/cdpcli/data/drscp/drscp.yaml
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-05-05 02:26:28.278208 cdpcli-beta-0.9.86/cdpcli/data/dw/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)   193567 2023-05-05 02:26:24.000000 cdpcli-beta-0.9.86/cdpcli/data/dw/dw.yaml
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-05-05 02:26:28.278208 cdpcli-beta-0.9.86/cdpcli/data/environments/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)   175988 2023-05-05 02:26:23.000000 cdpcli-beta-0.9.86/cdpcli/data/environments/environments.yaml
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-05-05 02:26:28.278208 cdpcli-beta-0.9.86/cdpcli/data/iam/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)   149065 2023-05-05 02:26:25.000000 cdpcli-beta-0.9.86/cdpcli/data/iam/iam.yaml
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-05-05 02:26:28.282208 cdpcli-beta-0.9.86/cdpcli/data/imagecatalog/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    25663 2023-05-05 02:26:24.000000 cdpcli-beta-0.9.86/cdpcli/data/imagecatalog/imagecatalog.yaml
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-05-05 02:26:28.282208 cdpcli-beta-0.9.86/cdpcli/data/ml/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    56911 2023-05-05 02:26:26.000000 cdpcli-beta-0.9.86/cdpcli/data/ml/ml.yaml
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-05-05 02:26:28.282208 cdpcli-beta-0.9.86/cdpcli/data/opdb/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    72346 2023-05-05 02:26:26.000000 cdpcli-beta-0.9.86/cdpcli/data/opdb/opdb.yaml
--rw-rw-r--   0 jenkins    (108) jenkins    (109)        4 2023-05-05 02:26:27.000000 cdpcli-beta-0.9.86/cdpcli/data/release.txt
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-05-05 02:26:28.282208 cdpcli-beta-0.9.86/cdpcli/data/replicationmanager/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    30963 2023-05-05 02:26:27.000000 cdpcli-beta-0.9.86/cdpcli/data/replicationmanager/replicationmanager.yaml
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-05-05 02:26:28.282208 cdpcli-beta-0.9.86/cdpcli/doc/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)        0 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/cdpcli/doc/__init__.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     1857 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/cdpcli/doc/docstringparser.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     7269 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/cdpcli/doc/restdoc.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    10873 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/cdpcli/doc/style.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    29420 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/cdpcli/docs.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    17043 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/cdpcli/endpoint.py
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-05-05 02:26:28.270208 cdpcli-beta-0.9.86/cdpcli/examples/
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-05-05 02:26:28.282208 cdpcli-beta-0.9.86/cdpcli/examples/configure/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     1942 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/cdpcli/examples/configure/_description.rst
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-05-05 02:26:28.282208 cdpcli-beta-0.9.86/cdpcli/examples/configure/get/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     1940 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/cdpcli/examples/configure/get/_description.rst
--rw-rw-r--   0 jenkins    (108) jenkins    (109)      764 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/cdpcli/examples/configure/get/_examples.rst
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-05-05 02:26:28.282208 cdpcli-beta-0.9.86/cdpcli/examples/configure/set/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)      862 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/cdpcli/examples/configure/set/_description.rst
--rw-rw-r--   0 jenkins    (108) jenkins    (109)      560 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/cdpcli/examples/configure/set/_examples.rst
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     9213 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/cdpcli/exceptions.py
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-05-05 02:26:28.282208 cdpcli-beta-0.9.86/cdpcli/extensions/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)      971 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/cdpcli/extensions/__init__.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     2650 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/cdpcli/extensions/arguments.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     3908 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/cdpcli/extensions/cliinputjson.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    17226 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/cdpcli/extensions/commands.py
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-05-05 02:26:28.286208 cdpcli-beta-0.9.86/cdpcli/extensions/configure/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     1330 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/cdpcli/extensions/configure/__init__.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     2047 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/cdpcli/extensions/configure/classify.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     6210 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/cdpcli/extensions/configure/configure.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     3749 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/cdpcli/extensions/configure/get.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     6414 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/cdpcli/extensions/configure/list.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     5108 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/cdpcli/extensions/configure/set.py
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-05-05 02:26:28.286208 cdpcli-beta-0.9.86/cdpcli/extensions/df/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    12046 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/cdpcli/extensions/df/__init__.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    29050 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/cdpcli/extensions/df/createdeployment.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     1575 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/cdpcli/extensions/df/register.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     3353 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/cdpcli/extensions/generatecliskeleton.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    10396 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/cdpcli/extensions/interactivelogin.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     2154 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/cdpcli/extensions/logout.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     9335 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/cdpcli/extensions/paginate.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     2642 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/cdpcli/extensions/redirect.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     6277 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/cdpcli/extensions/refdoc.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     3771 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/cdpcli/extensions/workload.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    11071 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/cdpcli/extensions/writer.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     9343 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/cdpcli/formatter.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     8083 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/cdpcli/help.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     9314 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/cdpcli/loader.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)      771 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/cdpcli/main.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    18902 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/cdpcli/model.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     7307 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/cdpcli/paginate.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     5898 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/cdpcli/paramfile.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     3218 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/cdpcli/paramformfactor.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     4085 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/cdpcli/parser.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    11836 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/cdpcli/retryhandler.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     5732 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/cdpcli/schema.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     4322 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/cdpcli/serialize.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    14202 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/cdpcli/shorthand.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     2258 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/cdpcli/signers.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    14828 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/cdpcli/table.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     4389 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/cdpcli/text.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    20981 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/cdpcli/textwriter.py
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-05-05 02:26:28.286208 cdpcli-beta-0.9.86/cdpcli/thirdparty/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)        0 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/cdpcli/thirdparty/__init__.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    27344 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/cdpcli/thirdparty/six.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     1652 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/cdpcli/translate.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    10165 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/cdpcli/utils.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    10637 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/cdpcli/validate.py
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-05-05 02:26:28.286208 cdpcli-beta-0.9.86/cdpcli_beta.egg-info/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     7818 2023-05-05 02:26:27.000000 cdpcli-beta-0.9.86/cdpcli_beta.egg-info/PKG-INFO
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     4297 2023-05-05 02:26:27.000000 cdpcli-beta-0.9.86/cdpcli_beta.egg-info/SOURCES.txt
--rw-rw-r--   0 jenkins    (108) jenkins    (109)        1 2023-05-05 02:26:27.000000 cdpcli-beta-0.9.86/cdpcli_beta.egg-info/dependency_links.txt
--rw-rw-r--   0 jenkins    (108) jenkins    (109)       85 2023-05-05 02:26:27.000000 cdpcli-beta-0.9.86/cdpcli_beta.egg-info/entry_points.txt
--rw-rw-r--   0 jenkins    (108) jenkins    (109)      190 2023-05-05 02:26:27.000000 cdpcli-beta-0.9.86/cdpcli_beta.egg-info/requires.txt
--rw-rw-r--   0 jenkins    (108) jenkins    (109)       13 2023-05-05 02:26:27.000000 cdpcli-beta-0.9.86/cdpcli_beta.egg-info/top_level.txt
--rw-rw-r--   0 jenkins    (108) jenkins    (109)      271 2023-05-05 02:26:28.290208 cdpcli-beta-0.9.86/setup.cfg
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     1429 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/setup.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     2655 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/setup_common.py
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-05-05 02:26:28.270208 cdpcli-beta-0.9.86/tests/
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-05-05 02:26:28.290208 cdpcli-beta-0.9.86/tests/unit/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     4604 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/tests/unit/__init__.py
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-05-05 02:26:28.290208 cdpcli-beta-0.9.86/tests/unit/cdp/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     1815 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/tests/unit/cdp/__init__.py
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-05-05 02:26:28.290208 cdpcli-beta-0.9.86/tests/unit/extensions/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)      732 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/tests/unit/extensions/__init__.py
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-05-05 02:26:28.290208 cdpcli-beta-0.9.86/tests/unit/extensions/configure/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)        0 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/tests/unit/extensions/configure/__init__.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     2290 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/tests/unit/extensions/configure/test_classify.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    12860 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/tests/unit/extensions/configure/test_configure.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     5637 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/tests/unit/extensions/configure/test_get.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     6675 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/tests/unit/extensions/configure/test_list.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     6656 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/tests/unit/extensions/configure/test_set.py
-drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-05-05 02:26:28.290208 cdpcli-beta-0.9.86/tests/unit/extensions/df/
--rw-rw-r--   0 jenkins    (108) jenkins    (109)        0 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/tests/unit/extensions/df/__init__.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    38131 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/tests/unit/extensions/df/test_createdeployment.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     2253 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/tests/unit/extensions/df/test_upload_file.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     5854 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/tests/unit/extensions/test_cliinputjson.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    18795 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/tests/unit/extensions/test_df.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     3807 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/tests/unit/extensions/test_generatecliskeleton.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    17115 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/tests/unit/extensions/test_interactivelogin.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     2556 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/tests/unit/extensions/test_logout.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     8305 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/tests/unit/extensions/test_operation_extension.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    10918 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/tests/unit/extensions/test_paginate.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     4828 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/tests/unit/extensions/test_redirect.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     9041 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/tests/unit/extensions/test_workload.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    11649 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/tests/unit/extensions/test_writer.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     2709 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/tests/unit/test_argparser.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     4768 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/tests/unit/test_argprocess.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    11931 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/tests/unit/test_auth.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     4421 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/tests/unit/test_cli_data.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    12187 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/tests/unit/test_client.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    14018 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/tests/unit/test_completer.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    23039 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/tests/unit/test_credentials.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     7271 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/tests/unit/test_docs.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    31273 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/tests/unit/test_endpoint.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    10750 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/tests/unit/test_help.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    12035 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/tests/unit/test_loaders.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    14102 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/tests/unit/test_model.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    15246 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/tests/unit/test_paginate.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     8243 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/tests/unit/test_paramfile.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    14417 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/tests/unit/test_protocol.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    13714 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/tests/unit/test_retryhandler.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    11240 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/tests/unit/test_shorthand.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)     3227 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/tests/unit/test_signers.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    22467 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/tests/unit/test_table_formatter.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    12971 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/tests/unit/test_utils.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    12772 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/tests/unit/test_validate.py
--rw-rw-r--   0 jenkins    (108) jenkins    (109)    68612 2023-05-05 02:15:32.000000 cdpcli-beta-0.9.86/versioneer.py
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-05-19 07:55:44.270873 cdpcli-beta-0.9.87/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    11358 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/LICENSE.txt
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     2309 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/LICENSE_SUPPLEMENTAL_DISCLAIMER.txt
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)      301 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/MANIFEST.in
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     7818 2023-05-19 07:55:44.270873 cdpcli-beta-0.9.87/PKG-INFO
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     5510 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/README.md
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-05-19 07:55:44.270873 cdpcli-beta-0.9.87/cdpcli/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     3972 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/cdpcli/__init__.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)      497 2023-05-19 07:55:44.270873 cdpcli-beta-0.9.87/cdpcli/_version.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     8594 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/cdpcli/argparser.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    16126 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/cdpcli/argprocess.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    13419 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/cdpcli/arguments.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    11535 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/cdpcli/auth.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    16324 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/cdpcli/cdprequest.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     1207 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/cdpcli/clicommand.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    31143 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/cdpcli/clidriver.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    22668 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/cdpcli/client.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     6574 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/cdpcli/compat.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     6562 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/cdpcli/completer.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     4116 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/cdpcli/config.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     8338 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/cdpcli/configloader.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    15597 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/cdpcli/credentials.py
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-05-19 07:55:44.258873 cdpcli-beta-0.9.87/cdpcli/data/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     1002 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/cdpcli/data/_retry.json
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)      246 2023-05-19 07:55:43.000000 cdpcli-beta-0.9.87/cdpcli/data/aliases.yaml
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-05-19 07:55:44.258873 cdpcli-beta-0.9.87/cdpcli/data/audit/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    32709 2023-05-19 07:55:43.000000 cdpcli-beta-0.9.87/cdpcli/data/audit/audit.yaml
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     3965 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/cdpcli/data/cli.json
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-05-19 07:55:44.258873 cdpcli-beta-0.9.87/cdpcli/data/cloudprivatelinks/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     8803 2023-05-19 07:55:40.000000 cdpcli-beta-0.9.87/cdpcli/data/cloudprivatelinks/cloudprivatelinks.yaml
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-05-19 07:55:44.258873 cdpcli-beta-0.9.87/cdpcli/data/compute/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    95423 2023-05-19 07:55:40.000000 cdpcli-beta-0.9.87/cdpcli/data/compute/compute.yaml
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-05-19 07:55:44.258873 cdpcli-beta-0.9.87/cdpcli/data/datacatalog/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     4002 2023-05-19 07:55:43.000000 cdpcli-beta-0.9.87/cdpcli/data/datacatalog/datacatalog.yaml
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-05-19 07:55:44.258873 cdpcli-beta-0.9.87/cdpcli/data/datahub/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)   143027 2023-05-19 07:55:42.000000 cdpcli-beta-0.9.87/cdpcli/data/datahub/datahub.yaml
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-05-19 07:55:44.258873 cdpcli-beta-0.9.87/cdpcli/data/datalake/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)   104133 2023-05-19 07:55:41.000000 cdpcli-beta-0.9.87/cdpcli/data/datalake/datalake.yaml
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-05-19 07:55:44.258873 cdpcli-beta-0.9.87/cdpcli/data/de/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    31670 2023-05-19 07:55:43.000000 cdpcli-beta-0.9.87/cdpcli/data/de/de.yaml
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-05-19 07:55:44.258873 cdpcli-beta-0.9.87/cdpcli/data/df/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    91702 2023-05-19 07:55:41.000000 cdpcli-beta-0.9.87/cdpcli/data/df/df.yaml
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-05-19 07:55:44.258873 cdpcli-beta-0.9.87/cdpcli/data/dfworkload/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    81768 2023-05-19 07:55:42.000000 cdpcli-beta-0.9.87/cdpcli/data/dfworkload/dfworkload.yaml
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-05-19 07:55:44.258873 cdpcli-beta-0.9.87/cdpcli/data/drscp/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    21583 2023-05-19 07:55:41.000000 cdpcli-beta-0.9.87/cdpcli/data/drscp/drscp.yaml
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-05-19 07:55:44.258873 cdpcli-beta-0.9.87/cdpcli/data/dw/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)   193583 2023-05-19 07:55:40.000000 cdpcli-beta-0.9.87/cdpcli/data/dw/dw.yaml
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-05-19 07:55:44.258873 cdpcli-beta-0.9.87/cdpcli/data/environments/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)   175998 2023-05-19 07:55:39.000000 cdpcli-beta-0.9.87/cdpcli/data/environments/environments.yaml
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-05-19 07:55:44.258873 cdpcli-beta-0.9.87/cdpcli/data/iam/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)   149065 2023-05-19 07:55:41.000000 cdpcli-beta-0.9.87/cdpcli/data/iam/iam.yaml
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-05-19 07:55:44.258873 cdpcli-beta-0.9.87/cdpcli/data/imagecatalog/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    25663 2023-05-19 07:55:40.000000 cdpcli-beta-0.9.87/cdpcli/data/imagecatalog/imagecatalog.yaml
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-05-19 07:55:44.258873 cdpcli-beta-0.9.87/cdpcli/data/ml/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    56911 2023-05-19 07:55:43.000000 cdpcli-beta-0.9.87/cdpcli/data/ml/ml.yaml
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-05-19 07:55:44.258873 cdpcli-beta-0.9.87/cdpcli/data/opdb/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    72034 2023-05-19 07:55:42.000000 cdpcli-beta-0.9.87/cdpcli/data/opdb/opdb.yaml
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)        4 2023-05-19 07:55:43.000000 cdpcli-beta-0.9.87/cdpcli/data/release.txt
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-05-19 07:55:44.258873 cdpcli-beta-0.9.87/cdpcli/data/replicationmanager/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    30963 2023-05-19 07:55:43.000000 cdpcli-beta-0.9.87/cdpcli/data/replicationmanager/replicationmanager.yaml
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-05-19 07:55:44.258873 cdpcli-beta-0.9.87/cdpcli/doc/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)        0 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/cdpcli/doc/__init__.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     1857 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/cdpcli/doc/docstringparser.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     7269 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/cdpcli/doc/restdoc.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    10873 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/cdpcli/doc/style.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    29420 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/cdpcli/docs.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    17043 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/cdpcli/endpoint.py
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-05-19 07:55:44.250873 cdpcli-beta-0.9.87/cdpcli/examples/
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-05-19 07:55:44.262873 cdpcli-beta-0.9.87/cdpcli/examples/configure/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     1942 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/cdpcli/examples/configure/_description.rst
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-05-19 07:55:44.262873 cdpcli-beta-0.9.87/cdpcli/examples/configure/get/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     1940 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/cdpcli/examples/configure/get/_description.rst
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)      764 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/cdpcli/examples/configure/get/_examples.rst
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-05-19 07:55:44.262873 cdpcli-beta-0.9.87/cdpcli/examples/configure/set/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)      862 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/cdpcli/examples/configure/set/_description.rst
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)      560 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/cdpcli/examples/configure/set/_examples.rst
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     9213 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/cdpcli/exceptions.py
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-05-19 07:55:44.262873 cdpcli-beta-0.9.87/cdpcli/extensions/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)      971 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/cdpcli/extensions/__init__.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     2650 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/cdpcli/extensions/arguments.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     3908 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/cdpcli/extensions/cliinputjson.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    17226 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/cdpcli/extensions/commands.py
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-05-19 07:55:44.262873 cdpcli-beta-0.9.87/cdpcli/extensions/configure/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     1330 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/cdpcli/extensions/configure/__init__.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     2047 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/cdpcli/extensions/configure/classify.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     6210 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/cdpcli/extensions/configure/configure.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     3749 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/cdpcli/extensions/configure/get.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     6414 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/cdpcli/extensions/configure/list.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     5108 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/cdpcli/extensions/configure/set.py
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-05-19 07:55:44.262873 cdpcli-beta-0.9.87/cdpcli/extensions/df/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    12046 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/cdpcli/extensions/df/__init__.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    29050 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/cdpcli/extensions/df/createdeployment.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     1575 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/cdpcli/extensions/df/register.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     3353 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/cdpcli/extensions/generatecliskeleton.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    10396 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/cdpcli/extensions/interactivelogin.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     2154 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/cdpcli/extensions/logout.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     9335 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/cdpcli/extensions/paginate.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     2642 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/cdpcli/extensions/redirect.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     6277 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/cdpcli/extensions/refdoc.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     3771 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/cdpcli/extensions/workload.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    11071 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/cdpcli/extensions/writer.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     9343 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/cdpcli/formatter.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     8083 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/cdpcli/help.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     9314 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/cdpcli/loader.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)      771 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/cdpcli/main.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    18902 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/cdpcli/model.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     7307 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/cdpcli/paginate.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     5898 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/cdpcli/paramfile.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     3218 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/cdpcli/paramformfactor.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     4085 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/cdpcli/parser.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    11836 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/cdpcli/retryhandler.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     5732 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/cdpcli/schema.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     4322 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/cdpcli/serialize.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    14202 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/cdpcli/shorthand.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     2258 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/cdpcli/signers.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    14828 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/cdpcli/table.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     4389 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/cdpcli/text.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    20981 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/cdpcli/textwriter.py
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-05-19 07:55:44.262873 cdpcli-beta-0.9.87/cdpcli/thirdparty/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)        0 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/cdpcli/thirdparty/__init__.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    27344 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/cdpcli/thirdparty/six.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     1652 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/cdpcli/translate.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    10165 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/cdpcli/utils.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    10637 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/cdpcli/validate.py
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-05-19 07:55:44.266873 cdpcli-beta-0.9.87/cdpcli_beta.egg-info/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     7818 2023-05-19 07:55:44.000000 cdpcli-beta-0.9.87/cdpcli_beta.egg-info/PKG-INFO
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     4297 2023-05-19 07:55:44.000000 cdpcli-beta-0.9.87/cdpcli_beta.egg-info/SOURCES.txt
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)        1 2023-05-19 07:55:44.000000 cdpcli-beta-0.9.87/cdpcli_beta.egg-info/dependency_links.txt
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)       85 2023-05-19 07:55:44.000000 cdpcli-beta-0.9.87/cdpcli_beta.egg-info/entry_points.txt
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)      190 2023-05-19 07:55:44.000000 cdpcli-beta-0.9.87/cdpcli_beta.egg-info/requires.txt
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)       13 2023-05-19 07:55:44.000000 cdpcli-beta-0.9.87/cdpcli_beta.egg-info/top_level.txt
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)      271 2023-05-19 07:55:44.270873 cdpcli-beta-0.9.87/setup.cfg
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     1429 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/setup.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     2655 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/setup_common.py
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-05-19 07:55:44.250873 cdpcli-beta-0.9.87/tests/
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-05-19 07:55:44.266873 cdpcli-beta-0.9.87/tests/unit/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     4604 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/tests/unit/__init__.py
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-05-19 07:55:44.266873 cdpcli-beta-0.9.87/tests/unit/cdp/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     1815 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/tests/unit/cdp/__init__.py
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-05-19 07:55:44.270873 cdpcli-beta-0.9.87/tests/unit/extensions/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)      732 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/tests/unit/extensions/__init__.py
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-05-19 07:55:44.270873 cdpcli-beta-0.9.87/tests/unit/extensions/configure/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)        0 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/tests/unit/extensions/configure/__init__.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     2290 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/tests/unit/extensions/configure/test_classify.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    12860 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/tests/unit/extensions/configure/test_configure.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     5637 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/tests/unit/extensions/configure/test_get.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     6675 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/tests/unit/extensions/configure/test_list.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     6656 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/tests/unit/extensions/configure/test_set.py
+drwxrwxr-x   0 jenkins    (108) jenkins    (109)        0 2023-05-19 07:55:44.270873 cdpcli-beta-0.9.87/tests/unit/extensions/df/
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)        0 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/tests/unit/extensions/df/__init__.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    38131 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/tests/unit/extensions/df/test_createdeployment.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     2253 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/tests/unit/extensions/df/test_upload_file.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     5854 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/tests/unit/extensions/test_cliinputjson.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    18795 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/tests/unit/extensions/test_df.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     3807 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/tests/unit/extensions/test_generatecliskeleton.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    17115 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/tests/unit/extensions/test_interactivelogin.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     2556 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/tests/unit/extensions/test_logout.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     8305 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/tests/unit/extensions/test_operation_extension.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    10918 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/tests/unit/extensions/test_paginate.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     4828 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/tests/unit/extensions/test_redirect.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     9041 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/tests/unit/extensions/test_workload.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    11649 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/tests/unit/extensions/test_writer.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     2709 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/tests/unit/test_argparser.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     4768 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/tests/unit/test_argprocess.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    11931 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/tests/unit/test_auth.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     4421 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/tests/unit/test_cli_data.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    12187 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/tests/unit/test_client.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    14018 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/tests/unit/test_completer.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    23039 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/tests/unit/test_credentials.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     7271 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/tests/unit/test_docs.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    31273 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/tests/unit/test_endpoint.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    10750 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/tests/unit/test_help.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    12035 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/tests/unit/test_loaders.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    14102 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/tests/unit/test_model.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    15246 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/tests/unit/test_paginate.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     8243 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/tests/unit/test_paramfile.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    14417 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/tests/unit/test_protocol.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    13714 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/tests/unit/test_retryhandler.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    11240 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/tests/unit/test_shorthand.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)     3227 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/tests/unit/test_signers.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    22467 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/tests/unit/test_table_formatter.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    12971 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/tests/unit/test_utils.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    12772 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/tests/unit/test_validate.py
+-rw-rw-r--   0 jenkins    (108) jenkins    (109)    68612 2023-05-19 07:43:11.000000 cdpcli-beta-0.9.87/versioneer.py
```

### Comparing `cdpcli-beta-0.9.86/LICENSE.txt` & `cdpcli-beta-0.9.87/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.86/LICENSE_SUPPLEMENTAL_DISCLAIMER.txt` & `cdpcli-beta-0.9.87/LICENSE_SUPPLEMENTAL_DISCLAIMER.txt`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.86/PKG-INFO` & `cdpcli-beta-0.9.87/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdpcli-beta
-Version: 0.9.86
+Version: 0.9.87
 Summary: Cloudera CDP Command Line Interface (BETA)
 Home-page: https://console.cdp.cloudera.com/
 Author: Cloudera, Inc.
 License: Apache License 2.0
 Description: # Cloudera CDP Command Line Interface
         
         This package provides a unified command line interface to the Cloudera Data
```

### Comparing `cdpcli-beta-0.9.86/README.md` & `cdpcli-beta-0.9.87/README.md`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.86/cdpcli/__init__.py` & `cdpcli-beta-0.9.87/cdpcli/__init__.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.86/cdpcli/argparser.py` & `cdpcli-beta-0.9.87/cdpcli/argparser.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.86/cdpcli/argprocess.py` & `cdpcli-beta-0.9.87/cdpcli/argprocess.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.86/cdpcli/arguments.py` & `cdpcli-beta-0.9.87/cdpcli/arguments.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.86/cdpcli/auth.py` & `cdpcli-beta-0.9.87/cdpcli/auth.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.86/cdpcli/cdprequest.py` & `cdpcli-beta-0.9.87/cdpcli/cdprequest.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.86/cdpcli/clicommand.py` & `cdpcli-beta-0.9.87/cdpcli/clicommand.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.86/cdpcli/clidriver.py` & `cdpcli-beta-0.9.87/cdpcli/clidriver.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.86/cdpcli/client.py` & `cdpcli-beta-0.9.87/cdpcli/client.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.86/cdpcli/compat.py` & `cdpcli-beta-0.9.87/cdpcli/compat.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.86/cdpcli/completer.py` & `cdpcli-beta-0.9.87/cdpcli/completer.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.86/cdpcli/config.py` & `cdpcli-beta-0.9.87/cdpcli/config.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.86/cdpcli/configloader.py` & `cdpcli-beta-0.9.87/cdpcli/configloader.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.86/cdpcli/credentials.py` & `cdpcli-beta-0.9.87/cdpcli/credentials.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.86/cdpcli/data/_retry.json` & `cdpcli-beta-0.9.87/cdpcli/data/_retry.json`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.86/cdpcli/data/audit/audit.yaml` & `cdpcli-beta-0.9.87/cdpcli/data/audit/audit.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 x-generated: Automatically generated by CDP protoc plugin. Do not edit manually.
 swagger: '2.0'
 x-endpoint-name: audit
 x-products: CDP
 x-form-factors: public
 x-cdp-releases: PUBLIC
 info:
-  version: 0.9.86
+  version: 0.9.87
   title: Cloudera Audit Service
   license:
     name: Apache 2.0
   description: Cloudera CDP Auditing is a web service for interacting with the audit subsystem.
   termsOfService: https://www.cloudera.com/legal/commercial-terms-and-conditions.html
 schemes:
   - https
```

### Comparing `cdpcli-beta-0.9.86/cdpcli/data/cli.json` & `cdpcli-beta-0.9.87/cdpcli/data/cli.json`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.86/cdpcli/data/cloudprivatelinks/cloudprivatelinks.yaml` & `cdpcli-beta-0.9.87/cdpcli/data/cloudprivatelinks/cloudprivatelinks.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 x-generated: Automatically generated by CDP protoc plugin. Do not edit manually.
 swagger: '2.0'
 x-endpoint-name: cloudprivatelinks
 x-products: CDP
 x-form-factors: public
 x-cdp-releases: BETA
 info:
-  version: 0.9.86
+  version: 0.9.87
   title: Cloudera CloudPrivateLinks API Service
   license:
     name: Apache 2.0
   description: Provisions PrivateLink Endpoints on the cloud environments.
   termsOfService: https://www.cloudera.com/legal/commercial-terms-and-conditions.html
 schemes:
   - https
```

### Comparing `cdpcli-beta-0.9.86/cdpcli/data/compute/compute.yaml` & `cdpcli-beta-0.9.87/cdpcli/data/compute/compute.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 x-generated: Automatically generated by CDP protoc plugin. Do not edit manually.
 swagger: '2.0'
 x-endpoint-name: compute
 x-products: CDP
 x-form-factors: public,private
 x-cdp-releases: PUBLIC
 info:
-  version: 0.9.86
+  version: 0.9.87
   title: Cloudera Compute Service
   license:
     name: Apache 2.0
   description: Defining service of compute public API service
   termsOfService: https://www.cloudera.com/legal/commercial-terms-and-conditions.html
 schemes:
   - https
```

### Comparing `cdpcli-beta-0.9.86/cdpcli/data/datacatalog/datacatalog.yaml` & `cdpcli-beta-0.9.87/cdpcli/data/datacatalog/datacatalog.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 swagger: '2.0'
 x-endpoint-name: datacatalog
 x-products: CDP
 x-form-factors: public
 x-cdp-releases: PUBLIC
 x-audit: true
 info:
-  version: 0.9.86
+  version: 0.9.87
   title: Cloudera DataCatalog Service
   license:
     name: Apache 2.0
   description: Cloudera DataCatalog Service is a web service, using this service a user can execute operations like launching profilers in DataCatalog.
 schemes:
   - https
 consumes:
```

### Comparing `cdpcli-beta-0.9.86/cdpcli/data/datahub/datahub.yaml` & `cdpcli-beta-0.9.87/cdpcli/data/datahub/datahub.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 x-endpoint-name: datahub
 x-interface-model: cdp
 x-products: CDP
 x-form-factors: public
 x-cdp-releases: PUBLIC
 x-audit: true
 info:
-  version: 0.9.86
+  version: 0.9.87
   title: Cloudera Data hub Service
   license:
     name: Apache 2.0
   description: Cloudera data hub is a service for launching and managing workload clusters powered by Cloudera Runtime.
   termsOfService: https://www.cloudera.com/legal/commercial-terms-and-conditions.html
 schemes:
   - https
@@ -1374,15 +1374,15 @@
       name:
         type: string
         description: The name of the instance group where the given instance is located.
       instances:
         type: array
         items:
           $ref: '#/definitions/Instance'
-        description: Some information about the given instance.
+        description: List of instances in this instance group.
   StartClusterVerticalScalingRequest:
     type: object
     description: The request object for Data Hub vertical scaling.
     required:
       - datahub
       - group
       - instanceTemplate
@@ -1412,30 +1412,34 @@
         description: The type of the instance.
   Instance:
     type: object
     description: Object which holds some details of an instance for the given cluster.
     required:
       - id
       - state
+      - instanceType
     properties:
       id:
         type: string
         description: The ID of the given instance.
       state:
         type: string
         description: The health state of the instance. UNHEALTHY represents instances with unhealthy services, lost instances, or failed operations.
+      instanceType:
+        type: string
+        description: The type of the given instance (either GATEWAY, GATEWAY_PRIMARY, or CORE).
       privateIp:
         type: string
-        description: The private ip of the given instance.
+        description: The private IP of the given instance.
       publicIp:
         type: string
-        description: The public ip of the given instance.
+        description: The public IP of the given instance.
       fqdn:
         type: string
-        description: The FQDN for the instance
+        description: The FQDN of the instance.
       status:
         type: string
         description: The status of the instance. This includes information like whether the instance is being provisioned, stopped, decommissioning failures etc.
   Endpoints:
     type: object
     description: Object which holds the exposed endpoints for the given cluster.
     required:
```

### Comparing `cdpcli-beta-0.9.86/cdpcli/data/datalake/datalake.yaml` & `cdpcli-beta-0.9.87/cdpcli/data/datalake/datalake.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 x-endpoint-name: datalake
 x-interface-model: cdp
 x-products: CDP
 x-form-factors: public
 x-cdp-releases: PUBLIC
 x-audit: true
 info:
-  version: 0.9.86
+  version: 0.9.87
   title: Cloudera Datalake Service
   license:
     name: Apache 2.0
   description: Cloudera data lake is a service for launching and managing data lake clusters powered by Cloudera Runtime.
   termsOfService: https://www.cloudera.com/legal/commercial-terms-and-conditions.html
 schemes:
   - https
@@ -1052,39 +1052,84 @@
     description: The type of the instance group which also contains the actual instance(s)
     required:
       - name
       - instances
     properties:
       name:
         type: string
-        description: The name of the instance group where the given instance is located.
+        description: The name of the instance group.
       instances:
         type: array
         items:
           $ref: '#/definitions/Instance'
-        description: Some information about the given instance.
+        description: List of instances in this instance group.
   Instance:
     type: object
     description: Object which holds some details of an instance for the given cluster.
     required:
       - id
       - state
     properties:
       id:
         type: string
         description: The ID of the given instance.
       state:
         type: string
         description: The actual state of the instance.
+      discoveryFQDN:
+        type: string
+        description: The FQDN of the instance.
+      instanceStatus:
+        $ref: '#/definitions/DatalakeInstanceStatus'
+        description: The status of the instance.
+      statusReason:
+        type: string
+        description: The reason for the current status of this instance.
       privateIp:
         type: string
-        description: The private ip of the given instance.
+        description: The private IP of the given instance.
       publicIp:
         type: string
-        description: The public ip of the given instance.
+        description: The public IP of the given instance.
+      sshPort:
+        type: integer
+        format: int32
+        description: The SSH port for the instance.
+      instanceGroup:
+        type: string
+        description: The name of the instance group this instance belongs to.
+      instanceTypeVal:
+        $ref: '#/definitions/DatalakeInstanceType'
+        description: The instance type.
+  DatalakeInstanceStatus:
+    type: string
+    description: The status of the instance.
+    enum:
+      - REQUESTED
+      - FAILED
+      - CREATED
+      - ORCHESTRATION_FAILED
+      - SERVICES_RUNNING
+      - SERVICES_HEALTHY
+      - SERVICES_UNHEALTHY
+      - WAITING_FOR_REPAIR
+      - STOPPED
+      - DELETED_ON_PROVIDER_SIDE
+      - DELETED_BY_PROVIDER
+      - DELETE_REQUESTED
+      - DECOMMISSIONED
+      - DECOMMISION_FAILED
+      - TERMINATED
+  DatalakeInstanceType:
+    type: string
+    description: The type of the instance.
+    enum:
+      - GATEWAY
+      - GATEWAY_PRIMARY
+      - CORE
   Endpoints:
     type: object
     description: Object which holds the exposed endpoints for the given cluster.
     required:
       - endpoints
     properties:
       endpoints:
```

### Comparing `cdpcli-beta-0.9.86/cdpcli/data/de/de.yaml` & `cdpcli-beta-0.9.87/cdpcli/data/de/de.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 swagger: '2.0'
 x-endpoint-name: de
 x-products: CDP
 x-form-factors: public,private
 x-cdp-releases: PUBLIC
 x-audit: true
 info:
-  version: 0.9.86
+  version: 0.9.87
   title: Cloudera Data Engineering
   license:
     name: Apache 2.0
   description: Create and manage Cloudera Data Engineering Services.
   termsOfService: https://www.cloudera.com/legal/commercial-terms-and-conditions.html
 schemes:
   - https
@@ -897,18 +897,19 @@
         type: string
         description: Used to describe where the Driver and the Executors would run. By default the Driver would run on on-demand instances and the Executors on spot instances. Setting it to ALL will run both the Driver and the Executors on spot instances whereas setting it to NONE should run both the Driver and the Executor on on-demand instances. Currently applicable for aws services only. Use this option only on services with spot instances enabled.
         enum:
           - ALL
           - NONE
       sparkVersion:
         type: string
-        description: Spark version for the virtual cluster. Currently supported spark versions are 2.4.7 and 3.1.1. This feature is only supported in CDE-1.7.0 and beyond.
+        description: Spark version for the virtual cluster. Currently supported spark versions are SPARK2(deprecated), SPARK3 and SPARK3_3. This feature is only supported in CDE-1.7.0 and beyond. SPARK3_3 is supported in CDE-1.19 and beyond.
         enum:
           - SPARK2
           - SPARK3
+          - SPARK3_3
       aclUsers:
         description: Comma-separated Workload usernames of CDP users to be granted access to the Virtual Cluster.
         type: string
   CreateVcResponse:
     type: object
     description: Response object for CreateVc method.
     properties:
```

### Comparing `cdpcli-beta-0.9.86/cdpcli/data/df/df.yaml` & `cdpcli-beta-0.9.87/cdpcli/data/df/df.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 x-generated: Automatically generated by CDP protoc plugin. Do not edit manually.
 swagger: '2.0'
 x-endpoint-name: df
 x-products: CDP
 x-form-factors: public
 x-cdp-releases: PUBLIC
 info:
-  version: 0.9.86
+  version: 0.9.87
   title: Cloudera DataFlow Service
   license:
     name: Apache 2.0
   description: Manage DataFlow Services.
   termsOfService: https://www.cloudera.com/legal/commercial-terms-and-conditions.html
 schemes:
   - https
```

### Comparing `cdpcli-beta-0.9.86/cdpcli/data/dfworkload/dfworkload.yaml` & `cdpcli-beta-0.9.87/cdpcli/data/dfworkload/dfworkload.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 swagger: '2.0'
 x-endpoint-name: dfworkload
 x-products: CDP
 x-form-factors: public
 x-cdp-releases: PUBLIC
 info:
   description: "This REST API provides remote access to the DataFlow Service.\n Endpoints that are marked as [BETA] are subject to change in future releases of the application without backwards compatibility and without a major version change."
-  version: 0.9.86
+  version: 0.9.87
   title: Cloudera DataFlow Workload Service
   license:
     name: Apache 2.0
   termsOfService: https://www.cloudera.com/legal/commercial-terms-and-conditions.html
 schemes:
   - https
 consumes:
```

### Comparing `cdpcli-beta-0.9.86/cdpcli/data/drscp/drscp.yaml` & `cdpcli-beta-0.9.87/cdpcli/data/drscp/drscp.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 swagger: '2.0'
 x-endpoint-name: drscp
 x-products: CDP
 x-form-factors: private
 x-audit: true
 x-cdp-releases: PUBLIC
 info:
-  version: 0.9.86
+  version: 0.9.87
   title: CDP Control Plane Data Recovery Service
   license:
     name: Apache 2.0
   description: The API of Data Recovery Service for CDP Private Cloud Control Plane .
 schemes:
   - https
 consumes:
```

### Comparing `cdpcli-beta-0.9.86/cdpcli/data/dw/dw.yaml` & `cdpcli-beta-0.9.87/cdpcli/data/dw/dw.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 swagger: '2.0'
 x-endpoint-name: dw
 x-products: CDP
 x-form-factors: public,private
 x-cdp-releases: PUBLIC
 info:
-  version: 0.9.86
+  version: 0.9.87
   title: Cloudera Data Warehouse [EXPERIMENTAL]
   license:
     name: Apache 2.0
   description: Install and manage Cloudera Data Warehouse clusters.
   termsOfService: https://www.cloudera.com/legal/commercial-terms-and-conditions.html
 schemes:
   - https
@@ -3373,15 +3373,15 @@
         format: int32
         description: Maximum Concurrent Isolated Queries
       maxNodesPerQuery:
         type: integer
         format: int32
         description: Maximum Nodes Per Isolated Query
   ReplicaStatus:
-    x-form-factors: public
+    x-form-factors: public,private
     type: object
     description: Status information on the current state of replicas in the virtual warehouse.
     properties:
       totalExecutorReplicas:
         type: integer
         format: int32
         description: Total number of executor replicas scheduled for the virtual warehouse. This number contains the number of executor replicas in pending state, as well as the replicas that are already running. If this number is zero, then the executor functionality is stopped.
@@ -4232,15 +4232,15 @@
       impalaHaSettingsOptions:
         description: Current Impala High Availability settings.
         $ref: '#/definitions/ImpalaHASettingsOptionsResponse'
       queryIsolationOptions:
         description: The current settings stored for query-isolation.
         $ref: '#/definitions/QueryIsolationOptionsResponse'
       replicaStatus:
-        x-form-factors: public
+        x-form-factors: public,private
         description: Status information on the current state of replicas in the virtual warehouse.
         $ref: '#/definitions/ReplicaStatus'
   TagResponse:
     description: A key/value pair attached to some resources.
     type: object
     required:
       - key
```

### Comparing `cdpcli-beta-0.9.86/cdpcli/data/environments/environments.yaml` & `cdpcli-beta-0.9.87/cdpcli/data/environments/environments.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 x-endpoint-name: environments2
 x-display-name: environments
 x-products: CDP
 x-form-factors: public,private
 x-cdp-releases: PUBLIC
 x-audit: true
 info:
-  version: 0.9.86
+  version: 0.9.87
   title: Cloudera Environments Service
   license:
     name: Apache 2.0
   description: Cloudera Environments Service is a web service that manages cloud provider access.
   termsOfService: https://www.cloudera.com/legal/commercial-terms-and-conditions.html
 schemes:
   - https
@@ -4789,15 +4789,15 @@
         description: The number of volumes.
       volumeType:
         type: string
         description: The type of the volumes.
       size:
         type: integer
         format: int64
-        description: The size of volumes.
+        description: The size of each volume in GB.
   AwsFreeIpaInstanceTemplateParams:
     type: object
     description: AWS specific FreeIPA parameters.
     properties:
       spotPercentage:
         type: integer
         format: int32
```

### Comparing `cdpcli-beta-0.9.86/cdpcli/data/iam/iam.yaml` & `cdpcli-beta-0.9.87/cdpcli/data/iam/iam.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 x-endpoint-name: iam
 x-products: ALTUS,CDP
 x-form-factors: public,private
 x-altus-releases: PUBLIC
 x-cdp-releases: PUBLIC
 x-audit: true
 info:
-  version: 0.9.86
+  version: 0.9.87
   title: Cloudera IAM Service
   license:
     name: Apache 2.0
   description: Cloudera CDP IAM is a web service that you can use to manage users and user permissions under your CDP account.
   termsOfService: https://www.cloudera.com/legal/commercial-terms-and-conditions.html
 schemes:
   - https
```

### Comparing `cdpcli-beta-0.9.86/cdpcli/data/imagecatalog/imagecatalog.yaml` & `cdpcli-beta-0.9.87/cdpcli/data/imagecatalog/imagecatalog.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 x-generated: Automatically generated by CDP protoc plugin. Do not edit manually.
 swagger: '2.0'
 x-endpoint-name: imagecatalog
 x-products: CDP
 x-form-factors: public
 x-cdp-releases: PUBLIC
 info:
-  version: 0.9.86
+  version: 0.9.87
   title: Image catalog service
   license:
     name: Apache 2.0
   description: Service for managing custom image catalogs and their associated Cloudera Runtime and FreeIPA images.
   termsOfService: https://www.cloudera.com/legal/commercial-terms-and-conditions.html
 schemes:
   - https
```

### Comparing `cdpcli-beta-0.9.86/cdpcli/data/ml/ml.yaml` & `cdpcli-beta-0.9.87/cdpcli/data/ml/ml.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 x-generated: Automatically generated by CDP protoc plugin. Do not edit manually.
 swagger: '2.0'
 x-endpoint-name: ml
 x-products: CDP
 x-form-factors: public,private
 x-cdp-releases: PUBLIC
 info:
-  version: 0.9.86
+  version: 0.9.87
   title: Cloudera Machine Learning
   license:
     name: Apache 2.0
   description: Install and manage Cloudera Machine Learning applications.
   termsOfService: https://www.cloudera.com/legal/commercial-terms-and-conditions.html
 schemes:
   - https
```

### Comparing `cdpcli-beta-0.9.86/cdpcli/data/opdb/opdb.yaml` & `cdpcli-beta-0.9.87/cdpcli/data/opdb/opdb.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 x-generated: Automatically generated by CDP protoc plugin. Do not edit manually.
 swagger: '2.0'
 x-endpoint-name: opdb
 x-products: CDP
 x-form-factors: public
 x-cdp-releases: PUBLIC
 info:
-  version: 0.9.86
+  version: 0.9.87
   title: Operational Database service
   license:
     name: Apache 2.0
   description: Interact with the Cloudera Operational Database service
   termsOfService: https://www.cloudera.com/legal/commercial-terms-and-conditions.html
 schemes:
   - https
@@ -746,17 +746,14 @@
         description: Disable large block cache on ephemeral storage.
       disableMultiAz:
         type: boolean
         description: Disable deployment into multiple availability-zones (the database will be deployed into one subnet).
       attachedStorageForWorkers:
         description: Attached storage for the worker nodes for AWS, Azure, and GCP cloud providers.
         $ref: '#/definitions/AttachedStorageForWorkers'
-      masterNodeType:
-        description: Optional tags to select predefined master node type to handle different size of work load when hbase root deployed on hdfs
-        $ref: '#/definitions/MasterNodeType'
       disableKerberos:
         type: boolean
         description: Disable Kerberos authentication.
       numEdgeNodes:
         type: integer
         format: int32
         description: Number of edge nodes to be created for the database. A positive, non-zero number is required. The default value is 0. Requires the COD_EDGE_NODE entitlement.
@@ -794,31 +791,27 @@
       volumeSize:
         type: integer
         format: int32
         description: The target size of the volume, in GiB. Default is 2048.
       volumeType:
         description: The volume type. This parameter can be HDD or SSD. Default is HDD.
         $ref: '#/definitions/VolumeType'
-  MasterNodeType:
-    type: string
-    description: "Master node type\n `LITE` - Use small master instance type to handle less load for master services. `HEAVY` - Use large master instance type to handle more load for master services."
-    enum:
-      - LITE
-      - HEAVY
   GatewayNodeType:
     type: string
     description: "Gateway node type.\n `LITE` - Use a small gateway instance type to handle less load for gateway services. `HEAVY` - Use a large gateway instance type to handle more load for gateway services."
     enum:
       - LITE
       - HEAVY
   ScaleType:
     type: string
-    description: "Scale type.\n `MICRO` - Create a 2 node cluster (1 gateway and 1 worker) with high availability disabled."
+    description: "Scale type.\n `MICRO` - Create a 2-node cluster (1 gateway and 1 worker) with high availability disabled. `LIGHT` - Create a multi-node cluster with a light master instance type. `HEAVY` - Create a multi-node cluster with heavy master instance type."
     enum:
       - MICRO
+      - LIGHT
+      - HEAVY
   UpdateDatabaseRequest:
     type: object
     description: A request to update the database
     required:
       - environmentName
       - databaseName
     properties:
```

### Comparing `cdpcli-beta-0.9.86/cdpcli/data/replicationmanager/replicationmanager.yaml` & `cdpcli-beta-0.9.87/cdpcli/data/replicationmanager/replicationmanager.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 swagger: '2.0'
 x-endpoint-name: replicationmanager
 x-products: CDP
 x-form-factors: public
 x-cdp-releases: PUBLIC
 x-audit: true
 info:
-  version: 0.9.86
+  version: 0.9.87
   title: Cloudera Replication Manager Service
   license:
     name: Apache 2.0
   description: Create and manage replication policies using Cloudera Replication Manager.
   termsOfService: https://www.cloudera.com/legal/commercial-terms-and-conditions.html
 schemes:
   - https
```

### Comparing `cdpcli-beta-0.9.86/cdpcli/doc/docstringparser.py` & `cdpcli-beta-0.9.87/cdpcli/doc/docstringparser.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.86/cdpcli/doc/restdoc.py` & `cdpcli-beta-0.9.87/cdpcli/doc/restdoc.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.86/cdpcli/doc/style.py` & `cdpcli-beta-0.9.87/cdpcli/doc/style.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.86/cdpcli/docs.py` & `cdpcli-beta-0.9.87/cdpcli/docs.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.86/cdpcli/endpoint.py` & `cdpcli-beta-0.9.87/cdpcli/endpoint.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.86/cdpcli/examples/configure/_description.rst` & `cdpcli-beta-0.9.87/cdpcli/examples/configure/_description.rst`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.86/cdpcli/examples/configure/get/_description.rst` & `cdpcli-beta-0.9.87/cdpcli/examples/configure/get/_description.rst`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.86/cdpcli/examples/configure/get/_examples.rst` & `cdpcli-beta-0.9.87/cdpcli/examples/configure/get/_examples.rst`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.86/cdpcli/examples/configure/set/_description.rst` & `cdpcli-beta-0.9.87/cdpcli/examples/configure/set/_description.rst`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.86/cdpcli/examples/configure/set/_examples.rst` & `cdpcli-beta-0.9.87/cdpcli/examples/configure/set/_examples.rst`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.86/cdpcli/exceptions.py` & `cdpcli-beta-0.9.87/cdpcli/exceptions.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.86/cdpcli/extensions/__init__.py` & `cdpcli-beta-0.9.87/cdpcli/extensions/__init__.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.86/cdpcli/extensions/arguments.py` & `cdpcli-beta-0.9.87/cdpcli/extensions/arguments.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.86/cdpcli/extensions/cliinputjson.py` & `cdpcli-beta-0.9.87/cdpcli/extensions/cliinputjson.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.86/cdpcli/extensions/commands.py` & `cdpcli-beta-0.9.87/cdpcli/extensions/commands.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.86/cdpcli/extensions/configure/__init__.py` & `cdpcli-beta-0.9.87/cdpcli/extensions/configure/__init__.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.86/cdpcli/extensions/configure/classify.py` & `cdpcli-beta-0.9.87/cdpcli/extensions/configure/classify.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.86/cdpcli/extensions/configure/configure.py` & `cdpcli-beta-0.9.87/cdpcli/extensions/configure/configure.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.86/cdpcli/extensions/configure/get.py` & `cdpcli-beta-0.9.87/cdpcli/extensions/configure/get.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.86/cdpcli/extensions/configure/list.py` & `cdpcli-beta-0.9.87/cdpcli/extensions/configure/list.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.86/cdpcli/extensions/configure/set.py` & `cdpcli-beta-0.9.87/cdpcli/extensions/configure/set.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.86/cdpcli/extensions/df/__init__.py` & `cdpcli-beta-0.9.87/cdpcli/extensions/df/__init__.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.86/cdpcli/extensions/df/createdeployment.py` & `cdpcli-beta-0.9.87/cdpcli/extensions/df/createdeployment.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.86/cdpcli/extensions/df/register.py` & `cdpcli-beta-0.9.87/cdpcli/extensions/df/register.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.86/cdpcli/extensions/generatecliskeleton.py` & `cdpcli-beta-0.9.87/cdpcli/extensions/generatecliskeleton.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.86/cdpcli/extensions/interactivelogin.py` & `cdpcli-beta-0.9.87/cdpcli/extensions/interactivelogin.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.86/cdpcli/extensions/logout.py` & `cdpcli-beta-0.9.87/cdpcli/extensions/logout.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.86/cdpcli/extensions/paginate.py` & `cdpcli-beta-0.9.87/cdpcli/extensions/paginate.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.86/cdpcli/extensions/redirect.py` & `cdpcli-beta-0.9.87/cdpcli/extensions/redirect.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.86/cdpcli/extensions/refdoc.py` & `cdpcli-beta-0.9.87/cdpcli/extensions/refdoc.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.86/cdpcli/extensions/workload.py` & `cdpcli-beta-0.9.87/cdpcli/extensions/workload.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.86/cdpcli/extensions/writer.py` & `cdpcli-beta-0.9.87/cdpcli/extensions/writer.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.86/cdpcli/formatter.py` & `cdpcli-beta-0.9.87/cdpcli/formatter.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.86/cdpcli/help.py` & `cdpcli-beta-0.9.87/cdpcli/help.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.86/cdpcli/loader.py` & `cdpcli-beta-0.9.87/cdpcli/loader.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.86/cdpcli/main.py` & `cdpcli-beta-0.9.87/cdpcli/main.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.86/cdpcli/model.py` & `cdpcli-beta-0.9.87/cdpcli/model.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.86/cdpcli/paginate.py` & `cdpcli-beta-0.9.87/cdpcli/paginate.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.86/cdpcli/paramfile.py` & `cdpcli-beta-0.9.87/cdpcli/paramfile.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.86/cdpcli/paramformfactor.py` & `cdpcli-beta-0.9.87/cdpcli/paramformfactor.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.86/cdpcli/parser.py` & `cdpcli-beta-0.9.87/cdpcli/parser.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.86/cdpcli/retryhandler.py` & `cdpcli-beta-0.9.87/cdpcli/retryhandler.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.86/cdpcli/schema.py` & `cdpcli-beta-0.9.87/cdpcli/schema.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.86/cdpcli/serialize.py` & `cdpcli-beta-0.9.87/cdpcli/serialize.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.86/cdpcli/shorthand.py` & `cdpcli-beta-0.9.87/cdpcli/shorthand.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.86/cdpcli/signers.py` & `cdpcli-beta-0.9.87/cdpcli/signers.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.86/cdpcli/table.py` & `cdpcli-beta-0.9.87/cdpcli/table.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.86/cdpcli/text.py` & `cdpcli-beta-0.9.87/cdpcli/text.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.86/cdpcli/textwriter.py` & `cdpcli-beta-0.9.87/cdpcli/textwriter.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.86/cdpcli/thirdparty/six.py` & `cdpcli-beta-0.9.87/cdpcli/thirdparty/six.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.86/cdpcli/translate.py` & `cdpcli-beta-0.9.87/cdpcli/translate.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.86/cdpcli/utils.py` & `cdpcli-beta-0.9.87/cdpcli/utils.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.86/cdpcli/validate.py` & `cdpcli-beta-0.9.87/cdpcli/validate.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.86/cdpcli_beta.egg-info/PKG-INFO` & `cdpcli-beta-0.9.87/cdpcli_beta.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdpcli-beta
-Version: 0.9.86
+Version: 0.9.87
 Summary: Cloudera CDP Command Line Interface (BETA)
 Home-page: https://console.cdp.cloudera.com/
 Author: Cloudera, Inc.
 License: Apache License 2.0
 Description: # Cloudera CDP Command Line Interface
         
         This package provides a unified command line interface to the Cloudera Data
```

### Comparing `cdpcli-beta-0.9.86/cdpcli_beta.egg-info/SOURCES.txt` & `cdpcli-beta-0.9.87/cdpcli_beta.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.86/setup.py` & `cdpcli-beta-0.9.87/setup.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.86/setup_common.py` & `cdpcli-beta-0.9.87/setup_common.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.86/tests/unit/__init__.py` & `cdpcli-beta-0.9.87/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.86/tests/unit/cdp/__init__.py` & `cdpcli-beta-0.9.87/tests/unit/cdp/__init__.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.86/tests/unit/extensions/__init__.py` & `cdpcli-beta-0.9.87/tests/unit/extensions/__init__.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.86/tests/unit/extensions/configure/test_classify.py` & `cdpcli-beta-0.9.87/tests/unit/extensions/configure/test_classify.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.86/tests/unit/extensions/configure/test_configure.py` & `cdpcli-beta-0.9.87/tests/unit/extensions/configure/test_configure.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.86/tests/unit/extensions/configure/test_get.py` & `cdpcli-beta-0.9.87/tests/unit/extensions/configure/test_get.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.86/tests/unit/extensions/configure/test_list.py` & `cdpcli-beta-0.9.87/tests/unit/extensions/configure/test_list.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.86/tests/unit/extensions/configure/test_set.py` & `cdpcli-beta-0.9.87/tests/unit/extensions/configure/test_set.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.86/tests/unit/extensions/df/test_createdeployment.py` & `cdpcli-beta-0.9.87/tests/unit/extensions/df/test_createdeployment.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.86/tests/unit/extensions/df/test_upload_file.py` & `cdpcli-beta-0.9.87/tests/unit/extensions/df/test_upload_file.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.86/tests/unit/extensions/test_cliinputjson.py` & `cdpcli-beta-0.9.87/tests/unit/extensions/test_cliinputjson.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.86/tests/unit/extensions/test_df.py` & `cdpcli-beta-0.9.87/tests/unit/extensions/test_df.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.86/tests/unit/extensions/test_generatecliskeleton.py` & `cdpcli-beta-0.9.87/tests/unit/extensions/test_generatecliskeleton.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.86/tests/unit/extensions/test_interactivelogin.py` & `cdpcli-beta-0.9.87/tests/unit/extensions/test_interactivelogin.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.86/tests/unit/extensions/test_logout.py` & `cdpcli-beta-0.9.87/tests/unit/extensions/test_logout.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.86/tests/unit/extensions/test_operation_extension.py` & `cdpcli-beta-0.9.87/tests/unit/extensions/test_operation_extension.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.86/tests/unit/extensions/test_paginate.py` & `cdpcli-beta-0.9.87/tests/unit/extensions/test_paginate.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.86/tests/unit/extensions/test_redirect.py` & `cdpcli-beta-0.9.87/tests/unit/extensions/test_redirect.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.86/tests/unit/extensions/test_workload.py` & `cdpcli-beta-0.9.87/tests/unit/extensions/test_workload.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.86/tests/unit/extensions/test_writer.py` & `cdpcli-beta-0.9.87/tests/unit/extensions/test_writer.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.86/tests/unit/test_argparser.py` & `cdpcli-beta-0.9.87/tests/unit/test_argparser.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.86/tests/unit/test_argprocess.py` & `cdpcli-beta-0.9.87/tests/unit/test_argprocess.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.86/tests/unit/test_auth.py` & `cdpcli-beta-0.9.87/tests/unit/test_auth.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.86/tests/unit/test_cli_data.py` & `cdpcli-beta-0.9.87/tests/unit/test_cli_data.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.86/tests/unit/test_client.py` & `cdpcli-beta-0.9.87/tests/unit/test_client.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.86/tests/unit/test_completer.py` & `cdpcli-beta-0.9.87/tests/unit/test_completer.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.86/tests/unit/test_credentials.py` & `cdpcli-beta-0.9.87/tests/unit/test_credentials.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.86/tests/unit/test_docs.py` & `cdpcli-beta-0.9.87/tests/unit/test_docs.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.86/tests/unit/test_endpoint.py` & `cdpcli-beta-0.9.87/tests/unit/test_endpoint.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.86/tests/unit/test_help.py` & `cdpcli-beta-0.9.87/tests/unit/test_help.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.86/tests/unit/test_loaders.py` & `cdpcli-beta-0.9.87/tests/unit/test_loaders.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.86/tests/unit/test_model.py` & `cdpcli-beta-0.9.87/tests/unit/test_model.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.86/tests/unit/test_paginate.py` & `cdpcli-beta-0.9.87/tests/unit/test_paginate.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.86/tests/unit/test_paramfile.py` & `cdpcli-beta-0.9.87/tests/unit/test_paramfile.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.86/tests/unit/test_protocol.py` & `cdpcli-beta-0.9.87/tests/unit/test_protocol.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.86/tests/unit/test_retryhandler.py` & `cdpcli-beta-0.9.87/tests/unit/test_retryhandler.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.86/tests/unit/test_shorthand.py` & `cdpcli-beta-0.9.87/tests/unit/test_shorthand.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.86/tests/unit/test_signers.py` & `cdpcli-beta-0.9.87/tests/unit/test_signers.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.86/tests/unit/test_table_formatter.py` & `cdpcli-beta-0.9.87/tests/unit/test_table_formatter.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.86/tests/unit/test_utils.py` & `cdpcli-beta-0.9.87/tests/unit/test_utils.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.86/tests/unit/test_validate.py` & `cdpcli-beta-0.9.87/tests/unit/test_validate.py`

 * *Files identical despite different names*

### Comparing `cdpcli-beta-0.9.86/versioneer.py` & `cdpcli-beta-0.9.87/versioneer.py`

 * *Files identical despite different names*

