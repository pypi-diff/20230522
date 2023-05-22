# Comparing `tmp/dumpulator-0.2.4.tar.gz` & `tmp/dumpulator-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dumpulator-0.2.4.tar", last modified: Sat May  6 15:05:59 2023, max compression
+gzip compressed data, was "dumpulator-0.2.5.tar", last modified: Mon May 22 14:08:28 2023, max compression
```

## Comparing `dumpulator-0.2.4.tar` & `dumpulator-0.2.5.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 15:05:59.511441 dumpulator-0.2.4/
--rw-r--r--   0 runner    (1001) docker     (122)     1359 2023-05-06 15:05:58.000000 dumpulator-0.2.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)    10452 2023-05-06 15:05:59.511441 dumpulator-0.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    10080 2023-05-06 15:05:58.000000 dumpulator-0.2.4/README.md
--rw-r--r--   0 runner    (1001) docker     (122)      206 2023-05-06 15:05:58.000000 dumpulator-0.2.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)      802 2023-05-06 15:05:59.515442 dumpulator-0.2.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1588 2023-05-06 15:05:58.000000 dumpulator-0.2.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 15:05:59.499441 dumpulator-0.2.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 15:05:59.503441 dumpulator-0.2.4/src/dumpulator/
--rw-r--r--   0 runner    (1001) docker     (122)      116 2023-05-06 15:05:58.000000 dumpulator-0.2.4/src/dumpulator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    21634 2023-05-06 15:05:58.000000 dumpulator-0.2.4/src/dumpulator/details.py
--rw-r--r--   0 runner    (1001) docker     (122)    79009 2023-05-06 15:05:58.000000 dumpulator-0.2.4/src/dumpulator/dumpulator.py
--rw-r--r--   0 runner    (1001) docker     (122)    10865 2023-05-06 15:05:58.000000 dumpulator-0.2.4/src/dumpulator/handles.py
--rw-r--r--   0 runner    (1001) docker     (122)    16598 2023-05-06 15:05:58.000000 dumpulator-0.2.4/src/dumpulator/memory.py
--rw-r--r--   0 runner    (1001) docker     (122)     5442 2023-05-06 15:05:58.000000 dumpulator-0.2.4/src/dumpulator/modules.py
--rw-r--r--   0 runner    (1001) docker     (122)    21591 2023-05-06 15:05:58.000000 dumpulator-0.2.4/src/dumpulator/native.py
--rw-r--r--   0 runner    (1001) docker     (122)     3924 2023-05-06 15:05:58.000000 dumpulator-0.2.4/src/dumpulator/ntdevices.py
--rw-r--r--   0 runner    (1001) docker     (122)   123193 2023-05-06 15:05:58.000000 dumpulator-0.2.4/src/dumpulator/ntenums.py
--rw-r--r--   0 runner    (1001) docker     (122)    13633 2023-05-06 15:05:58.000000 dumpulator-0.2.4/src/dumpulator/ntprimitives.py
--rw-r--r--   0 runner    (1001) docker     (122)     3826 2023-05-06 15:05:58.000000 dumpulator-0.2.4/src/dumpulator/ntstructs.py
--rw-r--r--   0 runner    (1001) docker     (122)   235727 2023-05-06 15:05:58.000000 dumpulator-0.2.4/src/dumpulator/ntsyscalls.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 15:05:59.503441 dumpulator-0.2.4/src/dumpulator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    10452 2023-05-06 15:05:59.000000 dumpulator-0.2.4/src/dumpulator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2301 2023-05-06 15:05:59.000000 dumpulator-0.2.4/src/dumpulator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-06 15:05:59.000000 dumpulator-0.2.4/src/dumpulator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       48 2023-05-06 15:05:59.000000 dumpulator-0.2.4/src/dumpulator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       20 2023-05-06 15:05:59.000000 dumpulator-0.2.4/src/dumpulator.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 15:05:59.507441 dumpulator-0.2.4/src/minidump/
--rw-r--r--   0 runner    (1001) docker     (122)     3269 2023-05-06 15:05:58.000000 dumpulator-0.2.4/src/minidump/__amain__.py
--rw-r--r--   0 runner    (1001) docker     (122)       17 2023-05-06 15:05:58.000000 dumpulator-0.2.4/src/minidump/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3501 2023-05-06 15:05:58.000000 dumpulator-0.2.4/src/minidump/__main__.py
--rw-r--r--   0 runner    (1001) docker     (122)      132 2023-05-06 15:05:58.000000 dumpulator-0.2.4/src/minidump/_version.py
--rw-r--r--   0 runner    (1001) docker     (122)     9689 2023-05-06 15:05:58.000000 dumpulator-0.2.4/src/minidump/aminidumpfile.py
--rw-r--r--   0 runner    (1001) docker     (122)    11501 2023-05-06 15:05:58.000000 dumpulator-0.2.4/src/minidump/aminidumpreader.py
--rw-r--r--   0 runner    (1001) docker     (122)     9452 2023-05-06 15:05:58.000000 dumpulator-0.2.4/src/minidump/common_structs.py
--rw-r--r--   0 runner    (1001) docker     (122)     2387 2023-05-06 15:05:58.000000 dumpulator-0.2.4/src/minidump/constants.py
--rw-r--r--   0 runner    (1001) docker     (122)     2349 2023-05-06 15:05:58.000000 dumpulator-0.2.4/src/minidump/directory.py
--rw-r--r--   0 runner    (1001) docker     (122)      293 2023-05-06 15:05:58.000000 dumpulator-0.2.4/src/minidump/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)     2828 2023-05-06 15:05:58.000000 dumpulator-0.2.4/src/minidump/header.py
--rw-r--r--   0 runner    (1001) docker     (122)     9818 2023-05-06 15:05:58.000000 dumpulator-0.2.4/src/minidump/minidumpfile.py
--rw-r--r--   0 runner    (1001) docker     (122)    11724 2023-05-06 15:05:58.000000 dumpulator-0.2.4/src/minidump/minidumpreader.py
--rw-r--r--   0 runner    (1001) docker     (122)     5238 2023-05-06 15:05:58.000000 dumpulator-0.2.4/src/minidump/minidumpshell.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 15:05:59.511441 dumpulator-0.2.4/src/minidump/streams/
--rw-r--r--   0 runner    (1001) docker     (122)      599 2023-05-06 15:05:58.000000 dumpulator-0.2.4/src/minidump/streams/CommentStreamA.py
--rw-r--r--   0 runner    (1001) docker     (122)      627 2023-05-06 15:05:58.000000 dumpulator-0.2.4/src/minidump/streams/CommentStreamW.py
--rw-r--r--   0 runner    (1001) docker     (122)    25274 2023-05-06 15:05:58.000000 dumpulator-0.2.4/src/minidump/streams/ContextStream.py
--rw-r--r--   0 runner    (1001) docker     (122)    11428 2023-05-06 15:05:58.000000 dumpulator-0.2.4/src/minidump/streams/ExceptionStream.py
--rw-r--r--   0 runner    (1001) docker     (122)      975 2023-05-06 15:05:58.000000 dumpulator-0.2.4/src/minidump/streams/FunctionTableStream.py
--rw-r--r--   0 runner    (1001) docker     (122)     8898 2023-05-06 15:05:58.000000 dumpulator-0.2.4/src/minidump/streams/HandleDataStream.py
--rw-r--r--   0 runner    (1001) docker     (122)      682 2023-05-06 15:05:58.000000 dumpulator-0.2.4/src/minidump/streams/HandleOperationListStream.py
--rw-r--r--   0 runner    (1001) docker     (122)       86 2023-05-06 15:05:58.000000 dumpulator-0.2.4/src/minidump/streams/JavaScriptDataStream.py
--rw-r--r--   0 runner    (1001) docker     (122)      549 2023-05-06 15:05:58.000000 dumpulator-0.2.4/src/minidump/streams/LastReservedStream.py
--rw-r--r--   0 runner    (1001) docker     (122)     3211 2023-05-06 15:05:58.000000 dumpulator-0.2.4/src/minidump/streams/Memory64ListStream.py
--rw-r--r--   0 runner    (1001) docker     (122)    12503 2023-05-06 15:05:58.000000 dumpulator-0.2.4/src/minidump/streams/MemoryInfoListStream.py
--rw-r--r--   0 runner    (1001) docker     (122)     3252 2023-05-06 15:05:58.000000 dumpulator-0.2.4/src/minidump/streams/MemoryListStream.py
--rw-r--r--   0 runner    (1001) docker     (122)     6684 2023-05-06 15:05:58.000000 dumpulator-0.2.4/src/minidump/streams/MiscInfoStream.py
--rw-r--r--   0 runner    (1001) docker     (122)     8440 2023-05-06 15:05:58.000000 dumpulator-0.2.4/src/minidump/streams/ModuleListStream.py
--rw-r--r--   0 runner    (1001) docker     (122)      109 2023-05-06 15:05:58.000000 dumpulator-0.2.4/src/minidump/streams/ProcessVmCountersStream.py
--rw-r--r--   0 runner    (1001) docker     (122)    14530 2023-05-06 15:05:58.000000 dumpulator-0.2.4/src/minidump/streams/SystemInfoStream.py
--rw-r--r--   0 runner    (1001) docker     (122)       94 2023-05-06 15:05:58.000000 dumpulator-0.2.4/src/minidump/streams/SystemMemoryInfoStream.py
--rw-r--r--   0 runner    (1001) docker     (122)     2834 2023-05-06 15:05:58.000000 dumpulator-0.2.4/src/minidump/streams/ThreadExListStream.py
--rw-r--r--   0 runner    (1001) docker     (122)     6506 2023-05-06 15:05:58.000000 dumpulator-0.2.4/src/minidump/streams/ThreadInfoListStream.py
--rw-r--r--   0 runner    (1001) docker     (122)     3308 2023-05-06 15:05:58.000000 dumpulator-0.2.4/src/minidump/streams/ThreadListStream.py
--rw-r--r--   0 runner    (1001) docker     (122)       99 2023-05-06 15:05:58.000000 dumpulator-0.2.4/src/minidump/streams/TokenStream.py
--rw-r--r--   0 runner    (1001) docker     (122)     4906 2023-05-06 15:05:58.000000 dumpulator-0.2.4/src/minidump/streams/UnloadedModuleListStream.py
--rw-r--r--   0 runner    (1001) docker     (122)     3153 2023-05-06 15:05:58.000000 dumpulator-0.2.4/src/minidump/streams/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 15:05:59.511441 dumpulator-0.2.4/src/minidump/utils/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-06 15:05:58.000000 dumpulator-0.2.4/src/minidump/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    11347 2023-05-06 15:05:58.000000 dumpulator-0.2.4/src/minidump/utils/createminidump.py
--rw-r--r--   0 runner    (1001) docker     (122)     6644 2023-05-06 15:05:58.000000 dumpulator-0.2.4/src/minidump/utils/privileges.py
--rw-r--r--   0 runner    (1001) docker     (122)     7333 2023-05-06 15:05:58.000000 dumpulator-0.2.4/src/minidump/utils/privileges_types.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 15:05:59.511441 dumpulator-0.2.4/src/minidump/utils/winapi/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-06 15:05:58.000000 dumpulator-0.2.4/src/minidump/utils/winapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    23531 2023-05-06 15:05:58.000000 dumpulator-0.2.4/src/minidump/utils/winapi/defines.py
--rw-r--r--   0 runner    (1001) docker     (122)     6286 2023-05-06 15:05:58.000000 dumpulator-0.2.4/src/minidump/utils/winapi/kernel32.py
--rw-r--r--   0 runner    (1001) docker     (122)     2398 2023-05-06 15:05:58.000000 dumpulator-0.2.4/src/minidump/utils/winapi/psapi.py
--rw-r--r--   0 runner    (1001) docker     (122)     3768 2023-05-06 15:05:58.000000 dumpulator-0.2.4/src/minidump/utils/winapi/version.py
--rw-r--r--   0 runner    (1001) docker     (122)     6137 2023-05-06 15:05:58.000000 dumpulator-0.2.4/src/minidump/win_datatypes.py
--rw-r--r--   0 runner    (1001) docker     (122)     9188 2023-05-06 15:05:58.000000 dumpulator-0.2.4/src/minidump/writer.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 14:08:28.569607 dumpulator-0.2.5/
+-rw-r--r--   0 runner    (1001) docker     (122)     1359 2023-05-22 14:08:26.000000 dumpulator-0.2.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)    10847 2023-05-22 14:08:28.569607 dumpulator-0.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    10480 2023-05-22 14:08:26.000000 dumpulator-0.2.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)      206 2023-05-22 14:08:26.000000 dumpulator-0.2.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)      802 2023-05-22 14:08:28.569607 dumpulator-0.2.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1588 2023-05-22 14:08:26.000000 dumpulator-0.2.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 14:08:28.561607 dumpulator-0.2.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 14:08:28.565607 dumpulator-0.2.5/src/dumpulator/
+-rw-r--r--   0 runner    (1001) docker     (122)      116 2023-05-22 14:08:26.000000 dumpulator-0.2.5/src/dumpulator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    21634 2023-05-22 14:08:26.000000 dumpulator-0.2.5/src/dumpulator/details.py
+-rw-r--r--   0 runner    (1001) docker     (122)    79009 2023-05-22 14:08:26.000000 dumpulator-0.2.5/src/dumpulator/dumpulator.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10865 2023-05-22 14:08:26.000000 dumpulator-0.2.5/src/dumpulator/handles.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17629 2023-05-22 14:08:26.000000 dumpulator-0.2.5/src/dumpulator/memory.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5442 2023-05-22 14:08:26.000000 dumpulator-0.2.5/src/dumpulator/modules.py
+-rw-r--r--   0 runner    (1001) docker     (122)    21591 2023-05-22 14:08:26.000000 dumpulator-0.2.5/src/dumpulator/native.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3924 2023-05-22 14:08:26.000000 dumpulator-0.2.5/src/dumpulator/ntdevices.py
+-rw-r--r--   0 runner    (1001) docker     (122)   123193 2023-05-22 14:08:26.000000 dumpulator-0.2.5/src/dumpulator/ntenums.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13633 2023-05-22 14:08:26.000000 dumpulator-0.2.5/src/dumpulator/ntprimitives.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3826 2023-05-22 14:08:26.000000 dumpulator-0.2.5/src/dumpulator/ntstructs.py
+-rw-r--r--   0 runner    (1001) docker     (122)   235707 2023-05-22 14:08:26.000000 dumpulator-0.2.5/src/dumpulator/ntsyscalls.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 14:08:28.565607 dumpulator-0.2.5/src/dumpulator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    10847 2023-05-22 14:08:28.000000 dumpulator-0.2.5/src/dumpulator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2301 2023-05-22 14:08:28.000000 dumpulator-0.2.5/src/dumpulator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-22 14:08:28.000000 dumpulator-0.2.5/src/dumpulator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       48 2023-05-22 14:08:28.000000 dumpulator-0.2.5/src/dumpulator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       20 2023-05-22 14:08:28.000000 dumpulator-0.2.5/src/dumpulator.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 14:08:28.565607 dumpulator-0.2.5/src/minidump/
+-rw-r--r--   0 runner    (1001) docker     (122)     3269 2023-05-22 14:08:26.000000 dumpulator-0.2.5/src/minidump/__amain__.py
+-rw-r--r--   0 runner    (1001) docker     (122)       17 2023-05-22 14:08:26.000000 dumpulator-0.2.5/src/minidump/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3501 2023-05-22 14:08:26.000000 dumpulator-0.2.5/src/minidump/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      132 2023-05-22 14:08:26.000000 dumpulator-0.2.5/src/minidump/_version.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9689 2023-05-22 14:08:26.000000 dumpulator-0.2.5/src/minidump/aminidumpfile.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11501 2023-05-22 14:08:26.000000 dumpulator-0.2.5/src/minidump/aminidumpreader.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9452 2023-05-22 14:08:26.000000 dumpulator-0.2.5/src/minidump/common_structs.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2387 2023-05-22 14:08:26.000000 dumpulator-0.2.5/src/minidump/constants.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2349 2023-05-22 14:08:26.000000 dumpulator-0.2.5/src/minidump/directory.py
+-rw-r--r--   0 runner    (1001) docker     (122)      293 2023-05-22 14:08:26.000000 dumpulator-0.2.5/src/minidump/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2828 2023-05-22 14:08:26.000000 dumpulator-0.2.5/src/minidump/header.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9818 2023-05-22 14:08:26.000000 dumpulator-0.2.5/src/minidump/minidumpfile.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11724 2023-05-22 14:08:26.000000 dumpulator-0.2.5/src/minidump/minidumpreader.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5238 2023-05-22 14:08:26.000000 dumpulator-0.2.5/src/minidump/minidumpshell.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 14:08:28.569607 dumpulator-0.2.5/src/minidump/streams/
+-rw-r--r--   0 runner    (1001) docker     (122)      599 2023-05-22 14:08:26.000000 dumpulator-0.2.5/src/minidump/streams/CommentStreamA.py
+-rw-r--r--   0 runner    (1001) docker     (122)      627 2023-05-22 14:08:26.000000 dumpulator-0.2.5/src/minidump/streams/CommentStreamW.py
+-rw-r--r--   0 runner    (1001) docker     (122)    25274 2023-05-22 14:08:26.000000 dumpulator-0.2.5/src/minidump/streams/ContextStream.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11428 2023-05-22 14:08:26.000000 dumpulator-0.2.5/src/minidump/streams/ExceptionStream.py
+-rw-r--r--   0 runner    (1001) docker     (122)      975 2023-05-22 14:08:26.000000 dumpulator-0.2.5/src/minidump/streams/FunctionTableStream.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8898 2023-05-22 14:08:26.000000 dumpulator-0.2.5/src/minidump/streams/HandleDataStream.py
+-rw-r--r--   0 runner    (1001) docker     (122)      682 2023-05-22 14:08:26.000000 dumpulator-0.2.5/src/minidump/streams/HandleOperationListStream.py
+-rw-r--r--   0 runner    (1001) docker     (122)       86 2023-05-22 14:08:26.000000 dumpulator-0.2.5/src/minidump/streams/JavaScriptDataStream.py
+-rw-r--r--   0 runner    (1001) docker     (122)      549 2023-05-22 14:08:26.000000 dumpulator-0.2.5/src/minidump/streams/LastReservedStream.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3211 2023-05-22 14:08:26.000000 dumpulator-0.2.5/src/minidump/streams/Memory64ListStream.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12503 2023-05-22 14:08:26.000000 dumpulator-0.2.5/src/minidump/streams/MemoryInfoListStream.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3252 2023-05-22 14:08:26.000000 dumpulator-0.2.5/src/minidump/streams/MemoryListStream.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6684 2023-05-22 14:08:26.000000 dumpulator-0.2.5/src/minidump/streams/MiscInfoStream.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8440 2023-05-22 14:08:26.000000 dumpulator-0.2.5/src/minidump/streams/ModuleListStream.py
+-rw-r--r--   0 runner    (1001) docker     (122)      109 2023-05-22 14:08:26.000000 dumpulator-0.2.5/src/minidump/streams/ProcessVmCountersStream.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14530 2023-05-22 14:08:26.000000 dumpulator-0.2.5/src/minidump/streams/SystemInfoStream.py
+-rw-r--r--   0 runner    (1001) docker     (122)       94 2023-05-22 14:08:26.000000 dumpulator-0.2.5/src/minidump/streams/SystemMemoryInfoStream.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2834 2023-05-22 14:08:26.000000 dumpulator-0.2.5/src/minidump/streams/ThreadExListStream.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6506 2023-05-22 14:08:26.000000 dumpulator-0.2.5/src/minidump/streams/ThreadInfoListStream.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3308 2023-05-22 14:08:26.000000 dumpulator-0.2.5/src/minidump/streams/ThreadListStream.py
+-rw-r--r--   0 runner    (1001) docker     (122)       99 2023-05-22 14:08:26.000000 dumpulator-0.2.5/src/minidump/streams/TokenStream.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4906 2023-05-22 14:08:26.000000 dumpulator-0.2.5/src/minidump/streams/UnloadedModuleListStream.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3153 2023-05-22 14:08:26.000000 dumpulator-0.2.5/src/minidump/streams/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 14:08:28.569607 dumpulator-0.2.5/src/minidump/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-22 14:08:26.000000 dumpulator-0.2.5/src/minidump/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11347 2023-05-22 14:08:26.000000 dumpulator-0.2.5/src/minidump/utils/createminidump.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6644 2023-05-22 14:08:26.000000 dumpulator-0.2.5/src/minidump/utils/privileges.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7333 2023-05-22 14:08:26.000000 dumpulator-0.2.5/src/minidump/utils/privileges_types.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 14:08:28.569607 dumpulator-0.2.5/src/minidump/utils/winapi/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-22 14:08:26.000000 dumpulator-0.2.5/src/minidump/utils/winapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    23531 2023-05-22 14:08:26.000000 dumpulator-0.2.5/src/minidump/utils/winapi/defines.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6286 2023-05-22 14:08:26.000000 dumpulator-0.2.5/src/minidump/utils/winapi/kernel32.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2398 2023-05-22 14:08:26.000000 dumpulator-0.2.5/src/minidump/utils/winapi/psapi.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3768 2023-05-22 14:08:26.000000 dumpulator-0.2.5/src/minidump/utils/winapi/version.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6137 2023-05-22 14:08:26.000000 dumpulator-0.2.5/src/minidump/win_datatypes.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9188 2023-05-22 14:08:26.000000 dumpulator-0.2.5/src/minidump/writer.py
```

### Comparing `dumpulator-0.2.4/LICENSE` & `dumpulator-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `dumpulator-0.2.4/PKG-INFO` & `dumpulator-0.2.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dumpulator
-Version: 0.2.4
+Version: 0.2.5
 Summary: An easy-to-use library for emulating code in minidump files.
 Home-page: https://github.com/mrexodia/dumpulator
 Author: Duncan Ogilvie
 Author-email: dumpulator@mrexodia.re
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/mrexodia/dumpulator/issues
 Platform: UNKNOWN
@@ -19,17 +19,22 @@
 
 **Note: This is a work-in-progress prototype, please treat it as such. Pull requests are welcome! You can get your feet wet with [good first issues](https://github.com/mrexodia/dumpulator/issues?q=is%3Aissue+is%3Aopen+label%3A%22good+first+issue%22)**
 
 An easy-to-use library for emulating code in minidump files. Here are some links to posts/videos using dumpulator:
 
 - Introduction video with [OALabs](https://oalabs.openanalysis.net): [Dumpulator - Using Binary Emulation To Automate Reverse Engineering](https://youtu.be/4Pfu98Xx9Yo)
 - [Emulating malware with Dumpulator](https://rioasmara.com/2022/07/23/emulating-malware-with-dumpulator/)
-- [Emotet x64 Stack Strings Config Emulation | OALABS Research](https://research.openanalysis.net/emotet/emulation/config/dumpulator/malware/2022/05/19/emotet_x64_emulation.html)
+- [Emotet x64 Stack Strings Config Emulation | OALabs Research](https://research.openanalysis.net/emotet/emulation/config/dumpulator/malware/2022/05/19/emotet_x64_emulation.html)
 - [Native function and Assembly Code Invocation](https://research.checkpoint.com/2022/native-function-and-assembly-code-invocation/)
 - [Guloader string decryption (VEH)](https://research.openanalysis.net/guloader/emulation/dumpulator/veh/exceptions/2023/01/15/dumpulator-veh.html)
+- [Rhadamanthys | OALabs Research](https://research.openanalysis.net/rhadamanthys/config/ida/shifted%20pointers/peb/_list_entry/_ldr_data_table_entry/2023/01/19/rhadamanthys.html)
+- [\[Case study\] Decrypt strings using Dumpulator](https://kienmanowar.wordpress.com/2023/05/22/case-study-decrypt-strings-using-dumpulator/)
+
+<sub>Feel free to send a pull request to add your article here!</sub>
+
 
 ## Examples
 
 ### Calling a function
 
 The example below opens `StringEncryptionFun_x64.dmp` (download a copy [here](https://github.com/mrexodia/dumpulator/releases/download/v0.0.1/StringEncryptionFun_x64.dmp)), allocates some memory and calls the decryption function at `0x140001000` to decrypt the string at `0x140017000`:
```

### Comparing `dumpulator-0.2.4/README.md` & `dumpulator-0.2.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -2,17 +2,22 @@
 
 **Note: This is a work-in-progress prototype, please treat it as such. Pull requests are welcome! You can get your feet wet with [good first issues](https://github.com/mrexodia/dumpulator/issues?q=is%3Aissue+is%3Aopen+label%3A%22good+first+issue%22)**
 
 An easy-to-use library for emulating code in minidump files. Here are some links to posts/videos using dumpulator:
 
 - Introduction video with [OALabs](https://oalabs.openanalysis.net): [Dumpulator - Using Binary Emulation To Automate Reverse Engineering](https://youtu.be/4Pfu98Xx9Yo)
 - [Emulating malware with Dumpulator](https://rioasmara.com/2022/07/23/emulating-malware-with-dumpulator/)
-- [Emotet x64 Stack Strings Config Emulation | OALABS Research](https://research.openanalysis.net/emotet/emulation/config/dumpulator/malware/2022/05/19/emotet_x64_emulation.html)
+- [Emotet x64 Stack Strings Config Emulation | OALabs Research](https://research.openanalysis.net/emotet/emulation/config/dumpulator/malware/2022/05/19/emotet_x64_emulation.html)
 - [Native function and Assembly Code Invocation](https://research.checkpoint.com/2022/native-function-and-assembly-code-invocation/)
 - [Guloader string decryption (VEH)](https://research.openanalysis.net/guloader/emulation/dumpulator/veh/exceptions/2023/01/15/dumpulator-veh.html)
+- [Rhadamanthys | OALabs Research](https://research.openanalysis.net/rhadamanthys/config/ida/shifted%20pointers/peb/_list_entry/_ldr_data_table_entry/2023/01/19/rhadamanthys.html)
+- [\[Case study\] Decrypt strings using Dumpulator](https://kienmanowar.wordpress.com/2023/05/22/case-study-decrypt-strings-using-dumpulator/)
+
+<sub>Feel free to send a pull request to add your article here!</sub>
+
 
 ## Examples
 
 ### Calling a function
 
 The example below opens `StringEncryptionFun_x64.dmp` (download a copy [here](https://github.com/mrexodia/dumpulator/releases/download/v0.0.1/StringEncryptionFun_x64.dmp)), allocates some memory and calls the decryption function at `0x140001000` to decrypt the string at `0x140017000`:
```

### Comparing `dumpulator-0.2.4/setup.cfg` & `dumpulator-0.2.5/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = dumpulator
-version = v0.2.4
+version = v0.2.5
 author = Duncan Ogilvie
 author_email = dumpulator@mrexodia.re
 description = An easy-to-use library for emulating code in minidump files.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/mrexodia/dumpulator
 project_urls =
```

### Comparing `dumpulator-0.2.4/setup.py` & `dumpulator-0.2.5/setup.py`

 * *Files identical despite different names*

### Comparing `dumpulator-0.2.4/src/dumpulator/details.py` & `dumpulator-0.2.5/src/dumpulator/details.py`

 * *Files identical despite different names*

### Comparing `dumpulator-0.2.4/src/dumpulator/dumpulator.py` & `dumpulator-0.2.5/src/dumpulator/dumpulator.py`

 * *Files identical despite different names*

### Comparing `dumpulator-0.2.4/src/dumpulator/handles.py` & `dumpulator-0.2.5/src/dumpulator/handles.py`

 * *Files identical despite different names*

### Comparing `dumpulator-0.2.4/src/dumpulator/memory.py` & `dumpulator-0.2.5/src/dumpulator/memory.py`

 * *Files 5% similar despite different names*

```diff
@@ -177,15 +177,15 @@
                     diff = aligned_base - info.base
                     info.base = aligned_base
                     info.region_size -= diff
                 if info.region_size >= size:
                     return info.base
         return None
 
-    def reserve(self, start: int, size: int, protect: MemoryProtect, memory_type: MemoryType = MemoryType.MEM_PRIVATE, info: Any = None) -> None:
+    def reserve(self, start: int, size: int, protect: MemoryProtect, memory_type: MemoryType = MemoryType.MEM_PRIVATE, info: Any = None) -> MemoryRegion:
         assert isinstance(protect, MemoryProtect)
         assert isinstance(memory_type, MemoryType)
         assert size > 0 and self.align_page(size) == size
         assert self.align_allocation(start) == start
         region = MemoryRegion(start, size, protect, memory_type, info)
         if region.start < self._minimum or region.end > self._maximum:
             raise KeyError(f"Requested region {region} is out of bounds")
@@ -199,14 +199,15 @@
         index = bisect.bisect_right(self._regions, region)
         if index == 0:
             check_overlaps(index)
         else:
             check_overlaps(index - 1)
             check_overlaps(index)
         self._regions.insert(index, region)
+        return region
 
     def _decommit_region(self, parent_region: MemoryRegion, decommit_region: MemoryRegion):
         assert decommit_region in parent_region
         release_start = None
         release_count = 0
         for page in decommit_region.pages():
             if page in self._committed:
@@ -223,27 +224,50 @@
 
         if release_count > 0:
             self._page_manager.decommit(release_start, release_count * PAGE_SIZE)
             for i in range(release_count):
                 del self._committed[release_start + i * PAGE_SIZE]
                 parent_region.commit_count -= 1
 
-    def release(self, start: int) -> None:
+    def release(self, start: int, size: int = 0) -> None:
         assert self.align_allocation(start) == start
+        assert self.align_allocation(size) == size
 
-        parent_region = self.find_region(start)
-        if parent_region is None:
+        parent = self.find_region(start)
+        if parent is None:
             raise KeyError(f"Could not find parent for {hex(start)}")
-        if parent_region.start != start:
-            raise KeyError(f"You can only release the whole parent region")
 
-        self._decommit_region(parent_region, parent_region)
+        if size == 0:
+            size = parent.size
+        if start + size > parent.start + parent.size:
+            raise KeyError(f"You can only release part of the parent region")
+
+        decommit = MemoryRegion(start, size)
+        self._decommit_region(parent, decommit)
+        self._regions.remove(parent)
+
+        before = MemoryRegion(parent.start, decommit.start - parent.start)
+        after = MemoryRegion(decommit.end, parent.end - decommit.end)
+
+        if parent.size == decommit.size:
+            # Make sure the whole region was freed
+            assert parent.commit_count == 0
+
+        if before.size > 0:
+            before = self.reserve(before.start, before.size, parent.protect, parent.type, parent.info)
+            for page in before.pages():
+                if page in self._committed:
+                    before.commit_count += 1
+        if after.size > 0:
+            after = self.reserve(after.start, after.size, parent.protect, parent.type, parent.info)
+            for page in after.pages():
+                if page in self._committed:
+                    after.commit_count += 1
 
-        assert parent_region.commit_count == 0
-        self._regions.remove(parent_region)
+        assert before.commit_count + after.commit_count == parent.commit_count
 
     def commit(self, start: int, size: int, protect: MemoryProtect = MemoryProtect.UNDEFINED) -> None:
         assert isinstance(protect, MemoryProtect)
         assert size > 0 and self.align_page(size) == size
         assert self.containing_page(start) == start
         region = MemoryRegion(start, size)
         parent_region = self.find_region(region)
```

### Comparing `dumpulator-0.2.4/src/dumpulator/modules.py` & `dumpulator-0.2.5/src/dumpulator/modules.py`

 * *Files identical despite different names*

### Comparing `dumpulator-0.2.4/src/dumpulator/native.py` & `dumpulator-0.2.5/src/dumpulator/native.py`

 * *Files identical despite different names*

### Comparing `dumpulator-0.2.4/src/dumpulator/ntdevices.py` & `dumpulator-0.2.5/src/dumpulator/ntdevices.py`

 * *Files identical despite different names*

### Comparing `dumpulator-0.2.4/src/dumpulator/ntenums.py` & `dumpulator-0.2.5/src/dumpulator/ntenums.py`

 * *Files identical despite different names*

### Comparing `dumpulator-0.2.4/src/dumpulator/ntprimitives.py` & `dumpulator-0.2.5/src/dumpulator/ntprimitives.py`

 * *Files identical despite different names*

### Comparing `dumpulator-0.2.4/src/dumpulator/ntstructs.py` & `dumpulator-0.2.5/src/dumpulator/ntstructs.py`

 * *Files identical despite different names*

### Comparing `dumpulator-0.2.4/src/dumpulator/ntsyscalls.py` & `dumpulator-0.2.5/src/dumpulator/ntsyscalls.py`

 * *Files 0% similar despite different names*

```diff
@@ -1816,19 +1816,18 @@
                         RegionSize: Annotated[P[SIZE_T], SAL("_Inout_")],
                         FreeType: Annotated[ULONG, SAL("_In_")]
                         ):
     base = BaseAddress.read_ptr()
     size = RegionSize.read_ptr()
     if FreeType == MEM_RELEASE:
         print(f"release {hex(base)}[{hex(size)}]")
-        assert size == 0
         region = dp.memory.find_region(base)
         if region is None:
             return STATUS_MEMORY_NOT_ALLOCATED
-        dp.memory.release(base)
+        dp.memory.release(base, size)
         return STATUS_SUCCESS
     elif FreeType == MEM_DECOMMIT:
         print(f"decommit {hex(base)}[{hex(size)}]")
         region = dp.memory.find_region(base)
         if region is None:
             return STATUS_MEMORY_NOT_ALLOCATED
         dp.memory.decommit(base, size)
```

### Comparing `dumpulator-0.2.4/src/dumpulator.egg-info/PKG-INFO` & `dumpulator-0.2.5/src/dumpulator.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dumpulator
-Version: 0.2.4
+Version: 0.2.5
 Summary: An easy-to-use library for emulating code in minidump files.
 Home-page: https://github.com/mrexodia/dumpulator
 Author: Duncan Ogilvie
 Author-email: dumpulator@mrexodia.re
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/mrexodia/dumpulator/issues
 Platform: UNKNOWN
@@ -19,17 +19,22 @@
 
 **Note: This is a work-in-progress prototype, please treat it as such. Pull requests are welcome! You can get your feet wet with [good first issues](https://github.com/mrexodia/dumpulator/issues?q=is%3Aissue+is%3Aopen+label%3A%22good+first+issue%22)**
 
 An easy-to-use library for emulating code in minidump files. Here are some links to posts/videos using dumpulator:
 
 - Introduction video with [OALabs](https://oalabs.openanalysis.net): [Dumpulator - Using Binary Emulation To Automate Reverse Engineering](https://youtu.be/4Pfu98Xx9Yo)
 - [Emulating malware with Dumpulator](https://rioasmara.com/2022/07/23/emulating-malware-with-dumpulator/)
-- [Emotet x64 Stack Strings Config Emulation | OALABS Research](https://research.openanalysis.net/emotet/emulation/config/dumpulator/malware/2022/05/19/emotet_x64_emulation.html)
+- [Emotet x64 Stack Strings Config Emulation | OALabs Research](https://research.openanalysis.net/emotet/emulation/config/dumpulator/malware/2022/05/19/emotet_x64_emulation.html)
 - [Native function and Assembly Code Invocation](https://research.checkpoint.com/2022/native-function-and-assembly-code-invocation/)
 - [Guloader string decryption (VEH)](https://research.openanalysis.net/guloader/emulation/dumpulator/veh/exceptions/2023/01/15/dumpulator-veh.html)
+- [Rhadamanthys | OALabs Research](https://research.openanalysis.net/rhadamanthys/config/ida/shifted%20pointers/peb/_list_entry/_ldr_data_table_entry/2023/01/19/rhadamanthys.html)
+- [\[Case study\] Decrypt strings using Dumpulator](https://kienmanowar.wordpress.com/2023/05/22/case-study-decrypt-strings-using-dumpulator/)
+
+<sub>Feel free to send a pull request to add your article here!</sub>
+
 
 ## Examples
 
 ### Calling a function
 
 The example below opens `StringEncryptionFun_x64.dmp` (download a copy [here](https://github.com/mrexodia/dumpulator/releases/download/v0.0.1/StringEncryptionFun_x64.dmp)), allocates some memory and calls the decryption function at `0x140001000` to decrypt the string at `0x140017000`:
```

### Comparing `dumpulator-0.2.4/src/dumpulator.egg-info/SOURCES.txt` & `dumpulator-0.2.5/src/dumpulator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dumpulator-0.2.4/src/minidump/__amain__.py` & `dumpulator-0.2.5/src/minidump/__amain__.py`

 * *Files identical despite different names*

### Comparing `dumpulator-0.2.4/src/minidump/__main__.py` & `dumpulator-0.2.5/src/minidump/__main__.py`

 * *Files identical despite different names*

### Comparing `dumpulator-0.2.4/src/minidump/aminidumpfile.py` & `dumpulator-0.2.5/src/minidump/aminidumpfile.py`

 * *Files identical despite different names*

### Comparing `dumpulator-0.2.4/src/minidump/aminidumpreader.py` & `dumpulator-0.2.5/src/minidump/aminidumpreader.py`

 * *Files identical despite different names*

### Comparing `dumpulator-0.2.4/src/minidump/common_structs.py` & `dumpulator-0.2.5/src/minidump/common_structs.py`

 * *Files identical despite different names*

### Comparing `dumpulator-0.2.4/src/minidump/constants.py` & `dumpulator-0.2.5/src/minidump/constants.py`

 * *Files identical despite different names*

### Comparing `dumpulator-0.2.4/src/minidump/directory.py` & `dumpulator-0.2.5/src/minidump/directory.py`

 * *Files identical despite different names*

### Comparing `dumpulator-0.2.4/src/minidump/header.py` & `dumpulator-0.2.5/src/minidump/header.py`

 * *Files identical despite different names*

### Comparing `dumpulator-0.2.4/src/minidump/minidumpfile.py` & `dumpulator-0.2.5/src/minidump/minidumpfile.py`

 * *Files identical despite different names*

### Comparing `dumpulator-0.2.4/src/minidump/minidumpreader.py` & `dumpulator-0.2.5/src/minidump/minidumpreader.py`

 * *Files identical despite different names*

### Comparing `dumpulator-0.2.4/src/minidump/minidumpshell.py` & `dumpulator-0.2.5/src/minidump/minidumpshell.py`

 * *Files identical despite different names*

### Comparing `dumpulator-0.2.4/src/minidump/streams/CommentStreamA.py` & `dumpulator-0.2.5/src/minidump/streams/CommentStreamA.py`

 * *Files identical despite different names*

### Comparing `dumpulator-0.2.4/src/minidump/streams/CommentStreamW.py` & `dumpulator-0.2.5/src/minidump/streams/CommentStreamW.py`

 * *Files identical despite different names*

### Comparing `dumpulator-0.2.4/src/minidump/streams/ContextStream.py` & `dumpulator-0.2.5/src/minidump/streams/ContextStream.py`

 * *Files identical despite different names*

### Comparing `dumpulator-0.2.4/src/minidump/streams/ExceptionStream.py` & `dumpulator-0.2.5/src/minidump/streams/ExceptionStream.py`

 * *Files identical despite different names*

### Comparing `dumpulator-0.2.4/src/minidump/streams/FunctionTableStream.py` & `dumpulator-0.2.5/src/minidump/streams/FunctionTableStream.py`

 * *Files identical despite different names*

### Comparing `dumpulator-0.2.4/src/minidump/streams/HandleDataStream.py` & `dumpulator-0.2.5/src/minidump/streams/HandleDataStream.py`

 * *Files identical despite different names*

### Comparing `dumpulator-0.2.4/src/minidump/streams/HandleOperationListStream.py` & `dumpulator-0.2.5/src/minidump/streams/HandleOperationListStream.py`

 * *Files identical despite different names*

### Comparing `dumpulator-0.2.4/src/minidump/streams/LastReservedStream.py` & `dumpulator-0.2.5/src/minidump/streams/LastReservedStream.py`

 * *Files identical despite different names*

### Comparing `dumpulator-0.2.4/src/minidump/streams/Memory64ListStream.py` & `dumpulator-0.2.5/src/minidump/streams/Memory64ListStream.py`

 * *Files identical despite different names*

### Comparing `dumpulator-0.2.4/src/minidump/streams/MemoryInfoListStream.py` & `dumpulator-0.2.5/src/minidump/streams/MemoryInfoListStream.py`

 * *Files identical despite different names*

### Comparing `dumpulator-0.2.4/src/minidump/streams/MemoryListStream.py` & `dumpulator-0.2.5/src/minidump/streams/MemoryListStream.py`

 * *Files identical despite different names*

### Comparing `dumpulator-0.2.4/src/minidump/streams/MiscInfoStream.py` & `dumpulator-0.2.5/src/minidump/streams/MiscInfoStream.py`

 * *Files identical despite different names*

### Comparing `dumpulator-0.2.4/src/minidump/streams/ModuleListStream.py` & `dumpulator-0.2.5/src/minidump/streams/ModuleListStream.py`

 * *Files identical despite different names*

### Comparing `dumpulator-0.2.4/src/minidump/streams/SystemInfoStream.py` & `dumpulator-0.2.5/src/minidump/streams/SystemInfoStream.py`

 * *Files identical despite different names*

### Comparing `dumpulator-0.2.4/src/minidump/streams/ThreadExListStream.py` & `dumpulator-0.2.5/src/minidump/streams/ThreadExListStream.py`

 * *Files identical despite different names*

### Comparing `dumpulator-0.2.4/src/minidump/streams/ThreadInfoListStream.py` & `dumpulator-0.2.5/src/minidump/streams/ThreadInfoListStream.py`

 * *Files identical despite different names*

### Comparing `dumpulator-0.2.4/src/minidump/streams/ThreadListStream.py` & `dumpulator-0.2.5/src/minidump/streams/ThreadListStream.py`

 * *Files identical despite different names*

### Comparing `dumpulator-0.2.4/src/minidump/streams/UnloadedModuleListStream.py` & `dumpulator-0.2.5/src/minidump/streams/UnloadedModuleListStream.py`

 * *Files identical despite different names*

### Comparing `dumpulator-0.2.4/src/minidump/streams/__init__.py` & `dumpulator-0.2.5/src/minidump/streams/__init__.py`

 * *Files identical despite different names*

### Comparing `dumpulator-0.2.4/src/minidump/utils/createminidump.py` & `dumpulator-0.2.5/src/minidump/utils/createminidump.py`

 * *Files identical despite different names*

### Comparing `dumpulator-0.2.4/src/minidump/utils/privileges.py` & `dumpulator-0.2.5/src/minidump/utils/privileges.py`

 * *Files identical despite different names*

### Comparing `dumpulator-0.2.4/src/minidump/utils/privileges_types.py` & `dumpulator-0.2.5/src/minidump/utils/privileges_types.py`

 * *Files identical despite different names*

### Comparing `dumpulator-0.2.4/src/minidump/utils/winapi/defines.py` & `dumpulator-0.2.5/src/minidump/utils/winapi/defines.py`

 * *Files identical despite different names*

### Comparing `dumpulator-0.2.4/src/minidump/utils/winapi/kernel32.py` & `dumpulator-0.2.5/src/minidump/utils/winapi/kernel32.py`

 * *Files identical despite different names*

### Comparing `dumpulator-0.2.4/src/minidump/utils/winapi/psapi.py` & `dumpulator-0.2.5/src/minidump/utils/winapi/psapi.py`

 * *Files identical despite different names*

### Comparing `dumpulator-0.2.4/src/minidump/utils/winapi/version.py` & `dumpulator-0.2.5/src/minidump/utils/winapi/version.py`

 * *Files identical despite different names*

### Comparing `dumpulator-0.2.4/src/minidump/win_datatypes.py` & `dumpulator-0.2.5/src/minidump/win_datatypes.py`

 * *Files identical despite different names*

### Comparing `dumpulator-0.2.4/src/minidump/writer.py` & `dumpulator-0.2.5/src/minidump/writer.py`

 * *Files identical despite different names*

