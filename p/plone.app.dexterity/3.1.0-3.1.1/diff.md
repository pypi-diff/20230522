# Comparing `tmp/plone.app.dexterity-3.1.0.tar.gz` & `tmp/plone.app.dexterity-3.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plone.app.dexterity-3.1.0.tar", last modified: Mon May  8 19:40:13 2023, max compression
+gzip compressed data, was "plone.app.dexterity-3.1.1.tar", last modified: Mon May 22 17:52:45 2023, max compression
```

## Comparing `plone.app.dexterity-3.1.0.tar` & `plone.app.dexterity-3.1.1.tar`

### file list

```diff
@@ -1,197 +1,196 @@
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-08 19:40:13.121605 plone.app.dexterity-3.1.0/
--rw-r--r--   0 maurits    (501) staff       (20)    32191 2023-05-08 19:40:11.000000 plone.app.dexterity-3.1.0/CHANGES.rst
--rw-r--r--   0 maurits    (501) staff       (20)       70 2023-05-08 19:40:11.000000 plone.app.dexterity-3.1.0/CONTRIBUTING.rst
--rw-r--r--   0 maurits    (501) staff       (20)      149 2023-05-08 19:40:11.000000 plone.app.dexterity-3.1.0/MANIFEST.in
--rw-r--r--   0 maurits    (501) staff       (20)    44513 2023-05-08 19:40:13.121822 plone.app.dexterity-3.1.0/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)     6519 2023-05-08 19:40:11.000000 plone.app.dexterity-3.1.0/README.rst
--rw-r--r--   0 maurits    (501) staff       (20)     4640 2023-05-08 19:40:11.000000 plone.app.dexterity-3.1.0/RELEASE_NOTES.rst
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-08 19:40:13.057749 plone.app.dexterity-3.1.0/docs/
--rw-r--r--   0 maurits    (501) staff       (20)    12282 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/docs/LICENSE.GPL
--rw-r--r--   0 maurits    (501) staff       (20)      760 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/docs/LICENSE.txt
--rw-r--r--   0 maurits    (501) staff       (20)     3310 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/docs/Makefile
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-08 19:40:13.064704 plone.app.dexterity-3.1.0/docs/advanced/
--rw-r--r--   0 maurits    (501) staff       (20)     1951 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/docs/advanced/behaviours.rst
--rw-r--r--   0 maurits    (501) staff       (20)    14910 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/docs/advanced/catalog-indexing-strategies.rst
--rw-r--r--   0 maurits    (501) staff       (20)     9635 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/docs/advanced/custom-add-and-edit-forms.rst
--rw-r--r--   0 maurits    (501) staff       (20)     3181 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/docs/advanced/custom-content-classes.rst
--rw-r--r--   0 maurits    (501) staff       (20)     2145 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/docs/advanced/defaults.rst
--rw-r--r--   0 maurits    (501) staff       (20)     5191 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/docs/advanced/event-handlers.rst
--rw-r--r--   0 maurits    (501) staff       (20)     4599 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/docs/advanced/files-and-images.rst
--rw-r--r--   0 maurits    (501) staff       (20)      492 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/docs/advanced/index.rst
--rw-r--r--   0 maurits    (501) staff       (20)     6971 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/docs/advanced/permissions.rst
--rw-r--r--   0 maurits    (501) staff       (20)     7156 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/docs/advanced/references.rst
--rw-r--r--   0 maurits    (501) staff       (20)     7451 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/docs/advanced/rich-text-markup-transformations.rst
--rw-r--r--   0 maurits    (501) staff       (20)     5276 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/docs/advanced/static-resources.rst
--rw-r--r--   0 maurits    (501) staff       (20)     3814 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/docs/advanced/validators.rst
--rw-r--r--   0 maurits    (501) staff       (20)    13226 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/docs/advanced/vocabularies.rst
--rw-r--r--   0 maurits    (501) staff       (20)    21829 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/docs/advanced/webdav-and-other-file-representations.rst
--rw-r--r--   0 maurits    (501) staff       (20)    16315 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/docs/advanced/workflow.rst
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-08 19:40:13.067620 plone.app.dexterity-3.1.0/docs/behaviors/
--rw-r--r--   0 maurits    (501) staff       (20)     1931 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/docs/behaviors/behavior-basics.rst
--rw-r--r--   0 maurits    (501) staff       (20)     5438 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/docs/behaviors/creating-and-registering-behaviors.rst
--rw-r--r--   0 maurits    (501) staff       (20)      278 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/docs/behaviors/index.rst
--rw-r--r--   0 maurits    (501) staff       (20)     2083 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/docs/behaviors/intro.rst
--rw-r--r--   0 maurits    (501) staff       (20)    10191 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/docs/behaviors/providing-marker-interfaces.rst
--rw-r--r--   0 maurits    (501) staff       (20)     5855 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/docs/behaviors/schema-only-behaviors.rst
--rw-r--r--   0 maurits    (501) staff       (20)    11007 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/docs/behaviors/testing-behaviors.rst
--rw-r--r--   0 maurits    (501) staff       (20)     7095 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/docs/conf.py
--rw-r--r--   0 maurits    (501) staff       (20)    10739 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/docs/custom-views.rst
--rw-r--r--   0 maurits    (501) staff       (20)     2354 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/docs/designing.rst
--rw-r--r--   0 maurits    (501) staff       (20)      460 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/docs/index.rst
--rw-r--r--   0 maurits    (501) staff       (20)      943 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/docs/install.rst
--rw-r--r--   0 maurits    (501) staff       (20)     5693 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/docs/intro.rst
--rw-r--r--   0 maurits    (501) staff       (20)     3973 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/docs/model-driven-types.rst
--rw-r--r--   0 maurits    (501) staff       (20)     6303 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/docs/prerequisite.rst
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-08 19:40:13.071017 plone.app.dexterity-3.1.0/docs/reference/
--rw-r--r--   0 maurits    (501) staff       (20)     9806 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/docs/reference/dexterity-xml.rst
--rw-r--r--   0 maurits    (501) staff       (20)    14982 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/docs/reference/fields.rst
--rw-r--r--   0 maurits    (501) staff       (20)     8261 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/docs/reference/form-schema-hints.rst
--rw-r--r--   0 maurits    (501) staff       (20)      270 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/docs/reference/index.rst
--rw-r--r--   0 maurits    (501) staff       (20)    35076 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/docs/reference/manipulating-content-objects.rst
--rw-r--r--   0 maurits    (501) staff       (20)      871 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/docs/reference/misc.rst
--rw-r--r--   0 maurits    (501) staff       (20)     6133 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/docs/reference/standard-behaviours.rst
--rw-r--r--   0 maurits    (501) staff       (20)     3419 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/docs/reference/widgets.rst
--rw-r--r--   0 maurits    (501) staff       (20)    16977 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/docs/schema-driven-types.rst
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-08 19:40:13.072674 plone.app.dexterity-3.1.0/docs/testing/
--rw-r--r--   0 maurits    (501) staff       (20)      186 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/docs/testing/index.rst
--rw-r--r--   0 maurits    (501) staff       (20)    14392 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/docs/testing/integration-tests.rst
--rw-r--r--   0 maurits    (501) staff       (20)    10941 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/docs/testing/mock-testing.rst
--rw-r--r--   0 maurits    (501) staff       (20)     5860 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/docs/testing/unit-tests.rst
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-08 19:40:13.073091 plone.app.dexterity-3.1.0/plone/
--rw-r--r--   0 maurits    (501) staff       (20)       56 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/plone/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-08 19:40:13.076912 plone.app.dexterity-3.1.0/plone/app/
--rw-r--r--   0 maurits    (501) staff       (20)       56 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/plone/app/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-08 19:40:13.081401 plone.app.dexterity-3.1.0/plone/app/dexterity/
--rw-r--r--   0 maurits    (501) staff       (20)      672 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/plone/app/dexterity/TODO.txt
--rw-r--r--   0 maurits    (501) staff       (20)       76 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/plone/app/dexterity/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-08 19:40:13.085468 plone.app.dexterity-3.1.0/plone/app/dexterity/behaviors/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/plone/app/dexterity/behaviors/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     5114 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/plone/app/dexterity/behaviors/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     6908 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/plone/app/dexterity/behaviors/constrains.py
--rw-r--r--   0 maurits    (501) staff       (20)     1102 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/plone/app/dexterity/behaviors/discussion.py
--rw-r--r--   0 maurits    (501) staff       (20)     1759 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/plone/app/dexterity/behaviors/exclfromnav.py
--rw-r--r--   0 maurits    (501) staff       (20)      963 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/plone/app/dexterity/behaviors/filename.py
--rw-r--r--   0 maurits    (501) staff       (20)     1808 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/plone/app/dexterity/behaviors/id.py
--rw-r--r--   0 maurits    (501) staff       (20)    12317 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/plone/app/dexterity/behaviors/metadata.py
--rw-r--r--   0 maurits    (501) staff       (20)     4533 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/plone/app/dexterity/behaviors/nextprevious.py
--rw-r--r--   0 maurits    (501) staff       (20)      441 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/plone/app/dexterity/behaviors/related.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-08 19:40:13.087044 plone.app.dexterity-3.1.0/plone/app/dexterity/behaviors/tests/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/plone/app/dexterity/behaviors/tests/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     2827 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/plone/app/dexterity/behaviors/tests/test_contrains.py
--rw-r--r--   0 maurits    (501) staff       (20)     5128 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/plone/app/dexterity/behaviors/tests/test_id.py
--rw-r--r--   0 maurits    (501) staff       (20)     4370 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/plone/app/dexterity/behaviors/tests/test_metadata.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-08 19:40:13.097647 plone.app.dexterity-3.1.0/plone/app/dexterity/browser/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/plone/app/dexterity/browser/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     1751 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/plone/app/dexterity/browser/add_type.py
--rw-r--r--   0 maurits    (501) staff       (20)     2884 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/plone/app/dexterity/browser/behaviors.pt
--rw-r--r--   0 maurits    (501) staff       (20)     5024 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/plone/app/dexterity/browser/behaviors.py
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/plone/app/dexterity/browser/blank.css
--rw-r--r--   0 maurits    (501) staff       (20)     1223 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/plone/app/dexterity/browser/clone_type.py
--rw-r--r--   0 maurits    (501) staff       (20)     4177 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/plone/app/dexterity/browser/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     1740 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/plone/app/dexterity/browser/container.pt
--rw-r--r--   0 maurits    (501) staff       (20)      661 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/plone/app/dexterity/browser/default_page_warning.pt
--rw-r--r--   0 maurits    (501) staff       (20)     4539 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/plone/app/dexterity/browser/export.py
--rw-r--r--   0 maurits    (501) staff       (20)     1185 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/plone/app/dexterity/browser/fields.py
--rw-r--r--   0 maurits    (501) staff       (20)     6792 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/plone/app/dexterity/browser/folder_listing.pt
--rw-r--r--   0 maurits    (501) staff       (20)     3408 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/plone/app/dexterity/browser/folder_listing.py
--rw-r--r--   0 maurits    (501) staff       (20)     6391 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/plone/app/dexterity/browser/import_types.py
--rw-r--r--   0 maurits    (501) staff       (20)     1307 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/plone/app/dexterity/browser/item.pt
--rw-r--r--   0 maurits    (501) staff       (20)      429 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/plone/app/dexterity/browser/layout.py
--rw-r--r--   0 maurits    (501) staff       (20)     2493 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/plone/app/dexterity/browser/modeleditor.pt
--rw-r--r--   0 maurits    (501) staff       (20)     5644 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/plone/app/dexterity/browser/modeleditor.py
--rw-r--r--   0 maurits    (501) staff       (20)     2264 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/plone/app/dexterity/browser/overview.pt
--rw-r--r--   0 maurits    (501) staff       (20)     1177 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/plone/app/dexterity/browser/overview.py
--rw-r--r--   0 maurits    (501) staff       (20)     1297 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/plone/app/dexterity/browser/tabbed_forms.pt
--rw-r--r--   0 maurits    (501) staff       (20)    10142 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/plone/app/dexterity/browser/types.py
--rw-r--r--   0 maurits    (501) staff       (20)     1098 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/plone/app/dexterity/browser/types_listing.pt
--rw-r--r--   0 maurits    (501) staff       (20)     1350 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/plone/app/dexterity/browser/types_listing_row.pt
--rw-r--r--   0 maurits    (501) staff       (20)      710 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/plone/app/dexterity/browser/typesformwrapper.pt
--rw-r--r--   0 maurits    (501) staff       (20)      249 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/plone/app/dexterity/browser/utils.py
--rw-r--r--   0 maurits    (501) staff       (20)     2770 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/plone/app/dexterity/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)      547 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/plone/app/dexterity/events.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     2219 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/plone/app/dexterity/factories.py
--rw-r--r--   0 maurits    (501) staff       (20)     3667 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/plone/app/dexterity/interfaces.py
--rw-r--r--   0 maurits    (501) staff       (20)      482 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/plone/app/dexterity/meta.zcml
--rw-r--r--   0 maurits    (501) staff       (20)      271 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/plone/app/dexterity/overrides.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     4664 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/plone/app/dexterity/permissions.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-08 19:40:13.047597 plone.app.dexterity-3.1.0/plone/app/dexterity/profiles/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-08 19:40:13.098486 plone.app.dexterity-3.1.0/plone/app/dexterity/profiles/default/
--rw-r--r--   0 maurits    (501) staff       (20)      591 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/plone/app/dexterity/profiles/default/controlpanel.xml
--rw-r--r--   0 maurits    (501) staff       (20)      186 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/plone/app/dexterity/profiles/default/metadata.xml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-08 19:40:13.099321 plone.app.dexterity-3.1.0/plone/app/dexterity/profiles/testing/
--rw-r--r--   0 maurits    (501) staff       (20)      248 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/plone/app/dexterity/profiles/testing/metadata.xml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-08 19:40:13.100149 plone.app.dexterity-3.1.0/plone/app/dexterity/profiles/testing/types/
--rw-r--r--   0 maurits    (501) staff       (20)     2214 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/plone/app/dexterity/profiles/testing/types/Document.xml
--rw-r--r--   0 maurits    (501) staff       (20)     2467 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/plone/app/dexterity/profiles/testing/types/Folder.xml
--rw-r--r--   0 maurits    (501) staff       (20)      356 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/plone/app/dexterity/profiles/testing/types.xml
--rw-r--r--   0 maurits    (501) staff       (20)     1661 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/plone/app/dexterity/serialize.py
--rw-r--r--   0 maurits    (501) staff       (20)     1074 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/plone/app/dexterity/testing.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-08 19:40:13.106796 plone.app.dexterity-3.1.0/plone/app/dexterity/tests/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/plone/app/dexterity/tests/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     3656 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/plone/app/dexterity/tests/discussion.txt
--rw-r--r--   0 maurits    (501) staff       (20)    22722 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/plone/app/dexterity/tests/editing.rst
--rw-r--r--   0 maurits    (501) staff       (20)     1851 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/plone/app/dexterity/tests/filename.txt
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-08 19:40:13.107213 plone.app.dexterity-3.1.0/plone/app/dexterity/tests/import/
--rw-r--r--   0 maurits    (501) staff       (20)     5804 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/plone/app/dexterity/tests/import/dexterity_export.zip
--rw-r--r--   0 maurits    (501) staff       (20)     2498 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/plone/app/dexterity/tests/metadata.txt
--rw-r--r--   0 maurits    (501) staff       (20)     1777 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/plone/app/dexterity/tests/namefromtitle.txt
--rw-r--r--   0 maurits    (501) staff       (20)     3592 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/plone/app/dexterity/tests/nextprevious.txt
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-08 19:40:13.107647 plone.app.dexterity-3.1.0/plone/app/dexterity/tests/robot/
--rw-r--r--   0 maurits    (501) staff       (20)     1082 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/plone/app/dexterity/tests/robot/test_types.robot
--rw-r--r--   0 maurits    (501) staff       (20)     1458 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/plone/app/dexterity/tests/schema_events.txt
--rw-r--r--   0 maurits    (501) staff       (20)    19024 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/plone/app/dexterity/tests/test_constrains.py
--rw-r--r--   0 maurits    (501) staff       (20)      778 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/plone/app/dexterity/tests/test_doctests.py
--rw-r--r--   0 maurits    (501) staff       (20)     1857 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/plone/app/dexterity/tests/test_export.py
--rw-r--r--   0 maurits    (501) staff       (20)     2851 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/plone/app/dexterity/tests/test_import.py
--rw-r--r--   0 maurits    (501) staff       (20)     8202 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/plone/app/dexterity/tests/test_nextprevious.py
--rw-r--r--   0 maurits    (501) staff       (20)     9191 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/plone/app/dexterity/tests/test_permissions.py
--rw-r--r--   0 maurits    (501) staff       (20)      826 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/plone/app/dexterity/tests/test_robot.py
--rw-r--r--   0 maurits    (501) staff       (20)     1586 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/plone/app/dexterity/tests/test_upgrades.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-08 19:40:13.112191 plone.app.dexterity-3.1.0/plone/app/dexterity/textindexer/
--rw-r--r--   0 maurits    (501) staff       (20)      555 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/plone/app/dexterity/textindexer/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)      293 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/plone/app/dexterity/textindexer/behavior.py
--rw-r--r--   0 maurits    (501) staff       (20)     2066 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/plone/app/dexterity/textindexer/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     5051 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/plone/app/dexterity/textindexer/converters.py
--rw-r--r--   0 maurits    (501) staff       (20)      890 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/plone/app/dexterity/textindexer/directives.py
--rw-r--r--   0 maurits    (501) staff       (20)     5290 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/plone/app/dexterity/textindexer/indexer.py
--rw-r--r--   0 maurits    (501) staff       (20)     1046 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/plone/app/dexterity/textindexer/interfaces.py
--rw-r--r--   0 maurits    (501) staff       (20)     2339 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/plone/app/dexterity/textindexer/schemaeditor.py
--rw-r--r--   0 maurits    (501) staff       (20)     1340 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/plone/app/dexterity/textindexer/supermodel.py
--rw-r--r--   0 maurits    (501) staff       (20)     2662 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/plone/app/dexterity/textindexer/testing.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-08 19:40:13.117282 plone.app.dexterity-3.1.0/plone/app/dexterity/textindexer/tests/
--rw-r--r--   0 maurits    (501) staff       (20)       80 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/plone/app/dexterity/textindexer/tests/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     3249 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/plone/app/dexterity/textindexer/tests/behaviors.py
--rw-r--r--   0 maurits    (501) staff       (20)    11423 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/plone/app/dexterity/textindexer/tests/behaviors.rst
--rw-r--r--   0 maurits    (501) staff       (20)     2524 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/plone/app/dexterity/textindexer/tests/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)    21311 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/plone/app/dexterity/textindexer/tests/file.pdf
--rw-r--r--   0 maurits    (501) staff       (20)      376 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/plone/app/dexterity/textindexer/tests/helpers.py
--rw-r--r--   0 maurits    (501) staff       (20)      434 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/plone/app/dexterity/textindexer/tests/test_basic_behavior.py
--rw-r--r--   0 maurits    (501) staff       (20)      792 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/plone/app/dexterity/textindexer/tests/test_behaviors.py
--rw-r--r--   0 maurits    (501) staff       (20)     1610 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/plone/app/dexterity/textindexer/tests/test_directives.py
--rw-r--r--   0 maurits    (501) staff       (20)     3656 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/plone/app/dexterity/textindexer/tests/test_schemaeditor.py
--rw-r--r--   0 maurits    (501) staff       (20)     3767 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/plone/app/dexterity/textindexer/tests/test_supermodel_handler.py
--rw-r--r--   0 maurits    (501) staff       (20)     1793 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/plone/app/dexterity/textindexer/tests/test_utils.py
--rw-r--r--   0 maurits    (501) staff       (20)     1170 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/plone/app/dexterity/textindexer/utils.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-08 19:40:13.121271 plone.app.dexterity-3.1.0/plone/app/dexterity/upgrades/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/plone/app/dexterity/upgrades/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     2416 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/plone/app/dexterity/upgrades/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)      249 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/plone/app/dexterity/upgrades/to1.py
--rw-r--r--   0 maurits    (501) staff       (20)      195 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/plone/app/dexterity/upgrades/to2.py
--rw-r--r--   0 maurits    (501) staff       (20)      221 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/plone/app/dexterity/upgrades/to2000.py
--rw-r--r--   0 maurits    (501) staff       (20)      631 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/plone/app/dexterity/upgrades/to2001.py
--rw-r--r--   0 maurits    (501) staff       (20)      268 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/plone/app/dexterity/upgrades/to2002.py
--rw-r--r--   0 maurits    (501) staff       (20)      606 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/plone/app/dexterity/upgrades/to2003.py
--rw-r--r--   0 maurits    (501) staff       (20)      976 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/plone/app/dexterity/upgrades/to2004.py
--rw-r--r--   0 maurits    (501) staff       (20)     1444 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/plone/app/dexterity/upgrades/to2005.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-08 19:40:13.076510 plone.app.dexterity-3.1.0/plone.app.dexterity.egg-info/
--rw-r--r--   0 maurits    (501) staff       (20)    44513 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/plone.app.dexterity.egg-info/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)     6632 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/plone.app.dexterity.egg-info/SOURCES.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/plone.app.dexterity.egg-info/dependency_links.txt
--rw-r--r--   0 maurits    (501) staff       (20)       40 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/plone.app.dexterity.egg-info/entry_points.txt
--rw-r--r--   0 maurits    (501) staff       (20)       16 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/plone.app.dexterity.egg-info/namespace_packages.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/plone.app.dexterity.egg-info/not-zip-safe
--rw-r--r--   0 maurits    (501) staff       (20)      829 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/plone.app.dexterity.egg-info/requires.txt
--rw-r--r--   0 maurits    (501) staff       (20)        6 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/plone.app.dexterity.egg-info/top_level.txt
--rw-r--r--   0 maurits    (501) staff       (20)     1889 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/pyproject.toml
--rw-r--r--   0 maurits    (501) staff       (20)      287 2023-05-08 19:40:13.122584 plone.app.dexterity-3.1.0/setup.cfg
--rw-r--r--   0 maurits    (501) staff       (20)     3209 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/setup.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-22 17:52:45.308182 plone.app.dexterity-3.1.1/
+-rw-r--r--   0 maurits    (501) staff       (20)    32543 2023-05-22 17:52:44.000000 plone.app.dexterity-3.1.1/CHANGES.rst
+-rw-r--r--   0 maurits    (501) staff       (20)       70 2023-05-22 17:52:44.000000 plone.app.dexterity-3.1.1/CONTRIBUTING.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      149 2023-05-22 17:52:44.000000 plone.app.dexterity-3.1.1/MANIFEST.in
+-rw-r--r--   0 maurits    (501) staff       (20)    44865 2023-05-22 17:52:45.308413 plone.app.dexterity-3.1.1/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)     6519 2023-05-22 17:52:44.000000 plone.app.dexterity-3.1.1/README.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     4640 2023-05-22 17:52:44.000000 plone.app.dexterity-3.1.1/RELEASE_NOTES.rst
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-22 17:52:45.258844 plone.app.dexterity-3.1.1/docs/
+-rw-r--r--   0 maurits    (501) staff       (20)    12282 2023-05-22 17:52:44.000000 plone.app.dexterity-3.1.1/docs/LICENSE.GPL
+-rw-r--r--   0 maurits    (501) staff       (20)      760 2023-05-22 17:52:44.000000 plone.app.dexterity-3.1.1/docs/LICENSE.txt
+-rw-r--r--   0 maurits    (501) staff       (20)     3310 2023-05-22 17:52:44.000000 plone.app.dexterity-3.1.1/docs/Makefile
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-22 17:52:45.265276 plone.app.dexterity-3.1.1/docs/advanced/
+-rw-r--r--   0 maurits    (501) staff       (20)     1951 2023-05-22 17:52:44.000000 plone.app.dexterity-3.1.1/docs/advanced/behaviours.rst
+-rw-r--r--   0 maurits    (501) staff       (20)    14910 2023-05-22 17:52:44.000000 plone.app.dexterity-3.1.1/docs/advanced/catalog-indexing-strategies.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     9635 2023-05-22 17:52:44.000000 plone.app.dexterity-3.1.1/docs/advanced/custom-add-and-edit-forms.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     3181 2023-05-22 17:52:44.000000 plone.app.dexterity-3.1.1/docs/advanced/custom-content-classes.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     2145 2023-05-22 17:52:44.000000 plone.app.dexterity-3.1.1/docs/advanced/defaults.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     5191 2023-05-22 17:52:44.000000 plone.app.dexterity-3.1.1/docs/advanced/event-handlers.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     4599 2023-05-22 17:52:44.000000 plone.app.dexterity-3.1.1/docs/advanced/files-and-images.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      492 2023-05-22 17:52:44.000000 plone.app.dexterity-3.1.1/docs/advanced/index.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     6971 2023-05-22 17:52:44.000000 plone.app.dexterity-3.1.1/docs/advanced/permissions.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     7156 2023-05-22 17:52:44.000000 plone.app.dexterity-3.1.1/docs/advanced/references.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     7451 2023-05-22 17:52:44.000000 plone.app.dexterity-3.1.1/docs/advanced/rich-text-markup-transformations.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     5276 2023-05-22 17:52:44.000000 plone.app.dexterity-3.1.1/docs/advanced/static-resources.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     3814 2023-05-22 17:52:44.000000 plone.app.dexterity-3.1.1/docs/advanced/validators.rst
+-rw-r--r--   0 maurits    (501) staff       (20)    13226 2023-05-22 17:52:44.000000 plone.app.dexterity-3.1.1/docs/advanced/vocabularies.rst
+-rw-r--r--   0 maurits    (501) staff       (20)    21829 2023-05-22 17:52:44.000000 plone.app.dexterity-3.1.1/docs/advanced/webdav-and-other-file-representations.rst
+-rw-r--r--   0 maurits    (501) staff       (20)    16315 2023-05-22 17:52:44.000000 plone.app.dexterity-3.1.1/docs/advanced/workflow.rst
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-22 17:52:45.267847 plone.app.dexterity-3.1.1/docs/behaviors/
+-rw-r--r--   0 maurits    (501) staff       (20)     1931 2023-05-22 17:52:44.000000 plone.app.dexterity-3.1.1/docs/behaviors/behavior-basics.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     5438 2023-05-22 17:52:44.000000 plone.app.dexterity-3.1.1/docs/behaviors/creating-and-registering-behaviors.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      278 2023-05-22 17:52:44.000000 plone.app.dexterity-3.1.1/docs/behaviors/index.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     2083 2023-05-22 17:52:44.000000 plone.app.dexterity-3.1.1/docs/behaviors/intro.rst
+-rw-r--r--   0 maurits    (501) staff       (20)    10191 2023-05-22 17:52:44.000000 plone.app.dexterity-3.1.1/docs/behaviors/providing-marker-interfaces.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     5855 2023-05-22 17:52:44.000000 plone.app.dexterity-3.1.1/docs/behaviors/schema-only-behaviors.rst
+-rw-r--r--   0 maurits    (501) staff       (20)    11007 2023-05-22 17:52:44.000000 plone.app.dexterity-3.1.1/docs/behaviors/testing-behaviors.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     7095 2023-05-22 17:52:44.000000 plone.app.dexterity-3.1.1/docs/conf.py
+-rw-r--r--   0 maurits    (501) staff       (20)    10739 2023-05-22 17:52:44.000000 plone.app.dexterity-3.1.1/docs/custom-views.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     2354 2023-05-22 17:52:44.000000 plone.app.dexterity-3.1.1/docs/designing.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      460 2023-05-22 17:52:44.000000 plone.app.dexterity-3.1.1/docs/index.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      943 2023-05-22 17:52:44.000000 plone.app.dexterity-3.1.1/docs/install.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     5693 2023-05-22 17:52:44.000000 plone.app.dexterity-3.1.1/docs/intro.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     3973 2023-05-22 17:52:44.000000 plone.app.dexterity-3.1.1/docs/model-driven-types.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     6303 2023-05-22 17:52:44.000000 plone.app.dexterity-3.1.1/docs/prerequisite.rst
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-22 17:52:45.270723 plone.app.dexterity-3.1.1/docs/reference/
+-rw-r--r--   0 maurits    (501) staff       (20)     9806 2023-05-22 17:52:44.000000 plone.app.dexterity-3.1.1/docs/reference/dexterity-xml.rst
+-rw-r--r--   0 maurits    (501) staff       (20)    14982 2023-05-22 17:52:44.000000 plone.app.dexterity-3.1.1/docs/reference/fields.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     8261 2023-05-22 17:52:44.000000 plone.app.dexterity-3.1.1/docs/reference/form-schema-hints.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      270 2023-05-22 17:52:44.000000 plone.app.dexterity-3.1.1/docs/reference/index.rst
+-rw-r--r--   0 maurits    (501) staff       (20)    35076 2023-05-22 17:52:44.000000 plone.app.dexterity-3.1.1/docs/reference/manipulating-content-objects.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      871 2023-05-22 17:52:44.000000 plone.app.dexterity-3.1.1/docs/reference/misc.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     6133 2023-05-22 17:52:44.000000 plone.app.dexterity-3.1.1/docs/reference/standard-behaviours.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     3419 2023-05-22 17:52:44.000000 plone.app.dexterity-3.1.1/docs/reference/widgets.rst
+-rw-r--r--   0 maurits    (501) staff       (20)    16977 2023-05-22 17:52:44.000000 plone.app.dexterity-3.1.1/docs/schema-driven-types.rst
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-22 17:52:45.271759 plone.app.dexterity-3.1.1/docs/testing/
+-rw-r--r--   0 maurits    (501) staff       (20)      186 2023-05-22 17:52:44.000000 plone.app.dexterity-3.1.1/docs/testing/index.rst
+-rw-r--r--   0 maurits    (501) staff       (20)    14392 2023-05-22 17:52:44.000000 plone.app.dexterity-3.1.1/docs/testing/integration-tests.rst
+-rw-r--r--   0 maurits    (501) staff       (20)    10941 2023-05-22 17:52:44.000000 plone.app.dexterity-3.1.1/docs/testing/mock-testing.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     5860 2023-05-22 17:52:44.000000 plone.app.dexterity-3.1.1/docs/testing/unit-tests.rst
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-22 17:52:45.272017 plone.app.dexterity-3.1.1/plone/
+-rw-r--r--   0 maurits    (501) staff       (20)       56 2023-05-22 17:52:44.000000 plone.app.dexterity-3.1.1/plone/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-22 17:52:45.274575 plone.app.dexterity-3.1.1/plone/app/
+-rw-r--r--   0 maurits    (501) staff       (20)       56 2023-05-22 17:52:44.000000 plone.app.dexterity-3.1.1/plone/app/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-22 17:52:45.277402 plone.app.dexterity-3.1.1/plone/app/dexterity/
+-rw-r--r--   0 maurits    (501) staff       (20)      672 2023-05-22 17:52:44.000000 plone.app.dexterity-3.1.1/plone/app/dexterity/TODO.txt
+-rw-r--r--   0 maurits    (501) staff       (20)       76 2023-05-22 17:52:44.000000 plone.app.dexterity-3.1.1/plone/app/dexterity/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-22 17:52:45.280066 plone.app.dexterity-3.1.1/plone/app/dexterity/behaviors/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2023-05-22 17:52:44.000000 plone.app.dexterity-3.1.1/plone/app/dexterity/behaviors/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     5097 2023-05-22 17:52:44.000000 plone.app.dexterity-3.1.1/plone/app/dexterity/behaviors/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     6908 2023-05-22 17:52:44.000000 plone.app.dexterity-3.1.1/plone/app/dexterity/behaviors/constrains.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1102 2023-05-22 17:52:44.000000 plone.app.dexterity-3.1.1/plone/app/dexterity/behaviors/discussion.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1759 2023-05-22 17:52:44.000000 plone.app.dexterity-3.1.1/plone/app/dexterity/behaviors/exclfromnav.py
+-rw-r--r--   0 maurits    (501) staff       (20)      963 2023-05-22 17:52:44.000000 plone.app.dexterity-3.1.1/plone/app/dexterity/behaviors/filename.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1808 2023-05-22 17:52:44.000000 plone.app.dexterity-3.1.1/plone/app/dexterity/behaviors/id.py
+-rw-r--r--   0 maurits    (501) staff       (20)    12317 2023-05-22 17:52:44.000000 plone.app.dexterity-3.1.1/plone/app/dexterity/behaviors/metadata.py
+-rw-r--r--   0 maurits    (501) staff       (20)     5255 2023-05-22 17:52:44.000000 plone.app.dexterity-3.1.1/plone/app/dexterity/behaviors/nextprevious.py
+-rw-r--r--   0 maurits    (501) staff       (20)      441 2023-05-22 17:52:44.000000 plone.app.dexterity-3.1.1/plone/app/dexterity/behaviors/related.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-22 17:52:45.281318 plone.app.dexterity-3.1.1/plone/app/dexterity/behaviors/tests/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2023-05-22 17:52:44.000000 plone.app.dexterity-3.1.1/plone/app/dexterity/behaviors/tests/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2827 2023-05-22 17:52:44.000000 plone.app.dexterity-3.1.1/plone/app/dexterity/behaviors/tests/test_contrains.py
+-rw-r--r--   0 maurits    (501) staff       (20)     5128 2023-05-22 17:52:44.000000 plone.app.dexterity-3.1.1/plone/app/dexterity/behaviors/tests/test_id.py
+-rw-r--r--   0 maurits    (501) staff       (20)     4370 2023-05-22 17:52:44.000000 plone.app.dexterity-3.1.1/plone/app/dexterity/behaviors/tests/test_metadata.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-22 17:52:45.289067 plone.app.dexterity-3.1.1/plone/app/dexterity/browser/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2023-05-22 17:52:44.000000 plone.app.dexterity-3.1.1/plone/app/dexterity/browser/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1751 2023-05-22 17:52:44.000000 plone.app.dexterity-3.1.1/plone/app/dexterity/browser/add_type.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2884 2023-05-22 17:52:44.000000 plone.app.dexterity-3.1.1/plone/app/dexterity/browser/behaviors.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     5024 2023-05-22 17:52:44.000000 plone.app.dexterity-3.1.1/plone/app/dexterity/browser/behaviors.py
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2023-05-22 17:52:44.000000 plone.app.dexterity-3.1.1/plone/app/dexterity/browser/blank.css
+-rw-r--r--   0 maurits    (501) staff       (20)     1223 2023-05-22 17:52:44.000000 plone.app.dexterity-3.1.1/plone/app/dexterity/browser/clone_type.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3833 2023-05-22 17:52:44.000000 plone.app.dexterity-3.1.1/plone/app/dexterity/browser/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     1740 2023-05-22 17:52:44.000000 plone.app.dexterity-3.1.1/plone/app/dexterity/browser/container.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     4539 2023-05-22 17:52:44.000000 plone.app.dexterity-3.1.1/plone/app/dexterity/browser/export.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1185 2023-05-22 17:52:44.000000 plone.app.dexterity-3.1.1/plone/app/dexterity/browser/fields.py
+-rw-r--r--   0 maurits    (501) staff       (20)     6792 2023-05-22 17:52:44.000000 plone.app.dexterity-3.1.1/plone/app/dexterity/browser/folder_listing.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     3408 2023-05-22 17:52:44.000000 plone.app.dexterity-3.1.1/plone/app/dexterity/browser/folder_listing.py
+-rw-r--r--   0 maurits    (501) staff       (20)     6391 2023-05-22 17:52:44.000000 plone.app.dexterity-3.1.1/plone/app/dexterity/browser/import_types.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1307 2023-05-22 17:52:44.000000 plone.app.dexterity-3.1.1/plone/app/dexterity/browser/item.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      429 2023-05-22 17:52:44.000000 plone.app.dexterity-3.1.1/plone/app/dexterity/browser/layout.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2493 2023-05-22 17:52:44.000000 plone.app.dexterity-3.1.1/plone/app/dexterity/browser/modeleditor.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     5644 2023-05-22 17:52:44.000000 plone.app.dexterity-3.1.1/plone/app/dexterity/browser/modeleditor.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2264 2023-05-22 17:52:44.000000 plone.app.dexterity-3.1.1/plone/app/dexterity/browser/overview.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     1177 2023-05-22 17:52:44.000000 plone.app.dexterity-3.1.1/plone/app/dexterity/browser/overview.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1297 2023-05-22 17:52:44.000000 plone.app.dexterity-3.1.1/plone/app/dexterity/browser/tabbed_forms.pt
+-rw-r--r--   0 maurits    (501) staff       (20)    10142 2023-05-22 17:52:44.000000 plone.app.dexterity-3.1.1/plone/app/dexterity/browser/types.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1098 2023-05-22 17:52:44.000000 plone.app.dexterity-3.1.1/plone/app/dexterity/browser/types_listing.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     1350 2023-05-22 17:52:44.000000 plone.app.dexterity-3.1.1/plone/app/dexterity/browser/types_listing_row.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      710 2023-05-22 17:52:44.000000 plone.app.dexterity-3.1.1/plone/app/dexterity/browser/typesformwrapper.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      249 2023-05-22 17:52:44.000000 plone.app.dexterity-3.1.1/plone/app/dexterity/browser/utils.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2770 2023-05-22 17:52:44.000000 plone.app.dexterity-3.1.1/plone/app/dexterity/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)      547 2023-05-22 17:52:44.000000 plone.app.dexterity-3.1.1/plone/app/dexterity/events.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     2219 2023-05-22 17:52:44.000000 plone.app.dexterity-3.1.1/plone/app/dexterity/factories.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3667 2023-05-22 17:52:44.000000 plone.app.dexterity-3.1.1/plone/app/dexterity/interfaces.py
+-rw-r--r--   0 maurits    (501) staff       (20)      482 2023-05-22 17:52:44.000000 plone.app.dexterity-3.1.1/plone/app/dexterity/meta.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)      271 2023-05-22 17:52:44.000000 plone.app.dexterity-3.1.1/plone/app/dexterity/overrides.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     4664 2023-05-22 17:52:44.000000 plone.app.dexterity-3.1.1/plone/app/dexterity/permissions.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-22 17:52:45.249044 plone.app.dexterity-3.1.1/plone/app/dexterity/profiles/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-22 17:52:45.289650 plone.app.dexterity-3.1.1/plone/app/dexterity/profiles/default/
+-rw-r--r--   0 maurits    (501) staff       (20)      591 2023-05-22 17:52:44.000000 plone.app.dexterity-3.1.1/plone/app/dexterity/profiles/default/controlpanel.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      186 2023-05-22 17:52:44.000000 plone.app.dexterity-3.1.1/plone/app/dexterity/profiles/default/metadata.xml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-22 17:52:45.290403 plone.app.dexterity-3.1.1/plone/app/dexterity/profiles/testing/
+-rw-r--r--   0 maurits    (501) staff       (20)      248 2023-05-22 17:52:44.000000 plone.app.dexterity-3.1.1/plone/app/dexterity/profiles/testing/metadata.xml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-22 17:52:45.290998 plone.app.dexterity-3.1.1/plone/app/dexterity/profiles/testing/types/
+-rw-r--r--   0 maurits    (501) staff       (20)     2214 2023-05-22 17:52:44.000000 plone.app.dexterity-3.1.1/plone/app/dexterity/profiles/testing/types/Document.xml
+-rw-r--r--   0 maurits    (501) staff       (20)     2467 2023-05-22 17:52:44.000000 plone.app.dexterity-3.1.1/plone/app/dexterity/profiles/testing/types/Folder.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      356 2023-05-22 17:52:44.000000 plone.app.dexterity-3.1.1/plone/app/dexterity/profiles/testing/types.xml
+-rw-r--r--   0 maurits    (501) staff       (20)     1661 2023-05-22 17:52:44.000000 plone.app.dexterity-3.1.1/plone/app/dexterity/serialize.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1074 2023-05-22 17:52:44.000000 plone.app.dexterity-3.1.1/plone/app/dexterity/testing.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-22 17:52:45.296193 plone.app.dexterity-3.1.1/plone/app/dexterity/tests/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2023-05-22 17:52:44.000000 plone.app.dexterity-3.1.1/plone/app/dexterity/tests/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3656 2023-05-22 17:52:44.000000 plone.app.dexterity-3.1.1/plone/app/dexterity/tests/discussion.txt
+-rw-r--r--   0 maurits    (501) staff       (20)    22722 2023-05-22 17:52:44.000000 plone.app.dexterity-3.1.1/plone/app/dexterity/tests/editing.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     1851 2023-05-22 17:52:44.000000 plone.app.dexterity-3.1.1/plone/app/dexterity/tests/filename.txt
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-22 17:52:45.296446 plone.app.dexterity-3.1.1/plone/app/dexterity/tests/import/
+-rw-r--r--   0 maurits    (501) staff       (20)     5804 2023-05-22 17:52:44.000000 plone.app.dexterity-3.1.1/plone/app/dexterity/tests/import/dexterity_export.zip
+-rw-r--r--   0 maurits    (501) staff       (20)     2498 2023-05-22 17:52:44.000000 plone.app.dexterity-3.1.1/plone/app/dexterity/tests/metadata.txt
+-rw-r--r--   0 maurits    (501) staff       (20)     1777 2023-05-22 17:52:44.000000 plone.app.dexterity-3.1.1/plone/app/dexterity/tests/namefromtitle.txt
+-rw-r--r--   0 maurits    (501) staff       (20)     3592 2023-05-22 17:52:44.000000 plone.app.dexterity-3.1.1/plone/app/dexterity/tests/nextprevious.txt
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-22 17:52:45.296703 plone.app.dexterity-3.1.1/plone/app/dexterity/tests/robot/
+-rw-r--r--   0 maurits    (501) staff       (20)     1082 2023-05-22 17:52:44.000000 plone.app.dexterity-3.1.1/plone/app/dexterity/tests/robot/test_types.robot
+-rw-r--r--   0 maurits    (501) staff       (20)     1458 2023-05-22 17:52:44.000000 plone.app.dexterity-3.1.1/plone/app/dexterity/tests/schema_events.txt
+-rw-r--r--   0 maurits    (501) staff       (20)    19024 2023-05-22 17:52:44.000000 plone.app.dexterity-3.1.1/plone/app/dexterity/tests/test_constrains.py
+-rw-r--r--   0 maurits    (501) staff       (20)      778 2023-05-22 17:52:44.000000 plone.app.dexterity-3.1.1/plone/app/dexterity/tests/test_doctests.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1857 2023-05-22 17:52:44.000000 plone.app.dexterity-3.1.1/plone/app/dexterity/tests/test_export.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2851 2023-05-22 17:52:44.000000 plone.app.dexterity-3.1.1/plone/app/dexterity/tests/test_import.py
+-rw-r--r--   0 maurits    (501) staff       (20)     8186 2023-05-22 17:52:44.000000 plone.app.dexterity-3.1.1/plone/app/dexterity/tests/test_nextprevious.py
+-rw-r--r--   0 maurits    (501) staff       (20)     9191 2023-05-22 17:52:44.000000 plone.app.dexterity-3.1.1/plone/app/dexterity/tests/test_permissions.py
+-rw-r--r--   0 maurits    (501) staff       (20)      826 2023-05-22 17:52:44.000000 plone.app.dexterity-3.1.1/plone/app/dexterity/tests/test_robot.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1586 2023-05-22 17:52:44.000000 plone.app.dexterity-3.1.1/plone/app/dexterity/tests/test_upgrades.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-22 17:52:45.299897 plone.app.dexterity-3.1.1/plone/app/dexterity/textindexer/
+-rw-r--r--   0 maurits    (501) staff       (20)      555 2023-05-22 17:52:44.000000 plone.app.dexterity-3.1.1/plone/app/dexterity/textindexer/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)      293 2023-05-22 17:52:44.000000 plone.app.dexterity-3.1.1/plone/app/dexterity/textindexer/behavior.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2066 2023-05-22 17:52:44.000000 plone.app.dexterity-3.1.1/plone/app/dexterity/textindexer/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     5051 2023-05-22 17:52:44.000000 plone.app.dexterity-3.1.1/plone/app/dexterity/textindexer/converters.py
+-rw-r--r--   0 maurits    (501) staff       (20)      890 2023-05-22 17:52:44.000000 plone.app.dexterity-3.1.1/plone/app/dexterity/textindexer/directives.py
+-rw-r--r--   0 maurits    (501) staff       (20)     5290 2023-05-22 17:52:44.000000 plone.app.dexterity-3.1.1/plone/app/dexterity/textindexer/indexer.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1046 2023-05-22 17:52:44.000000 plone.app.dexterity-3.1.1/plone/app/dexterity/textindexer/interfaces.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2339 2023-05-22 17:52:44.000000 plone.app.dexterity-3.1.1/plone/app/dexterity/textindexer/schemaeditor.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1340 2023-05-22 17:52:44.000000 plone.app.dexterity-3.1.1/plone/app/dexterity/textindexer/supermodel.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2662 2023-05-22 17:52:44.000000 plone.app.dexterity-3.1.1/plone/app/dexterity/textindexer/testing.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-22 17:52:45.303802 plone.app.dexterity-3.1.1/plone/app/dexterity/textindexer/tests/
+-rw-r--r--   0 maurits    (501) staff       (20)       80 2023-05-22 17:52:44.000000 plone.app.dexterity-3.1.1/plone/app/dexterity/textindexer/tests/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3249 2023-05-22 17:52:44.000000 plone.app.dexterity-3.1.1/plone/app/dexterity/textindexer/tests/behaviors.py
+-rw-r--r--   0 maurits    (501) staff       (20)    11423 2023-05-22 17:52:44.000000 plone.app.dexterity-3.1.1/plone/app/dexterity/textindexer/tests/behaviors.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     2524 2023-05-22 17:52:44.000000 plone.app.dexterity-3.1.1/plone/app/dexterity/textindexer/tests/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)    21311 2023-05-22 17:52:44.000000 plone.app.dexterity-3.1.1/plone/app/dexterity/textindexer/tests/file.pdf
+-rw-r--r--   0 maurits    (501) staff       (20)      376 2023-05-22 17:52:44.000000 plone.app.dexterity-3.1.1/plone/app/dexterity/textindexer/tests/helpers.py
+-rw-r--r--   0 maurits    (501) staff       (20)      434 2023-05-22 17:52:44.000000 plone.app.dexterity-3.1.1/plone/app/dexterity/textindexer/tests/test_basic_behavior.py
+-rw-r--r--   0 maurits    (501) staff       (20)      792 2023-05-22 17:52:44.000000 plone.app.dexterity-3.1.1/plone/app/dexterity/textindexer/tests/test_behaviors.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1610 2023-05-22 17:52:44.000000 plone.app.dexterity-3.1.1/plone/app/dexterity/textindexer/tests/test_directives.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3656 2023-05-22 17:52:44.000000 plone.app.dexterity-3.1.1/plone/app/dexterity/textindexer/tests/test_schemaeditor.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3767 2023-05-22 17:52:44.000000 plone.app.dexterity-3.1.1/plone/app/dexterity/textindexer/tests/test_supermodel_handler.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1793 2023-05-22 17:52:44.000000 plone.app.dexterity-3.1.1/plone/app/dexterity/textindexer/tests/test_utils.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1170 2023-05-22 17:52:44.000000 plone.app.dexterity-3.1.1/plone/app/dexterity/textindexer/utils.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-22 17:52:45.307848 plone.app.dexterity-3.1.1/plone/app/dexterity/upgrades/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2023-05-22 17:52:44.000000 plone.app.dexterity-3.1.1/plone/app/dexterity/upgrades/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2416 2023-05-22 17:52:44.000000 plone.app.dexterity-3.1.1/plone/app/dexterity/upgrades/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)      249 2023-05-22 17:52:44.000000 plone.app.dexterity-3.1.1/plone/app/dexterity/upgrades/to1.py
+-rw-r--r--   0 maurits    (501) staff       (20)      195 2023-05-22 17:52:44.000000 plone.app.dexterity-3.1.1/plone/app/dexterity/upgrades/to2.py
+-rw-r--r--   0 maurits    (501) staff       (20)      221 2023-05-22 17:52:44.000000 plone.app.dexterity-3.1.1/plone/app/dexterity/upgrades/to2000.py
+-rw-r--r--   0 maurits    (501) staff       (20)      631 2023-05-22 17:52:44.000000 plone.app.dexterity-3.1.1/plone/app/dexterity/upgrades/to2001.py
+-rw-r--r--   0 maurits    (501) staff       (20)      268 2023-05-22 17:52:44.000000 plone.app.dexterity-3.1.1/plone/app/dexterity/upgrades/to2002.py
+-rw-r--r--   0 maurits    (501) staff       (20)      606 2023-05-22 17:52:44.000000 plone.app.dexterity-3.1.1/plone/app/dexterity/upgrades/to2003.py
+-rw-r--r--   0 maurits    (501) staff       (20)      976 2023-05-22 17:52:44.000000 plone.app.dexterity-3.1.1/plone/app/dexterity/upgrades/to2004.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1444 2023-05-22 17:52:44.000000 plone.app.dexterity-3.1.1/plone/app/dexterity/upgrades/to2005.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-22 17:52:45.274311 plone.app.dexterity-3.1.1/plone.app.dexterity.egg-info/
+-rw-r--r--   0 maurits    (501) staff       (20)    44865 2023-05-22 17:52:45.000000 plone.app.dexterity-3.1.1/plone.app.dexterity.egg-info/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)     6580 2023-05-22 17:52:45.000000 plone.app.dexterity-3.1.1/plone.app.dexterity.egg-info/SOURCES.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2023-05-22 17:52:45.000000 plone.app.dexterity-3.1.1/plone.app.dexterity.egg-info/dependency_links.txt
+-rw-r--r--   0 maurits    (501) staff       (20)       40 2023-05-22 17:52:45.000000 plone.app.dexterity-3.1.1/plone.app.dexterity.egg-info/entry_points.txt
+-rw-r--r--   0 maurits    (501) staff       (20)       16 2023-05-22 17:52:45.000000 plone.app.dexterity-3.1.1/plone.app.dexterity.egg-info/namespace_packages.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2023-05-22 17:52:45.000000 plone.app.dexterity-3.1.1/plone.app.dexterity.egg-info/not-zip-safe
+-rw-r--r--   0 maurits    (501) staff       (20)      829 2023-05-22 17:52:45.000000 plone.app.dexterity-3.1.1/plone.app.dexterity.egg-info/requires.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        6 2023-05-22 17:52:45.000000 plone.app.dexterity-3.1.1/plone.app.dexterity.egg-info/top_level.txt
+-rw-r--r--   0 maurits    (501) staff       (20)     1889 2023-05-22 17:52:44.000000 plone.app.dexterity-3.1.1/pyproject.toml
+-rw-r--r--   0 maurits    (501) staff       (20)      287 2023-05-22 17:52:45.309043 plone.app.dexterity-3.1.1/setup.cfg
+-rw-r--r--   0 maurits    (501) staff       (20)     3209 2023-05-22 17:52:44.000000 plone.app.dexterity-3.1.1/setup.py
```

### Comparing `plone.app.dexterity-3.1.0/CHANGES.rst` & `plone.app.dexterity-3.1.1/CHANGES.rst`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,27 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+3.1.1 (2023-05-22)
+------------------
+
+Bug fixes:
+
+
+- Fix transitive circular dependency on `plone.app.layout`.
+  Use moved imports in `plone.base`.
+  Move `plone.app.layout.nextprevious.interfaces.INextPreviousProvider` to `.behaviors.nextprevious`.
+  Move defaultpage warning viewlet to `plone.app.layout`.
+  [@jensens] (fix-circular-dep-palayout)
+
+
 3.1.0 (2023-05-08)
 ------------------
 
 New features:
 
 
 - Content types control panel: Show behavior name and interface. @ksuess, @stevepiercy (#363)
```

### Comparing `plone.app.dexterity-3.1.0/PKG-INFO` & `plone.app.dexterity-3.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plone.app.dexterity
-Version: 3.1.0
+Version: 3.1.1
 Summary: Dexterity is a content type framework for CMF  applications, with particular emphasis on Plone. It can be viewed as an alternative to Archetypes that is more light-weight and modular.
 Home-page: http://plone.org/products/dexterity
 Author: Martin Aspeli, David Glick, et al
 Author-email: dexterity-development@googlegroups.com
 License: GPL
 Keywords: plone ttw dexterity schema interface
 Classifier: Development Status :: 5 - Production/Stable
@@ -327,14 +327,27 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+3.1.1 (2023-05-22)
+------------------
+
+Bug fixes:
+
+
+- Fix transitive circular dependency on `plone.app.layout`.
+  Use moved imports in `plone.base`.
+  Move `plone.app.layout.nextprevious.interfaces.INextPreviousProvider` to `.behaviors.nextprevious`.
+  Move defaultpage warning viewlet to `plone.app.layout`.
+  [@jensens] (fix-circular-dep-palayout)
+
+
 3.1.0 (2023-05-08)
 ------------------
 
 New features:
 
 
 - Content types control panel: Show behavior name and interface. @ksuess, @stevepiercy (#363)
```

### Comparing `plone.app.dexterity-3.1.0/README.rst` & `plone.app.dexterity-3.1.1/README.rst`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.1.0/RELEASE_NOTES.rst` & `plone.app.dexterity-3.1.1/RELEASE_NOTES.rst`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.1.0/docs/LICENSE.GPL` & `plone.app.dexterity-3.1.1/docs/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.1.0/docs/LICENSE.txt` & `plone.app.dexterity-3.1.1/docs/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.1.0/docs/Makefile` & `plone.app.dexterity-3.1.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.1.0/docs/advanced/behaviours.rst` & `plone.app.dexterity-3.1.1/docs/advanced/behaviours.rst`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.1.0/docs/advanced/catalog-indexing-strategies.rst` & `plone.app.dexterity-3.1.1/docs/advanced/catalog-indexing-strategies.rst`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.1.0/docs/advanced/custom-add-and-edit-forms.rst` & `plone.app.dexterity-3.1.1/docs/advanced/custom-add-and-edit-forms.rst`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.1.0/docs/advanced/custom-content-classes.rst` & `plone.app.dexterity-3.1.1/docs/advanced/custom-content-classes.rst`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.1.0/docs/advanced/defaults.rst` & `plone.app.dexterity-3.1.1/docs/advanced/defaults.rst`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.1.0/docs/advanced/event-handlers.rst` & `plone.app.dexterity-3.1.1/docs/advanced/event-handlers.rst`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.1.0/docs/advanced/files-and-images.rst` & `plone.app.dexterity-3.1.1/docs/advanced/files-and-images.rst`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.1.0/docs/advanced/permissions.rst` & `plone.app.dexterity-3.1.1/docs/advanced/permissions.rst`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.1.0/docs/advanced/references.rst` & `plone.app.dexterity-3.1.1/docs/advanced/references.rst`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.1.0/docs/advanced/rich-text-markup-transformations.rst` & `plone.app.dexterity-3.1.1/docs/advanced/rich-text-markup-transformations.rst`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.1.0/docs/advanced/static-resources.rst` & `plone.app.dexterity-3.1.1/docs/advanced/static-resources.rst`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.1.0/docs/advanced/validators.rst` & `plone.app.dexterity-3.1.1/docs/advanced/validators.rst`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.1.0/docs/advanced/vocabularies.rst` & `plone.app.dexterity-3.1.1/docs/advanced/vocabularies.rst`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.1.0/docs/advanced/webdav-and-other-file-representations.rst` & `plone.app.dexterity-3.1.1/docs/advanced/webdav-and-other-file-representations.rst`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.1.0/docs/advanced/workflow.rst` & `plone.app.dexterity-3.1.1/docs/advanced/workflow.rst`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.1.0/docs/behaviors/behavior-basics.rst` & `plone.app.dexterity-3.1.1/docs/behaviors/behavior-basics.rst`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.1.0/docs/behaviors/creating-and-registering-behaviors.rst` & `plone.app.dexterity-3.1.1/docs/behaviors/creating-and-registering-behaviors.rst`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.1.0/docs/behaviors/intro.rst` & `plone.app.dexterity-3.1.1/docs/behaviors/intro.rst`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.1.0/docs/behaviors/providing-marker-interfaces.rst` & `plone.app.dexterity-3.1.1/docs/behaviors/providing-marker-interfaces.rst`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.1.0/docs/behaviors/schema-only-behaviors.rst` & `plone.app.dexterity-3.1.1/docs/behaviors/schema-only-behaviors.rst`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.1.0/docs/behaviors/testing-behaviors.rst` & `plone.app.dexterity-3.1.1/docs/behaviors/testing-behaviors.rst`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.1.0/docs/conf.py` & `plone.app.dexterity-3.1.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.1.0/docs/custom-views.rst` & `plone.app.dexterity-3.1.1/docs/custom-views.rst`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.1.0/docs/designing.rst` & `plone.app.dexterity-3.1.1/docs/designing.rst`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.1.0/docs/install.rst` & `plone.app.dexterity-3.1.1/docs/install.rst`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.1.0/docs/intro.rst` & `plone.app.dexterity-3.1.1/docs/intro.rst`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.1.0/docs/model-driven-types.rst` & `plone.app.dexterity-3.1.1/docs/model-driven-types.rst`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.1.0/docs/prerequisite.rst` & `plone.app.dexterity-3.1.1/docs/prerequisite.rst`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.1.0/docs/reference/dexterity-xml.rst` & `plone.app.dexterity-3.1.1/docs/reference/dexterity-xml.rst`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.1.0/docs/reference/fields.rst` & `plone.app.dexterity-3.1.1/docs/reference/fields.rst`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.1.0/docs/reference/form-schema-hints.rst` & `plone.app.dexterity-3.1.1/docs/reference/form-schema-hints.rst`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.1.0/docs/reference/manipulating-content-objects.rst` & `plone.app.dexterity-3.1.1/docs/reference/manipulating-content-objects.rst`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.1.0/docs/reference/misc.rst` & `plone.app.dexterity-3.1.1/docs/reference/misc.rst`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.1.0/docs/reference/standard-behaviours.rst` & `plone.app.dexterity-3.1.1/docs/reference/standard-behaviours.rst`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.1.0/docs/reference/widgets.rst` & `plone.app.dexterity-3.1.1/docs/reference/widgets.rst`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.1.0/docs/schema-driven-types.rst` & `plone.app.dexterity-3.1.1/docs/schema-driven-types.rst`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.1.0/docs/testing/integration-tests.rst` & `plone.app.dexterity-3.1.1/docs/testing/integration-tests.rst`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.1.0/docs/testing/mock-testing.rst` & `plone.app.dexterity-3.1.1/docs/testing/mock-testing.rst`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.1.0/docs/testing/unit-tests.rst` & `plone.app.dexterity-3.1.1/docs/testing/unit-tests.rst`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.1.0/plone/app/dexterity/TODO.txt` & `plone.app.dexterity-3.1.1/plone/app/dexterity/TODO.txt`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.1.0/plone/app/dexterity/behaviors/configure.zcml` & `plone.app.dexterity-3.1.1/plone/app/dexterity/behaviors/configure.zcml`

 * *Files 1% similar despite different names*

```diff
@@ -78,15 +78,15 @@
   <adapter factory=".filename.NameFromFileName" />
 
   <!-- Navigation root -->
   <plone:behavior
       name="plone.navigationroot"
       title="Navigation root"
       description="Make all items of this type a navigation root"
-      provides="plone.app.layout.navigation.interfaces.INavigationRoot"
+      provides="plone.base.interfaces.INavigationRoot"
       />
 
   <!-- Exclude from navigation -->
   <plone:behavior
       name="plone.excludefromnavigation"
       title="Exclude From navigation"
       description="Allow items to be excluded from navigation"
```

### Comparing `plone.app.dexterity-3.1.0/plone/app/dexterity/behaviors/constrains.py` & `plone.app.dexterity-3.1.1/plone/app/dexterity/behaviors/constrains.py`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.1.0/plone/app/dexterity/behaviors/discussion.py` & `plone.app.dexterity-3.1.1/plone/app/dexterity/behaviors/discussion.py`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.1.0/plone/app/dexterity/behaviors/exclfromnav.py` & `plone.app.dexterity-3.1.1/plone/app/dexterity/behaviors/exclfromnav.py`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.1.0/plone/app/dexterity/behaviors/filename.py` & `plone.app.dexterity-3.1.1/plone/app/dexterity/behaviors/filename.py`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.1.0/plone/app/dexterity/behaviors/id.py` & `plone.app.dexterity-3.1.1/plone/app/dexterity/behaviors/id.py`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.1.0/plone/app/dexterity/behaviors/metadata.py` & `plone.app.dexterity-3.1.1/plone/app/dexterity/behaviors/metadata.py`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.1.0/plone/app/dexterity/behaviors/nextprevious.py` & `plone.app.dexterity-3.1.1/plone/app/dexterity/behaviors/nextprevious.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from AccessControl import getSecurityManager
 from Acquisition import aq_base
 from plone.app.dexterity import _
-from plone.app.layout.nextprevious.interfaces import INextPreviousProvider
 from plone.autoform import directives
 from plone.autoform.interfaces import IFormFieldProvider
 from plone.registry.interfaces import IRegistry
 from plone.supermodel import model
 from Products.CMFCore.interfaces import IContentish
 from z3c.form import widget
 from z3c.form.interfaces import IAddForm
@@ -117,14 +116,40 @@
             url=url,
             title=obj.Title(),
             description=obj.Description(),
             portal_type=ptype,
         )
 
 
+class INextPreviousProvider(Interface):
+    """A folderish component capable of describing the next and previous
+    item relative to a particular id.
+    """
+
+    enabled = schema.Bool(title="True if next/previous behaviour is enabled")
+
+    def getNextItem(obj):
+        """Returns information about next item in the container relative to
+        the given object.
+
+        This is a dict with the following keys:
+
+            - id, the id of the object
+            - url, the url of the object
+            - title, the title of the object
+            - description, a description of the object
+            - portal_type, the object's portal type
+        """
+
+    def getPreviousItem(obj):
+        """Returns the previous item in the container relative to the given
+        object
+        """
+
+
 @implementer(INextPreviousProvider)
 @adapter(INextPreviousToggle)
 class NextPreviousToggle(NextPreviousBase):
     """adapter for acting as a next/previous provider"""
 
     @property
     def enabled(self):
```

### Comparing `plone.app.dexterity-3.1.0/plone/app/dexterity/behaviors/tests/test_contrains.py` & `plone.app.dexterity-3.1.1/plone/app/dexterity/behaviors/tests/test_contrains.py`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.1.0/plone/app/dexterity/behaviors/tests/test_id.py` & `plone.app.dexterity-3.1.1/plone/app/dexterity/behaviors/tests/test_id.py`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.1.0/plone/app/dexterity/behaviors/tests/test_metadata.py` & `plone.app.dexterity-3.1.1/plone/app/dexterity/behaviors/tests/test_metadata.py`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.1.0/plone/app/dexterity/browser/add_type.py` & `plone.app.dexterity-3.1.1/plone/app/dexterity/browser/add_type.py`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.1.0/plone/app/dexterity/browser/behaviors.pt` & `plone.app.dexterity-3.1.1/plone/app/dexterity/browser/behaviors.pt`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.1.0/plone/app/dexterity/browser/behaviors.py` & `plone.app.dexterity-3.1.1/plone/app/dexterity/browser/behaviors.py`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.1.0/plone/app/dexterity/browser/clone_type.py` & `plone.app.dexterity-3.1.1/plone/app/dexterity/browser/clone_type.py`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.1.0/plone/app/dexterity/browser/configure.zcml` & `plone.app.dexterity-3.1.1/plone/app/dexterity/browser/configure.zcml`

 * *Files 3% similar despite different names*

```diff
@@ -34,23 +34,14 @@
       name="folder_listing"
       for="plone.base.interfaces.IPloneSiteRoot"
       class=".folder_listing.FolderView"
       template="folder_listing.pt"
       permission="zope2.View"
       />
 
-  <!-- warning when editing default pages -->
-  <browser:viewlet
-      name="plone.app.dexterity.defaultpagewarning"
-      view="plone.dexterity.interfaces.IDexterityEditForm"
-      manager="plone.app.layout.viewlets.interfaces.IGlobalStatusMessage"
-      template="default_page_warning.pt"
-      permission="cmf.ModifyPortalContent"
-      />
-
   <!-- Control panel -->
 
   <browser:page
       name="dexterity-types"
       for="plone.base.interfaces.IPloneSiteRoot"
       class=".types.TypesContext"
       allowed_interface="OFS.interfaces.IItem"
```

### Comparing `plone.app.dexterity-3.1.0/plone/app/dexterity/browser/container.pt` & `plone.app.dexterity-3.1.1/plone/app/dexterity/browser/container.pt`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.1.0/plone/app/dexterity/browser/export.py` & `plone.app.dexterity-3.1.1/plone/app/dexterity/browser/export.py`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.1.0/plone/app/dexterity/browser/fields.py` & `plone.app.dexterity-3.1.1/plone/app/dexterity/browser/fields.py`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.1.0/plone/app/dexterity/browser/folder_listing.pt` & `plone.app.dexterity-3.1.1/plone/app/dexterity/browser/folder_listing.pt`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.1.0/plone/app/dexterity/browser/folder_listing.py` & `plone.app.dexterity-3.1.1/plone/app/dexterity/browser/folder_listing.py`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.1.0/plone/app/dexterity/browser/import_types.py` & `plone.app.dexterity-3.1.1/plone/app/dexterity/browser/import_types.py`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.1.0/plone/app/dexterity/browser/item.pt` & `plone.app.dexterity-3.1.1/plone/app/dexterity/browser/item.pt`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.1.0/plone/app/dexterity/browser/modeleditor.pt` & `plone.app.dexterity-3.1.1/plone/app/dexterity/browser/modeleditor.pt`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.1.0/plone/app/dexterity/browser/modeleditor.py` & `plone.app.dexterity-3.1.1/plone/app/dexterity/browser/modeleditor.py`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.1.0/plone/app/dexterity/browser/overview.pt` & `plone.app.dexterity-3.1.1/plone/app/dexterity/browser/overview.pt`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.1.0/plone/app/dexterity/browser/overview.py` & `plone.app.dexterity-3.1.1/plone/app/dexterity/browser/overview.py`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.1.0/plone/app/dexterity/browser/tabbed_forms.pt` & `plone.app.dexterity-3.1.1/plone/app/dexterity/browser/tabbed_forms.pt`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.1.0/plone/app/dexterity/browser/types.py` & `plone.app.dexterity-3.1.1/plone/app/dexterity/browser/types.py`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.1.0/plone/app/dexterity/browser/types_listing.pt` & `plone.app.dexterity-3.1.1/plone/app/dexterity/browser/types_listing.pt`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.1.0/plone/app/dexterity/browser/types_listing_row.pt` & `plone.app.dexterity-3.1.1/plone/app/dexterity/browser/types_listing_row.pt`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.1.0/plone/app/dexterity/browser/typesformwrapper.pt` & `plone.app.dexterity-3.1.1/plone/app/dexterity/browser/typesformwrapper.pt`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.1.0/plone/app/dexterity/configure.zcml` & `plone.app.dexterity-3.1.1/plone/app/dexterity/configure.zcml`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.1.0/plone/app/dexterity/events.zcml` & `plone.app.dexterity-3.1.1/plone/app/dexterity/events.zcml`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.1.0/plone/app/dexterity/factories.py` & `plone.app.dexterity-3.1.1/plone/app/dexterity/factories.py`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.1.0/plone/app/dexterity/interfaces.py` & `plone.app.dexterity-3.1.1/plone/app/dexterity/interfaces.py`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.1.0/plone/app/dexterity/permissions.py` & `plone.app.dexterity-3.1.1/plone/app/dexterity/permissions.py`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.1.0/plone/app/dexterity/profiles/default/controlpanel.xml` & `plone.app.dexterity-3.1.1/plone/app/dexterity/profiles/default/controlpanel.xml`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.1.0/plone/app/dexterity/profiles/testing/types/Document.xml` & `plone.app.dexterity-3.1.1/plone/app/dexterity/profiles/testing/types/Document.xml`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.1.0/plone/app/dexterity/profiles/testing/types/Folder.xml` & `plone.app.dexterity-3.1.1/plone/app/dexterity/profiles/testing/types/Folder.xml`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.1.0/plone/app/dexterity/serialize.py` & `plone.app.dexterity-3.1.1/plone/app/dexterity/serialize.py`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.1.0/plone/app/dexterity/testing.py` & `plone.app.dexterity-3.1.1/plone/app/dexterity/testing.py`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.1.0/plone/app/dexterity/tests/discussion.txt` & `plone.app.dexterity-3.1.1/plone/app/dexterity/tests/discussion.txt`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.1.0/plone/app/dexterity/tests/editing.rst` & `plone.app.dexterity-3.1.1/plone/app/dexterity/tests/editing.rst`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.1.0/plone/app/dexterity/tests/filename.txt` & `plone.app.dexterity-3.1.1/plone/app/dexterity/tests/filename.txt`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.1.0/plone/app/dexterity/tests/import/dexterity_export.zip` & `plone.app.dexterity-3.1.1/plone/app/dexterity/tests/import/dexterity_export.zip`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.1.0/plone/app/dexterity/tests/metadata.txt` & `plone.app.dexterity-3.1.1/plone/app/dexterity/tests/metadata.txt`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.1.0/plone/app/dexterity/tests/namefromtitle.txt` & `plone.app.dexterity-3.1.1/plone/app/dexterity/tests/namefromtitle.txt`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.1.0/plone/app/dexterity/tests/nextprevious.txt` & `plone.app.dexterity-3.1.1/plone/app/dexterity/tests/nextprevious.txt`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.1.0/plone/app/dexterity/tests/robot/test_types.robot` & `plone.app.dexterity-3.1.1/plone/app/dexterity/tests/robot/test_types.robot`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.1.0/plone/app/dexterity/tests/schema_events.txt` & `plone.app.dexterity-3.1.1/plone/app/dexterity/tests/schema_events.txt`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.1.0/plone/app/dexterity/tests/test_constrains.py` & `plone.app.dexterity-3.1.1/plone/app/dexterity/tests/test_constrains.py`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.1.0/plone/app/dexterity/tests/test_doctests.py` & `plone.app.dexterity-3.1.1/plone/app/dexterity/tests/test_doctests.py`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.1.0/plone/app/dexterity/tests/test_export.py` & `plone.app.dexterity-3.1.1/plone/app/dexterity/tests/test_export.py`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.1.0/plone/app/dexterity/tests/test_import.py` & `plone.app.dexterity-3.1.1/plone/app/dexterity/tests/test_import.py`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.1.0/plone/app/dexterity/tests/test_nextprevious.py` & `plone.app.dexterity-3.1.1/plone/app/dexterity/tests/test_nextprevious.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
+from ..behaviors.nextprevious import INextPreviousProvider
 from plone.app.dexterity.testing import DEXTERITY_INTEGRATION_TESTING
-from plone.app.layout.nextprevious.interfaces import INextPreviousProvider
 from plone.app.testing import login
 from plone.app.testing import logout
 from plone.app.testing import setRoles
 from plone.app.testing import TEST_USER_ID
 from plone.dexterity.fti import DexterityFTI
 from Products.CMFCore.utils import getToolByName
```

### Comparing `plone.app.dexterity-3.1.0/plone/app/dexterity/tests/test_permissions.py` & `plone.app.dexterity-3.1.1/plone/app/dexterity/tests/test_permissions.py`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.1.0/plone/app/dexterity/tests/test_robot.py` & `plone.app.dexterity-3.1.1/plone/app/dexterity/tests/test_robot.py`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.1.0/plone/app/dexterity/tests/test_upgrades.py` & `plone.app.dexterity-3.1.1/plone/app/dexterity/tests/test_upgrades.py`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.1.0/plone/app/dexterity/textindexer/__init__.py` & `plone.app.dexterity-3.1.1/plone/app/dexterity/textindexer/__init__.py`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.1.0/plone/app/dexterity/textindexer/configure.zcml` & `plone.app.dexterity-3.1.1/plone/app/dexterity/textindexer/configure.zcml`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.1.0/plone/app/dexterity/textindexer/converters.py` & `plone.app.dexterity-3.1.1/plone/app/dexterity/textindexer/converters.py`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.1.0/plone/app/dexterity/textindexer/directives.py` & `plone.app.dexterity-3.1.1/plone/app/dexterity/textindexer/directives.py`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.1.0/plone/app/dexterity/textindexer/indexer.py` & `plone.app.dexterity-3.1.1/plone/app/dexterity/textindexer/indexer.py`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.1.0/plone/app/dexterity/textindexer/interfaces.py` & `plone.app.dexterity-3.1.1/plone/app/dexterity/textindexer/interfaces.py`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.1.0/plone/app/dexterity/textindexer/schemaeditor.py` & `plone.app.dexterity-3.1.1/plone/app/dexterity/textindexer/schemaeditor.py`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.1.0/plone/app/dexterity/textindexer/supermodel.py` & `plone.app.dexterity-3.1.1/plone/app/dexterity/textindexer/supermodel.py`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.1.0/plone/app/dexterity/textindexer/testing.py` & `plone.app.dexterity-3.1.1/plone/app/dexterity/textindexer/testing.py`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.1.0/plone/app/dexterity/textindexer/tests/behaviors.py` & `plone.app.dexterity-3.1.1/plone/app/dexterity/textindexer/tests/behaviors.py`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.1.0/plone/app/dexterity/textindexer/tests/behaviors.rst` & `plone.app.dexterity-3.1.1/plone/app/dexterity/textindexer/tests/behaviors.rst`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.1.0/plone/app/dexterity/textindexer/tests/configure.zcml` & `plone.app.dexterity-3.1.1/plone/app/dexterity/textindexer/tests/configure.zcml`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.1.0/plone/app/dexterity/textindexer/tests/file.pdf` & `plone.app.dexterity-3.1.1/plone/app/dexterity/textindexer/tests/file.pdf`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.1.0/plone/app/dexterity/textindexer/tests/test_behaviors.py` & `plone.app.dexterity-3.1.1/plone/app/dexterity/textindexer/tests/test_behaviors.py`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.1.0/plone/app/dexterity/textindexer/tests/test_directives.py` & `plone.app.dexterity-3.1.1/plone/app/dexterity/textindexer/tests/test_directives.py`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.1.0/plone/app/dexterity/textindexer/tests/test_schemaeditor.py` & `plone.app.dexterity-3.1.1/plone/app/dexterity/textindexer/tests/test_schemaeditor.py`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.1.0/plone/app/dexterity/textindexer/tests/test_supermodel_handler.py` & `plone.app.dexterity-3.1.1/plone/app/dexterity/textindexer/tests/test_supermodel_handler.py`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.1.0/plone/app/dexterity/textindexer/tests/test_utils.py` & `plone.app.dexterity-3.1.1/plone/app/dexterity/textindexer/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.1.0/plone/app/dexterity/textindexer/utils.py` & `plone.app.dexterity-3.1.1/plone/app/dexterity/textindexer/utils.py`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.1.0/plone/app/dexterity/upgrades/configure.zcml` & `plone.app.dexterity-3.1.1/plone/app/dexterity/upgrades/configure.zcml`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.1.0/plone/app/dexterity/upgrades/to2001.py` & `plone.app.dexterity-3.1.1/plone/app/dexterity/upgrades/to2001.py`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.1.0/plone/app/dexterity/upgrades/to2003.py` & `plone.app.dexterity-3.1.1/plone/app/dexterity/upgrades/to2003.py`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.1.0/plone/app/dexterity/upgrades/to2004.py` & `plone.app.dexterity-3.1.1/plone/app/dexterity/upgrades/to2004.py`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.1.0/plone/app/dexterity/upgrades/to2005.py` & `plone.app.dexterity-3.1.1/plone/app/dexterity/upgrades/to2005.py`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.1.0/plone.app.dexterity.egg-info/PKG-INFO` & `plone.app.dexterity-3.1.1/plone.app.dexterity.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plone.app.dexterity
-Version: 3.1.0
+Version: 3.1.1
 Summary: Dexterity is a content type framework for CMF  applications, with particular emphasis on Plone. It can be viewed as an alternative to Archetypes that is more light-weight and modular.
 Home-page: http://plone.org/products/dexterity
 Author: Martin Aspeli, David Glick, et al
 Author-email: dexterity-development@googlegroups.com
 License: GPL
 Keywords: plone ttw dexterity schema interface
 Classifier: Development Status :: 5 - Production/Stable
@@ -327,14 +327,27 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+3.1.1 (2023-05-22)
+------------------
+
+Bug fixes:
+
+
+- Fix transitive circular dependency on `plone.app.layout`.
+  Use moved imports in `plone.base`.
+  Move `plone.app.layout.nextprevious.interfaces.INextPreviousProvider` to `.behaviors.nextprevious`.
+  Move defaultpage warning viewlet to `plone.app.layout`.
+  [@jensens] (fix-circular-dep-palayout)
+
+
 3.1.0 (2023-05-08)
 ------------------
 
 New features:
 
 
 - Content types control panel: Show behavior name and interface. @ksuess, @stevepiercy (#363)
```

### Comparing `plone.app.dexterity-3.1.0/plone.app.dexterity.egg-info/SOURCES.txt` & `plone.app.dexterity-3.1.1/plone.app.dexterity.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -92,15 +92,14 @@
 plone/app/dexterity/browser/add_type.py
 plone/app/dexterity/browser/behaviors.pt
 plone/app/dexterity/browser/behaviors.py
 plone/app/dexterity/browser/blank.css
 plone/app/dexterity/browser/clone_type.py
 plone/app/dexterity/browser/configure.zcml
 plone/app/dexterity/browser/container.pt
-plone/app/dexterity/browser/default_page_warning.pt
 plone/app/dexterity/browser/export.py
 plone/app/dexterity/browser/fields.py
 plone/app/dexterity/browser/folder_listing.pt
 plone/app/dexterity/browser/folder_listing.py
 plone/app/dexterity/browser/import_types.py
 plone/app/dexterity/browser/item.pt
 plone/app/dexterity/browser/layout.py
```

### Comparing `plone.app.dexterity-3.1.0/plone.app.dexterity.egg-info/requires.txt` & `plone.app.dexterity-3.1.1/plone.app.dexterity.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.1.0/pyproject.toml` & `plone.app.dexterity-3.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.1.0/setup.py` & `plone.app.dexterity-3.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages
 from setuptools import setup
 
 
-version = "3.1.0"
+version = "3.1.1"
 
 short_description = (
     "Dexterity is a content type framework for CMF  applications, "
     "with particular emphasis on Plone. It can be viewed as an "
     "alternative to Archetypes that is more light-weight and modular."
 )
```

