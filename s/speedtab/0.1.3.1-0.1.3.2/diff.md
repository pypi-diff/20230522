# Comparing `tmp/speedtab-0.1.3.1.tar.gz` & `tmp/speedtab-0.1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "speedtab-0.1.3.1.tar", max compression
+gzip compressed data, was "speedtab-0.1.3.2.tar", max compression
```

## Comparing `speedtab-0.1.3.1.tar` & `speedtab-0.1.3.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      567 2023-05-19 11:17:12.096613 speedtab-0.1.3.1/pyproject.toml
--rw-r--r--   0        0        0      352 2022-09-07 08:00:08.177672 speedtab-0.1.3.1/speedtab/__init__.py
--rw-r--r--   0        0        0    45415 2023-05-19 11:33:22.981049 speedtab-0.1.3.1/speedtab/client.py
--rw-r--r--   0        0        0     6192 2023-05-19 11:01:11.239027 speedtab-0.1.3.1/speedtab/enums.py
--rw-r--r--   0        0        0     1730 2023-05-19 11:23:08.076916 speedtab-0.1.3.1/speedtab/formats.py
--rw-r--r--   0        0        0      783 2023-05-19 11:46:14.721776 speedtab-0.1.3.1/setup.py
--rw-r--r--   0        0        0      808 2023-05-19 11:46:14.721776 speedtab-0.1.3.1/PKG-INFO
+-rw-r--r--   0        0        0      567 2023-05-22 10:27:03.691219 speedtab-0.1.3.2/pyproject.toml
+-rw-r--r--   0        0        0      352 2022-09-07 08:00:08.177672 speedtab-0.1.3.2/speedtab/__init__.py
+-rw-r--r--   0        0        0    45532 2023-05-22 10:26:29.269245 speedtab-0.1.3.2/speedtab/client.py
+-rw-r--r--   0        0        0     6192 2023-05-19 11:01:11.239027 speedtab-0.1.3.2/speedtab/enums.py
+-rw-r--r--   0        0        0     1730 2023-05-19 11:23:08.076916 speedtab-0.1.3.2/speedtab/formats.py
+-rw-r--r--   0        0        0      783 2023-05-22 10:27:24.043638 speedtab-0.1.3.2/setup.py
+-rw-r--r--   0        0        0      808 2023-05-22 10:27:24.043638 speedtab-0.1.3.2/PKG-INFO
```

### Comparing `speedtab-0.1.3.1/pyproject.toml` & `speedtab-0.1.3.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "speedtab"
-version = "0.1.3.1"
+version = "0.1.3.2"
 description = "Convenient wrapper for working with Google Spreadsheets"
 authors = ["Bogdan Gergel <bogger147@gmail.com>"]
 license = "MIT"
 homepage = "https://github.com/BoggerSancho/SpeedTab-beta"
 repository = "https://github.com/BoggerSancho/SpeedTab-beta"
 
 [tool.poetry.dependencies]
```

### Comparing `speedtab-0.1.3.1/speedtab/client.py` & `speedtab-0.1.3.2/speedtab/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -884,15 +884,18 @@
 
     def __enter__(self):
         return self
 
     def __exit__(self, *args):
         self.exec()
 
-    def create_spreadsheet(self, title, sheets: list = ['Sheet1'], hide_grid_lines: Union[list, bool] = False):
+    def create_spreadsheet(self, title, sheets: list = None, hide_grid_lines: Union[list, bool] = False):
+        if sheets is None:
+            sheets = ['Sheet1']
+
         if isinstance(hide_grid_lines, bool):
             hide_grid_lines = [hide_grid_lines] * len(sheets)
 
         if len(hide_grid_lines) != len(sheets):
             raise NameError(f'Wrong list lenghts. Number of tabs: {len(sheets)}, number of grid options: {len(hide_grid_lines)}')
 
         ss = SpreedSheet(self.connect_v4.spreadsheets()
@@ -903,28 +906,27 @@
                                                                 'gridProperties': {'hideGridlines': grid}}}
                                                 for sheet_name, grid in zip(sheets, hide_grid_lines)]})
                          .execute().get('spreadsheetId'), token_path=self.token_path,
                          credentials=self.credentials, connect=self.connect_v4)
         self.list_of_spreadsheets.append(ss)
         return ss
 
-
-    def create_folder(self, folderName, parentID=None):
+    def create_folder(self, folder_name: str, parent_id: str = None):
         return self.connect_v3.files().create(body={
-            'name': folderName,
+            'name': folder_name,
             'mimeType': "application/vnd.google-apps.folder",
-            'parents': [parentID] if parentID else None,
+            'parents': [parent_id] if parent_id else None,
         }, supportsAllDrives=True).execute()['id']
 
     def rename_folder(self, fileId, name):
         self.connect_v3.files().update(body={
             'name': name,
         }, fileId=fileId, supportsAllDrives=True).execute()
 
-    def search_files(self, folder_id=None, trashed=False):
+    def search_files(self, folder_id: str = None, trashed: bool = False):
         files = []
         page_token = None
         while True:
             response = self.connect_v3.files().list(q=('trashed = true' if trashed else 'trashed = false') + (
                 f' and "{folder_id}" in parents' if folder_id else ''),
                                                        spaces='drive',
                                                        fields='nextPageToken, files(id, name, mimeType)',
@@ -937,31 +939,31 @@
             page_token = response.get('nextPageToken', None)
 
             if page_token is None:
                 break
 
         return files
 
-    def search_folder(self, folder_name, current_folder, mkdir=False):
+    def search_folder(self, folder_name, current_folder: str = None, mkdir: bool = False):
         folders = [file for file in self.search_files(current_folder) if
                    file.get('file_type') == 'folder' and file.get('name') == folder_name]
 
         if folders:
             return folders[0].get('id')
         elif mkdir:
             return self.create_folder(folder_name, current_folder)
         else:
             return None
 
-    def move_spreadsheet_to_folder(self, ss: SpreedSheet, real_folder_id):
+    def move_spreadsheet_to_folder(self, ss: SpreedSheet, real_folder_id: str):
         previous_parents = ','.join(self.connect_v3.files().get(fileId=ss.spreadsheet_id, fields='parents').execute().get('parents'))
         self.connect_v3.files().update(fileId=ss.spreadsheet_id, addParents=real_folder_id,
                                        removeParents=previous_parents, fields='id, parents').execute()
 
-    def share_spreadsheet_with_domain(self, ss: SpreedSheet, domain, role: ShareRole):
+    def share_spreadsheet_with_domain(self, ss: SpreedSheet, domain: str, role: ShareRole):
         self.connect_v3.permissions().create(**{
             'fileId': ss.spreadsheet_id,
             'body': {
                 'type': 'domain',
                 'role': role,
                 'domain': domain,
                 'allowFileDiscovery': True,
```

### Comparing `speedtab-0.1.3.1/speedtab/enums.py` & `speedtab-0.1.3.2/speedtab/enums.py`

 * *Files identical despite different names*

### Comparing `speedtab-0.1.3.1/speedtab/formats.py` & `speedtab-0.1.3.2/speedtab/formats.py`

 * *Files identical despite different names*

### Comparing `speedtab-0.1.3.1/setup.py` & `speedtab-0.1.3.2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 install_requires = \
 ['google-api-python-client>=2.58.0,<3.0.0',
  'google-auth-httplib2>=0.1.0,<0.2.0',
  'google-auth-oauthlib>=0.5.2,<0.6.0']
 
 setup_kwargs = {
     'name': 'speedtab',
-    'version': '0.1.3.1',
+    'version': '0.1.3.2',
     'description': 'Convenient wrapper for working with Google Spreadsheets',
     'long_description': None,
     'author': 'Bogdan Gergel',
     'author_email': 'bogger147@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/BoggerSancho/SpeedTab-beta',
```

### Comparing `speedtab-0.1.3.1/PKG-INFO` & `speedtab-0.1.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: speedtab
-Version: 0.1.3.1
+Version: 0.1.3.2
 Summary: Convenient wrapper for working with Google Spreadsheets
 Home-page: https://github.com/BoggerSancho/SpeedTab-beta
 License: MIT
 Author: Bogdan Gergel
 Author-email: bogger147@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

