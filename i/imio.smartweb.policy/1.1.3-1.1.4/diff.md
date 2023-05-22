# Comparing `tmp/imio.smartweb.policy-1.1.3.tar.gz` & `tmp/imio.smartweb.policy-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/imio.smartweb.policy-1.1.3.tar", last modified: Fri Feb 17 12:55:26 2023, max compression
+gzip compressed data, was "imio.smartweb.policy-1.1.4.tar", last modified: Mon May 22 07:07:34 2023, max compression
```

## Comparing `imio.smartweb.policy-1.1.3.tar` & `imio.smartweb.policy-1.1.4.tar`

### file list

```diff
@@ -1,137 +1,141 @@
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-02-17 12:55:26.000000 imio.smartweb.policy-1.1.3/
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-02-17 12:55:26.000000 imio.smartweb.policy-1.1.3/docs/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     7998 2023-02-17 12:55:26.000000 imio.smartweb.policy-1.1.3/docs/conf.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)       83 2023-02-17 12:55:26.000000 imio.smartweb.policy-1.1.3/docs/index.rst
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      520 2023-02-17 12:55:26.000000 imio.smartweb.policy-1.1.3/DEVELOP.rst
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)    14050 2023-02-17 12:55:26.000000 imio.smartweb.policy-1.1.3/PKG-INFO
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)       80 2023-02-17 12:55:26.000000 imio.smartweb.policy-1.1.3/CONTRIBUTORS.rst
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2090 2023-02-17 12:55:26.000000 imio.smartweb.policy-1.1.3/README.rst
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     7071 2023-02-17 12:55:26.000000 imio.smartweb.policy-1.1.3/CHANGES.rst
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)       61 2023-02-17 12:55:26.000000 imio.smartweb.policy-1.1.3/MANIFEST.in
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2890 2023-02-17 12:55:26.000000 imio.smartweb.policy-1.1.3/setup.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      671 2023-02-17 12:55:26.000000 imio.smartweb.policy-1.1.3/LICENSE.rst
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      518 2023-02-17 12:55:26.000000 imio.smartweb.policy-1.1.3/setup.cfg
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-02-17 12:55:26.000000 imio.smartweb.policy-1.1.3/src/
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-02-17 12:55:26.000000 imio.smartweb.policy-1.1.3/src/imio/
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-02-17 12:55:26.000000 imio.smartweb.policy-1.1.3/src/imio/smartweb/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)       80 2023-02-17 12:55:26.000000 imio.smartweb.policy-1.1.3/src/imio/smartweb/__init__.py
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-02-17 12:55:26.000000 imio.smartweb.policy-1.1.3/src/imio/smartweb/policy/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1749 2023-02-17 12:55:26.000000 imio.smartweb.policy-1.1.3/src/imio/smartweb/policy/testing.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      268 2023-02-17 12:55:26.000000 imio.smartweb.policy-1.1.3/src/imio/smartweb/policy/interfaces.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     4308 2023-02-17 12:55:26.000000 imio.smartweb.policy-1.1.3/src/imio/smartweb/policy/setuphandlers.py
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-02-17 12:55:26.000000 imio.smartweb.policy-1.1.3/src/imio/smartweb/policy/tests/
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-02-17 12:55:26.000000 imio.smartweb.policy-1.1.3/src/imio/smartweb/policy/tests/robot/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2011 2023-02-17 12:55:26.000000 imio.smartweb.policy-1.1.3/src/imio/smartweb/policy/tests/robot/test_example.robot
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-02-17 12:55:26.000000 imio.smartweb.policy-1.1.3/src/imio/smartweb/policy/tests/__init__.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2102 2023-02-17 12:55:26.000000 imio.smartweb.policy-1.1.3/src/imio/smartweb/policy/tests/test_setup.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      955 2023-02-17 12:55:26.000000 imio.smartweb.policy-1.1.3/src/imio/smartweb/policy/tests/test_robot.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      497 2023-02-17 12:55:26.000000 imio.smartweb.policy-1.1.3/src/imio/smartweb/policy/overrides.zcml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      864 2023-02-17 12:55:26.000000 imio.smartweb.policy-1.1.3/src/imio/smartweb/policy/pattern_settings.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      814 2023-02-17 12:55:26.000000 imio.smartweb.policy-1.1.3/src/imio/smartweb/policy/caching.zcml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      533 2023-02-17 12:55:26.000000 imio.smartweb.policy-1.1.3/src/imio/smartweb/policy/caching.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2250 2023-02-17 12:55:26.000000 imio.smartweb.policy-1.1.3/src/imio/smartweb/policy/setupdemo.py
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-02-17 12:55:26.000000 imio.smartweb.policy-1.1.3/src/imio/smartweb/policy/profiles/
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-02-17 12:55:26.000000 imio.smartweb.policy-1.1.3/src/imio/smartweb/policy/profiles/multilingual/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1432 2023-02-17 12:55:26.000000 imio.smartweb.policy-1.1.3/src/imio/smartweb/policy/profiles/multilingual/registry.xml
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-02-17 12:55:26.000000 imio.smartweb.policy-1.1.3/src/imio/smartweb/policy/profiles/uninstall/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      205 2023-02-17 12:55:26.000000 imio.smartweb.policy-1.1.3/src/imio/smartweb/policy/profiles/uninstall/browserlayer.xml
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-02-17 12:55:26.000000 imio.smartweb.policy-1.1.3/src/imio/smartweb/policy/profiles/default/
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-02-17 12:55:26.000000 imio.smartweb.policy-1.1.3/src/imio/smartweb/policy/profiles/default/types/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      216 2023-02-17 12:55:26.000000 imio.smartweb.policy-1.1.3/src/imio/smartweb/policy/profiles/default/types/News_Item.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      215 2023-02-17 12:55:26.000000 imio.smartweb.policy-1.1.3/src/imio/smartweb/policy/profiles/default/types/Document.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      212 2023-02-17 12:55:26.000000 imio.smartweb.policy-1.1.3/src/imio/smartweb/policy/profiles/default/types/Event.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      355 2023-02-17 12:55:26.000000 imio.smartweb.policy-1.1.3/src/imio/smartweb/policy/profiles/default/types/Image.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      591 2023-02-17 12:55:26.000000 imio.smartweb.policy-1.1.3/src/imio/smartweb/policy/profiles/default/types/File.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      468 2023-02-17 12:55:26.000000 imio.smartweb.policy-1.1.3/src/imio/smartweb/policy/profiles/default/types/Collection.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      354 2023-02-17 12:55:26.000000 imio.smartweb.policy-1.1.3/src/imio/smartweb/policy/profiles/default/types/Link.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      186 2023-02-17 12:55:26.000000 imio.smartweb.policy-1.1.3/src/imio/smartweb/policy/profiles/default/types/Plone_Site.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      213 2023-02-17 12:55:26.000000 imio.smartweb.policy-1.1.3/src/imio/smartweb/policy/profiles/default/types/Folder.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1177 2023-02-17 12:55:26.000000 imio.smartweb.policy-1.1.3/src/imio/smartweb/policy/profiles/default/controlpanel.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      780 2023-02-17 12:55:26.000000 imio.smartweb.policy-1.1.3/src/imio/smartweb/policy/profiles/default/metadata.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2901 2023-02-17 12:55:26.000000 imio.smartweb.policy-1.1.3/src/imio/smartweb/policy/profiles/default/viewlets.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1870 2023-02-17 12:55:26.000000 imio.smartweb.policy-1.1.3/src/imio/smartweb/policy/profiles/default/rolemap.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      185 2023-02-17 12:55:26.000000 imio.smartweb.policy-1.1.3/src/imio/smartweb/policy/profiles/default/browserlayer.xml
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-02-17 12:55:26.000000 imio.smartweb.policy-1.1.3/src/imio/smartweb/policy/profiles/default/registry/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     8287 2023-02-17 12:55:26.000000 imio.smartweb.policy-1.1.3/src/imio/smartweb/policy/profiles/default/registry/autopublishing.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      961 2023-02-17 12:55:26.000000 imio.smartweb.policy-1.1.3/src/imio/smartweb/policy/profiles/default/registry/smartweb.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     4086 2023-02-17 12:55:26.000000 imio.smartweb.policy-1.1.3/src/imio/smartweb/policy/profiles/default/registry/caching.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      417 2023-02-17 12:55:26.000000 imio.smartweb.policy-1.1.3/src/imio/smartweb/policy/profiles/default/registry/messagesviewlet.xml
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-02-17 12:55:26.000000 imio.smartweb.policy-1.1.3/src/imio/smartweb/policy/profiles/demo/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      189 2023-02-17 12:55:26.000000 imio.smartweb.policy-1.1.3/src/imio/smartweb/policy/profiles/demo/metadata.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      234 2023-02-17 12:55:26.000000 imio.smartweb.policy-1.1.3/src/imio/smartweb/policy/subscribers.zcml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1585 2023-02-17 12:55:26.000000 imio.smartweb.policy-1.1.3/src/imio/smartweb/policy/profiles.zcml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2954 2023-02-17 12:55:26.000000 imio.smartweb.policy-1.1.3/src/imio/smartweb/policy/utils.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      350 2023-02-17 12:55:26.000000 imio.smartweb.policy-1.1.3/src/imio/smartweb/policy/permissions.zcml
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-02-17 12:55:26.000000 imio.smartweb.policy-1.1.3/src/imio/smartweb/policy/upgrades/
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-02-17 12:55:26.000000 imio.smartweb.policy-1.1.3/src/imio/smartweb/policy/upgrades/profiles/
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-02-17 12:55:26.000000 imio.smartweb.policy-1.1.3/src/imio/smartweb/policy/upgrades/profiles/1023_to_1024/
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-02-17 12:55:26.000000 imio.smartweb.policy-1.1.3/src/imio/smartweb/policy/upgrades/profiles/1023_to_1024/registry/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      332 2023-02-17 12:55:26.000000 imio.smartweb.policy-1.1.3/src/imio/smartweb/policy/upgrades/profiles/1023_to_1024/registry/bundles.xml
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-02-17 12:55:26.000000 imio.smartweb.policy-1.1.3/src/imio/smartweb/policy/upgrades/profiles/1006_to_1007/
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-02-17 12:55:26.000000 imio.smartweb.policy-1.1.3/src/imio/smartweb/policy/upgrades/profiles/1006_to_1007/registry/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     3749 2023-02-17 12:55:26.000000 imio.smartweb.policy-1.1.3/src/imio/smartweb/policy/upgrades/profiles/1006_to_1007/registry/caching.xml
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-02-17 12:55:26.000000 imio.smartweb.policy-1.1.3/src/imio/smartweb/policy/upgrades/profiles/1028_to_1029/
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-02-17 12:55:26.000000 imio.smartweb.policy-1.1.3/src/imio/smartweb/policy/upgrades/profiles/1028_to_1029/registry/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      417 2023-02-17 12:55:26.000000 imio.smartweb.policy-1.1.3/src/imio/smartweb/policy/upgrades/profiles/1028_to_1029/registry/messagesviewlet.xml
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-02-17 12:55:26.000000 imio.smartweb.policy-1.1.3/src/imio/smartweb/policy/upgrades/profiles/1019_to_1020/
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-02-17 12:55:26.000000 imio.smartweb.policy-1.1.3/src/imio/smartweb/policy/upgrades/profiles/1019_to_1020/registry/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      235 2023-02-17 12:55:26.000000 imio.smartweb.policy-1.1.3/src/imio/smartweb/policy/upgrades/profiles/1019_to_1020/registry/caching.xml
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-02-17 12:55:26.000000 imio.smartweb.policy-1.1.3/src/imio/smartweb/policy/upgrades/profiles/1011_to_1012/
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-02-17 12:55:26.000000 imio.smartweb.policy-1.1.3/src/imio/smartweb/policy/upgrades/profiles/1011_to_1012/registry/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1307 2023-02-17 12:55:26.000000 imio.smartweb.policy-1.1.3/src/imio/smartweb/policy/upgrades/profiles/1011_to_1012/registry/collective.autoscaling.values.xml
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-02-17 12:55:26.000000 imio.smartweb.policy-1.1.3/src/imio/smartweb/policy/upgrades/profiles/1017_to_1018/
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-02-17 12:55:26.000000 imio.smartweb.policy-1.1.3/src/imio/smartweb/policy/upgrades/profiles/1017_to_1018/registry/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      311 2023-02-17 12:55:26.000000 imio.smartweb.policy-1.1.3/src/imio/smartweb/policy/upgrades/profiles/1017_to_1018/registry/smartweb.xml
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-02-17 12:55:26.000000 imio.smartweb.policy-1.1.3/src/imio/smartweb/policy/upgrades/profiles/1013_to_1014/
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-02-17 12:55:26.000000 imio.smartweb.policy-1.1.3/src/imio/smartweb/policy/upgrades/profiles/1013_to_1014/registry/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      561 2023-02-17 12:55:26.000000 imio.smartweb.policy-1.1.3/src/imio/smartweb/policy/upgrades/profiles/1013_to_1014/registry/collective.autoscaling.values.xml
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-02-17 12:55:26.000000 imio.smartweb.policy-1.1.3/src/imio/smartweb/policy/upgrades/profiles/1021_to_1022/
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-02-17 12:55:26.000000 imio.smartweb.policy-1.1.3/src/imio/smartweb/policy/upgrades/profiles/1021_to_1022/registry/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     3970 2023-02-17 12:55:26.000000 imio.smartweb.policy-1.1.3/src/imio/smartweb/policy/upgrades/profiles/1021_to_1022/registry/caching.xml
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-02-17 12:55:26.000000 imio.smartweb.policy-1.1.3/src/imio/smartweb/policy/upgrades/profiles/1022_to_1023/
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-02-17 12:55:26.000000 imio.smartweb.policy-1.1.3/src/imio/smartweb/policy/upgrades/profiles/1022_to_1023/registry/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     4086 2023-02-17 12:55:26.000000 imio.smartweb.policy-1.1.3/src/imio/smartweb/policy/upgrades/profiles/1022_to_1023/registry/caching.xml
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-02-17 12:55:26.000000 imio.smartweb.policy-1.1.3/src/imio/smartweb/policy/upgrades/profiles/1010_to_1011/
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-02-17 12:55:26.000000 imio.smartweb.policy-1.1.3/src/imio/smartweb/policy/upgrades/profiles/1010_to_1011/registry/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      148 2023-02-17 12:55:26.000000 imio.smartweb.policy-1.1.3/src/imio/smartweb/policy/upgrades/profiles/1010_to_1011/registry/caching.xml
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-02-17 12:55:26.000000 imio.smartweb.policy-1.1.3/src/imio/smartweb/policy/upgrades/profiles/1020_to_1021/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1177 2023-02-17 12:55:26.000000 imio.smartweb.policy-1.1.3/src/imio/smartweb/policy/upgrades/profiles/1020_to_1021/controlpanel.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1787 2023-02-17 12:55:26.000000 imio.smartweb.policy-1.1.3/src/imio/smartweb/policy/upgrades/profiles/1020_to_1021/rolemap.xml
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-02-17 12:55:26.000000 imio.smartweb.policy-1.1.3/src/imio/smartweb/policy/upgrades/profiles/1018_to_1019/
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-02-17 12:55:26.000000 imio.smartweb.policy-1.1.3/src/imio/smartweb/policy/upgrades/profiles/1018_to_1019/registry/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      235 2023-02-17 12:55:26.000000 imio.smartweb.policy-1.1.3/src/imio/smartweb/policy/upgrades/profiles/1018_to_1019/registry/smartweb.xml
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-02-17 12:55:26.000000 imio.smartweb.policy-1.1.3/src/imio/smartweb/policy/upgrades/profiles/1014_to_1015/
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-02-17 12:55:26.000000 imio.smartweb.policy-1.1.3/src/imio/smartweb/policy/upgrades/profiles/1014_to_1015/registry/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      515 2023-02-17 12:55:26.000000 imio.smartweb.policy-1.1.3/src/imio/smartweb/policy/upgrades/profiles/1014_to_1015/registry/caching.xml
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-02-17 12:55:26.000000 imio.smartweb.policy-1.1.3/src/imio/smartweb/policy/upgrades/profiles/1008_to_1009/
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-02-17 12:55:26.000000 imio.smartweb.policy-1.1.3/src/imio/smartweb/policy/upgrades/profiles/1008_to_1009/registry/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      136 2023-02-17 12:55:26.000000 imio.smartweb.policy-1.1.3/src/imio/smartweb/policy/upgrades/profiles/1008_to_1009/registry/caching.xml
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-02-17 12:55:26.000000 imio.smartweb.policy-1.1.3/src/imio/smartweb/policy/upgrades/profiles/1026_to_1027/
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-02-17 12:55:26.000000 imio.smartweb.policy-1.1.3/src/imio/smartweb/policy/upgrades/profiles/1026_to_1027/registry/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     8287 2023-02-17 12:55:26.000000 imio.smartweb.policy-1.1.3/src/imio/smartweb/policy/upgrades/profiles/1026_to_1027/registry/autopublishing.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1586 2023-02-17 12:55:26.000000 imio.smartweb.policy-1.1.3/src/imio/smartweb/policy/upgrades/upgrades.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-02-17 12:55:26.000000 imio.smartweb.policy-1.1.3/src/imio/smartweb/policy/upgrades/__init__.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)    14858 2023-02-17 12:55:26.000000 imio.smartweb.policy-1.1.3/src/imio/smartweb/policy/upgrades/configure.zcml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      290 2023-02-17 12:55:26.000000 imio.smartweb.policy-1.1.3/src/imio/smartweb/policy/__init__.py
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-02-17 12:55:26.000000 imio.smartweb.policy-1.1.3/src/imio/smartweb/policy/browser/
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-02-17 12:55:26.000000 imio.smartweb.policy-1.1.3/src/imio/smartweb/policy/browser/faceted/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      707 2023-02-17 12:55:26.000000 imio.smartweb.policy-1.1.3/src/imio/smartweb/policy/browser/faceted/subtyper.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-02-17 12:55:26.000000 imio.smartweb.policy-1.1.3/src/imio/smartweb/policy/browser/faceted/__init__.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      944 2023-02-17 12:55:26.000000 imio.smartweb.policy-1.1.3/src/imio/smartweb/policy/browser/faceted/configure.zcml
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-02-17 12:55:26.000000 imio.smartweb.policy-1.1.3/src/imio/smartweb/policy/browser/static/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-02-17 12:55:26.000000 imio.smartweb.policy-1.1.3/src/imio/smartweb/policy/browser/static/.gitkeep
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-02-17 12:55:26.000000 imio.smartweb.policy-1.1.3/src/imio/smartweb/policy/browser/overrides/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-02-17 12:55:26.000000 imio.smartweb.policy-1.1.3/src/imio/smartweb/policy/browser/overrides/.gitkeep
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-02-17 12:55:26.000000 imio.smartweb.policy-1.1.3/src/imio/smartweb/policy/browser/__init__.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1326 2023-02-17 12:55:26.000000 imio.smartweb.policy-1.1.3/src/imio/smartweb/policy/browser/configure.zcml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1200 2023-02-17 12:55:26.000000 imio.smartweb.policy-1.1.3/src/imio/smartweb/policy/viewlets.zcml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1529 2023-02-17 12:55:26.000000 imio.smartweb.policy-1.1.3/src/imio/smartweb/policy/configure.zcml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)       80 2023-02-17 12:55:26.000000 imio.smartweb.policy-1.1.3/src/imio/__init__.py
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-02-17 12:55:26.000000 imio.smartweb.policy-1.1.3/src/imio.smartweb.policy.egg-info/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        5 2023-02-17 12:55:26.000000 imio.smartweb.policy-1.1.3/src/imio.smartweb.policy.egg-info/top_level.txt
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)    14050 2023-02-17 12:55:26.000000 imio.smartweb.policy-1.1.3/src/imio.smartweb.policy.egg-info/PKG-INFO
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        1 2023-02-17 12:55:26.000000 imio.smartweb.policy-1.1.3/src/imio.smartweb.policy.egg-info/dependency_links.txt
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      518 2023-02-17 12:55:26.000000 imio.smartweb.policy-1.1.3/src/imio.smartweb.policy.egg-info/requires.txt
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)       19 2023-02-17 12:55:26.000000 imio.smartweb.policy-1.1.3/src/imio.smartweb.policy.egg-info/namespace_packages.txt
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     4330 2023-02-17 12:55:26.000000 imio.smartweb.policy-1.1.3/src/imio.smartweb.policy.egg-info/SOURCES.txt
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        1 2023-02-17 12:55:26.000000 imio.smartweb.policy-1.1.3/src/imio.smartweb.policy.egg-info/not-zip-safe
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-05-22 07:07:34.990144 imio.smartweb.policy-1.1.4/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     7267 2023-05-22 07:07:34.000000 imio.smartweb.policy-1.1.4/CHANGES.rst
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)       80 2023-05-22 07:07:34.000000 imio.smartweb.policy-1.1.4/CONTRIBUTORS.rst
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      520 2023-05-22 07:07:34.000000 imio.smartweb.policy-1.1.4/DEVELOP.rst
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)    18092 2023-05-22 07:07:34.000000 imio.smartweb.policy-1.1.4/LICENSE.GPL
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      671 2023-05-22 07:07:34.000000 imio.smartweb.policy-1.1.4/LICENSE.rst
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)       61 2023-05-22 07:07:34.000000 imio.smartweb.policy-1.1.4/MANIFEST.in
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)    10491 2023-05-22 07:07:34.990144 imio.smartweb.policy-1.1.4/PKG-INFO
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2090 2023-05-22 07:07:34.000000 imio.smartweb.policy-1.1.4/README.rst
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-05-22 07:07:34.982144 imio.smartweb.policy-1.1.4/docs/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     7998 2023-05-22 07:07:34.000000 imio.smartweb.policy-1.1.4/docs/conf.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)       83 2023-05-22 07:07:34.000000 imio.smartweb.policy-1.1.4/docs/index.rst
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      518 2023-05-22 07:07:34.990144 imio.smartweb.policy-1.1.4/setup.cfg
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2890 2023-05-22 07:07:34.000000 imio.smartweb.policy-1.1.4/setup.py
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-05-22 07:07:34.978144 imio.smartweb.policy-1.1.4/src/
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-05-22 07:07:34.982144 imio.smartweb.policy-1.1.4/src/imio/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)       80 2023-05-22 07:07:34.000000 imio.smartweb.policy-1.1.4/src/imio/__init__.py
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-05-22 07:07:34.982144 imio.smartweb.policy-1.1.4/src/imio/smartweb/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)       80 2023-05-22 07:07:34.000000 imio.smartweb.policy-1.1.4/src/imio/smartweb/__init__.py
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-05-22 07:07:34.986144 imio.smartweb.policy-1.1.4/src/imio/smartweb/policy/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      290 2023-05-22 07:07:34.000000 imio.smartweb.policy-1.1.4/src/imio/smartweb/policy/__init__.py
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-05-22 07:07:34.986144 imio.smartweb.policy-1.1.4/src/imio/smartweb/policy/browser/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-05-22 07:07:34.000000 imio.smartweb.policy-1.1.4/src/imio/smartweb/policy/browser/__init__.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1326 2023-05-22 07:07:34.000000 imio.smartweb.policy-1.1.4/src/imio/smartweb/policy/browser/configure.zcml
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-05-22 07:07:34.986144 imio.smartweb.policy-1.1.4/src/imio/smartweb/policy/browser/faceted/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-05-22 07:07:34.000000 imio.smartweb.policy-1.1.4/src/imio/smartweb/policy/browser/faceted/__init__.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      944 2023-05-22 07:07:34.000000 imio.smartweb.policy-1.1.4/src/imio/smartweb/policy/browser/faceted/configure.zcml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      707 2023-05-22 07:07:34.000000 imio.smartweb.policy-1.1.4/src/imio/smartweb/policy/browser/faceted/subtyper.py
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-05-22 07:07:34.986144 imio.smartweb.policy-1.1.4/src/imio/smartweb/policy/browser/overrides/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-05-22 07:07:34.000000 imio.smartweb.policy-1.1.4/src/imio/smartweb/policy/browser/overrides/.gitkeep
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-05-22 07:07:34.986144 imio.smartweb.policy-1.1.4/src/imio/smartweb/policy/browser/static/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-05-22 07:07:34.000000 imio.smartweb.policy-1.1.4/src/imio/smartweb/policy/browser/static/.gitkeep
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      533 2023-05-22 07:07:34.000000 imio.smartweb.policy-1.1.4/src/imio/smartweb/policy/caching.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      814 2023-05-22 07:07:34.000000 imio.smartweb.policy-1.1.4/src/imio/smartweb/policy/caching.zcml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1529 2023-05-22 07:07:34.000000 imio.smartweb.policy-1.1.4/src/imio/smartweb/policy/configure.zcml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      268 2023-05-22 07:07:34.000000 imio.smartweb.policy-1.1.4/src/imio/smartweb/policy/interfaces.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      497 2023-05-22 07:07:34.000000 imio.smartweb.policy-1.1.4/src/imio/smartweb/policy/overrides.zcml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      864 2023-05-22 07:07:34.000000 imio.smartweb.policy-1.1.4/src/imio/smartweb/policy/pattern_settings.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      549 2023-05-22 07:07:34.000000 imio.smartweb.policy-1.1.4/src/imio/smartweb/policy/permissions.zcml
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-05-22 07:07:34.982144 imio.smartweb.policy-1.1.4/src/imio/smartweb/policy/profiles/
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-05-22 07:07:34.986144 imio.smartweb.policy-1.1.4/src/imio/smartweb/policy/profiles/default/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      185 2023-05-22 07:07:34.000000 imio.smartweb.policy-1.1.4/src/imio/smartweb/policy/profiles/default/browserlayer.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1177 2023-05-22 07:07:34.000000 imio.smartweb.policy-1.1.4/src/imio/smartweb/policy/profiles/default/controlpanel.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      780 2023-05-22 07:07:34.000000 imio.smartweb.policy-1.1.4/src/imio/smartweb/policy/profiles/default/metadata.xml
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-05-22 07:07:34.986144 imio.smartweb.policy-1.1.4/src/imio/smartweb/policy/profiles/default/registry/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     8287 2023-05-22 07:07:34.000000 imio.smartweb.policy-1.1.4/src/imio/smartweb/policy/profiles/default/registry/autopublishing.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     4086 2023-05-22 07:07:34.000000 imio.smartweb.policy-1.1.4/src/imio/smartweb/policy/profiles/default/registry/caching.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      296 2023-05-22 07:07:34.000000 imio.smartweb.policy-1.1.4/src/imio/smartweb/policy/profiles/default/registry/messagesviewlet.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      961 2023-05-22 07:07:34.000000 imio.smartweb.policy-1.1.4/src/imio/smartweb/policy/profiles/default/registry/smartweb.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2026 2023-05-22 07:07:34.000000 imio.smartweb.policy-1.1.4/src/imio/smartweb/policy/profiles/default/rolemap.xml
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-05-22 07:07:34.986144 imio.smartweb.policy-1.1.4/src/imio/smartweb/policy/profiles/default/types/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      468 2023-05-22 07:07:34.000000 imio.smartweb.policy-1.1.4/src/imio/smartweb/policy/profiles/default/types/Collection.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      215 2023-05-22 07:07:34.000000 imio.smartweb.policy-1.1.4/src/imio/smartweb/policy/profiles/default/types/Document.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      212 2023-05-22 07:07:34.000000 imio.smartweb.policy-1.1.4/src/imio/smartweb/policy/profiles/default/types/Event.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      591 2023-05-22 07:07:34.000000 imio.smartweb.policy-1.1.4/src/imio/smartweb/policy/profiles/default/types/File.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      213 2023-05-22 07:07:34.000000 imio.smartweb.policy-1.1.4/src/imio/smartweb/policy/profiles/default/types/Folder.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      355 2023-05-22 07:07:34.000000 imio.smartweb.policy-1.1.4/src/imio/smartweb/policy/profiles/default/types/Image.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      354 2023-05-22 07:07:34.000000 imio.smartweb.policy-1.1.4/src/imio/smartweb/policy/profiles/default/types/Link.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      216 2023-05-22 07:07:34.000000 imio.smartweb.policy-1.1.4/src/imio/smartweb/policy/profiles/default/types/News_Item.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      186 2023-05-22 07:07:34.000000 imio.smartweb.policy-1.1.4/src/imio/smartweb/policy/profiles/default/types/Plone_Site.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2901 2023-05-22 07:07:34.000000 imio.smartweb.policy-1.1.4/src/imio/smartweb/policy/profiles/default/viewlets.xml
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-05-22 07:07:34.986144 imio.smartweb.policy-1.1.4/src/imio/smartweb/policy/profiles/demo/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      189 2023-05-22 07:07:34.000000 imio.smartweb.policy-1.1.4/src/imio/smartweb/policy/profiles/demo/metadata.xml
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-05-22 07:07:34.986144 imio.smartweb.policy-1.1.4/src/imio/smartweb/policy/profiles/multilingual/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1432 2023-05-22 07:07:34.000000 imio.smartweb.policy-1.1.4/src/imio/smartweb/policy/profiles/multilingual/registry.xml
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-05-22 07:07:34.986144 imio.smartweb.policy-1.1.4/src/imio/smartweb/policy/profiles/uninstall/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      205 2023-05-22 07:07:34.000000 imio.smartweb.policy-1.1.4/src/imio/smartweb/policy/profiles/uninstall/browserlayer.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1585 2023-05-22 07:07:34.000000 imio.smartweb.policy-1.1.4/src/imio/smartweb/policy/profiles.zcml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2250 2023-05-22 07:07:34.000000 imio.smartweb.policy-1.1.4/src/imio/smartweb/policy/setupdemo.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     4308 2023-05-22 07:07:34.000000 imio.smartweb.policy-1.1.4/src/imio/smartweb/policy/setuphandlers.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      234 2023-05-22 07:07:34.000000 imio.smartweb.policy-1.1.4/src/imio/smartweb/policy/subscribers.zcml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1749 2023-05-22 07:07:34.000000 imio.smartweb.policy-1.1.4/src/imio/smartweb/policy/testing.py
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-05-22 07:07:34.986144 imio.smartweb.policy-1.1.4/src/imio/smartweb/policy/tests/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-05-22 07:07:34.000000 imio.smartweb.policy-1.1.4/src/imio/smartweb/policy/tests/__init__.py
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-05-22 07:07:34.986144 imio.smartweb.policy-1.1.4/src/imio/smartweb/policy/tests/robot/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2011 2023-05-22 07:07:34.000000 imio.smartweb.policy-1.1.4/src/imio/smartweb/policy/tests/robot/test_example.robot
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      955 2023-05-22 07:07:34.000000 imio.smartweb.policy-1.1.4/src/imio/smartweb/policy/tests/test_robot.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2102 2023-05-22 07:07:34.000000 imio.smartweb.policy-1.1.4/src/imio/smartweb/policy/tests/test_setup.py
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-05-22 07:07:34.986144 imio.smartweb.policy-1.1.4/src/imio/smartweb/policy/upgrades/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-05-22 07:07:34.000000 imio.smartweb.policy-1.1.4/src/imio/smartweb/policy/upgrades/__init__.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)    15498 2023-05-22 07:07:34.000000 imio.smartweb.policy-1.1.4/src/imio/smartweb/policy/upgrades/configure.zcml
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-05-22 07:07:34.982144 imio.smartweb.policy-1.1.4/src/imio/smartweb/policy/upgrades/profiles/
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-05-22 07:07:34.982144 imio.smartweb.policy-1.1.4/src/imio/smartweb/policy/upgrades/profiles/1006_to_1007/
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-05-22 07:07:34.986144 imio.smartweb.policy-1.1.4/src/imio/smartweb/policy/upgrades/profiles/1006_to_1007/registry/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     3749 2023-05-22 07:07:34.000000 imio.smartweb.policy-1.1.4/src/imio/smartweb/policy/upgrades/profiles/1006_to_1007/registry/caching.xml
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-05-22 07:07:34.982144 imio.smartweb.policy-1.1.4/src/imio/smartweb/policy/upgrades/profiles/1008_to_1009/
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-05-22 07:07:34.986144 imio.smartweb.policy-1.1.4/src/imio/smartweb/policy/upgrades/profiles/1008_to_1009/registry/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      136 2023-05-22 07:07:34.000000 imio.smartweb.policy-1.1.4/src/imio/smartweb/policy/upgrades/profiles/1008_to_1009/registry/caching.xml
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-05-22 07:07:34.982144 imio.smartweb.policy-1.1.4/src/imio/smartweb/policy/upgrades/profiles/1010_to_1011/
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-05-22 07:07:34.986144 imio.smartweb.policy-1.1.4/src/imio/smartweb/policy/upgrades/profiles/1010_to_1011/registry/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      148 2023-05-22 07:07:34.000000 imio.smartweb.policy-1.1.4/src/imio/smartweb/policy/upgrades/profiles/1010_to_1011/registry/caching.xml
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-05-22 07:07:34.982144 imio.smartweb.policy-1.1.4/src/imio/smartweb/policy/upgrades/profiles/1011_to_1012/
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-05-22 07:07:34.986144 imio.smartweb.policy-1.1.4/src/imio/smartweb/policy/upgrades/profiles/1011_to_1012/registry/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1307 2023-05-22 07:07:34.000000 imio.smartweb.policy-1.1.4/src/imio/smartweb/policy/upgrades/profiles/1011_to_1012/registry/collective.autoscaling.values.xml
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-05-22 07:07:34.982144 imio.smartweb.policy-1.1.4/src/imio/smartweb/policy/upgrades/profiles/1013_to_1014/
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-05-22 07:07:34.986144 imio.smartweb.policy-1.1.4/src/imio/smartweb/policy/upgrades/profiles/1013_to_1014/registry/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      561 2023-05-22 07:07:34.000000 imio.smartweb.policy-1.1.4/src/imio/smartweb/policy/upgrades/profiles/1013_to_1014/registry/collective.autoscaling.values.xml
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-05-22 07:07:34.982144 imio.smartweb.policy-1.1.4/src/imio/smartweb/policy/upgrades/profiles/1014_to_1015/
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-05-22 07:07:34.990144 imio.smartweb.policy-1.1.4/src/imio/smartweb/policy/upgrades/profiles/1014_to_1015/registry/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      515 2023-05-22 07:07:34.000000 imio.smartweb.policy-1.1.4/src/imio/smartweb/policy/upgrades/profiles/1014_to_1015/registry/caching.xml
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-05-22 07:07:34.982144 imio.smartweb.policy-1.1.4/src/imio/smartweb/policy/upgrades/profiles/1017_to_1018/
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-05-22 07:07:34.990144 imio.smartweb.policy-1.1.4/src/imio/smartweb/policy/upgrades/profiles/1017_to_1018/registry/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      311 2023-05-22 07:07:34.000000 imio.smartweb.policy-1.1.4/src/imio/smartweb/policy/upgrades/profiles/1017_to_1018/registry/smartweb.xml
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-05-22 07:07:34.982144 imio.smartweb.policy-1.1.4/src/imio/smartweb/policy/upgrades/profiles/1018_to_1019/
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-05-22 07:07:34.990144 imio.smartweb.policy-1.1.4/src/imio/smartweb/policy/upgrades/profiles/1018_to_1019/registry/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      235 2023-05-22 07:07:34.000000 imio.smartweb.policy-1.1.4/src/imio/smartweb/policy/upgrades/profiles/1018_to_1019/registry/smartweb.xml
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-05-22 07:07:34.982144 imio.smartweb.policy-1.1.4/src/imio/smartweb/policy/upgrades/profiles/1019_to_1020/
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-05-22 07:07:34.990144 imio.smartweb.policy-1.1.4/src/imio/smartweb/policy/upgrades/profiles/1019_to_1020/registry/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      235 2023-05-22 07:07:34.000000 imio.smartweb.policy-1.1.4/src/imio/smartweb/policy/upgrades/profiles/1019_to_1020/registry/caching.xml
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-05-22 07:07:34.990144 imio.smartweb.policy-1.1.4/src/imio/smartweb/policy/upgrades/profiles/1020_to_1021/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1177 2023-05-22 07:07:34.000000 imio.smartweb.policy-1.1.4/src/imio/smartweb/policy/upgrades/profiles/1020_to_1021/controlpanel.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1787 2023-05-22 07:07:34.000000 imio.smartweb.policy-1.1.4/src/imio/smartweb/policy/upgrades/profiles/1020_to_1021/rolemap.xml
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-05-22 07:07:34.982144 imio.smartweb.policy-1.1.4/src/imio/smartweb/policy/upgrades/profiles/1021_to_1022/
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-05-22 07:07:34.990144 imio.smartweb.policy-1.1.4/src/imio/smartweb/policy/upgrades/profiles/1021_to_1022/registry/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     3970 2023-05-22 07:07:34.000000 imio.smartweb.policy-1.1.4/src/imio/smartweb/policy/upgrades/profiles/1021_to_1022/registry/caching.xml
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-05-22 07:07:34.982144 imio.smartweb.policy-1.1.4/src/imio/smartweb/policy/upgrades/profiles/1022_to_1023/
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-05-22 07:07:34.990144 imio.smartweb.policy-1.1.4/src/imio/smartweb/policy/upgrades/profiles/1022_to_1023/registry/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     4086 2023-05-22 07:07:34.000000 imio.smartweb.policy-1.1.4/src/imio/smartweb/policy/upgrades/profiles/1022_to_1023/registry/caching.xml
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-05-22 07:07:34.982144 imio.smartweb.policy-1.1.4/src/imio/smartweb/policy/upgrades/profiles/1023_to_1024/
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-05-22 07:07:34.990144 imio.smartweb.policy-1.1.4/src/imio/smartweb/policy/upgrades/profiles/1023_to_1024/registry/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      332 2023-05-22 07:07:34.000000 imio.smartweb.policy-1.1.4/src/imio/smartweb/policy/upgrades/profiles/1023_to_1024/registry/bundles.xml
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-05-22 07:07:34.982144 imio.smartweb.policy-1.1.4/src/imio/smartweb/policy/upgrades/profiles/1026_to_1027/
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-05-22 07:07:34.990144 imio.smartweb.policy-1.1.4/src/imio/smartweb/policy/upgrades/profiles/1026_to_1027/registry/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     8287 2023-05-22 07:07:34.000000 imio.smartweb.policy-1.1.4/src/imio/smartweb/policy/upgrades/profiles/1026_to_1027/registry/autopublishing.xml
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-05-22 07:07:34.982144 imio.smartweb.policy-1.1.4/src/imio/smartweb/policy/upgrades/profiles/1028_to_1029/
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-05-22 07:07:34.990144 imio.smartweb.policy-1.1.4/src/imio/smartweb/policy/upgrades/profiles/1028_to_1029/registry/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      296 2023-05-22 07:07:34.000000 imio.smartweb.policy-1.1.4/src/imio/smartweb/policy/upgrades/profiles/1028_to_1029/registry/messagesviewlet.xml
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-05-22 07:07:34.990144 imio.smartweb.policy-1.1.4/src/imio/smartweb/policy/upgrades/profiles/1029_to_1030/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      457 2023-05-22 07:07:34.000000 imio.smartweb.policy-1.1.4/src/imio/smartweb/policy/upgrades/profiles/1029_to_1030/controlpanel.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      233 2023-05-22 07:07:34.000000 imio.smartweb.policy-1.1.4/src/imio/smartweb/policy/upgrades/profiles/1029_to_1030/rolemap.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1586 2023-05-22 07:07:34.000000 imio.smartweb.policy-1.1.4/src/imio/smartweb/policy/upgrades/upgrades.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2954 2023-05-22 07:07:34.000000 imio.smartweb.policy-1.1.4/src/imio/smartweb/policy/utils.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1200 2023-05-22 07:07:34.000000 imio.smartweb.policy-1.1.4/src/imio/smartweb/policy/viewlets.zcml
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-05-22 07:07:34.982144 imio.smartweb.policy-1.1.4/src/imio.smartweb.policy.egg-info/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)    10491 2023-05-22 07:07:34.000000 imio.smartweb.policy-1.1.4/src/imio.smartweb.policy.egg-info/PKG-INFO
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     4483 2023-05-22 07:07:34.000000 imio.smartweb.policy-1.1.4/src/imio.smartweb.policy.egg-info/SOURCES.txt
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        1 2023-05-22 07:07:34.000000 imio.smartweb.policy-1.1.4/src/imio.smartweb.policy.egg-info/dependency_links.txt
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)       19 2023-05-22 07:07:34.000000 imio.smartweb.policy-1.1.4/src/imio.smartweb.policy.egg-info/namespace_packages.txt
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        1 2023-05-22 07:07:34.000000 imio.smartweb.policy-1.1.4/src/imio.smartweb.policy.egg-info/not-zip-safe
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      518 2023-05-22 07:07:34.000000 imio.smartweb.policy-1.1.4/src/imio.smartweb.policy.egg-info/requires.txt
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        5 2023-05-22 07:07:34.000000 imio.smartweb.policy-1.1.4/src/imio.smartweb.policy.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `imio.smartweb.policy-1.1.3/docs/conf.py` & `imio.smartweb.policy-1.1.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.policy-1.1.3/DEVELOP.rst` & `imio.smartweb.policy-1.1.4/DEVELOP.rst`

 * *Files identical despite different names*

### Comparing `imio.smartweb.policy-1.1.3/README.rst` & `imio.smartweb.policy-1.1.4/README.rst`

 * *Files identical despite different names*

### Comparing `imio.smartweb.policy-1.1.3/CHANGES.rst` & `imio.smartweb.policy-1.1.4/CHANGES.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,24 @@
 Changelog
 =========
 
 
+1.1.4 (2023-05-22)
+------------------
+
+- Migrate to Plone 6.0.4
+  [boulch]
+
+- Migrate to Plone 6.0.2
+  [boulch]
+
+- WEB-3763 : Add new permission to manage configlets in control panel
+  [boulch]
+
+
 1.1.3 (2023-02-17)
 ------------------
 
 - WEB-3820 : Added collective.geotransform but we don't deploy it automaticaly
   [boulch]
 
 - WEB-3833 : Hide plone.app.multilingual in control panel installable products
```

### Comparing `imio.smartweb.policy-1.1.3/setup.py` & `imio.smartweb.policy-1.1.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
         open("CHANGES.rst").read(),
     ]
 )
 
 
 setup(
     name="imio.smartweb.policy",
-    version="1.1.3",
+    version="1.1.4",
     description="Policies to setup imio.smartweb",
     long_description=long_description,
     # Get more from https://pypi.org/classifiers/
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Environment :: Web Environment",
         "Framework :: Plone",
```

### Comparing `imio.smartweb.policy-1.1.3/LICENSE.rst` & `imio.smartweb.policy-1.1.4/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `imio.smartweb.policy-1.1.3/setup.cfg` & `imio.smartweb.policy-1.1.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `imio.smartweb.policy-1.1.3/src/imio/smartweb/policy/testing.py` & `imio.smartweb.policy-1.1.4/src/imio/smartweb/policy/testing.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.policy-1.1.3/src/imio/smartweb/policy/setuphandlers.py` & `imio.smartweb.policy-1.1.4/src/imio/smartweb/policy/setuphandlers.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.policy-1.1.3/src/imio/smartweb/policy/tests/robot/test_example.robot` & `imio.smartweb.policy-1.1.4/src/imio/smartweb/policy/tests/robot/test_example.robot`

 * *Files identical despite different names*

### Comparing `imio.smartweb.policy-1.1.3/src/imio/smartweb/policy/tests/test_setup.py` & `imio.smartweb.policy-1.1.4/src/imio/smartweb/policy/tests/test_setup.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.policy-1.1.3/src/imio/smartweb/policy/tests/test_robot.py` & `imio.smartweb.policy-1.1.4/src/imio/smartweb/policy/tests/test_robot.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.policy-1.1.3/src/imio/smartweb/policy/pattern_settings.py` & `imio.smartweb.policy-1.1.4/src/imio/smartweb/policy/pattern_settings.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.policy-1.1.3/src/imio/smartweb/policy/caching.zcml` & `imio.smartweb.policy-1.1.4/src/imio/smartweb/policy/caching.zcml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.policy-1.1.3/src/imio/smartweb/policy/caching.py` & `imio.smartweb.policy-1.1.4/src/imio/smartweb/policy/caching.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.policy-1.1.3/src/imio/smartweb/policy/setupdemo.py` & `imio.smartweb.policy-1.1.4/src/imio/smartweb/policy/setupdemo.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.policy-1.1.3/src/imio/smartweb/policy/profiles/multilingual/registry.xml` & `imio.smartweb.policy-1.1.4/src/imio/smartweb/policy/profiles/multilingual/registry.xml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.policy-1.1.3/src/imio/smartweb/policy/profiles/default/types/File.xml` & `imio.smartweb.policy-1.1.4/src/imio/smartweb/policy/profiles/default/types/File.xml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.policy-1.1.3/src/imio/smartweb/policy/profiles/default/controlpanel.xml` & `imio.smartweb.policy-1.1.4/src/imio/smartweb/policy/profiles/default/controlpanel.xml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.policy-1.1.3/src/imio/smartweb/policy/profiles/default/metadata.xml` & `imio.smartweb.policy-1.1.4/src/imio/smartweb/policy/profiles/default/metadata.xml`

 * *Files 1% similar despite different names*

#### Comparing `imio.smartweb.policy-1.1.3/src/imio/smartweb/policy/profiles/default/metadata.xml` & `imio.smartweb.policy-1.1.4/src/imio/smartweb/policy/profiles/default/metadata.xml`

```diff
@@ -1,10 +1,10 @@
 <?xml version="1.0" encoding="utf-8"?>
 <metadata>
-  <version>1029</version>
+  <version>1030</version>
   <dependencies>
     <dependency>profile-plone.app.contenttypes:plone-content</dependency>
     <dependency>profile-plone.app.caching:default</dependency>
     <dependency>profile-pas.plugins.imio:default</dependency>
     <dependency>profile-collective.autopublishing:default</dependency>
     <dependency>profile-collective.autoscaling:default</dependency>
     <dependency>profile-collective.messagesviewlet:default</dependency>
```

### Comparing `imio.smartweb.policy-1.1.3/src/imio/smartweb/policy/profiles/default/viewlets.xml` & `imio.smartweb.policy-1.1.4/src/imio/smartweb/policy/profiles/default/viewlets.xml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.policy-1.1.3/src/imio/smartweb/policy/profiles/default/rolemap.xml` & `imio.smartweb.policy-1.1.4/src/imio/smartweb/policy/upgrades/profiles/1020_to_1021/rolemap.xml`

 * *Files 2% similar despite different names*

#### Comparing `imio.smartweb.policy-1.1.3/src/imio/smartweb/policy/profiles/default/rolemap.xml` & `imio.smartweb.policy-1.1.4/src/imio/smartweb/policy/upgrades/profiles/1020_to_1021/rolemap.xml`

```diff
@@ -1,11 +1,10 @@
 <?xml version="1.0" encoding="utf-8"?>
 <rolemap>
   <permissions>
-    <permission name="Portlets: Manage portlets" acquire="False"/>
     <permission name="Plone Site Setup: Site" acquire="False">
       <role name="Manager"/>
     </permission>
     <permission name="Plone Site Setup: Mail" acquire="False">
       <role name="Manager"/>
     </permission>
     <permission name="Plone Site Setup: Language" acquire="False">
```

### Comparing `imio.smartweb.policy-1.1.3/src/imio/smartweb/policy/profiles/default/registry/autopublishing.xml` & `imio.smartweb.policy-1.1.4/src/imio/smartweb/policy/profiles/default/registry/autopublishing.xml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.policy-1.1.3/src/imio/smartweb/policy/profiles/default/registry/smartweb.xml` & `imio.smartweb.policy-1.1.4/src/imio/smartweb/policy/profiles/default/registry/smartweb.xml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.policy-1.1.3/src/imio/smartweb/policy/profiles/default/registry/caching.xml` & `imio.smartweb.policy-1.1.4/src/imio/smartweb/policy/profiles/default/registry/caching.xml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.policy-1.1.3/src/imio/smartweb/policy/profiles.zcml` & `imio.smartweb.policy-1.1.4/src/imio/smartweb/policy/profiles.zcml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.policy-1.1.3/src/imio/smartweb/policy/utils.py` & `imio.smartweb.policy-1.1.4/src/imio/smartweb/policy/utils.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.policy-1.1.3/src/imio/smartweb/policy/upgrades/profiles/1006_to_1007/registry/caching.xml` & `imio.smartweb.policy-1.1.4/src/imio/smartweb/policy/upgrades/profiles/1006_to_1007/registry/caching.xml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.policy-1.1.3/src/imio/smartweb/policy/upgrades/profiles/1011_to_1012/registry/collective.autoscaling.values.xml` & `imio.smartweb.policy-1.1.4/src/imio/smartweb/policy/upgrades/profiles/1011_to_1012/registry/collective.autoscaling.values.xml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.policy-1.1.3/src/imio/smartweb/policy/upgrades/profiles/1013_to_1014/registry/collective.autoscaling.values.xml` & `imio.smartweb.policy-1.1.4/src/imio/smartweb/policy/upgrades/profiles/1013_to_1014/registry/collective.autoscaling.values.xml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.policy-1.1.3/src/imio/smartweb/policy/upgrades/profiles/1021_to_1022/registry/caching.xml` & `imio.smartweb.policy-1.1.4/src/imio/smartweb/policy/upgrades/profiles/1021_to_1022/registry/caching.xml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.policy-1.1.3/src/imio/smartweb/policy/upgrades/profiles/1022_to_1023/registry/caching.xml` & `imio.smartweb.policy-1.1.4/src/imio/smartweb/policy/upgrades/profiles/1022_to_1023/registry/caching.xml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.policy-1.1.3/src/imio/smartweb/policy/upgrades/profiles/1020_to_1021/controlpanel.xml` & `imio.smartweb.policy-1.1.4/src/imio/smartweb/policy/upgrades/profiles/1020_to_1021/controlpanel.xml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.policy-1.1.3/src/imio/smartweb/policy/upgrades/profiles/1020_to_1021/rolemap.xml` & `imio.smartweb.policy-1.1.4/src/imio/smartweb/policy/profiles/default/rolemap.xml`

 * *Files 9% similar despite different names*

#### Comparing `imio.smartweb.policy-1.1.3/src/imio/smartweb/policy/upgrades/profiles/1020_to_1021/rolemap.xml` & `imio.smartweb.policy-1.1.4/src/imio/smartweb/policy/profiles/default/rolemap.xml`

```diff
@@ -1,10 +1,11 @@
 <?xml version="1.0" encoding="utf-8"?>
 <rolemap>
   <permissions>
+    <permission name="Portlets: Manage portlets" acquire="False"/>
     <permission name="Plone Site Setup: Site" acquire="False">
       <role name="Manager"/>
     </permission>
     <permission name="Plone Site Setup: Mail" acquire="False">
       <role name="Manager"/>
     </permission>
     <permission name="Plone Site Setup: Language" acquire="False">
@@ -42,9 +43,13 @@
     </permission>
     <permission name="Plone Site Setup: Filtering" acquire="False">
       <role name="Manager"/>
     </permission>
     <permission name="Smartweb: Manager-only configlets" acquire="False">
       <role name="Manager"/>
     </permission>
+    <permission name="Smartweb: Manage configlets" acquire="False">
+      <role name="Manager"/>
+      <role name="Site Administrator"/>
+    </permission>
   </permissions>
 </rolemap>
```

### Comparing `imio.smartweb.policy-1.1.3/src/imio/smartweb/policy/upgrades/profiles/1014_to_1015/registry/caching.xml` & `imio.smartweb.policy-1.1.4/src/imio/smartweb/policy/upgrades/profiles/1014_to_1015/registry/caching.xml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.policy-1.1.3/src/imio/smartweb/policy/upgrades/profiles/1026_to_1027/registry/autopublishing.xml` & `imio.smartweb.policy-1.1.4/src/imio/smartweb/policy/upgrades/profiles/1026_to_1027/registry/autopublishing.xml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.policy-1.1.3/src/imio/smartweb/policy/upgrades/upgrades.py` & `imio.smartweb.policy-1.1.4/src/imio/smartweb/policy/upgrades/upgrades.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.policy-1.1.3/src/imio/smartweb/policy/upgrades/configure.zcml` & `imio.smartweb.policy-1.1.4/src/imio/smartweb/policy/upgrades/configure.zcml`

 * *Files 2% similar despite different names*

```diff
@@ -119,14 +119,22 @@
       name="upgrade_1028_to_1029"
       title="Upgrade policy from 1028 to 1029"
       directory="profiles/1028_to_1029"
       description="Change collective.messagesviwlet control panel default values"
       provides="Products.GenericSetup.interfaces.EXTENSION"
       />
 
+  <genericsetup:registerProfile
+      name="upgrade_1029_to_1030"
+      title="Upgrade policy 1029 to 1030"
+      directory="profiles/1029_to_1030"
+      description="Add new permission to manage configlets in control panel"
+      provides="Products.GenericSetup.interfaces.EXTENSION"
+      />
+
   <genericsetup:upgradeStep
       title="Configure first official release"
       description="Install pas.plugins.imio and run needed profiles steps"
       source="1000"
       destination="1001"
       handler=".upgrades.configure_first_official_release"
       profile="imio.smartweb.policy:default"
@@ -437,8 +445,18 @@
     <genericsetup:upgradeDepends
         title="Change collective.messagesviwlet control panel default values"
         import_profile="imio.smartweb.policy.upgrades:upgrade_1028_to_1029"
         import_steps="plone.app.registry"
         />
   </genericsetup:upgradeSteps>
 
+  <genericsetup:upgradeSteps
+      source="1029"
+      destination="1030"
+      profile="imio.smartweb.policy:default">
+    <genericsetup:upgradeDepends
+        title="Add new permission to manage configlets in control panel"
+        import_profile="imio.smartweb.policy.upgrades:upgrade_1029_to_1030"
+        />
+  </genericsetup:upgradeSteps>
+
 </configure>
```

### Comparing `imio.smartweb.policy-1.1.3/src/imio/smartweb/policy/browser/faceted/subtyper.py` & `imio.smartweb.policy-1.1.4/src/imio/smartweb/policy/browser/faceted/subtyper.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.policy-1.1.3/src/imio/smartweb/policy/browser/faceted/configure.zcml` & `imio.smartweb.policy-1.1.4/src/imio/smartweb/policy/browser/faceted/configure.zcml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.policy-1.1.3/src/imio/smartweb/policy/browser/configure.zcml` & `imio.smartweb.policy-1.1.4/src/imio/smartweb/policy/browser/configure.zcml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.policy-1.1.3/src/imio/smartweb/policy/viewlets.zcml` & `imio.smartweb.policy-1.1.4/src/imio/smartweb/policy/viewlets.zcml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.policy-1.1.3/src/imio/smartweb/policy/configure.zcml` & `imio.smartweb.policy-1.1.4/src/imio/smartweb/policy/configure.zcml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.policy-1.1.3/src/imio.smartweb.policy.egg-info/requires.txt` & `imio.smartweb.policy-1.1.4/src/imio.smartweb.policy.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `imio.smartweb.policy-1.1.3/src/imio.smartweb.policy.egg-info/SOURCES.txt` & `imio.smartweb.policy-1.1.4/src/imio.smartweb.policy.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 CHANGES.rst
 CONTRIBUTORS.rst
 DEVELOP.rst
+LICENSE.GPL
 LICENSE.rst
 MANIFEST.in
 README.rst
 setup.cfg
 setup.py
 docs/conf.py
 docs/index.rst
@@ -78,8 +79,10 @@
 src/imio/smartweb/policy/upgrades/profiles/1019_to_1020/registry/caching.xml
 src/imio/smartweb/policy/upgrades/profiles/1020_to_1021/controlpanel.xml
 src/imio/smartweb/policy/upgrades/profiles/1020_to_1021/rolemap.xml
 src/imio/smartweb/policy/upgrades/profiles/1021_to_1022/registry/caching.xml
 src/imio/smartweb/policy/upgrades/profiles/1022_to_1023/registry/caching.xml
 src/imio/smartweb/policy/upgrades/profiles/1023_to_1024/registry/bundles.xml
 src/imio/smartweb/policy/upgrades/profiles/1026_to_1027/registry/autopublishing.xml
-src/imio/smartweb/policy/upgrades/profiles/1028_to_1029/registry/messagesviewlet.xml
+src/imio/smartweb/policy/upgrades/profiles/1028_to_1029/registry/messagesviewlet.xml
+src/imio/smartweb/policy/upgrades/profiles/1029_to_1030/controlpanel.xml
+src/imio/smartweb/policy/upgrades/profiles/1029_to_1030/rolemap.xml
```

