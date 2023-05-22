# Comparing `tmp/pyrc-python-utils-0.0.1.tar.gz` & `tmp/pyrc-python-utils-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrc-python-utils-0.0.1.tar", last modified: Thu May 11 20:42:21 2023, max compression
+gzip compressed data, was "pyrc-python-utils-0.0.2.tar", last modified: Mon May 22 19:35:44 2023, max compression
```

## Comparing `pyrc-python-utils-0.0.1.tar` & `pyrc-python-utils-0.0.2.tar`

### file list

```diff
@@ -1,20 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-05-11 20:42:21.774668 pyrc-python-utils-0.0.1/
--rw-rw-rw-   0        0        0     1085 2023-05-10 20:22:54.000000 pyrc-python-utils-0.0.1/LICENSE
--rw-rw-rw-   0        0        0       57 2023-05-10 20:22:54.000000 pyrc-python-utils-0.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0      200 2023-05-11 20:42:21.773667 pyrc-python-utils-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       63 2023-05-10 20:22:54.000000 pyrc-python-utils-0.0.1/README.md
--rw-rw-rw-   0        0        0       42 2023-05-11 20:42:21.774668 pyrc-python-utils-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      359 2023-05-11 20:28:07.000000 pyrc-python-utils-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-11 20:42:21.761155 pyrc-python-utils-0.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-05-11 20:42:21.769664 pyrc-python-utils-0.0.1/src/pyrc_python_utils/
--rw-rw-rw-   0        0        0        0 2023-05-11 02:33:58.000000 pyrc-python-utils-0.0.1/src/pyrc_python_utils/__init__.py
--rw-rw-rw-   0        0        0      503 2023-05-11 02:33:58.000000 pyrc-python-utils-0.0.1/src/pyrc_python_utils/util_datetime.py
--rw-rw-rw-   0        0        0     3409 2023-05-11 02:33:58.000000 pyrc-python-utils-0.0.1/src/pyrc_python_utils/util_exchange.py
--rw-rw-rw-   0        0        0      229 2023-05-11 02:33:58.000000 pyrc-python-utils-0.0.1/src/pyrc_python_utils/util_file.py
--rw-rw-rw-   0        0        0    10020 2023-05-11 02:33:58.000000 pyrc-python-utils-0.0.1/src/pyrc_python_utils/util_sftp.py
--rw-rw-rw-   0        0        0     4408 2023-05-11 02:33:58.000000 pyrc-python-utils-0.0.1/src/pyrc_python_utils/util_sharepoint.py
-drwxrwxrwx   0        0        0        0 2023-05-11 20:42:21.772667 pyrc-python-utils-0.0.1/src/pyrc_python_utils.egg-info/
--rw-rw-rw-   0        0        0      200 2023-05-11 20:42:21.000000 pyrc-python-utils-0.0.1/src/pyrc_python_utils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      441 2023-05-11 20:42:21.000000 pyrc-python-utils-0.0.1/src/pyrc_python_utils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-11 20:42:21.000000 pyrc-python-utils-0.0.1/src/pyrc_python_utils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2023-05-11 20:42:21.000000 pyrc-python-utils-0.0.1/src/pyrc_python_utils.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-22 19:35:44.669543 pyrc-python-utils-0.0.2/
+-rw-rw-rw-   0        0        0     1085 2023-05-22 19:25:35.000000 pyrc-python-utils-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0       57 2023-05-22 19:25:35.000000 pyrc-python-utils-0.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0      460 2023-05-22 19:35:44.668543 pyrc-python-utils-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       63 2023-05-06 11:45:56.000000 pyrc-python-utils-0.0.2/README.md
+-rw-rw-rw-   0        0        0      630 2023-05-22 19:34:17.000000 pyrc-python-utils-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-22 19:35:44.669543 pyrc-python-utils-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      394 2023-05-22 19:30:49.000000 pyrc-python-utils-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-22 19:35:44.633543 pyrc-python-utils-0.0.2/src/
+drwxrwxrwx   0        0        0        0 2023-05-22 19:35:44.655543 pyrc-python-utils-0.0.2/src/pyrc_python_utils/
+-rw-rw-rw-   0        0        0        0 2023-05-22 19:25:35.000000 pyrc-python-utils-0.0.2/src/pyrc_python_utils/__init__.py
+-rw-rw-rw-   0        0        0     1153 2023-05-22 19:25:35.000000 pyrc-python-utils-0.0.2/src/pyrc_python_utils/util_datetime.py
+-rw-rw-rw-   0        0        0     5730 2023-05-22 19:25:35.000000 pyrc-python-utils-0.0.2/src/pyrc_python_utils/util_exchange.py
+-rw-rw-rw-   0        0        0      229 2023-05-22 19:25:35.000000 pyrc-python-utils-0.0.2/src/pyrc_python_utils/util_file.py
+-rw-rw-rw-   0        0        0     1352 2023-05-22 19:25:35.000000 pyrc-python-utils-0.0.2/src/pyrc_python_utils/util_ms_teams.py
+-rw-rw-rw-   0        0        0    28193 2023-05-22 19:25:35.000000 pyrc-python-utils-0.0.2/src/pyrc_python_utils/util_sftp.py
+-rw-rw-rw-   0        0        0     6416 2023-05-22 19:25:35.000000 pyrc-python-utils-0.0.2/src/pyrc_python_utils/util_sharepoint.py
+drwxrwxrwx   0        0        0        0 2023-05-22 19:35:44.666543 pyrc-python-utils-0.0.2/src/pyrc_python_utils.egg-info/
+-rw-rw-rw-   0        0        0      460 2023-05-22 19:35:44.000000 pyrc-python-utils-0.0.2/src/pyrc_python_utils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      539 2023-05-22 19:35:44.000000 pyrc-python-utils-0.0.2/src/pyrc_python_utils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-22 19:35:44.000000 pyrc-python-utils-0.0.2/src/pyrc_python_utils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2023-05-22 19:35:44.000000 pyrc-python-utils-0.0.2/src/pyrc_python_utils.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-05-22 19:35:44.000000 pyrc-python-utils-0.0.2/src/pyrc_python_utils.egg-info/top_level.txt
```

### Comparing `pyrc-python-utils-0.0.1/LICENSE` & `pyrc-python-utils-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyrc-python-utils-0.0.1/src/pyrc_python_utils/util_sharepoint.py` & `pyrc-python-utils-0.0.2/src/pyrc_python_utils/util_sharepoint.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,39 +1,76 @@
 # A SharePoint convenience wrapper around python-o365 library - https://github.com/O365/python-o365
 # Source reference
 #   https://github.com/O365/python-o365/blob/master/O365/sharepoint.py
 # See examples/sharepoint folder for usage scenarios
 
 import os
+from multiprocessing import AuthenticationError
 from pathlib import Path
+from typing import Tuple
 
 from O365 import Account
 from O365.drive import Drive, Folder
 from O365.sharepoint import Sharepoint, Site
 
 
 def get_sharepoint(client_id: str, client_secret: str, tenant_id: str) -> Sharepoint:
-    credentials = (client_id, client_secret)
+    """
+    Authenticates and retrieves a SharePoint instance.
 
-    account = Account(credentials, auth_flow_type='credentials', tenant_id=tenant_id)
-    account.authenticate()
-
-    return account.sharepoint()
+    :param client_id: The client ID for authentication.
+    :type client_id: str
+    :param client_secret: The client secret for authentication.
+    :type client_secret: str
+    :param tenant_id: The tenant ID for the SharePoint account.
+    :type tenant_id: str
+    :returns: An authenticated SharePoint instance.
+    :rtype: Sharepoint
+    :raises TypeError: If any of the inputs are not strings.
+    :raises AuthenticationError: If there is an issue with authentication.
+
+    """
+    # Type checking
+    if not all(isinstance(i, str) for i in [client_id, client_secret, tenant_id]):
+        raise TypeError("All inputs must be strings.")
+
+    try:
+        credentials: Tuple[str, str] = (client_id, client_secret)
+
+        account = Account(credentials, auth_flow_type='credentials', tenant_id=tenant_id)
+        account.authenticate()
+
+        return account.sharepoint()
+    except Exception as e:
+        raise AuthenticationError("There was an issue with authentication.") from e
 
 
 def get_site_from_sharepoint(sharepoint: Sharepoint, host: str, site_name: str) -> Site:
     # The get_site call expects the spaces to be stripped out of name for lookup purposes
     return sharepoint.get_site(host, 'sites/' + site_name.replace(" ", ""))
 
 
 def get_document_library_from_site(site: Site, document_library_name: str) -> Drive or None:
+    """
+    Searches for a specific document library in a given SharePoint site.
+
+    :param site: The SharePoint site to search in.
+    :type site: Site
+    :param document_library_name: The name of the document library to search for.
+    :type document_library_name: str
+    :returns: The found document library if it exists, else None.
+    :rtype: Drive or None
+    """
+    # Iterate over document libraries in the site
     for doc_lib in site.list_document_libraries():
+        # Return the document library if the name matches
         if doc_lib.name == document_library_name:
             return doc_lib
 
+    # Return None if no matching document library is found
     return None
 
 
 def get_document_library(client_id: str, client_secret: str, tenant_id: str, host: str, site_name: str,
                          document_library_name: str) -> Drive or None:
     sharepoint = get_sharepoint(client_id, client_secret, tenant_id)
     site = get_site_from_sharepoint(sharepoint, host, site_name)
@@ -80,24 +117,34 @@
 def create_folder(document_library: Drive, parent_folder_path: str or Path, name: str) -> Folder:
     # Based on path from doc library, create a folder given a parent path and folder name
     folder = get_folder(document_library, parent_folder_path)
     return create_child_folder(folder, name)
 
 
 def create_child_folder(parent_folder: Folder or Drive, name: str) -> Folder:
-    child_folder = get_child_folder(parent_folder, name)
+    """
+    Creates a child folder under the given parent folder. If the folder already exists, returns the existing one.
 
-    # If the folder already exists, return it instead
+    :param parent_folder: The parent folder under which the child folder should be created. This can be a Folder or Drive.
+    :type parent_folder: Folder or Drive
+    :param name: The name of the child folder to be created.
+    :type name: str
+    :returns: The newly created or existing child folder.
+    :rtype: Folder
+    """
+    # If the folder already exists, return it
+    child_folder = get_child_folder(parent_folder, name)
     if child_folder is not None:
         return child_folder
 
+    # If parent_folder is a Drive, get its root folder
     if isinstance(parent_folder, Drive):
         parent_folder = parent_folder.get_root_folder()
 
-    # Otherwise create the child folder
+    # Create the child folder
     return parent_folder.create_child_folder(name)
 
 
 def rebuild_child_folder(parent_folder: Folder or Drive, name: str) -> Folder:
     child_folder = get_child_folder(parent_folder, name)
 
     if child_folder:
```

