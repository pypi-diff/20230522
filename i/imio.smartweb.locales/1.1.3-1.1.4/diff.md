# Comparing `tmp/imio.smartweb.locales-1.1.3.tar.gz` & `tmp/imio.smartweb.locales-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/imio.smartweb.locales-1.1.3.tar", last modified: Mon Mar 13 13:32:31 2023, max compression
+gzip compressed data, was "imio.smartweb.locales-1.1.4.tar", last modified: Mon May 22 07:05:12 2023, max compression
```

## Comparing `imio.smartweb.locales-1.1.3.tar` & `imio.smartweb.locales-1.1.4.tar`

### file list

```diff
@@ -1,40 +1,41 @@
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-13 13:32:31.000000 imio.smartweb.locales-1.1.3/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     9250 2023-03-13 13:32:31.000000 imio.smartweb.locales-1.1.3/PKG-INFO
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      106 2023-03-13 13:32:31.000000 imio.smartweb.locales-1.1.3/CONTRIBUTORS.rst
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1696 2023-03-13 13:32:31.000000 imio.smartweb.locales-1.1.3/README.rst
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     3642 2023-03-13 13:32:31.000000 imio.smartweb.locales-1.1.3/CHANGES.rst
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)       61 2023-03-13 13:32:31.000000 imio.smartweb.locales-1.1.3/MANIFEST.in
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1722 2023-03-13 13:32:31.000000 imio.smartweb.locales-1.1.3/setup.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      656 2023-03-13 13:32:31.000000 imio.smartweb.locales-1.1.3/LICENSE.rst
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      518 2023-03-13 13:32:31.000000 imio.smartweb.locales-1.1.3/setup.cfg
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-13 13:32:31.000000 imio.smartweb.locales-1.1.3/src/
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-13 13:32:31.000000 imio.smartweb.locales-1.1.3/src/imio/
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-13 13:32:31.000000 imio.smartweb.locales-1.1.3/src/imio/smartweb/
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-13 13:32:31.000000 imio.smartweb.locales-1.1.3/src/imio/smartweb/locales/
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-13 13:32:31.000000 imio.smartweb.locales-1.1.3/src/imio/smartweb/locales/locales/
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-13 13:32:31.000000 imio.smartweb.locales-1.1.3/src/imio/smartweb/locales/locales/fr/
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-13 13:32:31.000000 imio.smartweb.locales-1.1.3/src/imio/smartweb/locales/locales/fr/LC_MESSAGES/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)    88486 2023-03-13 13:32:31.000000 imio.smartweb.locales-1.1.3/src/imio/smartweb/locales/locales/fr/LC_MESSAGES/imio.smartweb.po
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1579 2023-03-13 13:32:31.000000 imio.smartweb.locales-1.1.3/src/imio/smartweb/locales/locales/fr/LC_MESSAGES/plone.po
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-13 13:32:31.000000 imio.smartweb.locales-1.1.3/src/imio/smartweb/locales/locales/nl/
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-13 13:32:31.000000 imio.smartweb.locales-1.1.3/src/imio/smartweb/locales/locales/nl/LC_MESSAGES/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)    70962 2023-03-13 13:32:31.000000 imio.smartweb.locales-1.1.3/src/imio/smartweb/locales/locales/nl/LC_MESSAGES/imio.smartweb.po
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1133 2023-03-13 13:32:31.000000 imio.smartweb.locales-1.1.3/src/imio/smartweb/locales/locales/nl/LC_MESSAGES/plone.po
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)    71135 2023-03-13 13:32:31.000000 imio.smartweb.locales-1.1.3/src/imio/smartweb/locales/locales/imio.smartweb.pot
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1236 2023-03-13 13:32:31.000000 imio.smartweb.locales-1.1.3/src/imio/smartweb/locales/locales/plone-manual.pot
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-13 13:32:31.000000 imio.smartweb.locales-1.1.3/src/imio/smartweb/locales/locales/de/
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-13 13:32:31.000000 imio.smartweb.locales-1.1.3/src/imio/smartweb/locales/locales/de/LC_MESSAGES/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)    87737 2023-03-13 13:32:31.000000 imio.smartweb.locales-1.1.3/src/imio/smartweb/locales/locales/de/LC_MESSAGES/imio.smartweb.po
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1568 2023-03-13 13:32:31.000000 imio.smartweb.locales-1.1.3/src/imio/smartweb/locales/locales/de/LC_MESSAGES/plone.po
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      151 2023-03-13 13:32:31.000000 imio.smartweb.locales-1.1.3/src/imio/smartweb/locales/__init__.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      204 2023-03-13 13:32:31.000000 imio.smartweb.locales-1.1.3/src/imio/smartweb/locales/configure.zcml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)       80 2023-03-13 13:32:31.000000 imio.smartweb.locales-1.1.3/src/imio/smartweb/__init__.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)       80 2023-03-13 13:32:31.000000 imio.smartweb.locales-1.1.3/src/imio/__init__.py
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-13 13:32:31.000000 imio.smartweb.locales-1.1.3/src/imio.smartweb.locales.egg-info/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        5 2023-03-13 13:32:31.000000 imio.smartweb.locales-1.1.3/src/imio.smartweb.locales.egg-info/top_level.txt
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     9250 2023-03-13 13:32:31.000000 imio.smartweb.locales-1.1.3/src/imio.smartweb.locales.egg-info/PKG-INFO
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        1 2023-03-13 13:32:31.000000 imio.smartweb.locales-1.1.3/src/imio.smartweb.locales.egg-info/dependency_links.txt
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)       11 2023-03-13 13:32:31.000000 imio.smartweb.locales-1.1.3/src/imio.smartweb.locales.egg-info/requires.txt
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)       19 2023-03-13 13:32:31.000000 imio.smartweb.locales-1.1.3/src/imio.smartweb.locales.egg-info/namespace_packages.txt
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1037 2023-03-13 13:32:31.000000 imio.smartweb.locales-1.1.3/src/imio.smartweb.locales.egg-info/SOURCES.txt
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        1 2023-03-13 13:32:31.000000 imio.smartweb.locales-1.1.3/src/imio.smartweb.locales.egg-info/not-zip-safe
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-05-22 07:05:12.429948 imio.smartweb.locales-1.1.4/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     3795 2023-05-22 07:05:12.000000 imio.smartweb.locales-1.1.4/CHANGES.rst
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      106 2023-05-22 07:05:12.000000 imio.smartweb.locales-1.1.4/CONTRIBUTORS.rst
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)    18092 2023-05-22 07:05:12.000000 imio.smartweb.locales-1.1.4/LICENSE.GPL
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      656 2023-05-22 07:05:12.000000 imio.smartweb.locales-1.1.4/LICENSE.rst
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)       61 2023-05-22 07:05:12.000000 imio.smartweb.locales-1.1.4/MANIFEST.in
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     6616 2023-05-22 07:05:12.429948 imio.smartweb.locales-1.1.4/PKG-INFO
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1696 2023-05-22 07:05:12.000000 imio.smartweb.locales-1.1.4/README.rst
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      518 2023-05-22 07:05:12.429948 imio.smartweb.locales-1.1.4/setup.cfg
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1722 2023-05-22 07:05:12.000000 imio.smartweb.locales-1.1.4/setup.py
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-05-22 07:05:12.425948 imio.smartweb.locales-1.1.4/src/
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-05-22 07:05:12.429948 imio.smartweb.locales-1.1.4/src/imio/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)       80 2023-05-22 07:05:12.000000 imio.smartweb.locales-1.1.4/src/imio/__init__.py
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-05-22 07:05:12.429948 imio.smartweb.locales-1.1.4/src/imio/smartweb/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)       80 2023-05-22 07:05:12.000000 imio.smartweb.locales-1.1.4/src/imio/smartweb/__init__.py
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-05-22 07:05:12.429948 imio.smartweb.locales-1.1.4/src/imio/smartweb/locales/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      151 2023-05-22 07:05:12.000000 imio.smartweb.locales-1.1.4/src/imio/smartweb/locales/__init__.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      204 2023-05-22 07:05:12.000000 imio.smartweb.locales-1.1.4/src/imio/smartweb/locales/configure.zcml
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-05-22 07:05:12.429948 imio.smartweb.locales-1.1.4/src/imio/smartweb/locales/locales/
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-05-22 07:05:12.429948 imio.smartweb.locales-1.1.4/src/imio/smartweb/locales/locales/de/
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-05-22 07:05:12.429948 imio.smartweb.locales-1.1.4/src/imio/smartweb/locales/locales/de/LC_MESSAGES/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)    88162 2023-05-22 07:05:12.000000 imio.smartweb.locales-1.1.4/src/imio/smartweb/locales/locales/de/LC_MESSAGES/imio.smartweb.po
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1568 2023-05-22 07:05:12.000000 imio.smartweb.locales-1.1.4/src/imio/smartweb/locales/locales/de/LC_MESSAGES/plone.po
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-05-22 07:05:12.429948 imio.smartweb.locales-1.1.4/src/imio/smartweb/locales/locales/fr/
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-05-22 07:05:12.429948 imio.smartweb.locales-1.1.4/src/imio/smartweb/locales/locales/fr/LC_MESSAGES/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)    89005 2023-05-22 07:05:12.000000 imio.smartweb.locales-1.1.4/src/imio/smartweb/locales/locales/fr/LC_MESSAGES/imio.smartweb.po
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1579 2023-05-22 07:05:12.000000 imio.smartweb.locales-1.1.4/src/imio/smartweb/locales/locales/fr/LC_MESSAGES/plone.po
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)    71560 2023-05-22 07:05:12.000000 imio.smartweb.locales-1.1.4/src/imio/smartweb/locales/locales/imio.smartweb.pot
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-05-22 07:05:12.429948 imio.smartweb.locales-1.1.4/src/imio/smartweb/locales/locales/nl/
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-05-22 07:05:12.429948 imio.smartweb.locales-1.1.4/src/imio/smartweb/locales/locales/nl/LC_MESSAGES/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)    71387 2023-05-22 07:05:12.000000 imio.smartweb.locales-1.1.4/src/imio/smartweb/locales/locales/nl/LC_MESSAGES/imio.smartweb.po
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1133 2023-05-22 07:05:12.000000 imio.smartweb.locales-1.1.4/src/imio/smartweb/locales/locales/nl/LC_MESSAGES/plone.po
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1236 2023-05-22 07:05:12.000000 imio.smartweb.locales-1.1.4/src/imio/smartweb/locales/locales/plone-manual.pot
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-05-22 07:05:12.429948 imio.smartweb.locales-1.1.4/src/imio.smartweb.locales.egg-info/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     6616 2023-05-22 07:05:12.000000 imio.smartweb.locales-1.1.4/src/imio.smartweb.locales.egg-info/PKG-INFO
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1049 2023-05-22 07:05:12.000000 imio.smartweb.locales-1.1.4/src/imio.smartweb.locales.egg-info/SOURCES.txt
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        1 2023-05-22 07:05:12.000000 imio.smartweb.locales-1.1.4/src/imio.smartweb.locales.egg-info/dependency_links.txt
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)       19 2023-05-22 07:05:12.000000 imio.smartweb.locales-1.1.4/src/imio.smartweb.locales.egg-info/namespace_packages.txt
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        1 2023-05-22 07:05:12.000000 imio.smartweb.locales-1.1.4/src/imio.smartweb.locales.egg-info/not-zip-safe
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)       11 2023-05-22 07:05:12.000000 imio.smartweb.locales-1.1.4/src/imio.smartweb.locales.egg-info/requires.txt
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        5 2023-05-22 07:05:12.000000 imio.smartweb.locales-1.1.4/src/imio.smartweb.locales.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `imio.smartweb.locales-1.1.3/README.rst` & `imio.smartweb.locales-1.1.4/README.rst`

 * *Files identical despite different names*

### Comparing `imio.smartweb.locales-1.1.3/CHANGES.rst` & `imio.smartweb.locales-1.1.4/CHANGES.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,21 @@
 Changelog
 =========
 
 
+1.1.4 (2023-05-22)
+------------------
+
+- Add missing French translation (`folder_contents` properties)
+  [laulaz]
+
+- Migrate to Plone 6.0.4
+  [boulch]
+
+
 1.1.3 (2023-03-13)
 ------------------
 
 - Add missing French translations (Cirkwi & image dimensions warning)
   [laulaz]
 
 - Migrate to Plone 6.0.2
```

### Comparing `imio.smartweb.locales-1.1.3/setup.py` & `imio.smartweb.locales-1.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
         open("CHANGES.rst").read(),
     ]
 )
 
 
 setup(
     name="imio.smartweb.locales",
-    version="1.1.3",
+    version="1.1.4",
     description="Locales for iMio smartweb packages",
     long_description=long_description,
     # Get more from https://pypi.org/classifiers/
     classifiers=[
         "Environment :: Web Environment",
         "Framework :: Plone",
         "Framework :: Plone :: Addon",
```

### Comparing `imio.smartweb.locales-1.1.3/LICENSE.rst` & `imio.smartweb.locales-1.1.4/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `imio.smartweb.locales-1.1.3/setup.cfg` & `imio.smartweb.locales-1.1.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `imio.smartweb.locales-1.1.3/src/imio/smartweb/locales/locales/fr/LC_MESSAGES/imio.smartweb.po` & `imio.smartweb.locales-1.1.4/src/imio/smartweb/locales/locales/de/LC_MESSAGES/imio.smartweb.po`

 * *Files 1% similar despite different names*

```diff
@@ -4,21 +4,21 @@
 "POT-Creation-Date: YEAR-MO-DA HO:MI +ZONE\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI +ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=(n > 1);\n"
-"Language-Code: fr\n"
-"Language-Name: French\n"
+"Plural-Forms: nplurals=1; plural=0;\n"
+"Language-Code: de\n"
+"Language-Name: Deutsch\n"
 "Preferred-Encodings: utf-8 latin1\n"
 "Domain: imio.smartweb\n"
-"Language: fr\n"
-"X-Is-Fallback-For: fr-be fr-ca fr-lu fr-mc fr-ch fr-fr\n"
+"Language: de\n"
+"X-Is-Fallback-For: de-at de-li de-lu de-ch de-de\n"
 
 #: imio/smartweb/core/contents/sections/base.py:85
 msgid "<div class=\"section_error_txt\">Error in section : \"{}\" <a href=\"{}/edit\">[edit]</a></div>"
 msgstr "<div class=\"section_error_txt\">Erreur dans la section : \"{}\" <a href=\"{}/edit\">[modifier]</a></div>"
 
 #: imio/smartweb/common/browser/privacy/form.py:31
 #: imio/smartweb/common/viewlets/privacy.pt:15
@@ -195,21 +195,21 @@
 msgid "Allow to select quick access elements for current context."
 msgstr "Permet de sélectionner des éléments Accès Direct pour l'élément courant."
 
 #: imio/smartweb/core/contents/sections/slide/content.py:53
 msgid "Alternatively as a picture"
 msgstr "Comme alternative à une image"
 
-#: imio/smartweb/core/contents/folder/views.py:132
+#: imio/smartweb/core/contents/folder/views.py:134
 msgid "Apply"
 msgstr "Appliquer"
 
 #: imio/smartweb/core/viewlets/toolbar.py:19
 msgid "Authentic sources"
-msgstr "Sources authentiques"
+msgstr ""
 
 #: imio/smartweb/policy/upgrades/configure.zcml:68
 msgid "Automatically publish GDPR article"
 msgstr ""
 
 #: imio/smartweb/core/browser/instancebehaviors/form.py:22
 msgid "Available taxonomies"
@@ -228,15 +228,15 @@
 msgid "Bad URL format '${val}' (good format sample: https://www.imio.be)."
 msgstr "Mauvais format d'URL pour '${val}' (format correct: https://www.imio.be)."
 
 #: imio/directory/core/browser/import.py:90
 msgid "Bad mail format '${val}' (good format sample: noreply@imio.be)."
 msgstr "Mauvais format d'email pour '${val}' (format correct: noreply@imio.be)."
 
-#: imio/directory/core/contents/contact/content.py:42
+#: imio/directory/core/contents/contact/content.py:44
 msgid "Bad phone format"
 msgstr "Mauvais format de téléphone"
 
 #: imio/directory/core/browser/import.py:72
 msgid "Bad phone format '${val}' (good format sample: +32444556677)."
 msgstr "Mauvais format de numéro de téléphone pour '${val}' (format correct: +32444556677)."
 
@@ -286,15 +286,15 @@
 msgid "CSV file"
 msgstr "Fichier CSV"
 
 #: imio/smartweb/common/sharing/localroles.py:12
 msgid "Can manage locally"
 msgstr "Peut administrer"
 
-#: imio/smartweb/core/vocabularies.py:570
+#: imio/smartweb/core/vocabularies.py:571
 msgid "Carousel"
 msgstr "Carrousel"
 
 #: imio/smartweb/core/contents/sections/links/configure.zcml:26
 #: imio/smartweb/core/contents/sections/selections/configure.zcml:26
 msgid "Carousel view"
 msgstr "Affichage carrousel"
@@ -487,19 +487,19 @@
 #: imio/directory/core/browser/import.py:227
 msgid "Chosen topic '${val}' doesn't exist."
 msgstr "La thématique choisie '${val}' n'existe pas."
 
 #: imio/smartweb/core/profiles/default/types/imio.smartweb.CirkwiView.xml
 #: imio/smartweb/core/upgrades/profiles/1035_to_1036/types/imio.smartweb.CirkwiView.xml
 msgid "Cirkwi view"
-msgstr "Vue Cirkwi"
+msgstr ""
 
 #: imio/smartweb/core/contents/pages/cirkwi/content.py:14
 msgid "Cirkwi widget ID"
-msgstr "Identifiant de votre widget \"Cirkwi\""
+msgstr ""
 
 #: imio/smartweb/common/profiles/default/registry.xml
 msgid "Cities"
 msgstr ""
 
 #: imio/smartweb/common/vocabularies.py:27
 msgid "Citizen participation"
@@ -553,15 +553,15 @@
 msgid "Click to preview content (without editor actions)."
 msgstr "Prévisualiser le contenu (sans les boutons d'édition)."
 
 #: imio/smartweb/core/viewlets/navigation.py:85
 msgid "Close"
 msgstr "Fermer"
 
-#: imio/smartweb/core/contents/sections/contact/view.py:258
+#: imio/smartweb/core/contents/sections/contact/view.py:272
 msgid "Closed"
 msgstr "Fermé"
 
 #: imio/smartweb/core/profiles/default/types/imio.smartweb.SectionCollection.xml
 msgid "Collection section"
 msgstr "Section collection"
 
@@ -600,15 +600,15 @@
 msgid "Contact"
 msgstr "Contact"
 
 #: imio/directory/core/profiles/default/types/imio.directory.Contact.xml
 msgid "Contact content type"
 msgstr "Contact"
 
-#: imio/directory/core/contents/contact/content.py:106
+#: imio/directory/core/contents/contact/content.py:134
 #: imio/smartweb/core/vocabularies.py:158
 msgid "Contact informations"
 msgstr "Coordonnées"
 
 #: imio/smartweb/core/profiles/default/types/imio.smartweb.SectionContact.xml
 msgid "Contact section"
 msgstr "Section contact"
@@ -673,15 +673,15 @@
 msgid "Define number of levels in menu navigation subsite"
 msgstr "Définir un nombre de niveaux pour le menu de navigation du sous-site"
 
 #: imio/smartweb/core/contents/sections/macros.pt:57
 msgid "Delete section"
 msgstr "Supprimer la section"
 
-#: imio/directory/core/contents/contact/content.py:209
+#: imio/directory/core/contents/contact/content.py:237
 #: imio/events/core/contents/event/content.py:53
 #: imio/news/core/contents/newsitem/content.py:39
 msgid "Description"
 msgstr "Description"
 
 #: imio/smartweb/core/browser/controlpanel.py:72
 msgid "Directory SolR Core ID"
@@ -710,15 +710,15 @@
 #: imio/smartweb/core/viewlets/banner.pt:11
 msgid "Display banner from this item"
 msgstr "Afficher la bannière"
 
 #: imio/smartweb/core/profiles/default/types/imio.smartweb.CirkwiView.xml
 #: imio/smartweb/core/upgrades/profiles/1035_to_1036/types/imio.smartweb.CirkwiView.xml
 msgid "Display cirkwi informations and map."
-msgstr "Affiche les informations et la carte Cirkwi"
+msgstr ""
 
 #: imio/smartweb/core/profiles/default/types/imio.smartweb.DirectoryView.xml
 msgid "Display linked directory from imio directory instance."
 msgstr "Affiche des contacts depuis la source authentique"
 
 #: imio/smartweb/core/profiles/default/types/imio.smartweb.EventsView.xml
 msgid "Display linked events from imio events instance."
@@ -728,29 +728,29 @@
 msgid "Display linked news from imio news instance."
 msgstr "Affiche des actualités depuis la source authentique"
 
 #: imio/directory/core/vocabularies.py:85
 msgid "Drinking water point"
 msgstr "Points d'eau potable"
 
-#: imio/directory/core/contents/contact/content.py:232
+#: imio/directory/core/contents/contact/content.py:260
 #: imio/events/core/contents/event/content.py:77
 #: imio/news/core/contents/newsitem/content.py:63
 msgid "Dutch translations"
 msgstr "Traductions néerlandophones"
 
 #: imio/smartweb/core/contents/pages/procedure/content.py:21
 msgid "E-Guichet procedure"
 msgstr "Lien vers la démarche dans l'e-guichet iMio"
 
-#: imio/directory/core/contents/contact/content.py:81
+#: imio/directory/core/contents/contact/content.py:109
 msgid "E-mail"
 msgstr "Adresse e-mail"
 
-#: imio/directory/core/contents/contact/content.py:121
+#: imio/directory/core/contents/contact/content.py:149
 msgid "E-mails"
 msgstr ""
 
 #: imio/smartweb/common/vocabularies.py:22
 msgid "Economics"
 msgstr "Économie"
 
@@ -782,15 +782,15 @@
 msgid "Enable minisite"
 msgstr "Activer le mode site partenaire"
 
 #: imio/smartweb/core/profiles/default/actions.xml
 msgid "Enable subsite"
 msgstr "Activer le mode sous-site"
 
-#: imio/directory/core/contents/contact/content.py:215
+#: imio/directory/core/contents/contact/content.py:243
 #: imio/events/core/contents/event/content.py:60
 #: imio/news/core/contents/newsitem/content.py:46
 msgid "English translations"
 msgstr "Traductions anglophones"
 
 #: imio/smartweb/core/browser/controlpanel.py:17
 msgid "Enter the language code. Ex.: en"
@@ -876,15 +876,15 @@
 msgid "Example : Photo of a person or organization building"
 msgstr "Exemple : Photo d'une personne ou d'un bâtiment d'une organisation"
 
 #: imio/smartweb/core/browser/controlpanel.py:26
 msgid "Example : https://COMMUNE-formulaires.guichet-citoyen.be/api/formdefs/"
 msgstr "Exemple : https://COMMUNE-formulaires.guichet-citoyen.be/api/formdefs/"
 
-#: imio/directory/core/contents/contact/content.py:269
+#: imio/directory/core/contents/contact/content.py:297
 msgid "Example : shop, service, association logo"
 msgstr "Exemple : Logo d'un magasin ou d'un service ou d'une association"
 
 #: imio/smartweb/core/behaviors/listing.py:19
 msgid "Exclude from parent listing"
 msgstr "Exclure dans l'affichage listing du parent"
 
@@ -934,15 +934,15 @@
 msgid "Faceted summary view"
 msgstr "Affichage liste"
 
 #: imio/smartweb/core/browser/faceted/configure.zcml:88
 msgid "Faceted summary view with images"
 msgstr "Affichage liste avec images"
 
-#: imio/directory/core/contents/contact/content.py:286
+#: imio/directory/core/contents/contact/content.py:314
 msgid "Facilities"
 msgstr "Facilités"
 
 #: imio/events/core/contents/event/content.py:151
 #: imio/events/core/contents/event/view.pt:57
 msgid "Facilities for person with reduced mobility"
 msgstr "Accessible aux personnes à mobilité réduite"
@@ -1015,28 +1015,28 @@
 msgid "Footer has been successfully added"
 msgstr "Le pied de page a été ajouté avec succès"
 
 #: imio/smartweb/core/contents/folder/content.py:26
 msgid "For the anonymous visitor, the folder and the selected item are one. When he clicks on the folder, the item is displayed."
 msgstr "Pour le visiteur anonyme, le dossier et l'élément sélectionné ne font qu'un. Lorsqu'il clique sur le dossier, l'élément s'affiche."
 
-#: imio/smartweb/core/contents/folder/views.py:103
+#: imio/smartweb/core/contents/folder/views.py:105
 msgid "Form to choose item to be displayed as the home page of the folder"
 msgstr "Formulaire de choix de l'élément à afficher comme page d'accueil du dossier"
 
 #: imio/directory/core/vocabularies.py:88
 msgid "Free WIFI"
 msgstr "Wifi gratuit"
 
 #: imio/events/core/contents/event/content.py:144
 #: imio/events/core/contents/event/view.pt:47
 msgid "Free entry"
 msgstr "Gratuit"
 
-#: imio/smartweb/core/contents/sections/contact/view.py:117
+#: imio/smartweb/core/contents/sections/contact/view.py:131
 msgid "Friday"
 msgstr "Vendredi"
 
 #: imio/smartweb/core/contents/sections/events/macros.pt:13
 msgid "From"
 msgstr "Du"
 
@@ -1056,27 +1056,27 @@
 msgid "Gallery section"
 msgstr "Section galerie"
 
 #: imio/smartweb/core/profiles/default/types/imio.smartweb.SectionGallery.xml
 msgid "Gallery section for a page"
 msgstr "Création d'une section galerie qui affichera ses images dans votre page. "
 
-#: imio/directory/core/contents/contact/content.py:198
+#: imio/directory/core/contents/contact/content.py:226
 #: imio/events/core/contents/event/content.py:43
 #: imio/news/core/contents/newsitem/content.py:29
 msgid "German translations"
 msgstr "Traductions germanophones"
 
 #: imio/smartweb/core/contents/sections/events/content.py:37
 msgid "Get priory on related agenda for these specifics events."
 msgstr "Ces événéments prennent la priorité sur le champ d'agenda lié."
 
 #: imio/smartweb/core/contents/sections/news/content.py:37
 msgid "Get priory on related news for these specifics news."
-msgstr "Ces actualités prennent la priorité sur le champ des actualités liées."
+msgstr ""
 
 #: imio/smartweb/core/viewlets/minisite_link.pt:8
 msgid "Go to ${url}"
 msgstr "Aller sur ${url}"
 
 #: imio/smartweb/core/contents/sections/html/content.py:17
 msgid "HTML"
@@ -1210,15 +1210,15 @@
 msgstr "Important! Ces catégories sont utilisées pour créer des listes accessibles via le menu navigation"
 
 #: imio/events/core/contents/event/content.py:175
 #: imio/news/core/contents/newsitem/content.py:130
 msgid "Important! These categories are used to supplement the information provided by the topics"
 msgstr "Important! Ces catégories permettent de compléter l'information apportée par les thématiques"
 
-#: imio/directory/core/contents/contact/content.py:287
+#: imio/directory/core/contents/contact/content.py:315
 msgid "Important! These categories make it possible to highlight and geolocate certain basic services"
 msgstr "Important! Ces catégories permettent de mettre en avant et de géolocaliser certains services de base"
 
 #: imio/smartweb/common/behaviors/topics.py:17
 msgid "Important! Topics are used to filter search results and create lists"
 msgstr "Important! Les thématiques sont utilisées pour filtrer les résultats de la recherche et créer des listes"
 
@@ -1236,41 +1236,41 @@
 msgid "Instagram url for this event"
 msgstr "Lien Instagram pour cet événement"
 
 #: imio/news/core/contents/newsitem/content.py:110
 msgid "Instagram url for this news"
 msgstr "Lien Instagram de cette actualité"
 
-#: imio/directory/policy/configure.zcml:34
+#: imio/directory/policy/configure.zcml:35
 msgid "Installs the imio.directory.policy add-on."
 msgstr ""
 
-#: imio/events/policy/configure.zcml:35
+#: imio/events/policy/configure.zcml:36
 msgid "Installs the imio.events.policy add-on."
 msgstr ""
 
-#: imio/news/policy/configure.zcml:35
+#: imio/news/policy/configure.zcml:36
 msgid "Installs the imio.news.policy add-on."
 msgstr ""
 
-#: imio/directory/core/contents/contact/content.py:179
+#: imio/directory/core/contents/contact/content.py:207
 msgid "Internal note"
 msgstr "Note interne"
 
 #: imio/events/core/vocabularies.py:26
 msgid "Internships and courses"
 msgstr "Stages et cours"
 
 #: imio/smartweb/core/contents/folder/content.py:25
 msgid "Item(s) that can be selected as the folder default page."
 msgstr "Elément(s) pouvant être sélectionné(s) comme page d'accueil du dossier."
 
-#: imio/events/core/contents/event/views.py:75
+#: imio/events/core/contents/event/views.py:77
 #: imio/smartweb/core/contents/sections/contact/view.pt:122
-#: imio/smartweb/core/contents/sections/contact/view.py:62
+#: imio/smartweb/core/contents/sections/contact/view.py:77
 msgid "Itinerary"
 msgstr "Itinéraire"
 
 #: imio/news/core/vocabularies.py:18
 msgid "Job offer"
 msgstr "Emploi"
 
@@ -1283,19 +1283,19 @@
 msgstr "Journaliste"
 
 #: imio/events/core/contents/event/view.pt:107
 #: imio/news/core/contents/newsitem/view.pt:64
 msgid "Keywords"
 msgstr "Mots-clés"
 
-#: imio/directory/core/contents/contact/content.py:69
+#: imio/directory/core/contents/contact/content.py:97
 msgid "Label (Secretariat, Manager office, Sales,...)"
 msgstr "Intitulé (Secrétariat, Bureau de la direction, Ventes, ...)"
 
-#: imio/directory/core/contents/contact/content.py:48
+#: imio/directory/core/contents/contact/content.py:76
 msgid "Label (direction, Main number,...)"
 msgstr "Intitulé (direction, numéro principal, ...)"
 
 #: imio/smartweb/core/browser/controlpanel.py:16
 msgid "Language (en, fr,...)"
 msgstr "Langue (en, fr, ...)"
 
@@ -1369,30 +1369,30 @@
 msgid "List of events categories values available for this entity (one per line)"
 msgstr "Liste de catégories spécifiques d'événements disponibes pour cette entité (un par ligne)"
 
 #: imio/news/core/contents/entity/content.py:26
 msgid "List of news categories values available for this entity (one per line)"
 msgstr "Liste de catégories spécifiques d'actualités disponibes pour cette entité (une par ligne)"
 
-#: imio/directory/core/contents/contact/content.py:268
+#: imio/directory/core/contents/contact/content.py:296
 #: imio/smartweb/core/behaviors/minisite.py:41
 #: imio/smartweb/core/behaviors/subsite.py:33
 msgid "Logo"
 msgstr "Logo"
 
 #: imio/smartweb/core/vocabularies.py:143
 msgid "Logo and title"
 msgstr "Logo et titre"
 
 #: imio/smartweb/core/behaviors/minisite.py:47
 #: imio/smartweb/core/behaviors/subsite.py:39
 msgid "Logo display"
 msgstr "Type d'affichage du logo"
 
-#: imio/smartweb/core/contents/sections/contact/view.py:288
+#: imio/smartweb/core/contents/sections/contact/view.py:302
 msgid "Lunch time"
 msgstr "Heure du midi"
 
 #: imio/smartweb/core/contents/sections/macros.pt:46
 msgid "Manage section contents"
 msgstr "Modifier contenu"
 
@@ -1459,15 +1459,15 @@
 msgid "Mobility"
 msgstr "Mobilité"
 
 #: imio/smartweb/core/contents/sections/macros.pt:63
 msgid "Modified"
 msgstr "Modifié"
 
-#: imio/smartweb/core/contents/sections/contact/view.py:113
+#: imio/smartweb/core/contents/sections/contact/view.py:127
 msgid "Monday"
 msgstr "Lundi"
 
 #: imio/smartweb/core/profiles/default/actions.xml
 msgid "My account"
 msgstr "Mon compte"
 
@@ -1527,15 +1527,15 @@
 msgid "Not allowed to add Files or Images in imio.directory.Entity"
 msgstr ""
 
 #: imio/smartweb/common/interfaces.py:34
 msgid "Number"
 msgstr "Numéro"
 
-#: imio/directory/core/contents/contact/content.py:61
+#: imio/directory/core/contents/contact/content.py:89
 msgid "Number (format: +32475010203)"
 msgstr "Numéro (format: +32475010203)"
 
 #: imio/smartweb/core/contents/sections/collection/content.py:41
 #: imio/smartweb/core/contents/sections/events/content.py:63
 #: imio/smartweb/core/contents/sections/files/content.py:15
 msgid "Number of items per batch"
@@ -1567,19 +1567,19 @@
 msgid "Only one procedure field can be filled !"
 msgstr "Un seul champ \"démarche\" peut être rempli !"
 
 #: imio/smartweb/core/contents/blocks/link/content.py:34
 msgid "Only used in table view (takes precedence over image)"
 msgstr "Utilisée uniquement dans l'affichage tableau (prend la priorité sur l'image)"
 
-#: imio/smartweb/core/contents/sections/contact/view.py:265
+#: imio/smartweb/core/contents/sections/contact/view.py:279
 msgid "Open"
 msgstr "Ouvert"
 
-#: imio/smartweb/core/contents/sections/contact/view.py:282
+#: imio/smartweb/core/contents/sections/contact/view.py:296
 msgid "Open at "
 msgstr "Ouvre à "
 
 #: imio/smartweb/core/contents/blocks/link/content.py:23
 #: imio/smartweb/core/contents/sections/slide/content.py:66
 msgid "Open in a new tab"
 msgstr "Ouvrir dans un nouvel onglet"
@@ -1632,23 +1632,27 @@
 msgid "Parent listing"
 msgstr "Listing du parent"
 
 #: imio/events/core/vocabularies.py:23
 msgid "Party and folklore"
 msgstr "Fête et folklore"
 
+#: imio/smartweb/common/upgrades/configure.zcml:69
+msgid "Patch (Remove select2) eea.facetednavigation jquery"
+msgstr ""
+
 #: imio/directory/core/vocabularies.py:53
 msgid "Personal email"
 msgstr "Adresse e-mail personnelle"
 
 #: imio/directory/core/vocabularies.py:39
 msgid "Personal phone"
 msgstr "Numéro de téléphone personnel"
 
-#: imio/directory/core/contents/contact/content.py:111
+#: imio/directory/core/contents/contact/content.py:139
 msgid "Phones"
 msgstr "Téléphones"
 
 #: imio/smartweb/core/contents/sections/slide/content.py:41
 msgid "Picture will be displayed as slide background"
 msgstr "L'image est affichée en background du slide"
 
@@ -1706,15 +1710,15 @@
 msgid "Presse"
 msgstr "Presse"
 
 #: imio/smartweb/core/profiles/default/actions.xml
 msgid "Preview"
 msgstr "Prévisualiser"
 
-#: imio/directory/core/contents/contact/content.py:144
+#: imio/directory/core/contents/contact/content.py:172
 msgid "Private contact informations"
 msgstr "Coordonnées privées"
 
 #: imio/smartweb/core/profiles/default/types/imio.smartweb.Procedure.xml
 msgid "Procedure"
 msgstr "Démarche"
 
@@ -1804,15 +1808,15 @@
 msgid "Right"
 msgstr "Droite"
 
 #: imio/smartweb/common/vocabularies.py:30
 msgid "Safety and prevention"
 msgstr "Sécurité et prévention"
 
-#: imio/smartweb/core/contents/sections/contact/view.py:118
+#: imio/smartweb/core/contents/sections/contact/view.py:132
 msgid "Saturday"
 msgstr "Samedi"
 
 #: imio/smartweb/common/browser/privacy/form.py:27
 msgid "Save my choices"
 msgstr "Enregistrer mes choix"
 
@@ -1829,19 +1833,19 @@
 msgid "Secret key"
 msgstr "Clé secrète"
 
 #: imio/smartweb/core/browser/controlpanel.py:34
 msgid "Secret key to use API"
 msgstr "Clé secrète pour utiliser l'API"
 
-#: imio/smartweb/core/contents/sections/views.py:34
+#: imio/smartweb/core/contents/sections/views.py:44
 msgid "Section title has been hidden"
 msgstr "Le titre de la section a été caché (pour le visiteur)"
 
-#: imio/smartweb/core/contents/sections/views.py:41
+#: imio/smartweb/core/contents/sections/views.py:51
 msgid "Section title has been shown"
 msgstr "Le titre de la section a été affiché"
 
 #: imio/smartweb/core/contents/sections/base.py:58
 msgid "Section width"
 msgstr "Largeur de la section"
 
@@ -1869,15 +1873,15 @@
 msgid "Select agenda to display"
 msgstr "Sélectionnez l'agenda à afficher"
 
 #: imio/events/core/contents/event/content.py:165
 msgid "Select agendas where this event will be displayed. Current agenda is always selected."
 msgstr "Sélectionnez les agendas dans lesquels cet événement sera affiché. L'agenda courant sera toujours sélectionné."
 
-#: imio/directory/core/contents/contact/content.py:277
+#: imio/directory/core/contents/contact/content.py:305
 msgid "Select entities where this contact will be displayed. Current entity will always be selected."
 msgstr "Sélectionnez les entités dans lesquelles ce contact sera affiché. L'entité courante sera toujours sélectionnée."
 
 #: imio/smartweb/core/contents/sections/text/content.py:37
 msgid "Select image size"
 msgstr "Sélectionnez la taille de l'image"
 
@@ -1909,15 +1913,15 @@
 msgid "Selected agenda"
 msgstr "Agenda sélectionné"
 
 #: imio/events/core/contents/event/content.py:164
 msgid "Selected agendas"
 msgstr "Agendas concernés"
 
-#: imio/directory/core/contents/contact/content.py:276
+#: imio/directory/core/contents/contact/content.py:304
 msgid "Selected entities"
 msgstr "Entités concernées"
 
 #: imio/smartweb/core/contents/rest/events/content.py:17
 msgid "Selected event types"
 msgstr "Types d'événements sélectionnés"
 
@@ -2044,19 +2048,19 @@
 
 #: imio/smartweb/core/contents/sections/events/content.py:36
 msgid "Specific related events"
 msgstr "Evénements spécifiquement sélectionnés"
 
 #: imio/smartweb/core/contents/sections/news/content.py:36
 msgid "Specific related news"
-msgstr "Actualités spécifiquement sélectionnées"
+msgstr ""
 
 #: imio/smartweb/core/contents/pages/cirkwi/content.py:15
 msgid "Specify your cirkwi widget ID. You can find it when you create a new widget in Cirkwi."
-msgstr "Précisez votre identifiant de widget Cirkwi. Vous pouvez le trouver lorsque vous créez un nouveau widget dans Cirkwi."
+msgstr ""
 
 #: imio/smartweb/common/vocabularies.py:32
 msgid "Sports"
 msgstr "Sports"
 
 #: imio/smartweb/core/profiles/default/types/imio.smartweb.Page.xml
 msgid "Standard Page content type to print informations"
@@ -2090,28 +2094,28 @@
 msgid "Subsite has been disabled"
 msgstr "Le mode sous-site a été désactivé"
 
 #: imio/smartweb/core/browser/subsite/settings.py:25
 msgid "Subsite has been successfully activated"
 msgstr "Le mode sous-site a été activé avec succès"
 
-#: imio/directory/core/contents/contact/content.py:208
+#: imio/directory/core/contents/contact/content.py:236
 #: imio/smartweb/core/contents/sections/postit/content.py:26
 msgid "Subtitle"
 msgstr "Sous-titre"
 
 #: imio/smartweb/core/contents/folder/configure.zcml:72
 msgid "Summary view"
 msgstr "Affichage liste"
 
 #: imio/smartweb/core/contents/folder/configure.zcml:83
 msgid "Summary view with images"
 msgstr "Affichage liste avec images"
 
-#: imio/smartweb/core/contents/sections/contact/view.py:119
+#: imio/smartweb/core/contents/sections/contact/view.py:133
 msgid "Sunday"
 msgstr "Dimanche"
 
 #: imio/smartweb/core/contents/sections/contact/content.py:47
 msgid "Switch lead image to portrait mode"
 msgstr "Passer l'image de garde en mode portrait"
 
@@ -2156,15 +2160,15 @@
 
 #: imio/directory/core/contents/contact/forms.py:18
 msgid "The geolocation is generated on the basis of the address during contact save. It is possible to change the pointer manually if it is not correctly positioned."
 msgstr "La géolocalisation est générée sur base de l'adresse lors de l'enregistrement de la fiche. Il est possible de modifier le pointeur manuellement si ce dernier n'est pas bien positionné."
 
 #: imio/smartweb/common/utils.py:133
 msgid "The image uploaded in the \"${field_title}\" field may be degraded because it does not meet the required minimum dimensions of ${min_width}px width by ${min_height}px height (uploaded image size: ${width}px width by ${height}px height). You can see the detail via the Cropping menu."
-msgstr "L'image téléversée dans le champ \"${field_title}\" risque d'être dégradée, car elle ne correspond pas aux dimensions minimales requises de ${min_width}px de largeur sur ${min_height}px de hauteur (taille de l'image téléversée : ${width}px de largeur / ${height}px de hauteur). Vous pouvez voir le détail via le menu Découpe."
+msgstr ""
 
 #: imio/smartweb/core/contents/folder/element_view.pt:6
 msgid "The item selected as the folder home page is :"
 msgstr "L'élément sélectionné comme page d'accueil du dossier est :"
 
 #: imio/smartweb/core/contents/sections/base.py:44
 msgid "The title will always be displayed if this behavior is enabled."
@@ -2176,29 +2180,29 @@
 
 #: imio/smartweb/core/contents/pages/views.py:64
 msgid "There is no section on this page."
 msgstr "Il n'y a aucune section dans cette page."
 
 #: imio/smartweb/core/contents/pages/procedure/view.py:13
 msgid "There is no section on this procedure."
-msgstr "Il n'y a aucune section présente dans cette démarche."
+msgstr ""
 
 #: imio/smartweb/core/vocabularies.py:125
 msgid "Third of width"
 msgstr "Tiers de la page"
 
 #: imio/smartweb/core/vocabularies.py:310
 msgid "Third page"
 msgstr "Tiers de la page"
 
 #: imio/smartweb/common/privacy.py:70
 msgid "This feature requires cookies acceptation.<br/><a class=\"pat-plone-modal\" href=\"${consent_url}\">Review your cookies preferences</a>."
 msgstr "Cette fonctionnalité nécessite l'acceptation des cookies.<br/><a class=\"pat-plone-modal\" href=\"${consent_url}\">Modifier vos préférences en matière de cookies</a>."
 
-#: imio/directory/core/contents/contact/content.py:203
+#: imio/directory/core/contents/contact/content.py:231
 #: imio/events/core/contents/event/content.py:48
 #: imio/news/core/contents/newsitem/content.py:34
 msgid "This field is required if the content must be available in this language"
 msgstr "Ce champ est requis si le contenu doit être disponible dans cette langue"
 
 #: imio/smartweb/core/browser/controlpanel.py:91
 msgid "This information is used for search results redirection"
@@ -2208,28 +2212,28 @@
 msgid "This site uses cookies to provide you with an optimal experience (playing videos, displaying maps and content from social networks in particular)."
 msgstr "Ce site utilise des cookies pour vous fournir une expérience optimale (lecture de vidéos, affichage de plans et de contenus issus des réseaux sociaux notamment)."
 
 #: imio/smartweb/core/vocabularies.py:128
 msgid "Three quarter of width"
 msgstr "Trois quarts de la page"
 
-#: imio/smartweb/core/contents/sections/contact/view.py:116
+#: imio/smartweb/core/contents/sections/contact/view.py:130
 msgid "Thursday"
 msgstr "Jeudi"
 
 #: imio/events/core/contents/event/content.py:114
 #: imio/events/core/contents/event/view.pt:67
 msgid "Ticket url"
 msgstr "Billeterie"
 
 #: imio/events/core/contents/event/content.py:115
 msgid "Ticket url to subscribe to this event"
 msgstr "Lien de la billeterie pour s'inscrire à cet événement"
 
-#: imio/directory/core/contents/contact/content.py:202
+#: imio/directory/core/contents/contact/content.py:230
 #: imio/events/core/contents/event/content.py:47
 #: imio/news/core/contents/newsitem/content.py:33
 msgid "Title"
 msgstr "Titre"
 
 #: imio/smartweb/core/vocabularies.py:157
 msgid "Title and Subtitle"
@@ -2257,15 +2261,15 @@
 msgid "Tourist"
 msgstr "Touriste"
 
 #: imio/events/core/vocabularies.py:25
 msgid "Trade Fair and Fair"
 msgstr "Salon et Foire"
 
-#: imio/smartweb/core/contents/sections/contact/view.py:114
+#: imio/smartweb/core/contents/sections/contact/view.py:128
 msgid "Tuesday"
 msgstr "Mardi"
 
 #: imio/directory/core/vocabularies.py:69
 #: imio/events/core/contents/event/content.py:132
 #: imio/events/core/contents/event/view.pt:77
 msgid "Twitter"
@@ -2279,35 +2283,35 @@
 msgid "Twitter url for this news"
 msgstr "Lien Twitter pour cette actualité"
 
 #: imio/smartweb/core/vocabularies.py:127
 msgid "Two third of width"
 msgstr "Deux tiers de la page"
 
-#: imio/directory/core/contents/contact/content.py:54
+#: imio/directory/core/contents/contact/content.py:82
 msgid "Type"
 msgstr ""
 
 #: imio/smartweb/core/contents/blocks/link/content.py:26
 msgid "URL"
 msgstr ""
 
-#: imio/directory/core/contents/contact/content.py:131
+#: imio/directory/core/contents/contact/content.py:159
 msgid "URLs"
 msgstr ""
 
-#: imio/directory/policy/configure.zcml:43
+#: imio/directory/policy/configure.zcml:44
 msgid "Uninstalls the imio.directory.policy add-on."
 msgstr ""
 
-#: imio/events/policy/configure.zcml:44
+#: imio/events/policy/configure.zcml:45
 msgid "Uninstalls the imio.events.policy add-on."
 msgstr ""
 
-#: imio/news/policy/configure.zcml:44
+#: imio/news/policy/configure.zcml:45
 msgid "Uninstalls the imio.news.policy add-on."
 msgstr ""
 
 #: imio/smartweb/policy/upgrades/configure.zcml:76
 msgid "Update caching configuration"
 msgstr ""
 
@@ -2339,14 +2343,18 @@
 msgid "Upgrade common from 1013 to 1014"
 msgstr ""
 
 #: imio/smartweb/common/upgrades/configure.zcml:61
 msgid "Upgrade common from 1014 to 1015"
 msgstr ""
 
+#: imio/smartweb/common/upgrades/configure.zcml:69
+msgid "Upgrade common from 1015 to 1016"
+msgstr ""
+
 #: imio/smartweb/core/upgrades/configure.zcml:92
 msgid "Upgrade common from 1031 to 1032"
 msgstr ""
 
 #: imio/smartweb/core/upgrades/configure.zcml:100
 msgid "Upgrade common from 1033 to 1034"
 msgstr ""
@@ -2497,15 +2505,15 @@
 msgid "Upgrade policy from 1026 to 1027"
 msgstr ""
 
 #: imio/smartweb/policy/upgrades/configure.zcml:124
 msgid "Upgrade policy from 1028 to 1029"
 msgstr ""
 
-#: imio/directory/core/contents/contact/content.py:92
+#: imio/directory/core/contents/contact/content.py:120
 msgid "Url"
 msgstr "URL"
 
 #: imio/smartweb/core/browser/controlpanel.py:25
 msgid "Url to get forms from your e-guichet"
 msgstr "Url de récupération des démarches de votre e-guichet"
 
@@ -2531,15 +2539,15 @@
 msgid "Use custom spotlight to avoid bad gallery refresh"
 msgstr ""
 
 #: imio/directory/core/vocabularies.py:86
 msgid "Useful numbers"
 msgstr "Numéros utiles"
 
-#: imio/directory/core/contents/contact/content.py:109
+#: imio/directory/core/contents/contact/content.py:137
 msgid "VAT number"
 msgstr "Numéro d'entreprise / TVA"
 
 #: imio/smartweb/core/profiles/default/types/imio.smartweb.SectionVideo.xml
 msgid "Video section"
 msgstr "Section vidéo"
 
@@ -2575,20 +2583,24 @@
 msgid "Visible blocks"
 msgstr "Blocs visibles"
 
 #: imio/smartweb/core/browser/controlpanel.py:116
 msgid "Vocabulary term"
 msgstr "Terme du vocabulaire"
 
+#: imio/smartweb/core/browser/overrides/plone.app.content.browser.contents.templates.properties.pt:3
+msgid "Warning: these options are not relevant for Sections and will not be applied."
+msgstr ""
+
 #: imio/directory/core/vocabularies.py:70
 #: imio/news/core/contents/newsitem/content.py:85
 msgid "Website"
 msgstr "Site Internet"
 
-#: imio/smartweb/core/contents/sections/contact/view.py:115
+#: imio/smartweb/core/contents/sections/contact/view.py:129
 msgid "Wednesday"
 msgstr "Mercredi"
 
 #: imio/directory/core/vocabularies.py:54
 msgid "Work email"
 msgstr "Adresse e-mail professionnelle"
 
@@ -2638,35 +2650,35 @@
 msgid "Zipcode '${val}' is not a number."
 msgstr "Le code postal '${val}' n'est pas un nombre."
 
 #: imio/smartweb/common/viewlets/colophon.pt:34
 msgid "free license"
 msgstr "licence libre"
 
-#: imio/directory/policy/configure.zcml:34
+#: imio/directory/policy/configure.zcml:35
 msgid "imio.directory.policy"
 msgstr ""
 
-#: imio/directory/policy/configure.zcml:43
+#: imio/directory/policy/configure.zcml:44
 msgid "imio.directory.policy (uninstall)"
 msgstr ""
 
-#: imio/events/policy/configure.zcml:35
+#: imio/events/policy/configure.zcml:36
 msgid "imio.events.policy"
 msgstr ""
 
-#: imio/events/policy/configure.zcml:44
+#: imio/events/policy/configure.zcml:45
 msgid "imio.events.policy (uninstall)"
 msgstr ""
 
-#: imio/news/policy/configure.zcml:35
+#: imio/news/policy/configure.zcml:36
 msgid "imio.news.policy"
 msgstr ""
 
-#: imio/news/policy/configure.zcml:44
+#: imio/news/policy/configure.zcml:45
 msgid "imio.news.policy (uninstall)"
 msgstr ""
 
 #. Default: "You are editing the default page of a container. If you wanted to edit the container itself, ${go_here}."
 #: imio/smartweb/core/viewlets/default_page_warning.pt:7
 msgid "label_edit_default_page_container"
 msgstr "Vous modifiez actuellement la page d'accueil d'un dossier. Si vous voulez modifier le dossier lui-même, ${go_here}."
```

### Comparing `imio.smartweb.locales-1.1.3/src/imio/smartweb/locales/locales/fr/LC_MESSAGES/plone.po` & `imio.smartweb.locales-1.1.4/src/imio/smartweb/locales/locales/fr/LC_MESSAGES/plone.po`

 * *Files identical despite different names*

### Comparing `imio.smartweb.locales-1.1.3/src/imio/smartweb/locales/locales/nl/LC_MESSAGES/imio.smartweb.po` & `imio.smartweb.locales-1.1.4/src/imio/smartweb/locales/locales/imio.smartweb.pot`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,29 @@
+#--- PLEASE EDIT THE LINES BELOW CORRECTLY ---
+#SOME DESCRIPTIVE TITLE.
+#FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 msgid ""
 msgstr ""
-"Project-Id-Version: 0.1\n"
-"POT-Creation-Date: YEAR-MO-DA HO:MI +ZONE\n"
+"Project-Id-Version: PACKAGE VERSION\n"
+"POT-Creation-Date: 2023-05-05 09:00+0000\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI +ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=(n != 1);\n"
-"Language-Code: nl\n"
-"Language-Name: Nederlands\n"
-"Preferred-Encodings: utf-8\n"
+"Plural-Forms: nplurals=1; plural=0\n"
+"Language-Code: en\n"
+"Language-Name: English\n"
+"Preferred-Encodings: utf-8 latin1\n"
 "Domain: imio.smartweb\n"
-"Language: nl\n"
+
+#: imio/directory/core/contents/contact/content.py:77
+msgid ""
+msgstr ""
 
 #: imio/smartweb/core/contents/sections/base.py:85
 msgid "<div class=\"section_error_txt\">Error in section : \"{}\" <a href=\"{}/edit\">[edit]</a></div>"
 msgstr ""
 
 #: imio/smartweb/common/browser/privacy/form.py:31
 #: imio/smartweb/common/viewlets/privacy.pt:15
@@ -194,15 +200,15 @@
 msgid "Allow to select quick access elements for current context."
 msgstr ""
 
 #: imio/smartweb/core/contents/sections/slide/content.py:53
 msgid "Alternatively as a picture"
 msgstr ""
 
-#: imio/smartweb/core/contents/folder/views.py:132
+#: imio/smartweb/core/contents/folder/views.py:134
 msgid "Apply"
 msgstr ""
 
 #: imio/smartweb/core/viewlets/toolbar.py:19
 msgid "Authentic sources"
 msgstr ""
 
@@ -227,15 +233,15 @@
 msgid "Bad URL format '${val}' (good format sample: https://www.imio.be)."
 msgstr ""
 
 #: imio/directory/core/browser/import.py:90
 msgid "Bad mail format '${val}' (good format sample: noreply@imio.be)."
 msgstr ""
 
-#: imio/directory/core/contents/contact/content.py:42
+#: imio/directory/core/contents/contact/content.py:44
 msgid "Bad phone format"
 msgstr ""
 
 #: imio/directory/core/browser/import.py:72
 msgid "Bad phone format '${val}' (good format sample: +32444556677)."
 msgstr ""
 
@@ -285,15 +291,15 @@
 msgid "CSV file"
 msgstr ""
 
 #: imio/smartweb/common/sharing/localroles.py:12
 msgid "Can manage locally"
 msgstr ""
 
-#: imio/smartweb/core/vocabularies.py:570
+#: imio/smartweb/core/vocabularies.py:571
 msgid "Carousel"
 msgstr ""
 
 #: imio/smartweb/core/contents/sections/links/configure.zcml:26
 #: imio/smartweb/core/contents/sections/selections/configure.zcml:26
 msgid "Carousel view"
 msgstr ""
@@ -552,15 +558,15 @@
 msgid "Click to preview content (without editor actions)."
 msgstr ""
 
 #: imio/smartweb/core/viewlets/navigation.py:85
 msgid "Close"
 msgstr ""
 
-#: imio/smartweb/core/contents/sections/contact/view.py:258
+#: imio/smartweb/core/contents/sections/contact/view.py:272
 msgid "Closed"
 msgstr ""
 
 #: imio/smartweb/core/profiles/default/types/imio.smartweb.SectionCollection.xml
 msgid "Collection section"
 msgstr ""
 
@@ -599,15 +605,15 @@
 msgid "Contact"
 msgstr ""
 
 #: imio/directory/core/profiles/default/types/imio.directory.Contact.xml
 msgid "Contact content type"
 msgstr ""
 
-#: imio/directory/core/contents/contact/content.py:106
+#: imio/directory/core/contents/contact/content.py:134
 #: imio/smartweb/core/vocabularies.py:158
 msgid "Contact informations"
 msgstr ""
 
 #: imio/smartweb/core/profiles/default/types/imio.smartweb.SectionContact.xml
 msgid "Contact section"
 msgstr ""
@@ -672,15 +678,15 @@
 msgid "Define number of levels in menu navigation subsite"
 msgstr ""
 
 #: imio/smartweb/core/contents/sections/macros.pt:57
 msgid "Delete section"
 msgstr ""
 
-#: imio/directory/core/contents/contact/content.py:209
+#: imio/directory/core/contents/contact/content.py:237
 #: imio/events/core/contents/event/content.py:53
 #: imio/news/core/contents/newsitem/content.py:39
 msgid "Description"
 msgstr ""
 
 #: imio/smartweb/core/browser/controlpanel.py:72
 msgid "Directory SolR Core ID"
@@ -727,29 +733,29 @@
 msgid "Display linked news from imio news instance."
 msgstr ""
 
 #: imio/directory/core/vocabularies.py:85
 msgid "Drinking water point"
 msgstr ""
 
-#: imio/directory/core/contents/contact/content.py:232
+#: imio/directory/core/contents/contact/content.py:260
 #: imio/events/core/contents/event/content.py:77
 #: imio/news/core/contents/newsitem/content.py:63
 msgid "Dutch translations"
 msgstr ""
 
 #: imio/smartweb/core/contents/pages/procedure/content.py:21
 msgid "E-Guichet procedure"
 msgstr ""
 
-#: imio/directory/core/contents/contact/content.py:81
+#: imio/directory/core/contents/contact/content.py:109
 msgid "E-mail"
 msgstr ""
 
-#: imio/directory/core/contents/contact/content.py:121
+#: imio/directory/core/contents/contact/content.py:149
 msgid "E-mails"
 msgstr ""
 
 #: imio/smartweb/common/vocabularies.py:22
 msgid "Economics"
 msgstr ""
 
@@ -781,15 +787,15 @@
 msgid "Enable minisite"
 msgstr ""
 
 #: imio/smartweb/core/profiles/default/actions.xml
 msgid "Enable subsite"
 msgstr ""
 
-#: imio/directory/core/contents/contact/content.py:215
+#: imio/directory/core/contents/contact/content.py:243
 #: imio/events/core/contents/event/content.py:60
 #: imio/news/core/contents/newsitem/content.py:46
 msgid "English translations"
 msgstr ""
 
 #: imio/smartweb/core/browser/controlpanel.py:17
 msgid "Enter the language code. Ex.: en"
@@ -875,15 +881,15 @@
 msgid "Example : Photo of a person or organization building"
 msgstr ""
 
 #: imio/smartweb/core/browser/controlpanel.py:26
 msgid "Example : https://COMMUNE-formulaires.guichet-citoyen.be/api/formdefs/"
 msgstr ""
 
-#: imio/directory/core/contents/contact/content.py:269
+#: imio/directory/core/contents/contact/content.py:297
 msgid "Example : shop, service, association logo"
 msgstr ""
 
 #: imio/smartweb/core/behaviors/listing.py:19
 msgid "Exclude from parent listing"
 msgstr ""
 
@@ -933,15 +939,15 @@
 msgid "Faceted summary view"
 msgstr ""
 
 #: imio/smartweb/core/browser/faceted/configure.zcml:88
 msgid "Faceted summary view with images"
 msgstr ""
 
-#: imio/directory/core/contents/contact/content.py:286
+#: imio/directory/core/contents/contact/content.py:314
 msgid "Facilities"
 msgstr ""
 
 #: imio/events/core/contents/event/content.py:151
 #: imio/events/core/contents/event/view.pt:57
 msgid "Facilities for person with reduced mobility"
 msgstr ""
@@ -1014,28 +1020,28 @@
 msgid "Footer has been successfully added"
 msgstr ""
 
 #: imio/smartweb/core/contents/folder/content.py:26
 msgid "For the anonymous visitor, the folder and the selected item are one. When he clicks on the folder, the item is displayed."
 msgstr ""
 
-#: imio/smartweb/core/contents/folder/views.py:103
+#: imio/smartweb/core/contents/folder/views.py:105
 msgid "Form to choose item to be displayed as the home page of the folder"
 msgstr ""
 
 #: imio/directory/core/vocabularies.py:88
 msgid "Free WIFI"
 msgstr ""
 
 #: imio/events/core/contents/event/content.py:144
 #: imio/events/core/contents/event/view.pt:47
 msgid "Free entry"
 msgstr ""
 
-#: imio/smartweb/core/contents/sections/contact/view.py:117
+#: imio/smartweb/core/contents/sections/contact/view.py:131
 msgid "Friday"
 msgstr ""
 
 #: imio/smartweb/core/contents/sections/events/macros.pt:13
 msgid "From"
 msgstr ""
 
@@ -1055,15 +1061,15 @@
 msgid "Gallery section"
 msgstr ""
 
 #: imio/smartweb/core/profiles/default/types/imio.smartweb.SectionGallery.xml
 msgid "Gallery section for a page"
 msgstr ""
 
-#: imio/directory/core/contents/contact/content.py:198
+#: imio/directory/core/contents/contact/content.py:226
 #: imio/events/core/contents/event/content.py:43
 #: imio/news/core/contents/newsitem/content.py:29
 msgid "German translations"
 msgstr ""
 
 #: imio/smartweb/core/contents/sections/events/content.py:37
 msgid "Get priory on related agenda for these specifics events."
@@ -1209,15 +1215,15 @@
 msgstr ""
 
 #: imio/events/core/contents/event/content.py:175
 #: imio/news/core/contents/newsitem/content.py:130
 msgid "Important! These categories are used to supplement the information provided by the topics"
 msgstr ""
 
-#: imio/directory/core/contents/contact/content.py:287
+#: imio/directory/core/contents/contact/content.py:315
 msgid "Important! These categories make it possible to highlight and geolocate certain basic services"
 msgstr ""
 
 #: imio/smartweb/common/behaviors/topics.py:17
 msgid "Important! Topics are used to filter search results and create lists"
 msgstr ""
 
@@ -1235,41 +1241,41 @@
 msgid "Instagram url for this event"
 msgstr ""
 
 #: imio/news/core/contents/newsitem/content.py:110
 msgid "Instagram url for this news"
 msgstr ""
 
-#: imio/directory/policy/configure.zcml:34
+#: imio/directory/policy/configure.zcml:35
 msgid "Installs the imio.directory.policy add-on."
 msgstr ""
 
-#: imio/events/policy/configure.zcml:35
+#: imio/events/policy/configure.zcml:36
 msgid "Installs the imio.events.policy add-on."
 msgstr ""
 
-#: imio/news/policy/configure.zcml:35
+#: imio/news/policy/configure.zcml:36
 msgid "Installs the imio.news.policy add-on."
 msgstr ""
 
-#: imio/directory/core/contents/contact/content.py:179
+#: imio/directory/core/contents/contact/content.py:207
 msgid "Internal note"
 msgstr ""
 
 #: imio/events/core/vocabularies.py:26
 msgid "Internships and courses"
 msgstr ""
 
 #: imio/smartweb/core/contents/folder/content.py:25
 msgid "Item(s) that can be selected as the folder default page."
 msgstr ""
 
-#: imio/events/core/contents/event/views.py:75
+#: imio/events/core/contents/event/views.py:77
 #: imio/smartweb/core/contents/sections/contact/view.pt:122
-#: imio/smartweb/core/contents/sections/contact/view.py:62
+#: imio/smartweb/core/contents/sections/contact/view.py:77
 msgid "Itinerary"
 msgstr ""
 
 #: imio/news/core/vocabularies.py:18
 msgid "Job offer"
 msgstr ""
 
@@ -1282,19 +1288,19 @@
 msgstr ""
 
 #: imio/events/core/contents/event/view.pt:107
 #: imio/news/core/contents/newsitem/view.pt:64
 msgid "Keywords"
 msgstr ""
 
-#: imio/directory/core/contents/contact/content.py:69
+#: imio/directory/core/contents/contact/content.py:97
 msgid "Label (Secretariat, Manager office, Sales,...)"
 msgstr ""
 
-#: imio/directory/core/contents/contact/content.py:48
+#: imio/directory/core/contents/contact/content.py:76
 msgid "Label (direction, Main number,...)"
 msgstr ""
 
 #: imio/smartweb/core/browser/controlpanel.py:16
 msgid "Language (en, fr,...)"
 msgstr ""
 
@@ -1368,30 +1374,30 @@
 msgid "List of events categories values available for this entity (one per line)"
 msgstr ""
 
 #: imio/news/core/contents/entity/content.py:26
 msgid "List of news categories values available for this entity (one per line)"
 msgstr ""
 
-#: imio/directory/core/contents/contact/content.py:268
+#: imio/directory/core/contents/contact/content.py:296
 #: imio/smartweb/core/behaviors/minisite.py:41
 #: imio/smartweb/core/behaviors/subsite.py:33
 msgid "Logo"
 msgstr ""
 
 #: imio/smartweb/core/vocabularies.py:143
 msgid "Logo and title"
 msgstr ""
 
 #: imio/smartweb/core/behaviors/minisite.py:47
 #: imio/smartweb/core/behaviors/subsite.py:39
 msgid "Logo display"
 msgstr ""
 
-#: imio/smartweb/core/contents/sections/contact/view.py:288
+#: imio/smartweb/core/contents/sections/contact/view.py:302
 msgid "Lunch time"
 msgstr ""
 
 #: imio/smartweb/core/contents/sections/macros.pt:46
 msgid "Manage section contents"
 msgstr ""
 
@@ -1458,15 +1464,15 @@
 msgid "Mobility"
 msgstr ""
 
 #: imio/smartweb/core/contents/sections/macros.pt:63
 msgid "Modified"
 msgstr ""
 
-#: imio/smartweb/core/contents/sections/contact/view.py:113
+#: imio/smartweb/core/contents/sections/contact/view.py:127
 msgid "Monday"
 msgstr ""
 
 #: imio/smartweb/core/profiles/default/actions.xml
 msgid "My account"
 msgstr ""
 
@@ -1526,15 +1532,15 @@
 msgid "Not allowed to add Files or Images in imio.directory.Entity"
 msgstr ""
 
 #: imio/smartweb/common/interfaces.py:34
 msgid "Number"
 msgstr ""
 
-#: imio/directory/core/contents/contact/content.py:61
+#: imio/directory/core/contents/contact/content.py:89
 msgid "Number (format: +32475010203)"
 msgstr ""
 
 #: imio/smartweb/core/contents/sections/collection/content.py:41
 #: imio/smartweb/core/contents/sections/events/content.py:63
 #: imio/smartweb/core/contents/sections/files/content.py:15
 msgid "Number of items per batch"
@@ -1566,19 +1572,19 @@
 msgid "Only one procedure field can be filled !"
 msgstr ""
 
 #: imio/smartweb/core/contents/blocks/link/content.py:34
 msgid "Only used in table view (takes precedence over image)"
 msgstr ""
 
-#: imio/smartweb/core/contents/sections/contact/view.py:265
+#: imio/smartweb/core/contents/sections/contact/view.py:279
 msgid "Open"
 msgstr ""
 
-#: imio/smartweb/core/contents/sections/contact/view.py:282
+#: imio/smartweb/core/contents/sections/contact/view.py:296
 msgid "Open at "
 msgstr ""
 
 #: imio/smartweb/core/contents/blocks/link/content.py:23
 #: imio/smartweb/core/contents/sections/slide/content.py:66
 msgid "Open in a new tab"
 msgstr ""
@@ -1631,23 +1637,27 @@
 msgid "Parent listing"
 msgstr ""
 
 #: imio/events/core/vocabularies.py:23
 msgid "Party and folklore"
 msgstr ""
 
+#: imio/smartweb/common/upgrades/configure.zcml:69
+msgid "Patch (Remove select2) eea.facetednavigation jquery"
+msgstr ""
+
 #: imio/directory/core/vocabularies.py:53
 msgid "Personal email"
 msgstr ""
 
 #: imio/directory/core/vocabularies.py:39
 msgid "Personal phone"
 msgstr ""
 
-#: imio/directory/core/contents/contact/content.py:111
+#: imio/directory/core/contents/contact/content.py:139
 msgid "Phones"
 msgstr ""
 
 #: imio/smartweb/core/contents/sections/slide/content.py:41
 msgid "Picture will be displayed as slide background"
 msgstr ""
 
@@ -1705,15 +1715,15 @@
 msgid "Presse"
 msgstr ""
 
 #: imio/smartweb/core/profiles/default/actions.xml
 msgid "Preview"
 msgstr ""
 
-#: imio/directory/core/contents/contact/content.py:144
+#: imio/directory/core/contents/contact/content.py:172
 msgid "Private contact informations"
 msgstr ""
 
 #: imio/smartweb/core/profiles/default/types/imio.smartweb.Procedure.xml
 msgid "Procedure"
 msgstr ""
 
@@ -1803,15 +1813,15 @@
 msgid "Right"
 msgstr ""
 
 #: imio/smartweb/common/vocabularies.py:30
 msgid "Safety and prevention"
 msgstr ""
 
-#: imio/smartweb/core/contents/sections/contact/view.py:118
+#: imio/smartweb/core/contents/sections/contact/view.py:132
 msgid "Saturday"
 msgstr ""
 
 #: imio/smartweb/common/browser/privacy/form.py:27
 msgid "Save my choices"
 msgstr ""
 
@@ -1828,19 +1838,19 @@
 msgid "Secret key"
 msgstr ""
 
 #: imio/smartweb/core/browser/controlpanel.py:34
 msgid "Secret key to use API"
 msgstr ""
 
-#: imio/smartweb/core/contents/sections/views.py:34
+#: imio/smartweb/core/contents/sections/views.py:44
 msgid "Section title has been hidden"
 msgstr ""
 
-#: imio/smartweb/core/contents/sections/views.py:41
+#: imio/smartweb/core/contents/sections/views.py:51
 msgid "Section title has been shown"
 msgstr ""
 
 #: imio/smartweb/core/contents/sections/base.py:58
 msgid "Section width"
 msgstr ""
 
@@ -1868,15 +1878,15 @@
 msgid "Select agenda to display"
 msgstr ""
 
 #: imio/events/core/contents/event/content.py:165
 msgid "Select agendas where this event will be displayed. Current agenda is always selected."
 msgstr ""
 
-#: imio/directory/core/contents/contact/content.py:277
+#: imio/directory/core/contents/contact/content.py:305
 msgid "Select entities where this contact will be displayed. Current entity will always be selected."
 msgstr ""
 
 #: imio/smartweb/core/contents/sections/text/content.py:37
 msgid "Select image size"
 msgstr ""
 
@@ -1908,15 +1918,15 @@
 msgid "Selected agenda"
 msgstr ""
 
 #: imio/events/core/contents/event/content.py:164
 msgid "Selected agendas"
 msgstr ""
 
-#: imio/directory/core/contents/contact/content.py:276
+#: imio/directory/core/contents/contact/content.py:304
 msgid "Selected entities"
 msgstr ""
 
 #: imio/smartweb/core/contents/rest/events/content.py:17
 msgid "Selected event types"
 msgstr ""
 
@@ -2089,28 +2099,28 @@
 msgid "Subsite has been disabled"
 msgstr ""
 
 #: imio/smartweb/core/browser/subsite/settings.py:25
 msgid "Subsite has been successfully activated"
 msgstr ""
 
-#: imio/directory/core/contents/contact/content.py:208
+#: imio/directory/core/contents/contact/content.py:236
 #: imio/smartweb/core/contents/sections/postit/content.py:26
 msgid "Subtitle"
 msgstr ""
 
 #: imio/smartweb/core/contents/folder/configure.zcml:72
 msgid "Summary view"
 msgstr ""
 
 #: imio/smartweb/core/contents/folder/configure.zcml:83
 msgid "Summary view with images"
 msgstr ""
 
-#: imio/smartweb/core/contents/sections/contact/view.py:119
+#: imio/smartweb/core/contents/sections/contact/view.py:133
 msgid "Sunday"
 msgstr ""
 
 #: imio/smartweb/core/contents/sections/contact/content.py:47
 msgid "Switch lead image to portrait mode"
 msgstr ""
 
@@ -2189,15 +2199,15 @@
 msgid "Third page"
 msgstr ""
 
 #: imio/smartweb/common/privacy.py:70
 msgid "This feature requires cookies acceptation.<br/><a class=\"pat-plone-modal\" href=\"${consent_url}\">Review your cookies preferences</a>."
 msgstr ""
 
-#: imio/directory/core/contents/contact/content.py:203
+#: imio/directory/core/contents/contact/content.py:231
 #: imio/events/core/contents/event/content.py:48
 #: imio/news/core/contents/newsitem/content.py:34
 msgid "This field is required if the content must be available in this language"
 msgstr ""
 
 #: imio/smartweb/core/browser/controlpanel.py:91
 msgid "This information is used for search results redirection"
@@ -2207,28 +2217,28 @@
 msgid "This site uses cookies to provide you with an optimal experience (playing videos, displaying maps and content from social networks in particular)."
 msgstr ""
 
 #: imio/smartweb/core/vocabularies.py:128
 msgid "Three quarter of width"
 msgstr ""
 
-#: imio/smartweb/core/contents/sections/contact/view.py:116
+#: imio/smartweb/core/contents/sections/contact/view.py:130
 msgid "Thursday"
 msgstr ""
 
 #: imio/events/core/contents/event/content.py:114
 #: imio/events/core/contents/event/view.pt:67
 msgid "Ticket url"
 msgstr ""
 
 #: imio/events/core/contents/event/content.py:115
 msgid "Ticket url to subscribe to this event"
 msgstr ""
 
-#: imio/directory/core/contents/contact/content.py:202
+#: imio/directory/core/contents/contact/content.py:230
 #: imio/events/core/contents/event/content.py:47
 #: imio/news/core/contents/newsitem/content.py:33
 msgid "Title"
 msgstr ""
 
 #: imio/smartweb/core/vocabularies.py:157
 msgid "Title and Subtitle"
@@ -2256,15 +2266,15 @@
 msgid "Tourist"
 msgstr ""
 
 #: imio/events/core/vocabularies.py:25
 msgid "Trade Fair and Fair"
 msgstr ""
 
-#: imio/smartweb/core/contents/sections/contact/view.py:114
+#: imio/smartweb/core/contents/sections/contact/view.py:128
 msgid "Tuesday"
 msgstr ""
 
 #: imio/directory/core/vocabularies.py:69
 #: imio/events/core/contents/event/content.py:132
 #: imio/events/core/contents/event/view.pt:77
 msgid "Twitter"
@@ -2278,35 +2288,35 @@
 msgid "Twitter url for this news"
 msgstr ""
 
 #: imio/smartweb/core/vocabularies.py:127
 msgid "Two third of width"
 msgstr ""
 
-#: imio/directory/core/contents/contact/content.py:54
+#: imio/directory/core/contents/contact/content.py:82
 msgid "Type"
 msgstr ""
 
 #: imio/smartweb/core/contents/blocks/link/content.py:26
 msgid "URL"
 msgstr ""
 
-#: imio/directory/core/contents/contact/content.py:131
+#: imio/directory/core/contents/contact/content.py:159
 msgid "URLs"
 msgstr ""
 
-#: imio/directory/policy/configure.zcml:43
+#: imio/directory/policy/configure.zcml:44
 msgid "Uninstalls the imio.directory.policy add-on."
 msgstr ""
 
-#: imio/events/policy/configure.zcml:44
+#: imio/events/policy/configure.zcml:45
 msgid "Uninstalls the imio.events.policy add-on."
 msgstr ""
 
-#: imio/news/policy/configure.zcml:44
+#: imio/news/policy/configure.zcml:45
 msgid "Uninstalls the imio.news.policy add-on."
 msgstr ""
 
 #: imio/smartweb/policy/upgrades/configure.zcml:76
 msgid "Update caching configuration"
 msgstr ""
 
@@ -2338,14 +2348,18 @@
 msgid "Upgrade common from 1013 to 1014"
 msgstr ""
 
 #: imio/smartweb/common/upgrades/configure.zcml:61
 msgid "Upgrade common from 1014 to 1015"
 msgstr ""
 
+#: imio/smartweb/common/upgrades/configure.zcml:69
+msgid "Upgrade common from 1015 to 1016"
+msgstr ""
+
 #: imio/smartweb/core/upgrades/configure.zcml:92
 msgid "Upgrade common from 1031 to 1032"
 msgstr ""
 
 #: imio/smartweb/core/upgrades/configure.zcml:100
 msgid "Upgrade common from 1033 to 1034"
 msgstr ""
@@ -2496,15 +2510,15 @@
 msgid "Upgrade policy from 1026 to 1027"
 msgstr ""
 
 #: imio/smartweb/policy/upgrades/configure.zcml:124
 msgid "Upgrade policy from 1028 to 1029"
 msgstr ""
 
-#: imio/directory/core/contents/contact/content.py:92
+#: imio/directory/core/contents/contact/content.py:120
 msgid "Url"
 msgstr ""
 
 #: imio/smartweb/core/browser/controlpanel.py:25
 msgid "Url to get forms from your e-guichet"
 msgstr ""
 
@@ -2530,15 +2544,15 @@
 msgid "Use custom spotlight to avoid bad gallery refresh"
 msgstr ""
 
 #: imio/directory/core/vocabularies.py:86
 msgid "Useful numbers"
 msgstr ""
 
-#: imio/directory/core/contents/contact/content.py:109
+#: imio/directory/core/contents/contact/content.py:137
 msgid "VAT number"
 msgstr ""
 
 #: imio/smartweb/core/profiles/default/types/imio.smartweb.SectionVideo.xml
 msgid "Video section"
 msgstr ""
 
@@ -2574,20 +2588,24 @@
 msgid "Visible blocks"
 msgstr ""
 
 #: imio/smartweb/core/browser/controlpanel.py:116
 msgid "Vocabulary term"
 msgstr ""
 
+#: imio/smartweb/core/browser/overrides/plone.app.content.browser.contents.templates.properties.pt:3
+msgid "Warning: these options are not relevant for Sections and will not be applied."
+msgstr ""
+
 #: imio/directory/core/vocabularies.py:70
 #: imio/news/core/contents/newsitem/content.py:85
 msgid "Website"
 msgstr ""
 
-#: imio/smartweb/core/contents/sections/contact/view.py:115
+#: imio/smartweb/core/contents/sections/contact/view.py:129
 msgid "Wednesday"
 msgstr ""
 
 #: imio/directory/core/vocabularies.py:54
 msgid "Work email"
 msgstr ""
 
@@ -2637,35 +2655,35 @@
 msgid "Zipcode '${val}' is not a number."
 msgstr ""
 
 #: imio/smartweb/common/viewlets/colophon.pt:34
 msgid "free license"
 msgstr ""
 
-#: imio/directory/policy/configure.zcml:34
+#: imio/directory/policy/configure.zcml:35
 msgid "imio.directory.policy"
 msgstr ""
 
-#: imio/directory/policy/configure.zcml:43
+#: imio/directory/policy/configure.zcml:44
 msgid "imio.directory.policy (uninstall)"
 msgstr ""
 
-#: imio/events/policy/configure.zcml:35
+#: imio/events/policy/configure.zcml:36
 msgid "imio.events.policy"
 msgstr ""
 
-#: imio/events/policy/configure.zcml:44
+#: imio/events/policy/configure.zcml:45
 msgid "imio.events.policy (uninstall)"
 msgstr ""
 
-#: imio/news/policy/configure.zcml:35
+#: imio/news/policy/configure.zcml:36
 msgid "imio.news.policy"
 msgstr ""
 
-#: imio/news/policy/configure.zcml:44
+#: imio/news/policy/configure.zcml:45
 msgid "imio.news.policy (uninstall)"
 msgstr ""
 
 #. Default: "You are editing the default page of a container. If you wanted to edit the container itself, ${go_here}."
 #: imio/smartweb/core/viewlets/default_page_warning.pt:7
 msgid "label_edit_default_page_container"
 msgstr ""
```

### Comparing `imio.smartweb.locales-1.1.3/src/imio/smartweb/locales/locales/nl/LC_MESSAGES/plone.po` & `imio.smartweb.locales-1.1.4/src/imio/smartweb/locales/locales/nl/LC_MESSAGES/plone.po`

 * *Files identical despite different names*

### Comparing `imio.smartweb.locales-1.1.3/src/imio/smartweb/locales/locales/imio.smartweb.pot` & `imio.smartweb.locales-1.1.4/src/imio/smartweb/locales/locales/nl/LC_MESSAGES/imio.smartweb.po`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,23 @@
-#--- PLEASE EDIT THE LINES BELOW CORRECTLY ---
-#SOME DESCRIPTIVE TITLE.
-#FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 msgid ""
 msgstr ""
-"Project-Id-Version: PACKAGE VERSION\n"
-"POT-Creation-Date: 2023-03-10 09:52+0000\n"
+"Project-Id-Version: 0.1\n"
+"POT-Creation-Date: YEAR-MO-DA HO:MI +ZONE\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI +ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=1; plural=0\n"
-"Language-Code: en\n"
-"Language-Name: English\n"
-"Preferred-Encodings: utf-8 latin1\n"
+"Plural-Forms: nplurals=2; plural=(n != 1);\n"
+"Language-Code: nl\n"
+"Language-Name: Nederlands\n"
+"Preferred-Encodings: utf-8\n"
 "Domain: imio.smartweb\n"
-
-#: imio/directory/core/contents/contact/content.py:49
-msgid ""
-msgstr ""
+"Language: nl\n"
 
 #: imio/smartweb/core/contents/sections/base.py:85
 msgid "<div class=\"section_error_txt\">Error in section : \"{}\" <a href=\"{}/edit\">[edit]</a></div>"
 msgstr ""
 
 #: imio/smartweb/common/browser/privacy/form.py:31
 #: imio/smartweb/common/viewlets/privacy.pt:15
@@ -200,15 +194,15 @@
 msgid "Allow to select quick access elements for current context."
 msgstr ""
 
 #: imio/smartweb/core/contents/sections/slide/content.py:53
 msgid "Alternatively as a picture"
 msgstr ""
 
-#: imio/smartweb/core/contents/folder/views.py:132
+#: imio/smartweb/core/contents/folder/views.py:134
 msgid "Apply"
 msgstr ""
 
 #: imio/smartweb/core/viewlets/toolbar.py:19
 msgid "Authentic sources"
 msgstr ""
 
@@ -233,15 +227,15 @@
 msgid "Bad URL format '${val}' (good format sample: https://www.imio.be)."
 msgstr ""
 
 #: imio/directory/core/browser/import.py:90
 msgid "Bad mail format '${val}' (good format sample: noreply@imio.be)."
 msgstr ""
 
-#: imio/directory/core/contents/contact/content.py:42
+#: imio/directory/core/contents/contact/content.py:44
 msgid "Bad phone format"
 msgstr ""
 
 #: imio/directory/core/browser/import.py:72
 msgid "Bad phone format '${val}' (good format sample: +32444556677)."
 msgstr ""
 
@@ -291,15 +285,15 @@
 msgid "CSV file"
 msgstr ""
 
 #: imio/smartweb/common/sharing/localroles.py:12
 msgid "Can manage locally"
 msgstr ""
 
-#: imio/smartweb/core/vocabularies.py:570
+#: imio/smartweb/core/vocabularies.py:571
 msgid "Carousel"
 msgstr ""
 
 #: imio/smartweb/core/contents/sections/links/configure.zcml:26
 #: imio/smartweb/core/contents/sections/selections/configure.zcml:26
 msgid "Carousel view"
 msgstr ""
@@ -558,15 +552,15 @@
 msgid "Click to preview content (without editor actions)."
 msgstr ""
 
 #: imio/smartweb/core/viewlets/navigation.py:85
 msgid "Close"
 msgstr ""
 
-#: imio/smartweb/core/contents/sections/contact/view.py:258
+#: imio/smartweb/core/contents/sections/contact/view.py:272
 msgid "Closed"
 msgstr ""
 
 #: imio/smartweb/core/profiles/default/types/imio.smartweb.SectionCollection.xml
 msgid "Collection section"
 msgstr ""
 
@@ -605,15 +599,15 @@
 msgid "Contact"
 msgstr ""
 
 #: imio/directory/core/profiles/default/types/imio.directory.Contact.xml
 msgid "Contact content type"
 msgstr ""
 
-#: imio/directory/core/contents/contact/content.py:106
+#: imio/directory/core/contents/contact/content.py:134
 #: imio/smartweb/core/vocabularies.py:158
 msgid "Contact informations"
 msgstr ""
 
 #: imio/smartweb/core/profiles/default/types/imio.smartweb.SectionContact.xml
 msgid "Contact section"
 msgstr ""
@@ -678,15 +672,15 @@
 msgid "Define number of levels in menu navigation subsite"
 msgstr ""
 
 #: imio/smartweb/core/contents/sections/macros.pt:57
 msgid "Delete section"
 msgstr ""
 
-#: imio/directory/core/contents/contact/content.py:209
+#: imio/directory/core/contents/contact/content.py:237
 #: imio/events/core/contents/event/content.py:53
 #: imio/news/core/contents/newsitem/content.py:39
 msgid "Description"
 msgstr ""
 
 #: imio/smartweb/core/browser/controlpanel.py:72
 msgid "Directory SolR Core ID"
@@ -733,29 +727,29 @@
 msgid "Display linked news from imio news instance."
 msgstr ""
 
 #: imio/directory/core/vocabularies.py:85
 msgid "Drinking water point"
 msgstr ""
 
-#: imio/directory/core/contents/contact/content.py:232
+#: imio/directory/core/contents/contact/content.py:260
 #: imio/events/core/contents/event/content.py:77
 #: imio/news/core/contents/newsitem/content.py:63
 msgid "Dutch translations"
 msgstr ""
 
 #: imio/smartweb/core/contents/pages/procedure/content.py:21
 msgid "E-Guichet procedure"
 msgstr ""
 
-#: imio/directory/core/contents/contact/content.py:81
+#: imio/directory/core/contents/contact/content.py:109
 msgid "E-mail"
 msgstr ""
 
-#: imio/directory/core/contents/contact/content.py:121
+#: imio/directory/core/contents/contact/content.py:149
 msgid "E-mails"
 msgstr ""
 
 #: imio/smartweb/common/vocabularies.py:22
 msgid "Economics"
 msgstr ""
 
@@ -787,15 +781,15 @@
 msgid "Enable minisite"
 msgstr ""
 
 #: imio/smartweb/core/profiles/default/actions.xml
 msgid "Enable subsite"
 msgstr ""
 
-#: imio/directory/core/contents/contact/content.py:215
+#: imio/directory/core/contents/contact/content.py:243
 #: imio/events/core/contents/event/content.py:60
 #: imio/news/core/contents/newsitem/content.py:46
 msgid "English translations"
 msgstr ""
 
 #: imio/smartweb/core/browser/controlpanel.py:17
 msgid "Enter the language code. Ex.: en"
@@ -881,15 +875,15 @@
 msgid "Example : Photo of a person or organization building"
 msgstr ""
 
 #: imio/smartweb/core/browser/controlpanel.py:26
 msgid "Example : https://COMMUNE-formulaires.guichet-citoyen.be/api/formdefs/"
 msgstr ""
 
-#: imio/directory/core/contents/contact/content.py:269
+#: imio/directory/core/contents/contact/content.py:297
 msgid "Example : shop, service, association logo"
 msgstr ""
 
 #: imio/smartweb/core/behaviors/listing.py:19
 msgid "Exclude from parent listing"
 msgstr ""
 
@@ -939,15 +933,15 @@
 msgid "Faceted summary view"
 msgstr ""
 
 #: imio/smartweb/core/browser/faceted/configure.zcml:88
 msgid "Faceted summary view with images"
 msgstr ""
 
-#: imio/directory/core/contents/contact/content.py:286
+#: imio/directory/core/contents/contact/content.py:314
 msgid "Facilities"
 msgstr ""
 
 #: imio/events/core/contents/event/content.py:151
 #: imio/events/core/contents/event/view.pt:57
 msgid "Facilities for person with reduced mobility"
 msgstr ""
@@ -1020,28 +1014,28 @@
 msgid "Footer has been successfully added"
 msgstr ""
 
 #: imio/smartweb/core/contents/folder/content.py:26
 msgid "For the anonymous visitor, the folder and the selected item are one. When he clicks on the folder, the item is displayed."
 msgstr ""
 
-#: imio/smartweb/core/contents/folder/views.py:103
+#: imio/smartweb/core/contents/folder/views.py:105
 msgid "Form to choose item to be displayed as the home page of the folder"
 msgstr ""
 
 #: imio/directory/core/vocabularies.py:88
 msgid "Free WIFI"
 msgstr ""
 
 #: imio/events/core/contents/event/content.py:144
 #: imio/events/core/contents/event/view.pt:47
 msgid "Free entry"
 msgstr ""
 
-#: imio/smartweb/core/contents/sections/contact/view.py:117
+#: imio/smartweb/core/contents/sections/contact/view.py:131
 msgid "Friday"
 msgstr ""
 
 #: imio/smartweb/core/contents/sections/events/macros.pt:13
 msgid "From"
 msgstr ""
 
@@ -1061,15 +1055,15 @@
 msgid "Gallery section"
 msgstr ""
 
 #: imio/smartweb/core/profiles/default/types/imio.smartweb.SectionGallery.xml
 msgid "Gallery section for a page"
 msgstr ""
 
-#: imio/directory/core/contents/contact/content.py:198
+#: imio/directory/core/contents/contact/content.py:226
 #: imio/events/core/contents/event/content.py:43
 #: imio/news/core/contents/newsitem/content.py:29
 msgid "German translations"
 msgstr ""
 
 #: imio/smartweb/core/contents/sections/events/content.py:37
 msgid "Get priory on related agenda for these specifics events."
@@ -1215,15 +1209,15 @@
 msgstr ""
 
 #: imio/events/core/contents/event/content.py:175
 #: imio/news/core/contents/newsitem/content.py:130
 msgid "Important! These categories are used to supplement the information provided by the topics"
 msgstr ""
 
-#: imio/directory/core/contents/contact/content.py:287
+#: imio/directory/core/contents/contact/content.py:315
 msgid "Important! These categories make it possible to highlight and geolocate certain basic services"
 msgstr ""
 
 #: imio/smartweb/common/behaviors/topics.py:17
 msgid "Important! Topics are used to filter search results and create lists"
 msgstr ""
 
@@ -1241,41 +1235,41 @@
 msgid "Instagram url for this event"
 msgstr ""
 
 #: imio/news/core/contents/newsitem/content.py:110
 msgid "Instagram url for this news"
 msgstr ""
 
-#: imio/directory/policy/configure.zcml:34
+#: imio/directory/policy/configure.zcml:35
 msgid "Installs the imio.directory.policy add-on."
 msgstr ""
 
-#: imio/events/policy/configure.zcml:35
+#: imio/events/policy/configure.zcml:36
 msgid "Installs the imio.events.policy add-on."
 msgstr ""
 
-#: imio/news/policy/configure.zcml:35
+#: imio/news/policy/configure.zcml:36
 msgid "Installs the imio.news.policy add-on."
 msgstr ""
 
-#: imio/directory/core/contents/contact/content.py:179
+#: imio/directory/core/contents/contact/content.py:207
 msgid "Internal note"
 msgstr ""
 
 #: imio/events/core/vocabularies.py:26
 msgid "Internships and courses"
 msgstr ""
 
 #: imio/smartweb/core/contents/folder/content.py:25
 msgid "Item(s) that can be selected as the folder default page."
 msgstr ""
 
-#: imio/events/core/contents/event/views.py:75
+#: imio/events/core/contents/event/views.py:77
 #: imio/smartweb/core/contents/sections/contact/view.pt:122
-#: imio/smartweb/core/contents/sections/contact/view.py:62
+#: imio/smartweb/core/contents/sections/contact/view.py:77
 msgid "Itinerary"
 msgstr ""
 
 #: imio/news/core/vocabularies.py:18
 msgid "Job offer"
 msgstr ""
 
@@ -1288,19 +1282,19 @@
 msgstr ""
 
 #: imio/events/core/contents/event/view.pt:107
 #: imio/news/core/contents/newsitem/view.pt:64
 msgid "Keywords"
 msgstr ""
 
-#: imio/directory/core/contents/contact/content.py:69
+#: imio/directory/core/contents/contact/content.py:97
 msgid "Label (Secretariat, Manager office, Sales,...)"
 msgstr ""
 
-#: imio/directory/core/contents/contact/content.py:48
+#: imio/directory/core/contents/contact/content.py:76
 msgid "Label (direction, Main number,...)"
 msgstr ""
 
 #: imio/smartweb/core/browser/controlpanel.py:16
 msgid "Language (en, fr,...)"
 msgstr ""
 
@@ -1374,30 +1368,30 @@
 msgid "List of events categories values available for this entity (one per line)"
 msgstr ""
 
 #: imio/news/core/contents/entity/content.py:26
 msgid "List of news categories values available for this entity (one per line)"
 msgstr ""
 
-#: imio/directory/core/contents/contact/content.py:268
+#: imio/directory/core/contents/contact/content.py:296
 #: imio/smartweb/core/behaviors/minisite.py:41
 #: imio/smartweb/core/behaviors/subsite.py:33
 msgid "Logo"
 msgstr ""
 
 #: imio/smartweb/core/vocabularies.py:143
 msgid "Logo and title"
 msgstr ""
 
 #: imio/smartweb/core/behaviors/minisite.py:47
 #: imio/smartweb/core/behaviors/subsite.py:39
 msgid "Logo display"
 msgstr ""
 
-#: imio/smartweb/core/contents/sections/contact/view.py:288
+#: imio/smartweb/core/contents/sections/contact/view.py:302
 msgid "Lunch time"
 msgstr ""
 
 #: imio/smartweb/core/contents/sections/macros.pt:46
 msgid "Manage section contents"
 msgstr ""
 
@@ -1464,15 +1458,15 @@
 msgid "Mobility"
 msgstr ""
 
 #: imio/smartweb/core/contents/sections/macros.pt:63
 msgid "Modified"
 msgstr ""
 
-#: imio/smartweb/core/contents/sections/contact/view.py:113
+#: imio/smartweb/core/contents/sections/contact/view.py:127
 msgid "Monday"
 msgstr ""
 
 #: imio/smartweb/core/profiles/default/actions.xml
 msgid "My account"
 msgstr ""
 
@@ -1532,15 +1526,15 @@
 msgid "Not allowed to add Files or Images in imio.directory.Entity"
 msgstr ""
 
 #: imio/smartweb/common/interfaces.py:34
 msgid "Number"
 msgstr ""
 
-#: imio/directory/core/contents/contact/content.py:61
+#: imio/directory/core/contents/contact/content.py:89
 msgid "Number (format: +32475010203)"
 msgstr ""
 
 #: imio/smartweb/core/contents/sections/collection/content.py:41
 #: imio/smartweb/core/contents/sections/events/content.py:63
 #: imio/smartweb/core/contents/sections/files/content.py:15
 msgid "Number of items per batch"
@@ -1572,19 +1566,19 @@
 msgid "Only one procedure field can be filled !"
 msgstr ""
 
 #: imio/smartweb/core/contents/blocks/link/content.py:34
 msgid "Only used in table view (takes precedence over image)"
 msgstr ""
 
-#: imio/smartweb/core/contents/sections/contact/view.py:265
+#: imio/smartweb/core/contents/sections/contact/view.py:279
 msgid "Open"
 msgstr ""
 
-#: imio/smartweb/core/contents/sections/contact/view.py:282
+#: imio/smartweb/core/contents/sections/contact/view.py:296
 msgid "Open at "
 msgstr ""
 
 #: imio/smartweb/core/contents/blocks/link/content.py:23
 #: imio/smartweb/core/contents/sections/slide/content.py:66
 msgid "Open in a new tab"
 msgstr ""
@@ -1637,23 +1631,27 @@
 msgid "Parent listing"
 msgstr ""
 
 #: imio/events/core/vocabularies.py:23
 msgid "Party and folklore"
 msgstr ""
 
+#: imio/smartweb/common/upgrades/configure.zcml:69
+msgid "Patch (Remove select2) eea.facetednavigation jquery"
+msgstr ""
+
 #: imio/directory/core/vocabularies.py:53
 msgid "Personal email"
 msgstr ""
 
 #: imio/directory/core/vocabularies.py:39
 msgid "Personal phone"
 msgstr ""
 
-#: imio/directory/core/contents/contact/content.py:111
+#: imio/directory/core/contents/contact/content.py:139
 msgid "Phones"
 msgstr ""
 
 #: imio/smartweb/core/contents/sections/slide/content.py:41
 msgid "Picture will be displayed as slide background"
 msgstr ""
 
@@ -1711,15 +1709,15 @@
 msgid "Presse"
 msgstr ""
 
 #: imio/smartweb/core/profiles/default/actions.xml
 msgid "Preview"
 msgstr ""
 
-#: imio/directory/core/contents/contact/content.py:144
+#: imio/directory/core/contents/contact/content.py:172
 msgid "Private contact informations"
 msgstr ""
 
 #: imio/smartweb/core/profiles/default/types/imio.smartweb.Procedure.xml
 msgid "Procedure"
 msgstr ""
 
@@ -1809,15 +1807,15 @@
 msgid "Right"
 msgstr ""
 
 #: imio/smartweb/common/vocabularies.py:30
 msgid "Safety and prevention"
 msgstr ""
 
-#: imio/smartweb/core/contents/sections/contact/view.py:118
+#: imio/smartweb/core/contents/sections/contact/view.py:132
 msgid "Saturday"
 msgstr ""
 
 #: imio/smartweb/common/browser/privacy/form.py:27
 msgid "Save my choices"
 msgstr ""
 
@@ -1834,19 +1832,19 @@
 msgid "Secret key"
 msgstr ""
 
 #: imio/smartweb/core/browser/controlpanel.py:34
 msgid "Secret key to use API"
 msgstr ""
 
-#: imio/smartweb/core/contents/sections/views.py:34
+#: imio/smartweb/core/contents/sections/views.py:44
 msgid "Section title has been hidden"
 msgstr ""
 
-#: imio/smartweb/core/contents/sections/views.py:41
+#: imio/smartweb/core/contents/sections/views.py:51
 msgid "Section title has been shown"
 msgstr ""
 
 #: imio/smartweb/core/contents/sections/base.py:58
 msgid "Section width"
 msgstr ""
 
@@ -1874,15 +1872,15 @@
 msgid "Select agenda to display"
 msgstr ""
 
 #: imio/events/core/contents/event/content.py:165
 msgid "Select agendas where this event will be displayed. Current agenda is always selected."
 msgstr ""
 
-#: imio/directory/core/contents/contact/content.py:277
+#: imio/directory/core/contents/contact/content.py:305
 msgid "Select entities where this contact will be displayed. Current entity will always be selected."
 msgstr ""
 
 #: imio/smartweb/core/contents/sections/text/content.py:37
 msgid "Select image size"
 msgstr ""
 
@@ -1914,15 +1912,15 @@
 msgid "Selected agenda"
 msgstr ""
 
 #: imio/events/core/contents/event/content.py:164
 msgid "Selected agendas"
 msgstr ""
 
-#: imio/directory/core/contents/contact/content.py:276
+#: imio/directory/core/contents/contact/content.py:304
 msgid "Selected entities"
 msgstr ""
 
 #: imio/smartweb/core/contents/rest/events/content.py:17
 msgid "Selected event types"
 msgstr ""
 
@@ -2095,28 +2093,28 @@
 msgid "Subsite has been disabled"
 msgstr ""
 
 #: imio/smartweb/core/browser/subsite/settings.py:25
 msgid "Subsite has been successfully activated"
 msgstr ""
 
-#: imio/directory/core/contents/contact/content.py:208
+#: imio/directory/core/contents/contact/content.py:236
 #: imio/smartweb/core/contents/sections/postit/content.py:26
 msgid "Subtitle"
 msgstr ""
 
 #: imio/smartweb/core/contents/folder/configure.zcml:72
 msgid "Summary view"
 msgstr ""
 
 #: imio/smartweb/core/contents/folder/configure.zcml:83
 msgid "Summary view with images"
 msgstr ""
 
-#: imio/smartweb/core/contents/sections/contact/view.py:119
+#: imio/smartweb/core/contents/sections/contact/view.py:133
 msgid "Sunday"
 msgstr ""
 
 #: imio/smartweb/core/contents/sections/contact/content.py:47
 msgid "Switch lead image to portrait mode"
 msgstr ""
 
@@ -2195,15 +2193,15 @@
 msgid "Third page"
 msgstr ""
 
 #: imio/smartweb/common/privacy.py:70
 msgid "This feature requires cookies acceptation.<br/><a class=\"pat-plone-modal\" href=\"${consent_url}\">Review your cookies preferences</a>."
 msgstr ""
 
-#: imio/directory/core/contents/contact/content.py:203
+#: imio/directory/core/contents/contact/content.py:231
 #: imio/events/core/contents/event/content.py:48
 #: imio/news/core/contents/newsitem/content.py:34
 msgid "This field is required if the content must be available in this language"
 msgstr ""
 
 #: imio/smartweb/core/browser/controlpanel.py:91
 msgid "This information is used for search results redirection"
@@ -2213,28 +2211,28 @@
 msgid "This site uses cookies to provide you with an optimal experience (playing videos, displaying maps and content from social networks in particular)."
 msgstr ""
 
 #: imio/smartweb/core/vocabularies.py:128
 msgid "Three quarter of width"
 msgstr ""
 
-#: imio/smartweb/core/contents/sections/contact/view.py:116
+#: imio/smartweb/core/contents/sections/contact/view.py:130
 msgid "Thursday"
 msgstr ""
 
 #: imio/events/core/contents/event/content.py:114
 #: imio/events/core/contents/event/view.pt:67
 msgid "Ticket url"
 msgstr ""
 
 #: imio/events/core/contents/event/content.py:115
 msgid "Ticket url to subscribe to this event"
 msgstr ""
 
-#: imio/directory/core/contents/contact/content.py:202
+#: imio/directory/core/contents/contact/content.py:230
 #: imio/events/core/contents/event/content.py:47
 #: imio/news/core/contents/newsitem/content.py:33
 msgid "Title"
 msgstr ""
 
 #: imio/smartweb/core/vocabularies.py:157
 msgid "Title and Subtitle"
@@ -2262,15 +2260,15 @@
 msgid "Tourist"
 msgstr ""
 
 #: imio/events/core/vocabularies.py:25
 msgid "Trade Fair and Fair"
 msgstr ""
 
-#: imio/smartweb/core/contents/sections/contact/view.py:114
+#: imio/smartweb/core/contents/sections/contact/view.py:128
 msgid "Tuesday"
 msgstr ""
 
 #: imio/directory/core/vocabularies.py:69
 #: imio/events/core/contents/event/content.py:132
 #: imio/events/core/contents/event/view.pt:77
 msgid "Twitter"
@@ -2284,35 +2282,35 @@
 msgid "Twitter url for this news"
 msgstr ""
 
 #: imio/smartweb/core/vocabularies.py:127
 msgid "Two third of width"
 msgstr ""
 
-#: imio/directory/core/contents/contact/content.py:54
+#: imio/directory/core/contents/contact/content.py:82
 msgid "Type"
 msgstr ""
 
 #: imio/smartweb/core/contents/blocks/link/content.py:26
 msgid "URL"
 msgstr ""
 
-#: imio/directory/core/contents/contact/content.py:131
+#: imio/directory/core/contents/contact/content.py:159
 msgid "URLs"
 msgstr ""
 
-#: imio/directory/policy/configure.zcml:43
+#: imio/directory/policy/configure.zcml:44
 msgid "Uninstalls the imio.directory.policy add-on."
 msgstr ""
 
-#: imio/events/policy/configure.zcml:44
+#: imio/events/policy/configure.zcml:45
 msgid "Uninstalls the imio.events.policy add-on."
 msgstr ""
 
-#: imio/news/policy/configure.zcml:44
+#: imio/news/policy/configure.zcml:45
 msgid "Uninstalls the imio.news.policy add-on."
 msgstr ""
 
 #: imio/smartweb/policy/upgrades/configure.zcml:76
 msgid "Update caching configuration"
 msgstr ""
 
@@ -2344,14 +2342,18 @@
 msgid "Upgrade common from 1013 to 1014"
 msgstr ""
 
 #: imio/smartweb/common/upgrades/configure.zcml:61
 msgid "Upgrade common from 1014 to 1015"
 msgstr ""
 
+#: imio/smartweb/common/upgrades/configure.zcml:69
+msgid "Upgrade common from 1015 to 1016"
+msgstr ""
+
 #: imio/smartweb/core/upgrades/configure.zcml:92
 msgid "Upgrade common from 1031 to 1032"
 msgstr ""
 
 #: imio/smartweb/core/upgrades/configure.zcml:100
 msgid "Upgrade common from 1033 to 1034"
 msgstr ""
@@ -2502,15 +2504,15 @@
 msgid "Upgrade policy from 1026 to 1027"
 msgstr ""
 
 #: imio/smartweb/policy/upgrades/configure.zcml:124
 msgid "Upgrade policy from 1028 to 1029"
 msgstr ""
 
-#: imio/directory/core/contents/contact/content.py:92
+#: imio/directory/core/contents/contact/content.py:120
 msgid "Url"
 msgstr ""
 
 #: imio/smartweb/core/browser/controlpanel.py:25
 msgid "Url to get forms from your e-guichet"
 msgstr ""
 
@@ -2536,15 +2538,15 @@
 msgid "Use custom spotlight to avoid bad gallery refresh"
 msgstr ""
 
 #: imio/directory/core/vocabularies.py:86
 msgid "Useful numbers"
 msgstr ""
 
-#: imio/directory/core/contents/contact/content.py:109
+#: imio/directory/core/contents/contact/content.py:137
 msgid "VAT number"
 msgstr ""
 
 #: imio/smartweb/core/profiles/default/types/imio.smartweb.SectionVideo.xml
 msgid "Video section"
 msgstr ""
 
@@ -2580,20 +2582,24 @@
 msgid "Visible blocks"
 msgstr ""
 
 #: imio/smartweb/core/browser/controlpanel.py:116
 msgid "Vocabulary term"
 msgstr ""
 
+#: imio/smartweb/core/browser/overrides/plone.app.content.browser.contents.templates.properties.pt:3
+msgid "Warning: these options are not relevant for Sections and will not be applied."
+msgstr ""
+
 #: imio/directory/core/vocabularies.py:70
 #: imio/news/core/contents/newsitem/content.py:85
 msgid "Website"
 msgstr ""
 
-#: imio/smartweb/core/contents/sections/contact/view.py:115
+#: imio/smartweb/core/contents/sections/contact/view.py:129
 msgid "Wednesday"
 msgstr ""
 
 #: imio/directory/core/vocabularies.py:54
 msgid "Work email"
 msgstr ""
 
@@ -2643,35 +2649,35 @@
 msgid "Zipcode '${val}' is not a number."
 msgstr ""
 
 #: imio/smartweb/common/viewlets/colophon.pt:34
 msgid "free license"
 msgstr ""
 
-#: imio/directory/policy/configure.zcml:34
+#: imio/directory/policy/configure.zcml:35
 msgid "imio.directory.policy"
 msgstr ""
 
-#: imio/directory/policy/configure.zcml:43
+#: imio/directory/policy/configure.zcml:44
 msgid "imio.directory.policy (uninstall)"
 msgstr ""
 
-#: imio/events/policy/configure.zcml:35
+#: imio/events/policy/configure.zcml:36
 msgid "imio.events.policy"
 msgstr ""
 
-#: imio/events/policy/configure.zcml:44
+#: imio/events/policy/configure.zcml:45
 msgid "imio.events.policy (uninstall)"
 msgstr ""
 
-#: imio/news/policy/configure.zcml:35
+#: imio/news/policy/configure.zcml:36
 msgid "imio.news.policy"
 msgstr ""
 
-#: imio/news/policy/configure.zcml:44
+#: imio/news/policy/configure.zcml:45
 msgid "imio.news.policy (uninstall)"
 msgstr ""
 
 #. Default: "You are editing the default page of a container. If you wanted to edit the container itself, ${go_here}."
 #: imio/smartweb/core/viewlets/default_page_warning.pt:7
 msgid "label_edit_default_page_container"
 msgstr ""
```

### Comparing `imio.smartweb.locales-1.1.3/src/imio/smartweb/locales/locales/plone-manual.pot` & `imio.smartweb.locales-1.1.4/src/imio/smartweb/locales/locales/plone-manual.pot`

 * *Files identical despite different names*

### Comparing `imio.smartweb.locales-1.1.3/src/imio/smartweb/locales/locales/de/LC_MESSAGES/imio.smartweb.po` & `imio.smartweb.locales-1.1.4/src/imio/smartweb/locales/locales/fr/LC_MESSAGES/imio.smartweb.po`

 * *Files 1% similar despite different names*

```diff
@@ -4,21 +4,21 @@
 "POT-Creation-Date: YEAR-MO-DA HO:MI +ZONE\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI +ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=1; plural=0;\n"
-"Language-Code: de\n"
-"Language-Name: Deutsch\n"
+"Plural-Forms: nplurals=2; plural=(n > 1);\n"
+"Language-Code: fr\n"
+"Language-Name: French\n"
 "Preferred-Encodings: utf-8 latin1\n"
 "Domain: imio.smartweb\n"
-"Language: de\n"
-"X-Is-Fallback-For: de-at de-li de-lu de-ch de-de\n"
+"Language: fr\n"
+"X-Is-Fallback-For: fr-be fr-ca fr-lu fr-mc fr-ch fr-fr\n"
 
 #: imio/smartweb/core/contents/sections/base.py:85
 msgid "<div class=\"section_error_txt\">Error in section : \"{}\" <a href=\"{}/edit\">[edit]</a></div>"
 msgstr "<div class=\"section_error_txt\">Erreur dans la section : \"{}\" <a href=\"{}/edit\">[modifier]</a></div>"
 
 #: imio/smartweb/common/browser/privacy/form.py:31
 #: imio/smartweb/common/viewlets/privacy.pt:15
@@ -195,21 +195,21 @@
 msgid "Allow to select quick access elements for current context."
 msgstr "Permet de sélectionner des éléments Accès Direct pour l'élément courant."
 
 #: imio/smartweb/core/contents/sections/slide/content.py:53
 msgid "Alternatively as a picture"
 msgstr "Comme alternative à une image"
 
-#: imio/smartweb/core/contents/folder/views.py:132
+#: imio/smartweb/core/contents/folder/views.py:134
 msgid "Apply"
 msgstr "Appliquer"
 
 #: imio/smartweb/core/viewlets/toolbar.py:19
 msgid "Authentic sources"
-msgstr ""
+msgstr "Sources authentiques"
 
 #: imio/smartweb/policy/upgrades/configure.zcml:68
 msgid "Automatically publish GDPR article"
 msgstr ""
 
 #: imio/smartweb/core/browser/instancebehaviors/form.py:22
 msgid "Available taxonomies"
@@ -228,15 +228,15 @@
 msgid "Bad URL format '${val}' (good format sample: https://www.imio.be)."
 msgstr "Mauvais format d'URL pour '${val}' (format correct: https://www.imio.be)."
 
 #: imio/directory/core/browser/import.py:90
 msgid "Bad mail format '${val}' (good format sample: noreply@imio.be)."
 msgstr "Mauvais format d'email pour '${val}' (format correct: noreply@imio.be)."
 
-#: imio/directory/core/contents/contact/content.py:42
+#: imio/directory/core/contents/contact/content.py:44
 msgid "Bad phone format"
 msgstr "Mauvais format de téléphone"
 
 #: imio/directory/core/browser/import.py:72
 msgid "Bad phone format '${val}' (good format sample: +32444556677)."
 msgstr "Mauvais format de numéro de téléphone pour '${val}' (format correct: +32444556677)."
 
@@ -286,15 +286,15 @@
 msgid "CSV file"
 msgstr "Fichier CSV"
 
 #: imio/smartweb/common/sharing/localroles.py:12
 msgid "Can manage locally"
 msgstr "Peut administrer"
 
-#: imio/smartweb/core/vocabularies.py:570
+#: imio/smartweb/core/vocabularies.py:571
 msgid "Carousel"
 msgstr "Carrousel"
 
 #: imio/smartweb/core/contents/sections/links/configure.zcml:26
 #: imio/smartweb/core/contents/sections/selections/configure.zcml:26
 msgid "Carousel view"
 msgstr "Affichage carrousel"
@@ -487,19 +487,19 @@
 #: imio/directory/core/browser/import.py:227
 msgid "Chosen topic '${val}' doesn't exist."
 msgstr "La thématique choisie '${val}' n'existe pas."
 
 #: imio/smartweb/core/profiles/default/types/imio.smartweb.CirkwiView.xml
 #: imio/smartweb/core/upgrades/profiles/1035_to_1036/types/imio.smartweb.CirkwiView.xml
 msgid "Cirkwi view"
-msgstr ""
+msgstr "Vue Cirkwi"
 
 #: imio/smartweb/core/contents/pages/cirkwi/content.py:14
 msgid "Cirkwi widget ID"
-msgstr ""
+msgstr "Identifiant de votre widget \"Cirkwi\""
 
 #: imio/smartweb/common/profiles/default/registry.xml
 msgid "Cities"
 msgstr ""
 
 #: imio/smartweb/common/vocabularies.py:27
 msgid "Citizen participation"
@@ -553,15 +553,15 @@
 msgid "Click to preview content (without editor actions)."
 msgstr "Prévisualiser le contenu (sans les boutons d'édition)."
 
 #: imio/smartweb/core/viewlets/navigation.py:85
 msgid "Close"
 msgstr "Fermer"
 
-#: imio/smartweb/core/contents/sections/contact/view.py:258
+#: imio/smartweb/core/contents/sections/contact/view.py:272
 msgid "Closed"
 msgstr "Fermé"
 
 #: imio/smartweb/core/profiles/default/types/imio.smartweb.SectionCollection.xml
 msgid "Collection section"
 msgstr "Section collection"
 
@@ -600,15 +600,15 @@
 msgid "Contact"
 msgstr "Contact"
 
 #: imio/directory/core/profiles/default/types/imio.directory.Contact.xml
 msgid "Contact content type"
 msgstr "Contact"
 
-#: imio/directory/core/contents/contact/content.py:106
+#: imio/directory/core/contents/contact/content.py:134
 #: imio/smartweb/core/vocabularies.py:158
 msgid "Contact informations"
 msgstr "Coordonnées"
 
 #: imio/smartweb/core/profiles/default/types/imio.smartweb.SectionContact.xml
 msgid "Contact section"
 msgstr "Section contact"
@@ -673,15 +673,15 @@
 msgid "Define number of levels in menu navigation subsite"
 msgstr "Définir un nombre de niveaux pour le menu de navigation du sous-site"
 
 #: imio/smartweb/core/contents/sections/macros.pt:57
 msgid "Delete section"
 msgstr "Supprimer la section"
 
-#: imio/directory/core/contents/contact/content.py:209
+#: imio/directory/core/contents/contact/content.py:237
 #: imio/events/core/contents/event/content.py:53
 #: imio/news/core/contents/newsitem/content.py:39
 msgid "Description"
 msgstr "Description"
 
 #: imio/smartweb/core/browser/controlpanel.py:72
 msgid "Directory SolR Core ID"
@@ -710,15 +710,15 @@
 #: imio/smartweb/core/viewlets/banner.pt:11
 msgid "Display banner from this item"
 msgstr "Afficher la bannière"
 
 #: imio/smartweb/core/profiles/default/types/imio.smartweb.CirkwiView.xml
 #: imio/smartweb/core/upgrades/profiles/1035_to_1036/types/imio.smartweb.CirkwiView.xml
 msgid "Display cirkwi informations and map."
-msgstr ""
+msgstr "Affiche les informations et la carte Cirkwi"
 
 #: imio/smartweb/core/profiles/default/types/imio.smartweb.DirectoryView.xml
 msgid "Display linked directory from imio directory instance."
 msgstr "Affiche des contacts depuis la source authentique"
 
 #: imio/smartweb/core/profiles/default/types/imio.smartweb.EventsView.xml
 msgid "Display linked events from imio events instance."
@@ -728,29 +728,29 @@
 msgid "Display linked news from imio news instance."
 msgstr "Affiche des actualités depuis la source authentique"
 
 #: imio/directory/core/vocabularies.py:85
 msgid "Drinking water point"
 msgstr "Points d'eau potable"
 
-#: imio/directory/core/contents/contact/content.py:232
+#: imio/directory/core/contents/contact/content.py:260
 #: imio/events/core/contents/event/content.py:77
 #: imio/news/core/contents/newsitem/content.py:63
 msgid "Dutch translations"
 msgstr "Traductions néerlandophones"
 
 #: imio/smartweb/core/contents/pages/procedure/content.py:21
 msgid "E-Guichet procedure"
 msgstr "Lien vers la démarche dans l'e-guichet iMio"
 
-#: imio/directory/core/contents/contact/content.py:81
+#: imio/directory/core/contents/contact/content.py:109
 msgid "E-mail"
 msgstr "Adresse e-mail"
 
-#: imio/directory/core/contents/contact/content.py:121
+#: imio/directory/core/contents/contact/content.py:149
 msgid "E-mails"
 msgstr ""
 
 #: imio/smartweb/common/vocabularies.py:22
 msgid "Economics"
 msgstr "Économie"
 
@@ -782,15 +782,15 @@
 msgid "Enable minisite"
 msgstr "Activer le mode site partenaire"
 
 #: imio/smartweb/core/profiles/default/actions.xml
 msgid "Enable subsite"
 msgstr "Activer le mode sous-site"
 
-#: imio/directory/core/contents/contact/content.py:215
+#: imio/directory/core/contents/contact/content.py:243
 #: imio/events/core/contents/event/content.py:60
 #: imio/news/core/contents/newsitem/content.py:46
 msgid "English translations"
 msgstr "Traductions anglophones"
 
 #: imio/smartweb/core/browser/controlpanel.py:17
 msgid "Enter the language code. Ex.: en"
@@ -876,15 +876,15 @@
 msgid "Example : Photo of a person or organization building"
 msgstr "Exemple : Photo d'une personne ou d'un bâtiment d'une organisation"
 
 #: imio/smartweb/core/browser/controlpanel.py:26
 msgid "Example : https://COMMUNE-formulaires.guichet-citoyen.be/api/formdefs/"
 msgstr "Exemple : https://COMMUNE-formulaires.guichet-citoyen.be/api/formdefs/"
 
-#: imio/directory/core/contents/contact/content.py:269
+#: imio/directory/core/contents/contact/content.py:297
 msgid "Example : shop, service, association logo"
 msgstr "Exemple : Logo d'un magasin ou d'un service ou d'une association"
 
 #: imio/smartweb/core/behaviors/listing.py:19
 msgid "Exclude from parent listing"
 msgstr "Exclure dans l'affichage listing du parent"
 
@@ -934,15 +934,15 @@
 msgid "Faceted summary view"
 msgstr "Affichage liste"
 
 #: imio/smartweb/core/browser/faceted/configure.zcml:88
 msgid "Faceted summary view with images"
 msgstr "Affichage liste avec images"
 
-#: imio/directory/core/contents/contact/content.py:286
+#: imio/directory/core/contents/contact/content.py:314
 msgid "Facilities"
 msgstr "Facilités"
 
 #: imio/events/core/contents/event/content.py:151
 #: imio/events/core/contents/event/view.pt:57
 msgid "Facilities for person with reduced mobility"
 msgstr "Accessible aux personnes à mobilité réduite"
@@ -1015,28 +1015,28 @@
 msgid "Footer has been successfully added"
 msgstr "Le pied de page a été ajouté avec succès"
 
 #: imio/smartweb/core/contents/folder/content.py:26
 msgid "For the anonymous visitor, the folder and the selected item are one. When he clicks on the folder, the item is displayed."
 msgstr "Pour le visiteur anonyme, le dossier et l'élément sélectionné ne font qu'un. Lorsqu'il clique sur le dossier, l'élément s'affiche."
 
-#: imio/smartweb/core/contents/folder/views.py:103
+#: imio/smartweb/core/contents/folder/views.py:105
 msgid "Form to choose item to be displayed as the home page of the folder"
 msgstr "Formulaire de choix de l'élément à afficher comme page d'accueil du dossier"
 
 #: imio/directory/core/vocabularies.py:88
 msgid "Free WIFI"
 msgstr "Wifi gratuit"
 
 #: imio/events/core/contents/event/content.py:144
 #: imio/events/core/contents/event/view.pt:47
 msgid "Free entry"
 msgstr "Gratuit"
 
-#: imio/smartweb/core/contents/sections/contact/view.py:117
+#: imio/smartweb/core/contents/sections/contact/view.py:131
 msgid "Friday"
 msgstr "Vendredi"
 
 #: imio/smartweb/core/contents/sections/events/macros.pt:13
 msgid "From"
 msgstr "Du"
 
@@ -1056,27 +1056,27 @@
 msgid "Gallery section"
 msgstr "Section galerie"
 
 #: imio/smartweb/core/profiles/default/types/imio.smartweb.SectionGallery.xml
 msgid "Gallery section for a page"
 msgstr "Création d'une section galerie qui affichera ses images dans votre page. "
 
-#: imio/directory/core/contents/contact/content.py:198
+#: imio/directory/core/contents/contact/content.py:226
 #: imio/events/core/contents/event/content.py:43
 #: imio/news/core/contents/newsitem/content.py:29
 msgid "German translations"
 msgstr "Traductions germanophones"
 
 #: imio/smartweb/core/contents/sections/events/content.py:37
 msgid "Get priory on related agenda for these specifics events."
 msgstr "Ces événéments prennent la priorité sur le champ d'agenda lié."
 
 #: imio/smartweb/core/contents/sections/news/content.py:37
 msgid "Get priory on related news for these specifics news."
-msgstr ""
+msgstr "Ces actualités prennent la priorité sur le champ des actualités liées."
 
 #: imio/smartweb/core/viewlets/minisite_link.pt:8
 msgid "Go to ${url}"
 msgstr "Aller sur ${url}"
 
 #: imio/smartweb/core/contents/sections/html/content.py:17
 msgid "HTML"
@@ -1210,15 +1210,15 @@
 msgstr "Important! Ces catégories sont utilisées pour créer des listes accessibles via le menu navigation"
 
 #: imio/events/core/contents/event/content.py:175
 #: imio/news/core/contents/newsitem/content.py:130
 msgid "Important! These categories are used to supplement the information provided by the topics"
 msgstr "Important! Ces catégories permettent de compléter l'information apportée par les thématiques"
 
-#: imio/directory/core/contents/contact/content.py:287
+#: imio/directory/core/contents/contact/content.py:315
 msgid "Important! These categories make it possible to highlight and geolocate certain basic services"
 msgstr "Important! Ces catégories permettent de mettre en avant et de géolocaliser certains services de base"
 
 #: imio/smartweb/common/behaviors/topics.py:17
 msgid "Important! Topics are used to filter search results and create lists"
 msgstr "Important! Les thématiques sont utilisées pour filtrer les résultats de la recherche et créer des listes"
 
@@ -1236,41 +1236,41 @@
 msgid "Instagram url for this event"
 msgstr "Lien Instagram pour cet événement"
 
 #: imio/news/core/contents/newsitem/content.py:110
 msgid "Instagram url for this news"
 msgstr "Lien Instagram de cette actualité"
 
-#: imio/directory/policy/configure.zcml:34
+#: imio/directory/policy/configure.zcml:35
 msgid "Installs the imio.directory.policy add-on."
 msgstr ""
 
-#: imio/events/policy/configure.zcml:35
+#: imio/events/policy/configure.zcml:36
 msgid "Installs the imio.events.policy add-on."
 msgstr ""
 
-#: imio/news/policy/configure.zcml:35
+#: imio/news/policy/configure.zcml:36
 msgid "Installs the imio.news.policy add-on."
 msgstr ""
 
-#: imio/directory/core/contents/contact/content.py:179
+#: imio/directory/core/contents/contact/content.py:207
 msgid "Internal note"
 msgstr "Note interne"
 
 #: imio/events/core/vocabularies.py:26
 msgid "Internships and courses"
 msgstr "Stages et cours"
 
 #: imio/smartweb/core/contents/folder/content.py:25
 msgid "Item(s) that can be selected as the folder default page."
 msgstr "Elément(s) pouvant être sélectionné(s) comme page d'accueil du dossier."
 
-#: imio/events/core/contents/event/views.py:75
+#: imio/events/core/contents/event/views.py:77
 #: imio/smartweb/core/contents/sections/contact/view.pt:122
-#: imio/smartweb/core/contents/sections/contact/view.py:62
+#: imio/smartweb/core/contents/sections/contact/view.py:77
 msgid "Itinerary"
 msgstr "Itinéraire"
 
 #: imio/news/core/vocabularies.py:18
 msgid "Job offer"
 msgstr "Emploi"
 
@@ -1283,19 +1283,19 @@
 msgstr "Journaliste"
 
 #: imio/events/core/contents/event/view.pt:107
 #: imio/news/core/contents/newsitem/view.pt:64
 msgid "Keywords"
 msgstr "Mots-clés"
 
-#: imio/directory/core/contents/contact/content.py:69
+#: imio/directory/core/contents/contact/content.py:97
 msgid "Label (Secretariat, Manager office, Sales,...)"
 msgstr "Intitulé (Secrétariat, Bureau de la direction, Ventes, ...)"
 
-#: imio/directory/core/contents/contact/content.py:48
+#: imio/directory/core/contents/contact/content.py:76
 msgid "Label (direction, Main number,...)"
 msgstr "Intitulé (direction, numéro principal, ...)"
 
 #: imio/smartweb/core/browser/controlpanel.py:16
 msgid "Language (en, fr,...)"
 msgstr "Langue (en, fr, ...)"
 
@@ -1369,30 +1369,30 @@
 msgid "List of events categories values available for this entity (one per line)"
 msgstr "Liste de catégories spécifiques d'événements disponibes pour cette entité (un par ligne)"
 
 #: imio/news/core/contents/entity/content.py:26
 msgid "List of news categories values available for this entity (one per line)"
 msgstr "Liste de catégories spécifiques d'actualités disponibes pour cette entité (une par ligne)"
 
-#: imio/directory/core/contents/contact/content.py:268
+#: imio/directory/core/contents/contact/content.py:296
 #: imio/smartweb/core/behaviors/minisite.py:41
 #: imio/smartweb/core/behaviors/subsite.py:33
 msgid "Logo"
 msgstr "Logo"
 
 #: imio/smartweb/core/vocabularies.py:143
 msgid "Logo and title"
 msgstr "Logo et titre"
 
 #: imio/smartweb/core/behaviors/minisite.py:47
 #: imio/smartweb/core/behaviors/subsite.py:39
 msgid "Logo display"
 msgstr "Type d'affichage du logo"
 
-#: imio/smartweb/core/contents/sections/contact/view.py:288
+#: imio/smartweb/core/contents/sections/contact/view.py:302
 msgid "Lunch time"
 msgstr "Heure du midi"
 
 #: imio/smartweb/core/contents/sections/macros.pt:46
 msgid "Manage section contents"
 msgstr "Modifier contenu"
 
@@ -1459,15 +1459,15 @@
 msgid "Mobility"
 msgstr "Mobilité"
 
 #: imio/smartweb/core/contents/sections/macros.pt:63
 msgid "Modified"
 msgstr "Modifié"
 
-#: imio/smartweb/core/contents/sections/contact/view.py:113
+#: imio/smartweb/core/contents/sections/contact/view.py:127
 msgid "Monday"
 msgstr "Lundi"
 
 #: imio/smartweb/core/profiles/default/actions.xml
 msgid "My account"
 msgstr "Mon compte"
 
@@ -1527,15 +1527,15 @@
 msgid "Not allowed to add Files or Images in imio.directory.Entity"
 msgstr ""
 
 #: imio/smartweb/common/interfaces.py:34
 msgid "Number"
 msgstr "Numéro"
 
-#: imio/directory/core/contents/contact/content.py:61
+#: imio/directory/core/contents/contact/content.py:89
 msgid "Number (format: +32475010203)"
 msgstr "Numéro (format: +32475010203)"
 
 #: imio/smartweb/core/contents/sections/collection/content.py:41
 #: imio/smartweb/core/contents/sections/events/content.py:63
 #: imio/smartweb/core/contents/sections/files/content.py:15
 msgid "Number of items per batch"
@@ -1567,19 +1567,19 @@
 msgid "Only one procedure field can be filled !"
 msgstr "Un seul champ \"démarche\" peut être rempli !"
 
 #: imio/smartweb/core/contents/blocks/link/content.py:34
 msgid "Only used in table view (takes precedence over image)"
 msgstr "Utilisée uniquement dans l'affichage tableau (prend la priorité sur l'image)"
 
-#: imio/smartweb/core/contents/sections/contact/view.py:265
+#: imio/smartweb/core/contents/sections/contact/view.py:279
 msgid "Open"
 msgstr "Ouvert"
 
-#: imio/smartweb/core/contents/sections/contact/view.py:282
+#: imio/smartweb/core/contents/sections/contact/view.py:296
 msgid "Open at "
 msgstr "Ouvre à "
 
 #: imio/smartweb/core/contents/blocks/link/content.py:23
 #: imio/smartweb/core/contents/sections/slide/content.py:66
 msgid "Open in a new tab"
 msgstr "Ouvrir dans un nouvel onglet"
@@ -1632,23 +1632,27 @@
 msgid "Parent listing"
 msgstr "Listing du parent"
 
 #: imio/events/core/vocabularies.py:23
 msgid "Party and folklore"
 msgstr "Fête et folklore"
 
+#: imio/smartweb/common/upgrades/configure.zcml:69
+msgid "Patch (Remove select2) eea.facetednavigation jquery"
+msgstr ""
+
 #: imio/directory/core/vocabularies.py:53
 msgid "Personal email"
 msgstr "Adresse e-mail personnelle"
 
 #: imio/directory/core/vocabularies.py:39
 msgid "Personal phone"
 msgstr "Numéro de téléphone personnel"
 
-#: imio/directory/core/contents/contact/content.py:111
+#: imio/directory/core/contents/contact/content.py:139
 msgid "Phones"
 msgstr "Téléphones"
 
 #: imio/smartweb/core/contents/sections/slide/content.py:41
 msgid "Picture will be displayed as slide background"
 msgstr "L'image est affichée en background du slide"
 
@@ -1706,15 +1710,15 @@
 msgid "Presse"
 msgstr "Presse"
 
 #: imio/smartweb/core/profiles/default/actions.xml
 msgid "Preview"
 msgstr "Prévisualiser"
 
-#: imio/directory/core/contents/contact/content.py:144
+#: imio/directory/core/contents/contact/content.py:172
 msgid "Private contact informations"
 msgstr "Coordonnées privées"
 
 #: imio/smartweb/core/profiles/default/types/imio.smartweb.Procedure.xml
 msgid "Procedure"
 msgstr "Démarche"
 
@@ -1804,15 +1808,15 @@
 msgid "Right"
 msgstr "Droite"
 
 #: imio/smartweb/common/vocabularies.py:30
 msgid "Safety and prevention"
 msgstr "Sécurité et prévention"
 
-#: imio/smartweb/core/contents/sections/contact/view.py:118
+#: imio/smartweb/core/contents/sections/contact/view.py:132
 msgid "Saturday"
 msgstr "Samedi"
 
 #: imio/smartweb/common/browser/privacy/form.py:27
 msgid "Save my choices"
 msgstr "Enregistrer mes choix"
 
@@ -1829,19 +1833,19 @@
 msgid "Secret key"
 msgstr "Clé secrète"
 
 #: imio/smartweb/core/browser/controlpanel.py:34
 msgid "Secret key to use API"
 msgstr "Clé secrète pour utiliser l'API"
 
-#: imio/smartweb/core/contents/sections/views.py:34
+#: imio/smartweb/core/contents/sections/views.py:44
 msgid "Section title has been hidden"
 msgstr "Le titre de la section a été caché (pour le visiteur)"
 
-#: imio/smartweb/core/contents/sections/views.py:41
+#: imio/smartweb/core/contents/sections/views.py:51
 msgid "Section title has been shown"
 msgstr "Le titre de la section a été affiché"
 
 #: imio/smartweb/core/contents/sections/base.py:58
 msgid "Section width"
 msgstr "Largeur de la section"
 
@@ -1869,15 +1873,15 @@
 msgid "Select agenda to display"
 msgstr "Sélectionnez l'agenda à afficher"
 
 #: imio/events/core/contents/event/content.py:165
 msgid "Select agendas where this event will be displayed. Current agenda is always selected."
 msgstr "Sélectionnez les agendas dans lesquels cet événement sera affiché. L'agenda courant sera toujours sélectionné."
 
-#: imio/directory/core/contents/contact/content.py:277
+#: imio/directory/core/contents/contact/content.py:305
 msgid "Select entities where this contact will be displayed. Current entity will always be selected."
 msgstr "Sélectionnez les entités dans lesquelles ce contact sera affiché. L'entité courante sera toujours sélectionnée."
 
 #: imio/smartweb/core/contents/sections/text/content.py:37
 msgid "Select image size"
 msgstr "Sélectionnez la taille de l'image"
 
@@ -1909,15 +1913,15 @@
 msgid "Selected agenda"
 msgstr "Agenda sélectionné"
 
 #: imio/events/core/contents/event/content.py:164
 msgid "Selected agendas"
 msgstr "Agendas concernés"
 
-#: imio/directory/core/contents/contact/content.py:276
+#: imio/directory/core/contents/contact/content.py:304
 msgid "Selected entities"
 msgstr "Entités concernées"
 
 #: imio/smartweb/core/contents/rest/events/content.py:17
 msgid "Selected event types"
 msgstr "Types d'événements sélectionnés"
 
@@ -2044,19 +2048,19 @@
 
 #: imio/smartweb/core/contents/sections/events/content.py:36
 msgid "Specific related events"
 msgstr "Evénements spécifiquement sélectionnés"
 
 #: imio/smartweb/core/contents/sections/news/content.py:36
 msgid "Specific related news"
-msgstr ""
+msgstr "Actualités spécifiquement sélectionnées"
 
 #: imio/smartweb/core/contents/pages/cirkwi/content.py:15
 msgid "Specify your cirkwi widget ID. You can find it when you create a new widget in Cirkwi."
-msgstr ""
+msgstr "Précisez votre identifiant de widget Cirkwi. Vous pouvez le trouver lorsque vous créez un nouveau widget dans Cirkwi."
 
 #: imio/smartweb/common/vocabularies.py:32
 msgid "Sports"
 msgstr "Sports"
 
 #: imio/smartweb/core/profiles/default/types/imio.smartweb.Page.xml
 msgid "Standard Page content type to print informations"
@@ -2090,28 +2094,28 @@
 msgid "Subsite has been disabled"
 msgstr "Le mode sous-site a été désactivé"
 
 #: imio/smartweb/core/browser/subsite/settings.py:25
 msgid "Subsite has been successfully activated"
 msgstr "Le mode sous-site a été activé avec succès"
 
-#: imio/directory/core/contents/contact/content.py:208
+#: imio/directory/core/contents/contact/content.py:236
 #: imio/smartweb/core/contents/sections/postit/content.py:26
 msgid "Subtitle"
 msgstr "Sous-titre"
 
 #: imio/smartweb/core/contents/folder/configure.zcml:72
 msgid "Summary view"
 msgstr "Affichage liste"
 
 #: imio/smartweb/core/contents/folder/configure.zcml:83
 msgid "Summary view with images"
 msgstr "Affichage liste avec images"
 
-#: imio/smartweb/core/contents/sections/contact/view.py:119
+#: imio/smartweb/core/contents/sections/contact/view.py:133
 msgid "Sunday"
 msgstr "Dimanche"
 
 #: imio/smartweb/core/contents/sections/contact/content.py:47
 msgid "Switch lead image to portrait mode"
 msgstr "Passer l'image de garde en mode portrait"
 
@@ -2156,15 +2160,15 @@
 
 #: imio/directory/core/contents/contact/forms.py:18
 msgid "The geolocation is generated on the basis of the address during contact save. It is possible to change the pointer manually if it is not correctly positioned."
 msgstr "La géolocalisation est générée sur base de l'adresse lors de l'enregistrement de la fiche. Il est possible de modifier le pointeur manuellement si ce dernier n'est pas bien positionné."
 
 #: imio/smartweb/common/utils.py:133
 msgid "The image uploaded in the \"${field_title}\" field may be degraded because it does not meet the required minimum dimensions of ${min_width}px width by ${min_height}px height (uploaded image size: ${width}px width by ${height}px height). You can see the detail via the Cropping menu."
-msgstr ""
+msgstr "L'image téléversée dans le champ \"${field_title}\" risque d'être dégradée, car elle ne correspond pas aux dimensions minimales requises de ${min_width}px de largeur sur ${min_height}px de hauteur (taille de l'image téléversée : ${width}px de largeur / ${height}px de hauteur). Vous pouvez voir le détail via le menu Découpe."
 
 #: imio/smartweb/core/contents/folder/element_view.pt:6
 msgid "The item selected as the folder home page is :"
 msgstr "L'élément sélectionné comme page d'accueil du dossier est :"
 
 #: imio/smartweb/core/contents/sections/base.py:44
 msgid "The title will always be displayed if this behavior is enabled."
@@ -2176,29 +2180,29 @@
 
 #: imio/smartweb/core/contents/pages/views.py:64
 msgid "There is no section on this page."
 msgstr "Il n'y a aucune section dans cette page."
 
 #: imio/smartweb/core/contents/pages/procedure/view.py:13
 msgid "There is no section on this procedure."
-msgstr ""
+msgstr "Il n'y a aucune section présente dans cette démarche."
 
 #: imio/smartweb/core/vocabularies.py:125
 msgid "Third of width"
 msgstr "Tiers de la page"
 
 #: imio/smartweb/core/vocabularies.py:310
 msgid "Third page"
 msgstr "Tiers de la page"
 
 #: imio/smartweb/common/privacy.py:70
 msgid "This feature requires cookies acceptation.<br/><a class=\"pat-plone-modal\" href=\"${consent_url}\">Review your cookies preferences</a>."
 msgstr "Cette fonctionnalité nécessite l'acceptation des cookies.<br/><a class=\"pat-plone-modal\" href=\"${consent_url}\">Modifier vos préférences en matière de cookies</a>."
 
-#: imio/directory/core/contents/contact/content.py:203
+#: imio/directory/core/contents/contact/content.py:231
 #: imio/events/core/contents/event/content.py:48
 #: imio/news/core/contents/newsitem/content.py:34
 msgid "This field is required if the content must be available in this language"
 msgstr "Ce champ est requis si le contenu doit être disponible dans cette langue"
 
 #: imio/smartweb/core/browser/controlpanel.py:91
 msgid "This information is used for search results redirection"
@@ -2208,28 +2212,28 @@
 msgid "This site uses cookies to provide you with an optimal experience (playing videos, displaying maps and content from social networks in particular)."
 msgstr "Ce site utilise des cookies pour vous fournir une expérience optimale (lecture de vidéos, affichage de plans et de contenus issus des réseaux sociaux notamment)."
 
 #: imio/smartweb/core/vocabularies.py:128
 msgid "Three quarter of width"
 msgstr "Trois quarts de la page"
 
-#: imio/smartweb/core/contents/sections/contact/view.py:116
+#: imio/smartweb/core/contents/sections/contact/view.py:130
 msgid "Thursday"
 msgstr "Jeudi"
 
 #: imio/events/core/contents/event/content.py:114
 #: imio/events/core/contents/event/view.pt:67
 msgid "Ticket url"
 msgstr "Billeterie"
 
 #: imio/events/core/contents/event/content.py:115
 msgid "Ticket url to subscribe to this event"
 msgstr "Lien de la billeterie pour s'inscrire à cet événement"
 
-#: imio/directory/core/contents/contact/content.py:202
+#: imio/directory/core/contents/contact/content.py:230
 #: imio/events/core/contents/event/content.py:47
 #: imio/news/core/contents/newsitem/content.py:33
 msgid "Title"
 msgstr "Titre"
 
 #: imio/smartweb/core/vocabularies.py:157
 msgid "Title and Subtitle"
@@ -2257,15 +2261,15 @@
 msgid "Tourist"
 msgstr "Touriste"
 
 #: imio/events/core/vocabularies.py:25
 msgid "Trade Fair and Fair"
 msgstr "Salon et Foire"
 
-#: imio/smartweb/core/contents/sections/contact/view.py:114
+#: imio/smartweb/core/contents/sections/contact/view.py:128
 msgid "Tuesday"
 msgstr "Mardi"
 
 #: imio/directory/core/vocabularies.py:69
 #: imio/events/core/contents/event/content.py:132
 #: imio/events/core/contents/event/view.pt:77
 msgid "Twitter"
@@ -2279,35 +2283,35 @@
 msgid "Twitter url for this news"
 msgstr "Lien Twitter pour cette actualité"
 
 #: imio/smartweb/core/vocabularies.py:127
 msgid "Two third of width"
 msgstr "Deux tiers de la page"
 
-#: imio/directory/core/contents/contact/content.py:54
+#: imio/directory/core/contents/contact/content.py:82
 msgid "Type"
 msgstr ""
 
 #: imio/smartweb/core/contents/blocks/link/content.py:26
 msgid "URL"
 msgstr ""
 
-#: imio/directory/core/contents/contact/content.py:131
+#: imio/directory/core/contents/contact/content.py:159
 msgid "URLs"
 msgstr ""
 
-#: imio/directory/policy/configure.zcml:43
+#: imio/directory/policy/configure.zcml:44
 msgid "Uninstalls the imio.directory.policy add-on."
 msgstr ""
 
-#: imio/events/policy/configure.zcml:44
+#: imio/events/policy/configure.zcml:45
 msgid "Uninstalls the imio.events.policy add-on."
 msgstr ""
 
-#: imio/news/policy/configure.zcml:44
+#: imio/news/policy/configure.zcml:45
 msgid "Uninstalls the imio.news.policy add-on."
 msgstr ""
 
 #: imio/smartweb/policy/upgrades/configure.zcml:76
 msgid "Update caching configuration"
 msgstr ""
 
@@ -2339,14 +2343,18 @@
 msgid "Upgrade common from 1013 to 1014"
 msgstr ""
 
 #: imio/smartweb/common/upgrades/configure.zcml:61
 msgid "Upgrade common from 1014 to 1015"
 msgstr ""
 
+#: imio/smartweb/common/upgrades/configure.zcml:69
+msgid "Upgrade common from 1015 to 1016"
+msgstr ""
+
 #: imio/smartweb/core/upgrades/configure.zcml:92
 msgid "Upgrade common from 1031 to 1032"
 msgstr ""
 
 #: imio/smartweb/core/upgrades/configure.zcml:100
 msgid "Upgrade common from 1033 to 1034"
 msgstr ""
@@ -2497,15 +2505,15 @@
 msgid "Upgrade policy from 1026 to 1027"
 msgstr ""
 
 #: imio/smartweb/policy/upgrades/configure.zcml:124
 msgid "Upgrade policy from 1028 to 1029"
 msgstr ""
 
-#: imio/directory/core/contents/contact/content.py:92
+#: imio/directory/core/contents/contact/content.py:120
 msgid "Url"
 msgstr "URL"
 
 #: imio/smartweb/core/browser/controlpanel.py:25
 msgid "Url to get forms from your e-guichet"
 msgstr "Url de récupération des démarches de votre e-guichet"
 
@@ -2531,15 +2539,15 @@
 msgid "Use custom spotlight to avoid bad gallery refresh"
 msgstr ""
 
 #: imio/directory/core/vocabularies.py:86
 msgid "Useful numbers"
 msgstr "Numéros utiles"
 
-#: imio/directory/core/contents/contact/content.py:109
+#: imio/directory/core/contents/contact/content.py:137
 msgid "VAT number"
 msgstr "Numéro d'entreprise / TVA"
 
 #: imio/smartweb/core/profiles/default/types/imio.smartweb.SectionVideo.xml
 msgid "Video section"
 msgstr "Section vidéo"
 
@@ -2575,20 +2583,24 @@
 msgid "Visible blocks"
 msgstr "Blocs visibles"
 
 #: imio/smartweb/core/browser/controlpanel.py:116
 msgid "Vocabulary term"
 msgstr "Terme du vocabulaire"
 
+#: imio/smartweb/core/browser/overrides/plone.app.content.browser.contents.templates.properties.pt:3
+msgid "Warning: these options are not relevant for Sections and will not be applied."
+msgstr "Attention: ces options ne sont pas pertinentes pour les Sections et ne seront pas appliquées."
+
 #: imio/directory/core/vocabularies.py:70
 #: imio/news/core/contents/newsitem/content.py:85
 msgid "Website"
 msgstr "Site Internet"
 
-#: imio/smartweb/core/contents/sections/contact/view.py:115
+#: imio/smartweb/core/contents/sections/contact/view.py:129
 msgid "Wednesday"
 msgstr "Mercredi"
 
 #: imio/directory/core/vocabularies.py:54
 msgid "Work email"
 msgstr "Adresse e-mail professionnelle"
 
@@ -2638,35 +2650,35 @@
 msgid "Zipcode '${val}' is not a number."
 msgstr "Le code postal '${val}' n'est pas un nombre."
 
 #: imio/smartweb/common/viewlets/colophon.pt:34
 msgid "free license"
 msgstr "licence libre"
 
-#: imio/directory/policy/configure.zcml:34
+#: imio/directory/policy/configure.zcml:35
 msgid "imio.directory.policy"
 msgstr ""
 
-#: imio/directory/policy/configure.zcml:43
+#: imio/directory/policy/configure.zcml:44
 msgid "imio.directory.policy (uninstall)"
 msgstr ""
 
-#: imio/events/policy/configure.zcml:35
+#: imio/events/policy/configure.zcml:36
 msgid "imio.events.policy"
 msgstr ""
 
-#: imio/events/policy/configure.zcml:44
+#: imio/events/policy/configure.zcml:45
 msgid "imio.events.policy (uninstall)"
 msgstr ""
 
-#: imio/news/policy/configure.zcml:35
+#: imio/news/policy/configure.zcml:36
 msgid "imio.news.policy"
 msgstr ""
 
-#: imio/news/policy/configure.zcml:44
+#: imio/news/policy/configure.zcml:45
 msgid "imio.news.policy (uninstall)"
 msgstr ""
 
 #. Default: "You are editing the default page of a container. If you wanted to edit the container itself, ${go_here}."
 #: imio/smartweb/core/viewlets/default_page_warning.pt:7
 msgid "label_edit_default_page_container"
 msgstr "Vous modifiez actuellement la page d'accueil d'un dossier. Si vous voulez modifier le dossier lui-même, ${go_here}."
```

### Comparing `imio.smartweb.locales-1.1.3/src/imio/smartweb/locales/locales/de/LC_MESSAGES/plone.po` & `imio.smartweb.locales-1.1.4/src/imio/smartweb/locales/locales/de/LC_MESSAGES/plone.po`

 * *Files identical despite different names*

### Comparing `imio.smartweb.locales-1.1.3/src/imio.smartweb.locales.egg-info/SOURCES.txt` & `imio.smartweb.locales-1.1.4/src/imio.smartweb.locales.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 CHANGES.rst
 CONTRIBUTORS.rst
+LICENSE.GPL
 LICENSE.rst
 MANIFEST.in
 README.rst
 setup.cfg
 setup.py
 src/imio/__init__.py
 src/imio.smartweb.locales.egg-info/PKG-INFO
```

