# Comparing `tmp/imio.smartweb.common-1.1.6.tar.gz` & `tmp/imio.smartweb.common-1.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imio.smartweb.common-1.1.6.tar", last modified: Fri Apr 14 07:20:45 2023, max compression
+gzip compressed data, was "imio.smartweb.common-1.1.7.tar", last modified: Mon May 22 07:06:13 2023, max compression
```

## Comparing `imio.smartweb.common-1.1.6.tar` & `imio.smartweb.common-1.1.7.tar`

### file list

```diff
@@ -1,175 +1,178 @@
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-04-14 07:20:45.469639 imio.smartweb.common-1.1.6/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     5511 2023-04-14 07:20:44.000000 imio.smartweb.common-1.1.6/CHANGES.rst
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)       64 2023-04-14 07:20:44.000000 imio.smartweb.common-1.1.6/CONTRIBUTORS.rst
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      586 2023-04-14 07:20:44.000000 imio.smartweb.common-1.1.6/DEVELOP.rst
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)    18092 2023-04-14 07:20:44.000000 imio.smartweb.common-1.1.6/LICENSE.GPL
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      655 2023-04-14 07:20:44.000000 imio.smartweb.common-1.1.6/LICENSE.rst
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      106 2023-04-14 07:20:44.000000 imio.smartweb.common-1.1.6/MANIFEST.in
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     9849 2023-04-14 07:20:45.469639 imio.smartweb.common-1.1.6/PKG-INFO
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     3161 2023-04-14 07:20:44.000000 imio.smartweb.common-1.1.6/README.rst
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-04-14 07:20:45.441639 imio.smartweb.common-1.1.6/docs/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     7966 2023-04-14 07:20:44.000000 imio.smartweb.common-1.1.6/docs/conf.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)       83 2023-04-14 07:20:44.000000 imio.smartweb.common-1.1.6/docs/index.rst
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)       64 2023-04-14 07:20:44.000000 imio.smartweb.common-1.1.6/requirements.txt
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      518 2023-04-14 07:20:45.473639 imio.smartweb.common-1.1.6/setup.cfg
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2749 2023-04-14 07:20:44.000000 imio.smartweb.common-1.1.6/setup.py
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-04-14 07:20:45.381639 imio.smartweb.common-1.1.6/src/
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-04-14 07:20:45.441639 imio.smartweb.common-1.1.6/src/imio/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)       80 2023-04-14 07:20:44.000000 imio.smartweb.common-1.1.6/src/imio/__init__.py
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-04-14 07:20:45.445639 imio.smartweb.common-1.1.6/src/imio/smartweb/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)       80 2023-04-14 07:20:44.000000 imio.smartweb.common-1.1.6/src/imio/smartweb/__init__.py
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-04-14 07:20:45.449639 imio.smartweb.common-1.1.6/src/imio/smartweb/common/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2709 2023-04-14 07:20:44.000000 imio.smartweb.common-1.1.6/src/imio/smartweb/common/__init__.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      508 2023-04-14 07:20:44.000000 imio.smartweb.common-1.1.6/src/imio/smartweb/common/adapters.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      254 2023-04-14 07:20:44.000000 imio.smartweb.common-1.1.6/src/imio/smartweb/common/adapters.zcml
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-04-14 07:20:45.449639 imio.smartweb.common-1.1.6/src/imio/smartweb/common/behaviors/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)       24 2023-04-14 07:20:44.000000 imio.smartweb.common-1.1.6/src/imio/smartweb/common/behaviors/__init__.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      531 2023-04-14 07:20:44.000000 imio.smartweb.common-1.1.6/src/imio/smartweb/common/behaviors/configure.zcml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      805 2023-04-14 07:20:44.000000 imio.smartweb.common-1.1.6/src/imio/smartweb/common/behaviors/iam.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      804 2023-04-14 07:20:44.000000 imio.smartweb.common-1.1.6/src/imio/smartweb/common/behaviors/topics.py
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-04-14 07:20:45.453639 imio.smartweb.common-1.1.6/src/imio/smartweb/common/browser/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-04-14 07:20:44.000000 imio.smartweb.common-1.1.6/src/imio/smartweb/common/browser/__init__.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2452 2023-04-14 07:20:44.000000 imio.smartweb.common-1.1.6/src/imio/smartweb/common/browser/configure.zcml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      922 2023-04-14 07:20:44.000000 imio.smartweb.common-1.1.6/src/imio/smartweb/common/browser/cropping.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      151 2023-04-14 07:20:44.000000 imio.smartweb.common-1.1.6/src/imio/smartweb/common/browser/description.pt
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      517 2023-04-14 07:20:44.000000 imio.smartweb.common-1.1.6/src/imio/smartweb/common/browser/description.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     4164 2023-04-14 07:20:44.000000 imio.smartweb.common-1.1.6/src/imio/smartweb/common/browser/forms.py
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-04-14 07:20:45.453639 imio.smartweb.common-1.1.6/src/imio/smartweb/common/browser/overrides/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1818 2023-04-14 07:20:44.000000 imio.smartweb.common-1.1.6/src/imio/smartweb/common/browser/overrides/plone.app.z3cform.templates.widget.pt
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-04-14 07:20:45.453639 imio.smartweb.common-1.1.6/src/imio/smartweb/common/browser/privacy/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-04-14 07:20:44.000000 imio.smartweb.common-1.1.6/src/imio/smartweb/common/browser/privacy/__init__.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1062 2023-04-14 07:20:44.000000 imio.smartweb.common-1.1.6/src/imio/smartweb/common/browser/privacy/configure.zcml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1672 2023-04-14 07:20:44.000000 imio.smartweb.common-1.1.6/src/imio/smartweb/common/browser/privacy/form.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      205 2023-04-14 07:20:44.000000 imio.smartweb.common-1.1.6/src/imio/smartweb/common/browser/privacy/utils.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1815 2023-04-14 07:20:44.000000 imio.smartweb.common-1.1.6/src/imio/smartweb/common/browser/privacy/views.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      297 2023-04-14 07:20:44.000000 imio.smartweb.common-1.1.6/src/imio/smartweb/common/browser/scaling.py
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-04-14 07:20:45.457639 imio.smartweb.common-1.1.6/src/imio/smartweb/common/browser/static/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1359 2023-04-14 07:20:44.000000 imio.smartweb.common-1.1.6/src/imio/smartweb/common/browser/static/edit.js
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      402 2023-04-14 07:20:44.000000 imio.smartweb.common-1.1.6/src/imio/smartweb/common/browser/static/edit.less
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)   403548 2023-04-14 07:20:44.000000 imio.smartweb.common-1.1.6/src/imio/smartweb/common/browser/static/patched.web3862.eea.faceted-jquery.min.js
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      461 2023-04-14 07:20:44.000000 imio.smartweb.common-1.1.6/src/imio/smartweb/common/browser/static/smartweb-common-edit-compiled.css
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)    12646 2023-04-14 07:20:44.000000 imio.smartweb.common-1.1.6/src/imio/smartweb/common/browser/static/smartweb-common-edit-compiled.css.map
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      780 2023-04-14 07:20:44.000000 imio.smartweb.common-1.1.6/src/imio/smartweb/common/browser/static/smartweb-common-edit-compiled.js
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      686 2023-04-14 07:20:44.000000 imio.smartweb.common-1.1.6/src/imio/smartweb/common/browser/static/smartweb-common-edit-compiled.js.map
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      352 2023-04-14 07:20:44.000000 imio.smartweb.common-1.1.6/src/imio/smartweb/common/browser/static/smartweb-common-view-compiled.css
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)    12842 2023-04-14 07:20:44.000000 imio.smartweb.common-1.1.6/src/imio/smartweb/common/browser/static/smartweb-common-view-compiled.css.map
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1030 2023-04-14 07:20:44.000000 imio.smartweb.common-1.1.6/src/imio/smartweb/common/browser/static/smartweb-common-view-compiled.js
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1271 2023-04-14 07:20:44.000000 imio.smartweb.common-1.1.6/src/imio/smartweb/common/browser/static/smartweb-common-view-compiled.js.map
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1874 2023-04-14 07:20:44.000000 imio.smartweb.common-1.1.6/src/imio/smartweb/common/browser/static/view.js
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      449 2023-04-14 07:20:44.000000 imio.smartweb.common-1.1.6/src/imio/smartweb/common/browser/static/view.less
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      895 2023-04-14 07:20:44.000000 imio.smartweb.common-1.1.6/src/imio/smartweb/common/caching.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      435 2023-04-14 07:20:44.000000 imio.smartweb.common-1.1.6/src/imio/smartweb/common/config.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      796 2023-04-14 07:20:44.000000 imio.smartweb.common-1.1.6/src/imio/smartweb/common/configure.zcml
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-04-14 07:20:45.461639 imio.smartweb.common-1.1.6/src/imio/smartweb/common/faceted/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-04-14 07:20:44.000000 imio.smartweb.common-1.1.6/src/imio/smartweb/common/faceted/__init__.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      236 2023-04-14 07:20:44.000000 imio.smartweb.common-1.1.6/src/imio/smartweb/common/faceted/configure.zcml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      642 2023-04-14 07:20:44.000000 imio.smartweb.common-1.1.6/src/imio/smartweb/common/faceted/utils.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      642 2023-04-14 07:20:44.000000 imio.smartweb.common-1.1.6/src/imio/smartweb/common/faceted/widget.pt
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      938 2023-04-14 07:20:44.000000 imio.smartweb.common-1.1.6/src/imio/smartweb/common/faceted/widget.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1148 2023-04-14 07:20:44.000000 imio.smartweb.common-1.1.6/src/imio/smartweb/common/indexers.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      324 2023-04-14 07:20:44.000000 imio.smartweb.common-1.1.6/src/imio/smartweb/common/indexers.zcml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1417 2023-04-14 07:20:44.000000 imio.smartweb.common-1.1.6/src/imio/smartweb/common/interfaces.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      260 2023-04-14 07:20:44.000000 imio.smartweb.common-1.1.6/src/imio/smartweb/common/permissions.zcml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     3476 2023-04-14 07:20:44.000000 imio.smartweb.common-1.1.6/src/imio/smartweb/common/privacy.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1772 2023-04-14 07:20:44.000000 imio.smartweb.common-1.1.6/src/imio/smartweb/common/privacy.zcml
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-04-14 07:20:45.381639 imio.smartweb.common-1.1.6/src/imio/smartweb/common/profiles/
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-04-14 07:20:45.461639 imio.smartweb.common-1.1.6/src/imio/smartweb/common/profiles/default/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1193 2023-04-14 07:20:44.000000 imio.smartweb.common-1.1.6/src/imio/smartweb/common/profiles/default/actions.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      185 2023-04-14 07:20:44.000000 imio.smartweb.common-1.1.6/src/imio/smartweb/common/profiles/default/browserlayer.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      576 2023-04-14 07:20:44.000000 imio.smartweb.common-1.1.6/src/imio/smartweb/common/profiles/default/catalog.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      432 2023-04-14 07:20:44.000000 imio.smartweb.common-1.1.6/src/imio/smartweb/common/profiles/default/metadata.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)    45969 2023-04-14 07:20:44.000000 imio.smartweb.common-1.1.6/src/imio/smartweb/common/profiles/default/registry.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1595 2023-04-14 07:20:44.000000 imio.smartweb.common-1.1.6/src/imio/smartweb/common/profiles/default/rolemap.xml
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-04-14 07:20:45.461639 imio.smartweb.common-1.1.6/src/imio/smartweb/common/profiles/testing/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      163 2023-04-14 07:20:44.000000 imio.smartweb.common-1.1.6/src/imio/smartweb/common/profiles/testing/metadata.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      813 2023-04-14 07:20:44.000000 imio.smartweb.common-1.1.6/src/imio/smartweb/common/profiles/testing/registry.xml
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-04-14 07:20:45.461639 imio.smartweb.common-1.1.6/src/imio/smartweb/common/profiles/testing/types/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      229 2023-04-14 07:20:44.000000 imio.smartweb.common-1.1.6/src/imio/smartweb/common/profiles/testing/types/Collection.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      358 2023-04-14 07:20:44.000000 imio.smartweb.common-1.1.6/src/imio/smartweb/common/profiles/testing/types/Document.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      312 2023-04-14 07:20:44.000000 imio.smartweb.common-1.1.6/src/imio/smartweb/common/profiles/testing/types/Folder.xml
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-04-14 07:20:45.461639 imio.smartweb.common-1.1.6/src/imio/smartweb/common/profiles/uninstall/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      130 2023-04-14 07:20:44.000000 imio.smartweb.common-1.1.6/src/imio/smartweb/common/profiles/uninstall/browserlayer.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1278 2023-04-14 07:20:44.000000 imio.smartweb.common-1.1.6/src/imio/smartweb/common/profiles.zcml
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-04-14 07:20:45.465639 imio.smartweb.common-1.1.6/src/imio/smartweb/common/rest/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-04-14 07:20:44.000000 imio.smartweb.common-1.1.6/src/imio/smartweb/common/rest/__init__.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      301 2023-04-14 07:20:44.000000 imio.smartweb.common-1.1.6/src/imio/smartweb/common/rest/configure.zcml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     3349 2023-04-14 07:20:44.000000 imio.smartweb.common-1.1.6/src/imio/smartweb/common/rest/search_filters.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      458 2023-04-14 07:20:44.000000 imio.smartweb.common-1.1.6/src/imio/smartweb/common/rest/utils.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1053 2023-04-14 07:20:44.000000 imio.smartweb.common-1.1.6/src/imio/smartweb/common/setuphandlers.py
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-04-14 07:20:45.465639 imio.smartweb.common-1.1.6/src/imio/smartweb/common/sharing/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)       56 2023-04-14 07:20:44.000000 imio.smartweb.common-1.1.6/src/imio/smartweb/common/sharing/__init__.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      255 2023-04-14 07:20:44.000000 imio.smartweb.common-1.1.6/src/imio/smartweb/common/sharing/configure.zcml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      509 2023-04-14 07:20:44.000000 imio.smartweb.common-1.1.6/src/imio/smartweb/common/sharing/localroles.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      452 2023-04-14 07:20:44.000000 imio.smartweb.common-1.1.6/src/imio/smartweb/common/sharing/permissions.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      224 2023-04-14 07:20:44.000000 imio.smartweb.common-1.1.6/src/imio/smartweb/common/sharing/permissions.zcml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1060 2023-04-14 07:20:44.000000 imio.smartweb.common-1.1.6/src/imio/smartweb/common/subscribers.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      860 2023-04-14 07:20:44.000000 imio.smartweb.common-1.1.6/src/imio/smartweb/common/subscribers.zcml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1964 2023-04-14 07:20:44.000000 imio.smartweb.common-1.1.6/src/imio/smartweb/common/testing.py
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-04-14 07:20:45.469639 imio.smartweb.common-1.1.6/src/imio/smartweb/common/tests/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-04-14 07:20:44.000000 imio.smartweb.common-1.1.6/src/imio/smartweb/common/tests/__init__.py
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-04-14 07:20:45.469639 imio.smartweb.common-1.1.6/src/imio/smartweb/common/tests/resources/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1185 2023-04-14 07:20:44.000000 imio.smartweb.common-1.1.6/src/imio/smartweb/common/tests/resources/image.png
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)    30604 2023-04-14 07:20:44.000000 imio.smartweb.common-1.1.6/src/imio/smartweb/common/tests/resources/image_1400x800.png
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)    32643 2023-04-14 07:20:44.000000 imio.smartweb.common-1.1.6/src/imio/smartweb/common/tests/resources/image_1800x700.png
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-04-14 07:20:45.469639 imio.smartweb.common-1.1.6/src/imio/smartweb/common/tests/robot/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2011 2023-04-14 07:20:44.000000 imio.smartweb.common-1.1.6/src/imio/smartweb/common/tests/robot/test_example.robot
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2109 2023-04-14 07:20:44.000000 imio.smartweb.common-1.1.6/src/imio/smartweb/common/tests/test_cropping.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2493 2023-04-14 07:20:44.000000 imio.smartweb.common-1.1.6/src/imio/smartweb/common/tests/test_description.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2413 2023-04-14 07:20:44.000000 imio.smartweb.common-1.1.6/src/imio/smartweb/common/tests/test_forms.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     4960 2023-04-14 07:20:44.000000 imio.smartweb.common-1.1.6/src/imio/smartweb/common/tests/test_indexes.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     3370 2023-04-14 07:20:44.000000 imio.smartweb.common-1.1.6/src/imio/smartweb/common/tests/test_local_roles.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1578 2023-04-14 07:20:44.000000 imio.smartweb.common-1.1.6/src/imio/smartweb/common/tests/test_permissions.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2953 2023-04-14 07:20:44.000000 imio.smartweb.common-1.1.6/src/imio/smartweb/common/tests/test_privacy.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     3799 2023-04-14 07:20:44.000000 imio.smartweb.common-1.1.6/src/imio/smartweb/common/tests/test_rest.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      955 2023-04-14 07:20:44.000000 imio.smartweb.common-1.1.6/src/imio/smartweb/common/tests/test_robot.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2102 2023-04-14 07:20:44.000000 imio.smartweb.common-1.1.6/src/imio/smartweb/common/tests/test_setup.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     8032 2023-04-14 07:20:44.000000 imio.smartweb.common-1.1.6/src/imio/smartweb/common/tests/test_utils.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      889 2023-04-14 07:20:44.000000 imio.smartweb.common-1.1.6/src/imio/smartweb/common/tests/test_viewlets.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      749 2023-04-14 07:20:44.000000 imio.smartweb.common-1.1.6/src/imio/smartweb/common/tests/test_vocabularies.py
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-04-14 07:20:45.469639 imio.smartweb.common-1.1.6/src/imio/smartweb/common/upgrades/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-04-14 07:20:44.000000 imio.smartweb.common-1.1.6/src/imio/smartweb/common/upgrades/__init__.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     7778 2023-04-14 07:20:44.000000 imio.smartweb.common-1.1.6/src/imio/smartweb/common/upgrades/configure.zcml
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-04-14 07:20:45.437639 imio.smartweb.common-1.1.6/src/imio/smartweb/common/upgrades/profiles/
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-04-14 07:20:45.469639 imio.smartweb.common-1.1.6/src/imio/smartweb/common/upgrades/profiles/1007_to_1008/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1346 2023-04-14 07:20:44.000000 imio.smartweb.common-1.1.6/src/imio/smartweb/common/upgrades/profiles/1007_to_1008/rolemap.xml
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-04-14 07:20:45.469639 imio.smartweb.common-1.1.6/src/imio/smartweb/common/upgrades/profiles/1008_to_1009/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      721 2023-04-14 07:20:44.000000 imio.smartweb.common-1.1.6/src/imio/smartweb/common/upgrades/profiles/1008_to_1009/actions.xml
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-04-14 07:20:45.381639 imio.smartweb.common-1.1.6/src/imio/smartweb/common/upgrades/profiles/1009_to_1010/
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-04-14 07:20:45.469639 imio.smartweb.common-1.1.6/src/imio/smartweb/common/upgrades/profiles/1009_to_1010/registry/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      587 2023-04-14 07:20:44.000000 imio.smartweb.common-1.1.6/src/imio/smartweb/common/upgrades/profiles/1009_to_1010/registry/tiny_nonbreakingspace.xml
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-04-14 07:20:45.381639 imio.smartweb.common-1.1.6/src/imio/smartweb/common/upgrades/profiles/1010_to_1011/
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-04-14 07:20:45.469639 imio.smartweb.common-1.1.6/src/imio/smartweb/common/upgrades/profiles/1010_to_1011/registry/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      965 2023-04-14 07:20:44.000000 imio.smartweb.common-1.1.6/src/imio/smartweb/common/upgrades/profiles/1010_to_1011/registry/resources.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      888 2023-04-14 07:20:44.000000 imio.smartweb.common-1.1.6/src/imio/smartweb/common/upgrades/profiles/1010_to_1011/registry/scales.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2366 2023-04-14 07:20:44.000000 imio.smartweb.common-1.1.6/src/imio/smartweb/common/upgrades/profiles/1010_to_1011/registry/tinymce.xml
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-04-14 07:20:45.381639 imio.smartweb.common-1.1.6/src/imio/smartweb/common/upgrades/profiles/1011_to_1012/
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-04-14 07:20:45.469639 imio.smartweb.common-1.1.6/src/imio/smartweb/common/upgrades/profiles/1011_to_1012/registry/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      565 2023-04-14 07:20:44.000000 imio.smartweb.common-1.1.6/src/imio/smartweb/common/upgrades/profiles/1011_to_1012/registry/bundles.xml
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-04-14 07:20:45.433639 imio.smartweb.common-1.1.6/src/imio/smartweb/common/upgrades/profiles/1013_to_1014/
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-04-14 07:20:45.469639 imio.smartweb.common-1.1.6/src/imio/smartweb/common/upgrades/profiles/1013_to_1014/registry/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      535 2023-04-14 07:20:44.000000 imio.smartweb.common-1.1.6/src/imio/smartweb/common/upgrades/profiles/1013_to_1014/registry/tinymce.xml
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-04-14 07:20:45.437639 imio.smartweb.common-1.1.6/src/imio/smartweb/common/upgrades/profiles/1014_to_1015/
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-04-14 07:20:45.469639 imio.smartweb.common-1.1.6/src/imio/smartweb/common/upgrades/profiles/1014_to_1015/registry/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      224 2023-04-14 07:20:45.000000 imio.smartweb.common-1.1.6/src/imio/smartweb/common/upgrades/profiles/1014_to_1015/registry/syndication.xml
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-04-14 07:20:45.437639 imio.smartweb.common-1.1.6/src/imio/smartweb/common/upgrades/profiles/1015_to_1016/
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-04-14 07:20:45.469639 imio.smartweb.common-1.1.6/src/imio/smartweb/common/upgrades/profiles/1015_to_1016/registry/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      372 2023-04-14 07:20:45.000000 imio.smartweb.common-1.1.6/src/imio/smartweb/common/upgrades/profiles/1015_to_1016/registry/patched-faceted-jquery.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      846 2023-04-14 07:20:45.000000 imio.smartweb.common-1.1.6/src/imio/smartweb/common/upgrades/upgrades.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     5270 2023-04-14 07:20:45.000000 imio.smartweb.common-1.1.6/src/imio/smartweb/common/utils.py
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-04-14 07:20:45.469639 imio.smartweb.common-1.1.6/src/imio/smartweb/common/viewlets/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)       24 2023-04-14 07:20:45.000000 imio.smartweb.common-1.1.6/src/imio/smartweb/common/viewlets/__init__.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)       33 2023-04-14 07:20:45.000000 imio.smartweb.common-1.1.6/src/imio/smartweb/common/viewlets/analytics.pt
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1278 2023-04-14 07:20:45.000000 imio.smartweb.common-1.1.6/src/imio/smartweb/common/viewlets/colophon.pt
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      586 2023-04-14 07:20:45.000000 imio.smartweb.common-1.1.6/src/imio/smartweb/common/viewlets/colophon.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1436 2023-04-14 07:20:45.000000 imio.smartweb.common-1.1.6/src/imio/smartweb/common/viewlets/configure.zcml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1214 2023-04-14 07:20:45.000000 imio.smartweb.common-1.1.6/src/imio/smartweb/common/viewlets/privacy.pt
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     3453 2023-04-14 07:20:45.000000 imio.smartweb.common-1.1.6/src/imio/smartweb/common/vocabularies.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      766 2023-04-14 07:20:45.000000 imio.smartweb.common-1.1.6/src/imio/smartweb/common/vocabularies.zcml
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-04-14 07:20:45.445639 imio.smartweb.common-1.1.6/src/imio.smartweb.common.egg-info/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     9849 2023-04-14 07:20:45.000000 imio.smartweb.common-1.1.6/src/imio.smartweb.common.egg-info/PKG-INFO
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     6455 2023-04-14 07:20:45.000000 imio.smartweb.common-1.1.6/src/imio.smartweb.common.egg-info/SOURCES.txt
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        1 2023-04-14 07:20:45.000000 imio.smartweb.common-1.1.6/src/imio.smartweb.common.egg-info/dependency_links.txt
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)       19 2023-04-14 07:20:45.000000 imio.smartweb.common-1.1.6/src/imio.smartweb.common.egg-info/namespace_packages.txt
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        1 2023-04-14 07:20:45.000000 imio.smartweb.common-1.1.6/src/imio.smartweb.common.egg-info/not-zip-safe
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      420 2023-04-14 07:20:45.000000 imio.smartweb.common-1.1.6/src/imio.smartweb.common.egg-info/requires.txt
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        5 2023-04-14 07:20:45.000000 imio.smartweb.common-1.1.6/src/imio.smartweb.common.egg-info/top_level.txt
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-05-22 07:06:13.653975 imio.smartweb.common-1.1.7/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     5646 2023-05-22 07:06:12.000000 imio.smartweb.common-1.1.7/CHANGES.rst
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)       64 2023-05-22 07:06:12.000000 imio.smartweb.common-1.1.7/CONTRIBUTORS.rst
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      586 2023-05-22 07:06:12.000000 imio.smartweb.common-1.1.7/DEVELOP.rst
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)    18092 2023-05-22 07:06:12.000000 imio.smartweb.common-1.1.7/LICENSE.GPL
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      655 2023-05-22 07:06:12.000000 imio.smartweb.common-1.1.7/LICENSE.rst
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      106 2023-05-22 07:06:12.000000 imio.smartweb.common-1.1.7/MANIFEST.in
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     9964 2023-05-22 07:06:13.653975 imio.smartweb.common-1.1.7/PKG-INFO
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     3161 2023-05-22 07:06:12.000000 imio.smartweb.common-1.1.7/README.rst
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-05-22 07:06:13.629975 imio.smartweb.common-1.1.7/docs/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     7966 2023-05-22 07:06:12.000000 imio.smartweb.common-1.1.7/docs/conf.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)       83 2023-05-22 07:06:12.000000 imio.smartweb.common-1.1.7/docs/index.rst
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)       64 2023-05-22 07:06:12.000000 imio.smartweb.common-1.1.7/requirements.txt
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      518 2023-05-22 07:06:13.653975 imio.smartweb.common-1.1.7/setup.cfg
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2749 2023-05-22 07:06:12.000000 imio.smartweb.common-1.1.7/setup.py
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-05-22 07:06:13.581975 imio.smartweb.common-1.1.7/src/
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-05-22 07:06:13.629975 imio.smartweb.common-1.1.7/src/imio/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)       80 2023-05-22 07:06:12.000000 imio.smartweb.common-1.1.7/src/imio/__init__.py
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-05-22 07:06:13.633975 imio.smartweb.common-1.1.7/src/imio/smartweb/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)       80 2023-05-22 07:06:12.000000 imio.smartweb.common-1.1.7/src/imio/smartweb/__init__.py
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-05-22 07:06:13.637975 imio.smartweb.common-1.1.7/src/imio/smartweb/common/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2709 2023-05-22 07:06:12.000000 imio.smartweb.common-1.1.7/src/imio/smartweb/common/__init__.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      508 2023-05-22 07:06:12.000000 imio.smartweb.common-1.1.7/src/imio/smartweb/common/adapters.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      254 2023-05-22 07:06:12.000000 imio.smartweb.common-1.1.7/src/imio/smartweb/common/adapters.zcml
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-05-22 07:06:13.637975 imio.smartweb.common-1.1.7/src/imio/smartweb/common/behaviors/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)       24 2023-05-22 07:06:12.000000 imio.smartweb.common-1.1.7/src/imio/smartweb/common/behaviors/__init__.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      531 2023-05-22 07:06:12.000000 imio.smartweb.common-1.1.7/src/imio/smartweb/common/behaviors/configure.zcml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      805 2023-05-22 07:06:12.000000 imio.smartweb.common-1.1.7/src/imio/smartweb/common/behaviors/iam.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      804 2023-05-22 07:06:12.000000 imio.smartweb.common-1.1.7/src/imio/smartweb/common/behaviors/topics.py
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-05-22 07:06:13.637975 imio.smartweb.common-1.1.7/src/imio/smartweb/common/browser/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-05-22 07:06:12.000000 imio.smartweb.common-1.1.7/src/imio/smartweb/common/browser/__init__.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2452 2023-05-22 07:06:12.000000 imio.smartweb.common-1.1.7/src/imio/smartweb/common/browser/configure.zcml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      922 2023-05-22 07:06:12.000000 imio.smartweb.common-1.1.7/src/imio/smartweb/common/browser/cropping.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      151 2023-05-22 07:06:12.000000 imio.smartweb.common-1.1.7/src/imio/smartweb/common/browser/description.pt
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      517 2023-05-22 07:06:12.000000 imio.smartweb.common-1.1.7/src/imio/smartweb/common/browser/description.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     4164 2023-05-22 07:06:12.000000 imio.smartweb.common-1.1.7/src/imio/smartweb/common/browser/forms.py
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-05-22 07:06:13.637975 imio.smartweb.common-1.1.7/src/imio/smartweb/common/browser/overrides/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1818 2023-05-22 07:06:12.000000 imio.smartweb.common-1.1.7/src/imio/smartweb/common/browser/overrides/plone.app.z3cform.templates.widget.pt
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-05-22 07:06:13.637975 imio.smartweb.common-1.1.7/src/imio/smartweb/common/browser/privacy/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-05-22 07:06:12.000000 imio.smartweb.common-1.1.7/src/imio/smartweb/common/browser/privacy/__init__.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1062 2023-05-22 07:06:12.000000 imio.smartweb.common-1.1.7/src/imio/smartweb/common/browser/privacy/configure.zcml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1672 2023-05-22 07:06:12.000000 imio.smartweb.common-1.1.7/src/imio/smartweb/common/browser/privacy/form.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      205 2023-05-22 07:06:12.000000 imio.smartweb.common-1.1.7/src/imio/smartweb/common/browser/privacy/utils.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1815 2023-05-22 07:06:12.000000 imio.smartweb.common-1.1.7/src/imio/smartweb/common/browser/privacy/views.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      297 2023-05-22 07:06:12.000000 imio.smartweb.common-1.1.7/src/imio/smartweb/common/browser/scaling.py
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-05-22 07:06:13.641975 imio.smartweb.common-1.1.7/src/imio/smartweb/common/browser/static/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1359 2023-05-22 07:06:12.000000 imio.smartweb.common-1.1.7/src/imio/smartweb/common/browser/static/edit.js
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      402 2023-05-22 07:06:12.000000 imio.smartweb.common-1.1.7/src/imio/smartweb/common/browser/static/edit.less
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)   403548 2023-05-22 07:06:12.000000 imio.smartweb.common-1.1.7/src/imio/smartweb/common/browser/static/patched.web3862.eea.faceted-jquery.min.js
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      461 2023-05-22 07:06:12.000000 imio.smartweb.common-1.1.7/src/imio/smartweb/common/browser/static/smartweb-common-edit-compiled.css
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)    12646 2023-05-22 07:06:12.000000 imio.smartweb.common-1.1.7/src/imio/smartweb/common/browser/static/smartweb-common-edit-compiled.css.map
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      780 2023-05-22 07:06:12.000000 imio.smartweb.common-1.1.7/src/imio/smartweb/common/browser/static/smartweb-common-edit-compiled.js
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      686 2023-05-22 07:06:12.000000 imio.smartweb.common-1.1.7/src/imio/smartweb/common/browser/static/smartweb-common-edit-compiled.js.map
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      352 2023-05-22 07:06:12.000000 imio.smartweb.common-1.1.7/src/imio/smartweb/common/browser/static/smartweb-common-view-compiled.css
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)    12842 2023-05-22 07:06:12.000000 imio.smartweb.common-1.1.7/src/imio/smartweb/common/browser/static/smartweb-common-view-compiled.css.map
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1030 2023-05-22 07:06:12.000000 imio.smartweb.common-1.1.7/src/imio/smartweb/common/browser/static/smartweb-common-view-compiled.js
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1271 2023-05-22 07:06:12.000000 imio.smartweb.common-1.1.7/src/imio/smartweb/common/browser/static/smartweb-common-view-compiled.js.map
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1874 2023-05-22 07:06:12.000000 imio.smartweb.common-1.1.7/src/imio/smartweb/common/browser/static/view.js
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      449 2023-05-22 07:06:12.000000 imio.smartweb.common-1.1.7/src/imio/smartweb/common/browser/static/view.less
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      895 2023-05-22 07:06:12.000000 imio.smartweb.common-1.1.7/src/imio/smartweb/common/caching.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      435 2023-05-22 07:06:12.000000 imio.smartweb.common-1.1.7/src/imio/smartweb/common/config.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      796 2023-05-22 07:06:12.000000 imio.smartweb.common-1.1.7/src/imio/smartweb/common/configure.zcml
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-05-22 07:06:13.641975 imio.smartweb.common-1.1.7/src/imio/smartweb/common/faceted/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-05-22 07:06:12.000000 imio.smartweb.common-1.1.7/src/imio/smartweb/common/faceted/__init__.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      236 2023-05-22 07:06:12.000000 imio.smartweb.common-1.1.7/src/imio/smartweb/common/faceted/configure.zcml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      642 2023-05-22 07:06:12.000000 imio.smartweb.common-1.1.7/src/imio/smartweb/common/faceted/utils.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      642 2023-05-22 07:06:12.000000 imio.smartweb.common-1.1.7/src/imio/smartweb/common/faceted/widget.pt
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      938 2023-05-22 07:06:12.000000 imio.smartweb.common-1.1.7/src/imio/smartweb/common/faceted/widget.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1148 2023-05-22 07:06:12.000000 imio.smartweb.common-1.1.7/src/imio/smartweb/common/indexers.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      324 2023-05-22 07:06:12.000000 imio.smartweb.common-1.1.7/src/imio/smartweb/common/indexers.zcml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1417 2023-05-22 07:06:12.000000 imio.smartweb.common-1.1.7/src/imio/smartweb/common/interfaces.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      260 2023-05-22 07:06:12.000000 imio.smartweb.common-1.1.7/src/imio/smartweb/common/permissions.zcml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     3476 2023-05-22 07:06:12.000000 imio.smartweb.common-1.1.7/src/imio/smartweb/common/privacy.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1772 2023-05-22 07:06:12.000000 imio.smartweb.common-1.1.7/src/imio/smartweb/common/privacy.zcml
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-05-22 07:06:13.581975 imio.smartweb.common-1.1.7/src/imio/smartweb/common/profiles/
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-05-22 07:06:13.645975 imio.smartweb.common-1.1.7/src/imio/smartweb/common/profiles/default/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1193 2023-05-22 07:06:12.000000 imio.smartweb.common-1.1.7/src/imio/smartweb/common/profiles/default/actions.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      185 2023-05-22 07:06:12.000000 imio.smartweb.common-1.1.7/src/imio/smartweb/common/profiles/default/browserlayer.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      576 2023-05-22 07:06:12.000000 imio.smartweb.common-1.1.7/src/imio/smartweb/common/profiles/default/catalog.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      432 2023-05-22 07:06:13.000000 imio.smartweb.common-1.1.7/src/imio/smartweb/common/profiles/default/metadata.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)    45971 2023-05-22 07:06:13.000000 imio.smartweb.common-1.1.7/src/imio/smartweb/common/profiles/default/registry.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1595 2023-05-22 07:06:13.000000 imio.smartweb.common-1.1.7/src/imio/smartweb/common/profiles/default/rolemap.xml
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-05-22 07:06:13.645975 imio.smartweb.common-1.1.7/src/imio/smartweb/common/profiles/testing/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      163 2023-05-22 07:06:13.000000 imio.smartweb.common-1.1.7/src/imio/smartweb/common/profiles/testing/metadata.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      813 2023-05-22 07:06:13.000000 imio.smartweb.common-1.1.7/src/imio/smartweb/common/profiles/testing/registry.xml
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-05-22 07:06:13.645975 imio.smartweb.common-1.1.7/src/imio/smartweb/common/profiles/testing/types/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      229 2023-05-22 07:06:13.000000 imio.smartweb.common-1.1.7/src/imio/smartweb/common/profiles/testing/types/Collection.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      358 2023-05-22 07:06:13.000000 imio.smartweb.common-1.1.7/src/imio/smartweb/common/profiles/testing/types/Document.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      312 2023-05-22 07:06:13.000000 imio.smartweb.common-1.1.7/src/imio/smartweb/common/profiles/testing/types/Folder.xml
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-05-22 07:06:13.645975 imio.smartweb.common-1.1.7/src/imio/smartweb/common/profiles/uninstall/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      130 2023-05-22 07:06:13.000000 imio.smartweb.common-1.1.7/src/imio/smartweb/common/profiles/uninstall/browserlayer.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1278 2023-05-22 07:06:12.000000 imio.smartweb.common-1.1.7/src/imio/smartweb/common/profiles.zcml
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-05-22 07:06:13.645975 imio.smartweb.common-1.1.7/src/imio/smartweb/common/rest/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-05-22 07:06:13.000000 imio.smartweb.common-1.1.7/src/imio/smartweb/common/rest/__init__.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      301 2023-05-22 07:06:13.000000 imio.smartweb.common-1.1.7/src/imio/smartweb/common/rest/configure.zcml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     3349 2023-05-22 07:06:13.000000 imio.smartweb.common-1.1.7/src/imio/smartweb/common/rest/search_filters.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      458 2023-05-22 07:06:13.000000 imio.smartweb.common-1.1.7/src/imio/smartweb/common/rest/utils.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1053 2023-05-22 07:06:13.000000 imio.smartweb.common-1.1.7/src/imio/smartweb/common/setuphandlers.py
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-05-22 07:06:13.649975 imio.smartweb.common-1.1.7/src/imio/smartweb/common/sharing/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)       56 2023-05-22 07:06:13.000000 imio.smartweb.common-1.1.7/src/imio/smartweb/common/sharing/__init__.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      255 2023-05-22 07:06:13.000000 imio.smartweb.common-1.1.7/src/imio/smartweb/common/sharing/configure.zcml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      509 2023-05-22 07:06:13.000000 imio.smartweb.common-1.1.7/src/imio/smartweb/common/sharing/localroles.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      452 2023-05-22 07:06:13.000000 imio.smartweb.common-1.1.7/src/imio/smartweb/common/sharing/permissions.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      224 2023-05-22 07:06:13.000000 imio.smartweb.common-1.1.7/src/imio/smartweb/common/sharing/permissions.zcml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1060 2023-05-22 07:06:13.000000 imio.smartweb.common-1.1.7/src/imio/smartweb/common/subscribers.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      860 2023-05-22 07:06:13.000000 imio.smartweb.common-1.1.7/src/imio/smartweb/common/subscribers.zcml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1964 2023-05-22 07:06:13.000000 imio.smartweb.common-1.1.7/src/imio/smartweb/common/testing.py
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-05-22 07:06:13.649975 imio.smartweb.common-1.1.7/src/imio/smartweb/common/tests/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-05-22 07:06:13.000000 imio.smartweb.common-1.1.7/src/imio/smartweb/common/tests/__init__.py
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-05-22 07:06:13.649975 imio.smartweb.common-1.1.7/src/imio/smartweb/common/tests/resources/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1185 2023-05-22 07:06:13.000000 imio.smartweb.common-1.1.7/src/imio/smartweb/common/tests/resources/image.png
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)    30604 2023-05-22 07:06:13.000000 imio.smartweb.common-1.1.7/src/imio/smartweb/common/tests/resources/image_1400x800.png
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)    32643 2023-05-22 07:06:13.000000 imio.smartweb.common-1.1.7/src/imio/smartweb/common/tests/resources/image_1800x700.png
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-05-22 07:06:13.649975 imio.smartweb.common-1.1.7/src/imio/smartweb/common/tests/robot/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2011 2023-05-22 07:06:13.000000 imio.smartweb.common-1.1.7/src/imio/smartweb/common/tests/robot/test_example.robot
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2109 2023-05-22 07:06:13.000000 imio.smartweb.common-1.1.7/src/imio/smartweb/common/tests/test_cropping.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2493 2023-05-22 07:06:13.000000 imio.smartweb.common-1.1.7/src/imio/smartweb/common/tests/test_description.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2413 2023-05-22 07:06:13.000000 imio.smartweb.common-1.1.7/src/imio/smartweb/common/tests/test_forms.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     4960 2023-05-22 07:06:13.000000 imio.smartweb.common-1.1.7/src/imio/smartweb/common/tests/test_indexes.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     3370 2023-05-22 07:06:13.000000 imio.smartweb.common-1.1.7/src/imio/smartweb/common/tests/test_local_roles.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1578 2023-05-22 07:06:13.000000 imio.smartweb.common-1.1.7/src/imio/smartweb/common/tests/test_permissions.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2953 2023-05-22 07:06:13.000000 imio.smartweb.common-1.1.7/src/imio/smartweb/common/tests/test_privacy.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     3799 2023-05-22 07:06:13.000000 imio.smartweb.common-1.1.7/src/imio/smartweb/common/tests/test_rest.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      955 2023-05-22 07:06:13.000000 imio.smartweb.common-1.1.7/src/imio/smartweb/common/tests/test_robot.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2102 2023-05-22 07:06:13.000000 imio.smartweb.common-1.1.7/src/imio/smartweb/common/tests/test_setup.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     8032 2023-05-22 07:06:13.000000 imio.smartweb.common-1.1.7/src/imio/smartweb/common/tests/test_utils.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      889 2023-05-22 07:06:13.000000 imio.smartweb.common-1.1.7/src/imio/smartweb/common/tests/test_viewlets.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      749 2023-05-22 07:06:13.000000 imio.smartweb.common-1.1.7/src/imio/smartweb/common/tests/test_vocabularies.py
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-05-22 07:06:13.649975 imio.smartweb.common-1.1.7/src/imio/smartweb/common/upgrades/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-05-22 07:06:13.000000 imio.smartweb.common-1.1.7/src/imio/smartweb/common/upgrades/__init__.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     8397 2023-05-22 07:06:13.000000 imio.smartweb.common-1.1.7/src/imio/smartweb/common/upgrades/configure.zcml
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-05-22 07:06:13.581975 imio.smartweb.common-1.1.7/src/imio/smartweb/common/upgrades/profiles/
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-05-22 07:06:13.653975 imio.smartweb.common-1.1.7/src/imio/smartweb/common/upgrades/profiles/1007_to_1008/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1346 2023-05-22 07:06:13.000000 imio.smartweb.common-1.1.7/src/imio/smartweb/common/upgrades/profiles/1007_to_1008/rolemap.xml
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-05-22 07:06:13.653975 imio.smartweb.common-1.1.7/src/imio/smartweb/common/upgrades/profiles/1008_to_1009/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      721 2023-05-22 07:06:13.000000 imio.smartweb.common-1.1.7/src/imio/smartweb/common/upgrades/profiles/1008_to_1009/actions.xml
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-05-22 07:06:13.581975 imio.smartweb.common-1.1.7/src/imio/smartweb/common/upgrades/profiles/1009_to_1010/
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-05-22 07:06:13.653975 imio.smartweb.common-1.1.7/src/imio/smartweb/common/upgrades/profiles/1009_to_1010/registry/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      587 2023-05-22 07:06:13.000000 imio.smartweb.common-1.1.7/src/imio/smartweb/common/upgrades/profiles/1009_to_1010/registry/tiny_nonbreakingspace.xml
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-05-22 07:06:13.581975 imio.smartweb.common-1.1.7/src/imio/smartweb/common/upgrades/profiles/1010_to_1011/
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-05-22 07:06:13.653975 imio.smartweb.common-1.1.7/src/imio/smartweb/common/upgrades/profiles/1010_to_1011/registry/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      965 2023-05-22 07:06:13.000000 imio.smartweb.common-1.1.7/src/imio/smartweb/common/upgrades/profiles/1010_to_1011/registry/resources.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      888 2023-05-22 07:06:13.000000 imio.smartweb.common-1.1.7/src/imio/smartweb/common/upgrades/profiles/1010_to_1011/registry/scales.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2366 2023-05-22 07:06:13.000000 imio.smartweb.common-1.1.7/src/imio/smartweb/common/upgrades/profiles/1010_to_1011/registry/tinymce.xml
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-05-22 07:06:13.581975 imio.smartweb.common-1.1.7/src/imio/smartweb/common/upgrades/profiles/1011_to_1012/
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-05-22 07:06:13.653975 imio.smartweb.common-1.1.7/src/imio/smartweb/common/upgrades/profiles/1011_to_1012/registry/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      565 2023-05-22 07:06:13.000000 imio.smartweb.common-1.1.7/src/imio/smartweb/common/upgrades/profiles/1011_to_1012/registry/bundles.xml
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-05-22 07:06:13.581975 imio.smartweb.common-1.1.7/src/imio/smartweb/common/upgrades/profiles/1013_to_1014/
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-05-22 07:06:13.653975 imio.smartweb.common-1.1.7/src/imio/smartweb/common/upgrades/profiles/1013_to_1014/registry/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      535 2023-05-22 07:06:13.000000 imio.smartweb.common-1.1.7/src/imio/smartweb/common/upgrades/profiles/1013_to_1014/registry/tinymce.xml
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-05-22 07:06:13.581975 imio.smartweb.common-1.1.7/src/imio/smartweb/common/upgrades/profiles/1014_to_1015/
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-05-22 07:06:13.653975 imio.smartweb.common-1.1.7/src/imio/smartweb/common/upgrades/profiles/1014_to_1015/registry/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      224 2023-05-22 07:06:13.000000 imio.smartweb.common-1.1.7/src/imio/smartweb/common/upgrades/profiles/1014_to_1015/registry/syndication.xml
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-05-22 07:06:13.581975 imio.smartweb.common-1.1.7/src/imio/smartweb/common/upgrades/profiles/1015_to_1016/
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-05-22 07:06:13.653975 imio.smartweb.common-1.1.7/src/imio/smartweb/common/upgrades/profiles/1015_to_1016/registry/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      372 2023-05-22 07:06:13.000000 imio.smartweb.common-1.1.7/src/imio/smartweb/common/upgrades/profiles/1015_to_1016/registry/patched-faceted-jquery.xml
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-05-22 07:06:13.581975 imio.smartweb.common-1.1.7/src/imio/smartweb/common/upgrades/profiles/1016_to_1017/
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-05-22 07:06:13.653975 imio.smartweb.common-1.1.7/src/imio/smartweb/common/upgrades/profiles/1016_to_1017/registry/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      890 2023-05-22 07:06:13.000000 imio.smartweb.common-1.1.7/src/imio/smartweb/common/upgrades/profiles/1016_to_1017/registry/scales.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      846 2023-05-22 07:06:13.000000 imio.smartweb.common-1.1.7/src/imio/smartweb/common/upgrades/upgrades.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     5270 2023-05-22 07:06:13.000000 imio.smartweb.common-1.1.7/src/imio/smartweb/common/utils.py
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-05-22 07:06:13.653975 imio.smartweb.common-1.1.7/src/imio/smartweb/common/viewlets/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)       24 2023-05-22 07:06:13.000000 imio.smartweb.common-1.1.7/src/imio/smartweb/common/viewlets/__init__.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)       33 2023-05-22 07:06:13.000000 imio.smartweb.common-1.1.7/src/imio/smartweb/common/viewlets/analytics.pt
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1278 2023-05-22 07:06:13.000000 imio.smartweb.common-1.1.7/src/imio/smartweb/common/viewlets/colophon.pt
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      586 2023-05-22 07:06:13.000000 imio.smartweb.common-1.1.7/src/imio/smartweb/common/viewlets/colophon.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1436 2023-05-22 07:06:13.000000 imio.smartweb.common-1.1.7/src/imio/smartweb/common/viewlets/configure.zcml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1214 2023-05-22 07:06:13.000000 imio.smartweb.common-1.1.7/src/imio/smartweb/common/viewlets/privacy.pt
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     3453 2023-05-22 07:06:13.000000 imio.smartweb.common-1.1.7/src/imio/smartweb/common/vocabularies.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      766 2023-05-22 07:06:13.000000 imio.smartweb.common-1.1.7/src/imio/smartweb/common/vocabularies.zcml
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-05-22 07:06:13.633975 imio.smartweb.common-1.1.7/src/imio.smartweb.common.egg-info/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     9964 2023-05-22 07:06:13.000000 imio.smartweb.common-1.1.7/src/imio.smartweb.common.egg-info/PKG-INFO
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     6531 2023-05-22 07:06:13.000000 imio.smartweb.common-1.1.7/src/imio.smartweb.common.egg-info/SOURCES.txt
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        1 2023-05-22 07:06:13.000000 imio.smartweb.common-1.1.7/src/imio.smartweb.common.egg-info/dependency_links.txt
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)       19 2023-05-22 07:06:13.000000 imio.smartweb.common-1.1.7/src/imio.smartweb.common.egg-info/namespace_packages.txt
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        1 2023-05-22 07:06:13.000000 imio.smartweb.common-1.1.7/src/imio.smartweb.common.egg-info/not-zip-safe
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      420 2023-05-22 07:06:13.000000 imio.smartweb.common-1.1.7/src/imio.smartweb.common.egg-info/requires.txt
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        5 2023-05-22 07:06:13.000000 imio.smartweb.common-1.1.7/src/imio.smartweb.common.egg-info/top_level.txt
```

### Comparing `imio.smartweb.common-1.1.6/CHANGES.rst` & `imio.smartweb.common-1.1.7/CHANGES.rst`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,21 @@
 Changelog
 =========
 
 
+1.1.7 (2023-05-22)
+------------------
+
+- Change banner scale to have infinite height
+  [laulaz]
+
+- Migrate to Plone 6.0.4
+  [boulch]
+
+
 1.1.6 (2023-04-14)
 ------------------
 
 - Don't use image_scales metadata anymore (Fix faceted)
   [boulch, laulaz]
 
 - Update object modification date if cropping was removed/updated
```

### Comparing `imio.smartweb.common-1.1.6/DEVELOP.rst` & `imio.smartweb.common-1.1.7/DEVELOP.rst`

 * *Files identical despite different names*

### Comparing `imio.smartweb.common-1.1.6/LICENSE.GPL` & `imio.smartweb.common-1.1.7/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `imio.smartweb.common-1.1.6/LICENSE.rst` & `imio.smartweb.common-1.1.7/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `imio.smartweb.common-1.1.6/PKG-INFO` & `imio.smartweb.common-1.1.7/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: imio.smartweb.common
-Version: 1.1.6
+Version: 1.1.7
 Summary: Common utilities, vocabularies, taxonomies for imio.smartweb & co products
 Home-page: https://github.com/imio/imio.smartweb.common
 Author: iMio
 Author-email: christophe.boulanger@imio.be
 License: GPL version 2
 Project-URL: PyPI, https://pypi.python.org/pypi/imio.smartweb.common
 Project-URL: Source, https://github.com/imio/imio.smartweb.common
 Project-URL: Tracker, https://github.com/imio/imio.smartweb.common/issues
 Keywords: Python Plone CMS
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Plone
 Classifier: Framework :: Plone :: Addon
 Classifier: Framework :: Plone :: 6.0
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -132,14 +131,24 @@
 - iMio, christophe.boulanger@imio.be
 
 
 Changelog
 =========
 
 
+1.1.7 (2023-05-22)
+------------------
+
+- Change banner scale to have infinite height
+  [laulaz]
+
+- Migrate to Plone 6.0.4
+  [boulch]
+
+
 1.1.6 (2023-04-14)
 ------------------
 
 - Don't use image_scales metadata anymore (Fix faceted)
   [boulch, laulaz]
 
 - Update object modification date if cropping was removed/updated
@@ -421,9 +430,7 @@
 
 
 1.0a1 (2021-11-05)
 ------------------
 
 - Initial release.
   [boulch]
-
-
```

### Comparing `imio.smartweb.common-1.1.6/README.rst` & `imio.smartweb.common-1.1.7/README.rst`

 * *Files identical despite different names*

### Comparing `imio.smartweb.common-1.1.6/docs/conf.py` & `imio.smartweb.common-1.1.7/docs/conf.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.common-1.1.6/setup.cfg` & `imio.smartweb.common-1.1.7/setup.cfg`

 * *Files identical despite different names*

### Comparing `imio.smartweb.common-1.1.6/setup.py` & `imio.smartweb.common-1.1.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
         open("CHANGES.rst").read(),
     ]
 )
 
 
 setup(
     name="imio.smartweb.common",
-    version="1.1.6",
+    version="1.1.7",
     description="Common utilities, vocabularies, taxonomies for imio.smartweb & co products",
     long_description=long_description,
     # Get more from https://pypi.org/classifiers/
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Environment :: Web Environment",
         "Framework :: Plone",
```

### Comparing `imio.smartweb.common-1.1.6/src/imio/smartweb/common/__init__.py` & `imio.smartweb.common-1.1.7/src/imio/smartweb/common/__init__.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.common-1.1.6/src/imio/smartweb/common/behaviors/configure.zcml` & `imio.smartweb.common-1.1.7/src/imio/smartweb/common/behaviors/configure.zcml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.common-1.1.6/src/imio/smartweb/common/behaviors/iam.py` & `imio.smartweb.common-1.1.7/src/imio/smartweb/common/behaviors/iam.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.common-1.1.6/src/imio/smartweb/common/behaviors/topics.py` & `imio.smartweb.common-1.1.7/src/imio/smartweb/common/behaviors/topics.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.common-1.1.6/src/imio/smartweb/common/browser/configure.zcml` & `imio.smartweb.common-1.1.7/src/imio/smartweb/common/browser/configure.zcml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.common-1.1.6/src/imio/smartweb/common/browser/cropping.py` & `imio.smartweb.common-1.1.7/src/imio/smartweb/common/browser/cropping.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.common-1.1.6/src/imio/smartweb/common/browser/description.py` & `imio.smartweb.common-1.1.7/src/imio/smartweb/common/browser/description.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.common-1.1.6/src/imio/smartweb/common/browser/forms.py` & `imio.smartweb.common-1.1.7/src/imio/smartweb/common/browser/forms.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.common-1.1.6/src/imio/smartweb/common/browser/overrides/plone.app.z3cform.templates.widget.pt` & `imio.smartweb.common-1.1.7/src/imio/smartweb/common/browser/overrides/plone.app.z3cform.templates.widget.pt`

 * *Files identical despite different names*

### Comparing `imio.smartweb.common-1.1.6/src/imio/smartweb/common/browser/privacy/configure.zcml` & `imio.smartweb.common-1.1.7/src/imio/smartweb/common/browser/privacy/configure.zcml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.common-1.1.6/src/imio/smartweb/common/browser/privacy/form.py` & `imio.smartweb.common-1.1.7/src/imio/smartweb/common/browser/privacy/form.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.common-1.1.6/src/imio/smartweb/common/browser/privacy/views.py` & `imio.smartweb.common-1.1.7/src/imio/smartweb/common/browser/privacy/views.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.common-1.1.6/src/imio/smartweb/common/browser/static/edit.js` & `imio.smartweb.common-1.1.7/src/imio/smartweb/common/browser/static/edit.js`

 * *Files identical despite different names*

### Comparing `imio.smartweb.common-1.1.6/src/imio/smartweb/common/browser/static/patched.web3862.eea.faceted-jquery.min.js` & `imio.smartweb.common-1.1.7/src/imio/smartweb/common/browser/static/patched.web3862.eea.faceted-jquery.min.js`

 * *Files identical despite different names*

### Comparing `imio.smartweb.common-1.1.6/src/imio/smartweb/common/browser/static/smartweb-common-edit-compiled.css.map` & `imio.smartweb.common-1.1.7/src/imio/smartweb/common/browser/static/smartweb-common-edit-compiled.css.map`

 * *Files identical despite different names*

### Comparing `imio.smartweb.common-1.1.6/src/imio/smartweb/common/browser/static/smartweb-common-edit-compiled.js` & `imio.smartweb.common-1.1.7/src/imio/smartweb/common/browser/static/smartweb-common-edit-compiled.js`

 * *Files identical despite different names*

### Comparing `imio.smartweb.common-1.1.6/src/imio/smartweb/common/browser/static/smartweb-common-edit-compiled.js.map` & `imio.smartweb.common-1.1.7/src/imio/smartweb/common/browser/static/smartweb-common-edit-compiled.js.map`

 * *Files identical despite different names*

### Comparing `imio.smartweb.common-1.1.6/src/imio/smartweb/common/browser/static/smartweb-common-view-compiled.css.map` & `imio.smartweb.common-1.1.7/src/imio/smartweb/common/browser/static/smartweb-common-view-compiled.css.map`

 * *Files identical despite different names*

### Comparing `imio.smartweb.common-1.1.6/src/imio/smartweb/common/browser/static/smartweb-common-view-compiled.js` & `imio.smartweb.common-1.1.7/src/imio/smartweb/common/browser/static/smartweb-common-view-compiled.js`

 * *Files identical despite different names*

### Comparing `imio.smartweb.common-1.1.6/src/imio/smartweb/common/browser/static/smartweb-common-view-compiled.js.map` & `imio.smartweb.common-1.1.7/src/imio/smartweb/common/browser/static/smartweb-common-view-compiled.js.map`

 * *Files identical despite different names*

### Comparing `imio.smartweb.common-1.1.6/src/imio/smartweb/common/browser/static/view.js` & `imio.smartweb.common-1.1.7/src/imio/smartweb/common/browser/static/view.js`

 * *Files identical despite different names*

### Comparing `imio.smartweb.common-1.1.6/src/imio/smartweb/common/caching.py` & `imio.smartweb.common-1.1.7/src/imio/smartweb/common/caching.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.common-1.1.6/src/imio/smartweb/common/configure.zcml` & `imio.smartweb.common-1.1.7/src/imio/smartweb/common/configure.zcml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.common-1.1.6/src/imio/smartweb/common/faceted/utils.py` & `imio.smartweb.common-1.1.7/src/imio/smartweb/common/faceted/utils.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.common-1.1.6/src/imio/smartweb/common/faceted/widget.pt` & `imio.smartweb.common-1.1.7/src/imio/smartweb/common/faceted/widget.pt`

 * *Files identical despite different names*

### Comparing `imio.smartweb.common-1.1.6/src/imio/smartweb/common/faceted/widget.py` & `imio.smartweb.common-1.1.7/src/imio/smartweb/common/faceted/widget.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.common-1.1.6/src/imio/smartweb/common/indexers.py` & `imio.smartweb.common-1.1.7/src/imio/smartweb/common/indexers.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.common-1.1.6/src/imio/smartweb/common/interfaces.py` & `imio.smartweb.common-1.1.7/src/imio/smartweb/common/interfaces.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.common-1.1.6/src/imio/smartweb/common/privacy.py` & `imio.smartweb.common-1.1.7/src/imio/smartweb/common/privacy.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.common-1.1.6/src/imio/smartweb/common/privacy.zcml` & `imio.smartweb.common-1.1.7/src/imio/smartweb/common/privacy.zcml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.common-1.1.6/src/imio/smartweb/common/profiles/default/actions.xml` & `imio.smartweb.common-1.1.7/src/imio/smartweb/common/profiles/default/actions.xml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.common-1.1.6/src/imio/smartweb/common/profiles/default/catalog.xml` & `imio.smartweb.common-1.1.7/src/imio/smartweb/common/profiles/default/catalog.xml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.common-1.1.6/src/imio/smartweb/common/profiles/default/registry.xml` & `imio.smartweb.common-1.1.7/src/imio/smartweb/common/profiles/default/registry.xml`

 * *Files 0% similar despite different names*

#### Comparing `imio.smartweb.common-1.1.6/src/imio/smartweb/common/profiles/default/registry.xml` & `imio.smartweb.common-1.1.7/src/imio/smartweb/common/profiles/default/registry.xml`

```diff
@@ -1,12 +1,12 @@
 <?xml version="1.0" encoding="utf-8"?>
 <registry xmlns:i18n="http://xml.zope.org/namespaces/i18n" i18n:domain="imio.smartweb">
   <record name="plone.allowed_sizes" interface="Products.CMFPlone.interfaces.controlpanel.IImagingSchema" field="allowed_sizes">
     <value purge="true">
-      <element>banner 1920:600</element>
+      <element>banner 1920:65536</element>
       <element>affiche 1320:440</element>
       <element>extralarge 1320:1320</element>
       <element>large 768:768</element>
       <element>slide 750:500</element>
       <element>medium 600:600</element>
       <element>preview 400:400</element>
       <element>vignette 390:260</element>
```

### Comparing `imio.smartweb.common-1.1.6/src/imio/smartweb/common/profiles/default/rolemap.xml` & `imio.smartweb.common-1.1.7/src/imio/smartweb/common/profiles/default/rolemap.xml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.common-1.1.6/src/imio/smartweb/common/profiles/testing/registry.xml` & `imio.smartweb.common-1.1.7/src/imio/smartweb/common/profiles/testing/registry.xml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.common-1.1.6/src/imio/smartweb/common/profiles.zcml` & `imio.smartweb.common-1.1.7/src/imio/smartweb/common/profiles.zcml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.common-1.1.6/src/imio/smartweb/common/rest/search_filters.py` & `imio.smartweb.common-1.1.7/src/imio/smartweb/common/rest/search_filters.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.common-1.1.6/src/imio/smartweb/common/setuphandlers.py` & `imio.smartweb.common-1.1.7/src/imio/smartweb/common/setuphandlers.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.common-1.1.6/src/imio/smartweb/common/subscribers.py` & `imio.smartweb.common-1.1.7/src/imio/smartweb/common/subscribers.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.common-1.1.6/src/imio/smartweb/common/subscribers.zcml` & `imio.smartweb.common-1.1.7/src/imio/smartweb/common/subscribers.zcml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.common-1.1.6/src/imio/smartweb/common/testing.py` & `imio.smartweb.common-1.1.7/src/imio/smartweb/common/testing.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.common-1.1.6/src/imio/smartweb/common/tests/resources/image.png` & `imio.smartweb.common-1.1.7/src/imio/smartweb/common/tests/resources/image.png`

 * *Files identical despite different names*

### Comparing `imio.smartweb.common-1.1.6/src/imio/smartweb/common/tests/resources/image_1400x800.png` & `imio.smartweb.common-1.1.7/src/imio/smartweb/common/tests/resources/image_1400x800.png`

 * *Files identical despite different names*

### Comparing `imio.smartweb.common-1.1.6/src/imio/smartweb/common/tests/resources/image_1800x700.png` & `imio.smartweb.common-1.1.7/src/imio/smartweb/common/tests/resources/image_1800x700.png`

 * *Files identical despite different names*

### Comparing `imio.smartweb.common-1.1.6/src/imio/smartweb/common/tests/robot/test_example.robot` & `imio.smartweb.common-1.1.7/src/imio/smartweb/common/tests/robot/test_example.robot`

 * *Files identical despite different names*

### Comparing `imio.smartweb.common-1.1.6/src/imio/smartweb/common/tests/test_cropping.py` & `imio.smartweb.common-1.1.7/src/imio/smartweb/common/tests/test_cropping.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.common-1.1.6/src/imio/smartweb/common/tests/test_description.py` & `imio.smartweb.common-1.1.7/src/imio/smartweb/common/tests/test_description.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.common-1.1.6/src/imio/smartweb/common/tests/test_forms.py` & `imio.smartweb.common-1.1.7/src/imio/smartweb/common/tests/test_forms.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.common-1.1.6/src/imio/smartweb/common/tests/test_indexes.py` & `imio.smartweb.common-1.1.7/src/imio/smartweb/common/tests/test_indexes.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.common-1.1.6/src/imio/smartweb/common/tests/test_local_roles.py` & `imio.smartweb.common-1.1.7/src/imio/smartweb/common/tests/test_local_roles.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.common-1.1.6/src/imio/smartweb/common/tests/test_permissions.py` & `imio.smartweb.common-1.1.7/src/imio/smartweb/common/tests/test_permissions.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.common-1.1.6/src/imio/smartweb/common/tests/test_privacy.py` & `imio.smartweb.common-1.1.7/src/imio/smartweb/common/tests/test_privacy.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.common-1.1.6/src/imio/smartweb/common/tests/test_rest.py` & `imio.smartweb.common-1.1.7/src/imio/smartweb/common/tests/test_rest.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.common-1.1.6/src/imio/smartweb/common/tests/test_robot.py` & `imio.smartweb.common-1.1.7/src/imio/smartweb/common/tests/test_robot.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.common-1.1.6/src/imio/smartweb/common/tests/test_setup.py` & `imio.smartweb.common-1.1.7/src/imio/smartweb/common/tests/test_setup.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.common-1.1.6/src/imio/smartweb/common/tests/test_utils.py` & `imio.smartweb.common-1.1.7/src/imio/smartweb/common/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.common-1.1.6/src/imio/smartweb/common/tests/test_viewlets.py` & `imio.smartweb.common-1.1.7/src/imio/smartweb/common/tests/test_viewlets.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.common-1.1.6/src/imio/smartweb/common/tests/test_vocabularies.py` & `imio.smartweb.common-1.1.7/src/imio/smartweb/common/tests/test_vocabularies.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.common-1.1.6/src/imio/smartweb/common/upgrades/configure.zcml` & `imio.smartweb.common-1.1.7/src/imio/smartweb/common/upgrades/configure.zcml`

 * *Files 3% similar despite different names*

```diff
@@ -64,14 +64,22 @@
       name="upgrade_1015_to_1016"
       title="Upgrade common from 1015 to 1016"
       directory="profiles/1015_to_1016"
       description="Patch (Remove select2) eea.facetednavigation jquery"
       provides="Products.GenericSetup.interfaces.EXTENSION"
       />
 
+  <genericsetup:registerProfile
+      name="upgrade_1016_to_1017"
+      title="Upgrade common from 1016 to 1017"
+      directory="profiles/1016_to_1017"
+      description="Change banner scale to have infinite height"
+      provides="Products.GenericSetup.interfaces.EXTENSION"
+      />
+
   <genericsetup:upgradeStep
       title="Configure first official release"
       description="Run needed registry step"
       source="1000"
       destination="1001"
       handler=".upgrades.reload_registry"
       profile="imio.smartweb.common:default"
@@ -232,8 +240,18 @@
       profile="imio.smartweb.common:default">
     <genericsetup:upgradeDepends
         title="Patch (Remove select2) eea.facetednavigation jquery"
         import_profile="imio.smartweb.common.upgrades:upgrade_1015_to_1016"
         />
   </genericsetup:upgradeSteps>
 
+  <genericsetup:upgradeSteps
+      source="1016"
+      destination="1017"
+      profile="imio.smartweb.common:default">
+    <genericsetup:upgradeDepends
+        title="Change banner scale to have infinite height"
+        import_profile="imio.smartweb.common.upgrades:upgrade_1016_to_1017"
+        />
+  </genericsetup:upgradeSteps>
+
 </configure>
```

### Comparing `imio.smartweb.common-1.1.6/src/imio/smartweb/common/upgrades/profiles/1007_to_1008/rolemap.xml` & `imio.smartweb.common-1.1.7/src/imio/smartweb/common/upgrades/profiles/1007_to_1008/rolemap.xml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.common-1.1.6/src/imio/smartweb/common/upgrades/profiles/1008_to_1009/actions.xml` & `imio.smartweb.common-1.1.7/src/imio/smartweb/common/upgrades/profiles/1008_to_1009/actions.xml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.common-1.1.6/src/imio/smartweb/common/upgrades/profiles/1009_to_1010/registry/tiny_nonbreakingspace.xml` & `imio.smartweb.common-1.1.7/src/imio/smartweb/common/upgrades/profiles/1009_to_1010/registry/tiny_nonbreakingspace.xml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.common-1.1.6/src/imio/smartweb/common/upgrades/profiles/1010_to_1011/registry/resources.xml` & `imio.smartweb.common-1.1.7/src/imio/smartweb/common/upgrades/profiles/1010_to_1011/registry/resources.xml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.common-1.1.6/src/imio/smartweb/common/upgrades/profiles/1010_to_1011/registry/scales.xml` & `imio.smartweb.common-1.1.7/src/imio/smartweb/common/upgrades/profiles/1010_to_1011/registry/scales.xml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.common-1.1.6/src/imio/smartweb/common/upgrades/profiles/1010_to_1011/registry/tinymce.xml` & `imio.smartweb.common-1.1.7/src/imio/smartweb/common/upgrades/profiles/1010_to_1011/registry/tinymce.xml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.common-1.1.6/src/imio/smartweb/common/upgrades/profiles/1011_to_1012/registry/bundles.xml` & `imio.smartweb.common-1.1.7/src/imio/smartweb/common/upgrades/profiles/1011_to_1012/registry/bundles.xml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.common-1.1.6/src/imio/smartweb/common/upgrades/profiles/1013_to_1014/registry/tinymce.xml` & `imio.smartweb.common-1.1.7/src/imio/smartweb/common/upgrades/profiles/1013_to_1014/registry/tinymce.xml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.common-1.1.6/src/imio/smartweb/common/upgrades/upgrades.py` & `imio.smartweb.common-1.1.7/src/imio/smartweb/common/upgrades/upgrades.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.common-1.1.6/src/imio/smartweb/common/utils.py` & `imio.smartweb.common-1.1.7/src/imio/smartweb/common/utils.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.common-1.1.6/src/imio/smartweb/common/viewlets/colophon.pt` & `imio.smartweb.common-1.1.7/src/imio/smartweb/common/viewlets/colophon.pt`

 * *Files identical despite different names*

### Comparing `imio.smartweb.common-1.1.6/src/imio/smartweb/common/viewlets/colophon.py` & `imio.smartweb.common-1.1.7/src/imio/smartweb/common/viewlets/colophon.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.common-1.1.6/src/imio/smartweb/common/viewlets/configure.zcml` & `imio.smartweb.common-1.1.7/src/imio/smartweb/common/viewlets/configure.zcml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.common-1.1.6/src/imio/smartweb/common/viewlets/privacy.pt` & `imio.smartweb.common-1.1.7/src/imio/smartweb/common/viewlets/privacy.pt`

 * *Files identical despite different names*

### Comparing `imio.smartweb.common-1.1.6/src/imio/smartweb/common/vocabularies.py` & `imio.smartweb.common-1.1.7/src/imio/smartweb/common/vocabularies.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.common-1.1.6/src/imio/smartweb/common/vocabularies.zcml` & `imio.smartweb.common-1.1.7/src/imio/smartweb/common/vocabularies.zcml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.common-1.1.6/src/imio.smartweb.common.egg-info/PKG-INFO` & `imio.smartweb.common-1.1.7/src/imio.smartweb.common.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: imio.smartweb.common
-Version: 1.1.6
+Version: 1.1.7
 Summary: Common utilities, vocabularies, taxonomies for imio.smartweb & co products
 Home-page: https://github.com/imio/imio.smartweb.common
 Author: iMio
 Author-email: christophe.boulanger@imio.be
 License: GPL version 2
 Project-URL: PyPI, https://pypi.python.org/pypi/imio.smartweb.common
 Project-URL: Source, https://github.com/imio/imio.smartweb.common
 Project-URL: Tracker, https://github.com/imio/imio.smartweb.common/issues
 Keywords: Python Plone CMS
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Plone
 Classifier: Framework :: Plone :: Addon
 Classifier: Framework :: Plone :: 6.0
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -132,14 +131,24 @@
 - iMio, christophe.boulanger@imio.be
 
 
 Changelog
 =========
 
 
+1.1.7 (2023-05-22)
+------------------
+
+- Change banner scale to have infinite height
+  [laulaz]
+
+- Migrate to Plone 6.0.4
+  [boulch]
+
+
 1.1.6 (2023-04-14)
 ------------------
 
 - Don't use image_scales metadata anymore (Fix faceted)
   [boulch, laulaz]
 
 - Update object modification date if cropping was removed/updated
@@ -421,9 +430,7 @@
 
 
 1.0a1 (2021-11-05)
 ------------------
 
 - Initial release.
   [boulch]
-
-
```

### Comparing `imio.smartweb.common-1.1.6/src/imio.smartweb.common.egg-info/SOURCES.txt` & `imio.smartweb.common-1.1.7/src/imio.smartweb.common.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -122,13 +122,14 @@
 src/imio/smartweb/common/upgrades/profiles/1010_to_1011/registry/resources.xml
 src/imio/smartweb/common/upgrades/profiles/1010_to_1011/registry/scales.xml
 src/imio/smartweb/common/upgrades/profiles/1010_to_1011/registry/tinymce.xml
 src/imio/smartweb/common/upgrades/profiles/1011_to_1012/registry/bundles.xml
 src/imio/smartweb/common/upgrades/profiles/1013_to_1014/registry/tinymce.xml
 src/imio/smartweb/common/upgrades/profiles/1014_to_1015/registry/syndication.xml
 src/imio/smartweb/common/upgrades/profiles/1015_to_1016/registry/patched-faceted-jquery.xml
+src/imio/smartweb/common/upgrades/profiles/1016_to_1017/registry/scales.xml
 src/imio/smartweb/common/viewlets/__init__.py
 src/imio/smartweb/common/viewlets/analytics.pt
 src/imio/smartweb/common/viewlets/colophon.pt
 src/imio/smartweb/common/viewlets/colophon.py
 src/imio/smartweb/common/viewlets/configure.zcml
 src/imio/smartweb/common/viewlets/privacy.pt
```

