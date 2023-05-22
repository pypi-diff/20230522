# Comparing `tmp/koios-api-1.0.10.2.tar.gz` & `tmp/koios-api-1.0.10.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "koios-api-1.0.10.2.tar", last modified: Fri May 19 08:41:21 2023, max compression
+gzip compressed data, was "koios-api-1.0.10.3.tar", last modified: Mon May 22 06:49:31 2023, max compression
```

## Comparing `koios-api-1.0.10.2.tar` & `koios-api-1.0.10.3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-05-19 08:41:21.159385 koios-api-1.0.10.2/
--rw-rw-r--   0 george    (1000) george    (1000)     1080 2023-04-22 10:04:11.000000 koios-api-1.0.10.2/LICENSE
--rw-rw-r--   0 george    (1000) george    (1000)   106197 2023-05-19 08:41:21.159385 koios-api-1.0.10.2/PKG-INFO
--rw-rw-r--   0 george    (1000) george    (1000)   105556 2023-05-19 07:45:13.000000 koios-api-1.0.10.2/README.md
--rw-rw-r--   0 george    (1000) george    (1000)      797 2023-05-19 08:38:22.000000 koios-api-1.0.10.2/pyproject.toml
--rw-rw-r--   0 george    (1000) george    (1000)       38 2023-05-19 08:41:21.159385 koios-api-1.0.10.2/setup.cfg
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-05-19 08:41:21.155384 koios-api-1.0.10.2/src/
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-05-19 08:41:21.159385 koios-api-1.0.10.2/src/koios_api/
--rw-rw-r--   0 george    (1000) george    (1000)     1393 2023-05-11 12:12:45.000000 koios-api-1.0.10.2/src/koios_api/__config__.py
--rw-rw-r--   0 george    (1000) george    (1000)      228 2022-10-13 07:47:20.000000 koios-api-1.0.10.2/src/koios_api/__init__.py
--rw-rw-r--   0 george    (1000) george    (1000)    10489 2023-05-11 12:03:05.000000 koios-api-1.0.10.2/src/koios_api/account.py
--rw-rw-r--   0 george    (1000) george    (1000)     5995 2023-05-18 15:33:57.000000 koios-api-1.0.10.2/src/koios_api/address.py
--rw-rw-r--   0 george    (1000) george    (1000)    16024 2023-05-11 13:26:52.000000 koios-api-1.0.10.2/src/koios_api/asset.py
--rw-rw-r--   0 george    (1000) george    (1000)     3177 2023-05-11 12:03:49.000000 koios-api-1.0.10.2/src/koios_api/block.py
--rw-rw-r--   0 george    (1000) george    (1000)     2690 2023-05-11 08:51:55.000000 koios-api-1.0.10.2/src/koios_api/epoch.py
--rw-rw-r--   0 george    (1000) george    (1000)     2514 2023-05-11 08:41:06.000000 koios-api-1.0.10.2/src/koios_api/network.py
--rw-rw-r--   0 george    (1000) george    (1000)    10428 2023-05-19 07:44:11.000000 koios-api-1.0.10.2/src/koios_api/pool.py
--rw-rw-r--   0 george    (1000) george    (1000)     3595 2023-05-11 12:04:31.000000 koios-api-1.0.10.2/src/koios_api/script.py
--rw-rw-r--   0 george    (1000) george    (1000)     5414 2023-05-11 12:04:23.000000 koios-api-1.0.10.2/src/koios_api/transactions.py
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-05-19 08:41:21.159385 koios-api-1.0.10.2/src/koios_api.egg-info/
--rw-rw-r--   0 george    (1000) george    (1000)   106197 2023-05-19 08:41:21.000000 koios-api-1.0.10.2/src/koios_api.egg-info/PKG-INFO
--rw-rw-r--   0 george    (1000) george    (1000)      490 2023-05-19 08:41:21.000000 koios-api-1.0.10.2/src/koios_api.egg-info/SOURCES.txt
--rw-rw-r--   0 george    (1000) george    (1000)        1 2023-05-19 08:41:21.000000 koios-api-1.0.10.2/src/koios_api.egg-info/dependency_links.txt
--rw-rw-r--   0 george    (1000) george    (1000)       17 2023-05-19 08:41:21.000000 koios-api-1.0.10.2/src/koios_api.egg-info/requires.txt
--rw-rw-r--   0 george    (1000) george    (1000)       16 2023-05-19 08:41:21.000000 koios-api-1.0.10.2/src/koios_api.egg-info/top_level.txt
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-05-22 06:49:31.777329 koios-api-1.0.10.3/
+-rw-rw-r--   0 george    (1000) george    (1000)     1080 2023-04-22 10:04:11.000000 koios-api-1.0.10.3/LICENSE
+-rw-rw-r--   0 george    (1000) george    (1000)   106449 2023-05-22 06:49:31.777329 koios-api-1.0.10.3/PKG-INFO
+-rw-rw-r--   0 george    (1000) george    (1000)   105808 2023-05-22 06:46:32.000000 koios-api-1.0.10.3/README.md
+-rw-rw-r--   0 george    (1000) george    (1000)      797 2023-05-22 06:41:10.000000 koios-api-1.0.10.3/pyproject.toml
+-rw-rw-r--   0 george    (1000) george    (1000)       38 2023-05-22 06:49:31.777329 koios-api-1.0.10.3/setup.cfg
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-05-22 06:49:31.777329 koios-api-1.0.10.3/src/
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-05-22 06:49:31.777329 koios-api-1.0.10.3/src/koios_api/
+-rw-rw-r--   0 george    (1000) george    (1000)     1393 2023-05-11 12:12:45.000000 koios-api-1.0.10.3/src/koios_api/__config__.py
+-rw-rw-r--   0 george    (1000) george    (1000)      228 2022-10-13 07:47:20.000000 koios-api-1.0.10.3/src/koios_api/__init__.py
+-rw-rw-r--   0 george    (1000) george    (1000)    10715 2023-05-22 04:51:43.000000 koios-api-1.0.10.3/src/koios_api/account.py
+-rw-rw-r--   0 george    (1000) george    (1000)     6164 2023-05-22 05:12:44.000000 koios-api-1.0.10.3/src/koios_api/address.py
+-rw-rw-r--   0 george    (1000) george    (1000)    16024 2023-05-11 13:26:52.000000 koios-api-1.0.10.3/src/koios_api/asset.py
+-rw-rw-r--   0 george    (1000) george    (1000)     3177 2023-05-11 12:03:49.000000 koios-api-1.0.10.3/src/koios_api/block.py
+-rw-rw-r--   0 george    (1000) george    (1000)     2690 2023-05-11 08:51:55.000000 koios-api-1.0.10.3/src/koios_api/epoch.py
+-rw-rw-r--   0 george    (1000) george    (1000)     2514 2023-05-11 08:41:06.000000 koios-api-1.0.10.3/src/koios_api/network.py
+-rw-rw-r--   0 george    (1000) george    (1000)    10428 2023-05-19 07:44:11.000000 koios-api-1.0.10.3/src/koios_api/pool.py
+-rw-rw-r--   0 george    (1000) george    (1000)     3595 2023-05-11 12:04:31.000000 koios-api-1.0.10.3/src/koios_api/script.py
+-rw-rw-r--   0 george    (1000) george    (1000)     5414 2023-05-11 12:04:23.000000 koios-api-1.0.10.3/src/koios_api/transactions.py
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-05-22 06:49:31.777329 koios-api-1.0.10.3/src/koios_api.egg-info/
+-rw-rw-r--   0 george    (1000) george    (1000)   106449 2023-05-22 06:49:31.000000 koios-api-1.0.10.3/src/koios_api.egg-info/PKG-INFO
+-rw-rw-r--   0 george    (1000) george    (1000)      490 2023-05-22 06:49:31.000000 koios-api-1.0.10.3/src/koios_api.egg-info/SOURCES.txt
+-rw-rw-r--   0 george    (1000) george    (1000)        1 2023-05-22 06:49:31.000000 koios-api-1.0.10.3/src/koios_api.egg-info/dependency_links.txt
+-rw-rw-r--   0 george    (1000) george    (1000)       17 2023-05-22 06:49:31.000000 koios-api-1.0.10.3/src/koios_api.egg-info/requires.txt
+-rw-rw-r--   0 george    (1000) george    (1000)       16 2023-05-22 06:49:31.000000 koios-api-1.0.10.3/src/koios_api.egg-info/top_level.txt
```

### Comparing `koios-api-1.0.10.2/LICENSE` & `koios-api-1.0.10.3/LICENSE`

 * *Files identical despite different names*

### Comparing `koios-api-1.0.10.2/PKG-INFO` & `koios-api-1.0.10.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: koios-api
-Version: 1.0.10.2
+Version: 1.0.10.3
 Summary: A python package for the Cardano Blockchain Koios API (https://api.koios.rest/)
 Author-email: APEX Stake Pool <cardanoapexpool@gmail.com>
 Project-URL: Homepage, https://github.com/cardano-apexpool/koios-api-python
 Project-URL: Bug Tracker, https://github.com/cardano-apexpool/koios-api-python/issues
 Keywords: koios,cardano,blockchain,REST,API
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -886,15 +886,17 @@
     ]
   }
 ]
 ```
 
 #### get_credential_txs
 Get the transaction hash list of input payment credential array, optionally filtering after specified block height (inclusive)<br>
-Parameters: Credential(s) as string (for one credential) or list (for multiple credentials)<br>
+Parameters: <br>
+Credential(s) as string (for one credential) or list (for multiple credentials)<br>
+After block height (optional): Only fetch information after specific block height<br> 
 Returns: The list of address information dictionaries<br>
 Example:<br>
 `credential_txs = get_credential_txs('dcc3fb415f1e0bf25bbabae6e261c61f85a1a23e4e063145b1efcc39')`<br>
 Example response:
 ```json
 [
   {
@@ -2368,15 +2370,18 @@
     ]
   }
 ]
 ```
 
 #### get_account_addresses
 Get all addresses associated with given staking accounts<br>
-Parameters: Stake address(es), as a string (for one address) or a list (for multiple addresses)<br>
+Parameters: <br>
+Stake address(es), as a string (for one address) or a list (for multiple addresses)<br>
+First Only boolean (optional): Only return the first result (default False)<br>
+Empty boolean (optional): Include zero quantity entries (default True)<br>
 Returns: The list of addresses dictionaries by account (stake address)<br>
 Example:<br>
 `account_addresses = get_account_addresses('stake1u8lhspu67x3jejzcfrh487rtu3hnm26cg0jsn0mgh2y6n9q9ve26z')`<br>
 Example response:
 ```json
 [
   {
```

### Comparing `koios-api-1.0.10.2/README.md` & `koios-api-1.0.10.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -871,15 +871,17 @@
     ]
   }
 ]
 ```
 
 #### get_credential_txs
 Get the transaction hash list of input payment credential array, optionally filtering after specified block height (inclusive)<br>
-Parameters: Credential(s) as string (for one credential) or list (for multiple credentials)<br>
+Parameters: <br>
+Credential(s) as string (for one credential) or list (for multiple credentials)<br>
+After block height (optional): Only fetch information after specific block height<br> 
 Returns: The list of address information dictionaries<br>
 Example:<br>
 `credential_txs = get_credential_txs('dcc3fb415f1e0bf25bbabae6e261c61f85a1a23e4e063145b1efcc39')`<br>
 Example response:
 ```json
 [
   {
@@ -2353,15 +2355,18 @@
     ]
   }
 ]
 ```
 
 #### get_account_addresses
 Get all addresses associated with given staking accounts<br>
-Parameters: Stake address(es), as a string (for one address) or a list (for multiple addresses)<br>
+Parameters: <br>
+Stake address(es), as a string (for one address) or a list (for multiple addresses)<br>
+First Only boolean (optional): Only return the first result (default False)<br>
+Empty boolean (optional): Include zero quantity entries (default True)<br>
 Returns: The list of addresses dictionaries by account (stake address)<br>
 Example:<br>
 `account_addresses = get_account_addresses('stake1u8lhspu67x3jejzcfrh487rtu3hnm26cg0jsn0mgh2y6n9q9ve26z')`<br>
 Example response:
 ```json
 [
   {
```

### Comparing `koios-api-1.0.10.2/pyproject.toml` & `koios-api-1.0.10.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ['setuptools>=61.0']
 build-backend = 'setuptools.build_meta'
 [project]
 name = "koios-api"
-version = "1.0.10.2"
+version = "1.0.10.3"
 authors = [
   { name="APEX Stake Pool", email="cardanoapexpool@gmail.com" },
 ]
 description = "A python package for the Cardano Blockchain Koios API (https://api.koios.rest/)"
 keywords = [
     "koios",
     "cardano",
```

### Comparing `koios-api-1.0.10.2/src/koios_api/__config__.py` & `koios-api-1.0.10.3/src/koios_api/__config__.py`

 * *Files identical despite different names*

### Comparing `koios-api-1.0.10.2/src/koios_api/account.py` & `koios-api-1.0.10.3/src/koios_api/account.py`

 * *Files 8% similar despite different names*

```diff
@@ -176,31 +176,35 @@
         except Exception as e:
             print(f"Exception in {inspect.getframeinfo(inspect.currentframe()).function}: {e}")
             sleep(SLEEP_TIME)
             print('retrying...')
     return resp
 
 
-def get_account_addresses(addr: [str, list]) -> list:
+def get_account_addresses(addr: [str, list], first_only: bool = False, empty: bool = True) -> list:
     """
     https://api.koios.rest/#post-/account_addresses
     Get all addresses associated with given staking accounts
     :param addr: Stake address(es), as a string (for one address) or a list (for multiple addresses)
+    :param first_only: Return only the first address if True
+    :param empty: Return also addresses with 0 balance if True
     :returns: The list of addresses maps by account (stake address)
     """
     url = API_BASE_URL + '/account_addresses'
     headers = {'Accept': 'application/json', 'Content-Type': 'application/json'}
-    stake_addresses = {}
+    parameters = {}
     if isinstance(addr, list):
-        stake_addresses['_stake_addresses'] = addr
+        parameters['_stake_addresses'] = addr
     else:
-        stake_addresses['_stake_addresses'] = [addr]
+        parameters['_stake_addresses'] = [addr]
+    parameters['_first_only'] = first_only
+    parameters['_empty'] = empty
     while True:
         try:
-            resp = json.loads(requests.post(url, headers=headers, data=json.dumps(stake_addresses)).text)
+            resp = json.loads(requests.post(url, headers=headers, data=json.dumps(parameters)).text)
             break
         except Exception as e:
             print(f"Exception in {inspect.getframeinfo(inspect.currentframe()).function}: {e}")
             sleep(SLEEP_TIME)
             print('retrying...')
     return resp
```

### Comparing `koios-api-1.0.10.2/src/koios_api/address.py` & `koios-api-1.0.10.3/src/koios_api/address.py`

 * *Files 12% similar despite different names*

```diff
@@ -128,31 +128,34 @@
         if len(resp) < API_RESP_COUNT:
             break
         else:
             offset += len(resp)
     return assets
 
 
-def get_credential_txs(cred: [str, list]) -> list:
+def get_credential_txs(cred: [str, list], after_block: int = 0) -> list:
     """
     https://api.koios.rest/#post-/credential_txs
     Get the transaction hash list of input payment credential array,
     optionally filtering after specified block height (inclusive)
     :param cred: Credential(s) as string (for one credential) or list (for multiple credentials)
+    :param after_block: Only fetch information after specific block height
     :returns: The list of address information maps
     """
     url = API_BASE_URL + '/credential_txs'
     headers = {'Accept': 'application/json', 'Content-Type': 'application/json'}
-    credentials = {}
+    parameters = {}
     if isinstance(cred, list):
-        credentials['_payment_credentials'] = cred
+        parameters['_payment_credentials'] = cred
     else:
-        credentials['_payment_credentials'] = [cred]
+        parameters['_payment_credentials'] = [cred]
+    if after_block:
+        parameters['_after_block_height'] = after_block
     while True:
         try:
-            resp = json.loads(requests.post(url, headers=headers, data=json.dumps(credentials)).text)
+            resp = json.loads(requests.post(url, headers=headers, data=json.dumps(parameters)).text)
             break
         except Exception as e:
             print(f"Exception in {inspect.getframeinfo(inspect.currentframe()).function}: {e}")
             sleep(SLEEP_TIME)
             print('retrying...')
     return resp
```

### Comparing `koios-api-1.0.10.2/src/koios_api/asset.py` & `koios-api-1.0.10.3/src/koios_api/asset.py`

 * *Files identical despite different names*

### Comparing `koios-api-1.0.10.2/src/koios_api/block.py` & `koios-api-1.0.10.3/src/koios_api/block.py`

 * *Files identical despite different names*

### Comparing `koios-api-1.0.10.2/src/koios_api/epoch.py` & `koios-api-1.0.10.3/src/koios_api/epoch.py`

 * *Files identical despite different names*

### Comparing `koios-api-1.0.10.2/src/koios_api/network.py` & `koios-api-1.0.10.3/src/koios_api/network.py`

 * *Files identical despite different names*

### Comparing `koios-api-1.0.10.2/src/koios_api/pool.py` & `koios-api-1.0.10.3/src/koios_api/pool.py`

 * *Files identical despite different names*

### Comparing `koios-api-1.0.10.2/src/koios_api/script.py` & `koios-api-1.0.10.3/src/koios_api/script.py`

 * *Files identical despite different names*

### Comparing `koios-api-1.0.10.2/src/koios_api/transactions.py` & `koios-api-1.0.10.3/src/koios_api/transactions.py`

 * *Files identical despite different names*

### Comparing `koios-api-1.0.10.2/src/koios_api.egg-info/PKG-INFO` & `koios-api-1.0.10.3/src/koios_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: koios-api
-Version: 1.0.10.2
+Version: 1.0.10.3
 Summary: A python package for the Cardano Blockchain Koios API (https://api.koios.rest/)
 Author-email: APEX Stake Pool <cardanoapexpool@gmail.com>
 Project-URL: Homepage, https://github.com/cardano-apexpool/koios-api-python
 Project-URL: Bug Tracker, https://github.com/cardano-apexpool/koios-api-python/issues
 Keywords: koios,cardano,blockchain,REST,API
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -886,15 +886,17 @@
     ]
   }
 ]
 ```
 
 #### get_credential_txs
 Get the transaction hash list of input payment credential array, optionally filtering after specified block height (inclusive)<br>
-Parameters: Credential(s) as string (for one credential) or list (for multiple credentials)<br>
+Parameters: <br>
+Credential(s) as string (for one credential) or list (for multiple credentials)<br>
+After block height (optional): Only fetch information after specific block height<br> 
 Returns: The list of address information dictionaries<br>
 Example:<br>
 `credential_txs = get_credential_txs('dcc3fb415f1e0bf25bbabae6e261c61f85a1a23e4e063145b1efcc39')`<br>
 Example response:
 ```json
 [
   {
@@ -2368,15 +2370,18 @@
     ]
   }
 ]
 ```
 
 #### get_account_addresses
 Get all addresses associated with given staking accounts<br>
-Parameters: Stake address(es), as a string (for one address) or a list (for multiple addresses)<br>
+Parameters: <br>
+Stake address(es), as a string (for one address) or a list (for multiple addresses)<br>
+First Only boolean (optional): Only return the first result (default False)<br>
+Empty boolean (optional): Include zero quantity entries (default True)<br>
 Returns: The list of addresses dictionaries by account (stake address)<br>
 Example:<br>
 `account_addresses = get_account_addresses('stake1u8lhspu67x3jejzcfrh487rtu3hnm26cg0jsn0mgh2y6n9q9ve26z')`<br>
 Example response:
 ```json
 [
   {
```

