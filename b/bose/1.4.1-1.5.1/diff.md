# Comparing `tmp/bose-1.4.1.tar.gz` & `tmp/bose-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bose-1.4.1.tar", last modified: Sat May 13 13:34:39 2023, max compression
+gzip compressed data, was "bose-1.5.1.tar", last modified: Mon May 22 11:20:43 2023, max compression
```

## Comparing `bose-1.4.1.tar` & `bose-1.5.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-05-13 13:34:39.800462 bose-1.4.1/
--rw-rw-rw-   0        0        0     1460 2023-05-13 13:34:39.801461 bose-1.4.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-13 13:34:39.800462 bose-1.4.1/bose/
--rw-rw-rw-   0        0        0      340 2023-05-13 11:28:45.126433 bose-1.4.1/bose/__init__.py
--rw-rw-rw-   0        0        0     3657 2023-05-10 09:24:37.900794 bose-1.4.1/bose/base_data.py
--rw-rw-rw-   0        0        0     5228 2023-05-13 11:28:17.686088 bose-1.4.1/bose/base_task.py
--rw-rw-rw-   0        0        0     9026 2023-05-13 11:28:17.686088 bose-1.4.1/bose/boss_driver.py
--rw-rw-rw-   0        0        0     9038 2023-05-13 11:28:17.686088 bose-1.4.1/bose/boss_undetected_driver.py
--rw-rw-rw-   0        0        0     7295 2023-05-13 11:28:17.686088 bose-1.4.1/bose/create_driver.py
--rw-rw-rw-   0        0        0     1391 2023-05-10 10:36:24.892682 bose-1.4.1/bose/download_driver.py
--rw-rw-rw-   0        0        0     2901 2023-05-13 11:28:17.687091 bose-1.4.1/bose/local_storage.py
--rw-rw-rw-   0        0        0     1728 2023-05-09 15:44:16.700182 bose-1.4.1/bose/local_storage_driver.py
--rw-rw-rw-   0        0        0       80 2023-05-09 06:14:41.273740 bose-1.4.1/bose/opponent.py
--rw-rw-rw-   0        0        0     3169 2023-05-13 11:28:17.687091 bose-1.4.1/bose/output.py
--rw-rw-rw-   0        0        0     1650 2023-05-13 11:28:17.687091 bose-1.4.1/bose/task_info.py
--rw-rw-rw-   0        0        0     3977 2023-05-13 13:31:08.141431 bose-1.4.1/bose/temp_mail.py
--rw-rw-rw-   0        0        0     7361 2023-05-10 09:24:37.900794 bose-1.4.1/bose/user_agent.py
--rw-rw-rw-   0        0        0     6050 2023-05-10 10:34:20.625623 bose-1.4.1/bose/utils.py
--rw-rw-rw-   0        0        0       60 2023-05-09 06:15:17.436327 bose-1.4.1/bose/wait.py
--rw-rw-rw-   0        0        0     1203 2023-05-09 07:09:28.075948 bose-1.4.1/bose/window_size.py
--rw-rw-rw-   0        0        0       40 2022-10-28 11:26:12.145036 bose-1.4.1/setup.cfg
--rw-rw-rw-   0        0        0     2328 2023-05-13 13:34:15.193389 bose-1.4.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-22 11:20:43.373329 bose-1.5.1/
+-rw-rw-rw-   0        0        0     1460 2023-05-22 11:20:43.373329 bose-1.5.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-22 11:20:43.373329 bose-1.5.1/bose/
+-rw-rw-rw-   0        0        0      340 2023-05-13 11:28:45.126433 bose-1.5.1/bose/__init__.py
+-rw-rw-rw-   0        0        0     3657 2023-05-10 09:24:37.900794 bose-1.5.1/bose/base_data.py
+-rw-rw-rw-   0        0        0     4990 2023-05-18 07:22:46.924306 bose-1.5.1/bose/base_task.py
+-rw-rw-rw-   0        0        0     9037 2023-05-13 23:12:33.521981 bose-1.5.1/bose/boss_driver.py
+-rw-rw-rw-   0        0        0     9049 2023-05-22 11:19:35.255308 bose-1.5.1/bose/boss_undetected_driver.py
+-rw-rw-rw-   0        0        0     7295 2023-05-13 11:28:17.686088 bose-1.5.1/bose/create_driver.py
+-rw-rw-rw-   0        0        0     1391 2023-05-10 10:36:24.892682 bose-1.5.1/bose/download_driver.py
+-rw-rw-rw-   0        0        0     3185 2023-05-18 07:50:25.651854 bose-1.5.1/bose/local_storage.py
+-rw-rw-rw-   0        0        0     1728 2023-05-09 15:44:16.700182 bose-1.5.1/bose/local_storage_driver.py
+-rw-rw-rw-   0        0        0       80 2023-05-09 06:14:41.273740 bose-1.5.1/bose/opponent.py
+-rw-rw-rw-   0        0        0     3187 2023-05-15 09:11:34.318135 bose-1.5.1/bose/output.py
+-rw-rw-rw-   0        0        0     1650 2023-05-13 11:28:17.687091 bose-1.5.1/bose/task_info.py
+-rw-rw-rw-   0        0        0     3977 2023-05-13 13:31:08.141431 bose-1.5.1/bose/temp_mail.py
+-rw-rw-rw-   0        0        0     7361 2023-05-10 09:24:37.900794 bose-1.5.1/bose/user_agent.py
+-rw-rw-rw-   0        0        0     6050 2023-05-10 10:34:20.625623 bose-1.5.1/bose/utils.py
+-rw-rw-rw-   0        0        0       60 2023-05-09 06:15:17.436327 bose-1.5.1/bose/wait.py
+-rw-rw-rw-   0        0        0     1203 2023-05-09 07:09:28.075948 bose-1.5.1/bose/window_size.py
+-rw-rw-rw-   0        0        0       40 2022-10-28 11:26:12.145036 bose-1.5.1/setup.cfg
+-rw-rw-rw-   0        0        0     2328 2023-05-22 11:19:06.029461 bose-1.5.1/setup.py
```

### Comparing `bose-1.4.1/PKG-INFO` & `bose-1.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: bose
-Version: 1.4.1
+Version: 1.5.1
 Summary: The Ultimate Web Scraping Framework
 Home-page: UNKNOWN
 Author: Chetan Jain
 Author-email: chetan@omkar.cloud
 License: MIT
 Description: # Bose - The Ultimate Web Scraping Framework!
```

### Comparing `bose-1.4.1/bose/base_data.py` & `bose-1.5.1/bose/base_data.py`

 * *Files identical despite different names*

### Comparing `bose-1.4.1/bose/base_task.py` & `bose-1.5.1/bose/base_task.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,18 +27,14 @@
     from .download_driver import download_driver
     download_driver()
     
 class BaseTask():
     def __init__(self):
         self.task_path = None
         self.task_id = None        
-        # if LocalStorage.get_item('is_driver_downloaded',  False) == False:
-        #   print('Downloading Driver in build/ directory.')
-        #   _download_driver()
-        #   LocalStorage.set_item('is_driver_downloaded',  True)
 
 
     browser_config = BrowserConfig()
 
     def get_browser_config(self):
         return self.browser_config
```

### Comparing `bose-1.4.1/bose/boss_driver.py` & `bose-1.5.1/bose/boss_driver.py`

 * *Files 0% similar despite different names*

```diff
@@ -164,26 +164,26 @@
         storage = LocalStorage(self)
         for key in local_storage:
             storage.set_item(key, local_storage[key])
 
     def add_cookies_and_local_storage_dict(self, site_data):
         cookies = site_data["cookies"]
         local_storage = site_data["local_storage"]
-        self.add_cookies(cookies)
-        self.add_local_storage(local_storage)
+        self.add_cookies_dict(cookies)
+        self.add_local_storage_dict(local_storage)
 
     def delete_cookies_dict(self):
         self.delete_all_cookies()
 
     def delete_local_storage_dict(self):
         self.execute_script("window.localStorage.clear();")
         self.execute_script("window.sessionStorage.clear();")
 
     def delete_cookies_and_local_storage_dict(self):
-        self.delete_all_cookies()
+        self.delete_cookies_dict()
         self.delete_local_storage_dict()
 
     def organic_get(self, link, wait=None):
         self.get("https://www.google.com/")
         self.get_by_current_page_referrer(link, wait)
 
     def get_google(self):
```

### Comparing `bose-1.4.1/bose/boss_undetected_driver.py` & `bose-1.5.1/bose/boss_undetected_driver.py`

 * *Files 2% similar despite different names*

```diff
@@ -164,26 +164,26 @@
         storage = LocalStorage(self)
         for key in local_storage:
             storage.set_item(key, local_storage[key])
 
     def add_cookies_and_local_storage_dict(self, site_data):
         cookies = site_data["cookies"]
         local_storage = site_data["local_storage"]
-        self.add_cookies(cookies)
-        self.add_local_storage(local_storage)
+        self.add_cookies_dict(cookies)
+        self.add_local_storage_dict(local_storage)
 
     def delete_cookies_dict(self):
         self.delete_all_cookies()
 
     def delete_local_storage_dict(self):
         self.execute_script("window.localStorage.clear();")
         self.execute_script("window.sessionStorage.clear();")
 
     def delete_cookies_and_local_storage_dict(self):
-        self.delete_all_cookies()
+        self.delete_cookies_dict()
         self.delete_local_storage_dict()
 
     def organic_get(self, link, wait=None):
         self.get("https://www.google.com/")
         self.get_by_current_page_referrer(link, wait)
 
     def get_google(self):
```

### Comparing `bose-1.4.1/bose/create_driver.py` & `bose-1.5.1/bose/create_driver.py`

 * *Files identical despite different names*

### Comparing `bose-1.4.1/bose/download_driver.py` & `bose-1.5.1/bose/download_driver.py`

 * *Files identical despite different names*

### Comparing `bose-1.4.1/bose/local_storage.py` & `bose-1.5.1/bose/local_storage.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,32 +22,39 @@
         self.raise_dummy_exception()
 
     def clear(self) -> None:
         self.raise_dummy_exception()
 
 class JSONStorageBackend(BasicStorageBackend):
     def __init__(self) -> None:
+        self.refresh()
+
+    def refresh(self):
         self.json_path = relative_path( "local_storage.json", 0)
         self.json_data = {}
 
         if not os.path.isfile(self.json_path):
             self.commit_to_disk()
 
         with open(self.json_path, "r") as json_file:
             self.json_data = json.load(json_file)
         
     def commit_to_disk(self):
         with open(self.json_path, "w") as json_file:
-            json.dump(self.json_data, json_file)
+            json.dump(self.json_data, json_file, indent=4)
 
     def get_item(self, key: str, default = None) -> str:
         if key in self.json_data:
             return self.json_data[key]
         return default
 
+
+    def items(self):
+        return self.json_data
+
     def set_item(self, key: str, value: any) -> None:
         self.json_data[key] = value
         self.commit_to_disk()
 
     def remove_item(self, key: str) -> None: 
         if key in self.json_data:
             self.json_data.pop(key)
@@ -72,26 +79,33 @@
         self.json_data = {}
         self.commit_to_disk()
     
 class _LocalStorage:
     def __init__(self) -> None:
         self.storage_backend_instance = JSONStorageBackend()
 
+    def refresh(self) -> None:
+        self.storage_backend_instance.refresh()
+    
     def get_item(self, item: str, default = None) -> any:
         return self.storage_backend_instance.get_item(item, default)
 
     def set_item(self, item: str, value: any) -> None:
         self.storage_backend_instance.set_item(item, value)
 
     def remove_item(self, item: str) -> None:
         self.storage_backend_instance.remove_item(item)
 
     def clear(self):
         self.storage_backend_instance.clear()
 
+    def items(self):
+        return self.storage_backend_instance.items()
+
+
     # def get_new_number(self):
     #     return self.storage_backend_instance.get_new_number()
 
 LocalStorage = _LocalStorage()
 
 if __name__ == "__main__":
     t = _LocalStorage()
```

### Comparing `bose-1.4.1/bose/local_storage_driver.py` & `bose-1.5.1/bose/local_storage_driver.py`

 * *Files identical despite different names*

### Comparing `bose-1.4.1/bose/output.py` & `bose-1.5.1/bose/output.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 
         if not filename.startswith("output/"):
             filename = "output/" +  filename
 
         if not filename.endswith(".csv"):
             filename = filename + ".csv"
 
-        with open(filename, 'w', newline='') as csvfile:
+        with open(filename, 'w', newline='', encoding='utf-8') as csvfile:
             fieldnames = data[0].keys()  # get the fieldnames from the first dictionary
             writer = csv.DictWriter(csvfile, fieldnames=fieldnames)
             writer.writeheader()  # write the header row
             writer.writerows(data)  # write each row of data
         print(f"View written CSV file at {filename}")        
     def write_xlsx(data, filename):
         """
```

### Comparing `bose-1.4.1/bose/task_info.py` & `bose-1.5.1/bose/task_info.py`

 * *Files identical despite different names*

### Comparing `bose-1.4.1/bose/temp_mail.py` & `bose-1.5.1/bose/temp_mail.py`

 * *Files identical despite different names*

### Comparing `bose-1.4.1/bose/user_agent.py` & `bose-1.5.1/bose/user_agent.py`

 * *Files identical despite different names*

### Comparing `bose-1.4.1/bose/utils.py` & `bose-1.5.1/bose/utils.py`

 * *Files identical despite different names*

### Comparing `bose-1.4.1/bose/window_size.py` & `bose-1.5.1/bose/window_size.py`

 * *Files identical despite different names*

### Comparing `bose-1.4.1/setup.py` & `bose-1.5.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     except:
       return None
     
 
 setup(
     name='bose',
     packages=['bose'],
-    version='1.4.1',
+    version='1.5.1',
     license='MIT',
     project_urls={
         "Documentation": "https://omkar.cloud/bose/docs/",
         "Source": "https://github.com/omkarcloud/boss",
         "Tracker": "https://github.com/omkarcloud/boss/issues",
     },
```

