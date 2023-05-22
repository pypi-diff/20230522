# Comparing `tmp/upbit-client-1.3.4.0.tar.gz` & `tmp/upbit-client-1.3.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "upbit-client-1.3.4.0.tar", last modified: Sun May 21 15:33:12 2023, max compression
+gzip compressed data, was "upbit-client-1.3.4.1.tar", last modified: Mon May 22 05:28:23 2023, max compression
```

## Comparing `upbit-client-1.3.4.0.tar` & `upbit-client-1.3.4.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 15:33:12.183725 upbit-client-1.3.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-05-21 15:33:00.000000 upbit-client-1.3.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3674 2023-05-21 15:33:12.183725 upbit-client-1.3.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2909 2023-05-21 15:33:00.000000 upbit-client-1.3.4.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-21 15:33:12.183725 upbit-client-1.3.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-05-21 15:33:00.000000 upbit-client-1.3.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 15:33:12.179725 upbit-client-1.3.4.0/upbit/
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-05-21 15:33:00.000000 upbit-client-1.3.4.0/upbit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2881 2023-05-21 15:33:00.000000 upbit-client-1.3.4.0/upbit/authentication.py
--rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-05-21 15:33:00.000000 upbit-client-1.3.4.0/upbit/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    24115 2023-05-21 15:33:00.000000 upbit-client-1.3.4.0/upbit/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-05-21 15:33:00.000000 upbit-client-1.3.4.0/upbit/pkginfo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-05-21 15:33:00.000000 upbit-client-1.3.4.0/upbit/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5053 2023-05-21 15:33:00.000000 upbit-client-1.3.4.0/upbit/websocket.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 15:33:12.183725 upbit-client-1.3.4.0/upbit_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3674 2023-05-21 15:33:12.000000 upbit-client-1.3.4.0/upbit_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-05-21 15:33:12.000000 upbit-client-1.3.4.0/upbit_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 15:33:12.000000 upbit-client-1.3.4.0/upbit_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-21 15:33:12.000000 upbit-client-1.3.4.0/upbit_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-21 15:33:12.000000 upbit-client-1.3.4.0/upbit_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 05:28:23.298618 upbit-client-1.3.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-05-22 05:27:56.000000 upbit-client-1.3.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3674 2023-05-22 05:28:23.298618 upbit-client-1.3.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2909 2023-05-22 05:27:56.000000 upbit-client-1.3.4.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-22 05:28:23.298618 upbit-client-1.3.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-05-22 05:27:56.000000 upbit-client-1.3.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 05:28:23.298618 upbit-client-1.3.4.1/upbit/
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-05-22 05:27:56.000000 upbit-client-1.3.4.1/upbit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2881 2023-05-22 05:27:56.000000 upbit-client-1.3.4.1/upbit/authentication.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-05-22 05:27:56.000000 upbit-client-1.3.4.1/upbit/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24309 2023-05-22 05:27:56.000000 upbit-client-1.3.4.1/upbit/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-05-22 05:27:56.000000 upbit-client-1.3.4.1/upbit/pkginfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-05-22 05:27:56.000000 upbit-client-1.3.4.1/upbit/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5053 2023-05-22 05:27:56.000000 upbit-client-1.3.4.1/upbit/websocket.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 05:28:23.298618 upbit-client-1.3.4.1/upbit_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3674 2023-05-22 05:28:23.000000 upbit-client-1.3.4.1/upbit_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-05-22 05:28:23.000000 upbit-client-1.3.4.1/upbit_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 05:28:23.000000 upbit-client-1.3.4.1/upbit_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-22 05:28:23.000000 upbit-client-1.3.4.1/upbit_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-22 05:28:23.000000 upbit-client-1.3.4.1/upbit_client.egg-info/top_level.txt
```

### Comparing `upbit-client-1.3.4.0/LICENSE` & `upbit-client-1.3.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `upbit-client-1.3.4.0/PKG-INFO` & `upbit-client-1.3.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: upbit-client
-Version: 1.3.4.0
+Version: 1.3.4.1
 Summary: Upbit OPEN API Client
 Home-page: https://github.com/uJhin/upbit-client
 Download-URL: https://github.com/uJhin/upbit-client/releases
 Author: ujhin
 Author-email: ujhin942@gmail.com
 License: MIT License
 Keywords: Upbit,upbit,upbit-client,Upbit-Client,Upbit_client,Upbit-api-connector,upbit-api-connector,Upbit_api_connector,upbit_api_connector
```

### Comparing `upbit-client-1.3.4.0/README.rst` & `upbit-client-1.3.4.1/README.rst`

 * *Files identical despite different names*

### Comparing `upbit-client-1.3.4.0/setup.py` & `upbit-client-1.3.4.1/setup.py`

 * *Files identical despite different names*

### Comparing `upbit-client-1.3.4.0/upbit/authentication.py` & `upbit-client-1.3.4.1/upbit/authentication.py`

 * *Files identical despite different names*

### Comparing `upbit-client-1.3.4.0/upbit/client.py` & `upbit-client-1.3.4.1/upbit/client.py`

 * *Files identical despite different names*

### Comparing `upbit-client-1.3.4.0/upbit/models.py` & `upbit-client-1.3.4.1/upbit/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -710,14 +710,19 @@
         """
         [POST] 원화 출금하기
 
         ## 원화 출금을 요청한다. 등록된 출금 계좌로 출금된다.
 
         :param amount: 출금 원화 수량
         :type amount: str
+        
+        :param two_factor_type: 2차 인증 수단 (optional)
+        - kakao_pay: 카카오페이 인증 (default)
+        - naver: 네이버 인증
+        :type two_factor_type: str
         """
 
         future = self.__client.Withdraw.Withdraw_krw(**kwargs)
         return HTTPFutureExtractor.future_extraction(future)
 
     def Withdraw_coin_addresses(self, **kwargs) -> dict:
         """
```

### Comparing `upbit-client-1.3.4.0/upbit/pkginfo.py` & `upbit-client-1.3.4.1/upbit/pkginfo.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     versions = data["releases"].keys()
     return sorted(versions, key=LooseVersion, reverse=True)
 
 
 PACKAGE_NAME     = "upbit-client"
 
 OPEN_API_VERSION = "1.3.4"
-CURRENT_VERSION  = OPEN_API_VERSION+".0"
+CURRENT_VERSION  = OPEN_API_VERSION+".1"
 
 RELEASED_VERSION = _get_versions(PACKAGE_NAME)
 LATEST_VERSION   = RELEASED_VERSION[0]
 
 
 if LATEST_VERSION != CURRENT_VERSION:
     logging.basicConfig(format="[%(levelname)s] %(message)s")
```

### Comparing `upbit-client-1.3.4.0/upbit/utils.py` & `upbit-client-1.3.4.1/upbit/utils.py`

 * *Files identical despite different names*

### Comparing `upbit-client-1.3.4.0/upbit/websocket.py` & `upbit-client-1.3.4.1/upbit/websocket.py`

 * *Files identical despite different names*

### Comparing `upbit-client-1.3.4.0/upbit_client.egg-info/PKG-INFO` & `upbit-client-1.3.4.1/upbit_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: upbit-client
-Version: 1.3.4.0
+Version: 1.3.4.1
 Summary: Upbit OPEN API Client
 Home-page: https://github.com/uJhin/upbit-client
 Download-URL: https://github.com/uJhin/upbit-client/releases
 Author: ujhin
 Author-email: ujhin942@gmail.com
 License: MIT License
 Keywords: Upbit,upbit,upbit-client,Upbit-Client,Upbit_client,Upbit-api-connector,upbit-api-connector,Upbit_api_connector,upbit_api_connector
```

