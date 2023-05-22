# Comparing `tmp/enebootools-2.0.1.tar.gz` & `tmp/enebootools-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "enebootools-2.0.1.tar", last modified: Thu May 18 09:31:21 2023, max compression
+gzip compressed data, was "enebootools-2.0.2.tar", last modified: Mon May 22 18:38:36 2023, max compression
```

## Comparing `enebootools-2.0.1.tar` & `enebootools-2.0.2.tar`

### file list

```diff
@@ -1,101 +1,101 @@
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-18 09:31:21.633914 enebootools-2.0.1/
--rw-r--r--   0 aulla     (1000) aulla     (1000)      259 2019-12-11 07:08:54.000000 enebootools-2.0.1/AUTHORS
--rw-r--r--   0 aulla     (1000) aulla     (1000)    35146 2019-12-11 07:08:54.000000 enebootools-2.0.1/LICENSE.gplv3
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    19837 2023-05-18 09:31:21.629913 enebootools-2.0.1/PKG-INFO
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    18665 2022-02-08 10:20:48.000000 enebootools-2.0.1/README.rst
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-18 09:31:21.613913 enebootools-2.0.1/enebootools/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     6052 2023-05-18 09:12:28.000000 enebootools-2.0.1/enebootools/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     7116 2020-06-27 08:28:15.000000 enebootools-2.0.1/enebootools/__init__.pyc
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-18 09:31:21.617913 enebootools-2.0.1/enebootools/assembler/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     6326 2023-05-18 09:15:32.000000 enebootools-2.0.1/enebootools/assembler/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     2584 2022-02-08 10:20:48.000000 enebootools-2.0.1/enebootools/assembler/config.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    29859 2023-05-18 09:20:33.000000 enebootools-2.0.1/enebootools/assembler/database.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1325 2022-02-08 10:20:48.000000 enebootools-2.0.1/enebootools/assembler/databasemodels.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1334 2022-03-05 09:43:22.000000 enebootools-2.0.1/enebootools/assembler/featureconfig.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    23182 2023-05-09 13:12:22.000000 enebootools-2.0.1/enebootools/assembler/kobjects.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     2276 2022-02-08 10:20:48.000000 enebootools-2.0.1/enebootools/assembler/mypeewee.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     3124 2022-12-07 11:24:39.000000 enebootools-2.0.1/enebootools/assembler/save_auto.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-18 09:31:21.617913 enebootools-2.0.1/enebootools/autoconfig/
--rw-r--r--   0 aulla     (1000) aulla     (1000)        0 2020-06-21 07:16:10.000000 enebootools-2.0.1/enebootools/autoconfig/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     7521 2022-03-05 21:54:44.000000 enebootools-2.0.1/enebootools/autoconfig/autoconfig.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1955 2022-02-08 10:20:48.000000 enebootools-2.0.1/enebootools/autoconfig/parsers.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-18 09:31:21.617913 enebootools-2.0.1/enebootools/config/
--rw-r--r--   0 aulla     (1000) aulla     (1000)        0 2020-06-21 07:16:10.000000 enebootools-2.0.1/enebootools/config/__init__.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-18 09:31:21.617913 enebootools-2.0.1/enebootools/crypto/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     3002 2022-02-08 10:20:48.000000 enebootools-2.0.1/enebootools/crypto/__init__.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-18 09:31:21.621913 enebootools-2.0.1/enebootools/crypto/certificates/
--rw-r--r--   0 aulla     (1000) aulla     (1000)     2244 2019-12-11 07:08:54.000000 enebootools-2.0.1/enebootools/crypto/certificates/CA_Partners_Gestiweb.crt
--rw-r--r--   0 aulla     (1000) aulla     (1000)     1854 2019-12-11 07:08:54.000000 enebootools-2.0.1/enebootools/crypto/certificates/CA_Test_Partners.crt
--rw-r--r--   0 aulla     (1000) aulla     (1000)     2545 2019-12-11 07:08:54.000000 enebootools-2.0.1/enebootools/crypto/certificates/Eneboo_Open_Source_ERP.crt
--rw-r--r--   0 aulla     (1000) aulla     (1000)     1285 2019-12-11 07:08:54.000000 enebootools-2.0.1/enebootools/crypto/certificates/Partner_Test.crt
--rw-r--r--   0 aulla     (1000) aulla     (1000)      963 2019-12-11 07:08:54.000000 enebootools-2.0.1/enebootools/crypto/certificates/Partner_Test.pem
--rw-r--r--   0 aulla     (1000) aulla     (1000)      884 2019-12-11 07:08:54.000000 enebootools-2.0.1/enebootools/crypto/certificates/README.txt
--rw-rw-r--   0 aulla     (1000) aulla     (1000)        0 2022-02-08 10:20:48.000000 enebootools-2.0.1/enebootools/crypto/certificates/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    27617 2022-09-12 08:13:27.000000 enebootools-2.0.1/enebootools/crypto/main.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-18 09:31:21.621913 enebootools-2.0.1/enebootools/databaseadmin/
--rw-r--r--   0 aulla     (1000) aulla     (1000)        0 2020-06-21 07:16:10.000000 enebootools-2.0.1/enebootools/databaseadmin/__init__.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-18 09:31:21.621913 enebootools-2.0.1/enebootools/databaseadmin/dblayer/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)        0 2022-02-08 10:20:48.000000 enebootools-2.0.1/enebootools/databaseadmin/dblayer/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     4516 2022-02-08 10:20:48.000000 enebootools-2.0.1/enebootools/databaseadmin/dblayer/drivers.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1507 2022-03-17 10:57:32.000000 enebootools-2.0.1/enebootools/entry_points.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-18 09:31:21.621913 enebootools-2.0.1/enebootools/extracttool/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    10935 2022-02-08 10:20:48.000000 enebootools-2.0.1/enebootools/extracttool/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     3087 2022-02-08 10:20:48.000000 enebootools-2.0.1/enebootools/extracttool/extractfunctions.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-18 09:31:21.621913 enebootools-2.0.1/enebootools/lib/
--rw-r--r--   0 aulla     (1000) aulla     (1000)        0 2020-06-21 07:16:10.000000 enebootools-2.0.1/enebootools/lib/__init__.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-18 09:31:21.625913 enebootools-2.0.1/enebootools/lib/etree/
--rw-r--r--   0 aulla     (1000) aulla     (1000)     5062 2020-06-21 07:16:10.000000 enebootools-2.0.1/enebootools/lib/etree/ElementInclude.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     9477 2022-02-08 10:20:48.000000 enebootools-2.0.1/enebootools/lib/etree/ElementPath.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    55969 2022-02-08 10:20:48.000000 enebootools-2.0.1/enebootools/lib/etree/ElementTree.py
--rw-r--r--   0 aulla     (1000) aulla     (1000)     1604 2020-06-21 07:16:11.000000 enebootools-2.0.1/enebootools/lib/etree/__init__.py
--rw-r--r--   0 aulla     (1000) aulla     (1000)       62 2020-06-21 07:16:11.000000 enebootools-2.0.1/enebootools/lib/etree/cElementTree.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    61938 2022-02-08 10:20:48.000000 enebootools-2.0.1/enebootools/lib/peewee.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     2395 2022-02-08 10:20:48.000000 enebootools-2.0.1/enebootools/lib/utils.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-18 09:31:21.625913 enebootools-2.0.1/enebootools/mergetool/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    25980 2023-05-09 12:42:37.000000 enebootools-2.0.1/enebootools/mergetool/__init__.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-18 09:31:21.629913 enebootools-2.0.1/enebootools/mergetool/etc/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)        0 2022-02-08 10:20:48.000000 enebootools-2.0.1/enebootools/mergetool/etc/__init__.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-18 09:31:21.629913 enebootools-2.0.1/enebootools/mergetool/etc/formats/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)        0 2022-02-08 10:20:48.000000 enebootools-2.0.1/enebootools/mergetool/etc/formats/__init__.py
--rw-r--r--   0 aulla     (1000) aulla     (1000)     1682 2019-12-11 07:08:54.000000 enebootools-2.0.1/enebootools/mergetool/etc/formats/aq23-kut.xml
--rw-r--r--   0 aulla     (1000) aulla     (1000)     2128 2022-02-13 17:42:27.000000 enebootools-2.0.1/enebootools/mergetool/etc/formats/aq23-mtd.xml
--rw-r--r--   0 aulla     (1000) aulla     (1000)     1629 2019-12-11 07:08:54.000000 enebootools-2.0.1/enebootools/mergetool/etc/formats/aq23-xml.xml
--rw-r--r--   0 aulla     (1000) aulla     (1000)     1981 2019-12-11 07:08:54.000000 enebootools-2.0.1/enebootools/mergetool/etc/formats/qt3-ts.xml
--rw-r--r--   0 aulla     (1000) aulla     (1000)     7419 2019-12-11 07:08:54.000000 enebootools-2.0.1/enebootools/mergetool/etc/formats/qt3-ui.xml
--rw-r--r--   0 aulla     (1000) aulla     (1000)      520 2019-12-11 07:08:54.000000 enebootools-2.0.1/enebootools/mergetool/etc/index.xml
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-18 09:31:21.629913 enebootools-2.0.1/enebootools/mergetool/etc/patch-styles/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)        0 2022-02-08 10:20:48.000000 enebootools-2.0.1/enebootools/mergetool/etc/patch-styles/__init__.py
--rw-r--r--   0 aulla     (1000) aulla     (1000)     2214 2019-12-11 07:08:54.000000 enebootools-2.0.1/enebootools/mergetool/etc/patch-styles/legacy1-savepatch1.xsl
--rw-r--r--   0 aulla     (1000) aulla     (1000)      807 2019-12-11 07:08:54.000000 enebootools-2.0.1/enebootools/mergetool/etc/patch-styles/legacy1.xml
--rw-r--r--   0 aulla     (1000) aulla     (1000)      460 2019-12-11 07:08:54.000000 enebootools-2.0.1/enebootools/mergetool/etc/patch-styles/semantic1.xml
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    76872 2023-05-17 19:00:59.000000 enebootools-2.0.1/enebootools/mergetool/flpatchapipy.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    31272 2023-05-09 12:42:28.000000 enebootools-2.0.1/enebootools/mergetool/flpatchdir.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    44114 2022-12-01 11:18:08.000000 enebootools-2.0.1/enebootools/mergetool/flpatchlxml.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    77764 2022-09-28 07:55:55.000000 enebootools-2.0.1/enebootools/mergetool/flpatchmodel.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    76822 2023-05-09 12:25:44.000000 enebootools-2.0.1/enebootools/mergetool/flpatchpy.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    77369 2022-03-06 07:56:52.000000 enebootools-2.0.1/enebootools/mergetool/flpatchqs.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    77651 2022-09-28 07:55:13.000000 enebootools-2.0.1/enebootools/mergetool/flpatchtest.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    24828 2022-02-08 10:20:48.000000 enebootools-2.0.1/enebootools/mergetool/flpatchxml.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     3680 2022-12-01 13:23:45.000000 enebootools-2.0.1/enebootools/mergetool/projectbuilder.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-18 09:31:21.629913 enebootools-2.0.1/enebootools/mergetool/test/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      552 2022-03-18 20:43:46.000000 enebootools-2.0.1/enebootools/mergetool/test/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     2732 2022-04-29 09:13:12.000000 enebootools-2.0.1/enebootools/mergetool/test/test_mergetool.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-18 09:31:21.629913 enebootools-2.0.1/enebootools/packager/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     4372 2022-09-12 07:54:48.000000 enebootools-2.0.1/enebootools/packager/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     6767 2023-01-16 11:50:25.000000 enebootools-2.0.1/enebootools/packager/pkgjoiner.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     8238 2022-02-08 10:20:48.000000 enebootools-2.0.1/enebootools/packager/pkgsplitter.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    15388 2022-11-29 10:40:19.000000 enebootools-2.0.1/enebootools/parseargs.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    13479 2020-06-27 08:28:15.000000 enebootools-2.0.1/enebootools/parseargs.pyc
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-18 09:31:21.629913 enebootools-2.0.1/enebootools/parser/
--rw-r--r--   0 aulla     (1000) aulla     (1000)        0 2020-06-21 07:16:13.000000 enebootools-2.0.1/enebootools/parser/__init__.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-18 09:31:21.629913 enebootools-2.0.1/enebootools/vcsworkflow/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      370 2022-02-08 10:20:48.000000 enebootools-2.0.1/enebootools/vcsworkflow/__init__.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-18 09:31:21.613913 enebootools-2.0.1/enebootools.egg-info/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    19837 2023-05-18 09:31:21.000000 enebootools-2.0.1/enebootools.egg-info/PKG-INFO
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     2874 2023-05-18 09:31:21.000000 enebootools-2.0.1/enebootools.egg-info/SOURCES.txt
--rw-rw-r--   0 aulla     (1000) aulla     (1000)        1 2023-05-18 09:31:21.000000 enebootools-2.0.1/enebootools.egg-info/dependency_links.txt
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      310 2023-05-18 09:31:21.000000 enebootools-2.0.1/enebootools.egg-info/entry_points.txt
--rw-rw-r--   0 aulla     (1000) aulla     (1000)       21 2023-05-18 09:31:21.000000 enebootools-2.0.1/enebootools.egg-info/requires.txt
--rw-rw-r--   0 aulla     (1000) aulla     (1000)       12 2023-05-18 09:31:21.000000 enebootools-2.0.1/enebootools.egg-info/top_level.txt
--rw-rw-r--   0 aulla     (1000) aulla     (1000)       38 2023-05-18 09:31:21.633914 enebootools-2.0.1/setup.cfg
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     2339 2022-02-08 10:20:48.000000 enebootools-2.0.1/setup.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-22 18:38:36.729294 enebootools-2.0.2/
+-rw-r--r--   0 aulla     (1000) aulla     (1000)      259 2019-12-11 07:08:54.000000 enebootools-2.0.2/AUTHORS
+-rw-r--r--   0 aulla     (1000) aulla     (1000)    35146 2019-12-11 07:08:54.000000 enebootools-2.0.2/LICENSE.gplv3
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    19837 2023-05-22 18:38:36.729294 enebootools-2.0.2/PKG-INFO
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    18665 2022-02-08 10:20:48.000000 enebootools-2.0.2/README.rst
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-22 18:38:36.725294 enebootools-2.0.2/enebootools/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     6052 2023-05-22 18:10:27.000000 enebootools-2.0.2/enebootools/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     7116 2020-06-27 08:28:15.000000 enebootools-2.0.2/enebootools/__init__.pyc
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-22 18:38:36.725294 enebootools-2.0.2/enebootools/assembler/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     6326 2023-05-18 09:15:32.000000 enebootools-2.0.2/enebootools/assembler/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     2584 2022-02-08 10:20:48.000000 enebootools-2.0.2/enebootools/assembler/config.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    29859 2023-05-22 17:15:33.000000 enebootools-2.0.2/enebootools/assembler/database.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1325 2022-02-08 10:20:48.000000 enebootools-2.0.2/enebootools/assembler/databasemodels.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1334 2022-03-05 09:43:22.000000 enebootools-2.0.2/enebootools/assembler/featureconfig.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    24737 2023-05-22 18:22:33.000000 enebootools-2.0.2/enebootools/assembler/kobjects.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     2276 2022-02-08 10:20:48.000000 enebootools-2.0.2/enebootools/assembler/mypeewee.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     3124 2022-12-07 11:24:39.000000 enebootools-2.0.2/enebootools/assembler/save_auto.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-22 18:38:36.725294 enebootools-2.0.2/enebootools/autoconfig/
+-rw-r--r--   0 aulla     (1000) aulla     (1000)        0 2020-06-21 07:16:10.000000 enebootools-2.0.2/enebootools/autoconfig/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     7521 2022-03-05 21:54:44.000000 enebootools-2.0.2/enebootools/autoconfig/autoconfig.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1955 2022-02-08 10:20:48.000000 enebootools-2.0.2/enebootools/autoconfig/parsers.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-22 18:38:36.725294 enebootools-2.0.2/enebootools/config/
+-rw-r--r--   0 aulla     (1000) aulla     (1000)        0 2020-06-21 07:16:10.000000 enebootools-2.0.2/enebootools/config/__init__.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-22 18:38:36.725294 enebootools-2.0.2/enebootools/crypto/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     3002 2022-02-08 10:20:48.000000 enebootools-2.0.2/enebootools/crypto/__init__.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-22 18:38:36.725294 enebootools-2.0.2/enebootools/crypto/certificates/
+-rw-r--r--   0 aulla     (1000) aulla     (1000)     2244 2019-12-11 07:08:54.000000 enebootools-2.0.2/enebootools/crypto/certificates/CA_Partners_Gestiweb.crt
+-rw-r--r--   0 aulla     (1000) aulla     (1000)     1854 2019-12-11 07:08:54.000000 enebootools-2.0.2/enebootools/crypto/certificates/CA_Test_Partners.crt
+-rw-r--r--   0 aulla     (1000) aulla     (1000)     2545 2019-12-11 07:08:54.000000 enebootools-2.0.2/enebootools/crypto/certificates/Eneboo_Open_Source_ERP.crt
+-rw-r--r--   0 aulla     (1000) aulla     (1000)     1285 2019-12-11 07:08:54.000000 enebootools-2.0.2/enebootools/crypto/certificates/Partner_Test.crt
+-rw-r--r--   0 aulla     (1000) aulla     (1000)      963 2019-12-11 07:08:54.000000 enebootools-2.0.2/enebootools/crypto/certificates/Partner_Test.pem
+-rw-r--r--   0 aulla     (1000) aulla     (1000)      884 2019-12-11 07:08:54.000000 enebootools-2.0.2/enebootools/crypto/certificates/README.txt
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)        0 2022-02-08 10:20:48.000000 enebootools-2.0.2/enebootools/crypto/certificates/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    27617 2022-09-12 08:13:27.000000 enebootools-2.0.2/enebootools/crypto/main.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-22 18:38:36.725294 enebootools-2.0.2/enebootools/databaseadmin/
+-rw-r--r--   0 aulla     (1000) aulla     (1000)        0 2020-06-21 07:16:10.000000 enebootools-2.0.2/enebootools/databaseadmin/__init__.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-22 18:38:36.725294 enebootools-2.0.2/enebootools/databaseadmin/dblayer/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)        0 2022-02-08 10:20:48.000000 enebootools-2.0.2/enebootools/databaseadmin/dblayer/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     4516 2022-02-08 10:20:48.000000 enebootools-2.0.2/enebootools/databaseadmin/dblayer/drivers.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1507 2022-03-17 10:57:32.000000 enebootools-2.0.2/enebootools/entry_points.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-22 18:38:36.725294 enebootools-2.0.2/enebootools/extracttool/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    10935 2022-02-08 10:20:48.000000 enebootools-2.0.2/enebootools/extracttool/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     3087 2022-02-08 10:20:48.000000 enebootools-2.0.2/enebootools/extracttool/extractfunctions.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-22 18:38:36.725294 enebootools-2.0.2/enebootools/lib/
+-rw-r--r--   0 aulla     (1000) aulla     (1000)        0 2020-06-21 07:16:10.000000 enebootools-2.0.2/enebootools/lib/__init__.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-22 18:38:36.725294 enebootools-2.0.2/enebootools/lib/etree/
+-rw-r--r--   0 aulla     (1000) aulla     (1000)     5062 2020-06-21 07:16:10.000000 enebootools-2.0.2/enebootools/lib/etree/ElementInclude.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     9477 2022-02-08 10:20:48.000000 enebootools-2.0.2/enebootools/lib/etree/ElementPath.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    55969 2022-02-08 10:20:48.000000 enebootools-2.0.2/enebootools/lib/etree/ElementTree.py
+-rw-r--r--   0 aulla     (1000) aulla     (1000)     1604 2020-06-21 07:16:11.000000 enebootools-2.0.2/enebootools/lib/etree/__init__.py
+-rw-r--r--   0 aulla     (1000) aulla     (1000)       62 2020-06-21 07:16:11.000000 enebootools-2.0.2/enebootools/lib/etree/cElementTree.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    61938 2022-02-08 10:20:48.000000 enebootools-2.0.2/enebootools/lib/peewee.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     2395 2022-02-08 10:20:48.000000 enebootools-2.0.2/enebootools/lib/utils.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-22 18:38:36.725294 enebootools-2.0.2/enebootools/mergetool/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    25980 2023-05-09 12:42:37.000000 enebootools-2.0.2/enebootools/mergetool/__init__.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-22 18:38:36.725294 enebootools-2.0.2/enebootools/mergetool/etc/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)        0 2022-02-08 10:20:48.000000 enebootools-2.0.2/enebootools/mergetool/etc/__init__.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-22 18:38:36.725294 enebootools-2.0.2/enebootools/mergetool/etc/formats/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)        0 2022-02-08 10:20:48.000000 enebootools-2.0.2/enebootools/mergetool/etc/formats/__init__.py
+-rw-r--r--   0 aulla     (1000) aulla     (1000)     1682 2019-12-11 07:08:54.000000 enebootools-2.0.2/enebootools/mergetool/etc/formats/aq23-kut.xml
+-rw-r--r--   0 aulla     (1000) aulla     (1000)     2128 2022-02-13 17:42:27.000000 enebootools-2.0.2/enebootools/mergetool/etc/formats/aq23-mtd.xml
+-rw-r--r--   0 aulla     (1000) aulla     (1000)     1629 2019-12-11 07:08:54.000000 enebootools-2.0.2/enebootools/mergetool/etc/formats/aq23-xml.xml
+-rw-r--r--   0 aulla     (1000) aulla     (1000)     1981 2019-12-11 07:08:54.000000 enebootools-2.0.2/enebootools/mergetool/etc/formats/qt3-ts.xml
+-rw-r--r--   0 aulla     (1000) aulla     (1000)     7419 2019-12-11 07:08:54.000000 enebootools-2.0.2/enebootools/mergetool/etc/formats/qt3-ui.xml
+-rw-r--r--   0 aulla     (1000) aulla     (1000)      520 2019-12-11 07:08:54.000000 enebootools-2.0.2/enebootools/mergetool/etc/index.xml
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-22 18:38:36.725294 enebootools-2.0.2/enebootools/mergetool/etc/patch-styles/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)        0 2022-02-08 10:20:48.000000 enebootools-2.0.2/enebootools/mergetool/etc/patch-styles/__init__.py
+-rw-r--r--   0 aulla     (1000) aulla     (1000)     2214 2019-12-11 07:08:54.000000 enebootools-2.0.2/enebootools/mergetool/etc/patch-styles/legacy1-savepatch1.xsl
+-rw-r--r--   0 aulla     (1000) aulla     (1000)      807 2019-12-11 07:08:54.000000 enebootools-2.0.2/enebootools/mergetool/etc/patch-styles/legacy1.xml
+-rw-r--r--   0 aulla     (1000) aulla     (1000)      460 2019-12-11 07:08:54.000000 enebootools-2.0.2/enebootools/mergetool/etc/patch-styles/semantic1.xml
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    76872 2023-05-17 19:00:59.000000 enebootools-2.0.2/enebootools/mergetool/flpatchapipy.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    31272 2023-05-22 14:39:34.000000 enebootools-2.0.2/enebootools/mergetool/flpatchdir.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    44114 2022-12-01 11:18:08.000000 enebootools-2.0.2/enebootools/mergetool/flpatchlxml.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    77764 2022-09-28 07:55:55.000000 enebootools-2.0.2/enebootools/mergetool/flpatchmodel.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    76822 2023-05-09 12:25:44.000000 enebootools-2.0.2/enebootools/mergetool/flpatchpy.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    77369 2022-03-06 07:56:52.000000 enebootools-2.0.2/enebootools/mergetool/flpatchqs.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    77651 2022-09-28 07:55:13.000000 enebootools-2.0.2/enebootools/mergetool/flpatchtest.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    24828 2022-02-08 10:20:48.000000 enebootools-2.0.2/enebootools/mergetool/flpatchxml.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     3708 2023-05-22 15:27:23.000000 enebootools-2.0.2/enebootools/mergetool/projectbuilder.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-22 18:38:36.725294 enebootools-2.0.2/enebootools/mergetool/test/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      552 2022-03-18 20:43:46.000000 enebootools-2.0.2/enebootools/mergetool/test/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     2732 2022-04-29 09:13:12.000000 enebootools-2.0.2/enebootools/mergetool/test/test_mergetool.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-22 18:38:36.725294 enebootools-2.0.2/enebootools/packager/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     4372 2022-09-12 07:54:48.000000 enebootools-2.0.2/enebootools/packager/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     6767 2023-01-16 11:50:25.000000 enebootools-2.0.2/enebootools/packager/pkgjoiner.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     8238 2022-02-08 10:20:48.000000 enebootools-2.0.2/enebootools/packager/pkgsplitter.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    15388 2022-11-29 10:40:19.000000 enebootools-2.0.2/enebootools/parseargs.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    13479 2020-06-27 08:28:15.000000 enebootools-2.0.2/enebootools/parseargs.pyc
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-22 18:38:36.725294 enebootools-2.0.2/enebootools/parser/
+-rw-r--r--   0 aulla     (1000) aulla     (1000)        0 2020-06-21 07:16:13.000000 enebootools-2.0.2/enebootools/parser/__init__.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-22 18:38:36.725294 enebootools-2.0.2/enebootools/vcsworkflow/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      370 2022-02-08 10:20:48.000000 enebootools-2.0.2/enebootools/vcsworkflow/__init__.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-22 18:38:36.725294 enebootools-2.0.2/enebootools.egg-info/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    19837 2023-05-22 18:38:36.000000 enebootools-2.0.2/enebootools.egg-info/PKG-INFO
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     2874 2023-05-22 18:38:36.000000 enebootools-2.0.2/enebootools.egg-info/SOURCES.txt
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)        1 2023-05-22 18:38:36.000000 enebootools-2.0.2/enebootools.egg-info/dependency_links.txt
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      310 2023-05-22 18:38:36.000000 enebootools-2.0.2/enebootools.egg-info/entry_points.txt
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)       21 2023-05-22 18:38:36.000000 enebootools-2.0.2/enebootools.egg-info/requires.txt
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)       12 2023-05-22 18:38:36.000000 enebootools-2.0.2/enebootools.egg-info/top_level.txt
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)       38 2023-05-22 18:38:36.729294 enebootools-2.0.2/setup.cfg
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     2339 2022-02-08 10:20:48.000000 enebootools-2.0.2/setup.py
```

### Comparing `enebootools-2.0.1/LICENSE.gplv3` & `enebootools-2.0.2/LICENSE.gplv3`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.1/PKG-INFO` & `enebootools-2.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: enebootools
-Version: 2.0.1
+Version: 2.0.2
 Summary: ERP tools for Eneboo
 Home-page: https://github.com/aulla/eneboo-tools
 Author: David Martínez Martí, José A. Fernández Fernández
 Author-email: deavidsedice@gmail.com, aullasistemas@gmail.com
 Keywords: erp pineboo eneboo tools
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `enebootools-2.0.1/README.rst` & `enebootools-2.0.2/README.rst`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.1/enebootools/__init__.py` & `enebootools-2.0.2/enebootools/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import os.path
 import sys
 import traceback
 from pprint import pformat
 import enebootools.parseargs as pa
 
 
-__VERSION__ = "2.0.1"
+__VERSION__ = "2.0.2"
 QS_EXTEND_MODE = "legacy"
 
 
 def ustr(value):
     """Ustr."""
     if isinstance(value, str):
         return value
```

### Comparing `enebootools-2.0.1/enebootools/__init__.pyc` & `enebootools-2.0.2/enebootools/__init__.pyc`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.1/enebootools/assembler/__init__.py` & `enebootools-2.0.2/enebootools/assembler/__init__.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.1/enebootools/assembler/config.py` & `enebootools-2.0.2/enebootools/assembler/config.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.1/enebootools/assembler/database.py` & `enebootools-2.0.2/enebootools/assembler/database.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.1/enebootools/assembler/databasemodels.py` & `enebootools-2.0.2/enebootools/assembler/databasemodels.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.1/enebootools/assembler/featureconfig.py` & `enebootools-2.0.2/enebootools/assembler/featureconfig.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.1/enebootools/assembler/kobjects.py` & `enebootools-2.0.2/enebootools/assembler/kobjects.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 from .databasemodels import KnownObjects
 
 
 class BaseObject(object):
     _by_name = {}
     _by_relpath = {}
     _by_formal_name = {}
+    _by_abspath = {}
 
     def __init__(self, iface, obj):
         self.iface = iface
         self.obj = obj
         self.info = {}
         self.all_required_modules = None
         self.all_required_features = None
@@ -31,62 +32,98 @@
             )
             raise
 
         self.__class__._by_name[(self.__class__.__name__, str(self.name))] = self
         self.__class__._by_relpath[(self.__class__.__name__, str(obj.relpath))] = self
         self.__class__._by_formal_name[(self.__class__.__name__, self.formal_name())] = self
 
+        self.__class__._by_abspath[
+            (self.__class__.__name__, str(obj.abspath), self.formal_name())
+        ] = self
+
     def get_info(self):
         self.info = {"provides": [], "requires": []}
         return self.info
 
     def formal_name(self):
         return str(self.obj.relpath)
 
     @classmethod
     def by_name(self, name):
-        return self._by_name.get((self.__name__, str(name)), None)
+        result = self._by_name.get((self.__name__, str(name)), None)
+        # print("1 ****", result)
+        return result
 
     @classmethod
     def by_formal_name(self, name):
-        return self._by_formal_name.get((self.__name__, str(name)), None)
+        result = self._by_formal_name.get((self.__name__, str(name)), None)
+        # print("1 ***", result)
+        return result
 
     @classmethod
     def by_relpath(self, relpath):
-        return self._by_relpath.get((self.__name__, str(relpath)), None)
+        result = self._by_relpath.get((self.__name__, str(relpath)), None)
+        # print("1 **", result)
+        return result
+
+    @classmethod
+    def by_abspath(self, relpath):
+        result = None
+        for num, key in enumerate([item for item in self._by_abspath if item[0] == self.__name__]):
+            obj = self._by_abspath[key]
+            if str(obj.fullpath).endswith("/%s" % relpath):
+                result = obj
+                break
+        result = [
+            value
+            for key, value in self._by_abspath.items()
+            if key[0] == self.__name__ and value.fullpath.endswith("/%s" % relpath)
+        ]
+        # print("1 *", result, getattr(result, "fullpath", None), relpath)
+        return result[0] if result else None
 
     @classmethod
     def items(self):
         return [v for k, v in list(self._by_name.items()) if k[0] == self.__name__]
 
     @classmethod
     def find(self, name):
-        return self.by_formal_name(name) or self.by_name(name) or self.by_relpath(name)
+        return (
+            self.by_abspath(name)
+            or self.by_formal_name(name)
+            or self.by_name(name)
+            or self.by_relpath(name)
+        )
 
     def setup(self):
         pass
 
     @classmethod
     def cls_finish_setup(self):
         for k, obj in list(self._by_name.items()):
             cname, name = k
             if cname != self.__name__:
                 continue
             obj.finish_setup()
 
     def _get_full_required_modules(self):
         if self.all_required_modules:
+            # print("***", self, self.all_required_modules)
             return self.all_required_modules
         req = []
         myreq = []
         for modname in self.required_modules:
             obj = ModuleObject.find(modname)
             if obj is None:
-                self.iface.info("Modulo con nombre %s no encontrado" % modname)
+                self.iface.info(
+                    "Modulo con nombre %s no encontrado (requerido por %s )"
+                    % (modname, self.formal_name())
+                )
                 continue
+            # print("*", self, modname)
             new_reqs = [
                 modulename
                 for modulename in obj._get_full_required_modules()
                 if modulename not in req
             ]
             if self.type == "prj":
                 for n in new_reqs:
@@ -94,22 +131,25 @@
                         continue
                     self.iface.debug(
                         "Proyecto %s, se agrega modulo %s solicitado por %s"
                         % (self.formal_name(), n, modname)
                     )
 
             req += new_reqs
-            myreq.append(obj.formal_name())
+            myreq.append(modname)
 
         self.all_required_features = self._get_full_required_features()
 
         for featname in self.all_required_features:
             obj = FeatureObject.find(featname)
             if obj is None:
-                self.iface.info("Funcionalidad con nombre %s no encontrada" % featname)
+                self.iface.info(
+                    "Funcionalidad con nombre %s no encontrada (requerida por %s )"
+                    % (featname, self.formal_name())
+                )
                 continue
 
             new_reqs = [
                 modulename
                 for modulename in obj._get_full_required_modules()
                 if modulename not in req and modulename not in myreq
             ]
@@ -117,30 +157,33 @@
                 for n in new_reqs:
                     if n in self.required_modules:
                         continue
                     self.iface.debug(
                         "Proyecto %s, se agrega modulo %s solicitado por funcionalidad %s"
                         % (self.formal_name(), n, featname)
                     )
+
             req += new_reqs
 
         req += [modulename for modulename in myreq if modulename not in req]
-
         self.all_required_modules = req
         return req
 
     def _get_full_required_features(self):
         if self.all_required_features:
             return self.all_required_features
         req = []
         myreq = []
         for featname in self.required_features:
             obj = FeatureObject.find(featname)
             if obj is None:
-                self.iface.info("Funcionalidad con nombre %s no encontrada" % featname)
+                self.iface.info(
+                    "Funcionalidad con nombre %s no encontrada (requerida por %s )"
+                    % (featname, self.formal_name())
+                )
                 continue
             new_reqs = [
                 featurename
                 for featurename in obj._get_full_required_features()
                 if featurename not in req
             ]
             if self.type == "prj":
@@ -205,20 +248,22 @@
         cfg = loadFeatureConfig(self.fullfilename)
         self.cfg = cfg
         self.name = cfg.feature.name
         self.code = cfg.feature.code
         self.description = cfg.feature.description
         self.type = cfg.feature.type
         self.dstfolder = None
+
         self.required_modules = read_file_list(
             self.fullpath, "conf/required_modules", errlog=self.iface.warn
         )
         self.required_features = read_file_list(
             self.fullpath, "conf/required_features", errlog=self.iface.warn
         )
+
         self.qs_extend_mode = cfg.feature.qs_extend_mode
 
         self.patch_series = read_file_list(
             self.fullpath, "conf/patch_series", errlog=self.iface.warn
         )
 
         self.iface.debug2("Se ha parseado la funcionalidad %s" % self.name)
@@ -263,14 +308,15 @@
         binstr.set("target", "base")
         binstr.set("path", self.fullpath)
         binstr.set("dstfolder", "build/base")
         if self.dstfolder:
             binstr.set("dstfolder", self.dstfolder)
         etree.SubElement(binstr, "Message", text="Copiando módulos . . .")
         for modulename in self._get_full_required_modules():
+            # print("------->", self.formal_name(), self, modulename)
             module = ModuleObject.find(modulename)
             cpfolder = etree.SubElement(binstr, "CopyFolderAction")
             cpfolder.set("src", module.fullpath)
             cpfolder.set("dst", module.obj.relpath)
             cpfolder.set("create_dst", "yes")
 
         for featurename in self._get_full_required_features():
@@ -579,14 +625,15 @@
         if not feature:
             self.iface.error("Funcionalidad %s desconocida." % func)
             return None
         feature.set_patch_list([newname])
 
     def get_build_actions(self, target, func, dstfolder=None):
         feature = FeatureObject.find(func)
+        # print("*******************", func, feature)
         if not feature:
             self.iface.error("Funcionalidad %s desconocida." % func)
             return None
 
         feature.set_dstfolder(dstfolder)
 
         if target == "base":
```

### Comparing `enebootools-2.0.1/enebootools/assembler/mypeewee.py` & `enebootools-2.0.2/enebootools/assembler/mypeewee.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.1/enebootools/assembler/save_auto.py` & `enebootools-2.0.2/enebootools/assembler/save_auto.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.1/enebootools/autoconfig/autoconfig.py` & `enebootools-2.0.2/enebootools/autoconfig/autoconfig.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.1/enebootools/autoconfig/parsers.py` & `enebootools-2.0.2/enebootools/autoconfig/parsers.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.1/enebootools/crypto/__init__.py` & `enebootools-2.0.2/enebootools/crypto/__init__.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.1/enebootools/crypto/certificates/CA_Partners_Gestiweb.crt` & `enebootools-2.0.2/enebootools/crypto/certificates/CA_Partners_Gestiweb.crt`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.1/enebootools/crypto/certificates/CA_Test_Partners.crt` & `enebootools-2.0.2/enebootools/crypto/certificates/CA_Test_Partners.crt`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.1/enebootools/crypto/certificates/Eneboo_Open_Source_ERP.crt` & `enebootools-2.0.2/enebootools/crypto/certificates/Eneboo_Open_Source_ERP.crt`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.1/enebootools/crypto/certificates/Partner_Test.crt` & `enebootools-2.0.2/enebootools/crypto/certificates/Partner_Test.crt`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.1/enebootools/crypto/certificates/Partner_Test.pem` & `enebootools-2.0.2/enebootools/crypto/certificates/Partner_Test.pem`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.1/enebootools/crypto/certificates/README.txt` & `enebootools-2.0.2/enebootools/crypto/certificates/README.txt`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.1/enebootools/crypto/main.py` & `enebootools-2.0.2/enebootools/crypto/main.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.1/enebootools/databaseadmin/dblayer/drivers.py` & `enebootools-2.0.2/enebootools/databaseadmin/dblayer/drivers.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.1/enebootools/entry_points.py` & `enebootools-2.0.2/enebootools/entry_points.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.1/enebootools/extracttool/__init__.py` & `enebootools-2.0.2/enebootools/extracttool/__init__.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.1/enebootools/extracttool/extractfunctions.py` & `enebootools-2.0.2/enebootools/extracttool/extractfunctions.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.1/enebootools/lib/etree/ElementInclude.py` & `enebootools-2.0.2/enebootools/lib/etree/ElementInclude.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.1/enebootools/lib/etree/ElementPath.py` & `enebootools-2.0.2/enebootools/lib/etree/ElementPath.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.1/enebootools/lib/etree/ElementTree.py` & `enebootools-2.0.2/enebootools/lib/etree/ElementTree.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.1/enebootools/lib/etree/__init__.py` & `enebootools-2.0.2/enebootools/lib/etree/__init__.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.1/enebootools/lib/peewee.py` & `enebootools-2.0.2/enebootools/lib/peewee.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.1/enebootools/lib/utils.py` & `enebootools-2.0.2/enebootools/lib/utils.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.1/enebootools/mergetool/__init__.py` & `enebootools-2.0.2/enebootools/mergetool/__init__.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.1/enebootools/mergetool/etc/formats/aq23-kut.xml` & `enebootools-2.0.2/enebootools/mergetool/etc/formats/aq23-kut.xml`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.1/enebootools/mergetool/etc/formats/aq23-mtd.xml` & `enebootools-2.0.2/enebootools/mergetool/etc/formats/aq23-mtd.xml`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.1/enebootools/mergetool/etc/formats/aq23-xml.xml` & `enebootools-2.0.2/enebootools/mergetool/etc/formats/aq23-xml.xml`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.1/enebootools/mergetool/etc/formats/qt3-ts.xml` & `enebootools-2.0.2/enebootools/mergetool/etc/formats/qt3-ts.xml`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.1/enebootools/mergetool/etc/formats/qt3-ui.xml` & `enebootools-2.0.2/enebootools/mergetool/etc/formats/qt3-ui.xml`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.1/enebootools/mergetool/etc/index.xml` & `enebootools-2.0.2/enebootools/mergetool/etc/index.xml`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.1/enebootools/mergetool/etc/patch-styles/legacy1-savepatch1.xsl` & `enebootools-2.0.2/enebootools/mergetool/etc/patch-styles/legacy1-savepatch1.xsl`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.1/enebootools/mergetool/etc/patch-styles/legacy1.xml` & `enebootools-2.0.2/enebootools/mergetool/etc/patch-styles/legacy1.xml`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.1/enebootools/mergetool/flpatchapipy.py` & `enebootools-2.0.2/enebootools/mergetool/flpatchapipy.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.1/enebootools/mergetool/flpatchdir.py` & `enebootools-2.0.2/enebootools/mergetool/flpatchdir.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.1/enebootools/mergetool/flpatchlxml.py` & `enebootools-2.0.2/enebootools/mergetool/flpatchlxml.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.1/enebootools/mergetool/flpatchmodel.py` & `enebootools-2.0.2/enebootools/mergetool/flpatchmodel.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.1/enebootools/mergetool/flpatchpy.py` & `enebootools-2.0.2/enebootools/mergetool/flpatchpy.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.1/enebootools/mergetool/flpatchqs.py` & `enebootools-2.0.2/enebootools/mergetool/flpatchqs.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.1/enebootools/mergetool/flpatchtest.py` & `enebootools-2.0.2/enebootools/mergetool/flpatchtest.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.1/enebootools/mergetool/flpatchxml.py` & `enebootools-2.0.2/enebootools/mergetool/flpatchxml.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.1/enebootools/mergetool/projectbuilder.py` & `enebootools-2.0.2/enebootools/mergetool/projectbuilder.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,14 @@
         self.path = self.instructions.get("path")
         self.dstfolder = self.instructions.get("dstfolder")
         self.feature = self.instructions.get("feature")
         self.target = self.instructions.get("target")
         self.dstpath = os.path.join(self.path, self.dstfolder)
 
     def execute(self, rebuild=True):
-
         if os.path.exists(self.dstpath):
             if self.instructions[0].tag != "UpdatePatchAction":
                 if not rebuild:
                     return True
 
                 self.iface.info("Borrando carpeta %s . . . " % self.dstpath)
                 shutil.rmtree(self.dstpath)
@@ -47,15 +46,15 @@
         self.iface.msg(text)
 
     def copyFolder(self, src, dst, create_dst=False):
         if create_dst == "yes":
             create_dst = True
         if create_dst == "no":
             create_dst = False
-        self.iface.info("Copiando %s . . . " % (dst))
+        self.iface.info("Copiando %s : %s -> %s. . . " % (dst, src, self.dstpath))
         dst = os.path.join(self.dstpath, dst)
         if not os.path.exists(src):
             self.iface.error("La carpeta %s no existe" % src)
             return False
         pdst = os.path.dirname(dst)
         if not os.path.exists(pdst):
             if create_dst:
```

### Comparing `enebootools-2.0.1/enebootools/mergetool/test/__init__.py` & `enebootools-2.0.2/enebootools/mergetool/test/__init__.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.1/enebootools/mergetool/test/test_mergetool.py` & `enebootools-2.0.2/enebootools/mergetool/test/test_mergetool.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.1/enebootools/packager/__init__.py` & `enebootools-2.0.2/enebootools/packager/__init__.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.1/enebootools/packager/pkgjoiner.py` & `enebootools-2.0.2/enebootools/packager/pkgjoiner.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.1/enebootools/packager/pkgsplitter.py` & `enebootools-2.0.2/enebootools/packager/pkgsplitter.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.1/enebootools/parseargs.py` & `enebootools-2.0.2/enebootools/parseargs.py`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.1/enebootools/parseargs.pyc` & `enebootools-2.0.2/enebootools/parseargs.pyc`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.1/enebootools.egg-info/PKG-INFO` & `enebootools-2.0.2/enebootools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: enebootools
-Version: 2.0.1
+Version: 2.0.2
 Summary: ERP tools for Eneboo
 Home-page: https://github.com/aulla/eneboo-tools
 Author: David Martínez Martí, José A. Fernández Fernández
 Author-email: deavidsedice@gmail.com, aullasistemas@gmail.com
 Keywords: erp pineboo eneboo tools
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `enebootools-2.0.1/enebootools.egg-info/SOURCES.txt` & `enebootools-2.0.2/enebootools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `enebootools-2.0.1/setup.py` & `enebootools-2.0.2/setup.py`

 * *Files identical despite different names*

