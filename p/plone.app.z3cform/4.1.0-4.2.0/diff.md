# Comparing `tmp/plone.app.z3cform-4.1.0.tar.gz` & `tmp/plone.app.z3cform-4.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plone.app.z3cform-4.1.0.tar", last modified: Wed Apr 26 21:55:46 2023, max compression
+gzip compressed data, was "plone.app.z3cform-4.2.0.tar", last modified: Mon May 22 21:11:04 2023, max compression
```

## Comparing `plone.app.z3cform-4.1.0.tar` & `plone.app.z3cform-4.2.0.tar`

### file list

```diff
@@ -1,103 +1,103 @@
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-26 21:55:46.671824 plone.app.z3cform-4.1.0/
--rw-r--r--   0 maurits    (501) staff       (20)    24989 2023-04-26 21:55:45.000000 plone.app.z3cform-4.1.0/CHANGES.rst
--rw-r--r--   0 maurits    (501) staff       (20)       70 2023-04-26 21:55:45.000000 plone.app.z3cform-4.1.0/CONTRIBUTING.rst
--rw-r--r--   0 maurits    (501) staff       (20)      146 2023-04-26 21:55:45.000000 plone.app.z3cform-4.1.0/MANIFEST.in
--rw-r--r--   0 maurits    (501) staff       (20)    48242 2023-04-26 21:55:46.671959 plone.app.z3cform-4.1.0/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)    13825 2023-04-26 21:55:45.000000 plone.app.z3cform-4.1.0/README.rst
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-26 21:55:46.648920 plone.app.z3cform-4.1.0/docs/
--rw-r--r--   0 maurits    (501) staff       (20)    12282 2023-04-26 21:55:45.000000 plone.app.z3cform-4.1.0/docs/LICENSE.GPL
--rw-r--r--   0 maurits    (501) staff       (20)      749 2023-04-26 21:55:45.000000 plone.app.z3cform-4.1.0/docs/LICENSE.txt
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-26 21:55:46.649168 plone.app.z3cform-4.1.0/plone/
--rw-r--r--   0 maurits    (501) staff       (20)       56 2023-04-26 21:55:45.000000 plone.app.z3cform-4.1.0/plone/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-26 21:55:46.651481 plone.app.z3cform-4.1.0/plone/app/
--rw-r--r--   0 maurits    (501) staff       (20)       56 2023-04-26 21:55:45.000000 plone.app.z3cform-4.1.0/plone/app/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-26 21:55:46.656343 plone.app.z3cform-4.1.0/plone/app/z3cform/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-04-26 21:55:45.000000 plone.app.z3cform-4.1.0/plone/app/z3cform/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     2935 2023-04-26 21:55:45.000000 plone.app.z3cform-4.1.0/plone/app/z3cform/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)    18540 2023-04-26 21:55:45.000000 plone.app.z3cform-4.1.0/plone/app/z3cform/converters.py
--rw-r--r--   0 maurits    (501) staff       (20)     1310 2023-04-26 21:55:45.000000 plone.app.z3cform-4.1.0/plone/app/z3cform/converters.zcml
--rw-r--r--   0 maurits    (501) staff       (20)      724 2023-04-26 21:55:45.000000 plone.app.z3cform-4.1.0/plone/app/z3cform/csrf.py
--rw-r--r--   0 maurits    (501) staff       (20)      431 2023-04-26 21:55:45.000000 plone.app.z3cform-4.1.0/plone/app/z3cform/factories.py
--rw-r--r--   0 maurits    (501) staff       (20)     2349 2023-04-26 21:55:45.000000 plone.app.z3cform-4.1.0/plone/app/z3cform/inline_validation.py
--rw-r--r--   0 maurits    (501) staff       (20)     7482 2023-04-26 21:55:45.000000 plone.app.z3cform-4.1.0/plone/app/z3cform/inline_validation.rst
--rw-r--r--   0 maurits    (501) staff       (20)     2500 2023-04-26 21:55:45.000000 plone.app.z3cform-4.1.0/plone/app/z3cform/interfaces.py
--rw-r--r--   0 maurits    (501) staff       (20)      212 2023-04-26 21:55:45.000000 plone.app.z3cform-4.1.0/plone/app/z3cform/layout.py
--rw-r--r--   0 maurits    (501) staff       (20)      152 2023-04-26 21:55:45.000000 plone.app.z3cform-4.1.0/plone/app/z3cform/overrides.zcml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-26 21:55:46.645957 plone.app.z3cform-4.1.0/plone/app/z3cform/profiles/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-26 21:55:46.657138 plone.app.z3cform-4.1.0/plone/app/z3cform/profiles/default/
--rw-r--r--   0 maurits    (501) staff       (20)      163 2023-04-26 21:55:45.000000 plone.app.z3cform-4.1.0/plone/app/z3cform/profiles/default/browserlayer.xml
--rw-r--r--   0 maurits    (501) staff       (20)       85 2023-04-26 21:55:45.000000 plone.app.z3cform-4.1.0/plone/app/z3cform/profiles/default/metadata.xml
--rw-r--r--   0 maurits    (501) staff       (20)      635 2023-04-26 21:55:45.000000 plone.app.z3cform-4.1.0/plone/app/z3cform/profiles.zcml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-26 21:55:46.664494 plone.app.z3cform-4.1.0/plone/app/z3cform/templates/
--rw-r--r--   0 maurits    (501) staff       (20)     1013 2023-04-26 21:55:45.000000 plone.app.z3cform-4.1.0/plone/app/z3cform/templates/ajaxselect_display.pt
--rw-r--r--   0 maurits    (501) staff       (20)     3643 2023-04-26 21:55:45.000000 plone.app.z3cform-4.1.0/plone/app/z3cform/templates/checkbox_input.pt
--rw-r--r--   0 maurits    (501) staff       (20)      140 2023-04-26 21:55:45.000000 plone.app.z3cform-4.1.0/plone/app/z3cform/templates/contentprovider-widget.pt
--rw-r--r--   0 maurits    (501) staff       (20)      209 2023-04-26 21:55:45.000000 plone.app.z3cform-4.1.0/plone/app/z3cform/templates/error.pt
--rw-r--r--   0 maurits    (501) staff       (20)     4806 2023-04-26 21:55:45.000000 plone.app.z3cform-4.1.0/plone/app/z3cform/templates/file_input.pt
--rw-r--r--   0 maurits    (501) staff       (20)      829 2023-04-26 21:55:45.000000 plone.app.z3cform-4.1.0/plone/app/z3cform/templates/form.pt
--rw-r--r--   0 maurits    (501) staff       (20)     4798 2023-04-26 21:55:45.000000 plone.app.z3cform-4.1.0/plone/app/z3cform/templates/image_input.pt
--rw-r--r--   0 maurits    (501) staff       (20)      677 2023-04-26 21:55:45.000000 plone.app.z3cform-4.1.0/plone/app/z3cform/templates/layout.pt
--rw-r--r--   0 maurits    (501) staff       (20)     3547 2023-04-26 21:55:45.000000 plone.app.z3cform-4.1.0/plone/app/z3cform/templates/link_input.pt
--rw-r--r--   0 maurits    (501) staff       (20)     9551 2023-04-26 21:55:45.000000 plone.app.z3cform-4.1.0/plone/app/z3cform/templates/macros.pt
--rw-r--r--   0 maurits    (501) staff       (20)     4033 2023-04-26 21:55:45.000000 plone.app.z3cform-4.1.0/plone/app/z3cform/templates/multi_input.pt
--rw-r--r--   0 maurits    (501) staff       (20)     1861 2023-04-26 21:55:45.000000 plone.app.z3cform-4.1.0/plone/app/z3cform/templates/object_input.pt
--rw-r--r--   0 maurits    (501) staff       (20)     5486 2023-04-26 21:55:45.000000 plone.app.z3cform-4.1.0/plone/app/z3cform/templates/orderedselect_input.pt
--rw-r--r--   0 maurits    (501) staff       (20)     1448 2023-04-26 21:55:45.000000 plone.app.z3cform-4.1.0/plone/app/z3cform/templates/password_input.pt
--rw-r--r--   0 maurits    (501) staff       (20)      650 2023-04-26 21:55:45.000000 plone.app.z3cform-4.1.0/plone/app/z3cform/templates/radio_input.pt
--rw-r--r--   0 maurits    (501) staff       (20)     1418 2023-04-26 21:55:45.000000 plone.app.z3cform-4.1.0/plone/app/z3cform/templates/radio_input_single.pt
--rw-r--r--   0 maurits    (501) staff       (20)     1869 2023-04-26 21:55:45.000000 plone.app.z3cform-4.1.0/plone/app/z3cform/templates/relateditems_display.pt
--rw-r--r--   0 maurits    (501) staff       (20)     1937 2023-04-26 21:55:45.000000 plone.app.z3cform-4.1.0/plone/app/z3cform/templates/select_input.pt
--rw-r--r--   0 maurits    (501) staff       (20)      976 2023-04-26 21:55:45.000000 plone.app.z3cform-4.1.0/plone/app/z3cform/templates/singlecheckbox.pt
--rw-r--r--   0 maurits    (501) staff       (20)      765 2023-04-26 21:55:45.000000 plone.app.z3cform-4.1.0/plone/app/z3cform/templates/singlecheckboxbool_display.pt
--rw-r--r--   0 maurits    (501) staff       (20)     1357 2023-04-26 21:55:45.000000 plone.app.z3cform-4.1.0/plone/app/z3cform/templates/singlecheckboxbool_hidden.pt
--rw-r--r--   0 maurits    (501) staff       (20)     4046 2023-04-26 21:55:45.000000 plone.app.z3cform-4.1.0/plone/app/z3cform/templates/singlecheckboxbool_input.pt
--rw-r--r--   0 maurits    (501) staff       (20)     1335 2023-04-26 21:55:45.000000 plone.app.z3cform-4.1.0/plone/app/z3cform/templates/submit_input.pt
--rw-r--r--   0 maurits    (501) staff       (20)     1574 2023-04-26 21:55:45.000000 plone.app.z3cform-4.1.0/plone/app/z3cform/templates/text_input.pt
--rw-r--r--   0 maurits    (501) staff       (20)     1414 2023-04-26 21:55:45.000000 plone.app.z3cform-4.1.0/plone/app/z3cform/templates/textarea_input.pt
--rw-r--r--   0 maurits    (501) staff       (20)     3703 2023-04-26 21:55:45.000000 plone.app.z3cform-4.1.0/plone/app/z3cform/templates/textfield_widget_input.pt
--rw-r--r--   0 maurits    (501) staff       (20)     1356 2023-04-26 21:55:45.000000 plone.app.z3cform-4.1.0/plone/app/z3cform/templates/textlines_input.pt
--rw-r--r--   0 maurits    (501) staff       (20)     1812 2023-04-26 21:55:45.000000 plone.app.z3cform-4.1.0/plone/app/z3cform/templates/widget.pt
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-26 21:55:46.667203 plone.app.z3cform-4.1.0/plone/app/z3cform/tests/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-04-26 21:55:45.000000 plone.app.z3cform-4.1.0/plone/app/z3cform/tests/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     2421 2023-04-26 21:55:45.000000 plone.app.z3cform-4.1.0/plone/app/z3cform/tests/example.py
--rw-r--r--   0 maurits    (501) staff       (20)     1139 2023-04-26 21:55:45.000000 plone.app.z3cform-4.1.0/plone/app/z3cform/tests/layer.py
--rw-r--r--   0 maurits    (501) staff       (20)      907 2023-04-26 21:55:45.000000 plone.app.z3cform-4.1.0/plone/app/z3cform/tests/test_csrf.py
--rw-r--r--   0 maurits    (501) staff       (20)    17512 2023-04-26 21:55:45.000000 plone.app.z3cform-4.1.0/plone/app/z3cform/tests/test_patterns.py
--rw-r--r--   0 maurits    (501) staff       (20)     4554 2023-04-26 21:55:45.000000 plone.app.z3cform-4.1.0/plone/app/z3cform/tests/test_utils.py
--rw-r--r--   0 maurits    (501) staff       (20)     1349 2023-04-26 21:55:45.000000 plone.app.z3cform-4.1.0/plone/app/z3cform/tests/test_widget.py
--rw-r--r--   0 maurits    (501) staff       (20)    66963 2023-04-26 21:55:45.000000 plone.app.z3cform-4.1.0/plone/app/z3cform/tests/test_widgets.py
--rw-r--r--   0 maurits    (501) staff       (20)      776 2023-04-26 21:55:45.000000 plone.app.z3cform-4.1.0/plone/app/z3cform/tests/testing.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     2208 2023-04-26 21:55:45.000000 plone.app.z3cform-4.1.0/plone/app/z3cform/tests/tests.py
--rw-r--r--   0 maurits    (501) staff       (20)     5619 2023-04-26 21:55:45.000000 plone.app.z3cform-4.1.0/plone/app/z3cform/utils.py
--rw-r--r--   0 maurits    (501) staff       (20)     2739 2023-04-26 21:55:45.000000 plone.app.z3cform-4.1.0/plone/app/z3cform/views.py
--rw-r--r--   0 maurits    (501) staff       (20)     2959 2023-04-26 21:55:45.000000 plone.app.z3cform-4.1.0/plone/app/z3cform/widget.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-26 21:55:46.669884 plone.app.z3cform-4.1.0/plone/app/z3cform/widgets/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-04-26 21:55:45.000000 plone.app.z3cform-4.1.0/plone/app/z3cform/widgets/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     1807 2023-04-26 21:55:45.000000 plone.app.z3cform-4.1.0/plone/app/z3cform/widgets/base.py
--rw-r--r--   0 maurits    (501) staff       (20)     4970 2023-04-26 21:55:45.000000 plone.app.z3cform-4.1.0/plone/app/z3cform/widgets/datetime.py
--rw-r--r--   0 maurits    (501) staff       (20)     1978 2023-04-26 21:55:45.000000 plone.app.z3cform-4.1.0/plone/app/z3cform/widgets/link.py
--rw-r--r--   0 maurits    (501) staff       (20)     9625 2023-04-26 21:55:45.000000 plone.app.z3cform-4.1.0/plone/app/z3cform/widgets/patterns.py
--rw-r--r--   0 maurits    (501) staff       (20)     2712 2023-04-26 21:55:45.000000 plone.app.z3cform-4.1.0/plone/app/z3cform/widgets/querystring.py
--rw-r--r--   0 maurits    (501) staff       (20)     8804 2023-04-26 21:55:45.000000 plone.app.z3cform-4.1.0/plone/app/z3cform/widgets/relateditems.py
--rw-r--r--   0 maurits    (501) staff       (20)     6381 2023-04-26 21:55:45.000000 plone.app.z3cform-4.1.0/plone/app/z3cform/widgets/richtext.py
--rw-r--r--   0 maurits    (501) staff       (20)    11155 2023-04-26 21:55:45.000000 plone.app.z3cform-4.1.0/plone/app/z3cform/widgets/select.py
--rw-r--r--   0 maurits    (501) staff       (20)     2962 2023-04-26 21:55:45.000000 plone.app.z3cform-4.1.0/plone/app/z3cform/widgets/singlecheckbox.py
--rw-r--r--   0 maurits    (501) staff       (20)     9303 2023-04-26 21:55:45.000000 plone.app.z3cform-4.1.0/plone/app/z3cform/widgets.zcml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-26 21:55:46.671621 plone.app.z3cform-4.1.0/plone/app/z3cform/wysiwyg/
--rw-r--r--   0 maurits    (501) staff       (20)      919 2023-04-26 21:55:45.000000 plone.app.z3cform-4.1.0/plone/app/z3cform/wysiwyg/README.rst
--rw-r--r--   0 maurits    (501) staff       (20)      127 2023-04-26 21:55:45.000000 plone.app.z3cform-4.1.0/plone/app/z3cform/wysiwyg/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)      639 2023-04-26 21:55:45.000000 plone.app.z3cform-4.1.0/plone/app/z3cform/wysiwyg/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     1693 2023-04-26 21:55:45.000000 plone.app.z3cform-4.1.0/plone/app/z3cform/wysiwyg/widget.py
--rw-r--r--   0 maurits    (501) staff       (20)      601 2023-04-26 21:55:45.000000 plone.app.z3cform-4.1.0/plone/app/z3cform/wysiwyg/wysiwyg_display.pt
--rw-r--r--   0 maurits    (501) staff       (20)     1048 2023-04-26 21:55:45.000000 plone.app.z3cform-4.1.0/plone/app/z3cform/wysiwyg/wysiwyg_input.pt
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-26 21:55:46.651230 plone.app.z3cform-4.1.0/plone.app.z3cform.egg-info/
--rw-r--r--   0 maurits    (501) staff       (20)    48242 2023-04-26 21:55:46.000000 plone.app.z3cform-4.1.0/plone.app.z3cform.egg-info/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)     3335 2023-04-26 21:55:46.000000 plone.app.z3cform-4.1.0/plone.app.z3cform.egg-info/SOURCES.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2023-04-26 21:55:46.000000 plone.app.z3cform-4.1.0/plone.app.z3cform.egg-info/dependency_links.txt
--rw-r--r--   0 maurits    (501) staff       (20)       16 2023-04-26 21:55:46.000000 plone.app.z3cform-4.1.0/plone.app.z3cform.egg-info/namespace_packages.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2023-04-26 21:55:46.000000 plone.app.z3cform-4.1.0/plone.app.z3cform.egg-info/not-zip-safe
--rw-r--r--   0 maurits    (501) staff       (20)      578 2023-04-26 21:55:46.000000 plone.app.z3cform-4.1.0/plone.app.z3cform.egg-info/requires.txt
--rw-r--r--   0 maurits    (501) staff       (20)        6 2023-04-26 21:55:46.000000 plone.app.z3cform-4.1.0/plone.app.z3cform.egg-info/top_level.txt
--rw-r--r--   0 maurits    (501) staff       (20)     1692 2023-04-26 21:55:45.000000 plone.app.z3cform-4.1.0/pyproject.toml
--rw-r--r--   0 maurits    (501) staff       (20)      242 2023-04-26 21:55:46.672532 plone.app.z3cform-4.1.0/setup.cfg
--rw-r--r--   0 maurits    (501) staff       (20)     2625 2023-04-26 21:55:45.000000 plone.app.z3cform-4.1.0/setup.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-22 21:11:04.421108 plone.app.z3cform-4.2.0/
+-rw-r--r--   0 maurits    (501) staff       (20)    25256 2023-05-22 21:11:03.000000 plone.app.z3cform-4.2.0/CHANGES.rst
+-rw-r--r--   0 maurits    (501) staff       (20)       70 2023-05-22 21:11:03.000000 plone.app.z3cform-4.2.0/CONTRIBUTING.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      146 2023-05-22 21:11:03.000000 plone.app.z3cform-4.2.0/MANIFEST.in
+-rw-r--r--   0 maurits    (501) staff       (20)    48509 2023-05-22 21:11:04.421269 plone.app.z3cform-4.2.0/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)    13825 2023-05-22 21:11:03.000000 plone.app.z3cform-4.2.0/README.rst
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-22 21:11:04.395281 plone.app.z3cform-4.2.0/docs/
+-rw-r--r--   0 maurits    (501) staff       (20)    12282 2023-05-22 21:11:03.000000 plone.app.z3cform-4.2.0/docs/LICENSE.GPL
+-rw-r--r--   0 maurits    (501) staff       (20)      749 2023-05-22 21:11:03.000000 plone.app.z3cform-4.2.0/docs/LICENSE.txt
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-22 21:11:04.395588 plone.app.z3cform-4.2.0/plone/
+-rw-r--r--   0 maurits    (501) staff       (20)       56 2023-05-22 21:11:03.000000 plone.app.z3cform-4.2.0/plone/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-22 21:11:04.398296 plone.app.z3cform-4.2.0/plone/app/
+-rw-r--r--   0 maurits    (501) staff       (20)       56 2023-05-22 21:11:03.000000 plone.app.z3cform-4.2.0/plone/app/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-22 21:11:04.403316 plone.app.z3cform-4.2.0/plone/app/z3cform/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2023-05-22 21:11:03.000000 plone.app.z3cform-4.2.0/plone/app/z3cform/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2763 2023-05-22 21:11:03.000000 plone.app.z3cform-4.2.0/plone/app/z3cform/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)    18540 2023-05-22 21:11:03.000000 plone.app.z3cform-4.2.0/plone/app/z3cform/converters.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1310 2023-05-22 21:11:03.000000 plone.app.z3cform-4.2.0/plone/app/z3cform/converters.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)      724 2023-05-22 21:11:03.000000 plone.app.z3cform-4.2.0/plone/app/z3cform/csrf.py
+-rw-r--r--   0 maurits    (501) staff       (20)      110 2023-05-22 21:11:03.000000 plone.app.z3cform-4.2.0/plone/app/z3cform/factories.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2349 2023-05-22 21:11:03.000000 plone.app.z3cform-4.2.0/plone/app/z3cform/inline_validation.py
+-rw-r--r--   0 maurits    (501) staff       (20)     7482 2023-05-22 21:11:03.000000 plone.app.z3cform-4.2.0/plone/app/z3cform/inline_validation.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     2500 2023-05-22 21:11:03.000000 plone.app.z3cform-4.2.0/plone/app/z3cform/interfaces.py
+-rw-r--r--   0 maurits    (501) staff       (20)      212 2023-05-22 21:11:03.000000 plone.app.z3cform-4.2.0/plone/app/z3cform/layout.py
+-rw-r--r--   0 maurits    (501) staff       (20)      152 2023-05-22 21:11:03.000000 plone.app.z3cform-4.2.0/plone/app/z3cform/overrides.zcml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-22 21:11:04.391822 plone.app.z3cform-4.2.0/plone/app/z3cform/profiles/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-22 21:11:04.403968 plone.app.z3cform-4.2.0/plone/app/z3cform/profiles/default/
+-rw-r--r--   0 maurits    (501) staff       (20)      163 2023-05-22 21:11:03.000000 plone.app.z3cform-4.2.0/plone/app/z3cform/profiles/default/browserlayer.xml
+-rw-r--r--   0 maurits    (501) staff       (20)       85 2023-05-22 21:11:03.000000 plone.app.z3cform-4.2.0/plone/app/z3cform/profiles/default/metadata.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      635 2023-05-22 21:11:03.000000 plone.app.z3cform-4.2.0/plone/app/z3cform/profiles.zcml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-22 21:11:04.412739 plone.app.z3cform-4.2.0/plone/app/z3cform/templates/
+-rw-r--r--   0 maurits    (501) staff       (20)     1013 2023-05-22 21:11:03.000000 plone.app.z3cform-4.2.0/plone/app/z3cform/templates/ajaxselect_display.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     3643 2023-05-22 21:11:03.000000 plone.app.z3cform-4.2.0/plone/app/z3cform/templates/checkbox_input.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      140 2023-05-22 21:11:03.000000 plone.app.z3cform-4.2.0/plone/app/z3cform/templates/contentprovider-widget.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      209 2023-05-22 21:11:03.000000 plone.app.z3cform-4.2.0/plone/app/z3cform/templates/error.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     4806 2023-05-22 21:11:03.000000 plone.app.z3cform-4.2.0/plone/app/z3cform/templates/file_input.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      829 2023-05-22 21:11:03.000000 plone.app.z3cform-4.2.0/plone/app/z3cform/templates/form.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     4798 2023-05-22 21:11:03.000000 plone.app.z3cform-4.2.0/plone/app/z3cform/templates/image_input.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      677 2023-05-22 21:11:03.000000 plone.app.z3cform-4.2.0/plone/app/z3cform/templates/layout.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     3547 2023-05-22 21:11:03.000000 plone.app.z3cform-4.2.0/plone/app/z3cform/templates/link_input.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     9551 2023-05-22 21:11:03.000000 plone.app.z3cform-4.2.0/plone/app/z3cform/templates/macros.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     4033 2023-05-22 21:11:03.000000 plone.app.z3cform-4.2.0/plone/app/z3cform/templates/multi_input.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     1861 2023-05-22 21:11:03.000000 plone.app.z3cform-4.2.0/plone/app/z3cform/templates/object_input.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     5486 2023-05-22 21:11:03.000000 plone.app.z3cform-4.2.0/plone/app/z3cform/templates/orderedselect_input.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     1448 2023-05-22 21:11:03.000000 plone.app.z3cform-4.2.0/plone/app/z3cform/templates/password_input.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      650 2023-05-22 21:11:03.000000 plone.app.z3cform-4.2.0/plone/app/z3cform/templates/radio_input.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     1418 2023-05-22 21:11:03.000000 plone.app.z3cform-4.2.0/plone/app/z3cform/templates/radio_input_single.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     1869 2023-05-22 21:11:03.000000 plone.app.z3cform-4.2.0/plone/app/z3cform/templates/relateditems_display.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     1937 2023-05-22 21:11:03.000000 plone.app.z3cform-4.2.0/plone/app/z3cform/templates/select_input.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      976 2023-05-22 21:11:03.000000 plone.app.z3cform-4.2.0/plone/app/z3cform/templates/singlecheckbox.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      765 2023-05-22 21:11:03.000000 plone.app.z3cform-4.2.0/plone/app/z3cform/templates/singlecheckboxbool_display.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     1357 2023-05-22 21:11:03.000000 plone.app.z3cform-4.2.0/plone/app/z3cform/templates/singlecheckboxbool_hidden.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     4046 2023-05-22 21:11:03.000000 plone.app.z3cform-4.2.0/plone/app/z3cform/templates/singlecheckboxbool_input.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     1335 2023-05-22 21:11:03.000000 plone.app.z3cform-4.2.0/plone/app/z3cform/templates/submit_input.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     1574 2023-05-22 21:11:03.000000 plone.app.z3cform-4.2.0/plone/app/z3cform/templates/text_input.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     1414 2023-05-22 21:11:03.000000 plone.app.z3cform-4.2.0/plone/app/z3cform/templates/textarea_input.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     3703 2023-05-22 21:11:03.000000 plone.app.z3cform-4.2.0/plone/app/z3cform/templates/textfield_widget_input.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     1356 2023-05-22 21:11:03.000000 plone.app.z3cform-4.2.0/plone/app/z3cform/templates/textlines_input.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     1812 2023-05-22 21:11:03.000000 plone.app.z3cform-4.2.0/plone/app/z3cform/templates/widget.pt
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-22 21:11:04.416032 plone.app.z3cform-4.2.0/plone/app/z3cform/tests/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2023-05-22 21:11:03.000000 plone.app.z3cform-4.2.0/plone/app/z3cform/tests/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2421 2023-05-22 21:11:03.000000 plone.app.z3cform-4.2.0/plone/app/z3cform/tests/example.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1139 2023-05-22 21:11:03.000000 plone.app.z3cform-4.2.0/plone/app/z3cform/tests/layer.py
+-rw-r--r--   0 maurits    (501) staff       (20)      907 2023-05-22 21:11:03.000000 plone.app.z3cform-4.2.0/plone/app/z3cform/tests/test_csrf.py
+-rw-r--r--   0 maurits    (501) staff       (20)    17512 2023-05-22 21:11:03.000000 plone.app.z3cform-4.2.0/plone/app/z3cform/tests/test_patterns.py
+-rw-r--r--   0 maurits    (501) staff       (20)     4921 2023-05-22 21:11:03.000000 plone.app.z3cform-4.2.0/plone/app/z3cform/tests/test_utils.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1349 2023-05-22 21:11:03.000000 plone.app.z3cform-4.2.0/plone/app/z3cform/tests/test_widget.py
+-rw-r--r--   0 maurits    (501) staff       (20)    67618 2023-05-22 21:11:03.000000 plone.app.z3cform-4.2.0/plone/app/z3cform/tests/test_widgets.py
+-rw-r--r--   0 maurits    (501) staff       (20)      776 2023-05-22 21:11:03.000000 plone.app.z3cform-4.2.0/plone/app/z3cform/tests/testing.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     2208 2023-05-22 21:11:03.000000 plone.app.z3cform-4.2.0/plone/app/z3cform/tests/tests.py
+-rw-r--r--   0 maurits    (501) staff       (20)     6163 2023-05-22 21:11:03.000000 plone.app.z3cform-4.2.0/plone/app/z3cform/utils.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2739 2023-05-22 21:11:03.000000 plone.app.z3cform-4.2.0/plone/app/z3cform/views.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2959 2023-05-22 21:11:03.000000 plone.app.z3cform-4.2.0/plone/app/z3cform/widget.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-22 21:11:04.419008 plone.app.z3cform-4.2.0/plone/app/z3cform/widgets/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2023-05-22 21:11:03.000000 plone.app.z3cform-4.2.0/plone/app/z3cform/widgets/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1807 2023-05-22 21:11:03.000000 plone.app.z3cform-4.2.0/plone/app/z3cform/widgets/base.py
+-rw-r--r--   0 maurits    (501) staff       (20)     4970 2023-05-22 21:11:03.000000 plone.app.z3cform-4.2.0/plone/app/z3cform/widgets/datetime.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1978 2023-05-22 21:11:03.000000 plone.app.z3cform-4.2.0/plone/app/z3cform/widgets/link.py
+-rw-r--r--   0 maurits    (501) staff       (20)     9722 2023-05-22 21:11:03.000000 plone.app.z3cform-4.2.0/plone/app/z3cform/widgets/patterns.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2712 2023-05-22 21:11:03.000000 plone.app.z3cform-4.2.0/plone/app/z3cform/widgets/querystring.py
+-rw-r--r--   0 maurits    (501) staff       (20)     8804 2023-05-22 21:11:03.000000 plone.app.z3cform-4.2.0/plone/app/z3cform/widgets/relateditems.py
+-rw-r--r--   0 maurits    (501) staff       (20)     6381 2023-05-22 21:11:03.000000 plone.app.z3cform-4.2.0/plone/app/z3cform/widgets/richtext.py
+-rw-r--r--   0 maurits    (501) staff       (20)    11155 2023-05-22 21:11:03.000000 plone.app.z3cform-4.2.0/plone/app/z3cform/widgets/select.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2962 2023-05-22 21:11:03.000000 plone.app.z3cform-4.2.0/plone/app/z3cform/widgets/singlecheckbox.py
+-rw-r--r--   0 maurits    (501) staff       (20)     9303 2023-05-22 21:11:03.000000 plone.app.z3cform-4.2.0/plone/app/z3cform/widgets.zcml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-22 21:11:04.420856 plone.app.z3cform-4.2.0/plone/app/z3cform/wysiwyg/
+-rw-r--r--   0 maurits    (501) staff       (20)      919 2023-05-22 21:11:03.000000 plone.app.z3cform-4.2.0/plone/app/z3cform/wysiwyg/README.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      127 2023-05-22 21:11:03.000000 plone.app.z3cform-4.2.0/plone/app/z3cform/wysiwyg/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)      639 2023-05-22 21:11:03.000000 plone.app.z3cform-4.2.0/plone/app/z3cform/wysiwyg/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     1693 2023-05-22 21:11:03.000000 plone.app.z3cform-4.2.0/plone/app/z3cform/wysiwyg/widget.py
+-rw-r--r--   0 maurits    (501) staff       (20)      601 2023-05-22 21:11:03.000000 plone.app.z3cform-4.2.0/plone/app/z3cform/wysiwyg/wysiwyg_display.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     1048 2023-05-22 21:11:03.000000 plone.app.z3cform-4.2.0/plone/app/z3cform/wysiwyg/wysiwyg_input.pt
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-22 21:11:04.397947 plone.app.z3cform-4.2.0/plone.app.z3cform.egg-info/
+-rw-r--r--   0 maurits    (501) staff       (20)    48509 2023-05-22 21:11:04.000000 plone.app.z3cform-4.2.0/plone.app.z3cform.egg-info/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)     3335 2023-05-22 21:11:04.000000 plone.app.z3cform-4.2.0/plone.app.z3cform.egg-info/SOURCES.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2023-05-22 21:11:04.000000 plone.app.z3cform-4.2.0/plone.app.z3cform.egg-info/dependency_links.txt
+-rw-r--r--   0 maurits    (501) staff       (20)       16 2023-05-22 21:11:04.000000 plone.app.z3cform-4.2.0/plone.app.z3cform.egg-info/namespace_packages.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2023-05-22 21:11:04.000000 plone.app.z3cform-4.2.0/plone.app.z3cform.egg-info/not-zip-safe
+-rw-r--r--   0 maurits    (501) staff       (20)      578 2023-05-22 21:11:04.000000 plone.app.z3cform-4.2.0/plone.app.z3cform.egg-info/requires.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        6 2023-05-22 21:11:04.000000 plone.app.z3cform-4.2.0/plone.app.z3cform.egg-info/top_level.txt
+-rw-r--r--   0 maurits    (501) staff       (20)     1692 2023-05-22 21:11:03.000000 plone.app.z3cform-4.2.0/pyproject.toml
+-rw-r--r--   0 maurits    (501) staff       (20)      242 2023-05-22 21:11:04.421806 plone.app.z3cform-4.2.0/setup.cfg
+-rw-r--r--   0 maurits    (501) staff       (20)     2625 2023-05-22 21:11:03.000000 plone.app.z3cform-4.2.0/setup.py
```

### Comparing `plone.app.z3cform-4.1.0/CHANGES.rst` & `plone.app.z3cform-4.2.0/CHANGES.rst`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,32 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+4.2.0 (2023-05-22)
+------------------
+
+New features:
+
+
+- Move storage utility to plone.namedfile
+  to break a dependency cycle between the two.
+  [gforcada] (#3764)
+
+
+Bug fixes:
+
+
+- Remove invalid unicode control characters for `TextareaWidget`
+  [petschki] (#167)
+
+
 4.1.0 (2023-04-26)
 ------------------
 
 New features:
 
 
 - Merge utils and base classes from  ``plone.app.widgets`` and do not depend
```

### Comparing `plone.app.z3cform-4.1.0/PKG-INFO` & `plone.app.z3cform-4.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plone.app.z3cform
-Version: 4.1.0
+Version: 4.2.0
 Summary: A collection of widgets, templates and other components for use with z3c.form and Plone
 Home-page: https://pypi.org/project/plone.app.z3cform
 Author: Plone Foundation
 Author-email: plone-developers@lists.sourceforge.net
 License: GPL
 Keywords: zope plone form widget template
 Classifier: Development Status :: 5 - Production/Stable
@@ -677,14 +677,32 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+4.2.0 (2023-05-22)
+------------------
+
+New features:
+
+
+- Move storage utility to plone.namedfile
+  to break a dependency cycle between the two.
+  [gforcada] (#3764)
+
+
+Bug fixes:
+
+
+- Remove invalid unicode control characters for `TextareaWidget`
+  [petschki] (#167)
+
+
 4.1.0 (2023-04-26)
 ------------------
 
 New features:
 
 
 - Merge utils and base classes from  ``plone.app.widgets`` and do not depend
```

### Comparing `plone.app.z3cform-4.1.0/README.rst` & `plone.app.z3cform-4.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.1.0/docs/LICENSE.GPL` & `plone.app.z3cform-4.2.0/docs/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.1.0/docs/LICENSE.txt` & `plone.app.z3cform-4.2.0/docs/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.1.0/plone/app/z3cform/configure.zcml` & `plone.app.z3cform-4.2.0/plone/app/z3cform/configure.zcml`

 * *Files 9% similar despite different names*

```diff
@@ -87,14 +87,8 @@
   <adapter
       factory=".views.ErrorViewTemplate"
       provides="zope.pagetemplate.interfaces.IPageTemplate"
       for="z3c.form.interfaces.IErrorViewSnippet
            .interfaces.IPloneFormLayer"
       />
 
-  <utility
-      factory=".factories.Zope2FileUploadStorable"
-      provides="plone.namedfile.interfaces.IStorage"
-      name="ZPublisher.HTTPRequest.FileUpload"
-      />
-
 </configure>
```

### Comparing `plone.app.z3cform-4.1.0/plone/app/z3cform/converters.py` & `plone.app.z3cform-4.2.0/plone/app/z3cform/converters.py`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.1.0/plone/app/z3cform/converters.zcml` & `plone.app.z3cform-4.2.0/plone/app/z3cform/converters.zcml`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.1.0/plone/app/z3cform/csrf.py` & `plone.app.z3cform-4.2.0/plone/app/z3cform/csrf.py`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.1.0/plone/app/z3cform/inline_validation.py` & `plone.app.z3cform-4.2.0/plone/app/z3cform/inline_validation.py`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.1.0/plone/app/z3cform/inline_validation.rst` & `plone.app.z3cform-4.2.0/plone/app/z3cform/inline_validation.rst`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.1.0/plone/app/z3cform/interfaces.py` & `plone.app.z3cform-4.2.0/plone/app/z3cform/interfaces.py`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.1.0/plone/app/z3cform/profiles.zcml` & `plone.app.z3cform-4.2.0/plone/app/z3cform/profiles.zcml`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.1.0/plone/app/z3cform/templates/ajaxselect_display.pt` & `plone.app.z3cform-4.2.0/plone/app/z3cform/templates/ajaxselect_display.pt`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.1.0/plone/app/z3cform/templates/checkbox_input.pt` & `plone.app.z3cform-4.2.0/plone/app/z3cform/templates/checkbox_input.pt`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.1.0/plone/app/z3cform/templates/file_input.pt` & `plone.app.z3cform-4.2.0/plone/app/z3cform/templates/file_input.pt`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.1.0/plone/app/z3cform/templates/form.pt` & `plone.app.z3cform-4.2.0/plone/app/z3cform/templates/form.pt`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.1.0/plone/app/z3cform/templates/image_input.pt` & `plone.app.z3cform-4.2.0/plone/app/z3cform/templates/image_input.pt`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.1.0/plone/app/z3cform/templates/layout.pt` & `plone.app.z3cform-4.2.0/plone/app/z3cform/templates/layout.pt`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.1.0/plone/app/z3cform/templates/link_input.pt` & `plone.app.z3cform-4.2.0/plone/app/z3cform/templates/link_input.pt`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.1.0/plone/app/z3cform/templates/macros.pt` & `plone.app.z3cform-4.2.0/plone/app/z3cform/templates/macros.pt`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.1.0/plone/app/z3cform/templates/multi_input.pt` & `plone.app.z3cform-4.2.0/plone/app/z3cform/templates/multi_input.pt`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.1.0/plone/app/z3cform/templates/object_input.pt` & `plone.app.z3cform-4.2.0/plone/app/z3cform/templates/object_input.pt`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.1.0/plone/app/z3cform/templates/orderedselect_input.pt` & `plone.app.z3cform-4.2.0/plone/app/z3cform/templates/orderedselect_input.pt`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.1.0/plone/app/z3cform/templates/password_input.pt` & `plone.app.z3cform-4.2.0/plone/app/z3cform/templates/password_input.pt`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.1.0/plone/app/z3cform/templates/radio_input.pt` & `plone.app.z3cform-4.2.0/plone/app/z3cform/templates/radio_input.pt`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.1.0/plone/app/z3cform/templates/radio_input_single.pt` & `plone.app.z3cform-4.2.0/plone/app/z3cform/templates/radio_input_single.pt`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.1.0/plone/app/z3cform/templates/relateditems_display.pt` & `plone.app.z3cform-4.2.0/plone/app/z3cform/templates/relateditems_display.pt`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.1.0/plone/app/z3cform/templates/select_input.pt` & `plone.app.z3cform-4.2.0/plone/app/z3cform/templates/select_input.pt`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.1.0/plone/app/z3cform/templates/singlecheckbox.pt` & `plone.app.z3cform-4.2.0/plone/app/z3cform/templates/singlecheckbox.pt`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.1.0/plone/app/z3cform/templates/singlecheckboxbool_display.pt` & `plone.app.z3cform-4.2.0/plone/app/z3cform/templates/singlecheckboxbool_display.pt`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.1.0/plone/app/z3cform/templates/singlecheckboxbool_hidden.pt` & `plone.app.z3cform-4.2.0/plone/app/z3cform/templates/singlecheckboxbool_hidden.pt`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.1.0/plone/app/z3cform/templates/singlecheckboxbool_input.pt` & `plone.app.z3cform-4.2.0/plone/app/z3cform/templates/singlecheckboxbool_input.pt`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.1.0/plone/app/z3cform/templates/submit_input.pt` & `plone.app.z3cform-4.2.0/plone/app/z3cform/templates/submit_input.pt`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.1.0/plone/app/z3cform/templates/text_input.pt` & `plone.app.z3cform-4.2.0/plone/app/z3cform/templates/text_input.pt`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.1.0/plone/app/z3cform/templates/textarea_input.pt` & `plone.app.z3cform-4.2.0/plone/app/z3cform/templates/textarea_input.pt`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.1.0/plone/app/z3cform/templates/textfield_widget_input.pt` & `plone.app.z3cform-4.2.0/plone/app/z3cform/templates/textfield_widget_input.pt`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.1.0/plone/app/z3cform/templates/textlines_input.pt` & `plone.app.z3cform-4.2.0/plone/app/z3cform/templates/textlines_input.pt`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.1.0/plone/app/z3cform/templates/widget.pt` & `plone.app.z3cform-4.2.0/plone/app/z3cform/templates/widget.pt`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.1.0/plone/app/z3cform/tests/example.py` & `plone.app.z3cform-4.2.0/plone/app/z3cform/tests/example.py`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.1.0/plone/app/z3cform/tests/layer.py` & `plone.app.z3cform-4.2.0/plone/app/z3cform/tests/layer.py`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.1.0/plone/app/z3cform/tests/test_csrf.py` & `plone.app.z3cform-4.2.0/plone/app/z3cform/tests/test_csrf.py`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.1.0/plone/app/z3cform/tests/test_patterns.py` & `plone.app.z3cform-4.2.0/plone/app/z3cform/tests/test_patterns.py`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.1.0/plone/app/z3cform/tests/test_utils.py` & `plone.app.z3cform-4.2.0/plone/app/z3cform/tests/test_utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -147,7 +147,16 @@
         # Here, different transport protocols are used. Returning False.
         self.assertTrue(
             not is_same_domain(
                 "https://plone.org",
                 "http://plone.org",
             )
         )
+
+    def test_unicode_control_character_removal(self):
+        from plone.app.z3cform.utils import remove_invalid_xml_characters
+
+        for x in range(32):
+            if x in (9, 10, 13):
+                self.assertTrue(remove_invalid_xml_characters(chr(x)) == chr(x))
+            else:
+                self.assertTrue(remove_invalid_xml_characters(chr(x)) == "")
```

### Comparing `plone.app.z3cform-4.1.0/plone/app/z3cform/tests/test_widget.py` & `plone.app.z3cform-4.2.0/plone/app/z3cform/tests/test_widget.py`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.1.0/plone/app/z3cform/tests/test_widgets.py` & `plone.app.z3cform-4.2.0/plone/app/z3cform/tests/test_widgets.py`

 * *Files 0% similar despite different names*

```diff
@@ -1696,14 +1696,30 @@
         widget = FieldWidget(self.field, RichTextWidget(self.request))
         # set the context so we can get tinymce settings
         widget.context = self.portal
         widget.value = RichTextValue("Lorem ipsum \u2026")
         base_args = widget._base_args()
         self.assertEqual(base_args["value"], "Lorem ipsum \u2026")
 
+    def test_unicode_control_characters_value(self):
+        # lxml doesn't allow unicode control characters.
+        # see
+        from plone.app.textfield.value import RichTextValue
+        from plone.app.z3cform.widgets.richtext import RichTextWidget
+
+        widget = FieldWidget(self.field, RichTextWidget(self.request))
+        # set the context so we can get tinymce settings
+        widget.context = self.portal
+        widget.value = RichTextValue("Lorem \u0000 ip\u001Fsum\n\u0002 dolorem\r\t")
+        widget.mode = "input"
+        self.assertIn(
+            ">Lorem  ipsum\n dolorem&#13;\t</textarea>",
+            widget.render(),
+        )
+
     def _set_mimetypes(self, default="text/html", allowed=("text/html")):
         """Set portal's mimetype settings."""
         if IMarkupSchema:
             registry = getUtility(IRegistry)
             self.settings = registry.forInterface(
                 IMarkupSchema,
                 prefix="plone",
```

### Comparing `plone.app.z3cform-4.1.0/plone/app/z3cform/tests/testing.zcml` & `plone.app.z3cform-4.2.0/plone/app/z3cform/tests/testing.zcml`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.1.0/plone/app/z3cform/tests/tests.py` & `plone.app.z3cform-4.2.0/plone/app/z3cform/tests/tests.py`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.1.0/plone/app/z3cform/utils.py` & `plone.app.z3cform-4.2.0/plone/app/z3cform/utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -177,7 +177,24 @@
     elif hasattr(context, "absolute_url"):
         url = context.absolute_url
         if callable(url):
             url = url()
     else:
         url = get_portal_url(context)
     return url
+
+
+# Invalid XML unicode control characters
+# NOTE: these control characters are allowed:
+# chr(9) = "\t"
+# chr(10) = "\n"
+# chr(13) = "\r"
+
+_unicode_ctl_chr_map = dict.fromkeys([x for x in range(32) if x not in (9, 10, 13)])
+
+
+def remove_invalid_xml_characters(txt):
+    # remove occurrences of the unicode "control characters"
+    # as they are invalid XML characters
+    # see https://en.wikipedia.org/wiki/Valid_characters_in_XML and
+    # https://en.wikipedia.org/wiki/C0_and_C1_control_codes
+    return txt.translate(_unicode_ctl_chr_map)
```

### Comparing `plone.app.z3cform-4.1.0/plone/app/z3cform/views.py` & `plone.app.z3cform-4.2.0/plone/app/z3cform/views.py`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.1.0/plone/app/z3cform/widget.py` & `plone.app.z3cform-4.2.0/plone/app/z3cform/widget.py`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.1.0/plone/app/z3cform/widgets/base.py` & `plone.app.z3cform-4.2.0/plone/app/z3cform/widgets/base.py`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.1.0/plone/app/z3cform/widgets/datetime.py` & `plone.app.z3cform-4.2.0/plone/app/z3cform/widgets/datetime.py`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.1.0/plone/app/z3cform/widgets/link.py` & `plone.app.z3cform-4.2.0/plone/app/z3cform/widgets/link.py`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.1.0/plone/app/z3cform/widgets/patterns.py` & `plone.app.z3cform-4.2.0/plone/app/z3cform/widgets/patterns.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from lxml import etree
+from plone.app.z3cform.utils import remove_invalid_xml_characters
 
 import collections
 import json
 
 
 def el_attrib(name):
     """Helper property methods to get/set/delete element property.
@@ -325,14 +326,14 @@
         return self.el.text
 
     def _set_value(self, value):
         """
         :param value: Set value of element.
         :type value: string
         """
-        self.el.text = value
+        self.el.text = remove_invalid_xml_characters(value)
 
     def _del_value(self):
         """Set empty string as value of element."""
         self.el.text = ""
 
     value = property(_get_value, _set_value, _del_value)
```

### Comparing `plone.app.z3cform-4.1.0/plone/app/z3cform/widgets/querystring.py` & `plone.app.z3cform-4.2.0/plone/app/z3cform/widgets/querystring.py`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.1.0/plone/app/z3cform/widgets/relateditems.py` & `plone.app.z3cform-4.2.0/plone/app/z3cform/widgets/relateditems.py`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.1.0/plone/app/z3cform/widgets/richtext.py` & `plone.app.z3cform-4.2.0/plone/app/z3cform/widgets/richtext.py`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.1.0/plone/app/z3cform/widgets/select.py` & `plone.app.z3cform-4.2.0/plone/app/z3cform/widgets/select.py`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.1.0/plone/app/z3cform/widgets/singlecheckbox.py` & `plone.app.z3cform-4.2.0/plone/app/z3cform/widgets/singlecheckbox.py`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.1.0/plone/app/z3cform/widgets.zcml` & `plone.app.z3cform-4.2.0/plone/app/z3cform/widgets.zcml`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.1.0/plone/app/z3cform/wysiwyg/README.rst` & `plone.app.z3cform-4.2.0/plone/app/z3cform/wysiwyg/README.rst`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.1.0/plone/app/z3cform/wysiwyg/configure.zcml` & `plone.app.z3cform-4.2.0/plone/app/z3cform/wysiwyg/configure.zcml`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.1.0/plone/app/z3cform/wysiwyg/widget.py` & `plone.app.z3cform-4.2.0/plone/app/z3cform/wysiwyg/widget.py`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.1.0/plone/app/z3cform/wysiwyg/wysiwyg_display.pt` & `plone.app.z3cform-4.2.0/plone/app/z3cform/wysiwyg/wysiwyg_display.pt`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.1.0/plone/app/z3cform/wysiwyg/wysiwyg_input.pt` & `plone.app.z3cform-4.2.0/plone/app/z3cform/wysiwyg/wysiwyg_input.pt`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.1.0/plone.app.z3cform.egg-info/PKG-INFO` & `plone.app.z3cform-4.2.0/plone.app.z3cform.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plone.app.z3cform
-Version: 4.1.0
+Version: 4.2.0
 Summary: A collection of widgets, templates and other components for use with z3c.form and Plone
 Home-page: https://pypi.org/project/plone.app.z3cform
 Author: Plone Foundation
 Author-email: plone-developers@lists.sourceforge.net
 License: GPL
 Keywords: zope plone form widget template
 Classifier: Development Status :: 5 - Production/Stable
@@ -677,14 +677,32 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+4.2.0 (2023-05-22)
+------------------
+
+New features:
+
+
+- Move storage utility to plone.namedfile
+  to break a dependency cycle between the two.
+  [gforcada] (#3764)
+
+
+Bug fixes:
+
+
+- Remove invalid unicode control characters for `TextareaWidget`
+  [petschki] (#167)
+
+
 4.1.0 (2023-04-26)
 ------------------
 
 New features:
 
 
 - Merge utils and base classes from  ``plone.app.widgets`` and do not depend
```

### Comparing `plone.app.z3cform-4.1.0/plone.app.z3cform.egg-info/SOURCES.txt` & `plone.app.z3cform-4.2.0/plone.app.z3cform.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.1.0/plone.app.z3cform.egg-info/requires.txt` & `plone.app.z3cform-4.2.0/plone.app.z3cform.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.1.0/pyproject.toml` & `plone.app.z3cform-4.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.1.0/setup.py` & `plone.app.z3cform-4.2.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import os
 
 
 def read(*rnames):
     return open(os.path.join(os.path.dirname(__file__), *rnames)).read()
 
 
-version = "4.1.0"
+version = "4.2.0"
 
 long_description = (
     read("README.rst")
     + "\n"
     + read("plone", "app", "z3cform", "wysiwyg", "README.rst")
     + "\n"
     + read("plone", "app", "z3cform", "inline_validation.rst")
```

