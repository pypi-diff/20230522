# Comparing `tmp/shinherpro-1.6.4.tar.gz` & `tmp/shinherpro-1.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shinherpro-1.6.4.tar", last modified: Sun May 21 15:22:46 2023, max compression
+gzip compressed data, was "shinherpro-1.6.5.tar", last modified: Mon May 22 15:34:34 2023, max compression
```

## Comparing `shinherpro-1.6.4.tar` & `shinherpro-1.6.5.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-21 15:22:46.550748 shinherpro-1.6.4/
--rw-rw-rw-   0        0        0     4623 2023-05-21 15:22:46.550251 shinherpro-1.6.4/PKG-INFO
--rw-rw-rw-   0        0        0     4443 2023-05-21 09:21:34.000000 shinherpro-1.6.4/README.md
--rw-rw-rw-   0        0        0       42 2023-05-21 15:22:46.551243 shinherpro-1.6.4/setup.cfg
--rw-rw-rw-   0        0        0      852 2023-05-21 15:22:25.000000 shinherpro-1.6.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-21 15:22:46.532648 shinherpro-1.6.4/shinherpro/
--rw-rw-rw-   0        0        0     9358 2023-05-21 15:22:31.000000 shinherpro-1.6.4/shinherpro/TYAI.py
--rw-rw-rw-   0        0        0        0 2023-05-18 14:47:36.000000 shinherpro-1.6.4/shinherpro/__init__.py
--rw-rw-rw-   0        0        0     1225 2023-05-21 09:03:22.000000 shinherpro-1.6.4/shinherpro/chormeDriver.py
--rw-rw-rw-   0        0        0     2127 2023-05-21 08:58:49.000000 shinherpro-1.6.4/shinherpro/vfcModel.py
-drwxrwxrwx   0        0        0        0 2023-05-21 15:22:46.548266 shinherpro-1.6.4/shinherpro.egg-info/
--rw-rw-rw-   0        0        0     4623 2023-05-21 15:22:46.000000 shinherpro-1.6.4/shinherpro.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      279 2023-05-21 15:22:46.000000 shinherpro-1.6.4/shinherpro.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-21 15:22:46.000000 shinherpro-1.6.4/shinherpro.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       62 2023-05-21 15:22:46.000000 shinherpro-1.6.4/shinherpro.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-05-21 15:22:46.000000 shinherpro-1.6.4/shinherpro.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-22 15:34:34.959704 shinherpro-1.6.5/
+-rw-rw-rw-   0        0        0     4623 2023-05-22 15:34:34.954297 shinherpro-1.6.5/PKG-INFO
+-rw-rw-rw-   0        0        0     4443 2023-05-21 09:21:34.000000 shinherpro-1.6.5/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-22 15:34:34.960202 shinherpro-1.6.5/setup.cfg
+-rw-rw-rw-   0        0        0      852 2023-05-22 12:54:15.000000 shinherpro-1.6.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-22 15:34:34.945370 shinherpro-1.6.5/shinherpro/
+-rw-rw-rw-   0        0        0    10375 2023-05-22 15:34:26.000000 shinherpro-1.6.5/shinherpro/TYAI.py
+-rw-rw-rw-   0        0        0        0 2023-05-22 15:34:31.000000 shinherpro-1.6.5/shinherpro/__init__.py
+-rw-rw-rw-   0        0        0     1225 2023-05-21 09:03:22.000000 shinherpro-1.6.5/shinherpro/chormeDriver.py
+-rw-rw-rw-   0        0        0     1186 2023-05-22 15:33:52.000000 shinherpro-1.6.5/shinherpro/serverLog.py
+-rw-rw-rw-   0        0        0     2127 2023-05-21 08:58:49.000000 shinherpro-1.6.5/shinherpro/vfcModel.py
+drwxrwxrwx   0        0        0        0 2023-05-22 15:34:34.953305 shinherpro-1.6.5/shinherpro.egg-info/
+-rw-rw-rw-   0        0        0     4623 2023-05-22 15:34:34.000000 shinherpro-1.6.5/shinherpro.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      303 2023-05-22 15:34:34.000000 shinherpro-1.6.5/shinherpro.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-22 15:34:34.000000 shinherpro-1.6.5/shinherpro.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       62 2023-05-22 15:34:34.000000 shinherpro-1.6.5/shinherpro.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-05-22 15:34:34.000000 shinherpro-1.6.5/shinherpro.egg-info/top_level.txt
```

### Comparing `shinherpro-1.6.4/PKG-INFO` & `shinherpro-1.6.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: shinherpro
-Version: 1.6.4
-Summary: shinher-pro 1.6.4
+Version: 1.6.5
+Summary: shinher-pro 1.6.5
 Author: Yihuan
 Author-email: ivan17.lai@gmail.com
 Description-Content-Type: text/markdown
 
 # Shinher-Pro V1.6.3
 
 ### 這個程式是一個自動化的成績查詢工具，它使用 Selenium 和 BeautifulSoup 套件來模擬網頁瀏覽和解析 HTML 內容，並使用 Keras 加載自訓練的 AI 模型進行圖形驗證碼自動辨識。它可以自動登入到支援的成績查詢網站，通常是欣河線上查詢系統，只需輸入帳號密碼，程序會自動操作到成績業面並返回成績，跳過原先繁雜的操作。
```

### Comparing `shinherpro-1.6.4/README.md` & `shinherpro-1.6.5/README.md`

 * *Files identical despite different names*

### Comparing `shinherpro-1.6.4/setup.py` & `shinherpro-1.6.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,16 +8,16 @@
     def run(self):
         print("\033[98m 正在安裝shinher-pro...")
         install.run(self)
         print("shinherpro安裝完成！ \033[0m")
 
 setup(
     name='shinherpro',
-    version='1.6.4',
-    description='shinher-pro 1.6.4',
+    version='1.6.5',
+    description='shinher-pro 1.6.5',
     author='Yihuan',
     author_email='ivan17.lai@gmail.com',
     packages=['shinherpro'],
     install_requires=[
         'selenium',
         'beautifulsoup4',
         'keras',
```

### Comparing `shinherpro-1.6.4/shinherpro/TYAI.py` & `shinherpro-1.6.5/shinherpro/TYAI.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,23 +15,29 @@
 import numpy as np
 import cv2
 import time
 import json
 import os
 from shinherpro import vfcModel
 from shinherpro import chormeDriver
+import sys
 
 
 ###################################################
 # V 1.6.4 By Yihuan Studio --> 2023/5/21/05:09:19
 
 #############################################
 #  vfcCode AI model 5.1  x4307 picture
 ##  image enhancement algorithm V1 By Sam
 
+RESET = "\033[0m"
+RED = "\033[31m"
+GREEN = "\033[32m"
+YELLOW = "\033[33m"
+
 def urlGet():
     return "https://sai.tyai.tyc.edu.tw/online/"
 
 def score_tolist(new_page_source):
     
     html = new_page_source
     soup = BeautifulSoup(html, 'html.parser')
@@ -69,26 +75,41 @@
         '平均': average_score,
         '排名': ranking,
         '科別排名': department_ranking
     }
 
     return result
 
+def logGenerate(start_time,result,vfcTry,vfcTryList):
+    end_time = time.time()
+    execution_time = end_time - start_time
+
+    new_log = [
+    {
+        'runTime': execution_time,
+        'VfcTry': vfcTry,
+        'vfcTryList': vfcTryList
+    }
+    ]
 
-def getGrades(username, password, driver, model,examname,LowConfidence=85):
+    result['log'] = new_log
+    return result
 
-    RESET = "\033[0m"
-    RED = "\033[31m"
-    GREEN = "\033[32m"
-    YELLOW = "\033[33m"
+def getGrades(username, password, driver, model,examname,LowConfidence=85,stepPrint=False):
 
+    if stepPrint == False :
+        sys.stdout = open(os.devnull, 'w')
+    
+    start_time = time.time()
     loginScess = False
-
+    
     while True:
         allConfidence = 0
+        vfcTry = 0
+        vfcTryList = []
         while allConfidence <= LowConfidence :
             vfc = ""
             while(True):
                 try:
                     captcha_element = driver.find_element(By.XPATH, '//img[@id="imgvcode"]')
                     break
                 except:
@@ -134,21 +155,22 @@
                 elif predicted_confidence < confidence_threshold_medium:
                     print(f"{YELLOW}驗證碼: {predicted_label} 置信度: {predicted_confidence} %{RESET}")
                 else:
                     print(f"{GREEN}驗證碼: {predicted_label} 置信度: {predicted_confidence} %{RESET}")
 
             allConfidence = confidence[0] * confidence[1] * confidence[2] * confidence[3] * 0.000001
             print("\033[33m 驗證碼影像辨識:" + str(vfc) + "  本次準確率:" + str(allConfidence) + " % \033[0m")
-
+            vfcTryList.append((vfc,allConfidence))
             if allConfidence <= LowConfidence :
                 driver.refresh()
         print("\033[36m 驗證碼準確率達標 \033[0m")
 
 
         vcode = vfc
+        vfcTry = vfcTry + 1
         # login
         username_element = driver.find_element(By.ID, 'Loginid')
         username_element.send_keys(username)
         password_element = driver.find_element(By.ID, 'LoginPwd')
         password_element.send_keys(password)
         vcode_element = driver.find_element(By.ID, 'vcode')
         vcode_element.send_keys(vcode)
@@ -157,22 +179,25 @@
 
         try:
             alert = Alert(driver)
             popup_text = alert.text
             print(popup_text)
             alert.dismiss()
             if popup_text == "帳號或密碼錯誤,請重新登入!":
-                return {'code':1,'reason':"帳號或密碼錯誤,請重新登入!"}
+                if stepPrint==False : sys.stdout = sys.__stdout__
+                return logGenerate(start_time,{'code':1,'reason':"帳號或密碼錯誤,請重新登入!"},vfcTry,vfcTryList)
             elif popup_text == "帳號登入失敗次數過多，請於15分鐘後再嘗試登入!!":
-                return {'code':2,'reason':"帳號登入失敗次數過多，請於15分鐘後再嘗試登入!!"}
+                if stepPrint==False : sys.stdout = sys.__stdout__
+                return logGenerate(start_time,{'code':2,'reason':"帳號登入失敗次數過多，請於15分鐘後再嘗試登入!!"},vfcTry,vfcTryList)
             elif popup_text == "驗證碼輸入錯誤，請重新輸入。":
                 print("驗證碼輸入錯誤,重新嘗試")
             else:
                 reason = popup_text
-                return {'code':3,'reason':reason}
+                if stepPrint==False : sys.stdout = sys.__stdout__
+                return logGenerate(start_time,{'code':3,'reason':reason},vfcTry,vfcTryList)
             
  
         except:
             print(f"{GREEN}密碼正確.{RESET}",end="")
             break
 
     print(f"{GREEN}驗證碼正確.{RESET}")
@@ -219,8 +244,13 @@
     new_page_source = driver.page_source
     # 成績表格分析
     result = score_tolist(new_page_source)
     loginScess = True
 
     driver.delete_all_cookies()
     driver.refresh()
-    return result
+
+    result = logGenerate( start_time,result,vfcTry,vfcTryList)
+
+
+    if stepPrint==False : sys.stdout = sys.__stdout__
+    return result
```

### Comparing `shinherpro-1.6.4/shinherpro/chormeDriver.py` & `shinherpro-1.6.5/shinherpro/chormeDriver.py`

 * *Files identical despite different names*

### Comparing `shinherpro-1.6.4/shinherpro/vfcModel.py` & `shinherpro-1.6.5/shinherpro/vfcModel.py`

 * *Files identical despite different names*

### Comparing `shinherpro-1.6.4/shinherpro.egg-info/PKG-INFO` & `shinherpro-1.6.5/shinherpro.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: shinherpro
-Version: 1.6.4
-Summary: shinher-pro 1.6.4
+Version: 1.6.5
+Summary: shinher-pro 1.6.5
 Author: Yihuan
 Author-email: ivan17.lai@gmail.com
 Description-Content-Type: text/markdown
 
 # Shinher-Pro V1.6.3
 
 ### 這個程式是一個自動化的成績查詢工具，它使用 Selenium 和 BeautifulSoup 套件來模擬網頁瀏覽和解析 HTML 內容，並使用 Keras 加載自訓練的 AI 模型進行圖形驗證碼自動辨識。它可以自動登入到支援的成績查詢網站，通常是欣河線上查詢系統，只需輸入帳號密碼，程序會自動操作到成績業面並返回成績，跳過原先繁雜的操作。
```

