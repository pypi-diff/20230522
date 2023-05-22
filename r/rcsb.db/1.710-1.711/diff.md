# Comparing `tmp/rcsb.db-1.710.tar.gz` & `tmp/rcsb.db-1.711.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rcsb.db-1.710.tar", last modified: Tue May  9 22:05:52 2023, max compression
+gzip compressed data, was "rcsb.db-1.711.tar", last modified: Mon May 22 13:51:03 2023, max compression
```

## Comparing `rcsb.db-1.710.tar` & `rcsb.db-1.711.tar`

### file list

```diff
@@ -1,93 +1,93 @@
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-09 22:05:52.238813 rcsb.db-1.710/
--rw-r--r--   0 vsts      (1001) docker     (122)    29779 2023-05-09 21:43:20.000000 rcsb.db-1.710/HISTORY.txt
--rw-r--r--   0 vsts      (1001) docker     (122)      552 2023-05-09 21:43:20.000000 rcsb.db-1.710/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (122)      100 2023-05-09 21:43:20.000000 rcsb.db-1.710/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (122)    27551 2023-05-09 22:05:52.238813 rcsb.db-1.710/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (122)    26823 2023-05-09 21:43:20.000000 rcsb.db-1.710/README.md
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-09 22:05:52.226813 rcsb.db-1.710/rcsb/
--rw-r--r--   0 vsts      (1001) docker     (122)       65 2023-05-09 21:43:20.000000 rcsb.db-1.710/rcsb/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-09 22:05:52.226813 rcsb.db-1.710/rcsb/db/
--rw-r--r--   0 vsts      (1001) docker     (122)       65 2023-05-09 21:43:20.000000 rcsb.db-1.710/rcsb/db/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-09 22:05:52.230814 rcsb.db-1.710/rcsb/db/cli/
--rw-r--r--   0 vsts      (1001) docker     (122)     9528 2023-05-09 21:43:20.000000 rcsb.db-1.710/rcsb/db/cli/ETLExec.py
--rw-r--r--   0 vsts      (1001) docker     (122)     7657 2023-05-09 21:43:20.000000 rcsb.db-1.710/rcsb/db/cli/RepoHoldingsEtlWorker.py
--rw-r--r--   0 vsts      (1001) docker     (122)    22767 2023-05-09 21:43:20.000000 rcsb.db-1.710/rcsb/db/cli/RepoLoadExec.py
--rw-r--r--   0 vsts      (1001) docker     (122)    10064 2023-05-09 21:43:20.000000 rcsb.db-1.710/rcsb/db/cli/RepoScanExec.py
--rw-r--r--   0 vsts      (1001) docker     (122)    11316 2023-05-09 21:43:20.000000 rcsb.db-1.710/rcsb/db/cli/SchemaUpdateExec.py
--rw-r--r--   0 vsts      (1001) docker     (122)     8774 2023-05-09 21:43:20.000000 rcsb.db-1.710/rcsb/db/cli/SequenceClustersEtlWorker.py
--rw-r--r--   0 vsts      (1001) docker     (122)      155 2023-05-09 21:43:20.000000 rcsb.db-1.710/rcsb/db/cli/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-09 22:05:52.230814 rcsb.db-1.710/rcsb/db/cockroach/
--rw-r--r--   0 vsts      (1001) docker     (122)     9848 2023-05-09 21:43:20.000000 rcsb.db-1.710/rcsb/db/cockroach/CockroachDbLoader.py
--rw-r--r--   0 vsts      (1001) docker     (122)     9605 2023-05-09 21:43:20.000000 rcsb.db-1.710/rcsb/db/cockroach/CockroachDbUtil.py
--rw-r--r--   0 vsts      (1001) docker     (122)     5467 2023-05-09 21:43:20.000000 rcsb.db-1.710/rcsb/db/cockroach/Connection.py
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-05-09 21:43:20.000000 rcsb.db-1.710/rcsb/db/cockroach/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-09 22:05:52.230814 rcsb.db-1.710/rcsb/db/crate/
--rw-r--r--   0 vsts      (1001) docker     (122)     5142 2023-05-09 21:43:20.000000 rcsb.db-1.710/rcsb/db/crate/Connection.py
--rw-r--r--   0 vsts      (1001) docker     (122)     7987 2023-05-09 21:43:20.000000 rcsb.db-1.710/rcsb/db/crate/CrateDbLoader.py
--rw-r--r--   0 vsts      (1001) docker     (122)     9990 2023-05-09 21:43:20.000000 rcsb.db-1.710/rcsb/db/crate/CrateDbUtil.py
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-05-09 21:43:20.000000 rcsb.db-1.710/rcsb/db/crate/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-09 22:05:52.230814 rcsb.db-1.710/rcsb/db/define/
--rw-r--r--   0 vsts      (1001) docker     (122)    33223 2023-05-09 21:43:20.000000 rcsb.db-1.710/rcsb/db/define/ContentDefinition.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4169 2023-05-09 21:43:20.000000 rcsb.db-1.710/rcsb/db/define/DataTypeApiProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)    15211 2023-05-09 21:43:20.000000 rcsb.db-1.710/rcsb/db/define/DataTypeApplicationInfo.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4188 2023-05-09 21:43:20.000000 rcsb.db-1.710/rcsb/db/define/DataTypeInstanceInfo.py
--rw-r--r--   0 vsts      (1001) docker     (122)    34868 2023-05-09 21:43:20.000000 rcsb.db-1.710/rcsb/db/define/SchemaDefAccess.py
--rw-r--r--   0 vsts      (1001) docker     (122)    60184 2023-05-09 21:43:20.000000 rcsb.db-1.710/rcsb/db/define/SchemaDefBuild.py
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-05-09 21:43:20.000000 rcsb.db-1.710/rcsb/db/define/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-09 22:05:52.230814 rcsb.db-1.710/rcsb/db/helpers/
--rw-r--r--   0 vsts      (1001) docker     (122)    16974 2023-05-09 21:43:20.000000 rcsb.db-1.710/rcsb/db/helpers/ContentDefinitionHelper.py
--rw-r--r--   0 vsts      (1001) docker     (122)    34236 2023-05-09 21:43:20.000000 rcsb.db-1.710/rcsb/db/helpers/DocumentDefinitionHelper.py
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-05-09 21:43:20.000000 rcsb.db-1.710/rcsb/db/helpers/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1611 2023-05-09 21:43:20.000000 rcsb.db-1.710/rcsb/db/helpers/r.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-09 22:05:52.234814 rcsb.db-1.710/rcsb/db/mongo/
--rw-r--r--   0 vsts      (1001) docker     (122)     5655 2023-05-09 21:43:20.000000 rcsb.db-1.710/rcsb/db/mongo/Connection.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4938 2023-05-09 21:43:20.000000 rcsb.db-1.710/rcsb/db/mongo/ConnectionBase.py
--rw-r--r--   0 vsts      (1001) docker     (122)    15040 2023-05-09 21:43:20.000000 rcsb.db-1.710/rcsb/db/mongo/DocumentLoader.py
--rw-r--r--   0 vsts      (1001) docker     (122)    23696 2023-05-09 21:43:20.000000 rcsb.db-1.710/rcsb/db/mongo/MongoDbUtil.py
--rw-r--r--   0 vsts      (1001) docker     (122)    71183 2023-05-09 21:43:20.000000 rcsb.db-1.710/rcsb/db/mongo/PdbxLoader.py
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-05-09 21:43:20.000000 rcsb.db-1.710/rcsb/db/mongo/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-09 22:05:52.234814 rcsb.db-1.710/rcsb/db/mysql/
--rw-r--r--   0 vsts      (1001) docker     (122)     2832 2023-05-09 21:43:20.000000 rcsb.db-1.710/rcsb/db/mysql/Connection.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4258 2023-05-09 21:43:20.000000 rcsb.db-1.710/rcsb/db/mysql/ConnectionBase.py
--rw-r--r--   0 vsts      (1001) docker     (122)    18626 2023-05-09 21:43:20.000000 rcsb.db-1.710/rcsb/db/mysql/MyDbAdapter.py
--rw-r--r--   0 vsts      (1001) docker     (122)    12211 2023-05-09 21:43:20.000000 rcsb.db-1.710/rcsb/db/mysql/MyDbUtil.py
--rw-r--r--   0 vsts      (1001) docker     (122)     5169 2023-05-09 21:43:20.000000 rcsb.db-1.710/rcsb/db/mysql/MysqlSchemaImporter.py
--rw-r--r--   0 vsts      (1001) docker     (122)    19129 2023-05-09 21:43:20.000000 rcsb.db-1.710/rcsb/db/mysql/SchemaDefLoader.py
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-05-09 21:43:20.000000 rcsb.db-1.710/rcsb/db/mysql/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-09 22:05:52.234814 rcsb.db-1.710/rcsb/db/processors/
--rw-r--r--   0 vsts      (1001) docker     (122)     7467 2023-05-09 21:43:20.000000 rcsb.db-1.710/rcsb/db/processors/ClusterDataPrep.py
--rw-r--r--   0 vsts      (1001) docker     (122)     5081 2023-05-09 21:43:20.000000 rcsb.db-1.710/rcsb/db/processors/DataExchangeStatus.py
--rw-r--r--   0 vsts      (1001) docker     (122)    19485 2023-05-09 21:43:20.000000 rcsb.db-1.710/rcsb/db/processors/DataTransformFactory.py
--rw-r--r--   0 vsts      (1001) docker     (122)    31322 2023-05-09 21:43:20.000000 rcsb.db-1.710/rcsb/db/processors/RepoHoldingsDataPrep.py
--rw-r--r--   0 vsts      (1001) docker     (122)     7596 2023-05-09 21:43:20.000000 rcsb.db-1.710/rcsb/db/processors/RepoHoldingsRemoteDataPrep.py
--rw-r--r--   0 vsts      (1001) docker     (122)    40786 2023-05-09 21:43:20.000000 rcsb.db-1.710/rcsb/db/processors/SchemaDefDataPrep.py
--rw-r--r--   0 vsts      (1001) docker     (122)    26654 2023-05-09 21:43:20.000000 rcsb.db-1.710/rcsb/db/processors/SchemaDefReShape.py
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-05-09 21:43:20.000000 rcsb.db-1.710/rcsb/db/processors/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-09 22:05:52.234814 rcsb.db-1.710/rcsb/db/sql/
--rw-r--r--   0 vsts      (1001) docker     (122)    23627 2023-05-09 21:43:20.000000 rcsb.db-1.710/rcsb/db/sql/QueryDirectives.py
--rw-r--r--   0 vsts      (1001) docker     (122)    40731 2023-05-09 21:43:20.000000 rcsb.db-1.710/rcsb/db/sql/SqlGen.py
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-05-09 21:43:20.000000 rcsb.db-1.710/rcsb/db/sql/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-09 22:05:52.238813 rcsb.db-1.710/rcsb/db/utils/
--rw-r--r--   0 vsts      (1001) docker     (122)     2696 2023-05-09 21:43:20.000000 rcsb.db-1.710/rcsb/db/utils/CaseNormalizedDict.py
--rw-r--r--   0 vsts      (1001) docker     (122)    12446 2023-05-09 21:43:20.000000 rcsb.db-1.710/rcsb/db/utils/PdbxSchemaMapReader.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3683 2023-05-09 21:43:20.000000 rcsb.db-1.710/rcsb/db/utils/ProvenanceProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)    22110 2023-05-09 21:43:20.000000 rcsb.db-1.710/rcsb/db/utils/SchemaProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1353 2023-05-09 21:43:20.000000 rcsb.db-1.710/rcsb/db/utils/TextUtil.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2172 2023-05-09 21:43:20.000000 rcsb.db-1.710/rcsb/db/utils/TimeUtil.py
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-05-09 21:43:20.000000 rcsb.db-1.710/rcsb/db/utils/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1614 2023-05-09 21:43:20.000000 rcsb.db-1.710/rcsb/db/utils/makePathList.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1055 2023-05-09 21:43:20.000000 rcsb.db-1.710/rcsb/db/utils/unescape.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-09 22:05:52.238813 rcsb.db-1.710/rcsb/db/wf/
--rw-r--r--   0 vsts      (1001) docker     (122)    11438 2023-05-09 21:43:20.000000 rcsb.db-1.710/rcsb/db/wf/RepoLoadWorkflow.py
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-05-09 21:43:20.000000 rcsb.db-1.710/rcsb/db/wf/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-09 22:05:52.226813 rcsb.db-1.710/rcsb.db.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (122)    27551 2023-05-09 22:05:52.000000 rcsb.db-1.710/rcsb.db.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (122)     2298 2023-05-09 22:05:52.000000 rcsb.db-1.710/rcsb.db.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-05-09 22:05:52.000000 rcsb.db-1.710/rcsb.db.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (122)      209 2023-05-09 22:05:52.000000 rcsb.db-1.710/rcsb.db.egg-info/entry_points.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-05-09 21:52:46.000000 rcsb.db-1.710/rcsb.db.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (122)      437 2023-05-09 22:05:52.000000 rcsb.db-1.710/rcsb.db.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        5 2023-05-09 22:05:52.000000 rcsb.db-1.710/rcsb.db.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (122)      513 2023-05-09 21:43:20.000000 rcsb.db-1.710/requirements.txt
--rwxr-xr-x   0 vsts      (1001) docker     (122)      108 2023-05-09 22:05:52.238813 rcsb.db-1.710/setup.cfg
--rwxr-xr-x   0 vsts      (1001) docker     (122)     2876 2023-05-09 21:43:20.000000 rcsb.db-1.710/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-22 13:51:03.555400 rcsb.db-1.711/
+-rw-r--r--   0 vsts      (1001) docker     (122)    29825 2023-05-22 13:35:22.000000 rcsb.db-1.711/HISTORY.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)      552 2023-05-22 13:35:22.000000 rcsb.db-1.711/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (122)      100 2023-05-22 13:35:22.000000 rcsb.db-1.711/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (122)    27551 2023-05-22 13:51:03.555400 rcsb.db-1.711/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (122)    26823 2023-05-22 13:35:22.000000 rcsb.db-1.711/README.md
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-22 13:51:03.547400 rcsb.db-1.711/rcsb/
+-rw-r--r--   0 vsts      (1001) docker     (122)       65 2023-05-22 13:35:22.000000 rcsb.db-1.711/rcsb/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-22 13:51:03.547400 rcsb.db-1.711/rcsb/db/
+-rw-r--r--   0 vsts      (1001) docker     (122)       65 2023-05-22 13:35:22.000000 rcsb.db-1.711/rcsb/db/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-22 13:51:03.551400 rcsb.db-1.711/rcsb/db/cli/
+-rw-r--r--   0 vsts      (1001) docker     (122)     9528 2023-05-22 13:35:22.000000 rcsb.db-1.711/rcsb/db/cli/ETLExec.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     7661 2023-05-22 13:35:22.000000 rcsb.db-1.711/rcsb/db/cli/RepoHoldingsEtlWorker.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    22767 2023-05-22 13:35:22.000000 rcsb.db-1.711/rcsb/db/cli/RepoLoadExec.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    10064 2023-05-22 13:35:22.000000 rcsb.db-1.711/rcsb/db/cli/RepoScanExec.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    11316 2023-05-22 13:35:22.000000 rcsb.db-1.711/rcsb/db/cli/SchemaUpdateExec.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     8774 2023-05-22 13:35:22.000000 rcsb.db-1.711/rcsb/db/cli/SequenceClustersEtlWorker.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      155 2023-05-22 13:35:22.000000 rcsb.db-1.711/rcsb/db/cli/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-22 13:51:03.551400 rcsb.db-1.711/rcsb/db/cockroach/
+-rw-r--r--   0 vsts      (1001) docker     (122)     9848 2023-05-22 13:35:22.000000 rcsb.db-1.711/rcsb/db/cockroach/CockroachDbLoader.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     9605 2023-05-22 13:35:22.000000 rcsb.db-1.711/rcsb/db/cockroach/CockroachDbUtil.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     5467 2023-05-22 13:35:22.000000 rcsb.db-1.711/rcsb/db/cockroach/Connection.py
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-05-22 13:35:22.000000 rcsb.db-1.711/rcsb/db/cockroach/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-22 13:51:03.551400 rcsb.db-1.711/rcsb/db/crate/
+-rw-r--r--   0 vsts      (1001) docker     (122)     5142 2023-05-22 13:35:22.000000 rcsb.db-1.711/rcsb/db/crate/Connection.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     7987 2023-05-22 13:35:22.000000 rcsb.db-1.711/rcsb/db/crate/CrateDbLoader.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     9990 2023-05-22 13:35:22.000000 rcsb.db-1.711/rcsb/db/crate/CrateDbUtil.py
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-05-22 13:35:22.000000 rcsb.db-1.711/rcsb/db/crate/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-22 13:51:03.551400 rcsb.db-1.711/rcsb/db/define/
+-rw-r--r--   0 vsts      (1001) docker     (122)    33223 2023-05-22 13:35:22.000000 rcsb.db-1.711/rcsb/db/define/ContentDefinition.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4169 2023-05-22 13:35:22.000000 rcsb.db-1.711/rcsb/db/define/DataTypeApiProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    15211 2023-05-22 13:35:22.000000 rcsb.db-1.711/rcsb/db/define/DataTypeApplicationInfo.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4188 2023-05-22 13:35:22.000000 rcsb.db-1.711/rcsb/db/define/DataTypeInstanceInfo.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    34868 2023-05-22 13:35:22.000000 rcsb.db-1.711/rcsb/db/define/SchemaDefAccess.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    60184 2023-05-22 13:35:22.000000 rcsb.db-1.711/rcsb/db/define/SchemaDefBuild.py
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-05-22 13:35:22.000000 rcsb.db-1.711/rcsb/db/define/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-22 13:51:03.551400 rcsb.db-1.711/rcsb/db/helpers/
+-rw-r--r--   0 vsts      (1001) docker     (122)    16974 2023-05-22 13:35:22.000000 rcsb.db-1.711/rcsb/db/helpers/ContentDefinitionHelper.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    34236 2023-05-22 13:35:22.000000 rcsb.db-1.711/rcsb/db/helpers/DocumentDefinitionHelper.py
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-05-22 13:35:22.000000 rcsb.db-1.711/rcsb/db/helpers/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1611 2023-05-22 13:35:22.000000 rcsb.db-1.711/rcsb/db/helpers/r.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-22 13:51:03.551400 rcsb.db-1.711/rcsb/db/mongo/
+-rw-r--r--   0 vsts      (1001) docker     (122)     5655 2023-05-22 13:35:22.000000 rcsb.db-1.711/rcsb/db/mongo/Connection.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4938 2023-05-22 13:35:22.000000 rcsb.db-1.711/rcsb/db/mongo/ConnectionBase.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    15040 2023-05-22 13:35:22.000000 rcsb.db-1.711/rcsb/db/mongo/DocumentLoader.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    23696 2023-05-22 13:35:22.000000 rcsb.db-1.711/rcsb/db/mongo/MongoDbUtil.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    71183 2023-05-22 13:35:22.000000 rcsb.db-1.711/rcsb/db/mongo/PdbxLoader.py
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-05-22 13:35:22.000000 rcsb.db-1.711/rcsb/db/mongo/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-22 13:51:03.555400 rcsb.db-1.711/rcsb/db/mysql/
+-rw-r--r--   0 vsts      (1001) docker     (122)     2832 2023-05-22 13:35:22.000000 rcsb.db-1.711/rcsb/db/mysql/Connection.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4258 2023-05-22 13:35:22.000000 rcsb.db-1.711/rcsb/db/mysql/ConnectionBase.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    18626 2023-05-22 13:35:22.000000 rcsb.db-1.711/rcsb/db/mysql/MyDbAdapter.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    12211 2023-05-22 13:35:22.000000 rcsb.db-1.711/rcsb/db/mysql/MyDbUtil.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     5169 2023-05-22 13:35:22.000000 rcsb.db-1.711/rcsb/db/mysql/MysqlSchemaImporter.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    19129 2023-05-22 13:35:22.000000 rcsb.db-1.711/rcsb/db/mysql/SchemaDefLoader.py
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-05-22 13:35:22.000000 rcsb.db-1.711/rcsb/db/mysql/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-22 13:51:03.555400 rcsb.db-1.711/rcsb/db/processors/
+-rw-r--r--   0 vsts      (1001) docker     (122)     7467 2023-05-22 13:35:22.000000 rcsb.db-1.711/rcsb/db/processors/ClusterDataPrep.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     5081 2023-05-22 13:35:22.000000 rcsb.db-1.711/rcsb/db/processors/DataExchangeStatus.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    19485 2023-05-22 13:35:22.000000 rcsb.db-1.711/rcsb/db/processors/DataTransformFactory.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    31322 2023-05-22 13:35:22.000000 rcsb.db-1.711/rcsb/db/processors/RepoHoldingsDataPrep.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     7596 2023-05-22 13:35:22.000000 rcsb.db-1.711/rcsb/db/processors/RepoHoldingsRemoteDataPrep.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    40786 2023-05-22 13:35:22.000000 rcsb.db-1.711/rcsb/db/processors/SchemaDefDataPrep.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    26654 2023-05-22 13:35:22.000000 rcsb.db-1.711/rcsb/db/processors/SchemaDefReShape.py
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-05-22 13:35:22.000000 rcsb.db-1.711/rcsb/db/processors/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-22 13:51:03.555400 rcsb.db-1.711/rcsb/db/sql/
+-rw-r--r--   0 vsts      (1001) docker     (122)    23627 2023-05-22 13:35:22.000000 rcsb.db-1.711/rcsb/db/sql/QueryDirectives.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    40731 2023-05-22 13:35:22.000000 rcsb.db-1.711/rcsb/db/sql/SqlGen.py
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-05-22 13:35:22.000000 rcsb.db-1.711/rcsb/db/sql/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-22 13:51:03.555400 rcsb.db-1.711/rcsb/db/utils/
+-rw-r--r--   0 vsts      (1001) docker     (122)     2696 2023-05-22 13:35:22.000000 rcsb.db-1.711/rcsb/db/utils/CaseNormalizedDict.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    12446 2023-05-22 13:35:22.000000 rcsb.db-1.711/rcsb/db/utils/PdbxSchemaMapReader.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3683 2023-05-22 13:35:22.000000 rcsb.db-1.711/rcsb/db/utils/ProvenanceProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    22110 2023-05-22 13:35:22.000000 rcsb.db-1.711/rcsb/db/utils/SchemaProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1353 2023-05-22 13:35:22.000000 rcsb.db-1.711/rcsb/db/utils/TextUtil.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2172 2023-05-22 13:35:22.000000 rcsb.db-1.711/rcsb/db/utils/TimeUtil.py
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-05-22 13:35:22.000000 rcsb.db-1.711/rcsb/db/utils/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1614 2023-05-22 13:35:22.000000 rcsb.db-1.711/rcsb/db/utils/makePathList.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1055 2023-05-22 13:35:22.000000 rcsb.db-1.711/rcsb/db/utils/unescape.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-22 13:51:03.555400 rcsb.db-1.711/rcsb/db/wf/
+-rw-r--r--   0 vsts      (1001) docker     (122)    11438 2023-05-22 13:35:22.000000 rcsb.db-1.711/rcsb/db/wf/RepoLoadWorkflow.py
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-05-22 13:35:22.000000 rcsb.db-1.711/rcsb/db/wf/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-22 13:51:03.547400 rcsb.db-1.711/rcsb.db.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (122)    27551 2023-05-22 13:51:03.000000 rcsb.db-1.711/rcsb.db.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (122)     2298 2023-05-22 13:51:03.000000 rcsb.db-1.711/rcsb.db.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-05-22 13:51:03.000000 rcsb.db-1.711/rcsb.db.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)      209 2023-05-22 13:51:03.000000 rcsb.db-1.711/rcsb.db.egg-info/entry_points.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-05-22 13:39:26.000000 rcsb.db-1.711/rcsb.db.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (122)      437 2023-05-22 13:51:03.000000 rcsb.db-1.711/rcsb.db.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        5 2023-05-22 13:51:03.000000 rcsb.db-1.711/rcsb.db.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)      513 2023-05-22 13:35:22.000000 rcsb.db-1.711/requirements.txt
+-rwxr-xr-x   0 vsts      (1001) docker     (122)      108 2023-05-22 13:51:03.555400 rcsb.db-1.711/setup.cfg
+-rwxr-xr-x   0 vsts      (1001) docker     (122)     2876 2023-05-22 13:35:22.000000 rcsb.db-1.711/setup.py
```

### Comparing `rcsb.db-1.710/HISTORY.txt` & `rcsb.db-1.711/HISTORY.txt`

 * *Files 1% similar despite different names*

```diff
@@ -341,7 +341,8 @@
  26-Jan-2023  V1.704 Update MA_DICT_LOCATOR path in exdb-config-example.yml and add uchar5 to DataTypeApplicationInfo.py
  30-Jan-2023  V1.705 Update requirements (pin SQLAlchemy)
  14-Feb-2023  V1.706 Updates to PdbxLoader and RepoLoadWorkflow to support resumability of core data loading tasks
  22-Feb-2023  V1.707 Updates to PdbxLoader to use case-sensitivity for brute force document purge
  06-Apr-2023  V1.708 Add support for entity_id_list cifType in DataTypeApplicationInfo
  26-Apr-2023  V1.709 Fix document pre-purge regex during load, and add regexPurge flag to control running that step
   8-May-2023  V1.710 Fix error handling in PdbxLoader to cause failure when documents fail to load
+ 19-May-2023  V1.711 Update DNS to PDB archive
```

### Comparing `rcsb.db-1.710/LICENSE` & `rcsb.db-1.711/LICENSE`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.710/PKG-INFO` & `rcsb.db-1.711/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rcsb.db
-Version: 1.710
+Version: 1.711
 Summary: RCSB Python Database Access and Loading Utility Classes
 Home-page: https://github.com/rcsb/py-rcsb_db
 Author: John Westbrook
 Author-email: john.westbrook@rcsb.org
 License: Apache 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `rcsb.db-1.710/README.md` & `rcsb.db-1.711/README.md`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.710/rcsb/db/cli/ETLExec.py` & `rcsb.db-1.711/rcsb/db/cli/ETLExec.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.710/rcsb/db/cli/RepoHoldingsEtlWorker.py` & `rcsb.db-1.711/rcsb/db/cli/RepoHoldingsEtlWorker.py`

 * *Files 2% similar despite different names*

```diff
@@ -78,16 +78,16 @@
         try:
             self.__statusList = []
             desp = DataExchangeStatus()
             statusStartTimestamp = desp.setStartTime()
 
             discoveryMode = self.__cfgOb.get("DISCOVERY_MODE", sectionName=self.__cfgSectionName, default="local")
             # ---
-            baseUrlPDB = self.__cfgOb.getPath("PDB_REPO_URL", sectionName=self.__cfgSectionName, default="https://ftp.wwpdb.org/pub")
-            fallbackUrlPDB = self.__cfgOb.getPath("PDB_REPO_FALLBACK_URL", sectionName=self.__cfgSectionName, default="https://ftp.wwpdb.org/pub")
+            baseUrlPDB = self.__cfgOb.getPath("PDB_REPO_URL", sectionName=self.__cfgSectionName, default="https://files.wwpdb.org/pub")
+            fallbackUrlPDB = self.__cfgOb.getPath("PDB_REPO_FALLBACK_URL", sectionName=self.__cfgSectionName, default="https://files.wwpdb.org/pub")
             edMapUrl = self.__cfgOb.getPath("RCSB_EDMAP_LIST_PATH", sectionName=self.__cfgSectionName, default=None)
             #
             kwD = {
                 "holdingsTargetUrl": os.path.join(baseUrlPDB, "pdb", "holdings"),
                 "holdingsFallbackUrl": os.path.join(fallbackUrlPDB, "pdb", "holdings"),
                 "edmapsLocator": edMapUrl,
                 "updateTargetUrl": os.path.join(baseUrlPDB, "pdb", "data", "status", "latest"),
```

### Comparing `rcsb.db-1.710/rcsb/db/cli/RepoLoadExec.py` & `rcsb.db-1.711/rcsb/db/cli/RepoLoadExec.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.710/rcsb/db/cli/RepoScanExec.py` & `rcsb.db-1.711/rcsb/db/cli/RepoScanExec.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.710/rcsb/db/cli/SchemaUpdateExec.py` & `rcsb.db-1.711/rcsb/db/cli/SchemaUpdateExec.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.710/rcsb/db/cli/SequenceClustersEtlWorker.py` & `rcsb.db-1.711/rcsb/db/cli/SequenceClustersEtlWorker.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.710/rcsb/db/cockroach/CockroachDbLoader.py` & `rcsb.db-1.711/rcsb/db/cockroach/CockroachDbLoader.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.710/rcsb/db/cockroach/CockroachDbUtil.py` & `rcsb.db-1.711/rcsb/db/cockroach/CockroachDbUtil.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.710/rcsb/db/cockroach/Connection.py` & `rcsb.db-1.711/rcsb/db/cockroach/Connection.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.710/rcsb/db/crate/Connection.py` & `rcsb.db-1.711/rcsb/db/crate/Connection.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.710/rcsb/db/crate/CrateDbLoader.py` & `rcsb.db-1.711/rcsb/db/crate/CrateDbLoader.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.710/rcsb/db/crate/CrateDbUtil.py` & `rcsb.db-1.711/rcsb/db/crate/CrateDbUtil.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.710/rcsb/db/define/ContentDefinition.py` & `rcsb.db-1.711/rcsb/db/define/ContentDefinition.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.710/rcsb/db/define/DataTypeApiProvider.py` & `rcsb.db-1.711/rcsb/db/define/DataTypeApiProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.710/rcsb/db/define/DataTypeApplicationInfo.py` & `rcsb.db-1.711/rcsb/db/define/DataTypeApplicationInfo.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.710/rcsb/db/define/DataTypeInstanceInfo.py` & `rcsb.db-1.711/rcsb/db/define/DataTypeInstanceInfo.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.710/rcsb/db/define/SchemaDefAccess.py` & `rcsb.db-1.711/rcsb/db/define/SchemaDefAccess.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.710/rcsb/db/define/SchemaDefBuild.py` & `rcsb.db-1.711/rcsb/db/define/SchemaDefBuild.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.710/rcsb/db/helpers/ContentDefinitionHelper.py` & `rcsb.db-1.711/rcsb/db/helpers/ContentDefinitionHelper.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.710/rcsb/db/helpers/DocumentDefinitionHelper.py` & `rcsb.db-1.711/rcsb/db/helpers/DocumentDefinitionHelper.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.710/rcsb/db/helpers/r.py` & `rcsb.db-1.711/rcsb/db/helpers/r.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.710/rcsb/db/mongo/Connection.py` & `rcsb.db-1.711/rcsb/db/mongo/Connection.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.710/rcsb/db/mongo/ConnectionBase.py` & `rcsb.db-1.711/rcsb/db/mongo/ConnectionBase.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.710/rcsb/db/mongo/DocumentLoader.py` & `rcsb.db-1.711/rcsb/db/mongo/DocumentLoader.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.710/rcsb/db/mongo/MongoDbUtil.py` & `rcsb.db-1.711/rcsb/db/mongo/MongoDbUtil.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.710/rcsb/db/mongo/PdbxLoader.py` & `rcsb.db-1.711/rcsb/db/mongo/PdbxLoader.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.710/rcsb/db/mysql/Connection.py` & `rcsb.db-1.711/rcsb/db/mysql/Connection.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.710/rcsb/db/mysql/ConnectionBase.py` & `rcsb.db-1.711/rcsb/db/mysql/ConnectionBase.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.710/rcsb/db/mysql/MyDbAdapter.py` & `rcsb.db-1.711/rcsb/db/mysql/MyDbAdapter.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.710/rcsb/db/mysql/MyDbUtil.py` & `rcsb.db-1.711/rcsb/db/mysql/MyDbUtil.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.710/rcsb/db/mysql/MysqlSchemaImporter.py` & `rcsb.db-1.711/rcsb/db/mysql/MysqlSchemaImporter.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.710/rcsb/db/mysql/SchemaDefLoader.py` & `rcsb.db-1.711/rcsb/db/mysql/SchemaDefLoader.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.710/rcsb/db/processors/ClusterDataPrep.py` & `rcsb.db-1.711/rcsb/db/processors/ClusterDataPrep.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.710/rcsb/db/processors/DataExchangeStatus.py` & `rcsb.db-1.711/rcsb/db/processors/DataExchangeStatus.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.710/rcsb/db/processors/DataTransformFactory.py` & `rcsb.db-1.711/rcsb/db/processors/DataTransformFactory.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.710/rcsb/db/processors/RepoHoldingsDataPrep.py` & `rcsb.db-1.711/rcsb/db/processors/RepoHoldingsDataPrep.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.710/rcsb/db/processors/RepoHoldingsRemoteDataPrep.py` & `rcsb.db-1.711/rcsb/db/processors/RepoHoldingsRemoteDataPrep.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.710/rcsb/db/processors/SchemaDefDataPrep.py` & `rcsb.db-1.711/rcsb/db/processors/SchemaDefDataPrep.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.710/rcsb/db/processors/SchemaDefReShape.py` & `rcsb.db-1.711/rcsb/db/processors/SchemaDefReShape.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.710/rcsb/db/sql/QueryDirectives.py` & `rcsb.db-1.711/rcsb/db/sql/QueryDirectives.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.710/rcsb/db/sql/SqlGen.py` & `rcsb.db-1.711/rcsb/db/sql/SqlGen.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.710/rcsb/db/utils/CaseNormalizedDict.py` & `rcsb.db-1.711/rcsb/db/utils/CaseNormalizedDict.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.710/rcsb/db/utils/PdbxSchemaMapReader.py` & `rcsb.db-1.711/rcsb/db/utils/PdbxSchemaMapReader.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.710/rcsb/db/utils/ProvenanceProvider.py` & `rcsb.db-1.711/rcsb/db/utils/ProvenanceProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.710/rcsb/db/utils/SchemaProvider.py` & `rcsb.db-1.711/rcsb/db/utils/SchemaProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.710/rcsb/db/utils/TextUtil.py` & `rcsb.db-1.711/rcsb/db/utils/TextUtil.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.710/rcsb/db/utils/TimeUtil.py` & `rcsb.db-1.711/rcsb/db/utils/TimeUtil.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.710/rcsb/db/utils/makePathList.py` & `rcsb.db-1.711/rcsb/db/utils/makePathList.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.710/rcsb/db/utils/unescape.py` & `rcsb.db-1.711/rcsb/db/utils/unescape.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.710/rcsb/db/wf/RepoLoadWorkflow.py` & `rcsb.db-1.711/rcsb/db/wf/RepoLoadWorkflow.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.710/rcsb.db.egg-info/PKG-INFO` & `rcsb.db-1.711/rcsb.db.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rcsb.db
-Version: 1.710
+Version: 1.711
 Summary: RCSB Python Database Access and Loading Utility Classes
 Home-page: https://github.com/rcsb/py-rcsb_db
 Author: John Westbrook
 Author-email: john.westbrook@rcsb.org
 License: Apache 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `rcsb.db-1.710/rcsb.db.egg-info/SOURCES.txt` & `rcsb.db-1.711/rcsb.db.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.710/requirements.txt` & `rcsb.db-1.711/requirements.txt`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.710/setup.py` & `rcsb.db-1.711/setup.py`

 * *Files identical despite different names*

