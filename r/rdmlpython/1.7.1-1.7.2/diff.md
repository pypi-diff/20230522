# Comparing `tmp/rdmlpython-1.7.1-py2.py3-none-any.whl.zip` & `tmp/rdmlpython-1.7.2-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 128215 bytes, number of entries: 14
+Zip file size: 128238 bytes, number of entries: 14
 -rw-rw-r--  2.0 unx     1081 b- defN 22-May-01 03:55 rdmlpython/LICENSE
 -rw-rw-r--  2.0 unx     1346 b- defN 22-May-01 03:55 rdmlpython/README.md
 -rw-rw-r--  2.0 unx       80 b- defN 22-May-01 03:55 rdmlpython/__init__.py
--rw-rw-r--  2.0 unx   715416 b- defN 23-Mar-06 07:07 rdmlpython/rdml.py
+-rw-rw-r--  2.0 unx   715343 b- defN 23-May-22 15:02 rdmlpython/rdml.py
 -rw-rw-r--  2.0 unx    45122 b- defN 22-May-01 03:55 rdmlpython/schema/RDML_v1_0_REC.xsd
 -rw-rw-r--  2.0 unx    48807 b- defN 22-May-01 03:55 rdmlpython/schema/RDML_v1_1_REC.xsd
 -rw-rw-r--  2.0 unx    50404 b- defN 22-May-01 03:55 rdmlpython/schema/RDML_v1_2_REC.xsd
 -rw-rw-r--  2.0 unx    62703 b- defN 23-Mar-06 07:06 rdmlpython/schema/RDML_v1_3_REC.xsd
--rw-rw-r--  2.0 unx     1081 b- defN 23-Mar-06 07:14 rdmlpython-1.7.1.dist-info/LICENSE.txt
--rw-rw-r--  2.0 unx      945 b- defN 23-Mar-06 07:14 rdmlpython-1.7.1.dist-info/METADATA
--rw-rw-r--  2.0 unx      110 b- defN 23-Mar-06 07:14 rdmlpython-1.7.1.dist-info/WHEEL
--rw-rw-r--  2.0 unx       53 b- defN 23-Mar-06 07:14 rdmlpython-1.7.1.dist-info/entry_points.txt
--rw-rw-r--  2.0 unx       11 b- defN 23-Mar-06 07:14 rdmlpython-1.7.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1181 b- defN 23-Mar-06 07:14 rdmlpython-1.7.1.dist-info/RECORD
-14 files, 928340 bytes uncompressed, 126251 bytes compressed:  86.4%
+-rw-rw-r--  2.0 unx     1081 b- defN 23-May-22 15:06 rdmlpython-1.7.2.dist-info/LICENSE.txt
+-rw-rw-r--  2.0 unx      981 b- defN 23-May-22 15:06 rdmlpython-1.7.2.dist-info/METADATA
+-rw-rw-r--  2.0 unx      110 b- defN 23-May-22 15:06 rdmlpython-1.7.2.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       53 b- defN 23-May-22 15:06 rdmlpython-1.7.2.dist-info/entry_points.txt
+-rw-rw-r--  2.0 unx       11 b- defN 23-May-22 15:06 rdmlpython-1.7.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1181 b- defN 23-May-22 15:06 rdmlpython-1.7.2.dist-info/RECORD
+14 files, 928303 bytes uncompressed, 126274 bytes compressed:  86.4%
```

## zipnote {}

```diff
@@ -18,26 +18,26 @@
 
 Filename: rdmlpython/schema/RDML_v1_2_REC.xsd
 Comment: 
 
 Filename: rdmlpython/schema/RDML_v1_3_REC.xsd
 Comment: 
 
-Filename: rdmlpython-1.7.1.dist-info/LICENSE.txt
+Filename: rdmlpython-1.7.2.dist-info/LICENSE.txt
 Comment: 
 
-Filename: rdmlpython-1.7.1.dist-info/METADATA
+Filename: rdmlpython-1.7.2.dist-info/METADATA
 Comment: 
 
-Filename: rdmlpython-1.7.1.dist-info/WHEEL
+Filename: rdmlpython-1.7.2.dist-info/WHEEL
 Comment: 
 
-Filename: rdmlpython-1.7.1.dist-info/entry_points.txt
+Filename: rdmlpython-1.7.2.dist-info/entry_points.txt
 Comment: 
 
-Filename: rdmlpython-1.7.1.dist-info/top_level.txt
+Filename: rdmlpython-1.7.2.dist-info/top_level.txt
 Comment: 
 
-Filename: rdmlpython-1.7.1.dist-info/RECORD
+Filename: rdmlpython-1.7.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## rdmlpython/rdml.py

```diff
@@ -25,15 +25,15 @@
 def get_rdml_lib_version():
     """Return the version string of the RDML library.
 
     Returns:
         The version string of the RDML library.
     """
 
-    return "1.7.1"
+    return "1.7.2"
 
 
 class NpEncoder(json.JSONEncoder):
     def default(self, obj):
         if isinstance(obj, np.integer):
             return int(obj)
         elif isinstance(obj, np.floating):
@@ -1875,40 +1875,39 @@
 
 
 def _getXMLPartitionDataType():
     return ["tar", "excluded", "note", "pos", "neg", "undef", "excl", "conc"]
 
 def runStatistics(statTarGroup, parametric):
     ret = {}
+    if len(statTarGroup) < 2:
+        ret["test name"] = "no test possible"
+        ret["stat name"] = "only 1 group"
+        ret["stat val"] = -1.0
+        ret["p val"] = -1.0
+        return ret
+
     if _string_to_bool(parametric, triple=False):
         if len(statTarGroup) == 2:
             ret["test name"] = "T-test"
             ret["stat name"] = "t-statistic"
             ret["stat val"], ret["p val"] = scp.ttest_ind(statTarGroup[0], statTarGroup[1])
         else:
             ret["test name"] = "One-way ANOVA"
             ret["stat name"] = "F statistic"
-            if len(statTarGroup) > 2:
-                ret["stat val"], ret["p val"] = scp.f_oneway(*statTarGroup)
-            else:
-                ret["stat val"] = -1.0
-                ret["p val"] = -1.0
+            ret["stat val"], ret["p val"] = scp.f_oneway(*statTarGroup)
     else:
         if len(statTarGroup) == 2:
             ret["test name"] = "Mann-Whitney U rank test"
             ret["stat name"] = "U statistic"
             ret["stat val"], ret["p val"] = scp.mannwhitneyu(statTarGroup[0], statTarGroup[1], alternative='two-sided', use_continuity=False, method='asymptotic')
         else:
             ret["test name"] = "Kruskal-Wallis H-test"
             ret["stat name"] = "H statistic"
-            if len(statTarGroup) > 2:
-                ret["stat val"], ret["p val"] = scp.kruskal(*statTarGroup)
-            else:
-                ret["stat val"] = -1.0
-                ret["p val"] = -1.0
+            ret["stat val"], ret["p val"] = scp.kruskal(*statTarGroup)
     return ret
 
 def webAppRunStatistics(data, parametric=False, seperator='\t', replaceComma=True):
     replaceComma = _string_to_bool(replaceComma, triple=False)
     goodData = []
     foundGrp = {}
     posGrp = 0
```

## Comparing `rdmlpython-1.7.1.dist-info/LICENSE.txt` & `rdmlpython-1.7.2.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `rdmlpython-1.7.1.dist-info/METADATA` & `rdmlpython-1.7.2.dist-info/METADATA`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: rdmlpython
-Version: 1.7.1
+Version: 1.7.2
 Summary: A package to read and edit RDML files.
 Home-page: https://github.com/RDML-consortium/rdmlpython
 Author: Andreas Untergasser
 Author-email: andreas@untergasser.de
 License: MIT
 Platform: UNKNOWN
 License-File: LICENSE.txt
 Requires-Dist: lxml (>=4.2.1)
+Requires-Dist: matplotlib (>=3.5.1)
 Requires-Dist: numpy (>=1.17.2)
 Requires-Dist: scipy (>=1.3.1)
 
 ==========
 rdmlpython
 ==========
```

## Comparing `rdmlpython-1.7.1.dist-info/RECORD` & `rdmlpython-1.7.2.dist-info/RECORD`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 rdmlpython/LICENSE,sha256=s63LBVUlw7-UsUMBWzxXzcSqoVhNdfyZRrbUwJbeWlE,1081
 rdmlpython/README.md,sha256=HkAq5cp8Qf_T5FWWUQXX2FFa8IeKSdHbvwPO35f8gXQ,1346
 rdmlpython/__init__.py,sha256=IlNJYd7eiSl5tQMG-ilfx5PmU69XAhyjMxKwrq5V0fQ,80
-rdmlpython/rdml.py,sha256=EzAB5WLeOMMdkgU3KblFHL7CnNOOR88JXhbZus1M-tE,715416
+rdmlpython/rdml.py,sha256=rb9Ntt_87bc79q3C-YL3LR2N0eAJf3ynyJNE8sykJ8U,715343
 rdmlpython/schema/RDML_v1_0_REC.xsd,sha256=xqB80i-CcCLuZG98aTeNGhaEKNuU8UkFFvMN6Avpk9Y,45122
 rdmlpython/schema/RDML_v1_1_REC.xsd,sha256=0aGXMjhWKHVTckkBUT6b8AmIbpGM4AfrW9HbCq_qsqQ,48807
 rdmlpython/schema/RDML_v1_2_REC.xsd,sha256=Xse7HgwzOprF8xuIGyBdFSG6MV4uC5Bx2FjHj8mN77Y,50404
 rdmlpython/schema/RDML_v1_3_REC.xsd,sha256=R-Y1A5xkgEtEx_MeGVe-lUd2pMm78p8gf6fuZq2IhdY,62703
-rdmlpython-1.7.1.dist-info/LICENSE.txt,sha256=s63LBVUlw7-UsUMBWzxXzcSqoVhNdfyZRrbUwJbeWlE,1081
-rdmlpython-1.7.1.dist-info/METADATA,sha256=o4xUctZPcK-7d2gb3Y4oqC5lse0cUSj982gpqcmbo9Y,945
-rdmlpython-1.7.1.dist-info/WHEEL,sha256=z9j0xAa_JmUKMpmz72K0ZGALSM_n-wQVmGbleXx2VHg,110
-rdmlpython-1.7.1.dist-info/entry_points.txt,sha256=XjqmToTCDPC-ZNh0HGi9tk_XrzVHr3cR0BZ0yCSIsH4,53
-rdmlpython-1.7.1.dist-info/top_level.txt,sha256=AzaMwJpLiO0z5uXzhbXxA-WwJWEfToq2G1Z_PTD1esE,11
-rdmlpython-1.7.1.dist-info/RECORD,,
+rdmlpython-1.7.2.dist-info/LICENSE.txt,sha256=s63LBVUlw7-UsUMBWzxXzcSqoVhNdfyZRrbUwJbeWlE,1081
+rdmlpython-1.7.2.dist-info/METADATA,sha256=yPmTrnMsr6KOwQW_zULf4d-2HBKakq6gGlg367-KIts,981
+rdmlpython-1.7.2.dist-info/WHEEL,sha256=z9j0xAa_JmUKMpmz72K0ZGALSM_n-wQVmGbleXx2VHg,110
+rdmlpython-1.7.2.dist-info/entry_points.txt,sha256=XjqmToTCDPC-ZNh0HGi9tk_XrzVHr3cR0BZ0yCSIsH4,53
+rdmlpython-1.7.2.dist-info/top_level.txt,sha256=AzaMwJpLiO0z5uXzhbXxA-WwJWEfToq2G1Z_PTD1esE,11
+rdmlpython-1.7.2.dist-info/RECORD,,
```

