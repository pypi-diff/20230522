# Comparing `tmp/dwiqc-0.1.6-py2.py3-none-any.whl.zip` & `tmp/dwiqc-0.1.7-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,22 +1,22 @@
-Zip file size: 22214 bytes, number of entries: 20
+Zip file size: 22218 bytes, number of entries: 20
 -rw-r--r--  2.0 unx      225 b- defN 23-May-19 16:11 dwiqc/__init__.py
--rw-r--r--  2.0 unx      247 b- defN 23-May-22 11:43 dwiqc/__version__.py
+-rw-r--r--  2.0 unx      247 b- defN 23-May-22 17:21 dwiqc/__version__.py
 -rw-r--r--  2.0 unx       62 b- defN 23-May-19 16:11 dwiqc/cli/__init__.py
 -rw-r--r--  2.0 unx     6651 b- defN 23-May-19 16:11 dwiqc/cli/get.py
 -rw-r--r--  2.0 unx     5273 b- defN 23-May-19 16:11 dwiqc/cli/process.py
 -rw-r--r--  2.0 unx      160 b- defN 23-May-19 16:11 dwiqc/config/__init__.py
 -rw-r--r--  2.0 unx      274 b- defN 23-May-19 16:11 dwiqc/config/dwiqc.yaml
 -rw-r--r--  2.0 unx       98 b- defN 23-May-19 16:11 dwiqc/state/__init__.py
 -rw-r--r--  2.0 unx     1892 b- defN 23-May-19 16:11 dwiqc/tasks/__init__.py
 -rw-r--r--  2.0 unx     9604 b- defN 23-May-22 11:40 dwiqc/tasks/prequal.py
 -rw-r--r--  2.0 unx     4209 b- defN 23-May-22 17:12 dwiqc/tasks/prequal_EQ.py
 -rw-r--r--  2.0 unx     6193 b- defN 23-May-19 16:11 dwiqc/tasks/qsiprep.py
 -rw-r--r--  2.0 unx     3782 b- defN 23-May-19 16:11 dwiqc/tasks/qsiprep_EQ.py
 -rw-r--r--  2.0 unx    13839 b- defN 23-May-19 16:11 dwiqc/xnat/__init__.py
--rwxr-xr-x  2.0 unx     3876 b- defN 23-May-22 17:17 dwiqc-0.1.6.data/scripts/dwiQC.py
--rw-r--r--  2.0 unx     1541 b- defN 23-May-22 17:17 dwiqc-0.1.6.dist-info/LICENSE
--rw-r--r--  2.0 unx      432 b- defN 23-May-22 17:17 dwiqc-0.1.6.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 23-May-22 17:17 dwiqc-0.1.6.dist-info/WHEEL
--rw-r--r--  2.0 unx        6 b- defN 23-May-22 17:17 dwiqc-0.1.6.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1559 b- defN 23-May-22 17:17 dwiqc-0.1.6.dist-info/RECORD
-20 files, 60033 bytes uncompressed, 19702 bytes compressed:  67.2%
+-rwxr-xr-x  2.0 unx     3889 b- defN 23-May-22 17:22 dwiqc-0.1.7.data/scripts/dwiQC.py
+-rw-r--r--  2.0 unx     1541 b- defN 23-May-22 17:22 dwiqc-0.1.7.dist-info/LICENSE
+-rw-r--r--  2.0 unx      432 b- defN 23-May-22 17:22 dwiqc-0.1.7.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 23-May-22 17:22 dwiqc-0.1.7.dist-info/WHEEL
+-rw-r--r--  2.0 unx        6 b- defN 23-May-22 17:22 dwiqc-0.1.7.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1559 b- defN 23-May-22 17:22 dwiqc-0.1.7.dist-info/RECORD
+20 files, 60046 bytes uncompressed, 19706 bytes compressed:  67.2%
```

## zipnote {}

```diff
@@ -36,26 +36,26 @@
 
 Filename: dwiqc/tasks/qsiprep_EQ.py
 Comment: 
 
 Filename: dwiqc/xnat/__init__.py
 Comment: 
 
-Filename: dwiqc-0.1.6.data/scripts/dwiQC.py
+Filename: dwiqc-0.1.7.data/scripts/dwiQC.py
 Comment: 
 
-Filename: dwiqc-0.1.6.dist-info/LICENSE
+Filename: dwiqc-0.1.7.dist-info/LICENSE
 Comment: 
 
-Filename: dwiqc-0.1.6.dist-info/METADATA
+Filename: dwiqc-0.1.7.dist-info/METADATA
 Comment: 
 
-Filename: dwiqc-0.1.6.dist-info/WHEEL
+Filename: dwiqc-0.1.7.dist-info/WHEEL
 Comment: 
 
-Filename: dwiqc-0.1.6.dist-info/top_level.txt
+Filename: dwiqc-0.1.7.dist-info/top_level.txt
 Comment: 
 
-Filename: dwiqc-0.1.6.dist-info/RECORD
+Filename: dwiqc-0.1.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## dwiqc/__version__.py

```diff
@@ -1,6 +1,6 @@
 __title__ = 'dwiqc'
 __description__ = 'Quality Assurance Pipeline for Diffusion MR Data'
 __url__ = 'https://github.com/harvard-nrg/dwiqc'
-__version__ = '0.1.6'
+__version__ = '0.1.7'
 __author__ = 'Neuroinformatics Research Group'
 __author_email__ = 'info@neuroinfo.org'
```

## Comparing `dwiqc-0.1.6.data/scripts/dwiQC.py` & `dwiqc-0.1.7.data/scripts/dwiQC.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 #!python
 import sys
+import dwiqc
 import dwiqc.cli as cli
 import logging
 import argparse as ap
 import dwiqc.config as config
 
 logger = logging.getLogger(__name__)
```

## Comparing `dwiqc-0.1.6.dist-info/LICENSE` & `dwiqc-0.1.7.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `dwiqc-0.1.6.dist-info/RECORD` & `dwiqc-0.1.7.dist-info/RECORD`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 dwiqc/__init__.py,sha256=MZJhUZKhHHoZ2w_GeoFCITk1m_0ASdRw_ZaeDixFEPU,225
-dwiqc/__version__.py,sha256=50io5Tx6T9X_YO_hb6xtNGd0H7R7JVEU_sGpfCbMeWY,247
+dwiqc/__version__.py,sha256=BdsNVD-rz7vCM7FhM2lAbUOCWPLzzSnEk2Nnljq1rmE,247
 dwiqc/cli/__init__.py,sha256=zGIm7lrjh3wA191D-VjQBZNjSlspFUx148VwDNQGaTk,62
 dwiqc/cli/get.py,sha256=6ixaBdwEgY_GXh8L-_3QDY4MEsNqSJgXle_mxW99mlk,6651
 dwiqc/cli/process.py,sha256=X4eUXf-jRuOR_3cVQ0FfcDXmNPVQzILH35uGAtz9upE,5273
 dwiqc/config/__init__.py,sha256=k_w5JzoJN_7R7eI_sIJxHA4FQQHs0_KGf-6jsbG4Xs8,160
 dwiqc/config/dwiqc.yaml,sha256=x8gKMFZyChdzvNX3GthRe0eWvyKDDL5itXo0kLWVfd0,274
 dwiqc/state/__init__.py,sha256=NaRifw26bI3F1J9BqeLa-KLSzEPq2m_UNhMbXdmPdh4,98
 dwiqc/tasks/__init__.py,sha256=LnlN7iYjpqiBic2ihFrM-_h7m8FD_N7Beh7UIwKyGZ8,1892
 dwiqc/tasks/prequal.py,sha256=5Bgf8D_ML0hXZlV-5s2j8tHiWqUMAQc9XuvV22LIkb4,9604
 dwiqc/tasks/prequal_EQ.py,sha256=PWmlo8u_D5qM1lyXdmT7iq865JL6xoPM0JHGEwzRnes,4209
 dwiqc/tasks/qsiprep.py,sha256=RS8M07BO7ngImbUl1uaOSwPu1BF3NOB_-NhVcuP8vVc,6193
 dwiqc/tasks/qsiprep_EQ.py,sha256=JWildptHsuyJVj7ZYMFlWWYvsAIszJpWk1a0m05JM-Q,3782
 dwiqc/xnat/__init__.py,sha256=PyJJtcfxf71c9x1LwdCem2bT_2MNuqhRmb0uLTfoGgs,13839
-dwiqc-0.1.6.data/scripts/dwiQC.py,sha256=PCkcQfG5Xpm83O_Da4nw_dAozAtN83d1rF5lmoUUyQg,3876
-dwiqc-0.1.6.dist-info/LICENSE,sha256=ReOF9BmlQdkCj4b2gQYogJrk_QkbUAuz8W1ZVqI0pcs,1541
-dwiqc-0.1.6.dist-info/METADATA,sha256=BrzjpugLoUJeSb_LCpI6qwXmXRxrE1IcDIXDAVDSrcg,432
-dwiqc-0.1.6.dist-info/WHEEL,sha256=z9j0xAa_JmUKMpmz72K0ZGALSM_n-wQVmGbleXx2VHg,110
-dwiqc-0.1.6.dist-info/top_level.txt,sha256=omH7pmKt7fzFyiNkTPDLX4yyBccoge5Saqc9rgyu0Wk,6
-dwiqc-0.1.6.dist-info/RECORD,,
+dwiqc-0.1.7.data/scripts/dwiQC.py,sha256=OkI1WZqnUIqS4DWSt-pSm01taEv3m_aNmqSJUM50N_U,3889
+dwiqc-0.1.7.dist-info/LICENSE,sha256=ReOF9BmlQdkCj4b2gQYogJrk_QkbUAuz8W1ZVqI0pcs,1541
+dwiqc-0.1.7.dist-info/METADATA,sha256=sWnfhM8BXX0Wg_UC4NyUeHnTM_goBXfMFP9XNNtOF0M,432
+dwiqc-0.1.7.dist-info/WHEEL,sha256=z9j0xAa_JmUKMpmz72K0ZGALSM_n-wQVmGbleXx2VHg,110
+dwiqc-0.1.7.dist-info/top_level.txt,sha256=omH7pmKt7fzFyiNkTPDLX4yyBccoge5Saqc9rgyu0Wk,6
+dwiqc-0.1.7.dist-info/RECORD,,
```

