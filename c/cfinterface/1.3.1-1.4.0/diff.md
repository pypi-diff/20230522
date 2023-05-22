# Comparing `tmp/cfinterface-1.3.1.tar.gz` & `tmp/cfinterface-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cfinterface-1.3.1.tar", last modified: Tue Mar 28 00:20:40 2023, max compression
+gzip compressed data, was "cfinterface-1.4.0.tar", last modified: Mon May 22 15:33:03 2023, max compression
```

## Comparing `cfinterface-1.3.1.tar` & `cfinterface-1.4.0.tar`

### file list

```diff
@@ -1,120 +1,120 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 00:20:40.263221 cfinterface-1.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-03-28 00:19:31.000000 cfinterface-1.3.1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     2815 2023-03-28 00:20:40.263221 cfinterface-1.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-03-28 00:19:31.000000 cfinterface-1.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 00:20:40.251221 cfinterface-1.3.1/cfinterface/
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-03-28 00:19:31.000000 cfinterface-1.3.1/cfinterface/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 00:20:40.255221 cfinterface-1.3.1/cfinterface/_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 00:19:31.000000 cfinterface-1.3.1/cfinterface/_utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 00:20:40.255221 cfinterface-1.3.1/cfinterface/adapters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 00:19:31.000000 cfinterface-1.3.1/cfinterface/adapters/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 00:20:40.255221 cfinterface-1.3.1/cfinterface/adapters/components/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 00:19:31.000000 cfinterface-1.3.1/cfinterface/adapters/components/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 00:20:40.255221 cfinterface-1.3.1/cfinterface/adapters/components/line/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 00:19:31.000000 cfinterface-1.3.1/cfinterface/adapters/components/line/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5674 2023-03-28 00:19:31.000000 cfinterface-1.3.1/cfinterface/adapters/components/line/repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     8344 2023-03-28 00:19:31.000000 cfinterface-1.3.1/cfinterface/adapters/components/repository.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 00:20:40.255221 cfinterface-1.3.1/cfinterface/adapters/reading/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 00:19:31.000000 cfinterface-1.3.1/cfinterface/adapters/reading/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2593 2023-03-28 00:19:31.000000 cfinterface-1.3.1/cfinterface/adapters/reading/repository.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 00:20:40.255221 cfinterface-1.3.1/cfinterface/adapters/writing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 00:19:31.000000 cfinterface-1.3.1/cfinterface/adapters/writing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2429 2023-03-28 00:19:31.000000 cfinterface-1.3.1/cfinterface/adapters/writing/repository.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 00:20:40.255221 cfinterface-1.3.1/cfinterface/components/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 00:19:31.000000 cfinterface-1.3.1/cfinterface/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3191 2023-03-28 00:19:31.000000 cfinterface-1.3.1/cfinterface/components/block.py
--rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-03-28 00:19:31.000000 cfinterface-1.3.1/cfinterface/components/datetimefield.py
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-03-28 00:19:31.000000 cfinterface-1.3.1/cfinterface/components/defaultblock.py
--rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-03-28 00:19:31.000000 cfinterface-1.3.1/cfinterface/components/defaultregister.py
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-03-28 00:19:31.000000 cfinterface-1.3.1/cfinterface/components/defaultsection.py
--rw-r--r--   0 runner    (1001) docker     (123)     3201 2023-03-28 00:19:31.000000 cfinterface-1.3.1/cfinterface/components/field.py
--rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-03-28 00:19:31.000000 cfinterface-1.3.1/cfinterface/components/floatfield.py
--rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-03-28 00:19:31.000000 cfinterface-1.3.1/cfinterface/components/integerfield.py
--rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-03-28 00:19:31.000000 cfinterface-1.3.1/cfinterface/components/line.py
--rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-03-28 00:19:31.000000 cfinterface-1.3.1/cfinterface/components/literalfield.py
--rw-r--r--   0 runner    (1001) docker     (123)     4639 2023-03-28 00:19:31.000000 cfinterface-1.3.1/cfinterface/components/register.py
--rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-03-28 00:19:31.000000 cfinterface-1.3.1/cfinterface/components/section.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 00:20:40.255221 cfinterface-1.3.1/cfinterface/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 00:19:31.000000 cfinterface-1.3.1/cfinterface/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3139 2023-03-28 00:19:31.000000 cfinterface-1.3.1/cfinterface/data/blockdata.py
--rw-r--r--   0 runner    (1001) docker     (123)     3262 2023-03-28 00:19:31.000000 cfinterface-1.3.1/cfinterface/data/registerdata.py
--rw-r--r--   0 runner    (1001) docker     (123)     3221 2023-03-28 00:19:31.000000 cfinterface-1.3.1/cfinterface/data/sectiondata.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 00:20:40.255221 cfinterface-1.3.1/cfinterface/files/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 00:19:31.000000 cfinterface-1.3.1/cfinterface/files/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3079 2023-03-28 00:19:31.000000 cfinterface-1.3.1/cfinterface/files/blockfile.py
--rw-r--r--   0 runner    (1001) docker     (123)     3985 2023-03-28 00:19:31.000000 cfinterface-1.3.1/cfinterface/files/registerfile.py
--rw-r--r--   0 runner    (1001) docker     (123)     3143 2023-03-28 00:19:31.000000 cfinterface-1.3.1/cfinterface/files/sectionfile.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 00:19:31.000000 cfinterface-1.3.1/cfinterface/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 00:20:40.259221 cfinterface-1.3.1/cfinterface/reading/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 00:19:31.000000 cfinterface-1.3.1/cfinterface/reading/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3616 2023-03-28 00:19:31.000000 cfinterface-1.3.1/cfinterface/reading/blockreading.py
--rw-r--r--   0 runner    (1001) docker     (123)     3829 2023-03-28 00:19:31.000000 cfinterface-1.3.1/cfinterface/reading/registerreading.py
--rw-r--r--   0 runner    (1001) docker     (123)     3175 2023-03-28 00:19:31.000000 cfinterface-1.3.1/cfinterface/reading/sectionreading.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 00:20:40.259221 cfinterface-1.3.1/cfinterface/writing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 00:19:31.000000 cfinterface-1.3.1/cfinterface/writing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-03-28 00:19:31.000000 cfinterface-1.3.1/cfinterface/writing/blockwriting.py
--rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-03-28 00:19:31.000000 cfinterface-1.3.1/cfinterface/writing/registerwriting.py
--rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-03-28 00:19:31.000000 cfinterface-1.3.1/cfinterface/writing/sectionwriting.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 00:20:40.255221 cfinterface-1.3.1/cfinterface.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2815 2023-03-28 00:20:40.000000 cfinterface-1.3.1/cfinterface.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3177 2023-03-28 00:20:40.000000 cfinterface-1.3.1/cfinterface.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-28 00:20:40.000000 cfinterface-1.3.1/cfinterface.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-03-28 00:20:40.000000 cfinterface-1.3.1/cfinterface.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-03-28 00:20:40.000000 cfinterface-1.3.1/cfinterface.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 00:20:40.259221 cfinterface-1.3.1/examples/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 00:19:31.000000 cfinterface-1.3.1/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-28 00:20:40.263221 cfinterface-1.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-03-28 00:19:31.000000 cfinterface-1.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 00:20:40.259221 cfinterface-1.3.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 00:19:31.000000 cfinterface-1.3.1/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 00:20:40.259221 cfinterface-1.3.1/tests/adapters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 00:19:31.000000 cfinterface-1.3.1/tests/adapters/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 00:20:40.259221 cfinterface-1.3.1/tests/adapters/components/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 00:19:31.000000 cfinterface-1.3.1/tests/adapters/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 00:19:31.000000 cfinterface-1.3.1/tests/adapters/components/test_blockrepository.py
--rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-03-28 00:19:31.000000 cfinterface-1.3.1/tests/adapters/components/test_linerepository.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 00:19:31.000000 cfinterface-1.3.1/tests/adapters/components/test_registerrepository.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 00:19:31.000000 cfinterface-1.3.1/tests/adapters/components/test_sectionrepository.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 00:20:40.259221 cfinterface-1.3.1/tests/adapters/reading/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 00:19:31.000000 cfinterface-1.3.1/tests/adapters/reading/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 00:19:31.000000 cfinterface-1.3.1/tests/adapters/reading/test_readingrepository.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 00:20:40.259221 cfinterface-1.3.1/tests/adapters/writing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 00:19:31.000000 cfinterface-1.3.1/tests/adapters/writing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 00:19:31.000000 cfinterface-1.3.1/tests/adapters/writing/test_writingrepository.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 00:20:40.259221 cfinterface-1.3.1/tests/components/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 00:19:31.000000 cfinterface-1.3.1/tests/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4315 2023-03-28 00:19:31.000000 cfinterface-1.3.1/tests/components/test_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     2518 2023-03-28 00:19:31.000000 cfinterface-1.3.1/tests/components/test_datetimefield.py
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-03-28 00:19:31.000000 cfinterface-1.3.1/tests/components/test_defaultblock.py
--rw-r--r--   0 runner    (1001) docker     (123)      942 2023-03-28 00:19:31.000000 cfinterface-1.3.1/tests/components/test_defaultregister.py
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-03-28 00:19:31.000000 cfinterface-1.3.1/tests/components/test_defaultsection.py
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-03-28 00:19:31.000000 cfinterface-1.3.1/tests/components/test_field.py
--rw-r--r--   0 runner    (1001) docker     (123)     2089 2023-03-28 00:19:31.000000 cfinterface-1.3.1/tests/components/test_floatfield.py
--rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-03-28 00:19:31.000000 cfinterface-1.3.1/tests/components/test_integerfield.py
--rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-03-28 00:19:31.000000 cfinterface-1.3.1/tests/components/test_line.py
--rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-03-28 00:19:31.000000 cfinterface-1.3.1/tests/components/test_literalfield.py
--rw-r--r--   0 runner    (1001) docker     (123)     3878 2023-03-28 00:19:31.000000 cfinterface-1.3.1/tests/components/test_register.py
--rw-r--r--   0 runner    (1001) docker     (123)     3829 2023-03-28 00:19:31.000000 cfinterface-1.3.1/tests/components/test_section.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 00:20:40.259221 cfinterface-1.3.1/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 00:19:31.000000 cfinterface-1.3.1/tests/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-03-28 00:19:31.000000 cfinterface-1.3.1/tests/data/test_blockdata.py
--rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-03-28 00:19:31.000000 cfinterface-1.3.1/tests/data/test_registerdata.py
--rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-03-28 00:19:31.000000 cfinterface-1.3.1/tests/data/test_sectiondata.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 00:20:40.259221 cfinterface-1.3.1/tests/files/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 00:19:31.000000 cfinterface-1.3.1/tests/files/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3634 2023-03-28 00:19:31.000000 cfinterface-1.3.1/tests/files/test_blockfile.py
--rw-r--r--   0 runner    (1001) docker     (123)     3315 2023-03-28 00:19:31.000000 cfinterface-1.3.1/tests/files/test_registerfile.py
--rw-r--r--   0 runner    (1001) docker     (123)     3413 2023-03-28 00:19:31.000000 cfinterface-1.3.1/tests/files/test_sectionfile.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 00:20:40.263221 cfinterface-1.3.1/tests/mocks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 00:19:31.000000 cfinterface-1.3.1/tests/mocks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3589 2023-03-28 00:19:31.000000 cfinterface-1.3.1/tests/mocks/mock_open.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 00:20:40.263221 cfinterface-1.3.1/tests/reading/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 00:19:31.000000 cfinterface-1.3.1/tests/reading/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-03-28 00:19:31.000000 cfinterface-1.3.1/tests/reading/test_blockreading.py
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-03-28 00:19:31.000000 cfinterface-1.3.1/tests/reading/test_registerreading.py
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-03-28 00:19:31.000000 cfinterface-1.3.1/tests/reading/test_sectionreading.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 00:20:40.263221 cfinterface-1.3.1/tests/writing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 00:19:31.000000 cfinterface-1.3.1/tests/writing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-03-28 00:19:31.000000 cfinterface-1.3.1/tests/writing/test_blockwriting.py
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-03-28 00:19:31.000000 cfinterface-1.3.1/tests/writing/test_registerwriting.py
--rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-03-28 00:19:31.000000 cfinterface-1.3.1/tests/writing/test_sectionwriting.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:33:03.212464 cfinterface-1.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-22 15:31:50.000000 cfinterface-1.4.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2815 2023-05-22 15:33:03.212464 cfinterface-1.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-05-22 15:31:50.000000 cfinterface-1.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:33:03.204464 cfinterface-1.4.0/cfinterface/
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-05-22 15:31:50.000000 cfinterface-1.4.0/cfinterface/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:33:03.204464 cfinterface-1.4.0/cfinterface/_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 15:31:50.000000 cfinterface-1.4.0/cfinterface/_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:33:03.204464 cfinterface-1.4.0/cfinterface/adapters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 15:31:50.000000 cfinterface-1.4.0/cfinterface/adapters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:33:03.204464 cfinterface-1.4.0/cfinterface/adapters/components/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 15:31:50.000000 cfinterface-1.4.0/cfinterface/adapters/components/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:33:03.204464 cfinterface-1.4.0/cfinterface/adapters/components/line/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 15:31:50.000000 cfinterface-1.4.0/cfinterface/adapters/components/line/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5674 2023-05-22 15:31:50.000000 cfinterface-1.4.0/cfinterface/adapters/components/line/repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8344 2023-05-22 15:31:50.000000 cfinterface-1.4.0/cfinterface/adapters/components/repository.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:33:03.204464 cfinterface-1.4.0/cfinterface/adapters/reading/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 15:31:50.000000 cfinterface-1.4.0/cfinterface/adapters/reading/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3078 2023-05-22 15:31:50.000000 cfinterface-1.4.0/cfinterface/adapters/reading/repository.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:33:03.204464 cfinterface-1.4.0/cfinterface/adapters/writing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 15:31:50.000000 cfinterface-1.4.0/cfinterface/adapters/writing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2644 2023-05-22 15:31:50.000000 cfinterface-1.4.0/cfinterface/adapters/writing/repository.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:33:03.204464 cfinterface-1.4.0/cfinterface/components/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 15:31:50.000000 cfinterface-1.4.0/cfinterface/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3191 2023-05-22 15:31:50.000000 cfinterface-1.4.0/cfinterface/components/block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-05-22 15:31:50.000000 cfinterface-1.4.0/cfinterface/components/datetimefield.py
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-05-22 15:31:50.000000 cfinterface-1.4.0/cfinterface/components/defaultblock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-05-22 15:31:50.000000 cfinterface-1.4.0/cfinterface/components/defaultregister.py
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-05-22 15:31:50.000000 cfinterface-1.4.0/cfinterface/components/defaultsection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3201 2023-05-22 15:31:50.000000 cfinterface-1.4.0/cfinterface/components/field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-05-22 15:31:50.000000 cfinterface-1.4.0/cfinterface/components/floatfield.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-05-22 15:31:50.000000 cfinterface-1.4.0/cfinterface/components/integerfield.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-05-22 15:31:50.000000 cfinterface-1.4.0/cfinterface/components/line.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-05-22 15:31:50.000000 cfinterface-1.4.0/cfinterface/components/literalfield.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4639 2023-05-22 15:31:50.000000 cfinterface-1.4.0/cfinterface/components/register.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-05-22 15:31:50.000000 cfinterface-1.4.0/cfinterface/components/section.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:33:03.204464 cfinterface-1.4.0/cfinterface/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 15:31:50.000000 cfinterface-1.4.0/cfinterface/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3139 2023-05-22 15:31:50.000000 cfinterface-1.4.0/cfinterface/data/blockdata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3262 2023-05-22 15:31:50.000000 cfinterface-1.4.0/cfinterface/data/registerdata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3221 2023-05-22 15:31:50.000000 cfinterface-1.4.0/cfinterface/data/sectiondata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:33:03.208464 cfinterface-1.4.0/cfinterface/files/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 15:31:50.000000 cfinterface-1.4.0/cfinterface/files/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2949 2023-05-22 15:31:50.000000 cfinterface-1.4.0/cfinterface/files/blockfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3844 2023-05-22 15:31:50.000000 cfinterface-1.4.0/cfinterface/files/registerfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3022 2023-05-22 15:31:50.000000 cfinterface-1.4.0/cfinterface/files/sectionfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 15:31:50.000000 cfinterface-1.4.0/cfinterface/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:33:03.208464 cfinterface-1.4.0/cfinterface/reading/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 15:31:50.000000 cfinterface-1.4.0/cfinterface/reading/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3530 2023-05-22 15:31:50.000000 cfinterface-1.4.0/cfinterface/reading/blockreading.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3766 2023-05-22 15:31:50.000000 cfinterface-1.4.0/cfinterface/reading/registerreading.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3112 2023-05-22 15:31:50.000000 cfinterface-1.4.0/cfinterface/reading/sectionreading.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:33:03.208464 cfinterface-1.4.0/cfinterface/writing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 15:31:50.000000 cfinterface-1.4.0/cfinterface/writing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-05-22 15:31:50.000000 cfinterface-1.4.0/cfinterface/writing/blockwriting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-05-22 15:31:50.000000 cfinterface-1.4.0/cfinterface/writing/registerwriting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-05-22 15:31:50.000000 cfinterface-1.4.0/cfinterface/writing/sectionwriting.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:33:03.204464 cfinterface-1.4.0/cfinterface.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2815 2023-05-22 15:33:03.000000 cfinterface-1.4.0/cfinterface.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3177 2023-05-22 15:33:03.000000 cfinterface-1.4.0/cfinterface.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 15:33:03.000000 cfinterface-1.4.0/cfinterface.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-22 15:33:03.000000 cfinterface-1.4.0/cfinterface.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-22 15:33:03.000000 cfinterface-1.4.0/cfinterface.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:33:03.208464 cfinterface-1.4.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 15:31:50.000000 cfinterface-1.4.0/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 15:33:03.212464 cfinterface-1.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-05-22 15:31:50.000000 cfinterface-1.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:33:03.208464 cfinterface-1.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 15:31:50.000000 cfinterface-1.4.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:33:03.208464 cfinterface-1.4.0/tests/adapters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 15:31:50.000000 cfinterface-1.4.0/tests/adapters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:33:03.208464 cfinterface-1.4.0/tests/adapters/components/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 15:31:50.000000 cfinterface-1.4.0/tests/adapters/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 15:31:50.000000 cfinterface-1.4.0/tests/adapters/components/test_blockrepository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-05-22 15:31:50.000000 cfinterface-1.4.0/tests/adapters/components/test_linerepository.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 15:31:50.000000 cfinterface-1.4.0/tests/adapters/components/test_registerrepository.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 15:31:50.000000 cfinterface-1.4.0/tests/adapters/components/test_sectionrepository.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:33:03.208464 cfinterface-1.4.0/tests/adapters/reading/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 15:31:50.000000 cfinterface-1.4.0/tests/adapters/reading/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 15:31:50.000000 cfinterface-1.4.0/tests/adapters/reading/test_readingrepository.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:33:03.208464 cfinterface-1.4.0/tests/adapters/writing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 15:31:50.000000 cfinterface-1.4.0/tests/adapters/writing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 15:31:50.000000 cfinterface-1.4.0/tests/adapters/writing/test_writingrepository.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:33:03.208464 cfinterface-1.4.0/tests/components/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 15:31:50.000000 cfinterface-1.4.0/tests/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4315 2023-05-22 15:31:50.000000 cfinterface-1.4.0/tests/components/test_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2518 2023-05-22 15:31:50.000000 cfinterface-1.4.0/tests/components/test_datetimefield.py
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-05-22 15:31:50.000000 cfinterface-1.4.0/tests/components/test_defaultblock.py
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-05-22 15:31:50.000000 cfinterface-1.4.0/tests/components/test_defaultregister.py
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-05-22 15:31:50.000000 cfinterface-1.4.0/tests/components/test_defaultsection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-05-22 15:31:50.000000 cfinterface-1.4.0/tests/components/test_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2089 2023-05-22 15:31:50.000000 cfinterface-1.4.0/tests/components/test_floatfield.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-05-22 15:31:50.000000 cfinterface-1.4.0/tests/components/test_integerfield.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-05-22 15:31:50.000000 cfinterface-1.4.0/tests/components/test_line.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-05-22 15:31:50.000000 cfinterface-1.4.0/tests/components/test_literalfield.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3878 2023-05-22 15:31:50.000000 cfinterface-1.4.0/tests/components/test_register.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3829 2023-05-22 15:31:50.000000 cfinterface-1.4.0/tests/components/test_section.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:33:03.208464 cfinterface-1.4.0/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 15:31:50.000000 cfinterface-1.4.0/tests/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-05-22 15:31:50.000000 cfinterface-1.4.0/tests/data/test_blockdata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-05-22 15:31:50.000000 cfinterface-1.4.0/tests/data/test_registerdata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-05-22 15:31:50.000000 cfinterface-1.4.0/tests/data/test_sectiondata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:33:03.212464 cfinterface-1.4.0/tests/files/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 15:31:50.000000 cfinterface-1.4.0/tests/files/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4254 2023-05-22 15:31:50.000000 cfinterface-1.4.0/tests/files/test_blockfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3905 2023-05-22 15:31:50.000000 cfinterface-1.4.0/tests/files/test_registerfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3939 2023-05-22 15:31:50.000000 cfinterface-1.4.0/tests/files/test_sectionfile.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:33:03.212464 cfinterface-1.4.0/tests/mocks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 15:31:50.000000 cfinterface-1.4.0/tests/mocks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3589 2023-05-22 15:31:50.000000 cfinterface-1.4.0/tests/mocks/mock_open.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:33:03.212464 cfinterface-1.4.0/tests/reading/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 15:31:50.000000 cfinterface-1.4.0/tests/reading/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2238 2023-05-22 15:31:50.000000 cfinterface-1.4.0/tests/reading/test_blockreading.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-05-22 15:31:50.000000 cfinterface-1.4.0/tests/reading/test_registerreading.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-05-22 15:31:50.000000 cfinterface-1.4.0/tests/reading/test_sectionreading.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:33:03.212464 cfinterface-1.4.0/tests/writing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 15:31:50.000000 cfinterface-1.4.0/tests/writing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-05-22 15:31:50.000000 cfinterface-1.4.0/tests/writing/test_blockwriting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-05-22 15:31:50.000000 cfinterface-1.4.0/tests/writing/test_registerwriting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-05-22 15:31:50.000000 cfinterface-1.4.0/tests/writing/test_sectionwriting.py
```

### Comparing `cfinterface-1.3.1/LICENSE.md` & `cfinterface-1.4.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `cfinterface-1.3.1/PKG-INFO` & `cfinterface-1.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cfinterface
-Version: 1.3.1
+Version: 1.4.0
 Summary: Interface for handling custom formatted files
 Home-page: https://github.com/rjmalves/cfi
 Author: Rogerio Alves
 Author-email: rogerioalves.ee@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `cfinterface-1.3.1/README.md` & `cfinterface-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `cfinterface-1.3.1/cfinterface/adapters/components/line/repository.py` & `cfinterface-1.4.0/cfinterface/adapters/components/line/repository.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.3.1/cfinterface/adapters/components/repository.py` & `cfinterface-1.4.0/cfinterface/adapters/components/repository.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.3.1/cfinterface/adapters/reading/repository.py` & `cfinterface-1.4.0/cfinterface/adapters/reading/repository.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 from typing import IO, BinaryIO, TextIO, Union, Type, Dict
 from abc import ABC, abstractmethod
+from io import BytesIO, StringIO
 
 
 class Repository(ABC):
-    def __init__(self, path: str, *args) -> None:
-        self._path = path
+    def __init__(
+        self, content: Union[str, bytes], wrap_io: bool = False, *args
+    ) -> None:
+        self._content = content
+        self._wrap_io = wrap_io
 
     def __enter__(self) -> "Repository":
         return self
 
     def __exit__(self, *args):
         pass
 
@@ -28,20 +32,26 @@
     @property
     @abstractmethod
     def file(self) -> IO:
         raise NotImplementedError
 
 
 class BinaryRepository(Repository):
-    def __init__(self, path: str, *args) -> None:
-        super().__init__(path)
+    def __init__(
+        self, content: Union[str, bytes], wrap_io: bool = False, *args
+    ) -> None:
+        super().__init__(content, wrap_io)
         self._filepointer: BinaryIO = None  # type: ignore
 
     def __enter__(self):
-        self._filepointer = open(self._path, "rb")
+        self._filepointer = (
+            BytesIO(self._content)
+            if self._wrap_io
+            else open(self._content, "rb")
+        )
         return super().__enter__()
 
     def __exit__(self, *args):
         super().__exit__(*args)
         self._filepointer.close()
 
     def read(self, n: int) -> bytes:
@@ -58,21 +68,31 @@
 
     @property
     def file(self) -> BinaryIO:
         return self._filepointer
 
 
 class TextualRepository(Repository):
-    def __init__(self, path: str, encoding: str) -> None:
-        super().__init__(path)
+    def __init__(
+        self,
+        content: str,
+        wrap_io: bool = False,
+        encoding: str = "utf-8",
+        *args
+    ) -> None:
+        super().__init__(content, wrap_io)
         self._encoding = encoding
         self._filepointer: TextIO = None  # type: ignore
 
     def __enter__(self):
-        self._filepointer = open(self._path, "r", encoding=self._encoding)
+        self._filepointer = (
+            StringIO(self._content)
+            if self._wrap_io
+            else open(self._content, "r", encoding=self._encoding)
+        )
         return super().__enter__()
 
     def __exit__(self, *args):
         super().__exit__(*args)
         self._filepointer.close()
 
     def read(self, n: int) -> str:
```

### Comparing `cfinterface-1.3.1/cfinterface/adapters/writing/repository.py` & `cfinterface-1.4.0/cfinterface/adapters/writing/repository.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from typing import IO, BinaryIO, TextIO, Union, Dict, Type
 from abc import ABC, abstractmethod
 
 
 class Repository(ABC):
-    def __init__(self, path: str, *args) -> None:
-        self._path = path
+    def __init__(self, to: Union[str, IO], *args) -> None:
+        self._to = to
+        self._wrap_io = isinstance(to, str)
 
     def __enter__(self) -> "Repository":
         return self
 
     def __exit__(self, *args):
         pass
 
@@ -30,20 +31,21 @@
 
 class BinaryRepository(Repository):
     def __init__(self, path: str, *args) -> None:
         super().__init__(path)
         self._filepointer: BinaryIO = None  # type: ignore
 
     def __enter__(self):
-        self._filepointer = open(self._path, "wb")
+        self._filepointer = open(self._to, "wb") if self._wrap_io else self._to
         return super().__enter__()
 
     def __exit__(self, *args):
         super().__exit__(*args)
-        self._filepointer.close()
+        if self._wrap_io:
+            self._filepointer.close()
 
     def write(self, data: Union[str, bytes]):
         """
         Writes an amount of information to a file.
 
         :param data: The bytes to be written
         :type data: str | bytes
@@ -59,20 +61,25 @@
 class TextualRepository(Repository):
     def __init__(self, path: str, encoding: str) -> None:
         super().__init__(path)
         self._filepointer: TextIO = None  # type: ignore
         self._encoding = encoding
 
     def __enter__(self):
-        self._filepointer = open(self._path, "w", encoding=self._encoding)
+        self._filepointer = (
+            open(self._to, "w", encoding=self._encoding)
+            if self._wrap_io
+            else self._to
+        )
         return super().__enter__()
 
     def __exit__(self, *args):
         super().__exit__(*args)
-        self._filepointer.close()
+        if self._wrap_io:
+            self._filepointer.close()
 
     def write(self, data: Union[str, bytes]):
         """
         Writes an amount of information to a file.
 
         :param data: The data to be written
         :type data: str | bytes
```

### Comparing `cfinterface-1.3.1/cfinterface/components/block.py` & `cfinterface-1.4.0/cfinterface/components/block.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.3.1/cfinterface/components/datetimefield.py` & `cfinterface-1.4.0/cfinterface/components/datetimefield.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.3.1/cfinterface/components/defaultblock.py` & `cfinterface-1.4.0/cfinterface/components/defaultblock.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.3.1/cfinterface/components/defaultregister.py` & `cfinterface-1.4.0/cfinterface/components/defaultregister.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.3.1/cfinterface/components/defaultsection.py` & `cfinterface-1.4.0/cfinterface/components/defaultsection.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.3.1/cfinterface/components/field.py` & `cfinterface-1.4.0/cfinterface/components/field.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.3.1/cfinterface/components/floatfield.py` & `cfinterface-1.4.0/cfinterface/components/floatfield.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.3.1/cfinterface/components/integerfield.py` & `cfinterface-1.4.0/cfinterface/components/integerfield.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.3.1/cfinterface/components/line.py` & `cfinterface-1.4.0/cfinterface/components/line.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.3.1/cfinterface/components/literalfield.py` & `cfinterface-1.4.0/cfinterface/components/literalfield.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.3.1/cfinterface/components/register.py` & `cfinterface-1.4.0/cfinterface/components/register.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.3.1/cfinterface/components/section.py` & `cfinterface-1.4.0/cfinterface/components/section.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.3.1/cfinterface/data/blockdata.py` & `cfinterface-1.4.0/cfinterface/data/blockdata.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.3.1/cfinterface/data/registerdata.py` & `cfinterface-1.4.0/cfinterface/data/registerdata.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.3.1/cfinterface/data/sectiondata.py` & `cfinterface-1.4.0/cfinterface/data/sectiondata.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.3.1/cfinterface/files/blockfile.py` & `cfinterface-1.4.0/cfinterface/files/blockfile.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import List, Dict, Type, Optional
+from typing import List, Dict, Type, Optional, Union, IO
 
 from cfinterface.components.block import Block
 from cfinterface.components.defaultblock import DefaultBlock
 from cfinterface.data.blockdata import BlockData
 from cfinterface.reading.blockreading import BlockReading
 from cfinterface.writing.blockwriting import BlockWriting
 
@@ -30,39 +30,34 @@
     def __eq__(self, o: object) -> bool:
         if not isinstance(o, BlockFile):
             return False
         bf: BlockFile = o
         return self.data == bf.data
 
     @classmethod
-    def read(cls, directory: str, filename: str = "", *args, **kwargs):
+    def read(cls, content: Union[str, bytes], *args, **kwargs):
         """
-        Reads the blockfile data from a given file in disk.
+        Reads the blockfile data from either a given file or a buffer.
 
-        :param filename: The file name in disk
-        :type filename: str
-        :param directory: The directory where the file is
-        :type directory: str
+        :param content: The file name in disk or the file contents themselves
+        :type content: str | bytes
         """
         reader = BlockReading(cls.BLOCKS, cls.STORAGE)
-        return cls(
-            reader.read(filename, directory, cls.ENCODING, *args, **kwargs)
-        )
+        return cls(reader.read(content, cls.ENCODING, *args, **kwargs))
 
-    def write(self, directory: str, filename: str = "", *args, **kwargs):
+    def write(self, to: Union[str, IO], *args, **kwargs):
         """
-        Write the blockfile data to a given file in disk.
+        Write the blockfile data to a given file or buffer.
 
-        :param filename: The file name in disk
-        :type filename: str
-        :param directory: The directory where the file will be
-        :type directory: str
+        :param to: The writing destination, being a string for writing
+            to a file or the IO buffer
+        :type to: str | IO
         """
         writer = BlockWriting(self.__data, self.__storage)
-        writer.write(filename, directory, self.__encoding, *args, **kwargs)
+        writer.write(to, self.__encoding, *args, **kwargs)
 
     @property
     def data(self) -> BlockData:
         return self.__data
 
     @classmethod
     def set_version(cls, v: str):
```

### Comparing `cfinterface-1.3.1/cfinterface/files/registerfile.py` & `cfinterface-1.4.0/cfinterface/files/registerfile.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import List, Dict, Type, Optional
+from typing import List, Dict, Type, Optional, Union, IO
 import pandas as pd  # type: ignore
 from cfinterface.components.register import Register
 from cfinterface.components.defaultregister import DefaultRegister
 from cfinterface.data.registerdata import RegisterData
 from cfinterface.reading.registerreading import RegisterReading
 from cfinterface.writing.registerwriting import RegisterWriting
 
@@ -49,39 +49,34 @@
             return pd.DataFrame()
         cols = registers[0].custom_properties
         return pd.DataFrame(
             data={c: [getattr(r, c) for r in registers] for c in cols}
         )
 
     @classmethod
-    def read(cls, directory: str, filename: str = "", *args, **kwargs):
+    def read(cls, content: Union[str, bytes], *args, **kwargs):
         """
         Reads the registerfile data from a given file in disk.
 
-        :param filename: The file name in disk
-        :type filename: str
-        :param directory: The directory where the file is
-        :type directory: str
+        :param content: The file name in disk or the file contents themselves
+        :type content: str | bytes
         """
         reader = RegisterReading(cls.REGISTERS, cls.STORAGE, *args, **kwargs)
-        return cls(
-            reader.read(filename, directory, cls.ENCODING, *args, **kwargs)
-        )
+        return cls(reader.read(content, cls.ENCODING, *args, **kwargs))
 
-    def write(self, directory: str, filename: str = "", *args, **kwargs):
+    def write(self, to: Union[str, IO], *args, **kwargs):
         """
-        Write the registerfile data to a given file in disk.
+        Write the registerfile data to a given file or buffer.
 
-        :param filename: The file name in disk
-        :type filename: str
-        :param directory: The directory where the file will be
-        :type directory: str
+        :param to: The writing destination, being a string for writing
+            to a file or the IO buffer
+        :type to: str | IO
         """
         writer = RegisterWriting(self.__data, self.__storage, *args, **kwargs)
-        writer.write(filename, directory, self.__encoding, *args, **kwargs)
+        writer.write(to, self.__encoding, *args, **kwargs)
 
     @property
     def data(self) -> RegisterData:
         return self.__data
 
     @classmethod
     def set_version(cls, v: str):
```

### Comparing `cfinterface-1.3.1/cfinterface/files/sectionfile.py` & `cfinterface-1.4.0/cfinterface/files/sectionfile.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import List, Dict, Type, Optional
+from typing import List, Dict, Type, Optional, Union, IO
 
 from cfinterface.components.section import Section
 from cfinterface.components.defaultsection import DefaultSection
 from cfinterface.data.sectiondata import SectionData
 from cfinterface.reading.sectionreading import SectionReading
 from cfinterface.writing.sectionwriting import SectionWriting
 
@@ -30,39 +30,34 @@
     def __eq__(self, o: object) -> bool:
         if not isinstance(o, SectionFile):
             return False
         bf: SectionFile = o
         return self.data == bf.data
 
     @classmethod
-    def read(cls, directory: str, filename: str = "", *args, **kwargs):
+    def read(cls, content: Union[str, bytes], *args, **kwargs):
         """
         Reads the sectionfile data from a given file in disk.
 
-        :param filename: The file name in disk
-        :type filename: str
-        :param directory: The directory where the file is
-        :type directory: str
+        :param content: The file name in disk or the file contents themselves
+        :type content: str | bytes
         """
         reader = SectionReading(cls.SECTIONS, cls.STORAGE)
-        return cls(
-            reader.read(filename, directory, cls.ENCODING, *args, **kwargs)
-        )
+        return cls(reader.read(content, cls.ENCODING, *args, **kwargs))
 
-    def write(self, directory: str, filename: str = "", *args, **kwargs):
+    def write(self, to: Union[str, IO], filename: str = "", *args, **kwargs):
         """
-        Write the sectionfile data to a given file in disk.
+        Write the sectionfile data to a given file or buffer.
 
-        :param filename: The file name in disk
-        :type filename: str
-        :param directory: The directory where the file will be
-        :type directory: str
+        :param to: The writing destination, being a string for writing
+            to a file or the IO buffer
+        :type to: str | IO
         """
         writer = SectionWriting(self.__data, self.__storage)
-        writer.write(filename, directory, self.__encoding, *args, **kwargs)
+        writer.write(to, self.__encoding, *args, **kwargs)
 
     @property
     def data(self) -> SectionData:
         return self.__data
 
     @classmethod
     def set_version(cls, v: str):
```

### Comparing `cfinterface-1.3.1/cfinterface/reading/blockreading.py` & `cfinterface-1.4.0/cfinterface/reading/blockreading.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from typing import List, Type, Union
-from os.path import join
+from os.path import isfile
 
 from cfinterface.components.block import Block
 from cfinterface.components.defaultblock import DefaultBlock
 from cfinterface.data.blockdata import BlockData
 
 from cfinterface.adapters.reading.repository import Repository, factory
 
@@ -78,31 +78,30 @@
             blocktype = self.__find_starting_block(line)
             block = blocktype()
             block.read(self.__repository.file, *args, **kwargs)
             self.__data.append(block)
         return self.__data
 
     def read(
-        self, filename: str, directory: str, encoding: str, *args, **kwargs
+        self, content: Union[str, bytes], encoding: str, *args, **kwargs
     ) -> BlockData:
         """
-        Reads a file with a given name in a given directory and
+        Reads a file in a given path and
         extracts the data from the specified blocks.
 
-        :param filename: The name of the file
-        :type filename: str
-        :param directory: The directory where the file is
-        :type directory: str
+        :param content: The file name in disk or the file contents
+        :type content: str | bytes
         :param encoding: The encoding for reading the file
         :type encoding: str
         :return: The data from the blocks found in the file
         :rtype: BlockData
         """
-        filepath = join(directory, filename)
-        self.__repository = factory(self.__storage)(filepath, encoding)
+        self.__repository = factory(self.__storage)(
+            content, not isfile(content), encoding
+        )
         with self.__repository:
             return self.__read_file(*args, **kwargs)
 
     @property
     def data(self) -> BlockData:
         return self.__data
```

### Comparing `cfinterface-1.3.1/cfinterface/reading/registerreading.py` & `cfinterface-1.4.0/cfinterface/reading/registerreading.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from typing import List, Type, Union
-from os.path import join
+from os.path import isfile
 
 from cfinterface.components.register import Register
 from cfinterface.components.defaultregister import DefaultRegister
 from cfinterface.data.registerdata import RegisterData
 
 from cfinterface.adapters.reading.repository import Repository, factory
 
@@ -82,31 +82,30 @@
             register.read(
                 self.__repository.file, self.__storage, *args, **kwargs
             )
             self.__data.append(register)
         return self.__data
 
     def read(
-        self, filename: str, directory: str, encoding: str, *args, **kwargs
+        self, content: Union[str, bytes], encoding: str, *args, **kwargs
     ) -> RegisterData:
         """
         Reads a file with a given name in a given directory and
         extracts the data from the specified registers.
 
-        :param filename: The name of the file
-        :type filename: str
-        :param directory: The directory where the file is
-        :type directory: str
+        :param content: The file name in disk or the file contents
+        :type content: str | bytes
         :param encoding: The encoding for reading the file
         :type encoding: str
         :return: The data from the registers found in the file
         :rtype: RegisterData
         """
-        filepath = join(directory, filename)
-        self.__repository = factory(self.__storage)(filepath, encoding)
+        self.__repository = factory(self.__storage)(
+            content, not isfile(content), encoding
+        )
         with self.__repository:
             return self.__read_file(*args, **kwargs)
 
     @property
     def data(self) -> RegisterData:
         return self.__data
```

### Comparing `cfinterface-1.3.1/cfinterface/reading/sectionreading.py` & `cfinterface-1.4.0/cfinterface/reading/sectionreading.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from typing import List, Type, Union
-from os.path import join
+from os.path import isfile
 
 from cfinterface.components.section import Section
 from cfinterface.components.defaultsection import DefaultSection
 from cfinterface.data.sectiondata import SectionData
 
 from cfinterface.adapters.reading.repository import Repository, factory
 
@@ -65,31 +65,30 @@
             self.__restore_previous_line()
             section = DefaultSection()
             section.read(self.__repository.file, *args, **kwargs)
             self.__data.append(section)
         return self.__data
 
     def read(
-        self, filename: str, directory: str, encoding: str, *args, **kwargs
+        self, content: Union[str, bytes], encoding: str, *args, **kwargs
     ) -> SectionData:
         """
         Reads a file with a given name in a given directory and
         extracts the data from the specified sections.
 
-        :param filename: The name of the file
-        :type filename: str
-        :param directory: The directory where the file is
-        :type directory: str
+        :param content: The file name in disk or the file contents
+        :type content: str | bytes
         :param encoding: The encoding for reading the file
         :type encoding: str
         :return: The data from the sections found in the file
         :rtype: SectionData
         """
-        filepath = join(directory, filename)
-        self.__repository = factory(self.__storage)(filepath, encoding)
+        self.__repository = factory(self.__storage)(
+            content, not isfile(content), encoding
+        )
         with self.__repository:
             return self.__read_file(*args, **kwargs)
 
     @property
     def data(self) -> SectionData:
         return self.__data
```

### Comparing `cfinterface-1.3.1/cfinterface/writing/blockwriting.py` & `cfinterface-1.4.0/cfinterface/writing/blockwriting.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-from os.path import join
-
+from typing import Union, IO
 from cfinterface.data.blockdata import BlockData
 from cfinterface.adapters.writing.repository import (
     Repository,
     factory,
 )
 
 
@@ -22,29 +21,25 @@
         Writes all the blocks from the given BlockData structure
         to the specified file.
 
         """
         for b in self.__data:
             b.write(self.__repository.file, *args, **kwargs)
 
-    def write(
-        self, filename: str, directory: str, encoding: str, *args, **kwargs
-    ):
+    def write(self, to: Union[str, IO], encoding: str, *args, **kwargs):
         """
         Writes a file with a given name in a given directory with
         the data from the BlockData structure.
 
-        :param filename: The name of the file
-        :type filename: str
-        :param directory: The directory where the file will be
-        :type directory: str
+        :param to: The writing destination, being a string for writing
+            to a file or the IO buffer
+        :type to: str | IO
         :param encoding: The encoding for reading the file
         :type encoding: str
         """
-        filepath = join(directory, filename)
-        self.__repository = factory(self.__storage)(filepath, encoding)
+        self.__repository = factory(self.__storage)(to, encoding)
         with self.__repository:
             return self.__write_file(*args, **kwargs)
 
     @property
     def data(self) -> BlockData:
         return self.__data
```

### Comparing `cfinterface-1.3.1/cfinterface/writing/sectionwriting.py` & `cfinterface-1.4.0/cfinterface/writing/sectionwriting.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from os.path import join
+from typing import Union, IO
 
 from cfinterface.data.sectiondata import SectionData
 from cfinterface.adapters.writing.repository import (
     Repository,
     factory,
 )
 
@@ -17,34 +17,29 @@
         self.__storage = storage
         self.__repository: Repository = None  # type: ignore
 
     def __write_file(self, *args, **kwargs):
         """
         Writes all the registers from the given SectionData structure
         to the specified file.
-
         """
         for s in self.__data:
             s.write(self.__repository.file, *args, **kwargs)
 
-    def write(
-        self, filename: str, directory: str, encoding: str, *args, **kwargs
-    ):
+    def write(self, to: Union[str, IO], encoding: str, *args, **kwargs):
         """
-        Writes a file with a given name in a given directory with
-        the data from the SectionData structure.
+        Writes to a file with a given name in a given directory or
+        to a buffer with the data from the SectionData structure.
 
-        :param filename: The name of the file
-        :type filename: str
-        :param directory: The directory where the file will be
-        :type directory: str
+        :param to: The writing destination, being a string for writing
+            to a file or the IO buffer
+        :type to: str | IO
         :param encoding: The encoding for reading the file
         :type encoding: str
         """
-        filepath = join(directory, filename)
-        self.__repository = factory(self.__storage)(filepath, encoding)
+        self.__repository = factory(self.__storage)(to, encoding)
         with self.__repository:
             return self.__write_file(*args, **kwargs)
 
     @property
     def data(self) -> SectionData:
         return self.__data
```

### Comparing `cfinterface-1.3.1/cfinterface.egg-info/PKG-INFO` & `cfinterface-1.4.0/cfinterface.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cfinterface
-Version: 1.3.1
+Version: 1.4.0
 Summary: Interface for handling custom formatted files
 Home-page: https://github.com/rjmalves/cfi
 Author: Rogerio Alves
 Author-email: rogerioalves.ee@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `cfinterface-1.3.1/cfinterface.egg-info/SOURCES.txt` & `cfinterface-1.4.0/cfinterface.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cfinterface-1.3.1/setup.py` & `cfinterface-1.4.0/setup.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.3.1/tests/adapters/components/test_linerepository.py` & `cfinterface-1.4.0/tests/adapters/components/test_linerepository.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.3.1/tests/components/test_block.py` & `cfinterface-1.4.0/tests/components/test_block.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.3.1/tests/components/test_datetimefield.py` & `cfinterface-1.4.0/tests/components/test_datetimefield.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.3.1/tests/components/test_defaultblock.py` & `cfinterface-1.4.0/tests/components/test_defaultblock.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.3.1/tests/components/test_defaultregister.py` & `cfinterface-1.4.0/tests/components/test_defaultregister.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.3.1/tests/components/test_defaultsection.py` & `cfinterface-1.4.0/tests/components/test_defaultsection.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.3.1/tests/components/test_floatfield.py` & `cfinterface-1.4.0/tests/components/test_floatfield.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.3.1/tests/components/test_integerfield.py` & `cfinterface-1.4.0/tests/components/test_integerfield.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.3.1/tests/components/test_line.py` & `cfinterface-1.4.0/tests/components/test_line.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.3.1/tests/components/test_literalfield.py` & `cfinterface-1.4.0/tests/components/test_literalfield.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.3.1/tests/components/test_register.py` & `cfinterface-1.4.0/tests/components/test_register.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.3.1/tests/components/test_section.py` & `cfinterface-1.4.0/tests/components/test_section.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.3.1/tests/data/test_blockdata.py` & `cfinterface-1.4.0/tests/data/test_blockdata.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.3.1/tests/data/test_registerdata.py` & `cfinterface-1.4.0/tests/data/test_registerdata.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.3.1/tests/data/test_sectiondata.py` & `cfinterface-1.4.0/tests/data/test_sectiondata.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.3.1/tests/files/test_blockfile.py` & `cfinterface-1.4.0/tests/files/test_blockfile.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import IO, List
 
 from cfinterface.components.block import Block
 from cfinterface.data.blockdata import BlockData
 from cfinterface.files.blockfile import BlockFile
 
 from tests.mocks.mock_open import mock_open
-
+from io import StringIO
 from unittest.mock import MagicMock, patch
 
 
 class DummyBlock(Block):
     BEGIN_PATTERN = "beg"
     END_PATTERN = "end"
 
@@ -95,31 +95,54 @@
     filedata = (
         "\n".join([DummyBlock.BEGIN_PATTERN, data, DummyBlock.END_PATTERN])
         + "\n"
     )
     BlockFile.BLOCKS = [DummyBlock]
     m: MagicMock = mock_open(read_data=filedata)
     with patch("builtins.open", m):
-        f = BlockFile.read("", "")
+        f = BlockFile.read("README.md")
         assert len(f.data) == 2
         assert len(f.data.last.data) == 3
         assert f.data.last.data[1] == data + "\n"
 
 
+def test_blockfile_read_frombuffer():
+    data = "Hello, world!"
+    filedata = (
+        "\n".join([DummyBlock.BEGIN_PATTERN, data, DummyBlock.END_PATTERN])
+        + "\n"
+    )
+    BlockFile.BLOCKS = [DummyBlock]
+    f = BlockFile.read(filedata)
+    assert len(f.data) == 2
+    assert len(f.data.last.data) == 3
+    assert f.data.last.data[1] == data + "\n"
+
+
 def test_blockfile_write():
     data = "Hello, world!"
     bd = BlockData(DummyBlock(data=[data]))
     BlockFile.BLOCKS = [DummyBlock]
     f = BlockFile(bd)
     m: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m):
-        f.write("", "")
+        f.write("")
     m().write.assert_called_once_with(data)
 
 
+def test_blockfile_write_tobuffer():
+    data = "Hello, world!"
+    bd = BlockData(DummyBlock(data=[data]))
+    BlockFile.BLOCKS = [DummyBlock]
+    f = BlockFile(bd)
+    m = StringIO()
+    f.write(m)
+    assert m.getvalue() == data
+
+
 def test_blockfile_set_version():
     assert VersionedBlockFile.BLOCKS[0] == DummyBlockV2
     VersionedBlockFile.set_version("v1")
     assert VersionedBlockFile.BLOCKS[0] == DummyBlock
     VersionedBlockFile.set_version("v1.5")
     assert VersionedBlockFile.BLOCKS[0] == DummyBlock
     VersionedBlockFile.set_version("v2")
```

### Comparing `cfinterface-1.3.1/tests/files/test_registerfile.py` & `cfinterface-1.4.0/tests/files/test_registerfile.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from cfinterface.components.literalfield import LiteralField
 from cfinterface.components.register import Register
 from cfinterface.data.registerdata import RegisterData
 from cfinterface.files.registerfile import RegisterFile
 
 import pandas as pd  # type: ignore
 from tests.mocks.mock_open import mock_open
-
+from io import StringIO
 from unittest.mock import MagicMock, patch
 
 
 class DummyRegister(Register):
     IDENTIFIER = "reg"
     IDENTIFIER_DIGITS = 4
     LINE = Line([LiteralField(13, 4)])
@@ -70,32 +70,51 @@
 
 def test_registerfile_read():
     data = "Hello, world!"
     filedata = DummyRegister.IDENTIFIER + " " + data + "\n"
     RegisterFile.REGISTERS = [DummyRegister]
     m: MagicMock = mock_open(read_data=filedata)
     with patch("builtins.open", m):
-        f = RegisterFile.read("", "")
+        f = RegisterFile.read("README.md")
         assert len(f.data) == 2
         assert f.data.last.data[0] == data
 
 
+def test_registerfile_read_frombuffer():
+    data = "Hello, world!"
+    filedata = DummyRegister.IDENTIFIER + " " + data + "\n"
+    RegisterFile.REGISTERS = [DummyRegister]
+    f = RegisterFile.read(filedata)
+    assert len(f.data) == 2
+    assert f.data.last.data[0] == data
+
+
 def test_registerfile_write():
     data = "Hello, world!"
     bd = RegisterData(DummyRegister(data=[data]))
     RegisterFile.REGISTERS = [DummyRegister]
     f = RegisterFile(bd)
     m: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m):
-        f.write("", "")
+        f.write("")
     m().write.assert_called_once_with(
         DummyRegister.IDENTIFIER + " " + data + "\n"
     )
 
 
+def test_registerfile_write_tobuffer():
+    data = "Hello, world!"
+    bd = RegisterData(DummyRegister(data=[data]))
+    RegisterFile.REGISTERS = [DummyRegister]
+    f = RegisterFile(bd)
+    m = StringIO()
+    f.write(m)
+    m.getvalue() == DummyRegister.IDENTIFIER + " " + data + "\n"
+
+
 def test_registerfile_set_version():
     assert VersionedRegisterFile.REGISTERS[0] == DummyRegisterV2
     VersionedRegisterFile.set_version("v1")
     assert VersionedRegisterFile.REGISTERS[0] == DummyRegister
     VersionedRegisterFile.set_version("v1.5")
     assert VersionedRegisterFile.REGISTERS[0] == DummyRegister
     VersionedRegisterFile.set_version("v2")
```

### Comparing `cfinterface-1.3.1/tests/files/test_sectionfile.py` & `cfinterface-1.4.0/tests/files/test_sectionfile.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import IO, List
 
 from cfinterface.components.section import Section
 from cfinterface.data.sectiondata import SectionData
 from cfinterface.files.sectionfile import SectionFile
 
 from tests.mocks.mock_open import mock_open
-
+from io import StringIO
 from unittest.mock import MagicMock, patch
 
 
 class DummySection(Section):
     def __eq__(self, o: object) -> bool:
         if not isinstance(o, self.__class__):
             return False
@@ -79,31 +79,50 @@
 
 
 def test_sectionfile_read():
     data = "Hello, world!"
     SectionFile.SECTIONS = [DummySection]
     m: MagicMock = mock_open(read_data=data + "\n")
     with patch("builtins.open", m):
-        f = SectionFile.read("", "")
+        f = SectionFile.read("README.md")
         assert len(f.data) == 2
         assert len(f.data.last.data) == 1
         assert f.data.last.data[0] == data + "\n"
 
 
+def test_sectionfile_read_frombuffer():
+    data = "Hello, world!"
+    SectionFile.SECTIONS = [DummySection]
+    f = SectionFile.read(data + "\n")
+    assert len(f.data) == 2
+    assert len(f.data.last.data) == 1
+    assert f.data.last.data[0] == data + "\n"
+
+
 def test_sectionfile_write():
     data = "Hello, world!"
     bd = SectionData(DummySection(data=[data]))
     SectionFile.SECTIONS = [DummySection]
     f = SectionFile(bd)
     m: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m):
-        f.write("", "")
+        f.write("")
     m().write.assert_called_once_with(data)
 
 
+def test_sectionfile_write_tobuffer():
+    data = "Hello, world!"
+    bd = SectionData(DummySection(data=[data]))
+    SectionFile.SECTIONS = [DummySection]
+    f = SectionFile(bd)
+    m = StringIO()
+    f.write(m)
+    m.getvalue() == data
+
+
 def test_sectionfile_set_version():
     assert VersionedSectionFile.SECTIONS[0] == DummySectionV2
     VersionedSectionFile.set_version("v1")
     assert VersionedSectionFile.SECTIONS[0] == DummySection
     VersionedSectionFile.set_version("v1.5")
     assert VersionedSectionFile.SECTIONS[0] == DummySection
     VersionedSectionFile.set_version("v2")
```

### Comparing `cfinterface-1.3.1/tests/mocks/mock_open.py` & `cfinterface-1.4.0/tests/mocks/mock_open.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.3.1/tests/reading/test_blockreading.py` & `cfinterface-1.4.0/tests/reading/test_blockreading.py`

 * *Files 17% similar despite different names*

```diff
@@ -34,28 +34,44 @@
 
 
 def test_blockreading_empty():
     filedata = ""
     br = BlockReading([DummyBlock])
     m: MagicMock = mock_open(read_data=filedata)
     with patch("builtins.open", m):
-        bd = br.read("", "", "utf-8")
+        bd = br.read("README.md", "utf-8")
         assert br.empty
         assert len(bd) == 1
 
 
 def test_blockreading_withdata():
     data = "Hello, world!"
     filedata = (
         "\n".join([DummyBlock.BEGIN_PATTERN, data, DummyBlock.END_PATTERN])
         + "\n"
     )
     br = BlockReading([DummyBlock])
     m: MagicMock = mock_open(read_data=filedata)
     with patch("builtins.open", m):
-        bd = br.read("", "", "utf-8")
+        bd = br.read("README.md", "utf-8")
         assert not br.empty
         dbs = [b for b in bd.of_type(DummyBlock)]
         assert len(dbs) == 1
         assert dbs[0].data[0].strip() == DummyBlock.BEGIN_PATTERN
         assert dbs[0].data[1].strip() == data
         assert dbs[0].data[2].strip() == DummyBlock.END_PATTERN
+
+
+def test_blockreading_withdata_frombuffer():
+    data = "Hello, world!"
+    filedata = (
+        "\n".join([DummyBlock.BEGIN_PATTERN, data, DummyBlock.END_PATTERN])
+        + "\n"
+    )
+    br = BlockReading([DummyBlock])
+    bd = br.read(filedata, "utf-8")
+    assert not br.empty
+    dbs = [b for b in bd.of_type(DummyBlock)]
+    assert len(dbs) == 1
+    assert dbs[0].data[0].strip() == DummyBlock.BEGIN_PATTERN
+    assert dbs[0].data[1].strip() == data
+    assert dbs[0].data[2].strip() == DummyBlock.END_PATTERN
```

### Comparing `cfinterface-1.3.1/tests/reading/test_registerreading.py` & `cfinterface-1.4.0/tests/reading/test_registerreading.py`

 * *Files 13% similar despite different names*

```diff
@@ -15,24 +15,35 @@
 
 
 def test_registerreading_empty():
     filedata = ""
     br = RegisterReading([DummyRegister])
     m: MagicMock = mock_open(read_data=filedata)
     with patch("builtins.open", m):
-        bd = br.read("", "", "utf-8")
+        bd = br.read("README.md", "utf-8")
         assert br.empty
         assert len(bd) == 1
 
 
 def test_registerreading_withdata():
     data = "Hello, world!"
     br = RegisterReading([DummyRegister])
     m: MagicMock = mock_open(
         read_data=DummyRegister.IDENTIFIER + " " + data + "\n"
     )
     with patch("builtins.open", m):
-        bd = br.read("", "", "utf-8")
+        bd = br.read("README.md", "utf-8")
         assert not br.empty
         dbs = [b for b in bd.of_type(DummyRegister)]
         assert len(dbs) == 1
         assert dbs[0].data[0].strip() == data
+
+
+def test_registerreading_withdata_frombuffer():
+    data = "Hello, world!"
+    br = RegisterReading([DummyRegister])
+    m = DummyRegister.IDENTIFIER + " " + data + "\n"
+    bd = br.read(m, "utf-8")
+    assert not br.empty
+    dbs = [b for b in bd.of_type(DummyRegister)]
+    assert len(dbs) == 1
+    assert dbs[0].data[0].strip() == data
```

### Comparing `cfinterface-1.3.1/tests/writing/test_blockwriting.py` & `cfinterface-1.4.0/tests/writing/test_blockwriting.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import IO, List
 
 from cfinterface.components.block import Block
 from cfinterface.data.blockdata import BlockData
 from cfinterface.writing.blockwriting import BlockWriting
 
 from tests.mocks.mock_open import mock_open
-
+from io import StringIO
 from unittest.mock import MagicMock, patch
 
 
 class DummyBlock(Block):
     BEGIN_PATTERN = "beg"
     END_PATTERN = "end"
 
@@ -35,9 +35,18 @@
 
 def test_blockwriting_withdata():
     filedata = "Hello, World!"
     bd = BlockData(DummyBlock(data=filedata))
     bw = BlockWriting(bd)
     m: MagicMock = mock_open(read_data=filedata)
     with patch("builtins.open", m):
-        bw.write("", "", "utf-8")
+        bw.write("./test.txt", "utf-8")
     m().write.assert_called_once_with(filedata)
+
+
+def test_blockwriting_withdata_tobuffer():
+    filedata = "Hello, World!"
+    bd = BlockData(DummyBlock(data=filedata))
+    bw = BlockWriting(bd)
+    m = StringIO("")
+    bw.write(m, "utf-8")
+    assert m.getvalue() == filedata
```

### Comparing `cfinterface-1.3.1/tests/writing/test_registerwriting.py` & `cfinterface-1.4.0/tests/writing/test_registerwriting.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,36 @@
-from typing import IO, List
-
 from cfinterface.components.line import Line
 from cfinterface.components.literalfield import LiteralField
 from cfinterface.components.register import Register
 from cfinterface.data.registerdata import RegisterData
 from cfinterface.writing.registerwriting import RegisterWriting
 
 from tests.mocks.mock_open import mock_open
-
+from io import StringIO
 from unittest.mock import MagicMock, patch
 
 
 class DummyRegister(Register):
     IDENTIFIER = "reg"
     IDENTIFIER_DIGITS = 4
     LINE = Line([LiteralField(13, 4)])
 
 
-def test_blockwriting_withdata():
+def test_registerwriting_withdata():
     filedata = "Hello, World!"
     bd = RegisterData(DummyRegister(data=[filedata]))
     bw = RegisterWriting(bd)
     m: MagicMock = mock_open(read_data=filedata)
     with patch("builtins.open", m):
-        bw.write("", "", "utf-8")
+        bw.write("", "utf-8")
     m().write.assert_called_once_with(
         DummyRegister.IDENTIFIER + " " + filedata + "\n"
     )
+
+
+def test_registerwriting_withdata_tobuffer():
+    filedata = "Hello, World!"
+    bd = RegisterData(DummyRegister(data=[filedata]))
+    bw = RegisterWriting(bd)
+    m = StringIO("")
+    bw.write(m, "utf-8")
+    assert m.getvalue() == (DummyRegister.IDENTIFIER + " " + filedata + "\n")
```

### Comparing `cfinterface-1.3.1/tests/writing/test_sectionwriting.py` & `cfinterface-1.4.0/tests/writing/test_sectionwriting.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import IO, List
 
 from cfinterface.components.section import Section
 from cfinterface.data.sectiondata import SectionData
 from cfinterface.writing.sectionwriting import SectionWriting
 
 from tests.mocks.mock_open import mock_open
-
+from io import StringIO
 from unittest.mock import MagicMock, patch
 
 
 class DummySection(Section):
     def __eq__(self, o: object) -> bool:
         if not isinstance(o, self.__class__):
             return False
@@ -29,9 +29,18 @@
 
 def test_sectionwriting_withdata():
     filedata = "Hello, World!"
     bd = SectionData(DummySection(data=filedata))
     bw = SectionWriting(bd)
     m: MagicMock = mock_open(read_data=filedata)
     with patch("builtins.open", m):
-        bw.write("", "", "utf-8")
+        bw.write("", "utf-8")
     m().write.assert_called_once_with(filedata)
+
+
+def test_sectionwriting_withdata_tobuffer():
+    filedata = "Hello, World!"
+    bd = SectionData(DummySection(data=filedata))
+    bw = SectionWriting(bd)
+    m = StringIO("")
+    bw.write(m, "utf-8")
+    assert m.getvalue() == filedata
```

