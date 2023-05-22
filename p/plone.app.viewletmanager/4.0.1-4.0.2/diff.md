# Comparing `tmp/plone.app.viewletmanager-4.0.1.tar.gz` & `tmp/plone.app.viewletmanager-4.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plone.app.viewletmanager-4.0.1.tar", last modified: Tue Mar 21 23:16:44 2023, max compression
+gzip compressed data, was "plone.app.viewletmanager-4.0.2.tar", last modified: Mon May 22 17:53:26 2023, max compression
```

## Comparing `plone.app.viewletmanager-4.0.1.tar` & `plone.app.viewletmanager-4.0.2.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-21 23:16:44.649998 plone.app.viewletmanager-4.0.1/
--rw-r--r--   0 maurits    (501) staff       (20)     6355 2023-03-21 23:16:43.000000 plone.app.viewletmanager-4.0.1/CHANGES.rst
--rw-r--r--   0 maurits    (501) staff       (20)       70 2023-03-21 23:16:43.000000 plone.app.viewletmanager-4.0.1/CONTRIBUTING.rst
--rw-r--r--   0 maurits    (501) staff       (20)      149 2023-03-21 23:16:43.000000 plone.app.viewletmanager-4.0.1/MANIFEST.in
--rw-r--r--   0 maurits    (501) staff       (20)     7782 2023-03-21 23:16:44.650102 plone.app.viewletmanager-4.0.1/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)      409 2023-03-21 23:16:43.000000 plone.app.viewletmanager-4.0.1/README.rst
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-21 23:16:44.641812 plone.app.viewletmanager-4.0.1/docs/
--rw-r--r--   0 maurits    (501) staff       (20)    15220 2023-03-21 23:16:43.000000 plone.app.viewletmanager-4.0.1/docs/LICENSE.GPL
--rw-r--r--   0 maurits    (501) staff       (20)      686 2023-03-21 23:16:43.000000 plone.app.viewletmanager-4.0.1/docs/LICENSE.txt
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-21 23:16:44.642172 plone.app.viewletmanager-4.0.1/plone/
--rw-r--r--   0 maurits    (501) staff       (20)       56 2023-03-21 23:16:43.000000 plone.app.viewletmanager-4.0.1/plone/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-21 23:16:44.644981 plone.app.viewletmanager-4.0.1/plone/app/
--rw-r--r--   0 maurits    (501) staff       (20)       56 2023-03-21 23:16:43.000000 plone.app.viewletmanager-4.0.1/plone/app/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-21 23:16:44.647392 plone.app.viewletmanager-4.0.1/plone/app/viewletmanager/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-03-21 23:16:43.000000 plone.app.viewletmanager-4.0.1/plone/app/viewletmanager/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)      528 2023-03-21 23:16:43.000000 plone.app.viewletmanager-4.0.1/plone/app/viewletmanager/configure.zcml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-21 23:16:44.648250 plone.app.viewletmanager-4.0.1/plone/app/viewletmanager/exportimport/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-03-21 23:16:43.000000 plone.app.viewletmanager-4.0.1/plone/app/viewletmanager/exportimport/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)      414 2023-03-21 23:16:43.000000 plone.app.viewletmanager-4.0.1/plone/app/viewletmanager/exportimport/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     9092 2023-03-21 23:16:43.000000 plone.app.viewletmanager-4.0.1/plone/app/viewletmanager/exportimport/storage.py
--rw-r--r--   0 maurits    (501) staff       (20)      847 2023-03-21 23:16:43.000000 plone.app.viewletmanager-4.0.1/plone/app/viewletmanager/interfaces.py
--rw-r--r--   0 maurits    (501) staff       (20)     3523 2023-03-21 23:16:43.000000 plone.app.viewletmanager-4.0.1/plone/app/viewletmanager/manage-viewletmanager.pt
--rw-r--r--   0 maurits    (501) staff       (20)     1930 2023-03-21 23:16:43.000000 plone.app.viewletmanager-4.0.1/plone/app/viewletmanager/manage-viewlets.pt
--rw-r--r--   0 maurits    (501) staff       (20)    11776 2023-03-21 23:16:43.000000 plone.app.viewletmanager-4.0.1/plone/app/viewletmanager/manager.py
--rw-r--r--   0 maurits    (501) staff       (20)     2024 2023-03-21 23:16:43.000000 plone.app.viewletmanager-4.0.1/plone/app/viewletmanager/storage.py
--rw-r--r--   0 maurits    (501) staff       (20)      793 2023-03-21 23:16:43.000000 plone.app.viewletmanager-4.0.1/plone/app/viewletmanager/testing.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-21 23:16:44.649746 plone.app.viewletmanager-4.0.1/plone/app/viewletmanager/tests/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-03-21 23:16:43.000000 plone.app.viewletmanager-4.0.1/plone/app/viewletmanager/tests/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     4306 2023-03-21 23:16:43.000000 plone.app.viewletmanager-4.0.1/plone/app/viewletmanager/tests/manager.rst
--rw-r--r--   0 maurits    (501) staff       (20)     2181 2023-03-21 23:16:43.000000 plone.app.viewletmanager-4.0.1/plone/app/viewletmanager/tests/storage.rst
--rw-r--r--   0 maurits    (501) staff       (20)      478 2023-03-21 23:16:43.000000 plone.app.viewletmanager-4.0.1/plone/app/viewletmanager/tests/test_docs.py
--rw-r--r--   0 maurits    (501) staff       (20)    20701 2023-03-21 23:16:43.000000 plone.app.viewletmanager-4.0.1/plone/app/viewletmanager/tests/test_exportimport.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-21 23:16:44.644649 plone.app.viewletmanager-4.0.1/plone.app.viewletmanager.egg-info/
--rw-r--r--   0 maurits    (501) staff       (20)     7782 2023-03-21 23:16:44.000000 plone.app.viewletmanager-4.0.1/plone.app.viewletmanager.egg-info/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)     1197 2023-03-21 23:16:44.000000 plone.app.viewletmanager-4.0.1/plone.app.viewletmanager.egg-info/SOURCES.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2023-03-21 23:16:44.000000 plone.app.viewletmanager-4.0.1/plone.app.viewletmanager.egg-info/dependency_links.txt
--rw-r--r--   0 maurits    (501) staff       (20)       16 2023-03-21 23:16:44.000000 plone.app.viewletmanager-4.0.1/plone.app.viewletmanager.egg-info/namespace_packages.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2023-03-21 23:16:44.000000 plone.app.viewletmanager-4.0.1/plone.app.viewletmanager.egg-info/not-zip-safe
--rw-r--r--   0 maurits    (501) staff       (20)      179 2023-03-21 23:16:44.000000 plone.app.viewletmanager-4.0.1/plone.app.viewletmanager.egg-info/requires.txt
--rw-r--r--   0 maurits    (501) staff       (20)        6 2023-03-21 23:16:44.000000 plone.app.viewletmanager-4.0.1/plone.app.viewletmanager.egg-info/top_level.txt
--rw-r--r--   0 maurits    (501) staff       (20)     1688 2023-03-21 23:16:43.000000 plone.app.viewletmanager-4.0.1/pyproject.toml
--rw-r--r--   0 maurits    (501) staff       (20)      217 2023-03-21 23:16:44.650676 plone.app.viewletmanager-4.0.1/setup.cfg
--rw-r--r--   0 maurits    (501) staff       (20)     1822 2023-03-21 23:16:43.000000 plone.app.viewletmanager-4.0.1/setup.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-22 17:53:26.742431 plone.app.viewletmanager-4.0.2/
+-rw-r--r--   0 maurits    (501) staff       (20)     6517 2023-05-22 17:53:26.000000 plone.app.viewletmanager-4.0.2/CHANGES.rst
+-rw-r--r--   0 maurits    (501) staff       (20)       70 2023-05-22 17:53:26.000000 plone.app.viewletmanager-4.0.2/CONTRIBUTING.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      149 2023-05-22 17:53:26.000000 plone.app.viewletmanager-4.0.2/MANIFEST.in
+-rw-r--r--   0 maurits    (501) staff       (20)     7944 2023-05-22 17:53:26.742568 plone.app.viewletmanager-4.0.2/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)      409 2023-05-22 17:53:26.000000 plone.app.viewletmanager-4.0.2/README.rst
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-22 17:53:26.734487 plone.app.viewletmanager-4.0.2/docs/
+-rw-r--r--   0 maurits    (501) staff       (20)    15220 2023-05-22 17:53:26.000000 plone.app.viewletmanager-4.0.2/docs/LICENSE.GPL
+-rw-r--r--   0 maurits    (501) staff       (20)      686 2023-05-22 17:53:26.000000 plone.app.viewletmanager-4.0.2/docs/LICENSE.txt
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-22 17:53:26.734793 plone.app.viewletmanager-4.0.2/plone/
+-rw-r--r--   0 maurits    (501) staff       (20)       56 2023-05-22 17:53:26.000000 plone.app.viewletmanager-4.0.2/plone/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-22 17:53:26.737273 plone.app.viewletmanager-4.0.2/plone/app/
+-rw-r--r--   0 maurits    (501) staff       (20)       56 2023-05-22 17:53:26.000000 plone.app.viewletmanager-4.0.2/plone/app/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-22 17:53:26.739720 plone.app.viewletmanager-4.0.2/plone/app/viewletmanager/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2023-05-22 17:53:26.000000 plone.app.viewletmanager-4.0.2/plone/app/viewletmanager/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)      528 2023-05-22 17:53:26.000000 plone.app.viewletmanager-4.0.2/plone/app/viewletmanager/configure.zcml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-22 17:53:26.740591 plone.app.viewletmanager-4.0.2/plone/app/viewletmanager/exportimport/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2023-05-22 17:53:26.000000 plone.app.viewletmanager-4.0.2/plone/app/viewletmanager/exportimport/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)      414 2023-05-22 17:53:26.000000 plone.app.viewletmanager-4.0.2/plone/app/viewletmanager/exportimport/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     9058 2023-05-22 17:53:26.000000 plone.app.viewletmanager-4.0.2/plone/app/viewletmanager/exportimport/storage.py
+-rw-r--r--   0 maurits    (501) staff       (20)      847 2023-05-22 17:53:26.000000 plone.app.viewletmanager-4.0.2/plone/app/viewletmanager/interfaces.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3539 2023-05-22 17:53:26.000000 plone.app.viewletmanager-4.0.2/plone/app/viewletmanager/manage-viewletmanager.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     1930 2023-05-22 17:53:26.000000 plone.app.viewletmanager-4.0.2/plone/app/viewletmanager/manage-viewlets.pt
+-rw-r--r--   0 maurits    (501) staff       (20)    11776 2023-05-22 17:53:26.000000 plone.app.viewletmanager-4.0.2/plone/app/viewletmanager/manager.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2024 2023-05-22 17:53:26.000000 plone.app.viewletmanager-4.0.2/plone/app/viewletmanager/storage.py
+-rw-r--r--   0 maurits    (501) staff       (20)      793 2023-05-22 17:53:26.000000 plone.app.viewletmanager-4.0.2/plone/app/viewletmanager/testing.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-22 17:53:26.742120 plone.app.viewletmanager-4.0.2/plone/app/viewletmanager/tests/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2023-05-22 17:53:26.000000 plone.app.viewletmanager-4.0.2/plone/app/viewletmanager/tests/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     4306 2023-05-22 17:53:26.000000 plone.app.viewletmanager-4.0.2/plone/app/viewletmanager/tests/manager.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     2181 2023-05-22 17:53:26.000000 plone.app.viewletmanager-4.0.2/plone/app/viewletmanager/tests/storage.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      478 2023-05-22 17:53:26.000000 plone.app.viewletmanager-4.0.2/plone/app/viewletmanager/tests/test_docs.py
+-rw-r--r--   0 maurits    (501) staff       (20)    20701 2023-05-22 17:53:26.000000 plone.app.viewletmanager-4.0.2/plone/app/viewletmanager/tests/test_exportimport.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-22 17:53:26.736949 plone.app.viewletmanager-4.0.2/plone.app.viewletmanager.egg-info/
+-rw-r--r--   0 maurits    (501) staff       (20)     7944 2023-05-22 17:53:26.000000 plone.app.viewletmanager-4.0.2/plone.app.viewletmanager.egg-info/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)     1197 2023-05-22 17:53:26.000000 plone.app.viewletmanager-4.0.2/plone.app.viewletmanager.egg-info/SOURCES.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2023-05-22 17:53:26.000000 plone.app.viewletmanager-4.0.2/plone.app.viewletmanager.egg-info/dependency_links.txt
+-rw-r--r--   0 maurits    (501) staff       (20)       16 2023-05-22 17:53:26.000000 plone.app.viewletmanager-4.0.2/plone.app.viewletmanager.egg-info/namespace_packages.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2023-05-22 17:53:26.000000 plone.app.viewletmanager-4.0.2/plone.app.viewletmanager.egg-info/not-zip-safe
+-rw-r--r--   0 maurits    (501) staff       (20)      173 2023-05-22 17:53:26.000000 plone.app.viewletmanager-4.0.2/plone.app.viewletmanager.egg-info/requires.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        6 2023-05-22 17:53:26.000000 plone.app.viewletmanager-4.0.2/plone.app.viewletmanager.egg-info/top_level.txt
+-rw-r--r--   0 maurits    (501) staff       (20)     1643 2023-05-22 17:53:26.000000 plone.app.viewletmanager-4.0.2/pyproject.toml
+-rw-r--r--   0 maurits    (501) staff       (20)      217 2023-05-22 17:53:26.743088 plone.app.viewletmanager-4.0.2/setup.cfg
+-rw-r--r--   0 maurits    (501) staff       (20)     1816 2023-05-22 17:53:26.000000 plone.app.viewletmanager-4.0.2/setup.py
```

### Comparing `plone.app.viewletmanager-4.0.1/CHANGES.rst` & `plone.app.viewletmanager-4.0.2/CHANGES.rst`

 * *Files 3% similar despite different names*

```diff
@@ -4,14 +4,24 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+4.0.2 (2023-05-22)
+------------------
+
+Bug fixes:
+
+
+- Remove transitive circular dependency on `plone.app.vocabularies`.
+  [@jensens] (fix-circular-dependency)
+
+
 4.0.1 (2023-03-22)
 ------------------
 
 Internal:
 
 
 - Update configuration files.
```

### Comparing `plone.app.viewletmanager-4.0.1/PKG-INFO` & `plone.app.viewletmanager-4.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plone.app.viewletmanager
-Version: 4.0.1
+Version: 4.0.2
 Summary: Configurable viewlet manager
 Home-page: https://pypi.org/project/plone.app.viewletmanager
 Author: Plone Foundation
 Author-email: plone-developers@lists.sourceforge.net
 License: GPL version 2
 Keywords: viewlets
 Classifier: Development Status :: 5 - Production/Stable
@@ -42,14 +42,24 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+4.0.2 (2023-05-22)
+------------------
+
+Bug fixes:
+
+
+- Remove transitive circular dependency on `plone.app.vocabularies`.
+  [@jensens] (fix-circular-dependency)
+
+
 4.0.1 (2023-03-22)
 ------------------
 
 Internal:
 
 
 - Update configuration files.
```

### Comparing `plone.app.viewletmanager-4.0.1/docs/LICENSE.GPL` & `plone.app.viewletmanager-4.0.2/docs/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `plone.app.viewletmanager-4.0.1/docs/LICENSE.txt` & `plone.app.viewletmanager-4.0.2/docs/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `plone.app.viewletmanager-4.0.1/plone/app/viewletmanager/configure.zcml` & `plone.app.viewletmanager-4.0.2/plone/app/viewletmanager/configure.zcml`

 * *Files identical despite different names*

### Comparing `plone.app.viewletmanager-4.0.1/plone/app/viewletmanager/exportimport/storage.py` & `plone.app.viewletmanager-4.0.2/plone/app/viewletmanager/exportimport/storage.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,20 +47,20 @@
 already been registered in each skin.
 
 .. These docs are used in c.developermanual
 .. original content from http://www.sixfeetup.com/company/technologies/plone-content-management-new/quick-reference-cards/swag/swag-images-files/generic_setup.pdf
 
 """
 from plone.app.viewletmanager.interfaces import IViewletSettingsStorage
+from Products.CMFCore.utils import getToolByName
 from Products.GenericSetup.interfaces import IBody
 from Products.GenericSetup.utils import XMLAdapterBase
 from zope.component import getUtility
 from zope.component import queryMultiAdapter
 from zope.component import queryUtility
-from zope.schema.interfaces import IVocabularyFactory
 
 import os
 
 
 def importViewletSettingsStorage(context):
     """Import viewlet settings."""
     logger = context.getLogger("plone.app.viewletmanager")
@@ -105,21 +105,16 @@
 
 
 class ViewletSettingsStorageNodeAdapter(XMLAdapterBase):
     __used_for__ = IViewletSettingsStorage
 
     def __init__(self, context, environ):
         super().__init__(context, environ)
-
-        self.skins = [
-            skin.token
-            for skin in getUtility(IVocabularyFactory, "plone.app.vocabularies.Skins")(
-                self.context
-            )
-        ]
+        skins_tool = getToolByName(self.context, "portal_skins", None)
+        self.skins = list(sorted(skins_tool.getSkinSelections())) if skins_tool else []
 
     def _exportNode(self):
         """
         Export the object as a DOM node.
         """
         output = self._doc.createElement("object")
         for nodename in ("order", "hidden"):
```

### Comparing `plone.app.viewletmanager-4.0.1/plone/app/viewletmanager/interfaces.py` & `plone.app.viewletmanager-4.0.2/plone/app/viewletmanager/interfaces.py`

 * *Files identical despite different names*

### Comparing `plone.app.viewletmanager-4.0.1/plone/app/viewletmanager/manage-viewletmanager.pt` & `plone.app.viewletmanager-4.0.2/plone/app/viewletmanager/manage-viewletmanager.pt`

 * *Files 2% similar despite different names*

```diff
@@ -38,15 +38,15 @@
                 <span class="text-muted"
                       tal:content="viewlet/name"
                 >Viewlet name</span>
                 (<span tal:replace="viewlet/index">Index</span>)
               </div>
 
               <a class="btn btn-sm btn-outline-primary mx-1 text-decoration-none pat-inject"
-                 href="${viewlet/up_url}&_authenticator=${auth_token}#${manager_id}"
+                 href="${viewlet/up_url}&amp;_authenticator=${auth_token}#${manager_id}"
                  tal:condition="viewlet/up_url | nothing"
               >
                 <svg xmlns="http://www.w3.org/2000/svg"
                      class="bi bi-arrow-up-short"
                      fill="currentColor"
                      height="16"
                      viewbox="0 0 16 16"
@@ -54,15 +54,15 @@
                 >
                   <path d="M8 12a.5.5 0 0 0 .5-.5V5.707l2.146 2.147a.5.5 0 0 0 .708-.708l-3-3a.5.5 0 0 0-.708 0l-3 3a.5.5 0 1 0 .708.708L7.5 5.707V11.5a.5.5 0 0 0 .5.5z"
                         fill-rule="evenodd"
                   ></path>
                 </svg>
               </a>
               <a class="btn btn-sm btn-outline-primary mx-1 text-decoration-none pat-inject"
-                 href="${viewlet/down_url}&_authenticator=${auth_token}#${manager_id}"
+                 href="${viewlet/down_url}&amp;_authenticator=${auth_token}#${manager_id}"
                  tal:condition="viewlet/down_url | nothing"
               >
                 <svg xmlns="http://www.w3.org/2000/svg"
                      class="bi bi-arrow-down-short"
                      fill="currentColor"
                      height="16"
                      viewbox="0 0 16 16"
@@ -70,19 +70,19 @@
                 >
                   <path d="M8 4a.5.5 0 0 1 .5.5v5.793l2.146-2.147a.5.5 0 0 1 .708.708l-3 3a.5.5 0 0 1-.708 0l-3-3a.5.5 0 1 1 .708-.708L7.5 10.293V4.5A.5.5 0 0 1 8 4z"
                         fill-rule="evenodd"
                   ></path>
                 </svg>
               </a>
               <a class="btn btn-sm btn-outline-primary mx-1 text-decoration-none pat-inject ${python:'active' if not viewlet['hidden'] else ''}"
-                 href="${viewlet/hide_url}&_authenticator=${auth_token}#${manager_id}"
+                 href="${viewlet/hide_url}&amp;_authenticator=${auth_token}#${manager_id}"
                  i18n:translate="label_hide_item"
               >Hide</a>
               <a class="btn btn-sm btn-outline-primary mx-1 text-decoration-none pat-inject ${python:'active' if viewlet['hidden'] else ''}"
-                 href="${viewlet/show_url}&_authenticator=${auth_token}#${manager_id}"
+                 href="${viewlet/show_url}&amp;_authenticator=${auth_token}#${manager_id}"
                  i18n:translate="label_show_item"
               >Show</a>
 
             </div>
 
             <div class="card-body">
               <div tal:replace="structure viewlet/content"></div>
```

### Comparing `plone.app.viewletmanager-4.0.1/plone/app/viewletmanager/manage-viewlets.pt` & `plone.app.viewletmanager-4.0.2/plone/app/viewletmanager/manage-viewlets.pt`

 * *Files identical despite different names*

### Comparing `plone.app.viewletmanager-4.0.1/plone/app/viewletmanager/manager.py` & `plone.app.viewletmanager-4.0.2/plone/app/viewletmanager/manager.py`

 * *Files identical despite different names*

### Comparing `plone.app.viewletmanager-4.0.1/plone/app/viewletmanager/storage.py` & `plone.app.viewletmanager-4.0.2/plone/app/viewletmanager/storage.py`

 * *Files identical despite different names*

### Comparing `plone.app.viewletmanager-4.0.1/plone/app/viewletmanager/testing.py` & `plone.app.viewletmanager-4.0.2/plone/app/viewletmanager/testing.py`

 * *Files identical despite different names*

### Comparing `plone.app.viewletmanager-4.0.1/plone/app/viewletmanager/tests/manager.rst` & `plone.app.viewletmanager-4.0.2/plone/app/viewletmanager/tests/manager.rst`

 * *Files identical despite different names*

### Comparing `plone.app.viewletmanager-4.0.1/plone/app/viewletmanager/tests/storage.rst` & `plone.app.viewletmanager-4.0.2/plone/app/viewletmanager/tests/storage.rst`

 * *Files identical despite different names*

### Comparing `plone.app.viewletmanager-4.0.1/plone/app/viewletmanager/tests/test_exportimport.py` & `plone.app.viewletmanager-4.0.2/plone/app/viewletmanager/tests/test_exportimport.py`

 * *Files identical despite different names*

### Comparing `plone.app.viewletmanager-4.0.1/plone.app.viewletmanager.egg-info/PKG-INFO` & `plone.app.viewletmanager-4.0.2/plone.app.viewletmanager.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plone.app.viewletmanager
-Version: 4.0.1
+Version: 4.0.2
 Summary: Configurable viewlet manager
 Home-page: https://pypi.org/project/plone.app.viewletmanager
 Author: Plone Foundation
 Author-email: plone-developers@lists.sourceforge.net
 License: GPL version 2
 Keywords: viewlets
 Classifier: Development Status :: 5 - Production/Stable
@@ -42,14 +42,24 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+4.0.2 (2023-05-22)
+------------------
+
+Bug fixes:
+
+
+- Remove transitive circular dependency on `plone.app.vocabularies`.
+  [@jensens] (fix-circular-dependency)
+
+
 4.0.1 (2023-03-22)
 ------------------
 
 Internal:
 
 
 - Update configuration files.
```

### Comparing `plone.app.viewletmanager-4.0.1/plone.app.viewletmanager.egg-info/SOURCES.txt` & `plone.app.viewletmanager-4.0.2/plone.app.viewletmanager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `plone.app.viewletmanager-4.0.1/pyproject.toml` & `plone.app.viewletmanager-4.0.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -56,8 +56,7 @@
   'zope.schema', 'zope.security', 'zope.site', 'zope.traversing', 'AccessControl',
 ]
 'plone.base' = [
   'AccessControl', 'Products.BTreeFolder2', 'Products.CMFCore',
   'Products.CMFDynamicViewFTI', 'zope.deprecation',
 ]
 python-dateutil = ['dateutil']
-ignore-packages = ['plone.app.vocabularies']
```

### Comparing `plone.app.viewletmanager-4.0.1/setup.py` & `plone.app.viewletmanager-4.0.2/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages
 from setuptools import setup
 
 
-version = "4.0.1"
+version = "4.0.2"
 
 long_description = "{}\n{}".format(
     open("README.rst").read(), open("CHANGES.rst").read()
 )
 
 extras_require = {
     "test": [
@@ -15,17 +15,17 @@
         "plone.testing",
         "zope.publisher",
     ]
 }
 
 install_requires = [
     "Products.GenericSetup",
+    "Products.CMFCore",
     "Zope",
     "persistent",
-    "plone.app.vocabularies",
     "setuptools",
     "zope.contentprovider",
     "zope.viewlet",
 ]
 
 setup(
     name="plone.app.viewletmanager",
```

