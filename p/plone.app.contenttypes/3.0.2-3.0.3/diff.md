# Comparing `tmp/plone.app.contenttypes-3.0.2.tar.gz` & `tmp/plone.app.contenttypes-3.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plone.app.contenttypes-3.0.2.tar", last modified: Thu Apr 13 23:44:06 2023, max compression
+gzip compressed data, was "plone.app.contenttypes-3.0.3.tar", last modified: Mon May 22 17:57:28 2023, max compression
```

## Comparing `plone.app.contenttypes-3.0.2.tar` & `plone.app.contenttypes-3.0.3.tar`

### file list

```diff
@@ -1,152 +1,152 @@
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:44:06.818029 plone.app.contenttypes-3.0.2/
--rw-r--r--   0 maurits    (501) staff       (20)    46077 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/CHANGES.rst
--rw-r--r--   0 maurits    (501) staff       (20)       70 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/CONTRIBUTING.rst
--rw-r--r--   0 maurits    (501) staff       (20)      122 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/MANIFEST.in
--rw-r--r--   0 maurits    (501) staff       (20)    54057 2023-04-13 23:44:06.818167 plone.app.contenttypes-3.0.2/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)     7006 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/README.rst
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:44:06.783993 plone.app.contenttypes-3.0.2/docs/
--rw-r--r--   0 maurits    (501) staff       (20)     1334 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/docs/INSTALL.txt
--rw-r--r--   0 maurits    (501) staff       (20)    17987 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/docs/LICENSE.GPL
--rw-r--r--   0 maurits    (501) staff       (20)      737 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/docs/LICENSE.txt
--rw-r--r--   0 maurits    (501) staff       (20)     7006 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/docs/README.rst
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:44:06.784697 plone.app.contenttypes-3.0.2/docs/source/
--rw-r--r--   0 maurits    (501) staff       (20)     8036 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/docs/source/conf.py
--rw-r--r--   0 maurits    (501) staff       (20)      471 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/docs/source/index.rst
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:44:06.784951 plone.app.contenttypes-3.0.2/plone/
--rw-r--r--   0 maurits    (501) staff       (20)       56 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/plone/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:44:06.787284 plone.app.contenttypes-3.0.2/plone/app/
--rw-r--r--   0 maurits    (501) staff       (20)       56 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/plone/app/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:44:06.791550 plone.app.contenttypes-3.0.2/plone/app/contenttypes/
--rw-r--r--   0 maurits    (501) staff       (20)      127 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/plone/app/contenttypes/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:44:06.794484 plone.app.contenttypes-3.0.2/plone/app/contenttypes/behaviors/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/plone/app/contenttypes/behaviors/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     6169 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/plone/app/contenttypes/behaviors/collection.py
--rw-r--r--   0 maurits    (501) staff       (20)     2809 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/plone/app/contenttypes/behaviors/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)      548 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/plone/app/contenttypes/behaviors/leadimage.pt
--rw-r--r--   0 maurits    (501) staff       (20)     1320 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/plone/app/contenttypes/behaviors/leadimage.py
--rw-r--r--   0 maurits    (501) staff       (20)     1312 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/plone/app/contenttypes/behaviors/richtext.py
--rw-r--r--   0 maurits    (501) staff       (20)       63 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/plone/app/contenttypes/behaviors/richtext_gettext.pt
--rw-r--r--   0 maurits    (501) staff       (20)      728 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/plone/app/contenttypes/behaviors/tableofcontents.py
--rw-r--r--   0 maurits    (501) staff       (20)     2787 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/plone/app/contenttypes/behaviors/thumb_icon.py
--rw-r--r--   0 maurits    (501) staff       (20)      340 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/plone/app/contenttypes/behaviors/viewlets.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:44:06.796958 plone.app.contenttypes-3.0.2/plone/app/contenttypes/browser/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/plone/app/contenttypes/browser/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     2931 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/plone/app/contenttypes/browser/collection.py
--rw-r--r--   0 maurits    (501) staff       (20)     6737 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/plone/app/contenttypes/browser/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     1091 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/plone/app/contenttypes/browser/file.py
--rw-r--r--   0 maurits    (501) staff       (20)     8782 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/plone/app/contenttypes/browser/folder.py
--rw-r--r--   0 maurits    (501) staff       (20)      991 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/plone/app/contenttypes/browser/full_view.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:44:06.797596 plone.app.contenttypes-3.0.2/plone/app/contenttypes/browser/images/
--rw-r--r--   0 maurits    (501) staff       (20)      414 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/plone/app/contenttypes/browser/images/icon_export_ical.png
--rw-r--r--   0 maurits    (501) staff       (20)      427 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/plone/app/contenttypes/browser/images/icon_export_vcal.png
--rw-r--r--   0 maurits    (501) staff       (20)     3810 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/plone/app/contenttypes/browser/link_redirect_view.py
--rw-r--r--   0 maurits    (501) staff       (20)     4092 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/plone/app/contenttypes/browser/migration.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:44:06.801274 plone.app.contenttypes-3.0.2/plone/app/contenttypes/browser/templates/
--rw-r--r--   0 maurits    (501) staff       (20)     1045 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/plone/app/contenttypes/browser/templates/document.pt
--rw-r--r--   0 maurits    (501) staff       (20)     3434 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/plone/app/contenttypes/browser/templates/file.pt
--rw-r--r--   0 maurits    (501) staff       (20)     1264 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/plone/app/contenttypes/browser/templates/full_view.pt
--rw-r--r--   0 maurits    (501) staff       (20)     2497 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/plone/app/contenttypes/browser/templates/full_view_item.pt
--rw-r--r--   0 maurits    (501) staff       (20)     3669 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/plone/app/contenttypes/browser/templates/image.pt
--rw-r--r--   0 maurits    (501) staff       (20)     2069 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/plone/app/contenttypes/browser/templates/image_view_fullscreen.pt
--rw-r--r--   0 maurits    (501) staff       (20)     2552 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/plone/app/contenttypes/browser/templates/link.pt
--rw-r--r--   0 maurits    (501) staff       (20)     8869 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/plone/app/contenttypes/browser/templates/listing.pt
--rw-r--r--   0 maurits    (501) staff       (20)     4474 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/plone/app/contenttypes/browser/templates/listing_album.pt
--rw-r--r--   0 maurits    (501) staff       (20)     2926 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/plone/app/contenttypes/browser/templates/listing_summary.pt
--rw-r--r--   0 maurits    (501) staff       (20)     7518 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/plone/app/contenttypes/browser/templates/listing_tabular.pt
--rw-r--r--   0 maurits    (501) staff       (20)     1091 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/plone/app/contenttypes/browser/templates/newsitem.pt
--rw-r--r--   0 maurits    (501) staff       (20)     1964 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/plone/app/contenttypes/browser/utils.py
--rw-r--r--   0 maurits    (501) staff       (20)     1781 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/plone/app/contenttypes/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     6481 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/plone/app/contenttypes/content.py
--rw-r--r--   0 maurits    (501) staff       (20)     5847 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/plone/app/contenttypes/indexers.py
--rw-r--r--   0 maurits    (501) staff       (20)     1251 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/plone/app/contenttypes/indexers.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     1018 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/plone/app/contenttypes/interfaces.py
--rw-r--r--   0 maurits    (501) staff       (20)      912 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/plone/app/contenttypes/permissions.py
--rw-r--r--   0 maurits    (501) staff       (20)     1227 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/plone/app/contenttypes/permissions.zcml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:44:06.780225 plone.app.contenttypes-3.0.2/plone/app/contenttypes/profiles/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:44:06.801770 plone.app.contenttypes-3.0.2/plone/app/contenttypes/profiles/content/
--rw-r--r--   0 maurits    (501) staff       (20)      191 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/plone/app/contenttypes/profiles/content/metadata.xml
--rw-r--r--   0 maurits    (501) staff       (20)      591 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/plone/app/contenttypes/profiles/content/portlets.xml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:44:06.803093 plone.app.contenttypes-3.0.2/plone/app/contenttypes/profiles/default/
--rw-r--r--   0 maurits    (501) staff       (20)      184 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/plone/app/contenttypes/profiles/default/browserlayer.xml
--rw-r--r--   0 maurits    (501) staff       (20)     1031 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/plone/app/contenttypes/profiles/default/diff_tool.xml
--rw-r--r--   0 maurits    (501) staff       (20)      522 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/plone/app/contenttypes/profiles/default/metadata.xml
--rw-r--r--   0 maurits    (501) staff       (20)     2113 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/plone/app/contenttypes/profiles/default/rolemap.xml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:44:06.805497 plone.app.contenttypes-3.0.2/plone/app/contenttypes/profiles/default/types/
--rw-r--r--   0 maurits    (501) staff       (20)     3097 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/plone/app/contenttypes/profiles/default/types/Collection.xml
--rw-r--r--   0 maurits    (501) staff       (20)     2943 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/plone/app/contenttypes/profiles/default/types/Document.xml
--rw-r--r--   0 maurits    (501) staff       (20)     3175 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/plone/app/contenttypes/profiles/default/types/Event.xml
--rw-r--r--   0 maurits    (501) staff       (20)     2810 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/plone/app/contenttypes/profiles/default/types/File.xml
--rw-r--r--   0 maurits    (501) staff       (20)     2974 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/plone/app/contenttypes/profiles/default/types/Folder.xml
--rw-r--r--   0 maurits    (501) staff       (20)     2844 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/plone/app/contenttypes/profiles/default/types/Image.xml
--rw-r--r--   0 maurits    (501) staff       (20)     2692 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/plone/app/contenttypes/profiles/default/types/Link.xml
--rw-r--r--   0 maurits    (501) staff       (20)     2947 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/plone/app/contenttypes/profiles/default/types/News_Item.xml
--rw-r--r--   0 maurits    (501) staff       (20)      648 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/plone/app/contenttypes/profiles/default/types/Plone_Site.xml
--rw-r--r--   0 maurits    (501) staff       (20)     1957 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/plone/app/contenttypes/profiles/default/types.xml
--rw-r--r--   0 maurits    (501) staff       (20)      963 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/plone/app/contenttypes/profiles.zcml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:44:06.807733 plone.app.contenttypes-3.0.2/plone/app/contenttypes/schema/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/plone/app/contenttypes/schema/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)      131 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/plone/app/contenttypes/schema/collection.xml
--rw-r--r--   0 maurits    (501) staff       (20)      131 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/plone/app/contenttypes/schema/document.xml
--rw-r--r--   0 maurits    (501) staff       (20)      131 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/plone/app/contenttypes/schema/event.xml
--rw-r--r--   0 maurits    (501) staff       (20)      865 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/plone/app/contenttypes/schema/file.xml
--rw-r--r--   0 maurits    (501) staff       (20)      131 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/plone/app/contenttypes/schema/folder.xml
--rw-r--r--   0 maurits    (501) staff       (20)      869 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/plone/app/contenttypes/schema/image.xml
--rw-r--r--   0 maurits    (501) staff       (20)      880 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/plone/app/contenttypes/schema/link.xml
--rw-r--r--   0 maurits    (501) staff       (20)      131 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/plone/app/contenttypes/schema/news_item.xml
--rw-r--r--   0 maurits    (501) staff       (20)    12355 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/plone/app/contenttypes/setuphandlers.py
--rw-r--r--   0 maurits    (501) staff       (20)      585 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/plone/app/contenttypes/subscribers.py
--rw-r--r--   0 maurits    (501) staff       (20)      401 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/plone/app/contenttypes/subscribers.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     2669 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/plone/app/contenttypes/testing.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:44:06.815409 plone.app.contenttypes-3.0.2/plone/app/contenttypes/tests/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/plone/app/contenttypes/tests/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     9216 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/plone/app/contenttypes/tests/file.doc
--rw-r--r--   0 maurits    (501) staff       (20)     9338 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/plone/app/contenttypes/tests/file.odt
--rw-r--r--   0 maurits    (501) staff       (20)     8561 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/plone/app/contenttypes/tests/file.pdf
--rw-r--r--   0 maurits    (501) staff       (20)     5131 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/plone/app/contenttypes/tests/image.jpg
--rw-r--r--   0 maurits    (501) staff       (20)     1185 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/plone/app/contenttypes/tests/image.png
--rw-r--r--   0 maurits    (501) staff       (20)     9344 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/plone/app/contenttypes/tests/image.svg
--rw-r--r--   0 maurits    (501) staff       (20)     4063 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/plone/app/contenttypes/tests/oldtypes.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:44:06.817816 plone.app.contenttypes-3.0.2/plone/app/contenttypes/tests/robot/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/plone/app/contenttypes/tests/robot/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     5132 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/plone/app/contenttypes/tests/robot/keywords.txt
--rw-r--r--   0 maurits    (501) staff       (20)     2117 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/plone/app/contenttypes/tests/robot/test_collection_creator_criterion.robot
--rw-r--r--   0 maurits    (501) staff       (20)     4067 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/plone/app/contenttypes/tests/robot/test_collection_location_criterion.robot
--rw-r--r--   0 maurits    (501) staff       (20)     2088 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/plone/app/contenttypes/tests/robot/test_collection_review_state_criterion.robot
--rw-r--r--   0 maurits    (501) staff       (20)     1869 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/plone/app/contenttypes/tests/robot/test_collection_short_name_criterion.robot
--rw-r--r--   0 maurits    (501) staff       (20)     1818 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/plone/app/contenttypes/tests/robot/test_collection_type_criterion.robot
--rw-r--r--   0 maurits    (501) staff       (20)    11981 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/plone/app/contenttypes/tests/robot/test_folderlisting.robot
--rw-r--r--   0 maurits    (501) staff       (20)      339 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/plone/app/contenttypes/tests/robot/variables.py
--rw-r--r--   0 maurits    (501) staff       (20)     3888 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/plone/app/contenttypes/tests/test_behaviors_collection.py
--rw-r--r--   0 maurits    (501) staff       (20)     3277 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/plone/app/contenttypes/tests/test_behaviors_leadimage.py
--rw-r--r--   0 maurits    (501) staff       (20)     2205 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/plone/app/contenttypes/tests/test_behaviors_richtext.py
--rw-r--r--   0 maurits    (501) staff       (20)     2278 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/plone/app/contenttypes/tests/test_behaviors_table_of_contents.py
--rw-r--r--   0 maurits    (501) staff       (20)     1524 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/plone/app/contenttypes/tests/test_browser_utils.py
--rw-r--r--   0 maurits    (501) staff       (20)    14842 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/plone/app/contenttypes/tests/test_collection.py
--rw-r--r--   0 maurits    (501) staff       (20)     2521 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/plone/app/contenttypes/tests/test_collection_rss.py
--rw-r--r--   0 maurits    (501) staff       (20)     5127 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/plone/app/contenttypes/tests/test_content_profile.py
--rw-r--r--   0 maurits    (501) staff       (20)     4321 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/plone/app/contenttypes/tests/test_document.py
--rw-r--r--   0 maurits    (501) staff       (20)     4346 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/plone/app/contenttypes/tests/test_event.py
--rw-r--r--   0 maurits    (501) staff       (20)     8996 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/plone/app/contenttypes/tests/test_file.py
--rw-r--r--   0 maurits    (501) staff       (20)     8912 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/plone/app/contenttypes/tests/test_folder.py
--rw-r--r--   0 maurits    (501) staff       (20)     7360 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/plone/app/contenttypes/tests/test_image.py
--rw-r--r--   0 maurits    (501) staff       (20)    11959 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/plone/app/contenttypes/tests/test_indexes.py
--rw-r--r--   0 maurits    (501) staff       (20)    13550 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/plone/app/contenttypes/tests/test_link.py
--rw-r--r--   0 maurits    (501) staff       (20)     5554 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/plone/app/contenttypes/tests/test_news_item.py
--rw-r--r--   0 maurits    (501) staff       (20)      965 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/plone/app/contenttypes/tests/test_robot.py
--rw-r--r--   0 maurits    (501) staff       (20)     8278 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/plone/app/contenttypes/tests/test_security.py
--rw-r--r--   0 maurits    (501) staff       (20)     1542 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/plone/app/contenttypes/tests/test_setup.py
--rw-r--r--   0 maurits    (501) staff       (20)     2318 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/plone/app/contenttypes/tests/test_webdav.py
--rw-r--r--   0 maurits    (501) staff       (20)     4530 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/plone/app/contenttypes/upgrades.py
--rw-r--r--   0 maurits    (501) staff       (20)      392 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/plone/app/contenttypes/upgrades.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     4071 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/plone/app/contenttypes/utils.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:44:06.786918 plone.app.contenttypes-3.0.2/plone.app.contenttypes.egg-info/
--rw-r--r--   0 maurits    (501) staff       (20)    54057 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/plone.app.contenttypes.egg-info/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)     5930 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/plone.app.contenttypes.egg-info/SOURCES.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/plone.app.contenttypes.egg-info/dependency_links.txt
--rw-r--r--   0 maurits    (501) staff       (20)       16 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/plone.app.contenttypes.egg-info/namespace_packages.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/plone.app.contenttypes.egg-info/not-zip-safe
--rw-r--r--   0 maurits    (501) staff       (20)      848 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/plone.app.contenttypes.egg-info/requires.txt
--rw-r--r--   0 maurits    (501) staff       (20)        6 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/plone.app.contenttypes.egg-info/top_level.txt
--rw-r--r--   0 maurits    (501) staff       (20)     1707 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/pyproject.toml
--rw-r--r--   0 maurits    (501) staff       (20)      217 2023-04-13 23:44:06.818623 plone.app.contenttypes-3.0.2/setup.cfg
--rw-r--r--   0 maurits    (501) staff       (20)     3164 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/setup.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-22 17:57:28.323477 plone.app.contenttypes-3.0.3/
+-rw-r--r--   0 maurits    (501) staff       (20)    46299 2023-05-22 17:57:27.000000 plone.app.contenttypes-3.0.3/CHANGES.rst
+-rw-r--r--   0 maurits    (501) staff       (20)       70 2023-05-22 17:57:27.000000 plone.app.contenttypes-3.0.3/CONTRIBUTING.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      122 2023-05-22 17:57:27.000000 plone.app.contenttypes-3.0.3/MANIFEST.in
+-rw-r--r--   0 maurits    (501) staff       (20)    54279 2023-05-22 17:57:28.323616 plone.app.contenttypes-3.0.3/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)     7006 2023-05-22 17:57:27.000000 plone.app.contenttypes-3.0.3/README.rst
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-22 17:57:28.285754 plone.app.contenttypes-3.0.3/docs/
+-rw-r--r--   0 maurits    (501) staff       (20)     1334 2023-05-22 17:57:27.000000 plone.app.contenttypes-3.0.3/docs/INSTALL.txt
+-rw-r--r--   0 maurits    (501) staff       (20)    17987 2023-05-22 17:57:27.000000 plone.app.contenttypes-3.0.3/docs/LICENSE.GPL
+-rw-r--r--   0 maurits    (501) staff       (20)      737 2023-05-22 17:57:27.000000 plone.app.contenttypes-3.0.3/docs/LICENSE.txt
+-rw-r--r--   0 maurits    (501) staff       (20)     7006 2023-05-22 17:57:27.000000 plone.app.contenttypes-3.0.3/docs/README.rst
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-22 17:57:28.286512 plone.app.contenttypes-3.0.3/docs/source/
+-rw-r--r--   0 maurits    (501) staff       (20)     8036 2023-05-22 17:57:27.000000 plone.app.contenttypes-3.0.3/docs/source/conf.py
+-rw-r--r--   0 maurits    (501) staff       (20)      471 2023-05-22 17:57:27.000000 plone.app.contenttypes-3.0.3/docs/source/index.rst
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-22 17:57:28.286996 plone.app.contenttypes-3.0.3/plone/
+-rw-r--r--   0 maurits    (501) staff       (20)       56 2023-05-22 17:57:27.000000 plone.app.contenttypes-3.0.3/plone/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-22 17:57:28.289704 plone.app.contenttypes-3.0.3/plone/app/
+-rw-r--r--   0 maurits    (501) staff       (20)       56 2023-05-22 17:57:27.000000 plone.app.contenttypes-3.0.3/plone/app/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-22 17:57:28.294399 plone.app.contenttypes-3.0.3/plone/app/contenttypes/
+-rw-r--r--   0 maurits    (501) staff       (20)      127 2023-05-22 17:57:27.000000 plone.app.contenttypes-3.0.3/plone/app/contenttypes/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-22 17:57:28.297352 plone.app.contenttypes-3.0.3/plone/app/contenttypes/behaviors/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2023-05-22 17:57:27.000000 plone.app.contenttypes-3.0.3/plone/app/contenttypes/behaviors/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     6169 2023-05-22 17:57:27.000000 plone.app.contenttypes-3.0.3/plone/app/contenttypes/behaviors/collection.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2809 2023-05-22 17:57:27.000000 plone.app.contenttypes-3.0.3/plone/app/contenttypes/behaviors/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)      548 2023-05-22 17:57:27.000000 plone.app.contenttypes-3.0.3/plone/app/contenttypes/behaviors/leadimage.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     1320 2023-05-22 17:57:27.000000 plone.app.contenttypes-3.0.3/plone/app/contenttypes/behaviors/leadimage.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1312 2023-05-22 17:57:27.000000 plone.app.contenttypes-3.0.3/plone/app/contenttypes/behaviors/richtext.py
+-rw-r--r--   0 maurits    (501) staff       (20)       63 2023-05-22 17:57:27.000000 plone.app.contenttypes-3.0.3/plone/app/contenttypes/behaviors/richtext_gettext.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      728 2023-05-22 17:57:27.000000 plone.app.contenttypes-3.0.3/plone/app/contenttypes/behaviors/tableofcontents.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2787 2023-05-22 17:57:27.000000 plone.app.contenttypes-3.0.3/plone/app/contenttypes/behaviors/thumb_icon.py
+-rw-r--r--   0 maurits    (501) staff       (20)      340 2023-05-22 17:57:27.000000 plone.app.contenttypes-3.0.3/plone/app/contenttypes/behaviors/viewlets.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-22 17:57:28.300015 plone.app.contenttypes-3.0.3/plone/app/contenttypes/browser/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2023-05-22 17:57:27.000000 plone.app.contenttypes-3.0.3/plone/app/contenttypes/browser/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2931 2023-05-22 17:57:27.000000 plone.app.contenttypes-3.0.3/plone/app/contenttypes/browser/collection.py
+-rw-r--r--   0 maurits    (501) staff       (20)     6737 2023-05-22 17:57:27.000000 plone.app.contenttypes-3.0.3/plone/app/contenttypes/browser/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     1091 2023-05-22 17:57:27.000000 plone.app.contenttypes-3.0.3/plone/app/contenttypes/browser/file.py
+-rw-r--r--   0 maurits    (501) staff       (20)     8782 2023-05-22 17:57:27.000000 plone.app.contenttypes-3.0.3/plone/app/contenttypes/browser/folder.py
+-rw-r--r--   0 maurits    (501) staff       (20)      991 2023-05-22 17:57:27.000000 plone.app.contenttypes-3.0.3/plone/app/contenttypes/browser/full_view.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-22 17:57:28.300844 plone.app.contenttypes-3.0.3/plone/app/contenttypes/browser/images/
+-rw-r--r--   0 maurits    (501) staff       (20)      414 2023-05-22 17:57:27.000000 plone.app.contenttypes-3.0.3/plone/app/contenttypes/browser/images/icon_export_ical.png
+-rw-r--r--   0 maurits    (501) staff       (20)      427 2023-05-22 17:57:27.000000 plone.app.contenttypes-3.0.3/plone/app/contenttypes/browser/images/icon_export_vcal.png
+-rw-r--r--   0 maurits    (501) staff       (20)     4101 2023-05-22 17:57:27.000000 plone.app.contenttypes-3.0.3/plone/app/contenttypes/browser/link_redirect_view.py
+-rw-r--r--   0 maurits    (501) staff       (20)     4092 2023-05-22 17:57:27.000000 plone.app.contenttypes-3.0.3/plone/app/contenttypes/browser/migration.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-22 17:57:28.304708 plone.app.contenttypes-3.0.3/plone/app/contenttypes/browser/templates/
+-rw-r--r--   0 maurits    (501) staff       (20)     1045 2023-05-22 17:57:27.000000 plone.app.contenttypes-3.0.3/plone/app/contenttypes/browser/templates/document.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     3434 2023-05-22 17:57:27.000000 plone.app.contenttypes-3.0.3/plone/app/contenttypes/browser/templates/file.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     1264 2023-05-22 17:57:27.000000 plone.app.contenttypes-3.0.3/plone/app/contenttypes/browser/templates/full_view.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     2497 2023-05-22 17:57:27.000000 plone.app.contenttypes-3.0.3/plone/app/contenttypes/browser/templates/full_view_item.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     3669 2023-05-22 17:57:27.000000 plone.app.contenttypes-3.0.3/plone/app/contenttypes/browser/templates/image.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     2069 2023-05-22 17:57:27.000000 plone.app.contenttypes-3.0.3/plone/app/contenttypes/browser/templates/image_view_fullscreen.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     2552 2023-05-22 17:57:27.000000 plone.app.contenttypes-3.0.3/plone/app/contenttypes/browser/templates/link.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     8869 2023-05-22 17:57:27.000000 plone.app.contenttypes-3.0.3/plone/app/contenttypes/browser/templates/listing.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     4474 2023-05-22 17:57:27.000000 plone.app.contenttypes-3.0.3/plone/app/contenttypes/browser/templates/listing_album.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     2926 2023-05-22 17:57:27.000000 plone.app.contenttypes-3.0.3/plone/app/contenttypes/browser/templates/listing_summary.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     7518 2023-05-22 17:57:27.000000 plone.app.contenttypes-3.0.3/plone/app/contenttypes/browser/templates/listing_tabular.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     1091 2023-05-22 17:57:27.000000 plone.app.contenttypes-3.0.3/plone/app/contenttypes/browser/templates/newsitem.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     1964 2023-05-22 17:57:27.000000 plone.app.contenttypes-3.0.3/plone/app/contenttypes/browser/utils.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1842 2023-05-22 17:57:27.000000 plone.app.contenttypes-3.0.3/plone/app/contenttypes/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     6481 2023-05-22 17:57:27.000000 plone.app.contenttypes-3.0.3/plone/app/contenttypes/content.py
+-rw-r--r--   0 maurits    (501) staff       (20)     5847 2023-05-22 17:57:27.000000 plone.app.contenttypes-3.0.3/plone/app/contenttypes/indexers.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1251 2023-05-22 17:57:27.000000 plone.app.contenttypes-3.0.3/plone/app/contenttypes/indexers.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     1018 2023-05-22 17:57:27.000000 plone.app.contenttypes-3.0.3/plone/app/contenttypes/interfaces.py
+-rw-r--r--   0 maurits    (501) staff       (20)      912 2023-05-22 17:57:27.000000 plone.app.contenttypes-3.0.3/plone/app/contenttypes/permissions.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1227 2023-05-22 17:57:27.000000 plone.app.contenttypes-3.0.3/plone/app/contenttypes/permissions.zcml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-22 17:57:28.281103 plone.app.contenttypes-3.0.3/plone/app/contenttypes/profiles/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-22 17:57:28.305228 plone.app.contenttypes-3.0.3/plone/app/contenttypes/profiles/content/
+-rw-r--r--   0 maurits    (501) staff       (20)      191 2023-05-22 17:57:27.000000 plone.app.contenttypes-3.0.3/plone/app/contenttypes/profiles/content/metadata.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      591 2023-05-22 17:57:27.000000 plone.app.contenttypes-3.0.3/plone/app/contenttypes/profiles/content/portlets.xml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-22 17:57:28.306743 plone.app.contenttypes-3.0.3/plone/app/contenttypes/profiles/default/
+-rw-r--r--   0 maurits    (501) staff       (20)      184 2023-05-22 17:57:27.000000 plone.app.contenttypes-3.0.3/plone/app/contenttypes/profiles/default/browserlayer.xml
+-rw-r--r--   0 maurits    (501) staff       (20)     1031 2023-05-22 17:57:27.000000 plone.app.contenttypes-3.0.3/plone/app/contenttypes/profiles/default/diff_tool.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      461 2023-05-22 17:57:27.000000 plone.app.contenttypes-3.0.3/plone/app/contenttypes/profiles/default/metadata.xml
+-rw-r--r--   0 maurits    (501) staff       (20)     2113 2023-05-22 17:57:27.000000 plone.app.contenttypes-3.0.3/plone/app/contenttypes/profiles/default/rolemap.xml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-22 17:57:28.309501 plone.app.contenttypes-3.0.3/plone/app/contenttypes/profiles/default/types/
+-rw-r--r--   0 maurits    (501) staff       (20)     3097 2023-05-22 17:57:27.000000 plone.app.contenttypes-3.0.3/plone/app/contenttypes/profiles/default/types/Collection.xml
+-rw-r--r--   0 maurits    (501) staff       (20)     2943 2023-05-22 17:57:27.000000 plone.app.contenttypes-3.0.3/plone/app/contenttypes/profiles/default/types/Document.xml
+-rw-r--r--   0 maurits    (501) staff       (20)     3175 2023-05-22 17:57:27.000000 plone.app.contenttypes-3.0.3/plone/app/contenttypes/profiles/default/types/Event.xml
+-rw-r--r--   0 maurits    (501) staff       (20)     2810 2023-05-22 17:57:27.000000 plone.app.contenttypes-3.0.3/plone/app/contenttypes/profiles/default/types/File.xml
+-rw-r--r--   0 maurits    (501) staff       (20)     2974 2023-05-22 17:57:27.000000 plone.app.contenttypes-3.0.3/plone/app/contenttypes/profiles/default/types/Folder.xml
+-rw-r--r--   0 maurits    (501) staff       (20)     2844 2023-05-22 17:57:27.000000 plone.app.contenttypes-3.0.3/plone/app/contenttypes/profiles/default/types/Image.xml
+-rw-r--r--   0 maurits    (501) staff       (20)     2692 2023-05-22 17:57:27.000000 plone.app.contenttypes-3.0.3/plone/app/contenttypes/profiles/default/types/Link.xml
+-rw-r--r--   0 maurits    (501) staff       (20)     2947 2023-05-22 17:57:27.000000 plone.app.contenttypes-3.0.3/plone/app/contenttypes/profiles/default/types/News_Item.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      648 2023-05-22 17:57:27.000000 plone.app.contenttypes-3.0.3/plone/app/contenttypes/profiles/default/types/Plone_Site.xml
+-rw-r--r--   0 maurits    (501) staff       (20)     1957 2023-05-22 17:57:27.000000 plone.app.contenttypes-3.0.3/plone/app/contenttypes/profiles/default/types.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      963 2023-05-22 17:57:27.000000 plone.app.contenttypes-3.0.3/plone/app/contenttypes/profiles.zcml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-22 17:57:28.312374 plone.app.contenttypes-3.0.3/plone/app/contenttypes/schema/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2023-05-22 17:57:27.000000 plone.app.contenttypes-3.0.3/plone/app/contenttypes/schema/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)      131 2023-05-22 17:57:27.000000 plone.app.contenttypes-3.0.3/plone/app/contenttypes/schema/collection.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      131 2023-05-22 17:57:27.000000 plone.app.contenttypes-3.0.3/plone/app/contenttypes/schema/document.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      131 2023-05-22 17:57:27.000000 plone.app.contenttypes-3.0.3/plone/app/contenttypes/schema/event.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      865 2023-05-22 17:57:27.000000 plone.app.contenttypes-3.0.3/plone/app/contenttypes/schema/file.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      131 2023-05-22 17:57:27.000000 plone.app.contenttypes-3.0.3/plone/app/contenttypes/schema/folder.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      869 2023-05-22 17:57:27.000000 plone.app.contenttypes-3.0.3/plone/app/contenttypes/schema/image.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      880 2023-05-22 17:57:27.000000 plone.app.contenttypes-3.0.3/plone/app/contenttypes/schema/link.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      131 2023-05-22 17:57:27.000000 plone.app.contenttypes-3.0.3/plone/app/contenttypes/schema/news_item.xml
+-rw-r--r--   0 maurits    (501) staff       (20)    12750 2023-05-22 17:57:27.000000 plone.app.contenttypes-3.0.3/plone/app/contenttypes/setuphandlers.py
+-rw-r--r--   0 maurits    (501) staff       (20)      585 2023-05-22 17:57:27.000000 plone.app.contenttypes-3.0.3/plone/app/contenttypes/subscribers.py
+-rw-r--r--   0 maurits    (501) staff       (20)      401 2023-05-22 17:57:27.000000 plone.app.contenttypes-3.0.3/plone/app/contenttypes/subscribers.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     2477 2023-05-22 17:57:27.000000 plone.app.contenttypes-3.0.3/plone/app/contenttypes/testing.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-22 17:57:28.320788 plone.app.contenttypes-3.0.3/plone/app/contenttypes/tests/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2023-05-22 17:57:27.000000 plone.app.contenttypes-3.0.3/plone/app/contenttypes/tests/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     9216 2023-05-22 17:57:27.000000 plone.app.contenttypes-3.0.3/plone/app/contenttypes/tests/file.doc
+-rw-r--r--   0 maurits    (501) staff       (20)     9338 2023-05-22 17:57:27.000000 plone.app.contenttypes-3.0.3/plone/app/contenttypes/tests/file.odt
+-rw-r--r--   0 maurits    (501) staff       (20)     8561 2023-05-22 17:57:27.000000 plone.app.contenttypes-3.0.3/plone/app/contenttypes/tests/file.pdf
+-rw-r--r--   0 maurits    (501) staff       (20)     5131 2023-05-22 17:57:27.000000 plone.app.contenttypes-3.0.3/plone/app/contenttypes/tests/image.jpg
+-rw-r--r--   0 maurits    (501) staff       (20)     1185 2023-05-22 17:57:27.000000 plone.app.contenttypes-3.0.3/plone/app/contenttypes/tests/image.png
+-rw-r--r--   0 maurits    (501) staff       (20)     9344 2023-05-22 17:57:27.000000 plone.app.contenttypes-3.0.3/plone/app/contenttypes/tests/image.svg
+-rw-r--r--   0 maurits    (501) staff       (20)     4063 2023-05-22 17:57:27.000000 plone.app.contenttypes-3.0.3/plone/app/contenttypes/tests/oldtypes.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-22 17:57:28.323278 plone.app.contenttypes-3.0.3/plone/app/contenttypes/tests/robot/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2023-05-22 17:57:27.000000 plone.app.contenttypes-3.0.3/plone/app/contenttypes/tests/robot/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     5132 2023-05-22 17:57:27.000000 plone.app.contenttypes-3.0.3/plone/app/contenttypes/tests/robot/keywords.txt
+-rw-r--r--   0 maurits    (501) staff       (20)     2117 2023-05-22 17:57:27.000000 plone.app.contenttypes-3.0.3/plone/app/contenttypes/tests/robot/test_collection_creator_criterion.robot
+-rw-r--r--   0 maurits    (501) staff       (20)     4067 2023-05-22 17:57:27.000000 plone.app.contenttypes-3.0.3/plone/app/contenttypes/tests/robot/test_collection_location_criterion.robot
+-rw-r--r--   0 maurits    (501) staff       (20)     2088 2023-05-22 17:57:27.000000 plone.app.contenttypes-3.0.3/plone/app/contenttypes/tests/robot/test_collection_review_state_criterion.robot
+-rw-r--r--   0 maurits    (501) staff       (20)     1869 2023-05-22 17:57:27.000000 plone.app.contenttypes-3.0.3/plone/app/contenttypes/tests/robot/test_collection_short_name_criterion.robot
+-rw-r--r--   0 maurits    (501) staff       (20)     1818 2023-05-22 17:57:27.000000 plone.app.contenttypes-3.0.3/plone/app/contenttypes/tests/robot/test_collection_type_criterion.robot
+-rw-r--r--   0 maurits    (501) staff       (20)    11981 2023-05-22 17:57:27.000000 plone.app.contenttypes-3.0.3/plone/app/contenttypes/tests/robot/test_folderlisting.robot
+-rw-r--r--   0 maurits    (501) staff       (20)      339 2023-05-22 17:57:27.000000 plone.app.contenttypes-3.0.3/plone/app/contenttypes/tests/robot/variables.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3888 2023-05-22 17:57:27.000000 plone.app.contenttypes-3.0.3/plone/app/contenttypes/tests/test_behaviors_collection.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3277 2023-05-22 17:57:27.000000 plone.app.contenttypes-3.0.3/plone/app/contenttypes/tests/test_behaviors_leadimage.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2205 2023-05-22 17:57:27.000000 plone.app.contenttypes-3.0.3/plone/app/contenttypes/tests/test_behaviors_richtext.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2278 2023-05-22 17:57:27.000000 plone.app.contenttypes-3.0.3/plone/app/contenttypes/tests/test_behaviors_table_of_contents.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1524 2023-05-22 17:57:27.000000 plone.app.contenttypes-3.0.3/plone/app/contenttypes/tests/test_browser_utils.py
+-rw-r--r--   0 maurits    (501) staff       (20)    14842 2023-05-22 17:57:27.000000 plone.app.contenttypes-3.0.3/plone/app/contenttypes/tests/test_collection.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2521 2023-05-22 17:57:27.000000 plone.app.contenttypes-3.0.3/plone/app/contenttypes/tests/test_collection_rss.py
+-rw-r--r--   0 maurits    (501) staff       (20)     5127 2023-05-22 17:57:27.000000 plone.app.contenttypes-3.0.3/plone/app/contenttypes/tests/test_content_profile.py
+-rw-r--r--   0 maurits    (501) staff       (20)     4321 2023-05-22 17:57:27.000000 plone.app.contenttypes-3.0.3/plone/app/contenttypes/tests/test_document.py
+-rw-r--r--   0 maurits    (501) staff       (20)     4346 2023-05-22 17:57:27.000000 plone.app.contenttypes-3.0.3/plone/app/contenttypes/tests/test_event.py
+-rw-r--r--   0 maurits    (501) staff       (20)     8996 2023-05-22 17:57:27.000000 plone.app.contenttypes-3.0.3/plone/app/contenttypes/tests/test_file.py
+-rw-r--r--   0 maurits    (501) staff       (20)     8912 2023-05-22 17:57:27.000000 plone.app.contenttypes-3.0.3/plone/app/contenttypes/tests/test_folder.py
+-rw-r--r--   0 maurits    (501) staff       (20)     7360 2023-05-22 17:57:27.000000 plone.app.contenttypes-3.0.3/plone/app/contenttypes/tests/test_image.py
+-rw-r--r--   0 maurits    (501) staff       (20)    11959 2023-05-22 17:57:27.000000 plone.app.contenttypes-3.0.3/plone/app/contenttypes/tests/test_indexes.py
+-rw-r--r--   0 maurits    (501) staff       (20)    14021 2023-05-22 17:57:27.000000 plone.app.contenttypes-3.0.3/plone/app/contenttypes/tests/test_link.py
+-rw-r--r--   0 maurits    (501) staff       (20)     5554 2023-05-22 17:57:27.000000 plone.app.contenttypes-3.0.3/plone/app/contenttypes/tests/test_news_item.py
+-rw-r--r--   0 maurits    (501) staff       (20)      965 2023-05-22 17:57:27.000000 plone.app.contenttypes-3.0.3/plone/app/contenttypes/tests/test_robot.py
+-rw-r--r--   0 maurits    (501) staff       (20)     8278 2023-05-22 17:57:27.000000 plone.app.contenttypes-3.0.3/plone/app/contenttypes/tests/test_security.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1542 2023-05-22 17:57:27.000000 plone.app.contenttypes-3.0.3/plone/app/contenttypes/tests/test_setup.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2318 2023-05-22 17:57:27.000000 plone.app.contenttypes-3.0.3/plone/app/contenttypes/tests/test_webdav.py
+-rw-r--r--   0 maurits    (501) staff       (20)     4530 2023-05-22 17:57:27.000000 plone.app.contenttypes-3.0.3/plone/app/contenttypes/upgrades.py
+-rw-r--r--   0 maurits    (501) staff       (20)      392 2023-05-22 17:57:27.000000 plone.app.contenttypes-3.0.3/plone/app/contenttypes/upgrades.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     4071 2023-05-22 17:57:27.000000 plone.app.contenttypes-3.0.3/plone/app/contenttypes/utils.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-22 17:57:28.289409 plone.app.contenttypes-3.0.3/plone.app.contenttypes.egg-info/
+-rw-r--r--   0 maurits    (501) staff       (20)    54279 2023-05-22 17:57:28.000000 plone.app.contenttypes-3.0.3/plone.app.contenttypes.egg-info/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)     5930 2023-05-22 17:57:28.000000 plone.app.contenttypes-3.0.3/plone.app.contenttypes.egg-info/SOURCES.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2023-05-22 17:57:28.000000 plone.app.contenttypes-3.0.3/plone.app.contenttypes.egg-info/dependency_links.txt
+-rw-r--r--   0 maurits    (501) staff       (20)       16 2023-05-22 17:57:28.000000 plone.app.contenttypes-3.0.3/plone.app.contenttypes.egg-info/namespace_packages.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2023-05-22 17:57:28.000000 plone.app.contenttypes-3.0.3/plone.app.contenttypes.egg-info/not-zip-safe
+-rw-r--r--   0 maurits    (501) staff       (20)      827 2023-05-22 17:57:28.000000 plone.app.contenttypes-3.0.3/plone.app.contenttypes.egg-info/requires.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        6 2023-05-22 17:57:28.000000 plone.app.contenttypes-3.0.3/plone.app.contenttypes.egg-info/top_level.txt
+-rw-r--r--   0 maurits    (501) staff       (20)     1707 2023-05-22 17:57:27.000000 plone.app.contenttypes-3.0.3/pyproject.toml
+-rw-r--r--   0 maurits    (501) staff       (20)      217 2023-05-22 17:57:28.324685 plone.app.contenttypes-3.0.3/setup.cfg
+-rw-r--r--   0 maurits    (501) staff       (20)     3130 2023-05-22 17:57:27.000000 plone.app.contenttypes-3.0.3/setup.py
```

### Comparing `plone.app.contenttypes-3.0.2/CHANGES.rst` & `plone.app.contenttypes-3.0.3/CHANGES.rst`

 * *Files 0% similar despite different names*

```diff
@@ -4,14 +4,25 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+3.0.3 (2023-05-22)
+------------------
+
+Bug fixes:
+
+
+- extends the the calculation of url if resolveuid part of link in LinkRedirectView @1letter (#626)
+- Remove the unused dependency plone.app.event
+  [@folix-01] (#663)
+
+
 3.0.2 (2023-04-14)
 ------------------
 
 Bug fixes:
 
 
 - Fix test_behaviors_table_of_contents: ordering of attrtributes changed.
```

### Comparing `plone.app.contenttypes-3.0.2/PKG-INFO` & `plone.app.contenttypes-3.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plone.app.contenttypes
-Version: 3.0.2
+Version: 3.0.3
 Summary: Default content types for Plone based on Dexterity
 Home-page: https://github.com/plone/plone.app.contenttypes
 Author: Plone Foundation
 Author-email: plone-developers@lists.sourceforge.net
 License: GPL
 Keywords: plone content types dexterity
 Classifier: Development Status :: 5 - Production/Stable
@@ -218,14 +218,25 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+3.0.3 (2023-05-22)
+------------------
+
+Bug fixes:
+
+
+- extends the the calculation of url if resolveuid part of link in LinkRedirectView @1letter (#626)
+- Remove the unused dependency plone.app.event
+  [@folix-01] (#663)
+
+
 3.0.2 (2023-04-14)
 ------------------
 
 Bug fixes:
 
 
 - Fix test_behaviors_table_of_contents: ordering of attrtributes changed.
```

### Comparing `plone.app.contenttypes-3.0.2/README.rst` & `plone.app.contenttypes-3.0.3/README.rst`

 * *Files identical despite different names*

### Comparing `plone.app.contenttypes-3.0.2/docs/INSTALL.txt` & `plone.app.contenttypes-3.0.3/docs/INSTALL.txt`

 * *Files identical despite different names*

### Comparing `plone.app.contenttypes-3.0.2/docs/LICENSE.GPL` & `plone.app.contenttypes-3.0.3/docs/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `plone.app.contenttypes-3.0.2/docs/LICENSE.txt` & `plone.app.contenttypes-3.0.3/docs/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `plone.app.contenttypes-3.0.2/docs/README.rst` & `plone.app.contenttypes-3.0.3/docs/README.rst`

 * *Files identical despite different names*

### Comparing `plone.app.contenttypes-3.0.2/docs/source/conf.py` & `plone.app.contenttypes-3.0.3/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `plone.app.contenttypes-3.0.2/plone/app/contenttypes/behaviors/collection.py` & `plone.app.contenttypes-3.0.3/plone/app/contenttypes/behaviors/collection.py`

 * *Files identical despite different names*

### Comparing `plone.app.contenttypes-3.0.2/plone/app/contenttypes/behaviors/configure.zcml` & `plone.app.contenttypes-3.0.3/plone/app/contenttypes/behaviors/configure.zcml`

 * *Files identical despite different names*

### Comparing `plone.app.contenttypes-3.0.2/plone/app/contenttypes/behaviors/leadimage.pt` & `plone.app.contenttypes-3.0.3/plone/app/contenttypes/behaviors/leadimage.pt`

 * *Files identical despite different names*

### Comparing `plone.app.contenttypes-3.0.2/plone/app/contenttypes/behaviors/leadimage.py` & `plone.app.contenttypes-3.0.3/plone/app/contenttypes/behaviors/leadimage.py`

 * *Files identical despite different names*

### Comparing `plone.app.contenttypes-3.0.2/plone/app/contenttypes/behaviors/richtext.py` & `plone.app.contenttypes-3.0.3/plone/app/contenttypes/behaviors/richtext.py`

 * *Files identical despite different names*

### Comparing `plone.app.contenttypes-3.0.2/plone/app/contenttypes/behaviors/tableofcontents.py` & `plone.app.contenttypes-3.0.3/plone/app/contenttypes/behaviors/tableofcontents.py`

 * *Files identical despite different names*

### Comparing `plone.app.contenttypes-3.0.2/plone/app/contenttypes/behaviors/thumb_icon.py` & `plone.app.contenttypes-3.0.3/plone/app/contenttypes/behaviors/thumb_icon.py`

 * *Files identical despite different names*

### Comparing `plone.app.contenttypes-3.0.2/plone/app/contenttypes/browser/collection.py` & `plone.app.contenttypes-3.0.3/plone/app/contenttypes/browser/collection.py`

 * *Files identical despite different names*

### Comparing `plone.app.contenttypes-3.0.2/plone/app/contenttypes/browser/configure.zcml` & `plone.app.contenttypes-3.0.3/plone/app/contenttypes/browser/configure.zcml`

 * *Files identical despite different names*

### Comparing `plone.app.contenttypes-3.0.2/plone/app/contenttypes/browser/file.py` & `plone.app.contenttypes-3.0.3/plone/app/contenttypes/browser/file.py`

 * *Files identical despite different names*

### Comparing `plone.app.contenttypes-3.0.2/plone/app/contenttypes/browser/folder.py` & `plone.app.contenttypes-3.0.3/plone/app/contenttypes/browser/folder.py`

 * *Files identical despite different names*

### Comparing `plone.app.contenttypes-3.0.2/plone/app/contenttypes/browser/full_view.py` & `plone.app.contenttypes-3.0.3/plone/app/contenttypes/browser/full_view.py`

 * *Files identical despite different names*

### Comparing `plone.app.contenttypes-3.0.2/plone/app/contenttypes/browser/link_redirect_view.py` & `plone.app.contenttypes-3.0.3/plone/app/contenttypes/browser/link_redirect_view.py`

 * *Files 9% similar despite different names*

```diff
@@ -104,11 +104,18 @@
         if url.startswith("."):
             # we just need to adapt ../relative/links, /absolute/ones work
             # anyway -> this requires relative links to start with ./ or
             # ../
             context_state = self.context.restrictedTraverse("@@plone_context_state")
             url = "/".join([context_state.canonical_object_url(), url])
         else:
+            if "resolveuid" in url:
+                uid = url.split("/")[-1]
+                obj = uuidToObject(uid)
+                if obj:
+                    url = "/".join(obj.getPhysicalPath()[2:])
+                    if not url.startswith("/"):
+                        url = "/" + url
             if not url.startswith(("http://", "https://")):
                 url = self.request["SERVER_URL"] + url
 
         return url
```

### Comparing `plone.app.contenttypes-3.0.2/plone/app/contenttypes/browser/migration.py` & `plone.app.contenttypes-3.0.3/plone/app/contenttypes/browser/migration.py`

 * *Files identical despite different names*

### Comparing `plone.app.contenttypes-3.0.2/plone/app/contenttypes/browser/templates/document.pt` & `plone.app.contenttypes-3.0.3/plone/app/contenttypes/browser/templates/document.pt`

 * *Files identical despite different names*

### Comparing `plone.app.contenttypes-3.0.2/plone/app/contenttypes/browser/templates/file.pt` & `plone.app.contenttypes-3.0.3/plone/app/contenttypes/browser/templates/file.pt`

 * *Files identical despite different names*

### Comparing `plone.app.contenttypes-3.0.2/plone/app/contenttypes/browser/templates/full_view.pt` & `plone.app.contenttypes-3.0.3/plone/app/contenttypes/browser/templates/full_view.pt`

 * *Files identical despite different names*

### Comparing `plone.app.contenttypes-3.0.2/plone/app/contenttypes/browser/templates/full_view_item.pt` & `plone.app.contenttypes-3.0.3/plone/app/contenttypes/browser/templates/full_view_item.pt`

 * *Files identical despite different names*

### Comparing `plone.app.contenttypes-3.0.2/plone/app/contenttypes/browser/templates/image.pt` & `plone.app.contenttypes-3.0.3/plone/app/contenttypes/browser/templates/image.pt`

 * *Files identical despite different names*

### Comparing `plone.app.contenttypes-3.0.2/plone/app/contenttypes/browser/templates/image_view_fullscreen.pt` & `plone.app.contenttypes-3.0.3/plone/app/contenttypes/browser/templates/image_view_fullscreen.pt`

 * *Files identical despite different names*

### Comparing `plone.app.contenttypes-3.0.2/plone/app/contenttypes/browser/templates/link.pt` & `plone.app.contenttypes-3.0.3/plone/app/contenttypes/browser/templates/link.pt`

 * *Files identical despite different names*

### Comparing `plone.app.contenttypes-3.0.2/plone/app/contenttypes/browser/templates/listing.pt` & `plone.app.contenttypes-3.0.3/plone/app/contenttypes/browser/templates/listing.pt`

 * *Files identical despite different names*

### Comparing `plone.app.contenttypes-3.0.2/plone/app/contenttypes/browser/templates/listing_album.pt` & `plone.app.contenttypes-3.0.3/plone/app/contenttypes/browser/templates/listing_album.pt`

 * *Files identical despite different names*

### Comparing `plone.app.contenttypes-3.0.2/plone/app/contenttypes/browser/templates/listing_summary.pt` & `plone.app.contenttypes-3.0.3/plone/app/contenttypes/browser/templates/listing_summary.pt`

 * *Files identical despite different names*

### Comparing `plone.app.contenttypes-3.0.2/plone/app/contenttypes/browser/templates/listing_tabular.pt` & `plone.app.contenttypes-3.0.3/plone/app/contenttypes/browser/templates/listing_tabular.pt`

 * *Files identical despite different names*

### Comparing `plone.app.contenttypes-3.0.2/plone/app/contenttypes/browser/templates/newsitem.pt` & `plone.app.contenttypes-3.0.3/plone/app/contenttypes/browser/templates/newsitem.pt`

 * *Files identical despite different names*

### Comparing `plone.app.contenttypes-3.0.2/plone/app/contenttypes/browser/utils.py` & `plone.app.contenttypes-3.0.3/plone/app/contenttypes/browser/utils.py`

 * *Files identical despite different names*

### Comparing `plone.app.contenttypes-3.0.2/plone/app/contenttypes/configure.zcml` & `plone.app.contenttypes-3.0.3/plone/app/contenttypes/configure.zcml`

 * *Files 8% similar despite different names*

```diff
@@ -31,15 +31,18 @@
       />
 
   <include package="plone.behavior" />
   <include package="plone.dexterity" />
   <include package="plone.namedfile" />
   <include package="plone.app.contentmenu" />
   <include package="plone.app.dexterity" />
-  <include package="plone.app.event" />
+  <include
+      package="plone.app.event"
+      zcml:condition="installed plone.app.event"
+      />
   <include package="plone.app.linkintegrity" />
   <include package="plone.app.lockingbehavior" />
   <include package="plone.app.querystring" />
   <include package="plone.app.relationfield" />
   <include package="plone.app.versioningbehavior" />
   <include package="plone.app.vocabularies" />
   <include package="plone.app.z3cform" />
```

### Comparing `plone.app.contenttypes-3.0.2/plone/app/contenttypes/content.py` & `plone.app.contenttypes-3.0.3/plone/app/contenttypes/content.py`

 * *Files identical despite different names*

### Comparing `plone.app.contenttypes-3.0.2/plone/app/contenttypes/indexers.py` & `plone.app.contenttypes-3.0.3/plone/app/contenttypes/indexers.py`

 * *Files identical despite different names*

### Comparing `plone.app.contenttypes-3.0.2/plone/app/contenttypes/indexers.zcml` & `plone.app.contenttypes-3.0.3/plone/app/contenttypes/indexers.zcml`

 * *Files identical despite different names*

### Comparing `plone.app.contenttypes-3.0.2/plone/app/contenttypes/interfaces.py` & `plone.app.contenttypes-3.0.3/plone/app/contenttypes/interfaces.py`

 * *Files identical despite different names*

### Comparing `plone.app.contenttypes-3.0.2/plone/app/contenttypes/permissions.py` & `plone.app.contenttypes-3.0.3/plone/app/contenttypes/permissions.py`

 * *Files identical despite different names*

### Comparing `plone.app.contenttypes-3.0.2/plone/app/contenttypes/permissions.zcml` & `plone.app.contenttypes-3.0.3/plone/app/contenttypes/permissions.zcml`

 * *Files identical despite different names*

### Comparing `plone.app.contenttypes-3.0.2/plone/app/contenttypes/profiles/content/portlets.xml` & `plone.app.contenttypes-3.0.3/plone/app/contenttypes/profiles/content/portlets.xml`

 * *Files identical despite different names*

### Comparing `plone.app.contenttypes-3.0.2/plone/app/contenttypes/profiles/default/diff_tool.xml` & `plone.app.contenttypes-3.0.3/plone/app/contenttypes/profiles/default/diff_tool.xml`

 * *Files identical despite different names*

### Comparing `plone.app.contenttypes-3.0.2/plone/app/contenttypes/profiles/default/rolemap.xml` & `plone.app.contenttypes-3.0.3/plone/app/contenttypes/profiles/default/rolemap.xml`

 * *Files identical despite different names*

### Comparing `plone.app.contenttypes-3.0.2/plone/app/contenttypes/profiles/default/types/Collection.xml` & `plone.app.contenttypes-3.0.3/plone/app/contenttypes/profiles/default/types/Collection.xml`

 * *Files identical despite different names*

### Comparing `plone.app.contenttypes-3.0.2/plone/app/contenttypes/profiles/default/types/Document.xml` & `plone.app.contenttypes-3.0.3/plone/app/contenttypes/profiles/default/types/Document.xml`

 * *Files identical despite different names*

### Comparing `plone.app.contenttypes-3.0.2/plone/app/contenttypes/profiles/default/types/Event.xml` & `plone.app.contenttypes-3.0.3/plone/app/contenttypes/profiles/default/types/Event.xml`

 * *Files identical despite different names*

### Comparing `plone.app.contenttypes-3.0.2/plone/app/contenttypes/profiles/default/types/File.xml` & `plone.app.contenttypes-3.0.3/plone/app/contenttypes/profiles/default/types/File.xml`

 * *Files identical despite different names*

### Comparing `plone.app.contenttypes-3.0.2/plone/app/contenttypes/profiles/default/types/Folder.xml` & `plone.app.contenttypes-3.0.3/plone/app/contenttypes/profiles/default/types/Folder.xml`

 * *Files identical despite different names*

### Comparing `plone.app.contenttypes-3.0.2/plone/app/contenttypes/profiles/default/types/Image.xml` & `plone.app.contenttypes-3.0.3/plone/app/contenttypes/profiles/default/types/Image.xml`

 * *Files identical despite different names*

### Comparing `plone.app.contenttypes-3.0.2/plone/app/contenttypes/profiles/default/types/Link.xml` & `plone.app.contenttypes-3.0.3/plone/app/contenttypes/profiles/default/types/Link.xml`

 * *Files identical despite different names*

### Comparing `plone.app.contenttypes-3.0.2/plone/app/contenttypes/profiles/default/types/News_Item.xml` & `plone.app.contenttypes-3.0.3/plone/app/contenttypes/profiles/default/types/News_Item.xml`

 * *Files identical despite different names*

### Comparing `plone.app.contenttypes-3.0.2/plone/app/contenttypes/profiles/default/types/Plone_Site.xml` & `plone.app.contenttypes-3.0.3/plone/app/contenttypes/profiles/default/types/Plone_Site.xml`

 * *Files identical despite different names*

### Comparing `plone.app.contenttypes-3.0.2/plone/app/contenttypes/profiles/default/types.xml` & `plone.app.contenttypes-3.0.3/plone/app/contenttypes/profiles/default/types.xml`

 * *Files identical despite different names*

### Comparing `plone.app.contenttypes-3.0.2/plone/app/contenttypes/profiles.zcml` & `plone.app.contenttypes-3.0.3/plone/app/contenttypes/profiles.zcml`

 * *Files identical despite different names*

### Comparing `plone.app.contenttypes-3.0.2/plone/app/contenttypes/schema/file.xml` & `plone.app.contenttypes-3.0.3/plone/app/contenttypes/schema/file.xml`

 * *Files identical despite different names*

### Comparing `plone.app.contenttypes-3.0.2/plone/app/contenttypes/schema/image.xml` & `plone.app.contenttypes-3.0.3/plone/app/contenttypes/schema/image.xml`

 * *Files identical despite different names*

### Comparing `plone.app.contenttypes-3.0.2/plone/app/contenttypes/schema/link.xml` & `plone.app.contenttypes-3.0.3/plone/app/contenttypes/schema/link.xml`

 * *Files identical despite different names*

### Comparing `plone.app.contenttypes-3.0.2/plone/app/contenttypes/setuphandlers.py` & `plone.app.contenttypes-3.0.3/plone/app/contenttypes/setuphandlers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from AccessControl import Unauthorized
 from Acquisition import aq_base
 from Acquisition import aq_inner
 from plone.app.dexterity.behaviors import constrains
 from plone.app.textfield.value import RichTextValue
 from plone.base.interfaces import INonInstallable
 from plone.base.interfaces.constrains import ISelectableConstrainTypes
+from plone.base.utils import get_installer
 from plone.base.utils import unrestricted_construct_instance
 from plone.dexterity.fti import IDexterityFTI
 from plone.dexterity.utils import createContent
 from plone.i18n.normalizer.interfaces import IURLNormalizer
 from plone.portlets.interfaces import ILocalPortletAssignmentManager
 from plone.portlets.interfaces import IPortletManager
 from plone.registry.interfaces import IRegistry
@@ -20,14 +21,23 @@
 from zope.component.hooks import getSite
 from zope.container.interfaces import INameChooser
 from zope.i18n.interfaces import ITranslationDomain
 from zope.i18n.locales import locales
 from zope.i18n.locales.provider import LoadLocaleError
 from zope.interface import implementer
 
+import pkg_resources
+
+
+try:
+    pkg_resources.get_distribution("plone.app.event")
+    HAS_EVENT = True
+except pkg_resources.DistributionNotFound:
+    HAS_EVENT = False
+
 
 @implementer(INonInstallable)
 class HiddenProfiles:
     def getNonInstallableProfiles(self):
         """
         Prevents all profiles but 'plone-content' from showing up in the
         profile list when creating a Plone site.
@@ -336,16 +346,24 @@
 
 def import_content(context):
     """Create default content."""
     portal = getSite()
     target_language, is_combined_language, locale = _get_locales_info(portal)
     create_frontpage(portal, target_language)
     create_news_topic(portal, target_language)
-    create_events_topic(portal, target_language)
+
+    if HAS_EVENT:
+        create_events_topic(portal, target_language)
+
     configure_members_folder(portal, target_language)
 
 
 def setup_various(context):
     portal = getSite()
     target_language, is_combined_language, locale = _get_locales_info(portal)
     _setup_calendar(portal, locale)
     _setup_visible_ids(portal, target_language, locale)
+
+    # install explicitly the plone.app.event
+    if HAS_EVENT:
+        installer = get_installer(portal)
+        installer.install_product("plone.app.event")
```

### Comparing `plone.app.contenttypes-3.0.2/plone/app/contenttypes/subscribers.py` & `plone.app.contenttypes-3.0.3/plone/app/contenttypes/subscribers.py`

 * *Files identical despite different names*

### Comparing `plone.app.contenttypes-3.0.2/plone/app/contenttypes/testing.py` & `plone.app.contenttypes-3.0.3/plone/app/contenttypes/testing.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from plone.app.contenttypes.interfaces import IPloneAppContenttypesLayer
 from plone.app.contenttypes.tests.robot.variables import TEST_FOLDER_ID
-from plone.app.event.testing import PAEvent_FIXTURE
 from plone.app.robotframework.testing import REMOTE_LIBRARY_BUNDLE_FIXTURE
 from plone.app.testing import FunctionalTesting
 from plone.app.testing import IntegrationTesting
 from plone.app.testing import login
 from plone.app.testing import PLONE_FIXTURE
 from plone.app.testing import PloneSandboxLayer
 from plone.app.testing import SITE_OWNER_NAME
@@ -19,35 +18,29 @@
     We have to set the browserlayer manually, since importing the profile alone
     doesn't do it in tests.
     """
     alsoProvides(request, IPloneAppContenttypesLayer)
 
 
 class PloneAppContenttypes(PloneSandboxLayer):
-    defaultBases = (
-        PAEvent_FIXTURE,
-        PLONE_FIXTURE,
-    )
+    defaultBases = (PLONE_FIXTURE,)
 
     def setUpZope(self, app, configurationContext):
         import plone.app.contenttypes
 
         self.loadZCML(package=plone.app.contenttypes)
-        import plone.app.event.dx
-
-        self.loadZCML(package=plone.app.event.dx)
 
     def setUpPloneSite(self, portal):
         portal.portal_workflow.setDefaultChain("simple_publication_workflow")
 
 
 class PloneAppContenttypesRobot(PloneAppContenttypes):
     """Same as the default but with a added folder 'robot-test-folder'."""
 
-    defaultBases = (PAEvent_FIXTURE, REMOTE_LIBRARY_BUNDLE_FIXTURE)
+    defaultBases = (REMOTE_LIBRARY_BUNDLE_FIXTURE,)
 
     def setUpPloneSite(self, portal):
         portal.acl_users.userFolderAddUser(
             SITE_OWNER_NAME, SITE_OWNER_PASSWORD, ["Manager"], []
         )
         login(portal, SITE_OWNER_NAME)
         super().setUpPloneSite(portal)
```

### Comparing `plone.app.contenttypes-3.0.2/plone/app/contenttypes/tests/file.doc` & `plone.app.contenttypes-3.0.3/plone/app/contenttypes/tests/file.doc`

 * *Files identical despite different names*

### Comparing `plone.app.contenttypes-3.0.2/plone/app/contenttypes/tests/file.odt` & `plone.app.contenttypes-3.0.3/plone/app/contenttypes/tests/file.odt`

 * *Files identical despite different names*

### Comparing `plone.app.contenttypes-3.0.2/plone/app/contenttypes/tests/file.pdf` & `plone.app.contenttypes-3.0.3/plone/app/contenttypes/tests/file.pdf`

 * *Files identical despite different names*

### Comparing `plone.app.contenttypes-3.0.2/plone/app/contenttypes/tests/image.jpg` & `plone.app.contenttypes-3.0.3/plone/app/contenttypes/tests/image.jpg`

 * *Files identical despite different names*

### Comparing `plone.app.contenttypes-3.0.2/plone/app/contenttypes/tests/image.png` & `plone.app.contenttypes-3.0.3/plone/app/contenttypes/tests/image.png`

 * *Files identical despite different names*

### Comparing `plone.app.contenttypes-3.0.2/plone/app/contenttypes/tests/image.svg` & `plone.app.contenttypes-3.0.3/plone/app/contenttypes/tests/image.svg`

 * *Files identical despite different names*

### Comparing `plone.app.contenttypes-3.0.2/plone/app/contenttypes/tests/oldtypes.py` & `plone.app.contenttypes-3.0.3/plone/app/contenttypes/tests/oldtypes.py`

 * *Files identical despite different names*

### Comparing `plone.app.contenttypes-3.0.2/plone/app/contenttypes/tests/robot/keywords.txt` & `plone.app.contenttypes-3.0.3/plone/app/contenttypes/tests/robot/keywords.txt`

 * *Files identical despite different names*

### Comparing `plone.app.contenttypes-3.0.2/plone/app/contenttypes/tests/robot/test_collection_creator_criterion.robot` & `plone.app.contenttypes-3.0.3/plone/app/contenttypes/tests/robot/test_collection_creator_criterion.robot`

 * *Files identical despite different names*

### Comparing `plone.app.contenttypes-3.0.2/plone/app/contenttypes/tests/robot/test_collection_location_criterion.robot` & `plone.app.contenttypes-3.0.3/plone/app/contenttypes/tests/robot/test_collection_location_criterion.robot`

 * *Files identical despite different names*

### Comparing `plone.app.contenttypes-3.0.2/plone/app/contenttypes/tests/robot/test_collection_review_state_criterion.robot` & `plone.app.contenttypes-3.0.3/plone/app/contenttypes/tests/robot/test_collection_review_state_criterion.robot`

 * *Files identical despite different names*

### Comparing `plone.app.contenttypes-3.0.2/plone/app/contenttypes/tests/robot/test_collection_short_name_criterion.robot` & `plone.app.contenttypes-3.0.3/plone/app/contenttypes/tests/robot/test_collection_short_name_criterion.robot`

 * *Files identical despite different names*

### Comparing `plone.app.contenttypes-3.0.2/plone/app/contenttypes/tests/robot/test_collection_type_criterion.robot` & `plone.app.contenttypes-3.0.3/plone/app/contenttypes/tests/robot/test_collection_type_criterion.robot`

 * *Files identical despite different names*

### Comparing `plone.app.contenttypes-3.0.2/plone/app/contenttypes/tests/robot/test_folderlisting.robot` & `plone.app.contenttypes-3.0.3/plone/app/contenttypes/tests/robot/test_folderlisting.robot`

 * *Files identical despite different names*

### Comparing `plone.app.contenttypes-3.0.2/plone/app/contenttypes/tests/test_behaviors_collection.py` & `plone.app.contenttypes-3.0.3/plone/app/contenttypes/tests/test_behaviors_collection.py`

 * *Files identical despite different names*

### Comparing `plone.app.contenttypes-3.0.2/plone/app/contenttypes/tests/test_behaviors_leadimage.py` & `plone.app.contenttypes-3.0.3/plone/app/contenttypes/tests/test_behaviors_leadimage.py`

 * *Files identical despite different names*

### Comparing `plone.app.contenttypes-3.0.2/plone/app/contenttypes/tests/test_behaviors_richtext.py` & `plone.app.contenttypes-3.0.3/plone/app/contenttypes/tests/test_behaviors_richtext.py`

 * *Files identical despite different names*

### Comparing `plone.app.contenttypes-3.0.2/plone/app/contenttypes/tests/test_behaviors_table_of_contents.py` & `plone.app.contenttypes-3.0.3/plone/app/contenttypes/tests/test_behaviors_table_of_contents.py`

 * *Files identical despite different names*

### Comparing `plone.app.contenttypes-3.0.2/plone/app/contenttypes/tests/test_browser_utils.py` & `plone.app.contenttypes-3.0.3/plone/app/contenttypes/tests/test_browser_utils.py`

 * *Files identical despite different names*

### Comparing `plone.app.contenttypes-3.0.2/plone/app/contenttypes/tests/test_collection.py` & `plone.app.contenttypes-3.0.3/plone/app/contenttypes/tests/test_collection.py`

 * *Files identical despite different names*

### Comparing `plone.app.contenttypes-3.0.2/plone/app/contenttypes/tests/test_collection_rss.py` & `plone.app.contenttypes-3.0.3/plone/app/contenttypes/tests/test_collection_rss.py`

 * *Files identical despite different names*

### Comparing `plone.app.contenttypes-3.0.2/plone/app/contenttypes/tests/test_content_profile.py` & `plone.app.contenttypes-3.0.3/plone/app/contenttypes/tests/test_content_profile.py`

 * *Files identical despite different names*

### Comparing `plone.app.contenttypes-3.0.2/plone/app/contenttypes/tests/test_document.py` & `plone.app.contenttypes-3.0.3/plone/app/contenttypes/tests/test_document.py`

 * *Files identical despite different names*

### Comparing `plone.app.contenttypes-3.0.2/plone/app/contenttypes/tests/test_event.py` & `plone.app.contenttypes-3.0.3/plone/app/contenttypes/tests/test_event.py`

 * *Files identical despite different names*

### Comparing `plone.app.contenttypes-3.0.2/plone/app/contenttypes/tests/test_file.py` & `plone.app.contenttypes-3.0.3/plone/app/contenttypes/tests/test_file.py`

 * *Files identical despite different names*

### Comparing `plone.app.contenttypes-3.0.2/plone/app/contenttypes/tests/test_folder.py` & `plone.app.contenttypes-3.0.3/plone/app/contenttypes/tests/test_folder.py`

 * *Files identical despite different names*

### Comparing `plone.app.contenttypes-3.0.2/plone/app/contenttypes/tests/test_image.py` & `plone.app.contenttypes-3.0.3/plone/app/contenttypes/tests/test_image.py`

 * *Files identical despite different names*

### Comparing `plone.app.contenttypes-3.0.2/plone/app/contenttypes/tests/test_indexes.py` & `plone.app.contenttypes-3.0.3/plone/app/contenttypes/tests/test_indexes.py`

 * *Files identical despite different names*

### Comparing `plone.app.contenttypes-3.0.2/plone/app/contenttypes/tests/test_link.py` & `plone.app.contenttypes-3.0.3/plone/app/contenttypes/tests/test_link.py`

 * *Files 7% similar despite different names*

```diff
@@ -361,7 +361,18 @@
         self.link.remoteUrl = "${portal_url}"
         self.assertEqual(view.url(), "/plone")
         self.assertEqual(view.absolute_target_url(), "http://nohost/plone")
 
         self.link.remoteUrl = "${navigation_root_url}"
         self.assertEqual(view.url(), "/plone")
         self.assertEqual(view.absolute_target_url(), "http://nohost/plone")
+
+    def test_resolve_uid_to_absolute_target(self):
+        view = getMultiAdapter((self.link, self.request), name="link_redirect_view")
+
+        self.portal.invokeFactory(
+            "Document", "doc1", title="A document", description="This is a document."
+        )
+        doc1 = self.portal["doc1"]
+        uid = IUUID(doc1)
+        self.link.remoteUrl = f"${{portal_url}}/resolveuid/{uid}"
+        self.assertEqual(view.absolute_target_url(), "http://nohost/doc1")
```

### Comparing `plone.app.contenttypes-3.0.2/plone/app/contenttypes/tests/test_news_item.py` & `plone.app.contenttypes-3.0.3/plone/app/contenttypes/tests/test_news_item.py`

 * *Files identical despite different names*

### Comparing `plone.app.contenttypes-3.0.2/plone/app/contenttypes/tests/test_robot.py` & `plone.app.contenttypes-3.0.3/plone/app/contenttypes/tests/test_robot.py`

 * *Files identical despite different names*

### Comparing `plone.app.contenttypes-3.0.2/plone/app/contenttypes/tests/test_security.py` & `plone.app.contenttypes-3.0.3/plone/app/contenttypes/tests/test_security.py`

 * *Files identical despite different names*

### Comparing `plone.app.contenttypes-3.0.2/plone/app/contenttypes/tests/test_setup.py` & `plone.app.contenttypes-3.0.3/plone/app/contenttypes/tests/test_setup.py`

 * *Files identical despite different names*

### Comparing `plone.app.contenttypes-3.0.2/plone/app/contenttypes/tests/test_webdav.py` & `plone.app.contenttypes-3.0.3/plone/app/contenttypes/tests/test_webdav.py`

 * *Files identical despite different names*

### Comparing `plone.app.contenttypes-3.0.2/plone/app/contenttypes/upgrades.py` & `plone.app.contenttypes-3.0.3/plone/app/contenttypes/upgrades.py`

 * *Files identical despite different names*

### Comparing `plone.app.contenttypes-3.0.2/plone/app/contenttypes/utils.py` & `plone.app.contenttypes-3.0.3/plone/app/contenttypes/utils.py`

 * *Files identical despite different names*

### Comparing `plone.app.contenttypes-3.0.2/plone.app.contenttypes.egg-info/PKG-INFO` & `plone.app.contenttypes-3.0.3/plone.app.contenttypes.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plone.app.contenttypes
-Version: 3.0.2
+Version: 3.0.3
 Summary: Default content types for Plone based on Dexterity
 Home-page: https://github.com/plone/plone.app.contenttypes
 Author: Plone Foundation
 Author-email: plone-developers@lists.sourceforge.net
 License: GPL
 Keywords: plone content types dexterity
 Classifier: Development Status :: 5 - Production/Stable
@@ -218,14 +218,25 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+3.0.3 (2023-05-22)
+------------------
+
+Bug fixes:
+
+
+- extends the the calculation of url if resolveuid part of link in LinkRedirectView @1letter (#626)
+- Remove the unused dependency plone.app.event
+  [@folix-01] (#663)
+
+
 3.0.2 (2023-04-14)
 ------------------
 
 Bug fixes:
 
 
 - Fix test_behaviors_table_of_contents: ordering of attrtributes changed.
```

### Comparing `plone.app.contenttypes-3.0.2/plone.app.contenttypes.egg-info/SOURCES.txt` & `plone.app.contenttypes-3.0.3/plone.app.contenttypes.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `plone.app.contenttypes-3.0.2/plone.app.contenttypes.egg-info/requires.txt` & `plone.app.contenttypes-3.0.3/plone.app.contenttypes.egg-info/requires.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 setuptools
 plone.app.contentmenu
-plone.app.event>=2.0
 plone.app.dexterity>=2.0.7
 plone.app.linkintegrity
 plone.app.querystring>=1.2.2
 plone.dexterity>=2.2.1
 plone.app.relationfield
 plone.namedfile>=4.2.0
 plone.app.versioningbehavior
```

### Comparing `plone.app.contenttypes-3.0.2/pyproject.toml` & `plone.app.contenttypes-3.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `plone.app.contenttypes-3.0.2/setup.py` & `plone.app.contenttypes-3.0.3/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import find_packages
 from setuptools import setup
 
 import os
 
 
-version = "3.0.2"
+version = "3.0.3"
 
 
 def read(*rnames):
     return open(os.path.join(os.path.dirname(__file__), *rnames)).read()
 
 
 long_description = read("README.rst") + "\n\n" + read("CHANGES.rst")
@@ -44,15 +44,14 @@
     namespace_packages=["plone", "plone.app"],
     include_package_data=True,
     zip_safe=False,
     python_requires=">=3.8",
     install_requires=[
         "setuptools",
         "plone.app.contentmenu",
-        "plone.app.event >= 2.0",
         "plone.app.dexterity >= 2.0.7",  # has a fix for INameFromFilename
         "plone.app.linkintegrity",
         "plone.app.querystring >= 1.2.2",  # custom_query support
         "plone.dexterity >= 2.2.1",  # behaviors can provide primaryfields
         "plone.app.relationfield",
         "plone.namedfile >= 4.2.0",
         "plone.app.versioningbehavior",
```

