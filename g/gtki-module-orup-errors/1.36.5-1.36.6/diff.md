# Comparing `tmp/gtki_module_orup_errors-1.36.5-py3-none-any.whl.zip` & `tmp/gtki_module_orup_errors-1.36.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,19 +1,19 @@
-Zip file size: 13041 bytes, number of entries: 17
+Zip file size: 13045 bytes, number of entries: 17
 -rw-rw-rw-  2.0 fat        0 b- defN 21-Oct-20 07:03 orup_errors/__init__.py
--rw-rw-rw-  2.0 fat    16857 b- defN 23-May-11 06:51 orup_errors/all_errors.py
+-rw-rw-rw-  2.0 fat    16858 b- defN 23-May-22 12:16 orup_errors/all_errors.py
 -rw-rw-rw-  2.0 fat     9664 b- defN 23-May-17 08:46 orup_errors/check_funcs.py
 -rw-rw-rw-  2.0 fat     2473 b- defN 23-May-11 06:51 orup_errors/general_functions.py
 -rw-rw-rw-  2.0 fat     2400 b- defN 23-May-15 09:31 orup_errors/main.py
 -rw-rw-rw-  2.0 fat        0 b- defN 21-Oct-20 07:03 orup_errors/tests/__init__.py
 -rw-rw-rw-  2.0 fat     1545 b- defN 21-Oct-20 07:03 orup_errors/tests/all_errors_test.py
 -rw-rw-rw-  2.0 fat      744 b- defN 21-Oct-20 07:03 orup_errors/tests/args_test.py
 -rw-rw-rw-  2.0 fat      288 b- defN 21-Dec-03 04:31 orup_errors/tests/check_funcs_test.py
 -rw-rw-rw-  2.0 fat     1385 b- defN 21-Oct-20 07:03 orup_errors/tests/draw_win_test.py
 -rw-rw-rw-  2.0 fat     1300 b- defN 21-Dec-03 04:20 orup_errors/tests/general_functions_test.py
 -rw-rw-rw-  2.0 fat        0 b- defN 21-Oct-20 07:03 orup_errors/tests/orup_errors_operator_test.py
--rw-rw-rw-  2.0 fat     1091 b- defN 23-May-17 08:47 gtki_module_orup_errors-1.36.5.dist-info/LICENSE
--rw-rw-rw-  2.0 fat      156 b- defN 23-May-17 08:47 gtki_module_orup_errors-1.36.5.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-May-17 08:47 gtki_module_orup_errors-1.36.5.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       12 b- defN 23-May-17 08:47 gtki_module_orup_errors-1.36.5.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1524 b- defN 23-May-17 08:47 gtki_module_orup_errors-1.36.5.dist-info/RECORD
-17 files, 39531 bytes uncompressed, 10479 bytes compressed:  73.5%
+-rw-rw-rw-  2.0 fat     1091 b- defN 23-May-22 12:17 gtki_module_orup_errors-1.36.6.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat      156 b- defN 23-May-22 12:17 gtki_module_orup_errors-1.36.6.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-May-22 12:17 gtki_module_orup_errors-1.36.6.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       12 b- defN 23-May-22 12:17 gtki_module_orup_errors-1.36.6.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1524 b- defN 23-May-22 12:17 gtki_module_orup_errors-1.36.6.dist-info/RECORD
+17 files, 39532 bytes uncompressed, 10483 bytes compressed:  73.5%
```

## zipnote {}

```diff
@@ -30,23 +30,23 @@
 
 Filename: orup_errors/tests/general_functions_test.py
 Comment: 
 
 Filename: orup_errors/tests/orup_errors_operator_test.py
 Comment: 
 
-Filename: gtki_module_orup_errors-1.36.5.dist-info/LICENSE
+Filename: gtki_module_orup_errors-1.36.6.dist-info/LICENSE
 Comment: 
 
-Filename: gtki_module_orup_errors-1.36.5.dist-info/METADATA
+Filename: gtki_module_orup_errors-1.36.6.dist-info/METADATA
 Comment: 
 
-Filename: gtki_module_orup_errors-1.36.5.dist-info/WHEEL
+Filename: gtki_module_orup_errors-1.36.6.dist-info/WHEEL
 Comment: 
 
-Filename: gtki_module_orup_errors-1.36.5.dist-info/top_level.txt
+Filename: gtki_module_orup_errors-1.36.6.dist-info/top_level.txt
 Comment: 
 
-Filename: gtki_module_orup_errors-1.36.5.dist-info/RECORD
+Filename: gtki_module_orup_errors-1.36.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## orup_errors/all_errors.py

```diff
@@ -172,15 +172,15 @@
                       'debtor_carrier':
                           {'check_func': check_funcs.check_carrier_debtor,
                            'description': 'Перевозчик в списке должников (статус 0 или False)',
                            'error_text': "Въезд для этого перевозчика запрещен!"
                                          "\nПричина: {}.\n"
                                          "Согласуйте заезд с офисом, добавьте комментарий и нажмите 'Принять' еще раз.",
                            'shown': False,
-                           'active': True,
+                           'active': False,
                            'skippable': False,
                            'tests': {'correct_values': {'carrier_name': 'TEST', 'debtors_list': ['TEST2']},
                                      'incorrect_values': {'carrier_name': 'TEST', 'debtors_list': ['TEST']}}
                            },
                       'debtor_client':
                           {'check_func': check_funcs.check_client_debtor,
                            'description': 'Клиент в списке должников (статус 0 или False)',
```

## Comparing `gtki_module_orup_errors-1.36.5.dist-info/LICENSE` & `gtki_module_orup_errors-1.36.6.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `gtki_module_orup_errors-1.36.5.dist-info/RECORD` & `gtki_module_orup_errors-1.36.6.dist-info/RECORD`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 orup_errors/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-orup_errors/all_errors.py,sha256=rU5KKPhSNn9JGTDybC_krJdhVdmNUzas_2tqDdhneYU,16857
+orup_errors/all_errors.py,sha256=TXogWR07YiWavuxNmwWa1d7w39vmslezvpCdHpq7EyM,16858
 orup_errors/check_funcs.py,sha256=d76bZO5SGf_SLFKI9h3hwhK9-oOLLveMcGdF4dj7CVg,9664
 orup_errors/general_functions.py,sha256=4nvGzaj0MwcFeQlDhR1JUaZB1DNdo2nLnwbcMjNxjP8,2473
 orup_errors/main.py,sha256=LSt2yarmVoUQct2gbvn4f4n62yD6YkHeU4eq4wd3GK4,2400
 orup_errors/tests/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 orup_errors/tests/all_errors_test.py,sha256=Lxq5C6Ka5XaHPOVMCQdMSuZT3l07TaJuoGP5l4ZJU_0,1545
 orup_errors/tests/args_test.py,sha256=rz64Iv4D8nPuDlATAHuO_4wFRS20b71gYsIyotaw1pI,744
 orup_errors/tests/check_funcs_test.py,sha256=m5e0kAHg5AcEi2VfRLBEslCAKfFDs8ARWb8emZ_j1Pk,288
 orup_errors/tests/draw_win_test.py,sha256=dsrfPhbnArm08IukF_zypmUFYOw1wjHD_5qYHYjk-88,1385
 orup_errors/tests/general_functions_test.py,sha256=CHoOqcw6k2qLUfgHnGA4TTgACt25jIZNDkF0UnKRtlQ,1300
 orup_errors/tests/orup_errors_operator_test.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-gtki_module_orup_errors-1.36.5.dist-info/LICENSE,sha256=6kbiFSfobTZ7beWiKnHpN902HgBx-Jzgcme0SvKqhKY,1091
-gtki_module_orup_errors-1.36.5.dist-info/METADATA,sha256=kz4PlOu5UwodPCAc9JTdKhtW9G-RH2aU01UnefMFe-w,156
-gtki_module_orup_errors-1.36.5.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-gtki_module_orup_errors-1.36.5.dist-info/top_level.txt,sha256=WzasBtx2xqnJAQK3vavyWJNr2nwUAPObo6jw7F1FFko,12
-gtki_module_orup_errors-1.36.5.dist-info/RECORD,,
+gtki_module_orup_errors-1.36.6.dist-info/LICENSE,sha256=6kbiFSfobTZ7beWiKnHpN902HgBx-Jzgcme0SvKqhKY,1091
+gtki_module_orup_errors-1.36.6.dist-info/METADATA,sha256=iqPaAp4adrm6lD4OEpvmqpgdz3KbZfoeCTJUtXRWulU,156
+gtki_module_orup_errors-1.36.6.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+gtki_module_orup_errors-1.36.6.dist-info/top_level.txt,sha256=WzasBtx2xqnJAQK3vavyWJNr2nwUAPObo6jw7F1FFko,12
+gtki_module_orup_errors-1.36.6.dist-info/RECORD,,
```

